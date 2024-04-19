# Comparing `tmp/simplepw-0.2.2-py3-none-any.whl.zip` & `tmp/simplepw-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4932 bytes, number of entries: 8
+Zip file size: 5766 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-04 15:45 simplepw/__init__.py
--rw-rw-rw-  2.0 fat    10746 b- defN 24-Apr-05 12:16 simplepw/main.py
+-rw-rw-rw-  2.0 fat    13272 b- defN 24-Apr-19 21:08 simplepw/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-04 15:49 simplepw/methods.py
--rw-rw-rw-  2.0 fat     1285 b- defN 24-Apr-05 13:27 simplepw-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 13:27 simplepw-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 24-Apr-05 13:27 simplepw-0.2.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-05 13:27 simplepw-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      618 b- defN 24-Apr-05 13:27 simplepw-0.2.2.dist-info/RECORD
-8 files, 12793 bytes uncompressed, 3846 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat     1309 b- defN 24-Apr-19 21:14 simplepw-0.2.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 21:14 simplepw-0.2.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 24-Apr-19 21:14 simplepw-0.2.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-19 21:14 simplepw-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      618 b- defN 24-Apr-19 21:14 simplepw-0.2.3.dist-info/RECORD
+8 files, 15343 bytes uncompressed, 4680 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: simplepw/main.py
 Comment: 
 
 Filename: simplepw/methods.py
 Comment: 
 
-Filename: simplepw-0.2.2.dist-info/METADATA
+Filename: simplepw-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: simplepw-0.2.2.dist-info/WHEEL
+Filename: simplepw-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: simplepw-0.2.2.dist-info/entry_points.txt
+Filename: simplepw-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: simplepw-0.2.2.dist-info/top_level.txt
+Filename: simplepw-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: simplepw-0.2.2.dist-info/RECORD
+Filename: simplepw-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplepw/main.py

