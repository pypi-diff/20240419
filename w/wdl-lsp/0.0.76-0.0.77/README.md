# Comparing `tmp/wdl-lsp-0.0.76.tar.gz` & `tmp/wdl-lsp-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wdl-lsp-0.0.76.tar", last modified: Fri May 21 17:30:00 2021, max compression
+gzip compressed data, was "dist/wdl-lsp-0.0.77.tar", last modified: Thu Sep  2 16:23:44 2021, max compression
```

## Comparing `wdl-lsp-0.0.76.tar` & `wdl-lsp-0.0.77.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-05-21 17:29:52.000000 wdl-lsp-0.0.76/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1214 2021-05-21 17:29:52.000000 wdl-lsp-0.0.76/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/wdl_lsp/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1232 2021-05-21 17:29:52.000000 wdl-lsp-0.0.76/wdl_lsp/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2261 2021-05-21 17:29:52.000000 wdl-lsp-0.0.76/wdl_lsp/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17170 2021-05-21 17:29:52.000000 wdl-lsp-0.0.76/wdl_lsp/server.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/wdl_lsp/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1232 2021-05-21 17:29:52.000000 wdl-lsp-0.0.76/wdl_lsp/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/wdl_lsp/tests/unit/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1232 2021-05-21 17:29:52.000000 wdl-lsp-0.0.76/wdl_lsp/tests/unit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3425 2021-05-21 17:29:52.000000 wdl-lsp-0.0.76/wdl_lsp/tests/unit/test_features.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/wdl_lsp.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/wdl_lsp.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      364 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/wdl_lsp.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/wdl_lsp.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/wdl_lsp.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/wdl_lsp.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2021-05-21 17:30:00.000000 wdl-lsp-0.0.76/wdl_lsp.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      744 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-09-02 16:23:36.000000 wdl-lsp-0.0.77/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1214 2021-09-02 16:23:36.000000 wdl-lsp-0.0.77/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/wdl_lsp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1232 2021-09-02 16:23:36.000000 wdl-lsp-0.0.77/wdl_lsp/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2261 2021-09-02 16:23:36.000000 wdl-lsp-0.0.77/wdl_lsp/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17170 2021-09-02 16:23:36.000000 wdl-lsp-0.0.77/wdl_lsp/server.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/wdl_lsp/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1232 2021-09-02 16:23:36.000000 wdl-lsp-0.0.77/wdl_lsp/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/wdl_lsp/tests/unit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1232 2021-09-02 16:23:36.000000 wdl-lsp-0.0.77/wdl_lsp/tests/unit/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3425 2021-09-02 16:23:36.000000 wdl-lsp-0.0.77/wdl_lsp/tests/unit/test_features.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/wdl_lsp.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      744 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/wdl_lsp.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      364 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/wdl_lsp.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/wdl_lsp.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/wdl_lsp.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       50 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/wdl_lsp.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2021-09-02 16:23:44.000000 wdl-lsp-0.0.77/wdl_lsp.egg-info/top_level.txt
```

### Comparing `wdl-lsp-0.0.76/PKG-INFO` & `wdl-lsp-0.0.77/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: wdl-lsp
-Version: 0.0.76
+Version: 0.0.77
 Summary: Language Server Protocol (LSP) implementation for Workflow Definition Language (WDL)
 Home-page: https://github.com/broadinstitute/wdl-ide
 Author: Broad Institute
 License: BSD 3-clause "New" or "Revised" License
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7.0
+
+UNKNOWN
+
```

### Comparing `wdl-lsp-0.0.76/setup.py` & `wdl-lsp-0.0.77/setup.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.76/wdl_lsp/__init__.py` & `wdl-lsp-0.0.77/wdl_lsp/__init__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.76/wdl_lsp/__main__.py` & `wdl-lsp-0.0.77/wdl_lsp/__main__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.76/wdl_lsp/server.py` & `wdl-lsp-0.0.77/wdl_lsp/server.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.76/wdl_lsp/tests/__init__.py` & `wdl-lsp-0.0.77/wdl_lsp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.76/wdl_lsp/tests/unit/__init__.py` & `wdl-lsp-0.0.77/wdl_lsp/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.76/wdl_lsp/tests/unit/test_features.py` & `wdl-lsp-0.0.77/wdl_lsp/tests/unit/test_features.py`

 * *Files identical despite different names*

### Comparing `wdl-lsp-0.0.76/wdl_lsp.egg-info/PKG-INFO` & `wdl-lsp-0.0.77/wdl_lsp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: wdl-lsp
-Version: 0.0.76
+Version: 0.0.77
 Summary: Language Server Protocol (LSP) implementation for Workflow Definition Language (WDL)
 Home-page: https://github.com/broadinstitute/wdl-ide
 Author: Broad Institute
 License: BSD 3-clause "New" or "Revised" License
-Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7.0
+
+UNKNOWN
+
```

