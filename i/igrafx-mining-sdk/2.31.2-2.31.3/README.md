# Comparing `tmp/igrafx_mining_sdk-2.31.2.tar.gz` & `tmp/igrafx_mining_sdk-2.31.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igrafx_mining_sdk-2.31.2.tar", last modified: Fri Apr 19 08:08:13 2024, max compression
+gzip compressed data, was "igrafx_mining_sdk-2.31.3.tar", last modified: Fri Apr 19 08:52:30 2024, max compression
```

## Comparing `igrafx_mining_sdk-2.31.2.tar` & `igrafx_mining_sdk-2.31.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/column_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    23262 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/workgroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-19 08:08:13.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 08:08:13.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:08:13.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 08:08:13.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:08:13.505211 igrafx_mining_sdk-2.31.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 08:07:59.000000 igrafx_mining_sdk-2.31.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.497211 igrafx_mining_sdk-2.31.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/tests/data/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/data/graphs/graph.json
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/data/graphs/graph_with_invalid_edges.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/tests/data/tables/
--rw-r--r--   0 runner    (1001) docker     (127)    27136 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/data/tables/p2pShortExcel.xls
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/data/tables/p2pShortExcel.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/data/tables/testdata.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_00_workgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_01_column_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    35094 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_02_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_03_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_04_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_05_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:52:30.475919 igrafx_mining_sdk-2.31.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-19 08:52:30.475919 igrafx_mining_sdk-2.31.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:52:30.471919 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23262 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/workgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:52:30.475919 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-19 08:52:30.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 08:52:30.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:52:30.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 08:52:30.000000 igrafx_mining_sdk-2.31.3/igrafx_mining_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:52:30.475919 igrafx_mining_sdk-2.31.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 08:52:15.000000 igrafx_mining_sdk-2.31.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:52:30.475919 igrafx_mining_sdk-2.31.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:52:30.471919 igrafx_mining_sdk-2.31.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:52:30.475919 igrafx_mining_sdk-2.31.3/tests/data/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/data/graphs/graph.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/data/graphs/graph_with_invalid_edges.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:52:30.475919 igrafx_mining_sdk-2.31.3/tests/data/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)    27136 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/data/tables/p2pShortExcel.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/data/tables/p2pShortExcel.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/data/tables/testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/test_00_workgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/test_01_column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35094 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/test_02_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/test_03_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/test_04_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 08:52:05.000000 igrafx_mining_sdk-2.31.3/tests/test_05_delete.py
```

### Comparing `igrafx_mining_sdk-2.31.2/LICENSE` & `igrafx_mining_sdk-2.31.3/LICENSE`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/PKG-INFO` & `igrafx_mining_sdk-2.31.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igrafx_mining_sdk
-Version: 2.31.2
+Version: 2.31.3
 Summary: The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects.
 Home-page: https://www.igrafx.com
 Author: iGrafx
 Author-email: contact@igrafx.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `igrafx_mining_sdk-2.31.2/README.md` & `igrafx_mining_sdk-2.31.3/README.md`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/__init__.py` & `igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/api_connector.py` & `igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/api_connector.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/column_mapping.py` & `igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/column_mapping.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/datasource.py` & `igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/datasource.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/graph.py` & `igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/graph.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/project.py` & `igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/project.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/workgroup.py` & `igrafx_mining_sdk-2.31.3/igrafx_mining_sdk/workgroup.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/PKG-INFO` & `igrafx_mining_sdk-2.31.3/igrafx_mining_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igrafx-mining-sdk
-Version: 2.31.2
+Version: 2.31.3
 Summary: The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects.
 Home-page: https://www.igrafx.com
 Author: iGrafx
 Author-email: contact@igrafx.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/SOURCES.txt` & `igrafx_mining_sdk-2.31.3/igrafx_mining_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/pyproject.toml` & `igrafx_mining_sdk-2.31.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "igrafx_mining_sdk"
-version = "2.31.1"
+version = "2.31.2"
 description = "The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects."
 authors = ["iGrafx <contact@igrafx.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.grafx.com/"
 repository = "https://github.com/igrafx/mining-python-sdk"
 keywords = ["process mining"]
```

### Comparing `igrafx_mining_sdk-2.31.2/setup.py` & `igrafx_mining_sdk-2.31.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 }
 
 # Extract requirements
 requirements = list(pyproject_data['tool']['poetry']['dependencies'].values())
 
 setup(
     name="igrafx_mining_sdk",
-    version='2.31.2',
+    version='2.31.3',
     description=package_infos['__doc__'],
     long_description=open("README.md", 'r').read(),
     long_description_content_type='text/markdown',
     url="https://www.igrafx.com",
     author=package_infos['__author__'],
     author_email=package_infos['__email__'],
     packages=find_packages(),
```

### Comparing `igrafx_mining_sdk-2.31.2/tests/data/graphs/graph.json` & `igrafx_mining_sdk-2.31.3/tests/data/graphs/graph.json`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/tests/data/graphs/graph_with_invalid_edges.json` & `igrafx_mining_sdk-2.31.3/tests/data/graphs/graph_with_invalid_edges.json`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/tests/data/tables/p2pShortExcel.xls` & `igrafx_mining_sdk-2.31.3/tests/data/tables/p2pShortExcel.xls`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/tests/data/tables/p2pShortExcel.xlsx` & `igrafx_mining_sdk-2.31.3/tests/data/tables/p2pShortExcel.xlsx`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/tests/test_00_workgroup.py` & `igrafx_mining_sdk-2.31.3/tests/test_00_workgroup.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/tests/test_01_column_mapping.py` & `igrafx_mining_sdk-2.31.3/tests/test_01_column_mapping.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/tests/test_02_project.py` & `igrafx_mining_sdk-2.31.3/tests/test_02_project.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/tests/test_03_datasource.py` & `igrafx_mining_sdk-2.31.3/tests/test_03_datasource.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.31.2/tests/test_04_graph.py` & `igrafx_mining_sdk-2.31.3/tests/test_04_graph.py`

 * *Files identical despite different names*