```diff
@@ -1,300 +1,383 @@
-import json
+import sqlite3
 import click
 import string
 import secrets
 import bcrypt
 from cryptography.fernet import Fernet
 from pathlib import Path
 import os
 
 
-config_dir_name = 'spw'
-if os.name == 'nt':  # Windows
-    CONFIG_DIR = Path(os.environ['APPDATA']) / config_dir_name
-else:
-    CONFIG_DIR = Path.home() / f".{config_dir_name}"
-
-CONFIG_KEY_FILE = CONFIG_DIR / 'pw.key'
-PASSWORD_STORE_FILE = CONFIG_DIR / 'data.json'
-MASTER_PASSWORD_FILE = CONFIG_DIR / 'master_password.hash'
+def get_config_dir():
+  """
+  Determines the appropriate configuration directory path based on the operating system.
+
+  Returns:
+    A pathlib.Path object representing the configuration directory path.
+  """
+  if os.name == 'nt':
+    return Path(os.environ['APPDATA']) / CONFIG_DIR_NAME
+  else:
+    return Path.home() / f".{CONFIG_DIR_NAME}"
+  
+# Define application constants
+CONFIG_DIR_NAME = 'spw'
+DATABASE_NAME = 'password_store.db'
+CONFIG_KEY_FILE = 'pw.key'
+MASTER_PASSWORD_FILE = Path(get_config_dir()) / 'master_password.hash'  # Use Path object
 
-def ensure_setup():
-    if not CONFIG_DIR.exists():
-        CONFIG_DIR.mkdir(parents=True, exist_ok=True)
 
-    if not CONFIG_KEY_FILE.exists():
-        key = Fernet.generate_key()
-        with open(CONFIG_KEY_FILE, 'wb') as key_file:
-            key_file.write(key)
+def ensure_setup():
+    """Creates necessary directories, files, and database setups for the application."""
+    config_dir = get_config_dir()
+    config_dir.mkdir(parents=True, exist_ok=True)
+    create_encryption_key(config_dir)
+    create_password_database(config_dir)
+    click.echo(f"Password manager setup complete. Data directory: {config_dir}")
+
+def get_database_connection():
+    """Return a connection to the database, ensuring it references the correct path."""
+    db_path = get_config_dir() / DATABASE_NAME
+    return sqlite3.connect(db_path)
+
+
+def create_encryption_key(config_dir):
+    """Creates an encryption key if it does not exist."""
+    key_file = config_dir / CONFIG_KEY_FILE
+    if not key_file.exists():
+        try:
+            with open(key_file, 'wb') as file:
+                file.write(Fernet.generate_key())
+        except IOError as e:
+            print(f"Failed to create key file: {e}")
+
+def create_password_database(config_dir):
+    """Creates the passwords table in the database if it does not exist."""
+    database_path = config_dir / DATABASE_NAME
+    try:
+        conn = sqlite3.connect(database_path)
+        c = conn.cursor()
+        c.execute("""
+            CREATE TABLE IF NOT EXISTS passwords (
+                id INTEGER PRIMARY KEY AUTOINCREMENT,
+                name TEXT NOT NULL,
+                encrypted_password TEXT NOT NULL
+            )
+        """)
+        conn.commit()
+    except sqlite3.Error as e:
+        print(f"Failed to create or connect to database: {e}")
+    finally:
+        conn.close()
+
+
+def create_database(database_path):
+  """Creates a new database with a 'passwords' table at the specified path.
+
+  Args:
+    database_path: The path to the database file.
+  """
+  conn = sqlite3.connect(database_path)  # Connect to the database
+  c = conn.cursor()
+
+  # Define default table name and schema
+  table_name = "passwords"
+  table_schema = {
+      "id": "INTEGER PRIMARY KEY AUTOINCREMENT",
+      "name": "TEXT NOT NULL",
+      "encrypted_password": "TEXT NOT NULL"  # Updated column name for clarity
+  }
+  # Build CREATE TABLE statement dynamically
+  columns = ", ".join([f"{col} {schema}" for col, schema in table_schema.items()])
+  sql = f"""CREATE TABLE IF NOT EXISTS {table_name} ({columns})"""
+
+  try:
+    c.execute(sql)
+    print(f"Database '{database_path}' created successfully.")
+  except sqlite3.Error as e:
+    print("Error creating table:", e)
 
+  conn.commit()  # Save changes
+  conn.close()
 
 def load_key():
-    return CONFIG_KEY_FILE.read_bytes()
+    """Loads the encryption key from the key file in the configuration directory."""
+    key_file_path = get_config_dir() / CONFIG_KEY_FILE
+    try:
+        with open(key_file_path, 'rb') as file:
+            return file.read()
+    except IOError as e:
+        print(f"Failed to read key file: {e}")
+        return None
 
 
 def encrypt_message(message, key):
-    return Fernet(key).encrypt(message.encode())
-
+    """Encrypt a message using the provided key."""
+    try:
+        f = Fernet(key)
+        return f.encrypt(message.encode())
+    except Exception as e:
+        print(f"Failed to encrypt message: {e}")
+        return None
 
 def decrypt_message(encrypted_message, key):
-    return Fernet(key).decrypt(encrypted_message).decode()
+    """Decrypt a message using the provided key."""
+    try:
+        f = Fernet(key)
+        return f.decrypt(encrypted_message).decode()
+    except Exception as e:
+        print(f"Failed to decrypt message: {e}")
+        return None
 
 
 def get_next_id():
-    try:
-        with open(PASSWORD_STORE_FILE, 'r') as file:
-            data = json.load(file)
-            return max(int(key) for key in data.keys()) + 1  # Find the highest ID and increment
-    except (FileNotFoundError, ValueError):
-        return 1  # Start with 1 if no saved passwords or invalid data
+    conn = sqlite3.connect('password_store.db')
+    c = conn.cursor()
+    c.execute('SELECT MAX(id) FROM passwords')
+    data = c.fetchone()
+    conn.close()
+
+    if data[0] is None:
+        return 1  # No entries yet, start with ID 1
+    else:
+        return data[0] + 1  # Return the highest ID + 1
+
 
 
 def generate_password(length):
     alphabet = string.ascii_letters + string.digits + string.punctuation
     return ''.join(secrets.choice(alphabet) for i in range(length))
 
 
 def set_master_password():
-    click.echo("It looks like you're running the Password Manager for the first time.")
-    show_tutorial()
-    password = click.prompt('Please set a master password for accessing this tool', hide_input=True, confirmation_prompt=True, type=str)
-    hashed = bcrypt.hashpw(password.encode(), bcrypt.gensalt())
-    with open(MASTER_PASSWORD_FILE, 'wb') as file:
-        file.write(hashed)
-    click.echo("Master password set successfully.")
+    """Sets the master password with proper error checking."""
+    password = click.prompt('Enter a new master password:', hide_input=True)
+    password_confirm = click.prompt('Confirm your new master password:', hide_input=True)
+    if password != password_confirm:
+        click.echo("Passwords do not match. Please try again.")
+        return False
+
+    try:
+        hashed_password = bcrypt.hashpw(password.encode(), bcrypt.gensalt())
+        with open(get_config_dir() / 'master_password.hash', 'wb') as file:
+            file.write(hashed_password)
+        click.echo("Master password set successfully.")
+        return True
+    except IOError as e:
+        click.echo(f"Failed to write master password: {e}")
+        return False
 
 
 def verify_master_password():
+    """Verifies the master password entered by the user."""
     try:
-        stored_hash = MASTER_PASSWORD_FILE.read_bytes()
-        password = click.prompt('Enter your master password to unlock the tool', hide_input=True, type=str)
-        if bcrypt.checkpw(password.encode(), stored_hash):
-            click.echo("Password verified successfully. Access granted.")
-            return True
-        else:
-            click.echo("Incorrect password. Access denied.")
-            return False
+        with open(get_config_dir() / 'master_password.hash', 'rb') as file:
+            stored_hash = file.read()
     except FileNotFoundError:
-        click.echo("Master password not set. Setting up now.")
-        set_master_password()
-        return True
+        click.echo("Master password not found. Please set a master password first.")
+        return False
 
+    password = click.prompt('Enter your master password:', hide_input=True)
+    if bcrypt.checkpw(password.encode(), stored_hash):
+        click.echo("Password verified successfully.")
+        return True
+    else:
+        click.echo("Incorrect password. Please try again.")
+        return False
 
 def save_password(name, password):
+    """Saves the named password into the database after encrypting both name and password."""
+    ensure_setup()  # Ensure setup is complete which includes database configuration
     key = load_key()
+    if key is None:
+        click.echo("Encryption key is missing. Cannot secure the name and password.")
+        return
+
+    encrypted_name = encrypt_message(name, key)
+    if encrypted_name is None:
+        click.echo("Failed to encrypt the name.")
+        return
+
     encrypted_password = encrypt_message(password, key)
-    entry_id = get_next_id()
+    if encrypted_password is None:
+        click.echo("Failed to encrypt the password.")
+        return
+
     try:
-        with open(PASSWORD_STORE_FILE, 'r+') as file:
-            data = json.load(file)
-            data[entry_id] = {"name": name, "password": encrypted_password.hex()}
-            file.seek(0)
-            file.truncate()
-            json.dump(data, file)
-    except FileNotFoundError:
-        with open(PASSWORD_STORE_FILE, 'w') as file:
-            json.dump({entry_id: {"name": name, "password": encrypted_password.hex()}}, file)
+        conn = get_database_connection()
+        cursor = conn.cursor()
+        cursor.execute("INSERT INTO passwords (name, encrypted_password) VALUES (?, ?)", (encrypted_name.hex(), encrypted_password.hex()))
+        conn.commit()
+        click.echo(f"Data for '{name}' added successfully.")
+    except sqlite3.Error as e:
+        click.echo(f"Failed to save data: {e}")
+    finally:
+        if conn:
+            conn.close()
 
 
 def delete_password(entry_id):
-    key = load_key()
+    """Deletes a password entry based on its ID from the database."""
+    conn = get_database_connection()
+    c = conn.cursor()
     try:
-        data = json.loads(PASSWORD_STORE_FILE.read_text())
-        if entry_id in data:
-            entry = data[entry_id]
-            decrypted_pass = decrypt_message(bytes.fromhex(entry["password"]), key)
-            confirmation = click.confirm(f"Are you sure you want to delete the password for '{entry['name']}'?",
-                                         default=False)
-            if confirmation:
-                del data[entry_id]
-                PASSWORD_STORE_FILE.write_text(json.dumps(data))
-                click.echo("Password deleted successfully.")
-            else:
-                click.echo("Deletion cancelled.")
-        else:
-            click.echo("No matching ID found.")
-    except FileNotFoundError:
-        click.echo("No saved passwords found.")
+        # Check if the entry exists
+        c.execute("SELECT id FROM passwords WHERE id = ?", (entry_id,))
+        if c.fetchone() is None:
+            click.echo("No password found with the provided ID.")
+            return
+    
+        # If the entry exists, proceed with deletion
+        c.execute("DELETE FROM passwords WHERE id = ?", (entry_id,))
+        conn.commit()
+        click.echo("Password deleted successfully.")
+    except sqlite3.Error as e:
+        click.echo(f"Failed to delete password: {e}")
+    finally:
+        conn.close()
 
 
 def delete_all_passwords():
-    confirmation = click.confirm("Are you sure you want to delete ALL saved passwords? This action cannot be undone.",
-                                 default=False)
+    """Deletes all password entries from the database after confirmation."""
+    # Confirm the user wants to delete all passwords
+    confirmation = click.confirm("Are you sure you want to delete ALL saved passwords? This action cannot be undone.", default=False)
     if confirmation:
         try:
-            PASSWORD_STORE_FILE.unlink()
+            conn = get_database_connection()
+            c = conn.cursor()
+            c.execute("DELETE FROM passwords")
+            conn.commit()
             click.echo("All passwords have been successfully deleted.")
-        except FileNotFoundError:
-            click.echo("No saved passwords found.")
+        except sqlite3.Error as e:
+            click.echo(f"Database error: {e}")
+        finally:
+            conn.close()
     else:
         click.echo("Deletion cancelled.")
 
 
 def display_saved_passwords():
+    """Displays all saved passwords within the database with decrypted forms."""
     key = load_key()
+    if not key:
+        click.echo("Failed to load the encryption key.")
+        return
+
     try:
-        data = json.loads(PASSWORD_STORE_FILE.read_text())
-        if data:
-            print(f"{'ID':<40} | {'Name':<20} | {'Password':<20}")
-            print("-" * 80)
-            for entry_id, details in data.items():
-                decrypted_pass = decrypt_message(bytes.fromhex(details["password"]), key)
-                print(f"{entry_id:<40} | {details['name']:<20} | {decrypted_pass:<20}")
-        else:
-            click.echo("No saved passwords found.")
-    except FileNotFoundError:
-        click.echo("No password file found.")
+        conn = get_database_connection()
+        c = conn.cursor()
+        c.execute('SELECT id, name, encrypted_password FROM passwords')
+        passwords = c.fetchall()
+    except sqlite3.Error as e:
+        click.echo(f"Database error when trying to retrieve passwords: {e}")
+        return
+    finally:
+        if conn:
+            conn.close()
 
+    if not passwords:
+        click.echo("No saved passwords found.")
+        return
 
-def add_existing_password():
-    """Prompts the user for an existing password's name and password, encrypts it, and saves it to the password store."""
+    # Display header
+    click.echo("{:<5} | {:<20} | {:<30}".format("ID", "Name", "Password"))
+    click.echo("-" * 60)
+
+    # Loop through each password record
+    for entry_id, encrypted_name_hex, encrypted_pass_hex in passwords:
+        decrypted_name = decrypt_message(bytes.fromhex(encrypted_name_hex), key)
+        decrypted_pass = decrypt_message(bytes.fromhex(encrypted_pass_hex), key)
+        
+        if decrypted_name is None:
+            decrypted_name = "Error decrypting name"
+        if decrypted_pass is None:
+            decrypted_pass = "Error decrypting password"
+            
+        click.echo("{:<5} | {:<20} | {:<30}".format(entry_id, decrypted_name, decrypted_pass))
 
-    key = load_key()  # Load the encryption key
 
+def add_existing_password():
+    """Prompts the user for an existing password's name and password, then saves it to the password store using the save_password function."""
     name = click.prompt('Please enter the name for the password', type=str)
     password = click.prompt('Please enter the password', hide_input=True, type=str)
 
-    encrypted_password = encrypt_message(password, key)  # Encrypt the password
-    entry_id = get_next_id()  # Generate a unique ID
+    save_password(name, password)
 
-    try:
-        with open(PASSWORD_STORE_FILE, 'r+') as file:
-            data = json.load(file)
-            data[entry_id] = {"name": name, "password": encrypted_password.hex()}
-            file.seek(0)
-            file.truncate()
-            json.dump(data, file)
-    except FileNotFoundError:
-        with open(PASSWORD_STORE_FILE, 'w') as file:
-            json.dump({entry_id: {"name": name, "password": encrypted_password.hex()}}, file)
-
-    click.echo(f"Password '{name}' added successfully.")
-
-def show_tutorial():
-    tutorial_text = """
-Welcome to the Password Manager Tutorial!
-
-Important Notice: This password generator and password safe are provided "as is" without warranty of any kind. 
-While designed with security in mind, the developer cannot guarantee its effectiveness for real-world use. 
-It is strongly recommended to exercise caution and consider the potential risks before using this tool for sensitive information.
-
-Enjoy using Password Manager!
-"""
-    click.echo(tutorial_text)
-
-def interactive_mode():
+def main_menu():
     click.clear()
-    click.echo("Welcome to Password Manager")
-
-    if not verify_master_password():
-        click.echo("Master password verification failed. Exiting interactive mode.")
-        return
-
     while True:
-        click.echo("\n1. Add Passwords")
+        click.echo("\nMain Menu:")
+        click.echo("1. Add Password")
         click.echo("2. Manage Saved Passwords")
         click.echo("3. Exit")
-        choice = click.prompt("\nPlease enter your choice", type=int)
+        choice = click.prompt("Please enter your choice", type=int)
 
         if choice == 1:
             add_password_menu()
         elif choice == 2:
-            manage_password_menu()
+            manage_passwords_menu()
         elif choice == 3:
-            click.echo("\nExiting interactive mode. Goodbye!")
+            click.echo("Exiting.")
             break
         else:
-            click.echo("\nInvalid choice. Please try again.")
-
-        click.pause(info='\nPress any key to continue...')
-
+            click.echo("Invalid selection. Please try again.")
 
 def add_password_menu():
-    click.clear()
-    click.echo("\nAdd Password")
-    click.echo("1. Generate and Save a Password")
-    click.echo("2. Add Existing Password")
-    click.echo("3. Exit.")
-    choice = click.prompt("\nPlease enter your choice", type=int)
-
-    if choice == 1:
-        length = click.prompt('\nPlease enter a password length', default=24, type=int)
-        name = click.prompt('Please enter a name for the password', type=str)
-        password = generate_password(length)
-        save_password(name, password)
-        click.echo(f'Generated and saved password: {password}\n')
-    elif choice == 2:
-        add_existing_password()
-    elif choice == 3:  
-        return
-    else:
-        click.echo("\nInvalid choice. Please try again.")
-
+    while True:
+        click.echo("\nAdd Password Menu:")
+        click.echo("1. Generate and Save a New Password")
+        click.echo("2. Add an Existing Password")
+        click.echo("3. Back to Main Menu")
+        choice = click.prompt("Please enter your choice", type=int)
 
-def manage_password_menu():
-    click.clear()
-    click.echo("\nManage Saved Passwords")
-    key = load_key()
-    try:
-        data = json.loads(PASSWORD_STORE_FILE.read_text())
-        if data:
-            print(f"{'ID':<40} | {'Name':<20} | {'Password':<20}")
-            print("-" * 80)
-            for entry_id, details in data.items():
-                decrypted_pass = decrypt_message(bytes.fromhex(details["password"]), key)
-                print(f"{entry_id:<40} | {details['name']:<20} | {decrypted_pass:<20}")
+        if choice == 1:
+            length = click.prompt('Enter the desired password length', default=24, type=int)
+            name = click.prompt('Enter a name for this password', type=str)
+            password = generate_password(length)
+            save_password(name, password)
+            click.echo(f"Generated and saved password: {password}")
+        elif choice == 2:
+            add_existing_password()
+        elif choice == 3:
+            click.clear()
+            return
         else:
-            click.echo("No saved passwords found.")
-    except FileNotFoundError:
-        click.echo("No saved passwords found.")
+            click.echo("Invalid selection. Please try again.")
 
-    click.echo("\n1. Delete a Password")
-    click.echo("2. Delete All Saved Passwords")
-    click.echo("3. Exit.")
-    choice = click.prompt("\nPlease enter your choice", type=int)
-
-    if choice == 1:
-        entry_id = click.prompt('\nPlease enter the ID of the password to delete', type=str)
-        delete_password(entry_id)
-    elif choice == 2:
-        delete_all_passwords()
-    elif choice == 3:
-        return
-    else:
-        click.echo("\nInvalid choice. Please try again.")
+
+def manage_passwords_menu():
+    display_saved_passwords()
+    while True:
+        click.echo("\nManage Saved Passwords Menu:")
+        click.echo("1. Delete a Specific Password")
+        click.echo("2. Delete All Passwords")
+        click.echo("3. Back to Main Menu")
+        choice = click.prompt("Please enter your choice", type=int)
+        if choice == 1:
+            entry_id = click.prompt('Enter the ID of the password to delete', type=int)
+            delete_password(entry_id)
+        elif choice == 2:
+            delete_all_passwords()
+        elif choice == 3:
+            click.clear()
+            return
+        else:
+            click.echo("Invalid selection. Please try again.")
 
 
 @click.command()
-@click.option('--length', default=24, help='Password length')
-@click.option('--save', is_flag=True, help='Save the generated password')
-@click.option('--list', is_flag=True, help='List all saved passwords')
-@click.option('--delete', type=str, help='Delete a password by its ID')
-@click.option('--generate', is_flag=True, help='Generate a password without saving')
-
-def main(length, save, list, delete, generate):
+@click.option('--length', default=24, help='Password length', required=False)
+def main(length):
+    click.echo("Welcome to Password Manager")
     ensure_setup()
 
-    if generate and not (save or list or delete):
-        password = generate_password(length)
-        click.echo(f'Generated password: {password}')
-        return
-
-    if save or list or delete:
-        if not verify_master_password():
+    if not MASTER_PASSWORD_FILE.exists() or not verify_master_password():
+        click.echo("Setting or verifying master password...")
+        if not set_master_password() and not verify_master_password():
+            click.echo("Failed to set or verify master password. Exiting.")
             return
-    if list:
-        display_saved_passwords()
-    elif delete:
-        delete_password(delete)
-    elif save:
-        password = generate_password(length)
-        click.echo(f'Generated password: {password}')
-        name = click.prompt('Please enter a name for the password', type=str)
-        save_password(name, password)
-        click.echo("Password saved successfully.")
-    else:
-        interactive_mode()
 
+    main_menu()
 
 if __name__ == '__main__':
-    main()
+    main()
```

