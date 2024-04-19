# Comparing `tmp/gspread_models-1.0.2.tar.gz` & `tmp/gspread_models-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspread_models-1.0.2.tar", last modified: Tue Mar 26 22:17:32 2024, max compression
+gzip compressed data, was "gspread_models-1.0.3.tar", last modified: Fri Apr 19 20:04:28 2024, max compression
```

## Comparing `gspread_models-1.0.2.tar` & `gspread_models-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:17:32.392211 gspread_models-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-26 22:17:28.000000 gspread_models-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-26 22:17:32.392211 gspread_models-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-26 22:17:28.000000 gspread_models-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:17:32.392211 gspread_models-1.0.2/gspread_models/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-26 22:17:28.000000 gspread_models-1.0.2/gspread_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-03-26 22:17:28.000000 gspread_models-1.0.2/gspread_models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-26 22:17:28.000000 gspread_models-1.0.2/gspread_models/date_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-26 22:17:28.000000 gspread_models-1.0.2/gspread_models/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:17:32.392211 gspread_models-1.0.2/gspread_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-26 22:17:32.000000 gspread_models-1.0.2/gspread_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-26 22:17:32.000000 gspread_models-1.0.2/gspread_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 22:17:32.000000 gspread_models-1.0.2/gspread_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 22:17:32.000000 gspread_models-1.0.2/gspread_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-26 22:17:32.000000 gspread_models-1.0.2/gspread_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 22:17:32.392211 gspread_models-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-26 22:17:28.000000 gspread_models-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:04:28.285833 gspread_models-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 20:04:14.000000 gspread_models-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-19 20:04:28.285833 gspread_models-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-19 20:04:14.000000 gspread_models-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:04:28.285833 gspread_models-1.0.3/gspread_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 20:04:14.000000 gspread_models-1.0.3/gspread_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-19 20:04:14.000000 gspread_models-1.0.3/gspread_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-19 20:04:14.000000 gspread_models-1.0.3/gspread_models/date_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-19 20:04:14.000000 gspread_models-1.0.3/gspread_models/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:04:28.285833 gspread_models-1.0.3/gspread_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-19 20:04:28.000000 gspread_models-1.0.3/gspread_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-19 20:04:28.000000 gspread_models-1.0.3/gspread_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:04:28.000000 gspread_models-1.0.3/gspread_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-19 20:04:28.000000 gspread_models-1.0.3/gspread_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 20:04:28.000000 gspread_models-1.0.3/gspread_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:04:28.285833 gspread_models-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-19 20:04:14.000000 gspread_models-1.0.3/setup.py
```

### Comparing `gspread_models-1.0.2/LICENSE` & `gspread_models-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gspread_models-1.0.2/PKG-INFO` & `gspread_models-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread_models
-Version: 1.0.2
+Version: 1.0.3
 Summary: Model based ORM interface into Google Sheets, using the gspread package.
 Home-page: https://github.com/s2t2/gspread-models-py
 Author: Michael Rossetti
 Author-email: datacreativellc@gmail.com
 License: MIT
 Keywords: google sheets gspread models orm spreadsheet
 Description-Content-Type: text/markdown
```

### Comparing `gspread_models-1.0.2/README.md` & `gspread_models-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gspread_models-1.0.2/gspread_models/base.py` & `gspread_models-1.0.3/gspread_models/base.py`

 * *Files identical despite different names*

### Comparing `gspread_models-1.0.2/gspread_models/date_parser.py` & `gspread_models-1.0.3/gspread_models/date_parser.py`

 * *Files identical despite different names*

### Comparing `gspread_models-1.0.2/gspread_models/service.py` & `gspread_models-1.0.3/gspread_models/service.py`

 * *Files identical despite different names*

### Comparing `gspread_models-1.0.2/gspread_models.egg-info/PKG-INFO` & `gspread_models-1.0.3/gspread_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread_models
-Version: 1.0.2
+Version: 1.0.3
 Summary: Model based ORM interface into Google Sheets, using the gspread package.
 Home-page: https://github.com/s2t2/gspread-models-py
 Author: Michael Rossetti
 Author-email: datacreativellc@gmail.com
 License: MIT
 Keywords: google sheets gspread models orm spreadsheet
 Description-Content-Type: text/markdown
```

