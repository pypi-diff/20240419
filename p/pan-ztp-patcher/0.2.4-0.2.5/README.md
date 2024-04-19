# Comparing `tmp/pan_ztp_patcher-0.2.4.tar.gz` & `tmp/pan_ztp_patcher-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_ztp_patcher-0.2.4.tar", max compression
+gzip compressed data, was "pan_ztp_patcher-0.2.5.tar", max compression
```

## Comparing `pan_ztp_patcher-0.2.4.tar` & `pan_ztp_patcher-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3906 2024-04-14 12:44:04.130157 pan_ztp_patcher-0.2.4/README.md
--rw-r--r--   0        0        0     5000 2024-04-17 21:05:25.214408 pan_ztp_patcher-0.2.4/pan_ztp_patcher/app.py
--rw-r--r--   0        0        0     1041 2024-04-16 12:06:48.369908 pan_ztp_patcher-0.2.4/pan_ztp_patcher/utils.py
--rw-r--r--   0        0        0    23839 2024-04-17 21:46:22.371705 pan_ztp_patcher-0.2.4/pan_ztp_patcher/ztp_patcher.py
--rw-r--r--   0        0        0      510 2024-04-17 21:46:31.058308 pan_ztp_patcher-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3912 2024-04-18 13:56:24.765685 pan_ztp_patcher-0.2.5/README.md
+-rw-r--r--   0        0        0    13707 2024-04-19 10:27:15.254371 pan_ztp_patcher-0.2.5/pan_ztp_patcher/app.py
+-rw-r--r--   0        0        0     1026 2024-04-18 15:55:37.498096 pan_ztp_patcher-0.2.5/pan_ztp_patcher/utils.py
+-rw-r--r--   0        0        0    37113 2024-04-19 10:35:42.142804 pan_ztp_patcher-0.2.5/pan_ztp_patcher/ztp_patcher.py
+-rw-r--r--   0        0        0      541 2024-04-19 11:01:49.890448 pan_ztp_patcher-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4650 1970-01-01 00:00:00.000000 pan_ztp_patcher-0.2.5/PKG-INFO
```

### Comparing `pan_ztp_patcher-0.2.4/README.md` & `pan_ztp_patcher-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 ```
 
 ## Usage
 
 To use the PAN-OS ZTP Patcher, run the following command:
 
 ```bash
-ztp_patcher --hostname <hostname> --username <username> --old-password <old_password> --new-password <new_password> [--pi-hostname <pi_hostname>] [--pi-content-path <pi_content_path>] [--content-file <content_file>]
+ztp_patcher --hostname <hostname> --username <username> --old-password <old_password> --new-password <new_password> [--pi-hostname <pi_hostname>] [--pi-content-path <pi_content_path>] [--content-file <content_version>]
 ```
 
 - `<hostname>`: The hostname or IP address of the PAN-OS firewall.
 - `<username>`: The username for accessing the PAN-OS firewall.
 - `<old_password>`: The current password for the specified user on the PAN-OS firewall.
 - `<new_password>`: The new password to be set for the specified user on the PAN-OS firewall.
 - `<pi_hostname>` (optional): The hostname or IP address of the Raspberry Pi Zero appliance (default: 192.168.1.2).
 - `<pi_content_path>` (optional): The path on the Raspberry Pi Zero where the content file is located (default: /var/tmp/).
-- `<content_file>` (optional): The name of the content file to be installed on the PAN-OS firewall (default: panupv2-all-contents-8834-8684).
+- `<content_version>` (optional): The name of the content file to be installed on the PAN-OS firewall (default: panupv2-all-contents-8834-8684).
 
 Example:
 
 ```bash
 ztp_patcher --hostname 192.168.1.1 --username admin --old-password admin --new-password PaloAlto123!
 ```
```

### Comparing `pan_ztp_patcher-0.2.4/pan_ztp_patcher/utils.py` & `pan_ztp_patcher-0.2.5/pan_ztp_patcher/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 import logging
 from logging.handlers import RotatingFileHandler
 
 
 def setup_logging():
     """
-    Configures the packages logging.
+    Configures the logging for the package.
 
-    Args: None
+    Args:
+        None
 
     Returns:
-        logger: A logging object.
+        logging.Logger: A logging object.
 
-    Raises: None
-
-    Example:
-        logger = setup_logging()
+    Raises:
+        None
     """
+
     logger = logging.getLogger()
     logger.setLevel(logging.DEBUG)
 
     # Configure file handler for debug level
     file_handler = RotatingFileHandler(
         "debug.log", maxBytes=5 * 1024 * 1024, backupCount=10
     )
```

### Comparing `pan_ztp_patcher-0.2.4/pan_ztp_patcher/ztp_patcher.py` & `pan_ztp_patcher-0.2.5/pan_ztp_patcher/ztp_patcher.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,308 +1,257 @@
 import logging
 import paramiko
-import sys
 import time
 import urllib.request
 import xml.etree.ElementTree as ET
 
