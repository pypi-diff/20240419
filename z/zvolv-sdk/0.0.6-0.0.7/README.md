# Comparing `tmp/zvolv_sdk-0.0.6.tar.gz` & `tmp/zvolv_sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zvolv_sdk-0.0.6.tar", last modified: Fri Apr 19 05:51:31 2024, max compression
+gzip compressed data, was "zvolv_sdk-0.0.7.tar", last modified: Fri Apr 19 07:16:22 2024, max compression
```

## Comparing `zvolv_sdk-0.0.6.tar` & `zvolv_sdk-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.291911 zvolv_sdk-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.291911 zvolv_sdk-0.0.6/src/devide/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/src/devide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/src/devide/divide_by_three.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.291911 zvolv_sdk-0.0.6/src/zvolv_client/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/src/zvolv_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/src/zvolv_client/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/tests/test_divide_by_three.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/zvolv_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/common_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/zvolv_sdk/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/modules/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/server_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/user_defined_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/zvolv_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/zvolv_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 05:51:31.000000 zvolv_sdk-0.0.6/zvolv_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-19 05:51:31.000000 zvolv_sdk-0.0.6/zvolv_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:51:31.000000 zvolv_sdk-0.0.6/zvolv_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 05:51:31.000000 zvolv_sdk-0.0.6/zvolv_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/tests/test_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/zvolv_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/zvolv_sdk/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/modules/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/modules/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/server_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 07:16:18.000000 zvolv_sdk-0.0.7/zvolv_sdk/zvolv_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:16:22.755703 zvolv_sdk-0.0.7/zvolv_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 07:16:22.000000 zvolv_sdk-0.0.7/zvolv_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-19 07:16:22.000000 zvolv_sdk-0.0.7/zvolv_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:16:22.000000 zvolv_sdk-0.0.7/zvolv_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 07:16:22.000000 zvolv_sdk-0.0.7/zvolv_sdk.egg-info/top_level.txt
```

### Comparing `zvolv_sdk-0.0.6/LICENSE` & `zvolv_sdk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.6/setup.py` & `zvolv_sdk-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.6/src/zvolv_client/auth.py` & `zvolv_sdk-0.0.7/zvolv_sdk/modules/auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import requests
+import hashlib
 
 class Auth:
     def __init__(self, session, base_url):
         self.session = session
         self.base_url = base_url
 
     def login(self, email, password):
         """Authenticate a user and store their auth token."""
         url = f"{self.base_url}/rest/v17/user/login"
-        data = {'email': email, 'password': password}
+        sha512pwd = hashlib.sha512(password.encode('utf-8')).hexdigest()
+        data = {'email': email, 'password': sha512pwd}
         response = self.session.post(url, json=data, headers={'Content-Type': 'application/json', 'jwt': True,
         'businessDomain': 'kapilwf', 'businessTagId' : '449VZ2DY54AF3'})
         if response.status_code == 200:
-            print("Login Successful")
-            print(response.json())
-            self.session.headers.update({'Authorization': f"Bearer {response.json()['token']}"})
+            resp = response.json()
+            if resp.get('error') == False:
+                token = resp['loginToken']
+                self.session.headers.update({'Authorization': f"Bearer {token}"})
+                print(self.session.headers)
+            else:
+                print("Login Failed")
+                print(response.json())
+
         return response.json()
```

### Comparing `zvolv_sdk-0.0.6/zvolv_sdk/server_configuration.py` & `zvolv_sdk-0.0.7/zvolv_sdk/server_configuration.py`

 * *Files identical despite different names*

