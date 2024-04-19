# Comparing `tmp/ltbfiles-3.2.0rc221.tar.gz` & `tmp/ltbfiles-4.0.0rc257.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltbfiles-3.2.0rc221.tar", last modified: Fri Mar 22 08:09:54 2024, max compression
+gzip compressed data, was "ltbfiles-4.0.0rc257.tar", last modified: Fri Apr 19 13:26:45 2024, max compression
```

## Comparing `ltbfiles-3.2.0rc221.tar` & `ltbfiles-4.0.0rc257.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 08:09:54.152100 ltbfiles-3.2.0rc221/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2024-03-22 08:09:46.000000 ltbfiles-3.2.0rc221/LICENSE_GPL_v3.txt
--rw-r--r--   0 root         (0) root         (0)     3042 2024-03-22 08:09:54.151100 ltbfiles-3.2.0rc221/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2057 2024-03-22 08:09:46.000000 ltbfiles-3.2.0rc221/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1139 2024-03-22 08:09:46.000000 ltbfiles-3.2.0rc221/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 08:09:54.148100 ltbfiles-3.2.0rc221/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 08:09:54.149100 ltbfiles-3.2.0rc221/python/ltbfiles/
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-03-22 08:09:46.000000 ltbfiles-3.2.0rc221/python/ltbfiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2024-03-22 08:09:46.000000 ltbfiles-3.2.0rc221/python/ltbfiles/autoimagelog.py
--rw-rw-rw-   0 root         (0) root         (0)    16973 2024-03-22 08:09:46.000000 ltbfiles-3.2.0rc221/python/ltbfiles/ltbfiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 08:09:54.151100 ltbfiles-3.2.0rc221/python/ltbfiles.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3042 2024-03-22 08:09:54.000000 ltbfiles-3.2.0rc221/python/ltbfiles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      325 2024-03-22 08:09:54.000000 ltbfiles-3.2.0rc221/python/ltbfiles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-22 08:09:54.000000 ltbfiles-3.2.0rc221/python/ltbfiles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-03-22 08:09:54.000000 ltbfiles-3.2.0rc221/python/ltbfiles.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-22 08:09:54.000000 ltbfiles-3.2.0rc221/python/ltbfiles.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-03-22 08:09:54.152100 ltbfiles-3.2.0rc221/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 13:26:45.381840 ltbfiles-4.0.0rc257/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2024-04-19 13:26:37.000000 ltbfiles-4.0.0rc257/LICENSE_GPL_v3.txt
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-04-19 13:26:45.381840 ltbfiles-4.0.0rc257/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2024-04-19 13:26:37.000000 ltbfiles-4.0.0rc257/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-04-19 13:26:37.000000 ltbfiles-4.0.0rc257/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 13:26:45.377840 ltbfiles-4.0.0rc257/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 13:26:45.379840 ltbfiles-4.0.0rc257/python/ltbfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-04-19 13:26:37.000000 ltbfiles-4.0.0rc257/python/ltbfiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-19 13:26:37.000000 ltbfiles-4.0.0rc257/python/ltbfiles/autoimagelog.py
+-rw-rw-rw-   0 root         (0) root         (0)    23709 2024-04-19 13:26:37.000000 ltbfiles-4.0.0rc257/python/ltbfiles/ltbfiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 13:26:45.380840 ltbfiles-4.0.0rc257/python/ltbfiles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-04-19 13:26:45.000000 ltbfiles-4.0.0rc257/python/ltbfiles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      325 2024-04-19 13:26:45.000000 ltbfiles-4.0.0rc257/python/ltbfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 13:26:45.000000 ltbfiles-4.0.0rc257/python/ltbfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-19 13:26:45.000000 ltbfiles-4.0.0rc257/python/ltbfiles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-19 13:26:45.000000 ltbfiles-4.0.0rc257/python/ltbfiles.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-04-19 13:26:45.381840 ltbfiles-4.0.0rc257/setup.cfg
```

### Comparing `ltbfiles-3.2.0rc221/LICENSE_GPL_v3.txt` & `ltbfiles-4.0.0rc257/LICENSE_GPL_v3.txt`

 * *Files identical despite different names*

### Comparing `ltbfiles-3.2.0rc221/PKG-INFO` & `ltbfiles-4.0.0rc257/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 3.2.0rc221
+Version: 4.0.0rc257
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
 Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE_GPL_v3.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

### Comparing `ltbfiles-3.2.0rc221/README.md` & `ltbfiles-4.0.0rc257/README.md`

 * *Files identical despite different names*

### Comparing `ltbfiles-3.2.0rc221/pyproject.toml` & `ltbfiles-4.0.0rc257/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 [project]
 name = "ltbfiles"
 authors = [
     {name="Sven Merk"},
 ]
 description = "Module for loading of files created with spectrometers from LTB"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
```

### Comparing `ltbfiles-3.2.0rc221/python/ltbfiles/autoimagelog.py` & `ltbfiles-4.0.0rc257/python/ltbfiles/autoimagelog.py`

 * *Files identical despite different names*

### Comparing `ltbfiles-3.2.0rc221/python/ltbfiles.egg-info/PKG-INFO` & `ltbfiles-4.0.0rc257/python/ltbfiles.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 3.2.0rc221
+Version: 4.0.0rc257
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
 Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE_GPL_v3.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
```

