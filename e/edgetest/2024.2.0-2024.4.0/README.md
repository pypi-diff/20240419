# Comparing `tmp/edgetest-2024.2.0.tar.gz` & `tmp/edgetest-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgetest-2024.2.0.tar", last modified: Fri Feb 16 19:59:40 2024, max compression
+gzip compressed data, was "edgetest-2024.4.0.tar", last modified: Fri Apr 19 16:58:17 2024, max compression
```

## Comparing `edgetest-2024.2.0.tar` & `edgetest-2024.4.0.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:59:40.919710 edgetest-2024.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-16 19:59:14.000000 edgetest-2024.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-16 19:59:14.000000 edgetest-2024.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-16 19:59:14.000000 edgetest-2024.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-02-16 19:59:40.919710 edgetest-2024.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-02-16 19:59:14.000000 edgetest-2024.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:59:40.911710 edgetest-2024.2.0/edgetest/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-16 19:59:14.000000 edgetest-2024.2.0/edgetest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-02-16 19:59:14.000000 edgetest-2024.2.0/edgetest/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-02-16 19:59:14.000000 edgetest-2024.2.0/edgetest/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-02-16 19:59:14.000000 edgetest-2024.2.0/edgetest/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-02-16 19:59:14.000000 edgetest-2024.2.0/edgetest/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-16 19:59:14.000000 edgetest-2024.2.0/edgetest/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-16 19:59:14.000000 edgetest-2024.2.0/edgetest/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-02-16 19:59:14.000000 edgetest-2024.2.0/edgetest/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-02-16 19:59:14.000000 edgetest-2024.2.0/edgetest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:59:40.915710 edgetest-2024.2.0/edgetest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-02-16 19:59:40.000000 edgetest-2024.2.0/edgetest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-16 19:59:40.000000 edgetest-2024.2.0/edgetest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 19:59:40.000000 edgetest-2024.2.0/edgetest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-16 19:59:40.000000 edgetest-2024.2.0/edgetest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 19:59:16.000000 edgetest-2024.2.0/edgetest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-16 19:59:40.000000 edgetest-2024.2.0/edgetest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-16 19:59:40.000000 edgetest-2024.2.0/edgetest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-16 19:59:14.000000 edgetest-2024.2.0/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-16 19:59:14.000000 edgetest-2024.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-02-16 19:59:40.919710 edgetest-2024.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-16 19:59:14.000000 edgetest-2024.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 19:59:40.915710 edgetest-2024.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/test_integration_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/test_integration_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)    19222 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/test_interface_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    19339 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/test_interface_toml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-02-16 19:59:14.000000 edgetest-2024.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:58:17.569427 edgetest-2024.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 16:57:50.000000 edgetest-2024.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 16:57:50.000000 edgetest-2024.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 16:57:50.000000 edgetest-2024.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-04-19 16:58:17.569427 edgetest-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-19 16:57:50.000000 edgetest-2024.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:58:17.561427 edgetest-2024.4.0/edgetest/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-19 16:57:50.000000 edgetest-2024.4.0/edgetest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-04-19 16:57:50.000000 edgetest-2024.4.0/edgetest/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-19 16:57:50.000000 edgetest-2024.4.0/edgetest/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-04-19 16:57:50.000000 edgetest-2024.4.0/edgetest/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-19 16:57:50.000000 edgetest-2024.4.0/edgetest/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-19 16:57:50.000000 edgetest-2024.4.0/edgetest/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-19 16:57:50.000000 edgetest-2024.4.0/edgetest/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-19 16:57:50.000000 edgetest-2024.4.0/edgetest/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18987 2024-04-19 16:57:50.000000 edgetest-2024.4.0/edgetest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:58:17.565427 edgetest-2024.4.0/edgetest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7695 2024-04-19 16:58:17.000000 edgetest-2024.4.0/edgetest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-19 16:58:17.000000 edgetest-2024.4.0/edgetest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:58:17.000000 edgetest-2024.4.0/edgetest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 16:58:17.000000 edgetest-2024.4.0/edgetest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:57:54.000000 edgetest-2024.4.0/edgetest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-19 16:58:17.000000 edgetest-2024.4.0/edgetest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 16:58:17.000000 edgetest-2024.4.0/edgetest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-19 16:57:50.000000 edgetest-2024.4.0/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-19 16:57:50.000000 edgetest-2024.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-19 16:58:17.569427 edgetest-2024.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-19 16:57:50.000000 edgetest-2024.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:58:17.565427 edgetest-2024.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-19 16:57:50.000000 edgetest-2024.4.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-19 16:57:50.000000 edgetest-2024.4.0/tests/test_integration_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-04-19 16:57:50.000000 edgetest-2024.4.0/tests/test_integration_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19222 2024-04-19 16:57:50.000000 edgetest-2024.4.0/tests/test_interface_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19339 2024-04-19 16:57:50.000000 edgetest-2024.4.0/tests/test_interface_toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-19 16:57:50.000000 edgetest-2024.4.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-19 16:57:50.000000 edgetest-2024.4.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-19 16:57:50.000000 edgetest-2024.4.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-04-19 16:57:50.000000 edgetest-2024.4.0/tests/test_utils.py
```

### Comparing `edgetest-2024.2.0/LICENSE` & `edgetest-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/PKG-INFO` & `edgetest-2024.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest
-Version: 2024.2.0
+Version: 2024.4.0
 Summary: Bleeding edge dependency testing
 Home-page: https://github.com/capitalone/edgetest
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 License: Apache Software License
@@ -20,19 +20,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: Cerberus<=1.3.4,>=1.3.0
-Requires-Dist: click<=8.1.3,>=7.0
-Requires-Dist: pluggy<=1.0.0,>=1.0.0
+Requires-Dist: Cerberus<=1.3.5,>=1.3.0
+Requires-Dist: click<=8.1.7,>=7.0
+Requires-Dist: pluggy<=1.4.0,>=1.0.0
 Requires-Dist: tabulate<=0.9.0,>=0.8.9