+from typing import Optional
+
 logger = logging.getLogger(__name__)
 
 
 def change_firewall_password(
-    pan_hostname,
-    pan_username,
-    pan_password,
-    pan_password_default,
-):
+    pan_hostname: str,
+    pan_password_new: str,
+    pan_password_old: str,
+    pan_username: str,
+) -> bool:
     """
     Changes the password of a user on the PAN-OS firewall.
 
     Args:
         pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
         pan_username (str): The username for authentication.
-        pan_password (str): The new password to set for the user.
-        pan_password_default (str): The current password of the user.
+        pan_password_new (str): The new password to set for the user.
+        pan_password_old (str): The current password of the user.
 
     Returns:
-        None
+        bool: True if the password change is successful, False otherwise.
 
     Raises:
         paramiko.AuthenticationException: If authentication fails.
         paramiko.SSHException: If an SSH exception occurs.
-        Exception: If any other error occurs during the password change process. # noqa: E501
-
-    Example:
-        change_firewall_password("192.168.1.1", "admin", "pan_password_default", "pan_password")
+        Exception: If any other error occurs during the password change process.
     """
 
     logger.info("=" * 79)
     logger.info("Changing firewall password...")
     logger.info("=" * 79)
 
     # Create an SSH client
     client = paramiko.SSHClient()
     client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     try:
         # Connect to the firewall
         logger.debug("Connecting to {}...".format(pan_hostname))
         client.connect(
-            pan_hostname, username=pan_username, password=pan_password_default
+            hostname=pan_hostname,
+            username=pan_username,
+            password=pan_password_old,
         )
         logger.info("Connected to {} successfully.".format(pan_hostname))
 
         # Create an interactive shell
         shell = client.invoke_shell()
 
         # Wait for the prompt
         logger.debug("Waiting for the prompt...")
         time.sleep(3)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Send the old password
-        logger.debug(
-            "Sending pan_password_default: {}".format(pan_password_default)
-        )  # noqa: E501
-        shell.send(pan_password_default + "\n")
+        logger.debug("Sending pan_password_old: {}".format(pan_password_old))
+        shell.send(pan_password_old + "\n")
         time.sleep(3)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Send the new password
-        logger.debug("Sending pan_password: {}".format(pan_password))
-        shell.send(pan_password + "\n")
+        logger.debug("Sending pan_password_new: {}".format(pan_password_new))
+        shell.send(pan_password_new + "\n")
         time.sleep(3)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Confirm the new password
-        logger.debug("Confirming pan_password: {}".format(pan_password))
-        shell.send(pan_password + "\n")
+        logger.debug("Confirming pan_password_new: {}".format(pan_password_new))
+        shell.send(pan_password_new + "\n")
         time.sleep(3)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Close the SSH connection
         logger.debug("Closing the SSH connection...")
         client.close()
         logger.info("Password changed successfully.")
+        return True
 
     except paramiko.AuthenticationException:
         logger.error("Authentication failed. Please check your credentials.")
+        return False
+
     except paramiko.SSHException as ssh_exception:
         logger.error("SSH exception occurred: {}".format(str(ssh_exception)))
-    except Exception as e:
-        logger.error("An error occurred: {}".format(str(e)))
-
-
-def retrieve_api_key(
-    pan_hostname,
-    pan_username,
-    pan_password,
-):
-    """
-    Retrieves the API key from the PAN-OS firewall.
-
-    Args:
-        pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
-        pan_username (str): The username for authentication.
-        pan_password (str): The password for authentication.
-
-    Returns:
-        str: The API key if successfully retrieved, None otherwise.
-
-    Raises:
-        urllib.error.URLError: If a URL error occurs during the API request.
-        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response. # noqa: E501
-        Exception: If any other error occurs during the API request.
-
-    Example:
-        api_key = retrieve_api_key("192.168.1.1", "admin", "password")
-    """
-
-    logger.info("=" * 79)
-    logger.info("Retrieving API key...")
-    logger.info("=" * 79)
-
-    try:
-        # Construct the API URL
-        url = "https://{}/api/?type=keygen&user={}&password={}".format(
-            pan_hostname, pan_username, urllib.parse.quote(pan_password)
-        )
-        logger.debug("API URL: {}".format(url))
-
-        # Create an HTTPS request with SSL verification disabled
-        logger.debug("Retrieving API key...")
-        request = urllib.request.Request(url)
-        response = urllib.request.urlopen(
-            request, context=urllib.request.ssl._create_unverified_context()
-        )
-        logger.debug("Received response: {}".format(response))
-
-        # Read the response content
-        logger.debug("Reading response content...")
-        response_content = response.read().decode("utf-8")
-        logger.debug("Received response: {}".format(response_content))
+        return False
 
-        # Parse the XML response
-        logger.debug("Parsing XML response...")
-        root = ET.fromstring(response_content)
-        logger.debug("Root element: {}".format(root.tag))
-
-        # Extract the API key from the response
-        logger.debug("Extracting API key...")
-        api_key_element = root.find("./result/key")
-        if api_key_element is not None:
-            api_key = api_key_element.text
-            logger.debug("Retrieved API key: {}".format(api_key))
-            logger.info("Retrieved API key: {}".format(api_key))
-            return api_key
-        else:
-            logger.error("API key not found in the response.")
-            return None
-
-    except urllib.error.URLError as url_error:
-        logger.error("URL error occurred: {}".format(str(url_error)))
-    except ET.ParseError as parse_error:
-        logger.error("XML parsing error occurred: {}".format(str(parse_error)))
     except Exception as e:
         logger.error("An error occurred: {}".format(str(e)))
