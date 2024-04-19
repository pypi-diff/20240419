# Comparing `tmp/gmaps_avoid_swiss-0.1.1.tar.gz` & `tmp/gmaps_avoid_swiss-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmaps_avoid_swiss-0.1.1.tar", last modified: Fri Apr 19 19:31:35 2024, max compression
+gzip compressed data, was "gmaps_avoid_swiss-0.1.2.tar", last modified: Fri Apr 19 19:43:41 2024, max compression
```

## Comparing `gmaps_avoid_swiss-0.1.1.tar` & `gmaps_avoid_swiss-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:31:35.743666 gmaps_avoid_swiss-0.1.1/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      162 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/AUTHORS.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     3851 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/CONTRIBUTING.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       89 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/HISTORY.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1072 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/LICENSE
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      262 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/MANIFEST.in
--rw-r--r--   0 gregor    (1000) gregor    (1000)     1886 2024-04-19 19:31:35.743666 gmaps_avoid_swiss-0.1.1/PKG-INFO
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      937 2024-04-19 18:35:36.000000 gmaps_avoid_swiss-0.1.1/README.rst
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:31:35.743666 gmaps_avoid_swiss-0.1.1/docs/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      618 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/docs/Makefile
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:31:35.739666 gmaps_avoid_swiss-0.1.1/docs/_build/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:31:35.739666 gmaps_avoid_swiss-0.1.1/docs/_build/html/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:31:35.743666 gmaps_avoid_swiss-0.1.1/docs/_build/html/_static/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      286 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/docs/authors.rst
--rwxrwxr-x   0 gregor    (1000) gregor    (1000)     4943 2024-04-19 14:38:21.000000 gmaps_avoid_swiss-0.1.1/docs/conf.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       33 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/docs/contributing.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      559 2024-04-19 14:44:07.000000 gmaps_avoid_swiss-0.1.1/docs/gmaps_avoid_swiss.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/docs/history.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      321 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/docs/index.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1211 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/docs/installation.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      815 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/docs/make.bat
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       88 2024-04-19 14:44:07.000000 gmaps_avoid_swiss-0.1.1/docs/modules.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       27 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/docs/readme.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       96 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/docs/usage.rst
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1309 2024-04-19 19:31:09.000000 gmaps_avoid_swiss-0.1.1/pyproject.toml
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-04-19 19:31:35.743666 gmaps_avoid_swiss-0.1.1/setup.cfg
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      879 2024-04-19 19:30:22.000000 gmaps_avoid_swiss-0.1.1/setup.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:31:35.739666 gmaps_avoid_swiss-0.1.1/src/
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:31:35.743666 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      148 2024-04-19 19:31:09.000000 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss/__init__.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      949 2024-04-19 19:15:01.000000 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss/cli.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1825 2024-04-19 18:33:24.000000 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss/gmaps_avoid_swiss.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     2292 2024-04-19 18:32:52.000000 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss/waypoints.py
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:31:35.743666 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss.egg-info/
--rw-r--r--   0 gregor    (1000) gregor    (1000)     1886 2024-04-19 19:31:35.000000 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss.egg-info/PKG-INFO
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      864 2024-04-19 19:31:35.000000 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss.egg-info/SOURCES.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-04-19 19:31:35.000000 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss.egg-info/dependency_links.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       39 2024-04-19 19:31:35.000000 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss.egg-info/requires.txt
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       18 2024-04-19 19:31:35.000000 gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss.egg-info/top_level.txt
-drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:31:35.743666 gmaps_avoid_swiss-0.1.1/tests/
--rw-rw-r--   0 gregor    (1000) gregor    (1000)       47 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.1/tests/__init__.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      757 2024-04-19 19:11:03.000000 gmaps_avoid_swiss-0.1.1/tests/test_cli.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)      941 2024-04-19 18:43:41.000000 gmaps_avoid_swiss-0.1.1/tests/test_gmaps_avoid_swiss.py
--rw-rw-r--   0 gregor    (1000) gregor    (1000)     1206 2024-04-19 18:46:00.000000 gmaps_avoid_swiss-0.1.1/tests/test_waypoints.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:43:41.484332 gmaps_avoid_swiss-0.1.2/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      162 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/AUTHORS.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     3851 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/CONTRIBUTING.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       89 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/HISTORY.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1072 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/LICENSE
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      262 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/MANIFEST.in
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     1941 2024-04-19 19:43:41.484332 gmaps_avoid_swiss-0.1.2/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      937 2024-04-19 18:35:36.000000 gmaps_avoid_swiss-0.1.2/README.rst
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:43:41.480332 gmaps_avoid_swiss-0.1.2/docs/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      618 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/docs/Makefile
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:43:41.480332 gmaps_avoid_swiss-0.1.2/docs/_build/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:43:41.480332 gmaps_avoid_swiss-0.1.2/docs/_build/html/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:43:41.480332 gmaps_avoid_swiss-0.1.2/docs/_build/html/_static/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      286 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.2/docs/_build/html/_static/file.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.2/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       90 2024-04-19 14:44:04.000000 gmaps_avoid_swiss-0.1.2/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/docs/authors.rst
+-rwxrwxr-x   0 gregor    (1000) gregor    (1000)     4943 2024-04-19 14:38:21.000000 gmaps_avoid_swiss-0.1.2/docs/conf.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       33 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/docs/contributing.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      559 2024-04-19 14:44:07.000000 gmaps_avoid_swiss-0.1.2/docs/gmaps_avoid_swiss.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       28 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/docs/history.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      321 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/docs/index.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1211 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/docs/installation.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      815 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/docs/make.bat
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       88 2024-04-19 14:44:07.000000 gmaps_avoid_swiss-0.1.2/docs/modules.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       27 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/docs/readme.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       96 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/docs/usage.rst
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1344 2024-04-19 19:43:15.000000 gmaps_avoid_swiss-0.1.2/pyproject.toml
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       38 2024-04-19 19:43:41.484332 gmaps_avoid_swiss-0.1.2/setup.cfg
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      996 2024-04-19 19:43:11.000000 gmaps_avoid_swiss-0.1.2/setup.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:43:41.480332 gmaps_avoid_swiss-0.1.2/src/
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:43:41.484332 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      148 2024-04-19 19:43:25.000000 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      949 2024-04-19 19:15:01.000000 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss/cli.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1825 2024-04-19 18:33:24.000000 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss/gmaps_avoid_swiss.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     2292 2024-04-19 18:32:52.000000 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss/waypoints.py
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:43:41.484332 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss.egg-info/
+-rw-r--r--   0 gregor    (1000) gregor    (1000)     1941 2024-04-19 19:43:41.000000 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss.egg-info/PKG-INFO
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      864 2024-04-19 19:43:41.000000 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)        1 2024-04-19 19:43:41.000000 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       64 2024-04-19 19:43:41.000000 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss.egg-info/requires.txt
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       18 2024-04-19 19:43:41.000000 gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss.egg-info/top_level.txt
+drwxrwxr-x   0 gregor    (1000) gregor    (1000)        0 2024-04-19 19:43:41.484332 gmaps_avoid_swiss-0.1.2/tests/
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)       47 2024-04-19 13:34:36.000000 gmaps_avoid_swiss-0.1.2/tests/__init__.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      757 2024-04-19 19:11:03.000000 gmaps_avoid_swiss-0.1.2/tests/test_cli.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)      941 2024-04-19 18:43:41.000000 gmaps_avoid_swiss-0.1.2/tests/test_gmaps_avoid_swiss.py
+-rw-rw-r--   0 gregor    (1000) gregor    (1000)     1206 2024-04-19 18:46:00.000000 gmaps_avoid_swiss-0.1.2/tests/test_waypoints.py
```

### Comparing `gmaps_avoid_swiss-0.1.1/CONTRIBUTING.rst` & `gmaps_avoid_swiss-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/LICENSE` & `gmaps_avoid_swiss-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/PKG-INFO` & `gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
-Name: gmaps_avoid_swiss
-Version: 0.1.1
+Name: gmaps-avoid-swiss
+Version: 0.1.2
 Summary: A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland.
 Home-page: https://github.com/xbencat/gmaps_avoid_swiss
 Author: Gregor Bencat
 Author-email: Gregor Bencat <bencat.gregor@gmail.com>
 Maintainer-email: Gregor Bencat <bencat.gregor@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/xbencat/gmaps_avoid_swiss/issues
 Project-URL: changelog, https://github.com/xbencat/gmaps_avoid_swiss/blob/master/changelog.md
 Project-URL: homepage, https://github.com/xbencat/gmaps_avoid_swiss
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: google-maps-routing
 Requires-Dist: typer
