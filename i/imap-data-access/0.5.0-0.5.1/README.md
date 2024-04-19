# Comparing `tmp/imap-data-access-0.5.0.tar.gz` & `tmp/imap_data_access-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imap-data-access-0.5.0.tar", last modified: Mon Mar 11 22:07:37 2024, max compression
+gzip compressed data, was "imap_data_access-0.5.1.tar", last modified: Fri Apr 19 14:35:36 2024, max compression
```

## Comparing `imap-data-access-0.5.0.tar` & `imap_data_access-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:07:37.535334 imap-data-access-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-11 22:07:30.000000 imap-data-access-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-11 22:07:37.535334 imap-data-access-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-03-11 22:07:30.000000 imap-data-access-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:07:37.535334 imap-data-access-0.5.0/imap_data_access/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-11 22:07:30.000000 imap-data-access-0.5.0/imap_data_access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-03-11 22:07:30.000000 imap-data-access-0.5.0/imap_data_access/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-03-11 22:07:30.000000 imap-data-access-0.5.0/imap_data_access/file_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-03-11 22:07:30.000000 imap-data-access-0.5.0/imap_data_access/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:07:37.535334 imap-data-access-0.5.0/imap_data_access.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-03-11 22:07:37.000000 imap-data-access-0.5.0/imap_data_access.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-11 22:07:37.000000 imap-data-access-0.5.0/imap_data_access.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 22:07:37.000000 imap-data-access-0.5.0/imap_data_access.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-11 22:07:37.000000 imap-data-access-0.5.0/imap_data_access.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 22:07:37.000000 imap-data-access-0.5.0/imap_data_access.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-11 22:07:37.000000 imap-data-access-0.5.0/imap_data_access.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-11 22:07:30.000000 imap-data-access-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 22:07:37.535334 imap-data-access-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:07:37.535334 imap-data-access-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-11 22:07:30.000000 imap-data-access-0.5.0/tests/test_config_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-03-11 22:07:30.000000 imap-data-access-0.5.0/tests/test_file_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-03-11 22:07:30.000000 imap-data-access-0.5.0/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:36.261167 imap_data_access-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-19 14:35:36.261167 imap_data_access-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:36.257167 imap_data_access-0.5.1/imap_data_access/
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/imap_data_access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/imap_data_access/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9903 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/imap_data_access/file_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/imap_data_access/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:36.257167 imap_data_access-0.5.1/imap_data_access.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 14:35:36.000000 imap_data_access-0.5.1/imap_data_access.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:35:36.261167 imap_data_access-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:36.257167 imap_data_access-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/tests/test_config_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/tests/test_file_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-19 14:35:28.000000 imap_data_access-0.5.1/tests/test_io.py
```

### Comparing `imap-data-access-0.5.0/LICENSE` & `imap_data_access-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imap-data-access-0.5.0/PKG-INFO` & `imap_data_access-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap-data-access
-Version: 0.5.0
+Version: 0.5.1
 Summary: IMAP SDC Data Access
 Author-email: IMAP SDC Developers <imap-sdc@lists.lasp.colorado.edu>
 License: MIT
 Project-URL: homepage, https://github.com/IMAP-Science-Operations-Center
 Project-URL: repository, https://github.com/IMAP-Science-Operations-Center/imap-data-access
 Keywords: IMAP,SDC,SOC,SDS,Science Operations
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `imap-data-access-0.5.0/README.md` & `imap_data_access-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `imap-data-access-0.5.0/imap_data_access/__init__.py` & `imap_data_access-0.5.1/imap_data_access/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Data Access for the IMAP Mission.
 
 The Interstellar Mapping and Acceleration Probe (IMAP) is a NASA mission to study the
 heliosphere. This package contains the data access tools for the IMAP mission. It
 provides a convenient way to query the IMAP data archive and download data files.
 """
+
 import os
 from pathlib import Path
 
 from imap_data_access.file_validation import ScienceFilePath
 from imap_data_access.io import download, query, upload
 
 __all__ = [
@@ -16,15 +17,15 @@
     "upload",
     "ScienceFilePath",
     "VALID_INSTRUMENTS",
     "VALID_DATALEVELS",
     "VALID_FILE_EXTENSION",
     "FILENAME_CONVENTION",
 ]
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 config = {
     "DATA_ACCESS_URL": os.getenv("IMAP_DATA_ACCESS_URL")
     or "https://api.dev.imap-mission.com",
     "DATA_DIR": Path(os.getenv("IMAP_DATA_DIR") or Path.cwd() / "data"),
 }
```

### Comparing `imap-data-access-0.5.0/imap_data_access/cli.py` & `imap_data_access-0.5.1/imap_data_access/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ---
     imap-data-access <command> [<args>]
     imap-data-access --help
     imap-data-access download <file_path>
     imap-data-access query <query-parameters>
     imap-data-access upload <file_path>
 """
