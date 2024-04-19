# Comparing `tmp/dagster-pipes-1.7.2rc2.tar.gz` & `tmp/dagster-pipes-1.7.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pipes-1.7.2rc2.tar", last modified: Tue Apr 16 20:27:47 2024, max compression
+gzip compressed data, was "dagster-pipes-1.7.2rc3.tar", last modified: Thu Apr 18 21:10:56 2024, max compression
```

## Comparing `dagster-pipes-1.7.2rc2.tar` & `dagster-pipes-1.7.2rc3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:47.250964 dagster-pipes-1.7.2rc2/
--rw-r--r--   0 root         (0) root         (0)    11348 2024-04-16 20:26:55.000000 dagster-pipes-1.7.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 20:26:55.000000 dagster-pipes-1.7.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      797 2024-04-16 20:27:47.250964 dagster-pipes-1.7.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2024-04-16 20:26:55.000000 dagster-pipes-1.7.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:47.250964 dagster-pipes-1.7.2rc2/dagster_pipes/
--rw-r--r--   0 root         (0) root         (0)    48163 2024-04-16 20:26:55.000000 dagster-pipes-1.7.2rc2/dagster_pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 20:26:55.000000 dagster-pipes-1.7.2rc2/dagster_pipes/py.typed
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 20:26:55.000000 dagster-pipes-1.7.2rc2/dagster_pipes/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:47.250964 dagster-pipes-1.7.2rc2/dagster_pipes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      797 2024-04-16 20:27:47.000000 dagster-pipes-1.7.2rc2/dagster_pipes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-16 20:27:47.000000 dagster-pipes-1.7.2rc2/dagster_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:27:47.000000 dagster-pipes-1.7.2rc2/dagster_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:27:47.000000 dagster-pipes-1.7.2rc2/dagster_pipes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 20:27:47.000000 dagster-pipes-1.7.2rc2/dagster_pipes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2024-04-16 20:27:47.250964 dagster-pipes-1.7.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1313 2024-04-16 20:26:55.000000 dagster-pipes-1.7.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:56.587325 dagster-pipes-1.7.2rc3/
+-rw-r--r--   0 root         (0) root         (0)    11348 2024-04-18 21:10:09.000000 dagster-pipes-1.7.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-18 21:10:09.000000 dagster-pipes-1.7.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-18 21:10:56.587325 dagster-pipes-1.7.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-18 21:10:09.000000 dagster-pipes-1.7.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:56.587325 dagster-pipes-1.7.2rc3/dagster_pipes/
+-rw-r--r--   0 root         (0) root         (0)    48159 2024-04-18 21:10:09.000000 dagster-pipes-1.7.2rc3/dagster_pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-18 21:10:09.000000 dagster-pipes-1.7.2rc3/dagster_pipes/py.typed
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-18 21:10:09.000000 dagster-pipes-1.7.2rc3/dagster_pipes/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:56.587325 dagster-pipes-1.7.2rc3/dagster_pipes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-18 21:10:56.000000 dagster-pipes-1.7.2rc3/dagster_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-18 21:10:56.000000 dagster-pipes-1.7.2rc3/dagster_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:10:56.000000 dagster-pipes-1.7.2rc3/dagster_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:10:56.000000 dagster-pipes-1.7.2rc3/dagster_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-18 21:10:56.000000 dagster-pipes-1.7.2rc3/dagster_pipes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-18 21:10:56.591325 dagster-pipes-1.7.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1313 2024-04-18 21:10:09.000000 dagster-pipes-1.7.2rc3/setup.py
```

### Comparing `dagster-pipes-1.7.2rc2/LICENSE` & `dagster-pipes-1.7.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pipes-1.7.2rc2/PKG-INFO` & `dagster-pipes-1.7.2rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pipes
-Version: 1.7.2rc2
+Version: 1.7.2rc3
 Summary: Toolkit for Dagster integrations with transform logic outside of Dagster
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-pipes
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pipes-1.7.2rc2/dagster_pipes/__init__.py` & `dagster-pipes-1.7.2rc3/dagster_pipes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,15 @@
         Yields:
             PipesMessageWriterChannel: Channel for writing messagse back to Dagster.
         """
 
     @final
     def get_opened_payload(self) -> PipesOpenedData:
         """Return a payload containing information about the external process to be passed back to
-        the the orchestration process. This should contain information that cannot be known before
+        the orchestration process. This should contain information that cannot be known before
         the external process is launched.
 
         This method should not be overridden by users. Instead, users should
         override `get_opened_extras` to inject custom data.
         """
         return {"extras": self.get_opened_extras()}
```

### Comparing `dagster-pipes-1.7.2rc2/dagster_pipes.egg-info/PKG-INFO` & `dagster-pipes-1.7.2rc3/dagster_pipes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pipes
-Version: 1.7.2rc2
+Version: 1.7.2rc3
 Summary: Toolkit for Dagster integrations with transform logic outside of Dagster
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-pipes
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pipes-1.7.2rc2/setup.py` & `dagster-pipes-1.7.2rc3/setup.py`

 * *Files identical despite different names*

