# Comparing `tmp/solvent_guide-0.4.5.tar.gz` & `tmp/solvent_guide-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\pczjh2\OneDrive - The University of Nottingham\PycharmProjects\solvent_guide\dist\.tmp-dlkpk0_w\solvent_guide-0.4.5.ta", last modified: Fri Apr 19 15:27:03 2024, max compression
+gzip compressed data, was "C:\Users\pczjh2\OneDrive - The University of Nottingham\PycharmProjects\solvent_guide\dist\.tmp-5x0xtfnr\solvent_guide-0.4.6.ta", last modified: Fri Apr 19 15:34:31 2024, max compression
```

## Comparing `solvent_guide-0.4.5.tar` & `solvent_guide-0.4.6.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.186120 solvent_guide-0.4.5/
--rw-rw-rw-   0        0        0    35163 2023-10-03 13:29:19.000000 solvent_guide-0.4.5/LICENSE
--rw-rw-rw-   0        0        0     9489 2024-04-19 15:27:03.185119 solvent_guide-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     8826 2024-04-19 09:51:44.000000 solvent_guide-0.4.5/README.md
--rw-rw-rw-   0        0        0      765 2024-04-19 14:15:01.000000 solvent_guide-0.4.5/pyproject.toml
--rw-rw-rw-   0        0        0      325 2024-04-19 15:27:03.190240 solvent_guide-0.4.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.031785 solvent_guide-0.4.5/src/
--rw-rw-rw-   0        0        0        0 2023-09-27 14:03:04.000000 solvent_guide-0.4.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.060813 solvent_guide-0.4.5/src/solvent_guide/
--rw-rw-rw-   0        0        0        0 2023-09-29 09:09:48.000000 solvent_guide-0.4.5/src/solvent_guide/__init__.py
--rw-rw-rw-   0        0        0     6594 2024-02-08 16:49:30.000000 solvent_guide-0.4.5/src/solvent_guide/add_solvent.py
--rw-rw-rw-   0        0        0     1116 2023-10-05 13:54:32.000000 solvent_guide-0.4.5/src/solvent_guide/remove_solvent.py
--rw-rw-rw-   0        0        0      544 2023-10-05 12:16:25.000000 solvent_guide-0.4.5/src/solvent_guide/reset_solvents.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.090209 solvent_guide-0.4.5/src/solvent_guide/sources/
--rw-rw-rw-   0        0        0      407 2023-10-03 15:45:26.000000 solvent_guide-0.4.5/src/solvent_guide/sources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.093123 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/
--rw-rw-rw-   0        0        0        0 2023-09-07 12:55:19.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.127122 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/
--rw-rw-rw-   0        0        0   501509 2023-09-06 14:40:31.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv
--rw-rw-rw-   0        0        0      112 2023-09-06 14:40:31.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/__init__.py
--rw-rw-rw-   0        0        0      231 2024-02-08 14:16:33.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/default_colours.txt
--rw-rw-rw-   0        0        0     4079 2024-02-08 14:32:56.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/routes.py
--rw-rw-rw-   0        0        0      232 2024-04-19 10:28:55.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/user_colours.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.008787 solvent_guide-0.4.5/src/solvent_guide/sources/static/
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.136177 solvent_guide-0.4.5/src/solvent_guide/sources/static/css/
--rw-rw-rw-   0        0        0      141 2023-10-06 08:46:41.000000 solvent_guide-0.4.5/src/solvent_guide/sources/static/css/hazard_colours.css
--rw-rw-rw-   0        0        0     1904 2023-09-27 09:44:06.000000 solvent_guide-0.4.5/src/solvent_guide/sources/static/css/pagestyle.css
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.144120 solvent_guide-0.4.5/src/solvent_guide/sources/static/js/
--rw-rw-rw-   0        0        0     2060 2024-04-19 12:09:25.000000 solvent_guide-0.4.5/src/solvent_guide/sources/static/js/custom_colours.js
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.177119 solvent_guide-0.4.5/src/solvent_guide/sources/templates/
--rw-rw-rw-   0        0        0    12967 2024-02-08 14:29:28.000000 solvent_guide-0.4.5/src/solvent_guide/sources/templates/accessibility.html
--rw-rw-rw-   0        0        0     2274 2024-04-19 12:53:45.000000 solvent_guide-0.4.5/src/solvent_guide/sources/templates/base.html
--rw-rw-rw-   0        0        0    17178 2024-04-19 13:59:02.000000 solvent_guide-0.4.5/src/solvent_guide/sources/templates/solvent_guide.html
--rw-rw-rw-   0        0        0     6067 2023-09-06 14:40:32.000000 solvent_guide-0.4.5/src/solvent_guide/sources/templates/solvent_guide_help.html
--rw-rw-rw-   0        0        0      519 2024-04-19 09:23:32.000000 solvent_guide-0.4.5/src/solvent_guide/webapp.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.182121 solvent_guide-0.4.5/src/solvent_guide.egg-info/
--rw-rw-rw-   0        0        0     9489 2024-04-19 15:27:02.000000 solvent_guide-0.4.5/src/solvent_guide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1179 2024-04-19 15:27:02.000000 solvent_guide-0.4.5/src/solvent_guide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 15:27:02.000000 solvent_guide-0.4.5/src/solvent_guide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-19 15:27:02.000000 solvent_guide-0.4.5/src/solvent_guide.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.489588 solvent_guide-0.4.6/
+-rw-rw-rw-   0        0        0    35163 2023-10-03 13:29:19.000000 solvent_guide-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0     9489 2024-04-19 15:34:31.488585 solvent_guide-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8826 2024-04-19 09:51:44.000000 solvent_guide-0.4.6/README.md
+-rw-rw-rw-   0        0        0      765 2024-04-19 15:34:16.000000 solvent_guide-0.4.6/pyproject.toml
+-rw-rw-rw-   0        0        0      325 2024-04-19 15:34:31.493607 solvent_guide-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0       37 2024-04-19 15:34:16.000000 solvent_guide-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.385788 solvent_guide-0.4.6/src/
+-rw-rw-rw-   0        0        0        0 2023-09-27 14:03:04.000000 solvent_guide-0.4.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.403018 solvent_guide-0.4.6/src/solvent_guide/
+-rw-rw-rw-   0        0        0        0 2023-09-29 09:09:48.000000 solvent_guide-0.4.6/src/solvent_guide/__init__.py
+-rw-rw-rw-   0        0        0     6594 2024-02-08 16:49:30.000000 solvent_guide-0.4.6/src/solvent_guide/add_solvent.py
+-rw-rw-rw-   0        0        0     1116 2023-10-05 13:54:32.000000 solvent_guide-0.4.6/src/solvent_guide/remove_solvent.py
+-rw-rw-rw-   0        0        0      544 2023-10-05 12:16:25.000000 solvent_guide-0.4.6/src/solvent_guide/reset_solvents.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.429985 solvent_guide-0.4.6/src/solvent_guide/sources/
+-rw-rw-rw-   0        0        0      407 2023-10-03 15:45:26.000000 solvent_guide-0.4.6/src/solvent_guide/sources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.432986 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/
+-rw-rw-rw-   0        0        0        0 2023-09-07 12:55:19.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.451629 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/
+-rw-rw-rw-   0        0        0   501509 2023-09-06 14:40:31.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv
+-rw-rw-rw-   0        0        0      112 2023-09-06 14:40:31.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/__init__.py
+-rw-rw-rw-   0        0        0      231 2024-02-08 14:16:33.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/default_colours.txt
+-rw-rw-rw-   0        0        0     4079 2024-02-08 14:32:56.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/routes.py
+-rw-rw-rw-   0        0        0      232 2024-04-19 10:28:55.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/user_colours.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.365788 solvent_guide-0.4.6/src/solvent_guide/sources/static/
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.460582 solvent_guide-0.4.6/src/solvent_guide/sources/static/css/
+-rw-rw-rw-   0        0        0      141 2023-10-06 08:46:41.000000 solvent_guide-0.4.6/src/solvent_guide/sources/static/css/hazard_colours.css
+-rw-rw-rw-   0        0        0     1904 2023-09-27 09:44:06.000000 solvent_guide-0.4.6/src/solvent_guide/sources/static/css/pagestyle.css
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.463585 solvent_guide-0.4.6/src/solvent_guide/sources/static/js/
+-rw-rw-rw-   0        0        0     2060 2024-04-19 12:09:25.000000 solvent_guide-0.4.6/src/solvent_guide/sources/static/js/custom_colours.js
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.480583 solvent_guide-0.4.6/src/solvent_guide/sources/templates/
+-rw-rw-rw-   0        0        0    12967 2024-02-08 14:29:28.000000 solvent_guide-0.4.6/src/solvent_guide/sources/templates/accessibility.html
+-rw-rw-rw-   0        0        0     2274 2024-04-19 12:53:45.000000 solvent_guide-0.4.6/src/solvent_guide/sources/templates/base.html
+-rw-rw-rw-   0        0        0    17178 2024-04-19 13:59:02.000000 solvent_guide-0.4.6/src/solvent_guide/sources/templates/solvent_guide.html
+-rw-rw-rw-   0        0        0     6067 2023-09-06 14:40:32.000000 solvent_guide-0.4.6/src/solvent_guide/sources/templates/solvent_guide_help.html
+-rw-rw-rw-   0        0        0      520 2024-04-19 15:31:48.000000 solvent_guide-0.4.6/src/solvent_guide/webapp.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.485586 solvent_guide-0.4.6/src/solvent_guide.egg-info/
+-rw-rw-rw-   0        0        0     9489 2024-04-19 15:34:31.000000 solvent_guide-0.4.6/src/solvent_guide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1188 2024-04-19 15:34:31.000000 solvent_guide-0.4.6/src/solvent_guide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 15:34:31.000000 solvent_guide-0.4.6/src/solvent_guide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-19 15:34:31.000000 solvent_guide-0.4.6/src/solvent_guide.egg-info/top_level.txt
```

### Comparing `solvent_guide-0.4.5/LICENSE` & `solvent_guide-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/PKG-INFO` & `solvent_guide-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvent_guide
-Version: 0.4.5
+Version: 0.4.6
 Summary: Standalone version of the solvent guide as shown in the AI4Green ELN
 Author-email: Joe Heeley <joe.heeley@nottingham.ac.uk>, Samuel Boobier <samuel.boobier@googlemail.com>
 Project-URL: Homepage, https://github.com/JoeHeeley2/solvent_flashcards
 Project-URL: Bug Tracker, https://github.com/JoeHeeley2/solvent_flashcards/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `solvent_guide-0.4.5/README.md` & `solvent_guide-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/pyproject.toml` & `solvent_guide-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "solvent_guide"
