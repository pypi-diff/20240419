# Comparing `tmp/pytmlr-0.0.3rc0.tar.gz` & `tmp/pytmlr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmlr-0.0.3rc0.tar", last modified: Wed Mar 27 03:15:16 2024, max compression
+gzip compressed data, was "pytmlr-0.0.4.tar", last modified: Fri Apr 19 21:08:37 2024, max compression
```

## Comparing `pytmlr-0.0.3rc0.tar` & `pytmlr-0.0.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-03-27 03:15:16.520553 pytmlr-0.0.3rc0/
--rw-r--r--   0 lz        (1000) lz        (1000)      436 2024-03-27 03:15:16.520553 pytmlr-0.0.3rc0/PKG-INFO
--rwxr-xr-x   0 lz        (1000) lz        (1000)     1166 2024-01-08 09:06:10.000000 pytmlr-0.0.3rc0/pyproject.toml
-drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-03-27 03:15:16.516553 pytmlr-0.0.3rc0/pyt/
--rwxr-xr-x   0 lz        (1000) lz        (1000)      111 2023-09-09 17:39:54.000000 pytmlr-0.0.3rc0/pyt/__init__.py
-drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-03-27 03:15:16.516553 pytmlr-0.0.3rc0/pyt/data/
--rwxr-xr-x   0 lz        (1000) lz        (1000)       54 2023-08-27 04:48:17.000000 pytmlr-0.0.3rc0/pyt/data/__init__.py
-drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-03-27 03:15:16.516553 pytmlr-0.0.3rc0/pyt/data/api_alignments/
--rwxr-xr-x   0 lz        (1000) lz        (1000)     6315 2023-06-03 02:45:31.000000 pytmlr-0.0.3rc0/pyt/data/api_alignments/align_np_torch copy.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)    22577 2023-06-20 22:54:22.000000 pytmlr-0.0.3rc0/pyt/data/api_alignments/align_np_torch.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     8653 2023-06-20 23:05:21.000000 pytmlr-0.0.3rc0/pyt/data/api_alignments/parse_parameters.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)       35 2023-06-03 06:32:28.000000 pytmlr-0.0.3rc0/pyt/data/api_alignments/test_np.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)       69 2023-06-03 03:22:37.000000 pytmlr-0.0.3rc0/pyt/data/api_alignments/unified_data.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     1022 2023-11-24 23:31:24.000000 pytmlr-0.0.3rc0/pyt/data/string_utils.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     3585 2023-08-27 04:47:42.000000 pytmlr-0.0.3rc0/pyt/data/type_utils.py
-drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-03-27 03:15:16.516553 pytmlr-0.0.3rc0/pyt/fileio/
--rwxr-xr-x   0 lz        (1000) lz        (1000)      189 2023-08-27 04:51:54.000000 pytmlr-0.0.3rc0/pyt/fileio/__init__.py
-drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-03-27 03:15:16.520553 pytmlr-0.0.3rc0/pyt/fileio/handlers/
--rwxr-xr-x   0 lz        (1000) lz        (1000)      298 2023-11-08 01:07:07.000000 pytmlr-0.0.3rc0/pyt/fileio/handlers/__init__.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)      652 2023-06-02 21:58:19.000000 pytmlr-0.0.3rc0/pyt/fileio/handlers/csv_handler.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     1153 2023-05-29 21:05:36.000000 pytmlr-0.0.3rc0/pyt/fileio/handlers/image_handler.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)      583 2023-06-06 02:07:27.000000 pytmlr-0.0.3rc0/pyt/fileio/handlers/jsonl_handler.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)      464 2023-05-29 20:35:57.000000 pytmlr-0.0.3rc0/pyt/fileio/handlers/npy_handler.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     1018 2023-05-29 20:49:04.000000 pytmlr-0.0.3rc0/pyt/fileio/handlers/pickle_handler.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)      967 2023-11-08 01:09:44.000000 pytmlr-0.0.3rc0/pyt/fileio/handlers/tensor_handler.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)      394 2023-05-29 21:13:34.000000 pytmlr-0.0.3rc0/pyt/fileio/handlers/txt_handler.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)      119 2023-09-10 05:51:45.000000 pytmlr-0.0.3rc0/pyt/fileio/serialization.py
-drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-03-27 03:15:16.520553 pytmlr-0.0.3rc0/pyt/meta/
--rwxr-xr-x   0 lz        (1000) lz        (1000)      121 2023-08-27 23:54:05.000000 pytmlr-0.0.3rc0/pyt/meta/__init__.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     1160 2023-08-27 23:53:55.000000 pytmlr-0.0.3rc0/pyt/meta/hash_utils.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)      325 2023-06-23 21:17:12.000000 pytmlr-0.0.3rc0/pyt/meta/network_utils.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     2117 2023-12-05 02:48:47.000000 pytmlr-0.0.3rc0/pyt/meta/process_utils.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     1057 2023-09-09 06:29:55.000000 pytmlr-0.0.3rc0/pyt/meta/time_utils.py
-drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-03-27 03:15:16.520553 pytmlr-0.0.3rc0/pyt/misc/
--rwxr-xr-x   0 lz        (1000) lz        (1000)       47 2023-08-27 04:54:17.000000 pytmlr-0.0.3rc0/pyt/misc/__init__.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     3482 2024-03-27 03:03:30.000000 pytmlr-0.0.3rc0/pyt/misc/dict_database.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     2909 2023-08-27 04:35:42.000000 pytmlr-0.0.3rc0/pyt/misc/git_utils.py
-drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-03-27 03:15:16.520553 pytmlr-0.0.3rc0/pyt/visualization/
--rwxr-xr-x   0 lz        (1000) lz        (1000)      274 2023-08-27 20:48:48.000000 pytmlr-0.0.3rc0/pyt/visualization/__init__.py
--rwxr-xr-x   0 lz        (1000) lz        (1000)     8906 2023-09-28 23:54:14.000000 pytmlr-0.0.3rc0/pyt/visualization/matplotlib_utils.py
-drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-03-27 03:15:16.520553 pytmlr-0.0.3rc0/pytmlr.egg-info/
--rw-r--r--   0 lz        (1000) lz        (1000)      436 2024-03-27 03:15:16.000000 pytmlr-0.0.3rc0/pytmlr.egg-info/PKG-INFO
--rwxr-xr-x   0 lz        (1000) lz        (1000)     1050 2024-03-27 03:15:16.000000 pytmlr-0.0.3rc0/pytmlr.egg-info/SOURCES.txt
--rwxr-xr-x   0 lz        (1000) lz        (1000)        1 2024-03-27 03:15:16.000000 pytmlr-0.0.3rc0/pytmlr.egg-info/dependency_links.txt
--rwxr-xr-x   0 lz        (1000) lz        (1000)       42 2024-03-27 03:15:16.000000 pytmlr-0.0.3rc0/pytmlr.egg-info/requires.txt
--rwxr-xr-x   0 lz        (1000) lz        (1000)        4 2024-03-27 03:15:16.000000 pytmlr-0.0.3rc0/pytmlr.egg-info/top_level.txt
--rw-rw-r--   0 lz        (1000) lz        (1000)       38 2024-03-27 03:15:16.520553 pytmlr-0.0.3rc0/setup.cfg
+drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-04-19 21:08:37.548706 pytmlr-0.0.4/
+-rw-r--r--   0 lz        (1000) lz        (1000)      433 2024-04-19 21:08:37.548706 pytmlr-0.0.4/PKG-INFO
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     1165 2024-04-19 21:08:34.000000 pytmlr-0.0.4/pyproject.toml
+drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-04-19 21:08:37.544706 pytmlr-0.0.4/pyt/
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      111 2023-09-09 17:39:54.000000 pytmlr-0.0.4/pyt/__init__.py
+drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-04-19 21:08:37.544706 pytmlr-0.0.4/pyt/data/
+-rwxr-xr-x   0 lz        (1000) lz        (1000)       54 2023-08-27 04:48:17.000000 pytmlr-0.0.4/pyt/data/__init__.py
+drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-04-19 21:08:37.544706 pytmlr-0.0.4/pyt/data/api_alignments/
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     6315 2023-06-03 02:45:31.000000 pytmlr-0.0.4/pyt/data/api_alignments/align_np_torch copy.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)    22577 2023-06-20 22:54:22.000000 pytmlr-0.0.4/pyt/data/api_alignments/align_np_torch.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     8653 2023-06-20 23:05:21.000000 pytmlr-0.0.4/pyt/data/api_alignments/parse_parameters.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)       35 2023-06-03 06:32:28.000000 pytmlr-0.0.4/pyt/data/api_alignments/test_np.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)       69 2023-06-03 03:22:37.000000 pytmlr-0.0.4/pyt/data/api_alignments/unified_data.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     1022 2023-11-24 23:31:24.000000 pytmlr-0.0.4/pyt/data/string_utils.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     3585 2023-08-27 04:47:42.000000 pytmlr-0.0.4/pyt/data/type_utils.py
+drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-04-19 21:08:37.544706 pytmlr-0.0.4/pyt/fileio/
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      189 2023-08-27 04:51:54.000000 pytmlr-0.0.4/pyt/fileio/__init__.py
+drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-04-19 21:08:37.548706 pytmlr-0.0.4/pyt/fileio/handlers/
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      298 2023-11-08 01:07:07.000000 pytmlr-0.0.4/pyt/fileio/handlers/__init__.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      652 2023-06-02 21:58:19.000000 pytmlr-0.0.4/pyt/fileio/handlers/csv_handler.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     1153 2023-05-29 21:05:36.000000 pytmlr-0.0.4/pyt/fileio/handlers/image_handler.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      583 2023-06-06 02:07:27.000000 pytmlr-0.0.4/pyt/fileio/handlers/jsonl_handler.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      464 2023-05-29 20:35:57.000000 pytmlr-0.0.4/pyt/fileio/handlers/npy_handler.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     1018 2023-05-29 20:49:04.000000 pytmlr-0.0.4/pyt/fileio/handlers/pickle_handler.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      967 2023-11-08 01:09:44.000000 pytmlr-0.0.4/pyt/fileio/handlers/tensor_handler.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      394 2023-05-29 21:13:34.000000 pytmlr-0.0.4/pyt/fileio/handlers/txt_handler.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      119 2023-09-10 05:51:45.000000 pytmlr-0.0.4/pyt/fileio/serialization.py
+drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-04-19 21:08:37.548706 pytmlr-0.0.4/pyt/meta/
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      121 2023-08-27 23:54:05.000000 pytmlr-0.0.4/pyt/meta/__init__.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     1160 2023-08-27 23:53:55.000000 pytmlr-0.0.4/pyt/meta/hash_utils.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      325 2023-06-23 21:17:12.000000 pytmlr-0.0.4/pyt/meta/network_utils.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     2117 2023-12-05 02:48:47.000000 pytmlr-0.0.4/pyt/meta/process_utils.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     1057 2023-09-09 06:29:55.000000 pytmlr-0.0.4/pyt/meta/time_utils.py
+drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-04-19 21:08:37.548706 pytmlr-0.0.4/pyt/misc/
+-rwxr-xr-x   0 lz        (1000) lz        (1000)       47 2023-08-27 04:54:17.000000 pytmlr-0.0.4/pyt/misc/__init__.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     4050 2024-04-19 19:05:38.000000 pytmlr-0.0.4/pyt/misc/dict_database.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     2909 2023-08-27 04:35:42.000000 pytmlr-0.0.4/pyt/misc/git_utils.py
+drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-04-19 21:08:37.548706 pytmlr-0.0.4/pyt/visualization/
+-rwxr-xr-x   0 lz        (1000) lz        (1000)      274 2023-08-27 20:48:48.000000 pytmlr-0.0.4/pyt/visualization/__init__.py
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     8906 2023-09-28 23:54:14.000000 pytmlr-0.0.4/pyt/visualization/matplotlib_utils.py
+drwxrwxr-x   0 lz        (1000) lz        (1000)        0 2024-04-19 21:08:37.548706 pytmlr-0.0.4/pytmlr.egg-info/
+-rw-r--r--   0 lz        (1000) lz        (1000)      433 2024-04-19 21:08:37.000000 pytmlr-0.0.4/pytmlr.egg-info/PKG-INFO
+-rwxr-xr-x   0 lz        (1000) lz        (1000)     1050 2024-04-19 21:08:37.000000 pytmlr-0.0.4/pytmlr.egg-info/SOURCES.txt
+-rwxr-xr-x   0 lz        (1000) lz        (1000)        1 2024-04-19 21:08:37.000000 pytmlr-0.0.4/pytmlr.egg-info/dependency_links.txt
+-rwxr-xr-x   0 lz        (1000) lz        (1000)       42 2024-04-19 21:08:37.000000 pytmlr-0.0.4/pytmlr.egg-info/requires.txt
+-rwxr-xr-x   0 lz        (1000) lz        (1000)        4 2024-04-19 21:08:37.000000 pytmlr-0.0.4/pytmlr.egg-info/top_level.txt
+-rw-rw-r--   0 lz        (1000) lz        (1000)       38 2024-04-19 21:08:37.548706 pytmlr-0.0.4/setup.cfg
```

### Comparing `pytmlr-0.0.3rc0/pyproject.toml` & `pytmlr-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pytmlr"
 description = "A useful tool for machine learning research."
