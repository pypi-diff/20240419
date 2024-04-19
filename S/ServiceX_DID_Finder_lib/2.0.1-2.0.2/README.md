# Comparing `tmp/servicex_did_finder_lib-2.0.1.tar.gz` & `tmp/servicex_did_finder_lib-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex_did_finder_lib-2.0.1.tar", max compression
+gzip compressed data, was "servicex_did_finder_lib-2.0.2.tar", max compression
```

## Comparing `servicex_did_finder_lib-2.0.1.tar` & `servicex_did_finder_lib-2.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11324 2024-01-11 17:31:06.275554 servicex_did_finder_lib-2.0.1/LICENSE
--rw-r--r--   0        0        0      556 2024-01-11 17:31:18.235558 servicex_did_finder_lib-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      113 2024-01-11 17:31:06.275554 servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/__init__.py
--rw-r--r--   0        0        0     9496 2024-01-11 17:31:06.275554 servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/communication.py
--rw-r--r--   0        0        0     1537 2024-01-11 17:31:06.275554 servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/did_logging.py
--rw-r--r--   0        0        0     3558 2024-01-11 17:31:06.275554 servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/did_summary.py
--rw-r--r--   0        0        0     4963 2024-01-11 17:31:06.275554 servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/servicex_adaptor.py
--rw-r--r--   0        0        0     1817 2024-01-11 17:31:06.275554 servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/util_uri.py
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 servicex_did_finder_lib-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-19 06:23:57.854448 servicex_did_finder_lib-2.0.2/LICENSE
+-rw-r--r--   0        0        0      556 2024-04-19 06:24:14.702579 servicex_did_finder_lib-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-04-19 06:23:57.854448 servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/__init__.py
+-rw-r--r--   0        0        0     9496 2024-04-19 06:23:57.854448 servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/communication.py
+-rw-r--r--   0        0        0     1537 2024-04-19 06:23:57.854448 servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/did_logging.py
+-rw-r--r--   0        0        0     3558 2024-04-19 06:23:57.854448 servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/did_summary.py
+-rw-r--r--   0        0        0     4964 2024-04-19 06:23:57.854448 servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/servicex_adaptor.py
+-rw-r--r--   0        0        0     1817 2024-04-19 06:23:57.854448 servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/util_uri.py
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 servicex_did_finder_lib-2.0.2/PKG-INFO
```

### Comparing `servicex_did_finder_lib-2.0.1/LICENSE` & `servicex_did_finder_lib-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex_did_finder_lib-2.0.1/pyproject.toml` & `servicex_did_finder_lib-2.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ServiceX_DID_Finder_lib"
-version = "2.0.1"
+version = "2.0.2"
 description = "ServiceX DID Library Routines"
 authors = ["Gordon Watts <gwatts@uw.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pika = "1.1.0"
 make-it-sync = "^1.0.0"
```

### Comparing `servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/communication.py` & `servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/communication.py`

 * *Files identical despite different names*

### Comparing `servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/did_logging.py` & `servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/did_logging.py`

 * *Files identical despite different names*

### Comparing `servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/did_summary.py` & `servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/did_summary.py`

 * *Files identical despite different names*

### Comparing `servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/servicex_adaptor.py` & `servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/servicex_adaptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 self.logger.exception(f'Connection error to ServiceX App. Will retry '
                                       f'(try {attempts} out of {MAX_RETRIES}')
                 attempts += 1
         if not success:
             self.logger.error(f'After {attempts} tries, failed to send ServiceX App a put_file '
                               f'message: {str(file_info)} - Ignoring error.')
 
-    def put_file_add_bulk(self, file_list, chunk_length=30):
+    def put_file_add_bulk(self, file_list, chunk_length=300):
         # we first chunk up file_list as it can be very large in
         # case there are a lot of replicas and a lot of files.
         chunks = [file_list[i:i + chunk_length] for i in range(0, len(file_list), chunk_length)]
         for chunk in chunks:
             success = False
             attempts = 0
             mesg = []
```

### Comparing `servicex_did_finder_lib-2.0.1/src/servicex_did_finder_lib/util_uri.py` & `servicex_did_finder_lib-2.0.2/src/servicex_did_finder_lib/util_uri.py`

 * *Files identical despite different names*

### Comparing `servicex_did_finder_lib-2.0.1/PKG-INFO` & `servicex_did_finder_lib-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ServiceX_DID_Finder_lib
-Version: 2.0.1
+Version: 2.0.2
 Summary: ServiceX DID Library Routines
 Author: Gordon Watts
 Author-email: gwatts@uw.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

