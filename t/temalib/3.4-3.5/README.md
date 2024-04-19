# Comparing `tmp/temalib-3.4.tar.gz` & `tmp/temalib-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temalib-3.4.tar", last modified: Sat Mar  9 07:29:05 2024, max compression
+gzip compressed data, was "temalib-3.5.tar", last modified: Fri Apr 19 17:13:35 2024, max compression
```

## Comparing `temalib-3.4.tar` & `temalib-3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 07:29:05.317476 temalib-3.4/
--rw-rw-rw-   0        0        0     1716 2024-03-09 07:04:50.000000 temalib-3.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1061 2024-01-25 13:27:43.000000 temalib-3.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2024-01-25 13:25:38.000000 temalib-3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      600 2024-03-09 07:29:05.316479 temalib-3.4/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-01-25 13:23:18.000000 temalib-3.4/README.txt
--rw-rw-rw-   0        0        0       42 2024-03-09 07:29:05.318947 temalib-3.4/setup.cfg
--rw-rw-rw-   0        0        0      697 2024-03-09 07:28:37.000000 temalib-3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-09 07:29:05.295566 temalib-3.4/temalib/
--rw-rw-rw-   0        0        0     8633 2024-03-09 07:28:33.000000 temalib-3.4/temalib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 07:29:05.315074 temalib-3.4/temalib.egg-info/
--rw-rw-rw-   0        0        0      600 2024-03-09 07:29:05.000000 temalib-3.4/temalib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-03-09 07:29:05.000000 temalib-3.4/temalib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 07:29:05.000000 temalib-3.4/temalib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-09 07:29:05.000000 temalib-3.4/temalib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 17:13:35.424825 temalib-3.5/
+-rw-rw-rw-   0        0        0     1833 2024-04-19 17:12:43.000000 temalib-3.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1061 2024-01-25 13:27:43.000000 temalib-3.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2024-01-25 13:25:38.000000 temalib-3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      600 2024-04-19 17:13:35.424825 temalib-3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-01-25 13:23:18.000000 temalib-3.5/README.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 17:13:35.424825 temalib-3.5/setup.cfg
+-rw-rw-rw-   0        0        0      697 2024-04-19 17:12:57.000000 temalib-3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:13:35.414803 temalib-3.5/temalib/
+-rw-rw-rw-   0        0        0     7407 2024-04-19 17:12:23.000000 temalib-3.5/temalib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:13:35.422831 temalib-3.5/temalib.egg-info/
+-rw-rw-rw-   0        0        0      600 2024-04-19 17:13:35.000000 temalib-3.5/temalib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-04-19 17:13:35.000000 temalib-3.5/temalib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 17:13:35.000000 temalib-3.5/temalib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-19 17:13:35.000000 temalib-3.5/temalib.egg-info/top_level.txt
```

### Comparing `temalib-3.4/CHANGELOG.txt` & `temalib-3.5/CHANGELOG.txt`

 * *Files 13% similar despite different names*

```diff
@@ -55,8 +55,14 @@
 version 3.2.0 (08.03.2024)
 - update functions description
 
 version 3.2.1 (08.03.2024)
 - fix spaces for functions descriptions
 
 version 3.3-3.3.1 (09.03.2024)
-- fix add_line
+- fix add_line
+
+version 3.4 (09.03.2024)
+- fix remove_line
+
+version 3.5 (19.04.2024)
+- removed is_online because its a bushes
```

### Comparing `temalib-3.4/LICENSE.txt` & `temalib-3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temalib-3.4/PKG-INFO` & `temalib-3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temalib
-Version: 3.4
+Version: 3.5
 Summary: a library that was made for some ammeter bullshuy
 Home-page: 
 Author: tema5002
 Author-email: xtema5002x@gmail.com
 License: MIT
 Keywords: bullshuy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `temalib-3.4/setup.py` & `temalib-3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "Operating System :: Microsoft :: Windows :: Windows 11",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3"
 ]
  
 setup(
     name="temalib",
-    version="3.4",
+    version="3.5",
     description="a library that was made for some ammeter bullshuy",
     long_description=open("README.txt").read(),
     url="",
     author="tema5002",
     author_email="xtema5002x@gmail.com",
     license="MIT",
     classifiers=classifiers,
```

