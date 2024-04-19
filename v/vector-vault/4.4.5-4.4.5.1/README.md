# Comparing `tmp/vector_vault-4.4.5.tar.gz` & `tmp/vector_vault-4.4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.4.5.tar", last modified: Thu Apr 18 17:18:44 2024, max compression
+gzip compressed data, was "vector_vault-4.4.5.1.tar", last modified: Thu Apr 18 17:22:36 2024, max compression
```

## Comparing `vector_vault-4.4.5.tar` & `vector_vault-4.4.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-18 17:18:44.270296 vector_vault-4.4.5/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.5/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-18 17:18:44.270104 vector_vault-4.4.5/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.5/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-18 17:18:44.270332 vector_vault-4.4.5/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-18 17:18:30.000000 vector_vault-4.4.5/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-18 17:18:44.266519 vector_vault-4.4.5/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-18 17:18:44.000000 vector_vault-4.4.5/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-18 17:18:44.000000 vector_vault-4.4.5/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-18 17:18:44.000000 vector_vault-4.4.5/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-18 17:18:44.000000 vector_vault-4.4.5/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-18 17:18:44.000000 vector_vault-4.4.5/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-18 17:18:44.269794 vector_vault-4.4.5/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.5/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16841 2024-04-12 02:24:53.000000 vector_vault-4.4.5/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.5/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6046 2024-04-11 19:12:06.000000 vector_vault-4.4.5/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2024-04-11 18:02:55.000000 vector_vault-4.4.5/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.5/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.5/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    22962 2024-04-12 07:29:05.000000 vector_vault-4.4.5/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62579 2024-04-18 17:18:21.000000 vector_vault-4.4.5/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5421 2024-04-12 02:36:29.000000 vector_vault-4.4.5/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.5/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-18 17:22:36.001361 vector_vault-4.4.5.1/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.5.1/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-18 17:22:36.001191 vector_vault-4.4.5.1/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.5.1/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-18 17:22:36.001395 vector_vault-4.4.5.1/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-18 17:22:29.000000 vector_vault-4.4.5.1/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-18 17:22:35.999304 vector_vault-4.4.5.1/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-18 17:22:35.000000 vector_vault-4.4.5.1/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-18 17:22:35.000000 vector_vault-4.4.5.1/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-18 17:22:35.000000 vector_vault-4.4.5.1/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-18 17:22:35.000000 vector_vault-4.4.5.1/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-18 17:22:35.000000 vector_vault-4.4.5.1/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-18 17:22:36.001003 vector_vault-4.4.5.1/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.5.1/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16841 2024-04-12 02:24:53.000000 vector_vault-4.4.5.1/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.5.1/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6046 2024-04-11 19:12:06.000000 vector_vault-4.4.5.1/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2024-04-11 18:02:55.000000 vector_vault-4.4.5.1/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.5.1/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.5.1/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    22962 2024-04-12 07:29:05.000000 vector_vault-4.4.5.1/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62412 2024-04-18 17:21:28.000000 vector_vault-4.4.5.1/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5421 2024-04-12 02:36:29.000000 vector_vault-4.4.5.1/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.5.1/vectorvault/wrap.py
```

### Comparing `vector_vault-4.4.5/LICENSE` & `vector_vault-4.4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5/PKG-INFO` & `vector_vault-4.4.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.4.5
+Version: 4.4.5.1
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.5/README.md` & `vector_vault-4.4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5/setup.py` & `vector_vault-4.4.5.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.4.5",
+    version="4.4.5.1",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.4.5/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.4.5.1/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.4.5
+Version: 4.4.5.1
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.5/vectorvault/ai.py` & `vector_vault-4.4.5.1/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5/vectorvault/cloud_api.py` & `vector_vault-4.4.5.1/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5/vectorvault/cloudmanager.py` & `vector_vault-4.4.5.1/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5/vectorvault/creds.py` & `vector_vault-4.4.5.1/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5/vectorvault/download.py` & `vector_vault-4.4.5.1/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5/vectorvault/itemize.py` & `vector_vault-4.4.5.1/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5/vectorvault/tools_gpt.py` & `vector_vault-4.4.5.1/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.5/vectorvault/vault.py` & `vector_vault-4.4.5.1/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,20 +74,17 @@
         '''
         self.user = user.lower()
         self.vault = vault.strip() if vault else 'home'
         self.api = api_key
         self.verbose = verbose
         self.embeddings_model = embeddings_model if embeddings_model else 'text-embedding-3-small'
         self.dims = 1536 if embeddings_model != 'text-embedding-3-large' else 3072
-        try:
-            self.cloud_manager = CloudManager(self.user, self.api, self.vault)
-            if self.verbose:
-                print(f'Connected vault: {self.vault}')
-        except Exception as e:
-            print('API KEY NOT FOUND! You need an active Vector Vault API key in order to use the service', e)
+        self.cloud_manager = CloudManager(self.user, self.api, self.vault)
+        if self.verbose:
+            print(f'Connected vault: {self.vault}')
 
         if openai_key:
             self.openai_key = openai_key
             openai.api_key = self.openai_key
         self.vectors = get_vectors(self.dims)
         self.x = 0
         self.x_checked = False
```

### Comparing `vector_vault-4.4.5/vectorvault/vecreq.py` & `vector_vault-4.4.5.1/vectorvault/vecreq.py`

 * *Files identical despite different names*

