# Comparing `tmp/meta_ai_api-1.0.5.tar.gz` & `tmp/meta_ai_api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.0.5.tar", last modified: Thu Apr 18 22:04:17 2024, max compression
+gzip compressed data, was "meta_ai_api-1.0.6.tar", last modified: Thu Apr 18 22:58:04 2024, max compression
```

## Comparing `meta_ai_api-1.0.5.tar` & `meta_ai_api-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:04:17.835620 meta_ai_api-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 22:04:17.835620 meta_ai_api-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-18 22:04:12.000000 meta_ai_api-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 22:04:12.000000 meta_ai_api-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 22:04:17.835620 meta_ai_api-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 22:04:12.000000 meta_ai_api-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:04:17.831620 meta_ai_api-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:04:17.831620 meta_ai_api-1.0.5/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 22:04:12.000000 meta_ai_api-1.0.5/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-18 22:04:12.000000 meta_ai_api-1.0.5/src/meta_ai_api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:04:17.835620 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 22:04:17.000000 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 22:04:17.000000 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:04:17.000000 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 22:04:17.000000 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 22:04:17.000000 meta_ai_api-1.0.5/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:58:04.779576 meta_ai_api-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 22:58:04.779576 meta_ai_api-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-18 22:57:59.000000 meta_ai_api-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 22:57:59.000000 meta_ai_api-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 22:58:04.779576 meta_ai_api-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 22:57:59.000000 meta_ai_api-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:58:04.775576 meta_ai_api-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:58:04.775576 meta_ai_api-1.0.6/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 22:57:59.000000 meta_ai_api-1.0.6/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-18 22:57:59.000000 meta_ai_api-1.0.6/src/meta_ai_api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:58:04.779576 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-18 22:58:04.000000 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 22:58:04.000000 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:58:04.000000 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 22:58:04.000000 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 22:58:04.000000 meta_ai_api-1.0.6/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.0.5/PKG-INFO` & `meta_ai_api-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
```

### Comparing `meta_ai_api-1.0.5/README.md` & `meta_ai_api-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.5/setup.py` & `meta_ai_api-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.5/src/meta_ai_api.egg-info/PKG-INFO` & `meta_ai_api-1.0.6/src/meta_ai_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta_ai_api
-Version: 1.0.5
+Version: 1.0.6
 Summary: Meta AI API Wrapper to interact with the Meta AI API
 Home-page: https://github.com/tomchen/example_pypi_package
 Author: Roméo Phillips
 Author-email: phillipsromeo@gmail.com
 Project-URL: Documentation, https://github.com/Strvm/meta-ai-api
 Project-URL: Bug Reports, https://github.com/Strvm/meta-ai-api
 Project-URL: Source Code, https://github.com/Strvm/meta-ai-api
```

