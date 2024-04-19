# Comparing `tmp/casepy-0.0.3a1.tar.gz` & `tmp/casepy-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casepy-0.0.3a1.tar", last modified: Fri Apr 19 07:33:29 2024, max compression
+gzip compressed data, was "casepy-0.0.4a1.tar", last modified: Fri Apr 19 07:46:33 2024, max compression
```

## Comparing `casepy-0.0.3a1.tar` & `casepy-0.0.4a1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:33:29.320043 casepy-0.0.3a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 07:33:19.000000 casepy-0.0.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 07:33:29.320043 casepy-0.0.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-19 07:33:19.000000 casepy-0.0.3a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:33:29.320043 casepy-0.0.3a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 07:33:19.000000 casepy-0.0.3a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:33:29.320043 casepy-0.0.3a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:33:29.320043 casepy-0.0.3a1/src/casepy/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 07:33:19.000000 casepy-0.0.3a1/src/casepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-19 07:33:19.000000 casepy-0.0.3a1/src/casepy/combination_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 07:33:19.000000 casepy-0.0.3a1/src/casepy/simple_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:33:29.320043 casepy-0.0.3a1/src/casepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 07:33:29.000000 casepy-0.0.3a1/src/casepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-19 07:33:29.000000 casepy-0.0.3a1/src/casepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:33:29.000000 casepy-0.0.3a1/src/casepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 07:33:29.000000 casepy-0.0.3a1/src/casepy.egg-info/top_level.txt
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

### Comparing `casepy-0.0.3a1/LICENSE` & `casepy-0.0.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `casepy-0.0.3a1/PKG-INFO` & `casepy-0.0.4a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.3a1
+Version: 0.0.4a1
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `casepy-0.0.3a1/README.md` & `casepy-0.0.4a1/README.md`

 * *Files identical despite different names*

### Comparing `casepy-0.0.3a1/setup.py` & `casepy-0.0.4a1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="casepy",
     py_modules=["casepy"],
-    version="0.0.3a1",
+    version="0.0.4a1",
     description="A Python package for generating cases in a list.",
     url="https://github.com/DongHoon5793/casepy",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     author="DongHoon Kim",
     author_email="donghoon5793@gmail.com",
```

### Comparing `casepy-0.0.3a1/src/casepy/combination_generator.py` & `casepy-0.0.4a1/src/casepy/combination_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import simple_methods
+from .simple_methods import combination
 import random
 
 
 class CombinationGenerator:
 
     def __init__(self):
         self.element_list_initialized = False
@@ -10,17 +10,15 @@
 
     def set_parameters(self, in_number_of_selection: int, element_list: list):
         self.in_number_of_selection = in_number_of_selection
         self.element_list = element_list
 
         self.element_list_initialized = True
         self.number_of_selection_initialized = True
-        self.max_possible = simple_methods.combination(
-            len(element_list), in_number_of_selection
-        )
+        self.max_possible = combination(len(element_list), in_number_of_selection)
 
     def all_case(self) -> list:
         if not self.element_list_initialized:
             raise Exception("element_list is not initialized")
         if not self.number_of_selection_initialized:
             raise Exception("number_of_selection is not initialized")
 
@@ -69,29 +67,25 @@
     #     )
 
     def combination_core(
         self, in_iterator: int, in_number_of_selection: int, element_list: list
     ) -> list:
         result_list = []
         number_of_elements = len(element_list)
-        max_possible = simple_methods.combination(
-            number_of_elements, in_number_of_selection
-        )
+        max_possible = combination(number_of_elements, in_number_of_selection)
 
         if in_iterator >= max_possible:
             return []
 
         target_iterator = 0
         while True:
             if in_number_of_selection == 0:
                 break
 
-            test = simple_methods.combination(
-                number_of_elements - 1, in_number_of_selection - 1
-            )
+            test = combination(number_of_elements - 1, in_number_of_selection - 1)
 
             if in_iterator >= test:
                 in_iterator -= test
 
                 number_of_elements -= 1
 
                 target_iterator += 1
```

### Comparing `casepy-0.0.3a1/src/casepy/simple_methods.py` & `casepy-0.0.4a1/src/casepy/simple_methods.py`

 * *Files identical despite different names*

### Comparing `casepy-0.0.3a1/src/casepy.egg-info/PKG-INFO` & `casepy-0.0.4a1/src/casepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.3a1
+Version: 0.0.4a1
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