-version = "0.4.5"
+version = "0.4.6"
 authors = [
   {name="Joe Heeley", email="joe.heeley@nottingham.ac.uk"},
     { name="Samuel Boobier", email="samuel.boobier@googlemail.com" }
 ]
 description = "Standalone version of the solvent guide as shown in the AI4Green ELN"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `solvent_guide-0.4.5/src/solvent_guide/add_solvent.py` & `solvent_guide-0.4.6/src/solvent_guide/add_solvent.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/remove_solvent.py` & `solvent_guide-0.4.6/src/solvent_guide/remove_solvent.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/reset_solvents.py` & `solvent_guide-0.4.6/src/solvent_guide/reset_solvents.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv` & `solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/routes.py` & `solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/routes.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/sources/static/css/pagestyle.css` & `solvent_guide-0.4.6/src/solvent_guide/sources/static/css/pagestyle.css`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/sources/static/js/custom_colours.js` & `solvent_guide-0.4.6/src/solvent_guide/sources/static/js/custom_colours.js`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/sources/templates/accessibility.html` & `solvent_guide-0.4.6/src/solvent_guide/sources/templates/accessibility.html`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/sources/templates/base.html` & `solvent_guide-0.4.6/src/solvent_guide/sources/templates/base.html`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/sources/templates/solvent_guide.html` & `solvent_guide-0.4.6/src/solvent_guide/sources/templates/solvent_guide.html`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/sources/templates/solvent_guide_help.html` & `solvent_guide-0.4.6/src/solvent_guide/sources/templates/solvent_guide_help.html`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.5/src/solvent_guide/webapp.py` & `solvent_guide-0.4.6/src/solvent_guide/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # !/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from sources import create_app
+from .sources import create_app
 from threading import Timer
 import webbrowser
 import os
 
 app = create_app()
 
 port = os.getenv("FLASK_RUN_PORT")
```

### Comparing `solvent_guide-0.4.5/src/solvent_guide.egg-info/PKG-INFO` & `solvent_guide-0.4.6/src/solvent_guide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvent_guide
-Version: 0.4.5
+Version: 0.4.6
 Summary: Standalone version of the solvent guide as shown in the AI4Green ELN
 Author-email: Joe Heeley <joe.heeley@nottingham.ac.uk>, Samuel Boobier <samuel.boobier@googlemail.com>
 Project-URL: Homepage, https://github.com/JoeHeeley2/solvent_flashcards
 Project-URL: Bug Tracker, https://github.com/JoeHeeley2/solvent_flashcards/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `solvent_guide-0.4.5/src/solvent_guide.egg-info/SOURCES.txt` & `solvent_guide-0.4.6/src/solvent_guide.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
+setup.py
 src/__init__.py
 src/solvent_guide/__init__.py
 src/solvent_guide/add_solvent.py
 src/solvent_guide/remove_solvent.py
 src/solvent_guide/reset_solvents.py
 src/solvent_guide/webapp.py
 src/solvent_guide.egg-info/PKG-INFO
```