-    return None
+        return False
 
 
-def retrieve_license(pan_hostname, api_key):
+def check_content_version(
+    api_key: str,
+    content_version: str,
+    pan_hostname: str,
+) -> bool:
     """
-    Retrieves the PAN-OS firewall licenses from the CSP.
+    Checks if the specified content version (filename) is available from the PANW servers.
 
     Args:
         pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
         api_key (str): The API key for authentication.
+        content_version (str): The content version (filename) to check for.
 
     Returns:
-        bool: True if the Threat Prevention license is present, False otherwise. # noqa: E501
+        bool: True if the content version (filename) is found, False otherwise.
 
     Raises:
         urllib.error.URLError: If a URL error occurs during the API request.
-        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response. # noqa: E501
+        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
         Exception: If any other error occurs during the API request.
-
-    Example:
-        has_threat_prevention = retrieve_license("192.168.1.1", "api_key")
     """
+
     logger.info("=" * 79)
-    logger.info("Retrieving licenses...")
+    logger.info(
+        f"Attempting to check if content version (filename) {content_version} is available"
+    )
     logger.info("=" * 79)
 
     try:
-        # Construct the API URL for retrieving licenses
+        # Construct the API URL
         url = "https://{}/api/?type=op&cmd={}".format(
             pan_hostname,
             urllib.parse.quote_plus(
-                "<request><license><fetch/></license></request>"
-            ),  # noqa: E501
+                "<request><content><upgrade><check/></upgrade></content></request>"
+            ),
         )
         logger.debug("API URL: {}".format(url))
 
         # Create an HTTPS request with SSL verification disabled
         request = urllib.request.Request(url)
         request.add_header("X-PAN-KEY", api_key)
 
         # Send the API request
-        logger.debug("Retrieving licenses...")
+        logger.debug("Sending API request...")
         response = urllib.request.urlopen(
             request, context=urllib.request.ssl._create_unverified_context()
         )
-        logger.debug("Received response: {}".format(response))
 
         # Read the response content
         logger.debug("Reading response content...")
         response_content = response.read().decode("utf-8")
         logger.debug("Received response: {}".format(response_content))
 
         # Parse the XML response
         logger.debug("Parsing XML response...")
         root = ET.fromstring(response_content)
         logger.debug("Root element: {}".format(root.tag))
 
         # Check the response status
-        status = root.attrib.get("status")
-        if status == "success":
-            # Search for the Threat Prevention license
-            threat_prevention_entry = root.find(
-                "./result/licenses/entry[feature='Threat Prevention']"
-            )
-            if threat_prevention_entry is not None:
-                logger.info("Threat Prevention license found.")
-                return True
-            else:
-                logger.warning("Threat Prevention license not found.")
-                return False
+        if root.attrib.get("status") == "success":
+            # Find all 'entry' elements in the XML response
+            entries = root.findall(".//entry")
+
+            # Iterate over each 'entry' element
+            for entry in entries:
+                # Find the 'filename' element within the 'entry'
+                filename_element = entry.find("filename")
+
+                # Check if the 'filename' element exists and matches the specified content version
+                if (
+                    filename_element is not None
+                    and filename_element.text == content_version
+                ):
+                    logger.info(f"Content version (filename) {content_version} found.")
+                    return True
+
+            # If the content version is not found in any entry
+            logger.info(f"Content version (filename) {content_version} not found.")
+            return False
+
         else:
-            logger.error("API request failed.")
+            error_message = root.find("./msg/line")
+            if error_message is not None:
+                logger.error("API request failed: {}".format(error_message.text))
+            else:
+                logger.error("API request failed.")
             return False
 
     except urllib.error.URLError as url_error:
         logger.error("URL error occurred: {}".format(str(url_error)))
+        return False
+
     except ET.ParseError as parse_error:
         logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+        return False
+
     except Exception as e:
         logger.error("An error occurred: {}".format(str(e)))
-    return False
+        return False
 
 
-def import_content_via_scp(
-    pan_hostname,
-    pan_username,
-    pan_password,
-    pi_hostname,
-    pi_username,
-    pi_password,
-    content_path,
-    content_file,
-):
+def copy_content_via_scp(
+    content_path: str,
+    content_version: str,
+    pan_hostname: str,
+    pan_password_new: str,
+    pan_username: str,
+    pi_hostname: str,
+    pi_password: str,
+    pi_username: str,
+) -> Optional[bool]:
     """
     Imports content to the PAN-OS firewall using SCP.
 
     Args:
         pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
         pan_username (str): The username for authentication.
-        pan_password (str): The password for authentication.
+        pan_password_new (str): The password for authentication.
         pi_hostname (str): The hostname or IP address of the Raspberry Pi.
-        pi_content_path (str): The path to the content file on the Raspberry Pi.
-        content_file (str): The name of the content file.
+        content_path (str): The path to the content file on the Raspberry Pi.
+        content_version (str): The name of the content file.
+        pi_username (str): The username for authentication on the Raspberry Pi.
+        pi_password (str): The password for authentication on the Raspberry Pi.
 
     Returns:
-        None
+        Optional[bool]: True if the SCP import is successful, False otherwise.
 
     Raises:
         paramiko.AuthenticationException: If authentication fails.
         paramiko.SSHException: If an SSH exception occurs.
         Exception: If any other error occurs during the SCP import process.
-
-    Example:
-        import_content_via_scp("192.168.1.1", "admin", "password", "192.168.1.2", "/var/tmp/", "content.txt") # noqa: E501
     """
 
     logger.info("=" * 79)
     logger.info("Importing content via SCP...")
     logger.info("=" * 79)
 
     # Create an SSH client
     client = paramiko.SSHClient()
     client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     try:
         # Connect to the firewall
         logger.debug("Connecting to {}...".format(pan_hostname))
         client.connect(
-            pan_hostname,
+            hostname=pan_hostname,
             username=pan_username,
-            password=pan_password,
+            password=pan_password_new,
         )
         logger.info("Connected to {} successfully.".format(pan_hostname))
 
         # Create an interactive shell
         shell = client.invoke_shell()
 
         # Wait for the prompt