-version = "0.0.3c"
+version = "0.0.4"
 authors = [
     { name = "Zhan Ling", email = "z6ling@ucsd.edu" }
 ]
 requires-python = ">=3.10"
 dependencies = [
     "mmengine",
     "numpy",
```

### Comparing `pytmlr-0.0.3rc0/pyt/data/api_alignments/align_np_torch copy.py` & `pytmlr-0.0.4/pyt/data/api_alignments/align_np_torch copy.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/data/api_alignments/align_np_torch.py` & `pytmlr-0.0.4/pyt/data/api_alignments/align_np_torch.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/data/api_alignments/parse_parameters.py` & `pytmlr-0.0.4/pyt/data/api_alignments/parse_parameters.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/data/string_utils.py` & `pytmlr-0.0.4/pyt/data/string_utils.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/data/type_utils.py` & `pytmlr-0.0.4/pyt/data/type_utils.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/fileio/handlers/csv_handler.py` & `pytmlr-0.0.4/pyt/fileio/handlers/csv_handler.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/fileio/handlers/image_handler.py` & `pytmlr-0.0.4/pyt/fileio/handlers/image_handler.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/fileio/handlers/jsonl_handler.py` & `pytmlr-0.0.4/pyt/fileio/handlers/jsonl_handler.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/fileio/handlers/pickle_handler.py` & `pytmlr-0.0.4/pyt/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/fileio/handlers/tensor_handler.py` & `pytmlr-0.0.4/pyt/fileio/handlers/tensor_handler.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/meta/hash_utils.py` & `pytmlr-0.0.4/pyt/meta/hash_utils.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/meta/process_utils.py` & `pytmlr-0.0.4/pyt/meta/process_utils.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/meta/time_utils.py` & `pytmlr-0.0.4/pyt/meta/time_utils.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/misc/dict_database.py` & `pytmlr-0.0.4/pyt/misc/dict_database.py`

 * *Files 22% similar despite different names*

```diff
@@ -52,17 +52,19 @@
     def to_str_key(cls, key):
         return str(key)
     
     def check_exist(self, key):
         key = self.to_str_key(key)
         return self.session.query(self.table.key).filter_by(key=key).first() is not None
 
-    def get(self, key):
-        key = self.to_str_key(key)
-        return self.__getitem__(key)
+    def batch_check_exist(self, keys):
+        keys = [self.to_str_key(key) for key in keys]
+        results = self.session.query(self.table.key).filter(self.table.key.in_(keys)).all()
+        found_keys = set(result[0] for result in results)
+        return [key in found_keys for key in keys]
 
     def get_full(self, key):
         key = self.to_str_key(key)
         item = self.session.query(self.table).filter_by(key=key).first()
         return deserialize(item.value), deserialize(item.version), item.last_modified
 
     def set(self, key, value, version=None, flush=True):
@@ -85,14 +87,23 @@
         self.session.commit()
 
     def __getitem__(self, key):
         key = self.to_str_key(key)
         if not self.check_exist(key):
             return None
         return deserialize(self.session.query(self.table).filter_by(key=key).first().value)
+    
+    def get(self, key):
+        return self.__getitem__(key)
+    
+    def batch_get(self, keys):
+        keys = [self.to_str_key(key) for key in keys]
+        results = self.session.query(self.table).filter(self.table.key.in_(keys)).all()
+        results = {result.key: deserialize(result.value) for result in results}
+        return [results[key] for key in keys]
 
     def __contains__(self, key):
         key = self.to_str_key(key)
         return self.check_exist(key)
     
     def __setitem__(self, key, value):
         key = self.to_str_key(key)
```

### Comparing `pytmlr-0.0.3rc0/pyt/misc/git_utils.py` & `pytmlr-0.0.4/pyt/misc/git_utils.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pyt/visualization/matplotlib_utils.py` & `pytmlr-0.0.4/pyt/visualization/matplotlib_utils.py`

 * *Files identical despite different names*

### Comparing `pytmlr-0.0.3rc0/pytmlr.egg-info/SOURCES.txt` & `pytmlr-0.0.4/pytmlr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

