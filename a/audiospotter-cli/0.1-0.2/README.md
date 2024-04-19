# Comparing `tmp/audiospotter-cli-0.1.tar.gz` & `tmp/audiospotter_cli-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiospotter-cli-0.1.tar", last modified: Mon Mar 25 12:36:51 2024, max compression
+gzip compressed data, was "audiospotter_cli-0.2.tar", last modified: Fri Apr 19 00:46:26 2024, max compression
```

## Comparing `audiospotter-cli-0.1.tar` & `audiospotter_cli-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:36:51.512256 audiospotter-cli-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-25 12:36:36.000000 audiospotter-cli-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-25 12:36:51.512256 audiospotter-cli-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-25 12:36:36.000000 audiospotter-cli-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:36:51.512256 audiospotter-cli-0.1/audiospotter_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 12:36:36.000000 audiospotter-cli-0.1/audiospotter_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-25 12:36:36.000000 audiospotter-cli-0.1/audiospotter_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-25 12:36:36.000000 audiospotter-cli-0.1/audiospotter_cli/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-25 12:36:36.000000 audiospotter-cli-0.1/audiospotter_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-25 12:36:36.000000 audiospotter-cli-0.1/audiospotter_cli/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-25 12:36:36.000000 audiospotter-cli-0.1/audiospotter_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:36:51.512256 audiospotter-cli-0.1/audiospotter_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-25 12:36:51.000000 audiospotter-cli-0.1/audiospotter_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-25 12:36:51.000000 audiospotter-cli-0.1/audiospotter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 12:36:51.000000 audiospotter-cli-0.1/audiospotter_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-25 12:36:51.000000 audiospotter-cli-0.1/audiospotter_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-25 12:36:51.000000 audiospotter-cli-0.1/audiospotter_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-25 12:36:51.000000 audiospotter-cli-0.1/audiospotter_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-25 12:36:36.000000 audiospotter-cli-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 12:36:51.512256 audiospotter-cli-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 12:36:51.512256 audiospotter-cli-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-25 12:36:36.000000 audiospotter-cli-0.1/tests/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:46:26.608316 audiospotter_cli-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 00:46:13.000000 audiospotter_cli-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-19 00:46:26.608316 audiospotter_cli-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-19 00:46:13.000000 audiospotter_cli-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:46:26.604316 audiospotter_cli-0.2/audiospotter_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:46:13.000000 audiospotter_cli-0.2/audiospotter_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-19 00:46:13.000000 audiospotter_cli-0.2/audiospotter_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-19 00:46:13.000000 audiospotter_cli-0.2/audiospotter_cli/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-19 00:46:13.000000 audiospotter_cli-0.2/audiospotter_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-19 00:46:13.000000 audiospotter_cli-0.2/audiospotter_cli/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 00:46:13.000000 audiospotter_cli-0.2/audiospotter_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:46:26.608316 audiospotter_cli-0.2/audiospotter_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-19 00:46:26.000000 audiospotter_cli-0.2/audiospotter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-19 00:46:26.000000 audiospotter_cli-0.2/audiospotter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:46:26.000000 audiospotter_cli-0.2/audiospotter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 00:46:26.000000 audiospotter_cli-0.2/audiospotter_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 00:46:26.000000 audiospotter_cli-0.2/audiospotter_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 00:46:26.000000 audiospotter_cli-0.2/audiospotter_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-19 00:46:13.000000 audiospotter_cli-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 00:46:26.608316 audiospotter_cli-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:46:26.608316 audiospotter_cli-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 00:46:13.000000 audiospotter_cli-0.2/tests/test_connection.py
```

### Comparing `audiospotter-cli-0.1/LICENSE` & `audiospotter_cli-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audiospotter-cli-0.1/PKG-INFO` & `audiospotter_cli-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: audiospotter-cli
-Version: 0.1
+Version: 0.2
 Summary: A command-line tool for initializing projects and uploading audio to AudioSpotter API servers
 Author-email: Joe Weiss <joe.weiss@gmail.com>
 Project-URL: Homepage, https://github.com/joeweiss/audiospotter-cli
 Project-URL: Bug Tracker, https://github.com/joeweiss/audiospotter-cli/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cachetools
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: boto3
 Requires-Dist: click
 Requires-Dist: uplink
 Requires-Dist: PyYAML
+Requires-Dist: wavinfo
 
 # audiospotter-cli
 
 [![PyPI](https://img.shields.io/pypi/v/audiospotter-cli.svg)](https://pypi.org/project/audiospotter-cli/)
 [![Test](https://github.com/joeweiss/audiospotter-cli/actions/workflows/test.yml/badge.svg)](https://github.com/joeweiss/audiospotter-cli/actions/workflows/test.yml)
 
 A command-line tool for initializing projects and uploading audio to AudioSpotter API servers
```

### Comparing `audiospotter-cli-0.1/README.md` & `audiospotter_cli-0.2/README.md`

 * *Files identical despite different names*

### Comparing `audiospotter-cli-0.1/audiospotter_cli/client.py` & `audiospotter_cli-0.2/audiospotter_cli/client.py`

 * *Files identical despite different names*

### Comparing `audiospotter-cli-0.1/audiospotter_cli/config.py` & `audiospotter_cli-0.2/audiospotter_cli/config.py`

 * *Files identical despite different names*

### Comparing `audiospotter-cli-0.1/audiospotter_cli/sources.py` & `audiospotter_cli-0.2/audiospotter_cli/sources.py`

 * *Files identical despite different names*

### Comparing `audiospotter-cli-0.1/audiospotter_cli/utils.py` & `audiospotter_cli-0.2/audiospotter_cli/utils.py`

 * *Files identical despite different names*

### Comparing `audiospotter-cli-0.1/audiospotter_cli.egg-info/PKG-INFO` & `audiospotter_cli-0.2/audiospotter_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: audiospotter-cli
-Version: 0.1
+Version: 0.2
 Summary: A command-line tool for initializing projects and uploading audio to AudioSpotter API servers
 Author-email: Joe Weiss <joe.weiss@gmail.com>
 Project-URL: Homepage, https://github.com/joeweiss/audiospotter-cli
 Project-URL: Bug Tracker, https://github.com/joeweiss/audiospotter-cli/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cachetools
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: boto3
 Requires-Dist: click
 Requires-Dist: uplink
 Requires-Dist: PyYAML
+Requires-Dist: wavinfo
 
 # audiospotter-cli
 
 [![PyPI](https://img.shields.io/pypi/v/audiospotter-cli.svg)](https://pypi.org/project/audiospotter-cli/)
 [![Test](https://github.com/joeweiss/audiospotter-cli/actions/workflows/test.yml/badge.svg)](https://github.com/joeweiss/audiospotter-cli/actions/workflows/test.yml)
 
 A command-line tool for initializing projects and uploading audio to AudioSpotter API servers
```

### Comparing `audiospotter-cli-0.1/pyproject.toml` & `audiospotter_cli-0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "audiospotter-cli"
-version = "0.1"
+version = "0.2"
 authors = [{name="Joe Weiss", email="joe.weiss@gmail.com" }]
 description = "A command-line tool for initializing projects and uploading audio to AudioSpotter API servers"
 readme = "README.md"
-dependencies = ["cachetools","requests","rich","boto3","click","uplink","PyYAML"]
+dependencies = ["cachetools","requests","rich","boto3","click","uplink","PyYAML","wavinfo"]
 requires-python = ">=3.8"
 
 [project.scripts]
 audiospotter = "audiospotter_cli.cli:run"
 
 [project.urls]
 "Homepage" = "https://github.com/joeweiss/audiospotter-cli"
```

