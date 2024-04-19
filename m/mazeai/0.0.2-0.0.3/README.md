# Comparing `tmp/mazeai-0.0.2.tar.gz` & `tmp/mazeai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazeai-0.0.2.tar", last modified: Fri Apr 19 08:36:58 2024, max compression
+gzip compressed data, was "mazeai-0.0.3.tar", last modified: Fri Apr 19 11:11:39 2024, max compression
```

## Comparing `mazeai-0.0.2.tar` & `mazeai-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:58.726109 mazeai-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 08:36:54.000000 mazeai-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-19 08:36:58.726109 mazeai-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:54.000000 mazeai-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:58.722109 mazeai-0.0.2/maze/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:54.000000 mazeai-0.0.2/maze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 08:36:54.000000 mazeai-0.0.2/maze/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 08:36:54.000000 mazeai-0.0.2/maze/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 08:36:54.000000 mazeai-0.0.2/maze/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:58.726109 mazeai-0.0.2/mazeai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-19 08:36:58.000000 mazeai-0.0.2/mazeai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 08:36:58.000000 mazeai-0.0.2/mazeai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:36:58.000000 mazeai-0.0.2/mazeai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 08:36:58.000000 mazeai-0.0.2/mazeai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 08:36:58.000000 mazeai-0.0.2/mazeai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:36:58.726109 mazeai-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-19 08:36:54.000000 mazeai-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:11:39.178406 mazeai-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 11:11:32.000000 mazeai-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 11:11:39.178406 mazeai-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 11:11:32.000000 mazeai-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:11:39.178406 mazeai-0.0.3/maze/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:11:32.000000 mazeai-0.0.3/maze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 11:11:32.000000 mazeai-0.0.3/maze/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 11:11:32.000000 mazeai-0.0.3/maze/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 11:11:32.000000 mazeai-0.0.3/maze/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:11:39.178406 mazeai-0.0.3/mazeai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 11:11:39.000000 mazeai-0.0.3/mazeai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:11:39.178406 mazeai-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 11:11:32.000000 mazeai-0.0.3/setup.py
```

### Comparing `mazeai-0.0.2/LICENSE` & `mazeai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mazeai-0.0.2/setup.py` & `mazeai-0.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 import io
 import os
 import re
 
 from pathlib import Path
-from setuptools import find_packages
-from setuptools import setup
+from setuptools import find_packages, setup
 
 
 def read(filename):
     filename = os.path.join(os.path.dirname(__file__), filename)
-    text_type = type(u"")
-    with io.open(filename, mode="r", encoding='utf-8') as fd:
-        return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
+    text_type = type("")
+    with io.open(filename, mode="r", encoding="utf-8") as fd:
+        return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 def version():
-    """ Get the local package version. """
+    """Get the local package version."""
     namespace = {}
     path = Path("maze/__version__.py")
     exec(path.read_text(), namespace)
     return namespace["__version__"]
 
 
 setup(
     name="mazeai",
     version=version(),
     url="https://github.com/zhaisilong/mazeai",
-    license='MIT',
+    license="MIT",
     author="Zhai Silong",
     author_email="zhaisilong@outlook.com",
     description="A General Tool Set for Science Researches",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
-    packages=find_packages(where='.', exclude=('tests',), include=('*')),
-    package_data={'maze': ['resource/*']},
+    packages=find_packages(where=".", exclude=("tests",), include=("*")),
+    package_data={"maze": ["resource/*"]},
     entry_points={
-        'console_scripts': [
-            'maze = maze.__main__:main',
+        "console_scripts": [
+            "maze = maze.__main__:main",
         ],
     },
     install_requires=[
-        
+        "rich",
+        "ipykernel",
+        "tqdm",
+        "loguru",
+        "hydra-core",
     ],
-
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
+        "Development Status :: 2 - Pre-Alpha",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.7",
     ],
-    python_requires='>=3.6',  # The recommended least version of python
+    python_requires=">=3.6",  # The recommended least version of python
 )
```

