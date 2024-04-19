# Comparing `tmp/loretta-0.1.0.tar.gz` & `tmp/loretta-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loretta-0.1.0.tar", last modified: Sun Mar 17 23:31:16 2024, max compression
+gzip compressed data, was "loretta-0.1.2.tar", last modified: Thu Apr 18 23:31:34 2024, max compression
```

## Comparing `loretta-0.1.0.tar` & `loretta-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,12 @@
-drwxr-xr-x   0 yifanycc   (501) staff       (20)        0 2024-03-17 23:31:16.287340 loretta-0.1.0/
--rw-r--r--   0 yifanycc   (501) staff       (20)    35149 2024-03-13 23:05:20.000000 loretta-0.1.0/LICENSE
--rw-r--r--   0 yifanycc   (501) staff       (20)     5323 2024-03-17 23:31:16.287140 loretta-0.1.0/PKG-INFO
-drwxr-xr-x   0 yifanycc   (501) staff       (20)        0 2024-03-17 23:31:16.283823 loretta-0.1.0/loretta/
--rw-r--r--   0 yifanycc   (501) staff       (20)     1363 2024-03-17 00:09:19.000000 loretta-0.1.0/loretta/__init__.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     8797 2024-03-17 17:58:05.000000 loretta-0.1.0/loretta/mapping.py
--rw-r--r--   0 yifanycc   (501) staff       (20)    45297 2024-03-14 22:47:08.000000 loretta-0.1.0/loretta/peft_model.py
-drwxr-xr-x   0 yifanycc   (501) staff       (20)        0 2024-03-17 23:31:16.285172 loretta-0.1.0/loretta/tensor_layers/
--rw-r--r--   0 yifanycc   (501) staff       (20)      118 2024-03-13 23:05:20.000000 loretta-0.1.0/loretta/tensor_layers/__init__.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     7130 2024-03-17 18:23:44.000000 loretta-0.1.0/loretta/tensor_layers/layers.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     6138 2024-03-17 18:23:44.000000 loretta-0.1.0/loretta/tensor_layers/low_rank_tensors.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     7252 2024-03-17 18:23:44.000000 loretta-0.1.0/loretta/tensor_layers/utils.py
-drwxr-xr-x   0 yifanycc   (501) staff       (20)        0 2024-03-17 23:31:16.286078 loretta-0.1.0/loretta/tuners/
--rw-r--r--   0 yifanycc   (501) staff       (20)     1137 2024-03-14 06:54:31.000000 loretta-0.1.0/loretta/tuners/__init__.py
--rw-r--r--   0 yifanycc   (501) staff       (20)    25953 2024-03-17 18:11:47.000000 loretta-0.1.0/loretta/tuners/loretta_adp.py
--rw-r--r--   0 yifanycc   (501) staff       (20)    28757 2024-03-17 18:19:31.000000 loretta-0.1.0/loretta/tuners/loretta_rep.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     6716 2023-11-29 07:13:56.000000 loretta-0.1.0/loretta/tuners/p_tuning.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     3740 2023-11-29 07:13:56.000000 loretta-0.1.0/loretta/tuners/prefix_tuning.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     4889 2023-11-29 07:13:56.000000 loretta-0.1.0/loretta/tuners/prompt_tuning.py
-drwxr-xr-x   0 yifanycc   (501) staff       (20)        0 2024-03-17 23:31:16.286764 loretta-0.1.0/loretta/utils/
--rw-r--r--   0 yifanycc   (501) staff       (20)     1341 2024-03-17 18:06:24.000000 loretta-0.1.0/loretta/utils/__init__.py
--rw-r--r--   0 yifanycc   (501) staff       (20)      730 2023-11-22 19:54:29.000000 loretta-0.1.0/loretta/utils/adapters_utils.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     6657 2023-11-29 07:13:56.000000 loretta-0.1.0/loretta/utils/config.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     5927 2023-11-22 19:54:29.000000 loretta-0.1.0/loretta/utils/other.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     4102 2023-11-22 19:54:29.000000 loretta-0.1.0/loretta/utils/save_and_load.py
--rw-r--r--   0 yifanycc   (501) staff       (20)     2386 2024-03-17 18:06:06.000000 loretta-0.1.0/loretta/utils/tensor_util.py
-drwxr-xr-x   0 yifanycc   (501) staff       (20)        0 2024-03-17 23:31:16.286919 loretta-0.1.0/loretta.egg-info/
--rw-r--r--   0 yifanycc   (501) staff       (20)     5323 2024-03-17 23:31:16.000000 loretta-0.1.0/loretta.egg-info/PKG-INFO
--rw-r--r--   0 yifanycc   (501) staff       (20)      713 2024-03-17 23:31:16.000000 loretta-0.1.0/loretta.egg-info/SOURCES.txt
--rw-r--r--   0 yifanycc   (501) staff       (20)        1 2024-03-17 23:31:16.000000 loretta-0.1.0/loretta.egg-info/dependency_links.txt
--rw-r--r--   0 yifanycc   (501) staff       (20)       33 2024-03-17 23:31:16.000000 loretta-0.1.0/loretta.egg-info/requires.txt
--rw-r--r--   0 yifanycc   (501) staff       (20)        8 2024-03-17 23:31:16.000000 loretta-0.1.0/loretta.egg-info/top_level.txt
--rw-r--r--   0 yifanycc   (501) staff       (20)       38 2024-03-17 23:31:16.287387 loretta-0.1.0/setup.cfg
--rw-r--r--   0 yifanycc   (501) staff       (20)      608 2024-03-17 23:31:03.000000 loretta-0.1.0/setup.py
+drwxr-xr-x   0 yifanycc   (501) staff       (20)        0 2024-04-18 23:31:34.817191 loretta-0.1.2/
+-rw-r--r--   0 yifanycc   (501) staff       (20)    35149 2024-03-13 23:05:20.000000 loretta-0.1.2/LICENSE
+-rw-r--r--   0 yifanycc   (501) staff       (20)     5323 2024-04-18 23:31:34.816974 loretta-0.1.2/PKG-INFO
+-rw-r--r--   0 yifanycc   (501) staff       (20)     4929 2024-03-17 23:25:28.000000 loretta-0.1.2/README.md
+drwxr-xr-x   0 yifanycc   (501) staff       (20)        0 2024-04-18 23:31:34.816666 loretta-0.1.2/loretta.egg-info/
+-rw-r--r--   0 yifanycc   (501) staff       (20)     5323 2024-04-18 23:31:34.000000 loretta-0.1.2/loretta.egg-info/PKG-INFO
+-rw-r--r--   0 yifanycc   (501) staff       (20)      180 2024-04-18 23:31:34.000000 loretta-0.1.2/loretta.egg-info/SOURCES.txt
+-rw-r--r--   0 yifanycc   (501) staff       (20)        1 2024-04-18 23:31:34.000000 loretta-0.1.2/loretta.egg-info/dependency_links.txt
+-rw-r--r--   0 yifanycc   (501) staff       (20)       33 2024-04-18 23:31:34.000000 loretta-0.1.2/loretta.egg-info/requires.txt
+-rw-r--r--   0 yifanycc   (501) staff       (20)        1 2024-04-18 23:31:34.000000 loretta-0.1.2/loretta.egg-info/top_level.txt
+-rw-r--r--   0 yifanycc   (501) staff       (20)       38 2024-04-18 23:31:34.817252 loretta-0.1.2/setup.cfg
+-rw-r--r--   0 yifanycc   (501) staff       (20)      608 2024-04-18 23:31:22.000000 loretta-0.1.2/setup.py
```

### Comparing `loretta-0.1.0/LICENSE` & `loretta-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loretta-0.1.0/PKG-INFO` & `loretta-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loretta
-Version: 0.1.0
+Version: 0.1.2
 Summary: Official implementation for the LoRETTA adapters
 Home-page: https://github.com/yifanycc/loretta
 Author: Yifan Yang, Jiajun Zhou, Ngai Wong, Zheng Zhang
 Author-email: yifanycc@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `loretta-0.1.0/loretta.egg-info/PKG-INFO` & `loretta-0.1.2/loretta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loretta
-Version: 0.1.0
+Version: 0.1.2
 Summary: Official implementation for the LoRETTA adapters
 Home-page: https://github.com/yifanycc/loretta
 Author: Yifan Yang, Jiajun Zhou, Ngai Wong, Zheng Zhang
 Author-email: yifanycc@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `loretta-0.1.0/setup.py` & `loretta-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="loretta",
-    version="0.1.0",
+    version="0.1.2",
     author="Yifan Yang, Jiajun Zhou, Ngai Wong, Zheng Zhang",
     author_email="yifanycc@gmail.com",
     description="Official implementation for the LoRETTA adapters",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yifanycc/loretta",
     packages=setuptools.find_packages(),
```

