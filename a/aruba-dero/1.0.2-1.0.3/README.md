# Comparing `tmp/aruba_dero-1.0.2.tar.gz` & `tmp/aruba_dero-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aruba_dero-1.0.2.tar", last modified: Fri Apr 19 09:42:02 2024, max compression
+gzip compressed data, was "aruba_dero-1.0.3.tar", last modified: Fri Apr 19 09:56:01 2024, max compression
```

## Comparing `aruba_dero-1.0.2.tar` & `aruba_dero-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:42:02.276400 aruba_dero-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 09:42:02.276400 aruba_dero-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-19 09:41:58.000000 aruba_dero-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-19 09:41:58.000000 aruba_dero-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:42:02.276400 aruba_dero-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:42:02.272400 aruba_dero-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:42:02.272400 aruba_dero-1.0.2/src/dero-modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:42:02.276400 aruba_dero-1.0.2/src/dero-modules/aruba_dero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 09:42:02.000000 aruba_dero-1.0.2/src/dero-modules/aruba_dero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-19 09:42:02.000000 aruba_dero-1.0.2/src/dero-modules/aruba_dero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:42:02.000000 aruba_dero-1.0.2/src/dero-modules/aruba_dero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 09:42:02.000000 aruba_dero-1.0.2/src/dero-modules/aruba_dero.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 09:42:02.000000 aruba_dero-1.0.2/src/dero-modules/aruba_dero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 09:42:02.000000 aruba_dero-1.0.2/src/dero-modules/aruba_dero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:42:02.276400 aruba_dero-1.0.2/src/dero-modules/clearpass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:41:58.000000 aruba_dero-1.0.2/src/dero-modules/clearpass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15281 2024-04-19 09:41:58.000000 aruba_dero-1.0.2/src/dero-modules/clearpass/clearpass.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 09:41:58.000000 aruba_dero-1.0.2/src/dero-modules/clearpass/module.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 09:41:58.000000 aruba_dero-1.0.2/src/dero-modules/clearpass/temp_webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-19 09:41:58.000000 aruba_dero-1.0.2/src/dero-modules/clearpass/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-19 09:41:58.000000 aruba_dero-1.0.2/src/dero-modules/clearpass/webserver-process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:56:01.717273 aruba_dero-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 09:56:01.717273 aruba_dero-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-19 09:55:54.000000 aruba_dero-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 09:55:54.000000 aruba_dero-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:56:01.717273 aruba_dero-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:56:01.713273 aruba_dero-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:56:01.717273 aruba_dero-1.0.3/src/aruba_dero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 09:56:01.000000 aruba_dero-1.0.3/src/aruba_dero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 09:56:01.000000 aruba_dero-1.0.3/src/aruba_dero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:56:01.000000 aruba_dero-1.0.3/src/aruba_dero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 09:56:01.000000 aruba_dero-1.0.3/src/aruba_dero.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 09:56:01.000000 aruba_dero-1.0.3/src/aruba_dero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 09:56:01.000000 aruba_dero-1.0.3/src/aruba_dero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:56:01.713273 aruba_dero-1.0.3/src/dero-modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:54.000000 aruba_dero-1.0.3/src/dero-modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:56:01.713273 aruba_dero-1.0.3/src/dero-modules/clearpass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:54.000000 aruba_dero-1.0.3/src/dero-modules/clearpass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15281 2024-04-19 09:55:54.000000 aruba_dero-1.0.3/src/dero-modules/clearpass/clearpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 09:55:54.000000 aruba_dero-1.0.3/src/dero-modules/clearpass/module.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 09:55:54.000000 aruba_dero-1.0.3/src/dero-modules/clearpass/temp_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-19 09:55:54.000000 aruba_dero-1.0.3/src/dero-modules/clearpass/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-19 09:55:54.000000 aruba_dero-1.0.3/src/dero-modules/clearpass/webserver-process.py
```

### Comparing `aruba_dero-1.0.2/PKG-INFO` & `aruba_dero-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aruba-dero
-Version: 1.0.2
+Version: 1.0.3
 Summary: DEmo ROllout helper - Modular Tool to automate demo rollouts
 Author-email: Lukas Lanzner <lukas.lanzner@hpe.com>
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pyclearpass>=1.0.4
 Requires-Dist: psutil~=5.9.8
 Requires-Dist: pyyaml~=6.0.1
```

### Comparing `aruba_dero-1.0.2/README.md` & `aruba_dero-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.2/pyproject.toml` & `aruba_dero-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aruba-dero"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     { name = "Lukas Lanzner", email = "lukas.lanzner@hpe.com" },
 ]
 description = "DEmo ROllout helper - Modular Tool to automate demo rollouts"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = [
@@ -16,14 +16,14 @@
     'psutil~=5.9.8',
     'pyyaml~=6.0.1',
     'cryptography~=42.0.5',
     'winBullet~=1.1',
     'setuptools~=69.2.0'
 ]
 [tool.setuptools.packages.find]
-where = ["src/dero-modules"]
+where = ["src"]
 
 [tool.setuptools.package-data]
-"*" = ["module.yml"]
+"*" = ["**/module.yml"]
 
 [project.scripts]
 dero = "src.main:main"
```

### Comparing `aruba_dero-1.0.2/src/dero-modules/aruba_dero.egg-info/PKG-INFO` & `aruba_dero-1.0.3/src/aruba_dero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aruba-dero
-Version: 1.0.2
+Version: 1.0.3
 Summary: DEmo ROllout helper - Modular Tool to automate demo rollouts
 Author-email: Lukas Lanzner <lukas.lanzner@hpe.com>
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pyclearpass>=1.0.4
 Requires-Dist: psutil~=5.9.8
 Requires-Dist: pyyaml~=6.0.1
```

### Comparing `aruba_dero-1.0.2/src/dero-modules/clearpass/clearpass.py` & `aruba_dero-1.0.3/src/dero-modules/clearpass/clearpass.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.2/src/dero-modules/clearpass/temp_webserver.py` & `aruba_dero-1.0.3/src/dero-modules/clearpass/temp_webserver.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.2/src/dero-modules/clearpass/utils.py` & `aruba_dero-1.0.3/src/dero-modules/clearpass/utils.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.2/src/dero-modules/clearpass/webserver-process.py` & `aruba_dero-1.0.3/src/dero-modules/clearpass/webserver-process.py`

 * *Files identical despite different names*

