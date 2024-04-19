# Comparing `tmp/aruba_dero-1.0.4.tar.gz` & `tmp/aruba_dero-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aruba_dero-1.0.4.tar", last modified: Fri Apr 19 09:58:26 2024, max compression
+gzip compressed data, was "aruba_dero-1.0.5.tar", last modified: Fri Apr 19 10:07:41 2024, max compression
```

## Comparing `aruba_dero-1.0.4.tar` & `aruba_dero-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:58:26.953267 aruba_dero-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 09:58:26.953267 aruba_dero-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-19 09:58:23.000000 aruba_dero-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-19 09:58:23.000000 aruba_dero-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:58:26.953267 aruba_dero-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:58:26.949267 aruba_dero-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:58:26.953267 aruba_dero-1.0.4/src/aruba_dero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 09:58:26.000000 aruba_dero-1.0.4/src/aruba_dero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 09:58:26.000000 aruba_dero-1.0.4/src/aruba_dero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:58:26.000000 aruba_dero-1.0.4/src/aruba_dero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 09:58:26.000000 aruba_dero-1.0.4/src/aruba_dero.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 09:58:26.000000 aruba_dero-1.0.4/src/aruba_dero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 09:58:26.000000 aruba_dero-1.0.4/src/aruba_dero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:58:26.953267 aruba_dero-1.0.4/src/dero-modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:58:23.000000 aruba_dero-1.0.4/src/dero-modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:58:26.953267 aruba_dero-1.0.4/src/dero-modules/clearpass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:58:23.000000 aruba_dero-1.0.4/src/dero-modules/clearpass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15281 2024-04-19 09:58:23.000000 aruba_dero-1.0.4/src/dero-modules/clearpass/clearpass.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 09:58:23.000000 aruba_dero-1.0.4/src/dero-modules/clearpass/module.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 09:58:23.000000 aruba_dero-1.0.4/src/dero-modules/clearpass/temp_webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-19 09:58:23.000000 aruba_dero-1.0.4/src/dero-modules/clearpass/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-19 09:58:23.000000 aruba_dero-1.0.4/src/dero-modules/clearpass/webserver-process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:41.235001 aruba_dero-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 10:07:41.231001 aruba_dero-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:07:41.235001 aruba_dero-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:41.231001 aruba_dero-1.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/Module.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:41.231001 aruba_dero-1.0.5/src/aruba_dero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 10:07:41.000000 aruba_dero-1.0.5/src/aruba_dero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-19 10:07:41.000000 aruba_dero-1.0.5/src/aruba_dero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:07:41.000000 aruba_dero-1.0.5/src/aruba_dero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 10:07:41.000000 aruba_dero-1.0.5/src/aruba_dero.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 10:07:41.000000 aruba_dero-1.0.5/src/aruba_dero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 10:07:41.000000 aruba_dero-1.0.5/src/aruba_dero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:41.231001 aruba_dero-1.0.5/src/dero-modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/dero-modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:41.231001 aruba_dero-1.0.5/src/dero-modules/clearpass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/dero-modules/clearpass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15281 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/dero-modules/clearpass/clearpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/dero-modules/clearpass/module.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/dero-modules/clearpass/temp_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/dero-modules/clearpass/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/dero-modules/clearpass/webserver-process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-19 10:07:34.000000 aruba_dero-1.0.5/src/utils.py
```

### Comparing `aruba_dero-1.0.4/PKG-INFO` & `aruba_dero-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aruba-dero
-Version: 1.0.4
+Version: 1.0.5
 Summary: DEmo ROllout helper - Modular Tool to automate demo rollouts
 Author-email: Lukas Lanzner <lukas.lanzner@hpe.com>
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pyclearpass>=1.0.4
 Requires-Dist: psutil~=5.9.8
 Requires-Dist: pyyaml~=6.0.1
```

### Comparing `aruba_dero-1.0.4/README.md` & `aruba_dero-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.4/pyproject.toml` & `aruba_dero-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aruba-dero"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     { name = "Lukas Lanzner", email = "lukas.lanzner@hpe.com" },
 ]
 description = "DEmo ROllout helper - Modular Tool to automate demo rollouts"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = [
     'pyclearpass >= 1.0.4',
     'psutil~=5.9.8',
     'pyyaml~=6.0.1',
     'cryptography~=42.0.5',
     'winBullet~=1.1',
     'setuptools~=69.2.0'
 ]
-[tool.setuptools.packages.find]
-where = ["src"]
 
 [tool.setuptools.package-data]
 "*" = ["**/module.yml"]
 
 [project.scripts]
 dero = "main:main"
```

### Comparing `aruba_dero-1.0.4/src/aruba_dero.egg-info/PKG-INFO` & `aruba_dero-1.0.5/src/aruba_dero.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aruba-dero
-Version: 1.0.4
+Version: 1.0.5
 Summary: DEmo ROllout helper - Modular Tool to automate demo rollouts
 Author-email: Lukas Lanzner <lukas.lanzner@hpe.com>
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pyclearpass>=1.0.4
 Requires-Dist: psutil~=5.9.8
 Requires-Dist: pyyaml~=6.0.1
```

### Comparing `aruba_dero-1.0.4/src/aruba_dero.egg-info/SOURCES.txt` & `aruba_dero-1.0.5/src/aruba_dero.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 README.md
 pyproject.toml
+src/Module.py
+src/__init__.py
+src/main.py
+src/utils.py
 src/aruba_dero.egg-info/PKG-INFO
 src/aruba_dero.egg-info/SOURCES.txt
 src/aruba_dero.egg-info/dependency_links.txt
 src/aruba_dero.egg-info/entry_points.txt
 src/aruba_dero.egg-info/requires.txt
 src/aruba_dero.egg-info/top_level.txt
 src/dero-modules/__init__.py
```

### Comparing `aruba_dero-1.0.4/src/dero-modules/clearpass/clearpass.py` & `aruba_dero-1.0.5/src/dero-modules/clearpass/clearpass.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.4/src/dero-modules/clearpass/temp_webserver.py` & `aruba_dero-1.0.5/src/dero-modules/clearpass/temp_webserver.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.4/src/dero-modules/clearpass/utils.py` & `aruba_dero-1.0.5/src/dero-modules/clearpass/utils.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.4/src/dero-modules/clearpass/webserver-process.py` & `aruba_dero-1.0.5/src/dero-modules/clearpass/webserver-process.py`

 * *Files identical despite different names*