## Comparing `simplepw-0.2.2.dist-info/METADATA` & `simplepw-0.2.3.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: simplepw
-Version: 0.2.2
+Version: 0.2.3
 Summary: A CLI Application for generating and managing passwords
 Author: pajhe
 Author-email: piejeys@proton.me
 Keywords: password generation
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography >=2.8
 Requires-Dist: click
 Requires-Dist: bcrypt
 Requires-Dist: pathlib
+Requires-Dist: sqlite3
 
 # SimplePW
 
 This password manager is a project designed for educational purposes to explore concepts of password security and encryption. While it utilizes encryption to protect your data, it is important to understand that it is not suitable for storing highly sensitive information in real-world scenarios.
 
 ## Installation
```

## Comparing `simplepw-0.2.2.dist-info/RECORD` & `simplepw-0.2.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 simplepw/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-simplepw/main.py,sha256=byRuMPAmrTcWBERFK_-yTTMyIBYQPE32tEzau6QJJkA,10746
+simplepw/main.py,sha256=slA_iGapQlDLeHdJfLZfDcb6RxwrZEtvotkXIq77TmE,13272
 simplepw/methods.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-simplepw-0.2.2.dist-info/METADATA,sha256=e7yO-cTUwBgETQuN89adCjS6X1QUpzrDLkEv5PVPLW8,1285
-simplepw-0.2.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-simplepw-0.2.2.dist-info/entry_points.txt,sha256=ITIw-nSN7wx7rDLBqsqrvi9tzctXCqzylhuLBCYpE9w,43
-simplepw-0.2.2.dist-info/top_level.txt,sha256=dj2pVaVkTqCV_uraTi_KDzGTC1-4WL9oPqZZqmYJ5-w,9
-simplepw-0.2.2.dist-info/RECORD,,
+simplepw-0.2.3.dist-info/METADATA,sha256=NJxwuWPYx9Y72fLbTmG3mj0YMCTV9DoOp2DUhXZHFvM,1309
+simplepw-0.2.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+simplepw-0.2.3.dist-info/entry_points.txt,sha256=ITIw-nSN7wx7rDLBqsqrvi9tzctXCqzylhuLBCYpE9w,43
+simplepw-0.2.3.dist-info/top_level.txt,sha256=dj2pVaVkTqCV_uraTi_KDzGTC1-4WL9oPqZZqmYJ5-w,9
+simplepw-0.2.3.dist-info/RECORD,,
```

