# Comparing `tmp/casepy-0.0.3.tar.gz` & `tmp/casepy-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casepy-0.0.3.tar", last modified: Fri Apr 19 06:39:34 2024, max compression
+gzip compressed data, was "casepy-0.0.3a1.tar", last modified: Fri Apr 19 07:33:29 2024, max compression
```

## Comparing `casepy-0.0.3.tar` & `casepy-0.0.3a1.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:39:34.243067 casepy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 06:39:27.000000 casepy-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-19 06:39:34.243067 casepy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-19 06:39:27.000000 casepy-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 06:39:34.243067 casepy-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 06:39:27.000000 casepy-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:39:34.243067 casepy-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:39:34.243067 casepy-0.0.3/src/casepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-19 06:39:34.000000 casepy-0.0.3/src/casepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 06:39:34.000000 casepy-0.0.3/src/casepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:39:34.000000 casepy-0.0.3/src/casepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:39:34.000000 casepy-0.0.3/src/casepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:33:29.320043 casepy-0.0.3a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 07:33:19.000000 casepy-0.0.3a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 07:33:29.320043 casepy-0.0.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-19 07:33:19.000000 casepy-0.0.3a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:33:29.320043 casepy-0.0.3a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 07:33:19.000000 casepy-0.0.3a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:33:29.320043 casepy-0.0.3a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:33:29.320043 casepy-0.0.3a1/src/casepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 07:33:19.000000 casepy-0.0.3a1/src/casepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-19 07:33:19.000000 casepy-0.0.3a1/src/casepy/combination_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 07:33:19.000000 casepy-0.0.3a1/src/casepy/simple_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:33:29.320043 casepy-0.0.3a1/src/casepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 07:33:29.000000 casepy-0.0.3a1/src/casepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-19 07:33:29.000000 casepy-0.0.3a1/src/casepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:33:29.000000 casepy-0.0.3a1/src/casepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 07:33:29.000000 casepy-0.0.3a1/src/casepy.egg-info/top_level.txt
```

### Comparing `casepy-0.0.3/LICENSE` & `casepy-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `casepy-0.0.3/PKG-INFO` & `casepy-0.0.3a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.3
+Version: 0.0.3a1
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
-Requires-Python: >2.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # casepy
 
 A Python package for generating cases in a list.
```

### Comparing `casepy-0.0.3/README.md` & `casepy-0.0.3a1/README.md`

 * *Files identical despite different names*

### Comparing `casepy-0.0.3/setup.py` & `casepy-0.0.3a1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="casepy",
-    version="0.0.3",
+    py_modules=["casepy"],
+    version="0.0.3a1",
     description="A Python package for generating cases in a list.",
     url="https://github.com/DongHoon5793/casepy",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     author="DongHoon Kim",
     author_email="donghoon5793@gmail.com",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
-    python_requires=">2.7.0",
+    # python_requires=">=2.7.0",
     install_requires=[],
 )
```

### Comparing `casepy-0.0.3/src/casepy.egg-info/PKG-INFO` & `casepy-0.0.3a1/src/casepy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: casepy
-Version: 0.0.3
+Version: 0.0.3a1
 Summary: A Python package for generating cases in a list.
 Home-page: https://github.com/DongHoon5793/casepy
 Author: DongHoon Kim
 Author-email: donghoon5793@gmail.com
 License: MIT
 Platform: UNKNOWN
-Requires-Python: >2.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # casepy
 
 A Python package for generating cases in a list.
```

