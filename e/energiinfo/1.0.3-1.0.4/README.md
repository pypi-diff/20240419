# Comparing `tmp/energiinfo-1.0.3.tar.gz` & `tmp/energiinfo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energiinfo-1.0.3.tar", last modified: Tue Apr 16 13:41:17 2024, max compression
+gzip compressed data, was "energiinfo-1.0.4.tar", last modified: Fri Apr 19 06:24:30 2024, max compression
```

## Comparing `energiinfo-1.0.3.tar` & `energiinfo-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:41:17.095988 energiinfo-1.0.3/
--rw-r--r--   0 veulsan  (2037719458) 1135428931    35149 2024-04-16 12:42:03.000000 energiinfo-1.0.3/LICENSE
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1917 2024-04-16 13:41:17.095754 energiinfo-1.0.3/PKG-INFO
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1359 2024-04-16 12:42:03.000000 energiinfo-1.0.3/README.md
--rw-r--r--   0 veulsan  (2037719458) 1135428931       87 2024-04-16 13:30:50.000000 energiinfo-1.0.3/pyproject.toml
--rw-r--r--   0 veulsan  (2037719458) 1135428931      685 2024-04-16 13:41:17.097957 energiinfo-1.0.3/setup.cfg
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:41:17.074510 energiinfo-1.0.3/src/
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:41:17.081491 energiinfo-1.0.3/src/energiinfo/
--rw-r--r--   0 veulsan  (2037719458) 1135428931       85 2024-04-16 13:40:51.000000 energiinfo-1.0.3/src/energiinfo/__init__.py
--rw-r--r--   0 veulsan  (2037719458) 1135428931     8579 2024-04-16 13:39:47.000000 energiinfo-1.0.3/src/energiinfo/api.py
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1009 2024-04-16 13:18:42.000000 energiinfo-1.0.3/src/energiinfo/const.py
-drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-16 13:41:17.095138 energiinfo-1.0.3/src/energiinfo.egg-info/
--rw-r--r--   0 veulsan  (2037719458) 1135428931     1917 2024-04-16 13:41:17.000000 energiinfo-1.0.3/src/energiinfo.egg-info/PKG-INFO
--rw-r--r--   0 veulsan  (2037719458) 1135428931      267 2024-04-16 13:41:17.000000 energiinfo-1.0.3/src/energiinfo.egg-info/SOURCES.txt
--rw-r--r--   0 veulsan  (2037719458) 1135428931        1 2024-04-16 13:41:17.000000 energiinfo-1.0.3/src/energiinfo.egg-info/dependency_links.txt
--rw-r--r--   0 veulsan  (2037719458) 1135428931       11 2024-04-16 13:41:17.000000 energiinfo-1.0.3/src/energiinfo.egg-info/top_level.txt
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-19 06:24:30.416330 energiinfo-1.0.4/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931    35149 2024-04-16 12:42:03.000000 energiinfo-1.0.4/LICENSE
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     3488 2024-04-19 06:24:30.416081 energiinfo-1.0.4/PKG-INFO
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     2930 2024-04-19 06:20:55.000000 energiinfo-1.0.4/README.md
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       87 2024-04-16 13:30:50.000000 energiinfo-1.0.4/pyproject.toml
+-rw-r--r--   0 veulsan  (2037719458) 1135428931      685 2024-04-19 06:24:30.420449 energiinfo-1.0.4/setup.cfg
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-19 06:24:30.389054 energiinfo-1.0.4/src/
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-19 06:24:30.408250 energiinfo-1.0.4/src/energiinfo/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       85 2024-04-19 06:23:06.000000 energiinfo-1.0.4/src/energiinfo/__init__.py
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     8328 2024-04-19 06:19:39.000000 energiinfo-1.0.4/src/energiinfo/api.py
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     1009 2024-04-16 13:18:42.000000 energiinfo-1.0.4/src/energiinfo/const.py
+drwxr-xr-x   0 veulsan  (2037719458) 1135428931        0 2024-04-19 06:24:30.415562 energiinfo-1.0.4/src/energiinfo.egg-info/
+-rw-r--r--   0 veulsan  (2037719458) 1135428931     3488 2024-04-19 06:24:30.000000 energiinfo-1.0.4/src/energiinfo.egg-info/PKG-INFO
+-rw-r--r--   0 veulsan  (2037719458) 1135428931      267 2024-04-19 06:24:30.000000 energiinfo-1.0.4/src/energiinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 veulsan  (2037719458) 1135428931        1 2024-04-19 06:24:30.000000 energiinfo-1.0.4/src/energiinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 veulsan  (2037719458) 1135428931       11 2024-04-19 06:24:30.000000 energiinfo-1.0.4/src/energiinfo.egg-info/top_level.txt
```

### Comparing `energiinfo-1.0.3/LICENSE` & `energiinfo-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `energiinfo-1.0.3/setup.cfg` & `energiinfo-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = energiinfo
-version = 1.0.3
+version = 1.0.4
 author = Ulrik Sannsell
 author_email = ulrik@sannsell.se
 description = Energiinfo API package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://gitlab.com/veulsan/energiinfo
 project_urls =
```

### Comparing `energiinfo-1.0.3/src/energiinfo/api.py` & `energiinfo-1.0.4/src/energiinfo/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
     def __init__(self, apiurl: str, siteid: str, token: str = None):
          self.api_url = apiurl
          self.session = requests.Session()
          self.siteid = siteid
          if token is not None:
              self.authenticateToken(token)
+
     def getStatus(self):
         return self.status
 
     def getErrorMessage(self):
         return self.error_message
 
     def authenticateToken(self, token: str):
@@ -56,36 +57,35 @@
 
         error_message = ''
 
         try:
             response = self.session.post(login_url, data=data)
             # Check if the login request was successful (status code 200)
             if response.status_code == 200:
-                # Parse the JSON response
+                # Parse the JSON responsee
                 self.status = response.json().get('status')
                 if self.status == 'ERR':
                     self.error_message = response.json().get('error_message')
                 if self.status == 'OK':
                     self.logged_in = True
                     self.access_token = response.json().get('access_token')
                     return self.access_token
             elif response.status_code >= 400 and response.status_code < 500:
                 self.status = 'ERR'
                 self.error_message = f"Client Error: {response.status_code}"
-                return {'status': self.status, 'error_message': self.error_message}
+                return None
             elif response.status_code == 500:
                 self.status = 'ERR'
                 self.error_message = 'Internal server error'
-                return {'status': self.status, 'error_message': self.error_message}
+                return None
             else:
                 self.status = 'ERR'
                 self.error_message = response.json().get('error_message')
                 # print(f"Failed to execute cmd: {command}. Status code: {response.status_code}")
                 return None
-                self.error_message = str(e)
         except requests.exceptions.RequestException as e:
             # Handle request exceptions such as network errors
             self.status = 'ERR'
             self.error_message = f"Request Exception: {e}"
             return None
         except ValueError as e:
             # Handle JSON parsing errors
@@ -95,17 +95,14 @@
         except Exception as e:
             # Catch any other unexpected exceptions
             self.status = 'ERR'
             self.error_message = f"An unexpected error occurred: {e}"
             return None
 
     def get_access_token(self):
-        if self.access_token is not None:
-            self.authenticateToken(self.access_token)
-
         return self.access_token
 
 
     def authenticate(self, username: str, password: str, type: str = 'permanent'):
         headers = {
             # ... (your headers for login)
         }
```

### Comparing `energiinfo-1.0.3/src/energiinfo/const.py` & `energiinfo-1.0.4/src/energiinfo/const.py`

 * *Files identical despite different names*