### Comparing `temalib-3.4/temalib/__init__.py` & `temalib-3.5/temalib/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,56 +3,20 @@
 from typing import Any
 
 """
 a library that was made for working with files
 """
 
 __author__ = "tema5002 <tema5002@gmail.com>"
-__version__ = "3.4"
+__version__ = "3.5"
 __license__ = "MIT"
 __copyright__ = "2024, tema5002"
 __short_description__ = "a library that works with files i guess"
 
 
-def is_online(guild, user_id: int) -> bool:
-    """
-Checks a guild member's online status across Discord.py libraries (discord.py, nextcord, or disnake).
-
-This function determines if a member is online (including idle),
-and returns False if the member is offline or not found within the guild.
-
-Parameters:
-
-- guild: The guild object to check for the member's presence.
-- user_id (int): The Discord user ID of the member to check.
-
-Returns:
-
-- bool: True if the member is online (not offline), False otherwise.
-
-Raises:
-
-- ModuleNotFoundError: If none of the supported Discord.py libraries (discord.py, nextcord, disnake) are found.
-    """
-    try:
-        import discord
-    except ModuleNotFoundError:
-        try:
-            import nextcord as discord
-        except ModuleNotFoundError:
-            try:
-                import disnake as discord
-            except ModuleNotFoundError:
-                raise ModuleNotFoundError("Neither discord or nextcord or disnake modules was found") from err
-
-    if member := guild.get_member(user_id):
-        return member.status != discord.Status.offline
-    return False
-
-
 def smthfile(fp: str, mode: str) -> codecs.StreamReaderWriter:
     """
 Opens a text file with UTF-8 encoding at the specified path (fp) with specified opening mode (mode)
 
 Keyword arguments:
 - fp (str): The filepath of the text file to open.
 - mode (str): The opening mode for the file.
@@ -84,41 +48,41 @@
 def get_folder_path(
         caller: str,
         *args: Any,
         # this is probably a bad idea to allow using anything but whatever
         create_folders: bool = True
 ) -> str:
     """
-    Construct a folder path relative to the caller's directory, optionally creating missing folders.
+Construct a folder path relative to the caller's directory, optionally creating missing folders.
 
-    This function builds a filepath by combining:
-    - The directory of the caller file (caller)
-    - Additional subfolders specified as positional arguments (args)
+This function builds a filepath by combining:
+- The directory of the caller file (caller)
+- Additional subfolders specified as positional arguments (args)
 
-    Parameters:
+Parameters:
 
-    - caller (str): The path of the caller file (usually __file__).
-    - *args (Any): One or more subfolder names to be added to the path.
-      (args will be converted to str but i don't recommend putting anything except str and int)
-    - create_folders (bool, optional): Whether to create missing folders in the path. (True by default)
+- caller (str): The path of the caller file (usually __file__).
+- *args (Any): One or more subfolder names to be added to the path.
+  (args will be converted to str but i don't recommend putting anything except str and int)
+- create_folders (bool, optional): Whether to create missing folders in the path. (True by default)
 
-    Returns:
+Returns:
 
-    - str: The constructed folder path.
+- str: The constructed folder path.
 
-    Raises:
+Raises:
 
-    - OSError: If there are errors creating folders (e.g., permission issues).
+- OSError: If there are errors creating folders (e.g., permission issues).
 
-    Example Usage:
+Example Usage:
 
-    folder_path = get_folder_path(__file__, "data", "results")
+folder_path = get_folder_path(__file__, "data", "results")
 
-    print(folder_path)
-    # Output: C:\\path\\to\\__file__\\data\\results
+print(folder_path)
+# Output: C:\\path\\to\\__file__\\data\\results
     """
     args = list(map(str, args))
 
     folder_dir = os.path.dirname(caller)
     for f in args:
         folder_dir = os.path.join(folder_dir, f)
         if create_folders and not os.path.exists(folder_dir):
```

### Comparing `temalib-3.4/temalib.egg-info/PKG-INFO` & `temalib-3.5/temalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temalib
-Version: 3.4
+Version: 3.5
 Summary: a library that was made for some ammeter bullshuy
 Home-page: 
 Author: tema5002
 Author-email: xtema5002x@gmail.com
 License: MIT
 Keywords: bullshuy
 Classifier: Development Status :: 5 - Production/Stable
```

