# Comparing `tmp/ai-models-0.5.2.tar.gz` & `tmp/ai-models-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-models-0.5.2.tar", last modified: Tue Apr 16 13:10:20 2024, max compression
+gzip compressed data, was "ai-models-0.5.3.tar", last modified: Fri Apr 19 12:46:10 2024, max compression
```

## Comparing `ai-models-0.5.2.tar` & `ai-models-0.5.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.093562 ai-models-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 13:10:08.000000 ai-models-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-16 13:10:20.093562 ai-models-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-16 13:10:08.000000 ai-models-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.089562 ai-models-0.5.2/ai_models/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.089562 ai-models-0.5.2/ai_models/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.089562 ai-models-0.5.2/ai_models/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/outputs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.093562 ai-models-0.5.2/ai_models/remote/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/remote/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/remote/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/remote/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-16 13:10:08.000000 ai-models-0.5.2/ai_models/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:10:20.089562 ai-models-0.5.2/ai_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:10:20.000000 ai-models-0.5.2/ai_models.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:10:20.093562 ai-models-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-16 13:10:08.000000 ai-models-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 12:46:02.000000 ai-models-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-19 12:46:10.285175 ai-models-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-19 12:46:02.000000 ai-models-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/ai_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/ai_models/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/ai_models/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/outputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/ai_models/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/remote/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/remote/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/remote/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-19 12:46:02.000000 ai-models-0.5.3/ai_models/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:46:10.285175 ai-models-0.5.3/ai_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:46:10.000000 ai-models-0.5.3/ai_models.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 12:46:10.285175 ai-models-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-19 12:46:02.000000 ai-models-0.5.3/setup.py
```

### Comparing `ai-models-0.5.2/LICENSE` & `ai-models-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/PKG-INFO` & `ai-models-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-models
-Version: 0.5.2
+Version: 0.5.3
 Summary: A package to run AI weather models
 Home-page: https://github.com/ecmwf-lab/ai-models
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ai-models-0.5.2/README.md` & `ai-models-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/ai_models/__main__.py` & `ai-models-0.5.3/ai_models/__main__.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/ai_models/checkpoint.py` & `ai-models-0.5.3/ai_models/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/ai_models/inputs/__init__.py` & `ai-models-0.5.3/ai_models/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/ai_models/model.py` & `ai-models-0.5.3/ai_models/model.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/ai_models/outputs/__init__.py` & `ai-models-0.5.3/ai_models/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/ai_models/remote/api.py` & `ai-models-0.5.3/ai_models/remote/api.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/ai_models/remote/config.py` & `ai-models-0.5.3/ai_models/remote/config.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/ai_models/remote/model.py` & `ai-models-0.5.3/ai_models/remote/model.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/ai_models/stepper.py` & `ai-models-0.5.3/ai_models/stepper.py`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/ai_models.egg-info/PKG-INFO` & `ai-models-0.5.3/ai_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-models
-Version: 0.5.2
+Version: 0.5.3
 Summary: A package to run AI weather models
 Home-page: https://github.com/ecmwf-lab/ai-models
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ai-models-0.5.2/ai_models.egg-info/SOURCES.txt` & `ai-models-0.5.3/ai_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai-models-0.5.2/setup.py` & `ai-models-0.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 
 
 import io
 import os
 
 import setuptools
-from setuptools.command.install import install
 
 
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return io.open(file_path, encoding="utf-8").read()
 
 
@@ -26,41 +25,29 @@
     if line.startswith("__version__"):
         version = line.split("=")[-1].strip()[1:-1]
 
 
 assert version
 
 
-class PostInstall(install):
-    def run(self):
-        from ai_models.remote.config import config_exists, create_config
-
-        if not config_exists():
-            create_config()
-
-        install.run(self)
-
-
 setuptools.setup(
     name="ai-models",
     version=version,
     description="A package to run AI weather models",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="European Centre for Medium-Range Weather Forecasts (ECMWF)",
     author_email="software.support@ecmwf.int",
     license="Apache License Version 2.0",
     url="https://github.com/ecmwf-lab/ai-models",
     packages=setuptools.find_packages(),
     include_package_data=True,
-    cmdclass={
-        "install": PostInstall,
-    },
     install_requires=[
         "entrypoints",
+        "requests",
         "climetlab>=0.20.11",
         "multiurl",
         "ecmwflibs>=0.6.1",
         "gputil",
         "earthkit-meteo",
         "pyyaml",
         "tqdm",
```

