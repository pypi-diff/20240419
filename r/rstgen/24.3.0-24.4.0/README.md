# Comparing `tmp/rstgen-24.3.0.tar.gz` & `tmp/rstgen-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstgen-24.3.0.tar", last modified: Tue Mar 19 12:29:03 2024, max compression
+gzip compressed data, was "rstgen-24.4.0.tar", last modified: Fri Apr 19 07:37:59 2024, max compression
```

## Comparing `rstgen-24.3.0.tar` & `rstgen-24.4.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-19 12:29:03.098133 rstgen-24.3.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:52:25.000000 rstgen-24.3.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      121 2022-06-08 22:41:00.000000 rstgen-24.3.0/MANIFEST.in
--rw-r--r--   0 luc       (1000) www-data    (33)     1155 2024-03-19 12:29:03.098133 rstgen-24.3.0/PKG-INFO
--rw-rw-r--   0 luc       (1000) www-data    (33)      512 2023-01-21 16:56:15.000000 rstgen-24.3.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-19 12:29:03.094133 rstgen-24.3.0/rstgen/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8097 2024-03-17 11:52:54.000000 rstgen-24.3.0/rstgen/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10889 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/buildblog.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     7012 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/confparser.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-19 12:29:03.098133 rstgen-24.3.0/rstgen/sphinxconf/
--rw-rw-r--   0 luc       (1000) www-data    (33)     4128 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/sphinxconf/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13604 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/sphinxconf/base.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11176 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/sphinxconf/blog.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4182 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/sphinxconf/complex_tables.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9403 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/sphinxconf/default_conf.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6389 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/sphinxconf/dirtables.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7775 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/sphinxconf/insert_input.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5917 2024-03-15 10:22:50.000000 rstgen-24.3.0/rstgen/sphinxconf/interproject.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-19 12:29:03.098133 rstgen-24.3.0/rstgen/sphinxconf/languages/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      107 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/sphinxconf/languages/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1768 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/sphinxconf/languages/et.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4121 2024-02-14 17:19:37.000000 rstgen-24.3.0/rstgen/sphinxconf/refstothis.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      584 2015-09-19 04:06:47.000000 rstgen-24.3.0/rstgen/sphinxconf/select_lang.html
--rw-rw-r--   0 luc       (1000) www-data    (33)     9516 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/sphinxconf/sigal_image.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-19 12:29:03.098133 rstgen-24.3.0/rstgen/sphinxconf/static/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      151 2021-06-16 03:15:52.000000 rstgen-24.3.0/rstgen/sphinxconf/static/atelier.css
--rw-rw-rw-   0 luc       (1000) www-data    (33)      320 2022-12-03 21:15:05.000000 rstgen-24.3.0/rstgen/sphinxconf/static/insipid-cust.css
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-19 12:29:03.098133 rstgen-24.3.0/rstgen/sphinxconf/templates/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      608 2021-04-12 10:59:41.000000 rstgen-24.3.0/rstgen/sphinxconf/templates/facebook-button.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)       97 2021-04-12 10:16:35.000000 rstgen-24.3.0/rstgen/sphinxconf/templates/home-button.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)       42 2022-04-18 19:33:41.000000 rstgen-24.3.0/rstgen/sphinxconf/templates/languages-button.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)       64 2021-10-22 03:29:01.000000 rstgen-24.3.0/rstgen/sphinxconf/templates/languages.html
--rw-rw-r--   0 luc       (1000) www-data    (33)      535 2023-11-23 18:29:38.000000 rstgen-24.3.0/rstgen/sphinxconf/templates/layout.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)       28 2021-04-12 10:16:35.000000 rstgen-24.3.0/rstgen/sphinxconf/templates/links.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5995 2022-09-28 04:15:08.000000 rstgen-24.3.0/rstgen/sphinxconf/templates/share-buttons.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      554 2024-01-08 04:46:35.000000 rstgen-24.3.0/rstgen/sphinxconf/templates/show-source.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)       64 2021-04-12 10:16:35.000000 rstgen-24.3.0/rstgen/sphinxconf/templates/unused_layout.html
--rw-rw-r--   0 luc       (1000) www-data    (33)    12501 2024-02-14 17:19:38.000000 rstgen-24.3.0/rstgen/utils.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-19 12:29:03.098133 rstgen-24.3.0/rstgen.egg-info/
--rw-r--r--   0 luc       (1000) www-data    (33)     1155 2024-03-19 12:29:03.000000 rstgen-24.3.0/rstgen.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1236 2024-03-19 12:29:03.000000 rstgen-24.3.0/rstgen.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-03-19 12:29:03.000000 rstgen-24.3.0/rstgen.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2022-06-08 22:45:26.000000 rstgen-24.3.0/rstgen.egg-info/not-zip-safe
--rw-rw-r--   0 luc       (1000) www-data    (33)       17 2024-03-19 12:29:03.000000 rstgen-24.3.0/rstgen.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        7 2024-03-19 12:29:03.000000 rstgen-24.3.0/rstgen.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-03-19 12:29:03.098133 rstgen-24.3.0/setup.cfg
--rw-rw-r--   0 luc       (1000) www-data    (33)      991 2024-03-19 12:28:45.000000 rstgen-24.3.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      131 2024-02-14 17:19:37.000000 rstgen-24.3.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-19 12:29:03.098133 rstgen-24.3.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      640 2024-02-14 17:19:37.000000 rstgen-24.3.0/tests/test_everything.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-19 07:37:59.166860 rstgen-24.4.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:52:25.000000 rstgen-24.4.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      121 2022-06-08 22:41:00.000000 rstgen-24.4.0/MANIFEST.in
+-rw-r--r--   0 luc       (1000) www-data    (33)     1155 2024-04-19 07:37:59.166860 rstgen-24.4.0/PKG-INFO
+-rw-rw-r--   0 luc       (1000) www-data    (33)      512 2023-01-21 16:56:15.000000 rstgen-24.4.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-19 07:37:59.166860 rstgen-24.4.0/rstgen/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     8097 2024-03-17 11:52:54.000000 rstgen-24.4.0/rstgen/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10889 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/buildblog.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     7012 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/confparser.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-19 07:37:59.166860 rstgen-24.4.0/rstgen/sphinxconf/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4663 2024-04-19 05:01:55.000000 rstgen-24.4.0/rstgen/sphinxconf/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13604 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/sphinxconf/base.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    11176 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/sphinxconf/blog.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4182 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/sphinxconf/complex_tables.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     9403 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/sphinxconf/default_conf.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6389 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/sphinxconf/dirtables.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     7775 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/sphinxconf/insert_input.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5839 2024-04-18 12:54:53.000000 rstgen-24.4.0/rstgen/sphinxconf/interproject.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-19 07:37:59.166860 rstgen-24.4.0/rstgen/sphinxconf/languages/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      107 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/sphinxconf/languages/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1768 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/sphinxconf/languages/et.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     4121 2024-02-14 17:19:37.000000 rstgen-24.4.0/rstgen/sphinxconf/refstothis.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      584 2015-09-19 04:06:47.000000 rstgen-24.4.0/rstgen/sphinxconf/select_lang.html
+-rw-rw-r--   0 luc       (1000) www-data    (33)     9557 2024-04-11 07:32:12.000000 rstgen-24.4.0/rstgen/sphinxconf/sigal_image.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-19 07:37:59.166860 rstgen-24.4.0/rstgen/sphinxconf/static/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      151 2021-06-16 03:15:52.000000 rstgen-24.4.0/rstgen/sphinxconf/static/atelier.css
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      320 2022-12-03 21:15:05.000000 rstgen-24.4.0/rstgen/sphinxconf/static/insipid-cust.css
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-19 07:37:59.166860 rstgen-24.4.0/rstgen/sphinxconf/templates/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      608 2021-04-12 10:59:41.000000 rstgen-24.4.0/rstgen/sphinxconf/templates/facebook-button.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       97 2021-04-12 10:16:35.000000 rstgen-24.4.0/rstgen/sphinxconf/templates/home-button.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       42 2022-04-18 19:33:41.000000 rstgen-24.4.0/rstgen/sphinxconf/templates/languages-button.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       64 2021-10-22 03:29:01.000000 rstgen-24.4.0/rstgen/sphinxconf/templates/languages.html
+-rw-rw-r--   0 luc       (1000) www-data    (33)      535 2023-11-23 18:29:38.000000 rstgen-24.4.0/rstgen/sphinxconf/templates/layout.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       28 2021-04-12 10:16:35.000000 rstgen-24.4.0/rstgen/sphinxconf/templates/links.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     5995 2022-09-28 04:15:08.000000 rstgen-24.4.0/rstgen/sphinxconf/templates/share-buttons.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      554 2024-01-08 04:46:35.000000 rstgen-24.4.0/rstgen/sphinxconf/templates/show-source.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       64 2021-04-12 10:16:35.000000 rstgen-24.4.0/rstgen/sphinxconf/templates/unused_layout.html
+-rw-rw-r--   0 luc       (1000) www-data    (33)    12501 2024-02-14 17:19:38.000000 rstgen-24.4.0/rstgen/utils.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-19 07:37:59.166860 rstgen-24.4.0/rstgen.egg-info/
+-rw-r--r--   0 luc       (1000) www-data    (33)     1155 2024-04-19 07:37:59.000000 rstgen-24.4.0/rstgen.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1236 2024-04-19 07:37:59.000000 rstgen-24.4.0/rstgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-04-19 07:37:59.000000 rstgen-24.4.0/rstgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2022-06-08 22:45:26.000000 rstgen-24.4.0/rstgen.egg-info/not-zip-safe
+-rw-rw-r--   0 luc       (1000) www-data    (33)       17 2024-04-19 07:37:59.000000 rstgen-24.4.0/rstgen.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        7 2024-04-19 07:37:59.000000 rstgen-24.4.0/rstgen.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-04-19 07:37:59.166860 rstgen-24.4.0/setup.cfg
+-rw-rw-r--   0 luc       (1000) www-data    (33)      991 2024-04-19 07:37:45.000000 rstgen-24.4.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      131 2024-02-14 17:19:37.000000 rstgen-24.4.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-19 07:37:59.166860 rstgen-24.4.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      640 2024-02-14 17:19:37.000000 rstgen-24.4.0/tests/test_everything.py
```

### Comparing `rstgen-24.3.0/COPYING` & `rstgen-24.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/PKG-INFO` & `rstgen-24.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstgen
-Version: 24.3.0
+Version: 24.4.0
 Summary: Pythonic API for generating reStructuredText.
 Home-page: https://gitlab.com/lino-framework/rstgen
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rstgen-24.3.0/README.rst` & `rstgen-24.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/__init__.py` & `rstgen-24.4.0/rstgen/__init__.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/buildblog.py` & `rstgen-24.4.0/rstgen/buildblog.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/confparser.py` & `rstgen-24.4.0/rstgen/confparser.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/__init__.py` & `rstgen-24.4.0/rstgen/sphinxconf/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2011-2022 Rumma & Ko Ltd
+# Copyright 2011-2024 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 """
 Sphinx extensions and a :func:`configure` function used to build
 the documentation trees maintained by us.
 
 .. autosummary::
    :toctree:
