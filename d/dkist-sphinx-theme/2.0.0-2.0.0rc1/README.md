# Comparing `tmp/dkist_sphinx_theme-2.0.0.tar.gz` & `tmp/dkist-sphinx-theme-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_sphinx_theme-2.0.0.tar", last modified: Fri Apr 19 15:52:41 2024, max compression
+gzip compressed data, was "dkist-sphinx-theme-2.0.0rc1.tar", last modified: Thu Apr 11 09:52:23 2024, max compression
```

## Comparing `dkist_sphinx_theme-2.0.0.tar` & `dkist-sphinx-theme-2.0.0rc1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.239758 dkist_sphinx_theme-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)    19617 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-19 15:52:41.239758 dkist_sphinx_theme-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      987 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-19 15:52:41.243758 dkist_sphinx_theme-2.0.0/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.235758 dkist_sphinx_theme-2.0.0/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.235758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/
--rw-rw-rw-   0 root         (0) root         (0)     3884 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.235758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/autoapi_templates/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.239758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/autoapi_templates/python/
--rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/autoapi_templates/python/module.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.239758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/conf/
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/conf/autoapi.py
--rw-rw-rw-   0 root         (0) root         (0)     2466 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/conf/core.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/conf/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/conf/verify_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     6191 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/create_intersphinx_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/create_requirements_table.py
--rw-rw-rw-   0 root         (0) root         (0)     6730 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/create_workflow_diagram.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.239758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/tests/test_import.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.235758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.239758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.235758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.239758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/css/
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/css/dkist.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.239758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/img/
--rw-rw-rw-   0 root         (0) root         (0)    46900 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-blue-text.png
--rw-rw-rw-   0 root         (0) root         (0)    23107 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-white-text.png
--rw-rw-rw-   0 root         (0) root         (0)    41662 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/img/favico.ico
--rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/img/nso_logo.png
--rw-rw-rw-   0 root         (0) root         (0)      494 2024-04-19 15:52:30.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/theme.conf
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-19 15:52:41.239758 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-19 15:52:41.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1264 2024-04-19 15:52:41.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-19 15:52:41.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-19 15:52:41.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-04-19 15:52:41.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-04-19 15:52:41.000000 dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.746403 dkist-sphinx-theme-2.0.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)    19617 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1006 2024-04-11 09:52:23.746403 dkist-sphinx-theme-2.0.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-11 09:52:23.746403 dkist-sphinx-theme-2.0.0rc1/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.738403 dkist-sphinx-theme-2.0.0rc1/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.738403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/
+-rw-rw-rw-   0 root         (0) root         (0)     3884 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.738403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/autoapi_templates/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/autoapi_templates/python/
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/autoapi_templates/python/module.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/autoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/core.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/verify_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     6191 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_intersphinx_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_requirements_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     6730 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_workflow_diagram.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/tests/test_import.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.738403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.738403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/css/dkist.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)    46900 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-blue-text.png
+-rw-rw-rw-   0 root         (0) root         (0)    23107 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-white-text.png
+-rw-rw-rw-   0 root         (0) root         (0)    41662 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/favico.ico
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/nso_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      494 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/theme.conf
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1006 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/top_level.txt
```

### Comparing `dkist_sphinx_theme-2.0.0/LICENSE.rst` & `dkist-sphinx-theme-2.0.0rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/PKG-INFO` & `dkist-sphinx-theme-2.0.0rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-sphinx-theme
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: The sphinx theme for the DKIST documentation.
 Author: NSO / AURA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Sphinx
```

### Comparing `dkist_sphinx_theme-2.0.0/bitbucket-pipelines.yml` & `dkist-sphinx-theme-2.0.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/pyproject.toml` & `dkist-sphinx-theme-2.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/__init__.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/autoapi_templates/python/module.rst` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/autoapi_templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/conf/autoapi.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/autoapi.py`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/conf/core.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/core.py`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/conf/verify_requirements.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/verify_requirements.py`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/create_intersphinx_mapping.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_intersphinx_mapping.py`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/create_requirements_table.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_requirements_table.py`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/create_workflow_diagram.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_workflow_diagram.py`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/css/dkist.css` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/css/dkist.css`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-blue-text.png` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-blue-text.png`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-white-text.png` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-white-text.png`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/img/favico.ico` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/favico.ico`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme/theme/dkist/static/img/nso_logo.png` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/nso_logo.png`

 * *Files identical despite different names*

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme.egg-info/PKG-INFO` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-sphinx-theme
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: The sphinx theme for the DKIST documentation.
 Author: NSO / AURA
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Sphinx
```

### Comparing `dkist_sphinx_theme-2.0.0/src/dkist_sphinx_theme.egg-info/SOURCES.txt` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

