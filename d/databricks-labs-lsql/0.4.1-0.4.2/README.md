# Comparing `tmp/databricks_labs_lsql-0.4.1.tar.gz` & `tmp/databricks_labs_lsql-0.4.2.tar.gz`

## Comparing `databricks_labs_lsql-0.4.1.tar` & `databricks_labs_lsql-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/databricks/labs/lsql/__about__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/databricks/labs/lsql/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/databricks/labs/lsql/__main__.py
--rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/databricks/labs/lsql/backends.py
--rw-r--r--   0        0        0    23637 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/databricks/labs/lsql/core.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/databricks/labs/lsql/deployment.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/databricks/labs/lsql/py.typed
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/LICENSE
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/NOTICE
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/README.md
--rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/__about__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/__main__.py
+-rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/backends.py
+-rw-r--r--   0        0        0    23725 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/core.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/deployment.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/py.typed
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/NOTICE
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/README.md
+-rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/PKG-INFO
```

### Comparing `databricks_labs_lsql-0.4.1/databricks/labs/lsql/backends.py` & `databricks_labs_lsql-0.4.2/databricks/labs/lsql/backends.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.1/databricks/labs/lsql/core.py` & `databricks_labs_lsql-0.4.2/databricks/labs/lsql/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,14 +444,16 @@
             error_message = ""
         if "SCHEMA_NOT_FOUND" in error_message:
             raise NotFound(error_message)
         if "TABLE_OR_VIEW_NOT_FOUND" in error_message:
             raise NotFound(error_message)
         if "DELTA_TABLE_NOT_FOUND" in error_message:
             raise NotFound(error_message)
+        if "does not exist" in error_message:
+            raise NotFound(error_message)
         if "DELTA_MISSING_TRANSACTION_LOG" in error_message:
             raise DataLoss(error_message)
         mapping = {
             ServiceErrorCode.ABORTED: errors.Aborted,
             ServiceErrorCode.ALREADY_EXISTS: errors.AlreadyExists,
             ServiceErrorCode.BAD_REQUEST: errors.BadRequest,
             ServiceErrorCode.CANCELLED: errors.Cancelled,
```

### Comparing `databricks_labs_lsql-0.4.1/databricks/labs/lsql/deployment.py` & `databricks_labs_lsql-0.4.2/databricks/labs/lsql/deployment.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.1/.gitignore` & `databricks_labs_lsql-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.1/LICENSE` & `databricks_labs_lsql-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.1/NOTICE` & `databricks_labs_lsql-0.4.2/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.1/README.md` & `databricks_labs_lsql-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.1/pyproject.toml` & `databricks_labs_lsql-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.1/PKG-INFO` & `databricks_labs_lsql-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-lsql
-Version: 0.4.1
+Version: 0.4.2
 Summary: Lightweight stateless SQL execution for Databricks with minimal dependencies
 Project-URL: Documentation, https://github.com/databrickslabs/lsql#readme
 Project-URL: Issues, https://github.com/databrickslabs/lsql/issues
 Project-URL: Source, https://github.com/databrickslabs/lsql
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
```