-Requires-Dist: packaging<=23.0,>20.6
+Requires-Dist: packaging<=24.0,>20.6
 Requires-Dist: tomlkit<=0.11.4,>=0.11.4
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-tabs; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
```

### Comparing `edgetest-2024.2.0/README.md` & `edgetest-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/edgetest/core.py` & `edgetest-2024.4.0/edgetest/core.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/edgetest/hookspecs.py` & `edgetest-2024.4.0/edgetest/hookspecs.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/edgetest/interface.py` & `edgetest-2024.4.0/edgetest/interface.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/edgetest/lib.py` & `edgetest-2024.4.0/edgetest/lib.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/edgetest/logger.py` & `edgetest-2024.4.0/edgetest/logger.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/edgetest/report.py` & `edgetest-2024.4.0/edgetest/report.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/edgetest/schema.py` & `edgetest-2024.4.0/edgetest/schema.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/edgetest/utils.py` & `edgetest-2024.4.0/edgetest/utils.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/edgetest.egg-info/PKG-INFO` & `edgetest-2024.4.0/edgetest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest
-Version: 2024.2.0
+Version: 2024.4.0
 Summary: Bleeding edge dependency testing
 Home-page: https://github.com/capitalone/edgetest
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 License: Apache Software License
@@ -20,19 +20,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: Cerberus<=1.3.4,>=1.3.0
-Requires-Dist: click<=8.1.3,>=7.0
-Requires-Dist: pluggy<=1.0.0,>=1.0.0
+Requires-Dist: Cerberus<=1.3.5,>=1.3.0
+Requires-Dist: click<=8.1.7,>=7.0
+Requires-Dist: pluggy<=1.4.0,>=1.0.0
 Requires-Dist: tabulate<=0.9.0,>=0.8.9
-Requires-Dist: packaging<=23.0,>20.6
+Requires-Dist: packaging<=24.0,>20.6
 Requires-Dist: tomlkit<=0.11.4,>=0.11.4
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-tabs; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
```

### Comparing `edgetest-2024.2.0/edgetest.egg-info/SOURCES.txt` & `edgetest-2024.4.0/edgetest.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 edgetest.egg-info/PKG-INFO
 edgetest.egg-info/SOURCES.txt
 edgetest.egg-info/dependency_links.txt
 edgetest.egg-info/entry_points.txt
 edgetest.egg-info/not-zip-safe
 edgetest.egg-info/requires.txt
 edgetest.egg-info/top_level.txt
-tests/__init__.py
-tests/conftest.py
 tests/test_core.py
 tests/test_integration_cfg.py
 tests/test_integration_toml.py
 tests/test_interface_cfg.py
 tests/test_interface_toml.py
 tests/test_lib.py
 tests/test_report.py
```

### Comparing `edgetest-2024.2.0/edgetest.egg-info/requires.txt` & `edgetest-2024.4.0/edgetest.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Cerberus<=1.3.4,>=1.3.0
-click<=8.1.3,>=7.0
-pluggy<=1.0.0,>=1.0.0
+Cerberus<=1.3.5,>=1.3.0
+click<=8.1.7,>=7.0
+pluggy<=1.4.0,>=1.0.0
 tabulate<=0.9.0,>=0.8.9
-packaging<=23.0,>20.6
+packaging<=24.0,>20.6
 tomlkit<=0.11.4,>=0.11.4
 
 [build]
 build
 twine
 wheel
 bumpver
```

### Comparing `edgetest-2024.2.0/pull_request_template.md` & `edgetest-2024.4.0/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/setup.cfg` & `edgetest-2024.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,20 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 zip_safe = False
 include_package_data = True
-packages = find:
 install_requires = 
-	Cerberus<=1.3.4,>=1.3.0
-	click<=8.1.3,>=7.0
-	pluggy<=1.0.0,>=1.0.0
+	Cerberus<=1.3.5,>=1.3.0
+	click<=8.1.7,>=7.0
+	pluggy<=1.4.0,>=1.0.0
 	tabulate<=0.9.0,>=0.8.9
-	packaging<=23.0,>20.6
+	packaging<=24.0,>20.6
 	tomlkit<=0.11.4,>=0.11.4
 
 [options.extras_require]
 docs = 
 	furo
 	sphinx
 	sphinx-copybutton
```

### Comparing `edgetest-2024.2.0/tests/test_core.py` & `edgetest-2024.4.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/tests/test_integration_cfg.py` & `edgetest-2024.4.0/tests/test_integration_cfg.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/tests/test_integration_toml.py` & `edgetest-2024.4.0/tests/test_integration_toml.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/tests/test_interface_cfg.py` & `edgetest-2024.4.0/tests/test_interface_cfg.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/tests/test_interface_toml.py` & `edgetest-2024.4.0/tests/test_interface_toml.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/tests/test_lib.py` & `edgetest-2024.4.0/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/tests/test_report.py` & `edgetest-2024.4.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/tests/test_schema.py` & `edgetest-2024.4.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `edgetest-2024.2.0/tests/test_utils.py` & `edgetest-2024.4.0/tests/test_utils.py`

 * *Files identical despite different names*

