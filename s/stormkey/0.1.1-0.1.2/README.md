# Comparing `tmp/stormkey-0.1.1.tar.gz` & `tmp/stormkey-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stormkey-0.1.1.tar", last modified: Fri Apr 19 19:18:56 2024, max compression
+gzip compressed data, was "stormkey-0.1.2.tar", last modified: Fri Apr 19 19:42:07 2024, max compression
```

## Comparing `stormkey-0.1.1.tar` & `stormkey-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:18:56.036666 stormkey-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 19:18:40.000000 stormkey-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-19 19:18:56.036666 stormkey-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 19:18:40.000000 stormkey-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:18:56.036666 stormkey-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 19:18:40.000000 stormkey-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:18:56.036666 stormkey-0.1.1/stormkey/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 19:18:40.000000 stormkey-0.1.1/stormkey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-19 19:18:40.000000 stormkey-0.1.1/stormkey/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:18:56.036666 stormkey-0.1.1/stormkey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-19 19:18:55.000000 stormkey-0.1.1/stormkey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 19:18:56.000000 stormkey-0.1.1/stormkey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:18:55.000000 stormkey-0.1.1/stormkey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 19:18:55.000000 stormkey-0.1.1/stormkey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:07.721714 stormkey-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 19:41:51.000000 stormkey-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-19 19:42:07.721714 stormkey-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 19:41:51.000000 stormkey-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:42:07.721714 stormkey-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 19:41:51.000000 stormkey-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:07.721714 stormkey-0.1.2/stormkey/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 19:41:51.000000 stormkey-0.1.2/stormkey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-19 19:41:51.000000 stormkey-0.1.2/stormkey/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:07.721714 stormkey-0.1.2/stormkey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-19 19:42:07.000000 stormkey-0.1.2/stormkey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 19:42:07.000000 stormkey-0.1.2/stormkey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:42:07.000000 stormkey-0.1.2/stormkey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 19:42:07.000000 stormkey-0.1.2/stormkey.egg-info/top_level.txt
```

### Comparing `stormkey-0.1.1/LICENSE` & `stormkey-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stormkey-0.1.1/PKG-INFO` & `stormkey-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: stormkey
-Version: 0.1.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Stormkey
 
 ## Introduction
 
 Stormkey is a Python library that provides a convenient interface for managing API keys for your applications. Whether you need to create, update, verify, or delete API keys, Stormkey simplifies the process with easy-to-use methods.
 
 ## Installation
```

### Comparing `stormkey-0.1.1/README.md` & `stormkey-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: stormkey
+Version: 0.1.2
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Stormkey
 
 ## Introduction
 
 Stormkey is a Python library that provides a convenient interface for managing API keys for your applications. Whether you need to create, update, verify, or delete API keys, Stormkey simplifies the process with easy-to-use methods.
 
 ## Installation
```

### Comparing `stormkey-0.1.1/stormkey/main.py` & `stormkey-0.1.2/stormkey/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
     def create(self, name:str, ownerId:str):
         data = json.dumps({"name": name, "ownerId": ownerId})
 
         response = requests.post(f"{self.host}/api/v1/apps/{self.appId}/keys", data = data, headers = self.headers)
         return response.json()["key"]
 
-    def update(self, name:str, ownerId:str):
+    def update(self, key_id:str, name:str, ownerId: str):
         data = json.dumps({"name": name, "ownerId": ownerId})
 
-        response = requests.patch(f"{self.host}/api/v1/apps/{self.appId}/keys", data = data, headers = self.headers)
+        response = requests.patch(f"{self.host}/api/v1/apps/{self.appId}/keys/{key_id}", data = data, headers = self.headers)
+        return response.json()["key"]
+
+    def delete(self, key_id:str, name:str):
+        data = json.dumps({"name": name})
+
+        response = requests.delete(f"{self.host}/api/v1/apps/{self.appId}/keys/{key_id}", data = data, headers = self.headers)
         return response.json()["key"]
     
     def verify(self, key:str):
         data = json.dumps({"key": key})
 
         response = requests.post(f"{self.host}/api/v1/apps/{self.appId}/keys/verify", data = data, headers = self.headers)
-        return response.json()
-
-    def delete(self, name:str):
-        data = json.dumps({"name": name})
-
-        response = requests.delete(f"{self.host}/api/v1/apps/{self.appId}/keys", data = data, headers = self.headers)
-        return response.json()["key"]
+        return response.json()
```

### Comparing `stormkey-0.1.1/stormkey.egg-info/PKG-INFO` & `stormkey-0.1.2/stormkey.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormkey
-Version: 0.1.1
+Version: 0.1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Stormkey
 
 ## Introduction
```

