# Comparing `tmp/macaw-auth-1.0.0.tar.gz` & `tmp/macaw_auth-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macaw-auth-1.0.0.tar", last modified: Tue May  9 04:43:08 2023, max compression
+gzip compressed data, was "macaw_auth-1.1.0.tar", last modified: Fri Apr 19 03:45:28 2024, max compression
```

## Comparing `macaw-auth-1.0.0.tar` & `macaw_auth-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:43:08.280560 macaw-auth-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-09 04:43:08.280560 macaw-auth-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:43:08.276560 macaw-auth-1.0.0/macaw_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-09 04:43:08.000000 macaw-auth-1.0.0/macaw_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-09 04:43:08.000000 macaw-auth-1.0.0/macaw_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:43:08.000000 macaw-auth-1.0.0/macaw_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 04:43:08.000000 macaw-auth-1.0.0/macaw_auth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-09 04:43:08.000000 macaw-auth-1.0.0/macaw_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-09 04:43:08.000000 macaw-auth-1.0.0/macaw_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 04:43:08.280560 macaw-auth-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:43:08.276560 macaw-auth-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:43:08.276560 macaw-auth-1.0.0/src/macaw_auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:43:08.276560 macaw-auth-1.0.0/src/macaw_auth/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/classes/aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/classes/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/classes/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/classes/idp_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/classes/sts_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/classes/user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/classes/username_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:43:08.280560 macaw-auth-1.0.0/src/macaw_auth/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/src/macaw_auth/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:43:08.280560 macaw-auth-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-09 04:42:56.000000 macaw-auth-1.0.0/tests/test_usernames.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.982154 macaw_auth-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-19 03:45:28.982154 macaw_auth-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.982154 macaw_auth-1.1.0/macaw_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 03:45:28.000000 macaw_auth-1.1.0/macaw_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:45:28.982154 macaw_auth-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.978153 macaw_auth-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.978153 macaw_auth-1.1.0/src/macaw_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.978153 macaw_auth-1.1.0/src/macaw_auth/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/idp_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/sts_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/classes/username_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.978153 macaw_auth-1.1.0/src/macaw_auth/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/src/macaw_auth/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:45:28.982154 macaw_auth-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-19 03:45:21.000000 macaw_auth-1.1.0/tests/test_usernames.py
```

### Comparing `macaw-auth-1.0.0/LICENSE` & `macaw_auth-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macaw-auth-1.0.0/PKG-INFO` & `macaw_auth-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: macaw-auth
-Version: 1.0.0
-Summary: Tool to obtain AWS CLI credentials from ADFS.
-Author-email: Travis Samuel <tsamuel@alum.mit.edu>
-Project-URL: Homepage, https://github.com/tsamuel33/macaw-auth
-Project-URL: Bug Tracker, https://github.com/tsamuel33/macaw-auth/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # macaw-auth
 
 ## Description
 
 This repository contains code used to run the macaw-auth utility. Named after the
 Hyacinth and Scarlet Macaws of the Amazon Rainforest, this tool allows users to
 authenticate to ADFS to obtain their AWS credentials for use with the AWS CLI.
@@ -35,15 +21,15 @@
 
 ```text
 pip install macaw-auth
 ```
 
 ### Usage
 
