# Comparing `tmp/mazeai-0.0.3.tar.gz` & `tmp/mazeai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazeai-0.0.3.tar", last modified: Fri Apr 19 11:11:39 2024, max compression
+gzip compressed data, was "mazeai-0.0.4.tar", last modified: Fri Apr 19 14:23:52 2024, max compression
```

## Comparing `mazeai-0.0.3.tar` & `mazeai-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:11:39.178406 mazeai-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 11:11:32.000000 mazeai-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 11:11:39.178406 mazeai-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 11:11:32.000000 mazeai-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:11:39.178406 mazeai-0.0.3/maze/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:11:32.000000 mazeai-0.0.3/maze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 11:11:32.000000 mazeai-0.0.3/maze/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 11:11:32.000000 mazeai-0.0.3/maze/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 11:11:32.000000 mazeai-0.0.3/maze/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:11:39.178406 mazeai-0.0.3/mazeai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:11:39.178406 mazeai-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 11:11:32.000000 mazeai-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:52.963861 mazeai-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 14:23:48.000000 mazeai-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-19 14:23:52.963861 mazeai-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 14:23:48.000000 mazeai-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:52.963861 mazeai-0.0.4/maze/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:48.000000 mazeai-0.0.4/maze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 14:23:48.000000 mazeai-0.0.4/maze/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 14:23:48.000000 mazeai-0.0.4/maze/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-19 14:23:48.000000 mazeai-0.0.4/maze/chem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-19 14:23:48.000000 mazeai-0.0.4/maze/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 14:23:48.000000 mazeai-0.0.4/maze/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:52.963861 mazeai-0.0.4/mazeai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-19 14:23:52.000000 mazeai-0.0.4/mazeai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-19 14:23:52.000000 mazeai-0.0.4/mazeai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:23:52.000000 mazeai-0.0.4/mazeai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 14:23:52.000000 mazeai-0.0.4/mazeai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:23:52.000000 mazeai-0.0.4/mazeai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 14:23:52.000000 mazeai-0.0.4/mazeai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:23:52.963861 mazeai-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 14:23:48.000000 mazeai-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:52.963861 mazeai-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-19 14:23:48.000000 mazeai-0.0.4/tests/test_chem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:48.000000 mazeai-0.0.4/tests/test_network.py
```

### Comparing `mazeai-0.0.3/LICENSE` & `mazeai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mazeai-0.0.3/PKG-INFO` & `mazeai-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazeai
-Version: 0.0.3
+Version: 0.0.4
 Summary: A General Tool Set for Science Researches
 Home-page: https://github.com/zhaisilong/mazeai
 Author: Zhai Silong
 Author-email: zhaisilong@outlook.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -26,12 +26,14 @@
 </p>
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/mazeai/"><img src="https://img.shields.io/pypi/v/mazeai" alt="pypi version"/></a>
 </p>
 
+![Conda Version](https://img.shields.io/conda/v/mazeai/mazeai.svg)
+
 ## 前言
 
 ## 环境安装
 
 ## 其他
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: mazeai Version: 0.0.3 Summary: A General Tool Set
+Metadata-Version: 2.1 Name: mazeai Version: 0.0.4 Summary: A General Tool Set
 for Science Researches Home-page: https://github.com/zhaisilong/mazeai Author:
 Zhai Silong Author-email: zhaisilong@outlook.com License: MIT Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3.7 Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: rich Requires-Dist: ipykernel Requires-Dist: tqdm Requires-Dist: loguru
 Requires-Dist: hydra-core
                                    [maze ai]
                                ******** MMAAZZEE AAII ********
                   äººå·¥æºè½è¾å©è¯ç©è®¾è®¡å·¥å·éå
                                 _[_p_y_p_i_ _v_e_r_s_i_o_n_]
-## åè¨ ## ç¯å¢å®è£ ## å¶ä»
+![Conda Version](https://img.shields.io/conda/v/mazeai/mazeai.svg) ## åè¨ ##
+ç¯å¢å®è£ ## å¶ä»
```

### Comparing `mazeai-0.0.3/mazeai.egg-info/PKG-INFO` & `mazeai-0.0.4/mazeai.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazeai
-Version: 0.0.3
+Version: 0.0.4
 Summary: A General Tool Set for Science Researches
 Home-page: https://github.com/zhaisilong/mazeai
 Author: Zhai Silong
 Author-email: zhaisilong@outlook.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -26,12 +26,14 @@
 </p>
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/mazeai/"><img src="https://img.shields.io/pypi/v/mazeai" alt="pypi version"/></a>
 </p>
 
+![Conda Version](https://img.shields.io/conda/v/mazeai/mazeai.svg)
+
 ## 前言
 
 ## 环境安装
 
 ## 其他
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: mazeai Version: 0.0.3 Summary: A General Tool Set
+Metadata-Version: 2.1 Name: mazeai Version: 0.0.4 Summary: A General Tool Set
 for Science Researches Home-page: https://github.com/zhaisilong/mazeai Author:
 Zhai Silong Author-email: zhaisilong@outlook.com License: MIT Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3.7 Requires-Python:
 >=3.6 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: rich Requires-Dist: ipykernel Requires-Dist: tqdm Requires-Dist: loguru
 Requires-Dist: hydra-core
                                    [maze ai]
                                ******** MMAAZZEE AAII ********
                   äººå·¥æºè½è¾å©è¯ç©è®¾è®¡å·¥å·éå
                                 _[_p_y_p_i_ _v_e_r_s_i_o_n_]
-## åè¨ ## ç¯å¢å®è£ ## å¶ä»
+![Conda Version](https://img.shields.io/conda/v/mazeai/mazeai.svg) ## åè¨ ##
+ç¯å¢å®è£ ## å¶ä»
```

### Comparing `mazeai-0.0.3/setup.py` & `mazeai-0.0.4/setup.py`

 * *Files identical despite different names*