+
 import argparse
 import logging
 import os
 from pathlib import Path
 
 import imap_data_access
 
@@ -68,15 +69,16 @@
     # Print data
     for item in query_results:
         values = [
             item["instrument"],
             item["data_level"],
             item["descriptor"],
             item["start_date"],
-            item["repointing"],
+            # Repointing is optional, so use an empty string if not present
+            item["repointing"] or "",
             item["version"],
             os.path.basename(item["file_path"]),
         ]
         print(format_string.format(*values))
     # Close the table
     print(hyphens)
 
@@ -285,12 +287,15 @@
 
     if args.url:
         # We got an explicit url from the command line
         imap_data_access.config["DATA_ACCESS_URL"] = args.url
 
     # Now process through the respective function for the invoked command
     # (set with set_defaults on the subparsers above)
-    args.func(args)
+    try:
+        args.func(args)
+    except Exception as e:
+        parser.error(e)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `imap-data-access-0.5.0/imap_data_access/file_validation.py` & `imap_data_access-0.5.1/imap_data_access/file_validation.py`

 * *Files identical despite different names*

### Comparing `imap-data-access-0.5.0/imap_data_access/io.py` & `imap_data_access-0.5.1/imap_data_access/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Input/output capabilities for the IMAP data processing pipeline."""
+
 # ruff: noqa: PLR0913 S310
 # too many arguments, but we want all of these explicitly listed
 # potentially unsafe usage of urlopen, but we aren't concerned here
 import contextlib
 import json
 import logging
 import urllib.request
```

### Comparing `imap-data-access-0.5.0/imap_data_access.egg-info/PKG-INFO` & `imap_data_access-0.5.1/imap_data_access.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imap-data-access
-Version: 0.5.0
+Version: 0.5.1
 Summary: IMAP SDC Data Access
 Author-email: IMAP SDC Developers <imap-sdc@lists.lasp.colorado.edu>
 License: MIT
 Project-URL: homepage, https://github.com/IMAP-Science-Operations-Center
 Project-URL: repository, https://github.com/IMAP-Science-Operations-Center/imap-data-access
 Keywords: IMAP,SDC,SOC,SDS,Science Operations
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `imap-data-access-0.5.0/pyproject.toml` & `imap_data_access-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imap-data-access"
-version = "0.5.0"
+version = "0.5.1"
 description = "IMAP SDC Data Access"
 authors = [{name = "IMAP SDC Developers", email = "imap-sdc@lists.lasp.colorado.edu"}]
 readme = "README.md"
 license = {text = "MIT"}
 keywords = ["IMAP", "SDC", "SOC", "SDS", "Science Operations"]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `imap-data-access-0.5.0/tests/test_config_options.py` & `imap_data_access-0.5.1/tests/test_config_options.py`

 * *Files identical despite different names*

### Comparing `imap-data-access-0.5.0/tests/test_file_validation.py` & `imap_data_access-0.5.1/tests/test_file_validation.py`

 * *Files identical despite different names*

### Comparing `imap-data-access-0.5.0/tests/test_io.py` & `imap_data_access-0.5.1/tests/test_io.py`

 * *Files identical despite different names*