-A sample config file can be found [here](/examples/config). Your config file should be stored in ~/.aws/config, but if you store it elsewhere, you can pass it to
+A sample config file can be found [here](https://github.com/tsamuel33/macaw-auth/blob/main/examples/config). Your config file should be stored in ~/.aws/config, but if you store it elsewhere, you can pass it to
 macaw-auth using the **--credentials-file** flag. Be sure to update the following values in your config:
 
 * identity_url
 * username
 * role_arn
 * principal_arn
 
@@ -98,13 +84,33 @@
   --credential-file CREDENTIAL_FILE
                         Path to credential file if ~/.aws/credentials will not be used
   --username-not-email  Indicates that the supplied username will not need to be in an email format
 ```
 
 ## Troubleshooting
 
+### Clear Saved Password
+
 If you receive an error indicating that there's no valid SAML assertation, please double check your config settings. If you have keyring enabled, you may have stored
-an incorrect password. To reset your keyring password, run the following command:
+an incorrect password. To reset your keyring password, run one of the following commands:
 
 ```text
 macaw-auth -r
 ```
+
+or
+
+```text
+macaw-auth --reset-password
+```
+
+### Errors Running the Utility With Keyring Enabled
+
+This utility gives the option to use [Keyring](https://pypi.org/project/keyring/) to locally store your password. If you attempt to use Keyring and do not have a proper backend set up as stated in the Keyring documentation, macaw-auth may not work. To disable Keyring, use one of the following options:
+
+#### 1. **Disable Keyring in Config File**
+
+In your config file, you can set ```enable_keyring = False``` in the **[macaw-auth]** section
+
+#### 2. **Disable Keyring via CLI**
+
+When running macaw-auth commands, you can add the **--disable-keyring** flag (e.g., ```macaw-auth --disable-keyring```).
```

### Comparing `macaw-auth-1.0.0/macaw_auth.egg-info/SOURCES.txt` & `macaw_auth-1.1.0/macaw_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macaw-auth-1.0.0/pyproject.toml` & `macaw_auth-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.5.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macaw-auth"
-version = "1.0.0"
+version = "1.1.0"
 description = "Tool to obtain AWS CLI credentials from ADFS."
 readme = "README.md"
 authors = [
     { name="Travis Samuel", email="tsamuel@alum.mit.edu" },
 ]
 requires-python = ">3.7"
 classifiers = [
```

### Comparing `macaw-auth-1.0.0/src/macaw_auth/classes/aws_credentials.py` & `macaw_auth-1.1.0/src/macaw_auth/classes/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `macaw-auth-1.0.0/src/macaw_auth/classes/configuration.py` & `macaw_auth-1.1.0/src/macaw_auth/classes/configuration.py`

 * *Files identical despite different names*

### Comparing `macaw-auth-1.0.0/src/macaw_auth/classes/errors.py` & `macaw_auth-1.1.0/src/macaw_auth/classes/errors.py`

 * *Files identical despite different names*

### Comparing `macaw-auth-1.0.0/src/macaw_auth/classes/idp_connection.py` & `macaw_auth-1.1.0/src/macaw_auth/classes/idp_connection.py`

 * *Files identical despite different names*

### Comparing `macaw-auth-1.0.0/src/macaw_auth/classes/sts_saml.py` & `macaw_auth-1.1.0/src/macaw_auth/classes/sts_saml.py`

 * *Files identical despite different names*

### Comparing `macaw-auth-1.0.0/src/macaw_auth/classes/user_credentials.py` & `macaw_auth-1.1.0/src/macaw_auth/classes/user_credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # from . import errors
 # Keyring may require importing dbus-python to work on Linux
 # dbus-python may not install properly via pip, so may need to disable keyring on linux
 import keyring
 from getpass import getpass
+from .idp_connection import SAMLAssertion
 
 class UserCredentials:
     """
     A class to represent a user's credentials for authenticating to AWS
 
     ...
 
@@ -21,29 +22,29 @@
     password_stored : bool
         boolean stating if the user's password is saved in keyring
     """
 
     # Set constant values
     keyring_service_name = "AWSUserCredentials"
 
-    def __init__(self, username, reset_password=False, enable_keyring=False):
+    def __init__(self, username, identity_url, auth_type, ssl_verification=True, reset_password=False, enable_keyring=False):
         self.username = username
-        self.reset_password = reset_password
         self.enable_keyring = enable_keyring
-        if enable_keyring:
+        if enable_keyring.lower() == "true":
             keyring.get_keyring()
             self._password_stored = self.check_if_password_stored()
             if not self._password_stored:
                 self.set_keyring_password(getpass())
-            elif self._password_stored and self.reset_password:
+            elif self._password_stored and reset_password:
                 print('Resetting password.')
                 self.set_keyring_password(getpass())
+            self.__password = self.get_keyring_password()
         else:
             self.__password = getpass()
-            #TODO - add a way to pass password if keyring is disabled
+        self.assertion = SAMLAssertion(self.username, self.__password, identity_url, auth_type, ssl_verification).assertion
 
     def get_keyring_password(self):
         if self.enable_keyring:
             print('Getting password from keyring...')
             creds = keyring.get_password(
                 self.keyring_service_name, self.username)
             return creds
```

### Comparing `macaw-auth-1.0.0/src/macaw_auth/classes/username_validation.py` & `macaw_auth-1.1.0/src/macaw_auth/classes/username_validation.py`

 * *Files identical despite different names*

### Comparing `macaw-auth-1.0.0/src/macaw_auth/cli/__main__.py` & `macaw_auth-1.1.0/src/macaw_auth/cli/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,36 +25,36 @@
         user = name
     else:
         user = input('User ID: ')
     return user
 
 def main() -> None:
     args = cli_main()
+    #FOR DEBUGGING
     # print(args)
 
     print('Welcome! Checking your configuration files...')
     client_config = Configuration('client', 'macaw-auth',
                            session_duration=(arg_to_string(args['duration_seconds']),False, '3600'),
                            identity_url=(arg_to_string(args['identity_url']),True, ''),
-                           enable_keyring=(arg_to_string(args['keyring']),False, 'True'),
+                           enable_keyring=(arg_to_string(args['enable_keyring']),False, 'False'),
                            username=(None, False, ''))
     client = client_config.config[client_config.config_section]
     role_config = Configuration('user', arg_to_string(args['SOURCE_PROFILE']),
                                 principal_arn=(arg_to_string(args['principal_arn']),False, ''),
                                 role_arn=(arg_to_string(args['role_arn']),False, ''),
                                 region=(arg_to_string(args['region']),False, 'us-east-1'),
                                 output=(arg_to_string(args['output']),False, 'json'),
                                 connection_type=(arg_to_string((args['auth_type'])),False, 'web_form'))
     role = role_config.config[role_config.config_section]
 
     user = get_username(client['username'])
     validation = UsernameValidation(user, args['username_not_email'])
-    user_creds = UserCredentials(validation.username, args['reset_password'], client['enable_keyring'])
-    assertion = SAMLAssertion(validation.username, user_creds.get_keyring_password(), client['identity_url'], args['auth_type'], args['no_ssl'])
-    roles = AWSSTSService(assertion.assertion, role['principal_arn'], role['role_arn'], int(client['session_duration']), role['region'])
+    user_creds = UserCredentials(validation.username, client['identity_url'], args['auth_type'], args['no_ssl'], args['reset_password'], client['enable_keyring'])
+    roles = AWSSTSService(user_creds.assertion, role['principal_arn'], role['role_arn'], int(client['session_duration']), role['region'])
 
 
     aws_creds = AWSCredentials('credential', arg_to_string(args['target_profile']),
                                #TODO - Add functionality for credential file
                                 # args['credential_file'],
                                 region=(role['region'],False, 'us-east-1'),
                                 output=(role['output'],False, 'json'),
```

### Comparing `macaw-auth-1.0.0/src/macaw_auth/cli/cli.py` & `macaw_auth-1.1.0/src/macaw_auth/cli/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     parser = argparse.ArgumentParser(prog='macaw-auth', description='Utility to obtain AWS CLI credentials')
     parser.add_argument('SOURCE_PROFILE', help='Name of the profile in your config file containing the desired configuration', nargs='?', default=None)
     parser.add_argument('--no-ssl-verify', action='store_false', help='Make insecure SAML request', dest='no_ssl')
     parser.add_argument('-r', '--reset-password', action='store_true', help='Reset keyring password')
     parser.add_argument('-a', '--auth-type', help='Authorization type used for SAML request', choices=['ntlm', 'web_form'], nargs='?', default='web_form')
     parser.add_argument('--duration-seconds', help="Length of time in seconds in which credentials are valid", type=int)
     parser.add_argument('--identity-url', help='URL used to initiate SAML request')
-    parser.add_argument('--disable-keyring', action='store_false', help='Disable storing password in keyring', dest='keyring')
+    parser.add_argument('--disable-keyring', action='store_const', help='Disable storing password in keyring', const=False, dest='enable_keyring')
     parser.add_argument('--region', help='Default AWS region for CLI commands')
     parser.add_argument('--output', help='The desired AWS CLI output format', choices=['json', 'yaml', 'yaml-stream', 'text', 'table'])
     parser.add_argument('--role-arn', help='ARN of the role that you want to assume')
     parser.add_argument('--principal-arn', help='ARN of the IAM SAML provider that describes the IdP')
     parser.add_argument('--target-profile', help='Name of the section where credentials will be stored in the credentials file', type=str)
     parser.add_argument('--config-file', help='Path to config file if ~/.aws/config will not be used')
     parser.add_argument('--credential-file', help='Path to credential file if ~/.aws/credentials will not be used')
```

### Comparing `macaw-auth-1.0.0/tests/test_usernames.py` & `macaw_auth-1.1.0/tests/test_usernames.py`

 * *Files identical despite different names*