@@ -312,273 +261,485 @@
         logger.debug("Received output: {}".format(output))
 
         # Send the scp import command
         scp_command = "scp import content from {}@{}:{}/{}".format(
             pi_username,
             pi_hostname,
             content_path,
-            content_file,
+            content_version,
         )
         logger.debug("Sending SCP command: {}".format(scp_command))
         shell.send(scp_command + "\n")
         time.sleep(5)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Check if the host authenticity prompt appears
         logger.debug("Checking for host authenticity prompt...")
         if (
             "Please type 'yes', 'no' or the fingerprint" in output
             or "Are you sure you want to continue connecting" in output
-        ):  # noqa: E501
+        ):
             logger.debug("Sending 'yes' to the prompt...")
             shell.send("yes\n")
             time.sleep(3)
             output = shell.recv(1024).decode("utf-8")
             logger.debug("Received output: {}".format(output))
 
-        # Send the password for pi@
-        logger.debug(
-            "Sending password for {}@{}...".format(pi_username, pi_hostname)
-        )  # noqa: E501
+        # Send the password for the Raspberry Pi
+        logger.debug("Sending password for {}@{}...".format(pi_username, pi_hostname))
         time.sleep(3)
         shell.send(pi_password + "\n")
         time.sleep(3)
         output = shell.recv(1024).decode("utf-8")
         logger.debug("Received output: {}".format(output))
 
         # Wait for the completion prompt
         logger.debug("Waiting for the completion prompt...")
         start_time = time.time()
         while True:
             if time.time() - start_time > 120:
                 logger.error(
                     "Timeout occurred while waiting for the completion prompt."
                 )
-                break
+
+                # Close the SSH connection
+                client.close()
+                return False
+
             output += shell.recv(1024).decode("utf-8")
             logger.debug("Received output: {}".format(output))
+
+            # Check if the content file already exists
             if "already exists" in output:
                 logger.info("Content file already exists on the firewall.")
-                break
+
+                # Close the SSH connection
+                client.close()
+                return True
+
+            # Check if the import is completed
             elif "saved" in output and "ETA" not in output:
                 logger.debug("SCP import content completed successfully.")
                 logger.info("SCP import content completed successfully.")
-                break
-            time.sleep(3)
 
-        # Close the SSH connection
-        client.close()
+                # Close the SSH connection
+                client.close()
+                return True
+
+            # Wait for 3 seconds before the next iteration
+            time.sleep(3)
 
     except paramiko.AuthenticationException:
         logger.error("Authentication failed. Please check your credentials.")
+        return False
+
     except paramiko.SSHException as ssh_exception:
         logger.error("SSH exception occurred: {}".format(str(ssh_exception)))
+        return False
+
     except Exception as e:
         logger.error("An error occurred: {}".format(str(e)))
+        return False
 
 
-def install_content_from_servers(
-    pan_hostname,
-    api_key,
-):
+def download_software(
+    api_key: str,
+    content_version: str,
+    pan_hostname: str,
+) -> Optional[str]:
     """
-    Sends an API request to install the content on the PAN-OS firewall.
+    Downloads the specified software version from the PANW servers.
 
     Args:
         pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
         api_key (str): The API key for authentication.
-        content_file (str): The name of the content file to install.
+        content_version (str): The version of the software to download.
 
     Returns:
-        str: The job ID if the API request is successful, None otherwise.
+        Optional[str]: The job ID if the API request is successful, None otherwise.
 
     Raises:
         urllib.error.URLError: If a URL error occurs during the API request.
-        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response. # noqa: E501
+        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
         Exception: If any other error occurs during the API request.
-
-    Example:
-        job_id = install_content_via_usb("192.168.1.1", "api_key", "content.txt")
     """
 
     logger.info("=" * 79)
-    logger.info("Attempting to update content from public PANW servers...")
+    logger.info("Attempting to download software version: {}".format(content_version))
     logger.info("=" * 79)
 
     try:
         # Construct the API URL
         url = "https://{}/api/?type=op&cmd={}".format(
             pan_hostname,
             urllib.parse.quote_plus(
-                "<request><content><upgrade><install><version>latest</version></install></upgrade></content></request>"  # noqa: E501
+                "<request><content><upgrade><download><file>{}</file></download></upgrade></content></request>".format(
+                    content_version
+                )
             ),
         )
         logger.debug("API URL: {}".format(url))
 
         # Create an HTTPS request with SSL verification disabled
         request = urllib.request.Request(url)
         request.add_header("X-PAN-KEY", api_key)
 
         # Send the API request
         logger.debug("Sending API request...")
         response = urllib.request.urlopen(
             request, context=urllib.request.ssl._create_unverified_context()
         )
-        logger.debug("Received response: {}".format(response))
 
         # Read the response content
         logger.debug("Reading response content...")
         response_content = response.read().decode("utf-8")
         logger.debug("Received response: {}".format(response_content))
 
         # Parse the XML response
         logger.debug("Parsing XML response...")
         root = ET.fromstring(response_content)
         logger.debug("Root element: {}".format(root.tag))
 
         # Check the response status
         if root.attrib.get("status") == "success":
             job_element = root.find("./result/job")
