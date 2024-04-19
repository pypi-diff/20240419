# Comparing `tmp/vector_vault-4.4.5.3.tar.gz` & `tmp/vector_vault-4.4.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.4.5.3.tar", last modified: Fri Apr 19 03:20:03 2024, max compression
+gzip compressed data, was "vector_vault-4.4.5.4.tar", last modified: Fri Apr 19 03:23:50 2024, max compression
```

## Comparing `vector_vault-4.4.5.3.tar` & `vector_vault-4.4.5.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-19 03:20:03.659702 vector_vault-4.4.5.3/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.5.3/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-19 03:20:03.659548 vector_vault-4.4.5.3/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.5.3/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-19 03:20:03.659737 vector_vault-4.4.5.3/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-19 03:19:22.000000 vector_vault-4.4.5.3/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-19 03:20:03.657963 vector_vault-4.4.5.3/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-19 03:20:03.000000 vector_vault-4.4.5.3/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-19 03:20:03.000000 vector_vault-4.4.5.3/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-19 03:20:03.000000 vector_vault-4.4.5.3/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-19 03:20:03.000000 vector_vault-4.4.5.3/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-19 03:20:03.000000 vector_vault-4.4.5.3/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-19 03:20:03.659371 vector_vault-4.4.5.3/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.5.3/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16841 2024-04-12 02:24:53.000000 vector_vault-4.4.5.3/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.5.3/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6046 2024-04-11 19:12:06.000000 vector_vault-4.4.5.3/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2108 2024-04-19 03:19:14.000000 vector_vault-4.4.5.3/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.5.3/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.5.3/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    22962 2024-04-12 07:29:05.000000 vector_vault-4.4.5.3/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62412 2024-04-18 17:21:28.000000 vector_vault-4.4.5.3/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5421 2024-04-12 02:36:29.000000 vector_vault-4.4.5.3/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.5.3/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-19 03:23:50.912326 vector_vault-4.4.5.4/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.5.4/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-19 03:23:50.912182 vector_vault-4.4.5.4/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.5.4/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-19 03:23:50.912358 vector_vault-4.4.5.4/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-19 03:23:25.000000 vector_vault-4.4.5.4/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-19 03:23:50.909489 vector_vault-4.4.5.4/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-19 03:23:50.000000 vector_vault-4.4.5.4/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-19 03:23:50.000000 vector_vault-4.4.5.4/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-19 03:23:50.000000 vector_vault-4.4.5.4/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-19 03:23:50.000000 vector_vault-4.4.5.4/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-19 03:23:50.000000 vector_vault-4.4.5.4/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-19 03:23:50.912005 vector_vault-4.4.5.4/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.5.4/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16841 2024-04-12 02:24:53.000000 vector_vault-4.4.5.4/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.5.4/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6046 2024-04-11 19:12:06.000000 vector_vault-4.4.5.4/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2152 2024-04-19 03:22:48.000000 vector_vault-4.4.5.4/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.5.4/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.5.4/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    22962 2024-04-12 07:29:05.000000 vector_vault-4.4.5.4/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62412 2024-04-18 17:21:28.000000 vector_vault-4.4.5.4/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5421 2024-04-12 02:36:29.000000 vector_vault-4.4.5.4/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.5.4/vectorvault/wrap.py
```

### Comparing `vector_vault-4.4.5.3/LICENSE` & `vector_vault-4.4.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5.3/PKG-INFO` & `vector_vault-4.4.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.4.5.3
+Version: 4.4.5.4
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.5.3/README.md` & `vector_vault-4.4.5.4/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5.3/setup.py` & `vector_vault-4.4.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.4.5.3",
+    version="4.4.5.4",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.4.5.3/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.4.5.4/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.4.5.3
+Version: 4.4.5.4
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.5.3/vectorvault/ai.py` & `vector_vault-4.4.5.4/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5.3/vectorvault/cloud_api.py` & `vector_vault-4.4.5.4/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5.3/vectorvault/cloudmanager.py` & `vector_vault-4.4.5.4/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5.3/vectorvault/creds.py` & `vector_vault-4.4.5.4/vectorvault/creds.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class CustomCredentials(Credentials):
     def __init__(self, user, api):
         self.user = user
         self.api = api
         self.token = None
         self.expiry = None
-        self._universe_domain = None
+        self._universe_domain = "https://www.googleapis.com/auth/cloud-platform"
         self.refresh(requests.Request())
 
     @property
     def universe_domain(self):
         return self._universe_domain
 
     @universe_domain.setter
```

### Comparing `vector_vault-4.4.5.3/vectorvault/download.py` & `vector_vault-4.4.5.4/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5.3/vectorvault/itemize.py` & `vector_vault-4.4.5.4/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5.3/vectorvault/tools_gpt.py` & `vector_vault-4.4.5.4/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5.3/vectorvault/vault.py` & `vector_vault-4.4.5.4/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5.3/vectorvault/vecreq.py` & `vector_vault-4.4.5.4/vectorvault/vecreq.py`

 * *Files identical despite different names*

