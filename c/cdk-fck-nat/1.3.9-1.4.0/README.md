# Comparing `tmp/cdk-fck-nat-1.3.9.tar.gz` & `tmp/cdk-fck-nat-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-fck-nat-1.3.9.tar", last modified: Fri Mar  1 20:12:19 2024, max compression
+gzip compressed data, was "cdk-fck-nat-1.4.0.tar", last modified: Fri Apr 19 06:44:04 2024, max compression
```

## Comparing `cdk-fck-nat-1.3.9.tar` & `cdk-fck-nat-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:12:19.976192 cdk-fck-nat-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-01 20:12:08.000000 cdk-fck-nat-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-01 20:12:08.000000 cdk-fck-nat-1.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-03-01 20:12:19.976192 cdk-fck-nat-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-01 20:12:08.000000 cdk-fck-nat-1.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-01 20:12:08.000000 cdk-fck-nat-1.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 20:12:19.976192 cdk-fck-nat-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-01 20:12:08.000000 cdk-fck-nat-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:12:19.976192 cdk-fck-nat-1.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:12:19.976192 cdk-fck-nat-1.3.9/src/cdk_fck_nat/
--rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-03-01 20:12:08.000000 cdk-fck-nat-1.3.9/src/cdk_fck_nat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:12:19.976192 cdk-fck-nat-1.3.9/src/cdk_fck_nat/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-01 20:12:08.000000 cdk-fck-nat-1.3.9/src/cdk_fck_nat/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31551 2024-03-01 20:12:08.000000 cdk-fck-nat-1.3.9/src/cdk_fck_nat/_jsii/cdk-fck-nat@1.3.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 20:12:08.000000 cdk-fck-nat-1.3.9/src/cdk_fck_nat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:12:19.976192 cdk-fck-nat-1.3.9/src/cdk_fck_nat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-03-01 20:12:19.000000 cdk-fck-nat-1.3.9/src/cdk_fck_nat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-01 20:12:19.000000 cdk-fck-nat-1.3.9/src/cdk_fck_nat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 20:12:19.000000 cdk-fck-nat-1.3.9/src/cdk_fck_nat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-01 20:12:19.000000 cdk-fck-nat-1.3.9/src/cdk_fck_nat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-01 20:12:19.000000 cdk-fck-nat-1.3.9/src/cdk_fck_nat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:44:04.363021 cdk-fck-nat-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-19 06:43:53.000000 cdk-fck-nat-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 06:43:53.000000 cdk-fck-nat-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-19 06:44:04.363021 cdk-fck-nat-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-19 06:43:53.000000 cdk-fck-nat-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-19 06:43:53.000000 cdk-fck-nat-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 06:44:04.363021 cdk-fck-nat-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-19 06:43:53.000000 cdk-fck-nat-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:44:04.363021 cdk-fck-nat-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:44:04.363021 cdk-fck-nat-1.4.0/src/cdk_fck_nat/
+-rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-04-19 06:43:53.000000 cdk-fck-nat-1.4.0/src/cdk_fck_nat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:44:04.363021 cdk-fck-nat-1.4.0/src/cdk_fck_nat/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-19 06:43:53.000000 cdk-fck-nat-1.4.0/src/cdk_fck_nat/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-04-19 06:43:53.000000 cdk-fck-nat-1.4.0/src/cdk_fck_nat/_jsii/cdk-fck-nat@1.4.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:43:53.000000 cdk-fck-nat-1.4.0/src/cdk_fck_nat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:44:04.363021 cdk-fck-nat-1.4.0/src/cdk_fck_nat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-19 06:44:04.000000 cdk-fck-nat-1.4.0/src/cdk_fck_nat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 06:44:04.000000 cdk-fck-nat-1.4.0/src/cdk_fck_nat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:44:04.000000 cdk-fck-nat-1.4.0/src/cdk_fck_nat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-19 06:44:04.000000 cdk-fck-nat-1.4.0/src/cdk_fck_nat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 06:44:04.000000 cdk-fck-nat-1.4.0/src/cdk_fck_nat.egg-info/top_level.txt
```

### Comparing `cdk-fck-nat-1.3.9/LICENSE` & `cdk-fck-nat-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-fck-nat-1.3.9/PKG-INFO` & `cdk-fck-nat-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-fck-nat
-Version: 1.3.9
+Version: 1.4.0
 Summary: A NAT Gateway instance construct built on the fck-nat AMI.
 Home-page: https://github.com/AndrewGuenther/cdk-fck-nat.git
 Author: Andrew Guenther<guenther.andrew.j@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/AndrewGuenther/cdk-fck-nat.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-fck-nat-1.3.9/README.md` & `cdk-fck-nat-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-fck-nat-1.3.9/setup.py` & `cdk-fck-nat-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-fck-nat",
-    "version": "1.3.9",
+    "version": "1.4.0",
     "description": "A NAT Gateway instance construct built on the fck-nat AMI.",
     "license": "MIT",
     "url": "https://github.com/AndrewGuenther/cdk-fck-nat.git",
     "long_description_content_type": "text/markdown",
     "author": "Andrew Guenther<guenther.andrew.j@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_fck_nat",
         "cdk_fck_nat._jsii"
     ],
     "package_data": {
         "cdk_fck_nat._jsii": [
-            "cdk-fck-nat@1.3.9.jsii.tgz"
+            "cdk-fck-nat@1.4.0.jsii.tgz"
         ],
         "cdk_fck_nat": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-fck-nat-1.3.9/src/cdk_fck_nat/__init__.py` & `cdk-fck-nat-1.4.0/src/cdk_fck_nat/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-fck-nat-1.3.9/src/cdk_fck_nat.egg-info/PKG-INFO` & `cdk-fck-nat-1.4.0/src/cdk_fck_nat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-fck-nat
-Version: 1.3.9
+Version: 1.4.0
 Summary: A NAT Gateway instance construct built on the fck-nat AMI.
 Home-page: https://github.com/AndrewGuenther/cdk-fck-nat.git
 Author: Andrew Guenther<guenther.andrew.j@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/AndrewGuenther/cdk-fck-nat.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

