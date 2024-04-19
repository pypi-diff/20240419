# Comparing `tmp/shipyard_googlecloud-0.2.0a0.tar.gz` & `tmp/shipyard_googlecloud-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_googlecloud-0.2.0a0.tar", max compression
+gzip compressed data, was "shipyard_googlecloud-0.2.0a1.tar", max compression
```

## Comparing `shipyard_googlecloud-0.2.0a0.tar` & `shipyard_googlecloud-0.2.0a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.831133 shipyard_googlecloud-0.2.0a0/README.md
--rw-r--r--   0        0        0      625 2024-04-10 16:50:44.088720 shipyard_googlecloud-0.2.0a0/pyproject.toml
--rw-r--r--   0        0        0       43 2023-05-12 18:48:21.831530 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.436211 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/__init__.py
--rw-r--r--   0        0        0      539 2024-03-25 01:03:55.080367 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/authtest.py
--rw-r--r--   0        0        0     5290 2024-04-01 15:54:40.971130 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/download.py
--rw-r--r--   0        0        0     6224 2024-03-25 01:03:55.081223 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/move.py
--rw-r--r--   0        0        0     3460 2024-03-25 01:03:55.081667 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/remove.py
--rw-r--r--   0        0        0     4377 2024-03-25 01:03:55.082080 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/upload.py
--rw-r--r--   0        0        0     1066 2024-03-25 01:03:55.082389 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/googlecloud.py
--rw-r--r--   0        0        0     3262 2024-04-10 16:42:37.478377 shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/utils.py
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 shipyard_googlecloud-0.2.0a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.831133 shipyard_googlecloud-0.2.0a1/README.md
+-rw-r--r--   0        0        0      625 2024-04-10 17:33:20.446069 shipyard_googlecloud-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-05-12 18:48:21.831530 shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.436211 shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/__init__.py
+-rw-r--r--   0        0        0      539 2024-04-10 17:03:26.878304 shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/authtest.py
+-rw-r--r--   0        0        0     5153 2024-04-10 17:33:13.568788 shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/download.py
+-rw-r--r--   0        0        0     6224 2024-04-10 17:03:26.879931 shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/move.py
+-rw-r--r--   0        0        0     3460 2024-04-10 17:03:26.880896 shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/remove.py
+-rw-r--r--   0        0        0     4377 2024-04-10 17:03:26.881869 shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/upload.py
+-rw-r--r--   0        0        0     1066 2024-04-10 17:03:26.882507 shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/googlecloud.py
+-rw-r--r--   0        0        0     3262 2024-04-10 16:42:37.478377 shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/utils.py
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 shipyard_googlecloud-0.2.0a1/PKG-INFO
```

### Comparing `shipyard_googlecloud-0.2.0a0/pyproject.toml` & `shipyard_googlecloud-0.2.0a1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "shipyard-googlecloud"
-version = "0.2.0a0"
+version = "0.2.0a1"
 description = "A local client for connecting and working with Google Cloud Service"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_googlecloud" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
 httplib2 = "0.15.0"
-shipyard-bp-utils = "^1.1.1"
 google-cloud-storage = "^2.15.0"
+shipyard-bp-utils = "^1.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.0"
 pytest = "^8.1.1"
 faker = "^24.2.0"
 pyfakefs = "^5.3.5"
```

### Comparing `shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/authtest.py` & `shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/download.py` & `shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,20 +83,17 @@
         )
         if destination_folder_name:
             shipyard.create_folder_if_dne(destination_folder_name)
 
         bucket = utils.get_bucket(gclient=gclient, bucket_name=bucket_name)
 
         if args.source_file_name_match_type == "exact_match":
-
             source_full_path = shipyard.combine_folder_and_file_name(
                 folder_name=source_folder_name, file_name=source_file_name
             )
-            if not os.path.exists(source_full_path):
-                raise FileNotFoundError(f"File {source_full_path} does not exist")
 
             blob = utils.get_storage_blob(
                 bucket=bucket,
                 source_folder_name=source_folder_name,
                 source_file_name=source_file_name,
             )
             destination_name = shipyard.determine_destination_full_path(
```

### Comparing `shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/move.py` & `shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/move.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/remove.py` & `shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/remove.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/cli/upload.py` & `shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/googlecloud.py` & `shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlecloud-0.2.0a0/shipyard_googlecloud/utils.py` & `shipyard_googlecloud-0.2.0a1/shipyard_googlecloud/utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_googlecloud-0.2.0a0/PKG-INFO` & `shipyard_googlecloud-0.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: shipyard-googlecloud
-Version: 0.2.0a0
+Version: 0.2.0a1
 Summary: A local client for connecting and working with Google Cloud Service
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: google-cloud-storage (>=2.15.0,<3.0.0)
 Requires-Dist: httplib2 (==0.15.0)
-Requires-Dist: shipyard-bp-utils (>=1.1.1,<2.0.0)
+Requires-Dist: shipyard-bp-utils (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
```