+
+            # Extract the job ID from the response
             if job_element is not None:
                 job_id = job_element.text
                 logger.info(
-                    "API request successful. Job ID: {}".format(job_id)
-                )  # noqa: E501
+                    "API request successful. Job ID: {}".format(job_id),
+                )
                 return job_id
+
+            # Log an error if the job ID is not found
             else:
                 logger.error("Job ID not found in the response.")
                 return None
-        elif root.attrib.get("line") > 0:
-            logger.error(
-                "API request failed: {}".format(root.attrib.get("line"))
-            )  # noqa: E501
-            return None
+
         else:
-            logger.error("API request failed.")
+            error_message = root.find("./msg/line")
+            if error_message is not None:
+                logger.error("API request failed: {}".format(error_message.text))
+            else:
+                logger.error("API request failed.")
             return None
 
     except urllib.error.URLError as url_error:
         logger.error("URL error occurred: {}".format(str(url_error)))
+        return None
+
     except ET.ParseError as parse_error:
         logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+        return None
+
     except Exception as e:
         logger.error("An error occurred: {}".format(str(e)))
+        return None
 
 
 def install_content_via_usb(
-    pan_hostname,
-    api_key,
-    content_file,
-):
+    api_key: str,
+    content_version: str,
+    pan_hostname: str,
+) -> Optional[str]:
     """
     Sends an API request to install the content on the PAN-OS firewall.
 
     Args:
         pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
         api_key (str): The API key for authentication.
-        content_file (str): The name of the content file to install.
+        content_version (str): The name of the content file to install.
 
     Returns:
-        str: The job ID if the API request is successful, None otherwise.
+        Optional[str]: The job ID if the API request is successful, None otherwise.
 
     Raises:
         urllib.error.URLError: If a URL error occurs during the API request.
-        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response. # noqa: E501
+        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
         Exception: If any other error occurs during the API request.
-
-    Example:
-        job_id = install_content_via_usb("192.168.1.1", "api_key", "content.txt")
     """
 
     logger.info("=" * 79)
     logger.info("Attempting to update content from USB...")
     logger.info("=" * 79)
 
     try:
         # Construct the API URL
         url = "https://{}/api/?type=op&cmd={}".format(
             pan_hostname,
             urllib.parse.quote_plus(
-                "<request><content><upgrade><install><file>{}</file></install></upgrade></content></request>".format(  # noqa: E501
-                    content_file
+                "<request><content><upgrade><install><file>{}</file></install></upgrade></content></request>".format(
+                    content_version
                 )
             ),
         )
         logger.debug("API URL: {}".format(url))
 
         # Create an HTTPS request with SSL verification disabled
         request = urllib.request.Request(url)
         request.add_header("X-PAN-KEY", api_key)
 
         # Send the API request
         logger.debug("Sending API request...")
         response = urllib.request.urlopen(
             request, context=urllib.request.ssl._create_unverified_context()
         )
-        logger.debug("Received response: {}".format(response))
 
         # Read the response content
         logger.debug("Reading response content...")
         response_content = response.read().decode("utf-8")
         logger.debug("Received response: {}".format(response_content))
 
         # Parse the XML response
         logger.debug("Parsing XML response...")
         root = ET.fromstring(response_content)
         logger.debug("Root element: {}".format(root.tag))
 
         # Check the response status
         if root.attrib.get("status") == "success":
             job_element = root.find("./result/job")
+
+            # Extract the job ID from the response
             if job_element is not None:
                 job_id = job_element.text
-                logger.info(
-                    "API request successful. Job ID: {}".format(job_id)
-                )  # noqa: E501
+                logger.info("API request successful. Job ID: {}".format(job_id))
                 return job_id
+
+            # Log an error if the job ID is not found
             else:
                 logger.error("Job ID not found in the response.")
                 return None
+
+        else:
+            error_message = root.find("./msg/line")
+            if error_message is not None:
+                logger.error("API request failed: {}".format(error_message.text))
+            else:
+                logger.error("API request failed.")
+            return None
+
+    except urllib.error.URLError as url_error:
+        logger.error("URL error occurred: {}".format(str(url_error)))
+        return None
+
+    except ET.ParseError as parse_error:
+        logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+
+        return None
+    except Exception as e:
+        logger.error("An error occurred: {}".format(str(e)))
+        return None
+
+
+def install_latest_content_from_servers(
+    pan_hostname: str,
+    api_key: str,
+) -> Optional[str]:
+    """
+    Sends an API request to install the latest content from the PANW servers.
+
+    Args:
+        pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
+        api_key (str): The API key for authentication.
+
+    Returns:
+        Optional[str]: The job ID if the API request is successful, None otherwise.
+
+    Raises:
+        urllib.error.URLError: If a URL error occurs during the API request.
+        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
+        Exception: If any other error occurs during the API request.
+    """
+
+    logger.info("=" * 79)
+    logger.info("Attempting to update content from public PANW servers...")
+    logger.info("=" * 79)
+
+    try:
+        # Construct the API URL
+        url = "https://{}/api/?type=op&cmd={}".format(
+            pan_hostname,
+            urllib.parse.quote_plus(
+                "<request><content><upgrade><install><version>latest</version></install></upgrade></content></request>"
+            ),
+        )
+        logger.debug("API URL: {}".format(url))
+
+        # Create an HTTPS request with SSL verification disabled
+        request = urllib.request.Request(url)
+        request.add_header("X-PAN-KEY", api_key)
+
+        # Send the API request
+        logger.debug("Sending API request...")
+        response = urllib.request.urlopen(
+            request, context=urllib.request.ssl._create_unverified_context()
+        )
+
+        # Read the response content
+        logger.debug("Reading response content...")
+        response_content = response.read().decode("utf-8")
+        logger.debug("Received response: {}".format(response_content))
+
+        # Parse the XML response
+        logger.debug("Parsing XML response...")
+        root = ET.fromstring(response_content)
+        logger.debug("Root element: {}".format(root.tag))
+
+        # Check the response status
+        if root.attrib.get("status") == "success":
+            job_element = root.find("./result/job")
+
+            # Extract the job ID from the response
+            if job_element is not None:
+                job_id = job_element.text
+                logger.info("API request successful. Job ID: {}".format(job_id))
+                return job_id
+
+            # Log an error if the job ID is not found
+            else:
+                logger.error("Job ID not found in the response.")
+                return None
+
         elif root.attrib.get("line") > 0:
-            logger.error(
-                "API request failed: {}".format(root.attrib.get("line"))
-            )  # noqa: E501
+            logger.error("API request failed: {}".format(root.attrib.get("line")))
             return None
+
         else:
             logger.error("API request failed.")
             return None
 
     except urllib.error.URLError as url_error:
         logger.error("URL error occurred: {}".format(str(url_error)))
+        return None
+
+    except ET.ParseError as parse_error:
+        logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+        return None
+
+    except Exception as e:
+        logger.error("An error occurred: {}".format(str(e)))
+        return None
+
+
+def install_specific_content_from_servers(
+    api_key: str,
+    content_version: str,
+    pan_hostname: str,
+) -> Optional[str]:
+    """
+    Sends an API request to install the specific content version from the PANW servers.
+
+    Args:
+        pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
+        api_key (str): The API key for authentication.
+        content_version (str): The version of the content to install.
+
+    Returns:
+        Optional[str]: The job ID if the API request is successful, None otherwise.
+
+    Raises:
+        urllib.error.URLError: If a URL error occurs during the API request.
+        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
+        Exception: If any other error occurs during the API request.
+    """
+
+    logger.info("=" * 79)
+    logger.info(f"Attempting to install specific content version: {content_version}")
+    logger.info("=" * 79)
+
+    try:
+        # Construct the API URL
+        url = "https://{}/api/?type=op&cmd={}".format(
+            pan_hostname,
+            urllib.parse.quote_plus(
+                "<request><content><upgrade><install><file>{}</file></install></upgrade></content></request>".format(
+                    content_version
+                )
+            ),
+        )
+        logger.debug("API URL: {}".format(url))
+
+        # Create an HTTPS request with SSL verification disabled
+        request = urllib.request.Request(url)
+        request.add_header("X-PAN-KEY", api_key)
+
+        # Send the API request
+        logger.debug("Sending API request...")
+        response = urllib.request.urlopen(
+            request, context=urllib.request.ssl._create_unverified_context()
+        )
+
+        # Read the response content
+        logger.debug("Reading response content...")
+        response_content = response.read().decode("utf-8")
+        logger.debug("Received response: {}".format(response_content))
+
+        # Parse the XML response
+        logger.debug("Parsing XML response...")
+        root = ET.fromstring(response_content)
+        logger.debug("Root element: {}".format(root.tag))
+
+        # Check the response status
+        if root.attrib.get("status") == "success":
+            job_element = root.find("./result/job")
+
+            # Extract the job ID from the response
+            if job_element is not None:
+                job_id = job_element.text
+                logger.info("API request successful. Job ID: {}".format(job_id))
+                return job_id
+
+            # Log an error if the job ID is not found
+            else:
+                logger.error("Job ID not found in the response.")
+                return None
+
+        else:
+            error_message = root.find("./msg/line")
+            if error_message is not None:
+                logger.error("API request failed: {}".format(error_message.text))
+            else:
+                logger.error("API request failed.")
+            return None
+
+    except urllib.error.URLError as url_error:
+        logger.error("URL error occurred: {}".format(str(url_error)))
+        return None
+
     except ET.ParseError as parse_error:
         logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+        return None
+
     except Exception as e:
         logger.error("An error occurred: {}".format(str(e)))
+        return None
 
 
-def monitor_job_status(pan_hostname, api_key, job_id):
+def monitor_job_status(
+    api_key: str,
+    job_id: str,
+    pan_hostname: str,
+) -> Optional[bool]:
     """
     Monitors the status of a job on the PAN-OS firewall.
 
     Args:
         pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
         api_key (str): The API key for authentication.
         job_id (str): The ID of the job to monitor.
 
     Returns:
-        None
+        Optional[bool]: True if the job is completed successfully, False otherwise.
 
     Raises:
         urllib.error.URLError: If a URL error occurs during the API request.
-        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response. # noqa: E501
+        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
         Exception: If any other error occurs during the job monitoring process.
-
-    Example:
-        monitor_job_status("192.168.1.1", "api_key", "job_id")
     """
 
     logger.info("=" * 79)
     logger.info("Monitoring job status...")
     logger.info("=" * 79)
 
     start_time = time.time()
@@ -598,59 +759,291 @@
             request = urllib.request.Request(url)
             request.add_header("X-PAN-KEY", api_key)
 
             # Send the API request
             logger.debug("Sending job monitoring request...")
             response = urllib.request.urlopen(
                 request,
-                context=urllib.request.ssl._create_unverified_context(),  # noqa: E501
+                context=urllib.request.ssl._create_unverified_context(),
             )
-            logger.debug("Received response: {}".format(response))
 
             # Read the response content
             logger.debug("Reading response content...")
             response_content = response.read().decode("utf-8")
             logger.debug("Received response: {}".format(response_content))
 
             # Parse the XML response
             logger.debug("Parsing XML response...")
             root = ET.fromstring(response_content)
             logger.debug("Root element: {}".format(root.tag))
 
             # Check the job status
             job_status_element = root.find("./result/job/status")
+
+            # Check if the job status is FIN
             if job_status_element is not None:
                 job_status = job_status_element.text
                 if job_status == "FIN":
                     job_result_element = root.find("./result/job/result")
+
+                    # Check the job result
                     if job_result_element is not None:
                         job_result = job_result_element.text
                         if job_result == "OK":
                             logger.info("Job completed successfully.")
-                            return
+                            return True
                         else:
-                            logger.error("Job completed with an error.")  # noqa: E501
+                            logger.error("Job completed with an error.")
                             logger.error(job_result)
-                            sys.exit(1)
+                            return False
+
+                    # Log an error if the job result is not found
                     else:
                         logger.error("Job result not found in the response.")
-                        sys.exit(1)
+                        return False
+
+            # Check if the job status is ACT
             else:
                 logger.error("Job status not found in the response.")
-                sys.exit(1)
+                return False
 
             # Check the timeout
             if time.time() - start_time > 300:
                 logger.error("Job monitoring timed out.")
-                sys.exit(1)
+                return False
 
             # Wait for 3 seconds before the next iteration
             time.sleep(3)
 
         except urllib.error.URLError as url_error:
             logger.error("URL error occurred: {}".format(str(url_error)))
         except ET.ParseError as parse_error:
-            logger.error(
-                "XML parsing error occurred: {}".format(str(parse_error))
-            )  # noqa: E501
+            logger.error("XML parsing error occurred: {}".format(str(parse_error)))
         except Exception as e:
             logger.error("An error occurred: {}".format(str(e)))
+
+
+def private_data_reset(
+    api_key: str,
+    pan_hostname: str,
+) -> bool:
+    """
+    Resets the configuration data on the PAN-OS firewall.
+
+    Args:
+        pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
+        api_key (str): The api key used for authentication.
+
+    Returns:
+        Optional[bool]: True if the job is completed successfully, False otherwise.
+
+    Raises:
+        urllib.error.URLError: If a URL error occurs during the API request.
+        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
+        Exception: If any other error occurs during the job monitoring process.
+    """
+
+    logger.info("=" * 79)
+    logger.info("Resetting the private data...")
+    logger.info("=" * 79)
+
+    while True:
+        try:
+            # Construct the API URL for private data reset
+            url = "https://{}/api/?type=op&cmd={}".format(
+                pan_hostname,
+                urllib.parse.quote_plus(
+                    "<request><system><private-data-reset/></system></request>"
+                ),
+            )
+            logger.debug("Request Private Data Reset URL: {}".format(url))
+
+            # Create an HTTPS request with SSL verification disabled
+            request = urllib.request.Request(url)
+            request.add_header("X-PAN-KEY", api_key)
+
+            # Send the API request
+            logger.debug("Sending job monitoring request...")
+            response = urllib.request.urlopen(
+                request,
+                context=urllib.request.ssl._create_unverified_context(),
+            )
+
+            # Check the status code
+            if response.getcode() != 200:
+                raise ValueError(
+                    "HTTP request failed with status code: {}".format(
+                        response.getcode()
+                    )
+                )
+
+            # Read the response content
+            logger.debug("Reading response content...")
+            response_content = response.read().decode("utf-8")
+            logger.debug("Received response: {}".format(response_content))
+
+            return True
+
+        except urllib.error.URLError as url_error:
+            logger.error("URL error occurred: {}".format(str(url_error)))
+            return False
+
+        except ET.ParseError as parse_error:
+            logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+            return False
+
+        except Exception as e:
+            logger.error("An error occurred: {}".format(str(e)))
+            return False
+
+
+def retrieve_api_key(
+    pan_hostname: str,
+    pan_password_new: str,
+    pan_username: str,
+) -> Optional[str]:
+    """
+    Retrieves the API key from the PAN-OS firewall.
+
+    Args:
+        pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
+        pan_username (str): The username for authentication.
+        pan_password_new (str): The password for authentication.
+
+    Returns:
+        Optional[str]: The API key if successfully retrieved, None otherwise.
+
+    Raises:
+        urllib.error.URLError: If a URL error occurs during the API request.
+        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
+        Exception: If any other error occurs during the API request.
+    """
+
+    logger.info("=" * 79)
+    logger.info("Retrieving API key...")
+    logger.info("=" * 79)
+
+    try:
+        # Construct the API URL
+        url = "https://{}/api/?type=keygen&user={}&password={}".format(
+            pan_hostname, pan_username, urllib.parse.quote(pan_password_new)
+        )
+        logger.debug("API URL: {}".format(url))
+
+        # Create an HTTPS request with SSL verification disabled
+        logger.debug("Retrieving API key...")
+        request = urllib.request.Request(url)
+        response = urllib.request.urlopen(
+            request, context=urllib.request.ssl._create_unverified_context()
+        )
+
+        # Read the response content
+        logger.debug("Reading response content...")
+        response_content = response.read().decode("utf-8")
+        logger.debug("Received response: {}".format(response_content))
+
+        # Parse the XML response
+        logger.debug("Parsing XML response...")
+        root = ET.fromstring(response_content)
+        logger.debug("Root element: {}".format(root.tag))
+
+        # Extract the API key from the response
+        logger.debug("Extracting API key...")
+        api_key_element = root.find("./result/key")
+        if api_key_element is not None:
+            api_key = api_key_element.text
+            logger.debug("Retrieved API key: {}".format(api_key))
+            logger.info("Retrieved API key: {}".format(api_key))
+            return api_key
+        else:
+            logger.error("API key not found in the response.")
+            return None
+
+    except urllib.error.URLError as url_error:
+        logger.error("URL error occurred: {}".format(str(url_error)))
+        return None
+
+    except ET.ParseError as parse_error:
+        logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+        return None
+
+    except Exception as e:
+        logger.error("An error occurred: {}".format(str(e)))
+        return None
+
+
+def retrieve_license(
+    api_key: str,
+    pan_hostname: str,
+) -> Optional[bool]:
+    """
+    Retrieves the PAN-OS firewall licenses from the CSP.
+
+    Args:
+        pan_hostname (str): The hostname or IP address of the PAN-OS firewall.
+        api_key (str): The API key for authentication.
+
+    Returns:
+        Optional[bool]: True if the Threat Prevention license is present, False otherwise.
+
+    Raises:
+        urllib.error.URLError: If a URL error occurs during the API request.
+        xml.etree.ElementTree.ParseError: If an error occurs while parsing the XML response.
+        Exception: If any other error occurs during the API request.
+    """
+
+    logger.info("=" * 79)
+    logger.info("Retrieving licenses...")
+    logger.info("=" * 79)
+
+    try:
+        # Construct the API URL for retrieving licenses
+        url = "https://{}/api/?type=op&cmd={}".format(
+            pan_hostname,
+            urllib.parse.quote_plus("<request><license><fetch/></license></request>"),
+        )
+        logger.debug("API URL: {}".format(url))
+
+        # Create an HTTPS request with SSL verification disabled
+        request = urllib.request.Request(url)
+        request.add_header("X-PAN-KEY", api_key)
+
+        # Send the API request
+        logger.debug("Retrieving licenses...")
+        response = urllib.request.urlopen(
+            request, context=urllib.request.ssl._create_unverified_context()
+        )
+
+        # Read the response content
+        logger.debug("Reading response content...")
+        response_content = response.read().decode("utf-8")
+        logger.debug("Received response: {}".format(response_content))
+
+        # Parse the XML response
+        logger.debug("Parsing XML response...")
+        root = ET.fromstring(response_content)
+        logger.debug("Root element: {}".format(root.tag))
+
+        # Check the response status
+        status = root.attrib.get("status")
+        if status == "success":
+            # Search for the Threat Prevention license
+            threat_prevention_entry = root.find(
+                "./result/licenses/entry[feature='Threat Prevention']"
+            )
+            if threat_prevention_entry is not None:
+                logger.info("Threat Prevention license found.")
+                return True
+            else:
+                logger.warning("Threat Prevention license not found.")
+                return False
+        else:
+            logger.error("API request failed.")
+            return False
+
+    except urllib.error.URLError as url_error:
+        logger.error("URL error occurred: {}".format(str(url_error)))
+    except ET.ParseError as parse_error:
+        logger.error("XML parsing error occurred: {}".format(str(parse_error)))
+    except Exception as e:
+        logger.error("An error occurred: {}".format(str(e)))
+    return False
```

### Comparing `pan_ztp_patcher-0.2.4/PKG-INFO` & `pan_ztp_patcher-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-ztp-patcher
-Version: 0.2.4
+Version: 0.2.5
 Summary: Update content version on PAN-OS firewalls
 License: Apache2.0
 Author: Calvin Remsburg
 Author-email: cremsburg.dev@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -53,24 +53,24 @@
 ```
 
 ## Usage
 
 To use the PAN-OS ZTP Patcher, run the following command:
 
 ```bash
-ztp_patcher --hostname <hostname> --username <username> --old-password <old_password> --new-password <new_password> [--pi-hostname <pi_hostname>] [--pi-content-path <pi_content_path>] [--content-file <content_file>]
+ztp_patcher --hostname <hostname> --username <username> --old-password <old_password> --new-password <new_password> [--pi-hostname <pi_hostname>] [--pi-content-path <pi_content_path>] [--content-file <content_version>]
 ```
 
 - `<hostname>`: The hostname or IP address of the PAN-OS firewall.
 - `<username>`: The username for accessing the PAN-OS firewall.
 - `<old_password>`: The current password for the specified user on the PAN-OS firewall.
 - `<new_password>`: The new password to be set for the specified user on the PAN-OS firewall.
 - `<pi_hostname>` (optional): The hostname or IP address of the Raspberry Pi Zero appliance (default: 192.168.1.2).
 - `<pi_content_path>` (optional): The path on the Raspberry Pi Zero where the content file is located (default: /var/tmp/).
-- `<content_file>` (optional): The name of the content file to be installed on the PAN-OS firewall (default: panupv2-all-contents-8834-8684).
+- `<content_version>` (optional): The name of the content file to be installed on the PAN-OS firewall (default: panupv2-all-contents-8834-8684).
 
 Example:
 
 ```bash
 ztp_patcher --hostname 192.168.1.1 --username admin --old-password admin --new-password PaloAlto123!
 ```
```