@@ -15,24 +15,22 @@
    sigal_image
    complex_tables
    blog
    interproject
 """
 
 import logging
-
-logger = logging.getLogger(__name__)
-
 import sys
 import os
-
 from pathlib import Path
 # from pkg_resources import parse_version
 import sphinx
+import synodal
 
+# logger = logging.getLogger(__name__)
 
 def configure(globals_dict, project=None, conffiles=["default_conf.py"]):
     """
     Adds to your `conf.py` an arbitrary series of things that all our
     Sphinx docs configuration files have in common.
 
     Usage: add the following two lines at the beginning of your
@@ -40,34 +38,43 @@
 
       from rstgen.sphinxconf import configure
       configure(globals())
 
     Incomplete list of settings that will be set:
 
     - `templates_path`
-    - `extensions`, `extlinks` and `intersphinx_mapping` are initialized but empty
+    - `extensions` and `extlinks` are initialized but empty
     - `master_doc` = 'index'
     - `source_suffix` = '.rst'
     - `primary_domain` = 'py'
     - `pygments_style` = 'sphinx'
     - `version` and `release` from SETUP_INFO
     - `exclude_trees` = ['old', 'include', '.build']
+    - Fill the Synodalsoft doctrees into :envvar:`intersphinx_mapping`
 
     """
+    globals_dict.setdefault('__file__', __file__)
+    # __file__ might not exist when called from test case
+    # pth = globals_dict.get('__file__', None)
     docs_root = Path(globals_dict['__file__']).parent.absolute()
     sys.path.append(docs_root)
 
     # https://insipid-sphinx-theme.readthedocs.io/en/0.2.0/configuration.html
     globals_dict.setdefault('html_theme', "insipid")
     # globals_dict.setdefault('html_theme', "pydata_sphinx_theme")
     # globals_dict.update(html_theme="bizstyle")
 
     globals_dict.setdefault('html_context', dict())
     globals_dict.setdefault('extlinks', dict())
-    globals_dict.setdefault('intersphinx_mapping', dict())
+    intersphinx_mapping = globals_dict.setdefault('intersphinx_mapping', dict())
+    for r in synodal.REPOS_LIST:
+        if r.public_url and r.nickname and r.git_repo:
+            if not r.nickname in intersphinx_mapping:
+                intersphinx_mapping[r.nickname] = (r.public_url, None)
+
     globals_dict.update(
         exclude_patterns=['old', 'include', 'shared', '.build'])
     extensions = []
     globals_dict.update(extensions=extensions)
 
     extensions += [
         'sphinx.ext.inheritance_diagram',
@@ -107,14 +114,15 @@
 
     globals_dict.update(master_doc='index')
     globals_dict.update(source_suffix='.rst')
     globals_dict.update(primary_domain='py')
     globals_dict.update(pygments_style='sphinx')
     globals_dict.update(autodoc_member_order='bysource')
     globals_dict.update(autodoc_inherit_docstrings=False)
+    globals_dict.update(suppress_warnings=['config.cache', 'image.nonlocal_uri'])
 
     for fn in conffiles:
         if not os.path.sep in fn:
             fn = mydir / fn
         with open(fn, "rb") as fd:
             exec(compile(fd.read(), fn, 'exec'), globals_dict)
```

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/base.py` & `rstgen-24.4.0/rstgen/sphinxconf/base.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/blog.py` & `rstgen-24.4.0/rstgen/sphinxconf/blog.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/complex_tables.py` & `rstgen-24.4.0/rstgen/sphinxconf/complex_tables.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/default_conf.py` & `rstgen-24.4.0/rstgen/sphinxconf/default_conf.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/dirtables.py` & `rstgen-24.4.0/rstgen/sphinxconf/dirtables.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/insert_input.py` & `rstgen-24.4.0/rstgen/sphinxconf/insert_input.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/interproject.py` & `rstgen-24.4.0/rstgen/sphinxconf/interproject.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2011-2020 Rumma & Ko Ltd
+# Copyright 2011-2024 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 """
 Defines the :func:`rstgen.sphinxconf.interproject.configure` function.
 
 """
 import os
 
@@ -23,17 +23,21 @@
 # E.g. on Travis no other projects are installed from source, so there we
 # cannot use it.
 
 
 def configure(globals_dict, prjspec=None, **nicknames):
     """
 