+Requires-Dist: rich
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 
 ========================
```

### Comparing `gmaps_avoid_swiss-0.1.1/README.rst` & `gmaps_avoid_swiss-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/docs/Makefile` & `gmaps_avoid_swiss-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/docs/conf.py` & `gmaps_avoid_swiss-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/docs/gmaps_avoid_swiss.rst` & `gmaps_avoid_swiss-0.1.2/docs/gmaps_avoid_swiss.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/docs/installation.rst` & `gmaps_avoid_swiss-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/docs/make.bat` & `gmaps_avoid_swiss-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/pyproject.toml` & `gmaps_avoid_swiss-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gmaps_avoid_swiss"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland."
 readme = "README.rst"
 authors = [
   {name = "Gregor Bencat", email = "bencat.gregor@gmail.com"}
 ]
 maintainers = [
   {name = "Gregor Bencat", email = "bencat.gregor@gmail.com"}
 ]
 classifiers = [
 
 ]
 license = {text = "MIT license"}
 dependencies = [
-  "typer"
+  "google-maps-routing",
+  "typer",
+  "rich"
 ]
 
 [project.optional-dependencies]
 dev = [
     "coverage",  # testing
     "mypy",  # linting
     "pytest",  # testing
```

### Comparing `gmaps_avoid_swiss-0.1.1/setup.py` & `gmaps_avoid_swiss-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gmaps_avoid_swiss',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/xbencat/gmaps_avoid_swiss',
     license='MIT',
     author='Gregor Bencat',
     author_email='bencat.gregor@gmail.com',
     description='A Python package that customizes Google Maps routing to avoid Swiss routes.',
+    install_requires=[
+        'typer~=0.12.3',
+        'rich~=13.7.1',
+        'google-maps-routing~=0.6.8',
+    ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
```

### Comparing `gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss/cli.py` & `gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss/cli.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss/gmaps_avoid_swiss.py` & `gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss/gmaps_avoid_swiss.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss/waypoints.py` & `gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss/waypoints.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss.egg-info/PKG-INFO` & `gmaps_avoid_swiss-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
-Name: gmaps-avoid-swiss
-Version: 0.1.1
+Name: gmaps_avoid_swiss
+Version: 0.1.2
 Summary: A Python package that customizes Google Maps routing to avoid Swiss routes unless the origin, destination, or waypoints include locations within Switzerland.
 Home-page: https://github.com/xbencat/gmaps_avoid_swiss
 Author: Gregor Bencat
 Author-email: Gregor Bencat <bencat.gregor@gmail.com>
 Maintainer-email: Gregor Bencat <bencat.gregor@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/xbencat/gmaps_avoid_swiss/issues
 Project-URL: changelog, https://github.com/xbencat/gmaps_avoid_swiss/blob/master/changelog.md
 Project-URL: homepage, https://github.com/xbencat/gmaps_avoid_swiss
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: google-maps-routing
 Requires-Dist: typer
+Requires-Dist: rich
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 
 ========================
```

### Comparing `gmaps_avoid_swiss-0.1.1/src/gmaps_avoid_swiss.egg-info/SOURCES.txt` & `gmaps_avoid_swiss-0.1.2/src/gmaps_avoid_swiss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/tests/test_cli.py` & `gmaps_avoid_swiss-0.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/tests/test_gmaps_avoid_swiss.py` & `gmaps_avoid_swiss-0.1.2/tests/test_gmaps_avoid_swiss.py`

 * *Files identical despite different names*

### Comparing `gmaps_avoid_swiss-0.1.1/tests/test_waypoints.py` & `gmaps_avoid_swiss-0.1.2/tests/test_waypoints.py`

 * *Files identical despite different names*

