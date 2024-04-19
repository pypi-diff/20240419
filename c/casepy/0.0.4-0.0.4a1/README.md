# Comparing `tmp/casepy-0.0.4.tar.gz` & `tmp/casepy-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casepy-0.0.4.tar", last modified: Fri Apr 19 07:51:34 2024, max compression
+gzip compressed data, was "casepy-0.0.4a1.tar", last modified: Fri Apr 19 07:46:33 2024, max compression
```

## Comparing `casepy-0.0.4.tar` & `casepy-0.0.4a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:34.013054 casepy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 07:51:26.000000 casepy-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-19 07:51:34.013054 casepy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-19 07:51:26.000000 casepy-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:51:34.013054 casepy-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-19 07:51:26.000000 casepy-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:34.013054 casepy-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:34.013054 casepy-0.0.4/src/casepy/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 07:51:26.000000 casepy-0.0.4/src/casepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-19 07:51:26.000000 casepy-0.0.4/src/casepy/combination_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 07:51:26.000000 casepy-0.0.4/src/casepy/simple_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:34.013054 casepy-0.0.4/src/casepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-19 07:51:33.000000 casepy-0.0.4/src/casepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-19 07:51:33.000000 casepy-0.0.4/src/casepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:51:33.000000 casepy-0.0.4/src/casepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 07:51:33.000000 casepy-0.0.4/src/casepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:46:33.486967 casepy-0.0.4a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 07:46:27.000000 casepy-0.0.4a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 07:46:33.486967 casepy-0.0.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-19 07:46:27.000000 casepy-0.0.4a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:46:33.486967 casepy-0.0.4a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 07:46:27.000000 casepy-0.0.4a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:46:33.482967 casepy-0.0.4a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:46:33.486967 casepy-0.0.4a1/src/casepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 07:46:27.000000 casepy-0.0.4a1/src/casepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-19 07:46:27.000000 casepy-0.0.4a1/src/casepy/combination_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 07:46:27.000000 casepy-0.0.4a1/src/casepy/simple_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:46:33.486967 casepy-0.0.4a1/src/casepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 07:46:33.000000 casepy-0.0.4a1/src/casepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-19 07:46:33.000000 casepy-0.0.4a1/src/casepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:46:33.000000 casepy-0.0.4a1/src/casepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 07:46:33.000000 casepy-0.0.4a1/src/casepy.egg-info/top_level.txt
```

### Comparing `casepy-0.0.4/LICENSE` & `casepy-0.0.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `casepy-0.0.4/PKG-INFO` & `casepy-0.0.4a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.4
+Version: 0.0.4a1
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -34,16 +34,15 @@
 With casepy, you can easily generate a combination of elements in a list.
 
 - Example
 
 Initialize generator
 
 ``` Python
-import casepy
-generator = casepy.CombinationGenerator()
+generator = CombinationGenerator()
 generator.set_parameters(4, [1,2,3,4,5])
 ```
 
 all_case()
 
 ``` Python
 all_case_list = generator.all_case()
```

### Comparing `casepy-0.0.4/README.md` & `casepy-0.0.4a1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 With casepy, you can easily generate a combination of elements in a list.
 
 - Example
 
 Initialize generator
 
 ``` Python
-import casepy
-generator = casepy.CombinationGenerator()
+generator = CombinationGenerator()
 generator.set_parameters(4, [1,2,3,4,5])
 ```
 
 all_case()
 
 ``` Python
 all_case_list = generator.all_case()
```

### Comparing `casepy-0.0.4/setup.py` & `casepy-0.0.4a1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="casepy",
     py_modules=["casepy"],
-    version="0.0.4",
+    version="0.0.4a1",
     description="A Python package for generating cases in a list.",
     url="https://github.com/DongHoon5793/casepy",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     author="DongHoon Kim",
     author_email="donghoon5793@gmail.com",
```

### Comparing `casepy-0.0.4/src/casepy/combination_generator.py` & `casepy-0.0.4a1/src/casepy/combination_generator.py`

 * *Files identical despite different names*

### Comparing `casepy-0.0.4/src/casepy/simple_methods.py` & `casepy-0.0.4a1/src/casepy/simple_methods.py`

 * *Files identical despite different names*

### Comparing `casepy-0.0.4/src/casepy.egg-info/PKG-INFO` & `casepy-0.0.4a1/src/casepy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.4
+Version: 0.0.4a1
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -34,16 +34,15 @@
 With casepy, you can easily generate a combination of elements in a list.
 
 - Example
 
 Initialize generator
 
 ``` Python
-import casepy
-generator = casepy.CombinationGenerator()
+generator = CombinationGenerator()
 generator.set_parameters(4, [1,2,3,4,5])
 ```
 
 all_case()
 
 ``` Python
 all_case_list = generator.all_case()
```