-    Install doctrees of all (or some) atelier projects into the
+    Install the specified atelier projects into the
     :envvar:`intersphinx_mapping` of your :xfile:`conf.py`.
 
+    The explicitly specified atelier projects are loaded from your local copies
+    of the repositories unless :envvar:`ATELIER_IGNORE_LOCAL_BUILDS` is set to
+    ``yes``.
+
     See :doc:`/sphinxext/interproject`.
 
     """
 
     intersphinx_mapping = globals_dict.setdefault('intersphinx_mapping',
                                                   dict())
     # extlinks = dict()
@@ -137,21 +141,15 @@
 
         if count == 0 and prjspec:
             logger.warning("No doctree for {}".format(prj))
         # if prj.srcref_url:
         #     k = '%s_srcref' % prj.nickname
         #     extlinks[str(k)] = (prj.srcref_url, '')
 
-    from synodal import REPOS_LIST
-    for r in REPOS_LIST:
-        if r.public_url and r.nickname and r.git_repo:
-            if not r.nickname in intersphinx_mapping:
-                intersphinx_mapping[r.nickname] = (r.public_url, None)
-
     # atelier.current_project = this
-    globals_dict.update(intersphinx_mapping=intersphinx_mapping)
+    # globals_dict.update(intersphinx_mapping=intersphinx_mapping)
 
     # logger.info("20190306 prjlist is {}, intersphinx_mapping is {}".format(
     #     prjlist, intersphinx_mapping))
 
     # if False:  # no longer used
     #     globals_dict.update(extlinks=extlinks)
```

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/languages/et.py` & `rstgen-24.4.0/rstgen/sphinxconf/languages/et.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/refstothis.py` & `rstgen-24.4.0/rstgen/sphinxconf/refstothis.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/select_lang.html` & `rstgen-24.4.0/rstgen/sphinxconf/select_lang.html`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/sigal_image.py` & `rstgen-24.4.0/rstgen/sphinxconf/sigal_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,30 +47,30 @@
 The file name can contain **formatting instructions** inspired by
 `Wikipedia pictures
 <https://en.wikipedia.org/wiki/Wikipedia:Picture_tutorial>`_ which
 uses a variable number of pipe characters. For example:
 
 
 >>> print(line2html("foo.jpg"))
-<a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="foo.jpg"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; height:10em" title="foo.jpg"/></a>
+<a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="foo.jpg"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; height:30ex" title="foo.jpg"/></a>
 
 >>> print(line2html("foo.jpg|This is a nice picture"))
-<a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="This is a nice picture"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; height:10em" title="This is a nice picture"/></a>
+<a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="This is a nice picture"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; height:30ex" title="This is a nice picture"/></a>
 
 >>> print(line2html("foo.jpg|thumb|This is a nice picture"))
-<a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="This is a nice picture"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; float:right; height:10em" title="This is a nice picture"/></a>
+<a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="This is a nice picture"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; float:right; height:30ex" title="This is a nice picture"/></a>
 
 >>> print(line2html("foo.jpg|thumb|left|This is a nice picture"))
-<a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="This is a nice picture"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; float:left; height:10em" title="This is a nice picture"/></a>
+<a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="This is a nice picture"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; float:left; height:30ex" title="This is a nice picture"/></a>
 
 >>> print(line2html("foo.jpg|wide|This is a wide picture"))
 <a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="This is a wide picture"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; width:100%" title="This is a wide picture"/></a>
 
 >>> print(line2html("foo.jpg | thumb | left | This is a nice picture"))
-<a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="This is a nice picture"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; float:left; height:10em" title="This is a nice picture"/></a>
+<a href="http://example.com/foo.jpg"  data-lightbox="image-1" data-title="This is a nice picture"/><img src="http://example.com/thumbnails/foo.jpg" style="padding:4px; float:left; height:30ex" title="This is a nice picture"/></a>
 
 
 The generated HTML also includes attributes for `lightbox
 <http://lokeshdhakar.com/projects/lightbox2/>`_.  In order to activate
 this feature you must add the content of the lighbox :file:`dist`
 directory somewhere to your web server and then change your
 `layout.html` template to something like this::
@@ -113,15 +113,16 @@
                 if v:
                     styles.append("{}:{}".format(k, v))
             context.update(style="; ".join(styles))
         self.context = context
 
 
 class Standard(Format):
-    height = "10em"
+    height = "30ex"
+    # width = "33%"
 
 
 class Thumb(Standard):
 
     float = "right"
 
     def __init__(self, caption, **context):
@@ -137,15 +138,16 @@
             # tplkw['style'] = "padding:4px; float:{0}; height:{1};".format(align, self.height)
         super().__init__(caption, **context)
 
         # tplkw.update(caption=caption)
 
 
 class Tiny(Thumb):
-    height = "5em"
+    height = "15ex"
+    # width = "25%"
 
 
 class Solo(Format):
     width = "90%"
 
 
 class Duo(Format):
```

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/templates/facebook-button.html` & `rstgen-24.4.0/rstgen/sphinxconf/templates/facebook-button.html`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/templates/layout.html` & `rstgen-24.4.0/rstgen/sphinxconf/templates/layout.html`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/templates/share-buttons.html` & `rstgen-24.4.0/rstgen/sphinxconf/templates/share-buttons.html`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/sphinxconf/templates/show-source.html` & `rstgen-24.4.0/rstgen/sphinxconf/templates/show-source.html`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen/utils.py` & `rstgen-24.4.0/rstgen/utils.py`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/rstgen.egg-info/PKG-INFO` & `rstgen-24.4.0/rstgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstgen
-Version: 24.3.0
+Version: 24.4.0
 Summary: Pythonic API for generating reStructuredText.
 Home-page: https://gitlab.com/lino-framework/rstgen
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rstgen-24.3.0/rstgen.egg-info/SOURCES.txt` & `rstgen-24.4.0/rstgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rstgen-24.3.0/setup.py` & `rstgen-24.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 SETUP_INFO = dict(
     name='rstgen',
-    version='24.3.0',
+    version='24.4.0',
     packages=['rstgen', 'rstgen.sphinxconf', 'rstgen.sphinxconf.languages'],
     install_requires=['synodal', 'docutils'],
     # tests_require=['atelier'],
     test_suite='tests',
     description="Pythonic API for generating reStructuredText.",
     license_files=['COPYING'],
     url='https://gitlab.com/lino-framework/rstgen',
```

### Comparing `rstgen-24.3.0/tests/test_everything.py` & `rstgen-24.4.0/tests/test_everything.py`

 * *Files identical despite different names*

