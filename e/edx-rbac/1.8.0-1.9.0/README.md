# Comparing `tmp/edx-rbac-1.8.0.tar.gz` & `tmp/edx-rbac-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-rbac-1.8.0.tar", last modified: Thu Jul 27 14:19:05 2023, max compression
+gzip compressed data, was "edx-rbac-1.9.0.tar", last modified: Fri Apr 19 18:44:14 2024, max compression
```

## Comparing `edx-rbac-1.8.0.tar` & `edx-rbac-1.9.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.997646 edx-rbac-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     6755 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35117 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10266 2023-07-27 14:19:04.997646 edx-rbac-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.993646 edx-rbac-1.8.0/edx_rbac/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.993646 edx-rbac-1.8.0/edx_rbac/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     7651 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     3412 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.989646 edx-rbac-1.8.0/edx_rbac/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.993646 edx-rbac-1.8.0/edx_rbac/templates/edx_rbac/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/templates/edx_rbac/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     8351 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/edx_rbac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.993646 edx-rbac-1.8.0/edx_rbac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10266 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-27 14:19:04.000000 edx-rbac-1.8.0/edx_rbac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.997646 edx-rbac-1.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-27 14:19:04.997646 edx-rbac-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5309 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 14:19:04.997646 edx-rbac-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_assignments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     2376 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     8860 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    24090 2023-07-27 14:18:59.000000 edx-rbac-1.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:44:14.742712 edx-rbac-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35117 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-04-19 18:44:14.742712 edx-rbac-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:44:14.742712 edx-rbac-1.9.0/edx_rbac/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:44:14.742712 edx-rbac-1.9.0/edx_rbac/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:44:14.738712 edx-rbac-1.9.0/edx_rbac/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:44:14.742712 edx-rbac-1.9.0/edx_rbac/templates/edx_rbac/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/templates/edx_rbac/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/edx_rbac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:44:14.742712 edx-rbac-1.9.0/edx_rbac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-04-19 18:44:14.000000 edx-rbac-1.9.0/edx_rbac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 18:44:14.000000 edx-rbac-1.9.0/edx_rbac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:44:14.000000 edx-rbac-1.9.0/edx_rbac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:44:14.000000 edx-rbac-1.9.0/edx_rbac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 18:44:14.000000 edx-rbac-1.9.0/edx_rbac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 18:44:14.000000 edx-rbac-1.9.0/edx_rbac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:44:14.742712 edx-rbac-1.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 18:44:14.746712 edx-rbac-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:44:14.742712 edx-rbac-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/tests/test_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24090 2024-04-19 18:44:11.000000 edx-rbac-1.9.0/tests/test_utils.py
```

### Comparing `edx-rbac-1.8.0/CHANGELOG.rst` & `edx-rbac-1.9.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 --------------------
 
+[1.9.0]
+-------
+* Add support for Python 3.11 & 3.12
+
 [1.8.0]
 -------
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 * Added support for Django 4.2
 
 [1.7.0]
```

### Comparing `edx-rbac-1.8.0/LICENSE` & `edx-rbac-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/LICENSE.txt` & `edx-rbac-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/PKG-INFO` & `edx-rbac-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: edx-rbac
-Version: 1.8.0
+Version: 1.9.0
 Summary: Library to help managing role based access controls for django apps
 Home-page: https://github.com/openedx/edx-rbac
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 License-File: LICENSE.txt
 License-File: AUTHORS
+Requires-Dist: Django
+Requires-Dist: django-crum
+Requires-Dist: django-model-utils
+Requires-Dist: edx-drf-extensions
+Requires-Dist: setuptools
+Requires-Dist: six
 
 edx-rbac
 =============================
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
 
@@ -58,15 +65,15 @@
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-rbac/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
 
@@ -110,14 +117,18 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 --------------------
 
+[1.9.0]
+-------
+* Add support for Python 3.11 & 3.12
+
 [1.8.0]
 -------
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 * Added support for Django 4.2
 
 [1.7.0]
```

### Comparing `edx-rbac-1.8.0/README.rst` & `edx-rbac-1.9.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-rbac/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
```

### Comparing `edx-rbac-1.8.0/edx_rbac/admin/__init__.py` & `edx-rbac-1.9.0/edx_rbac/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/edx_rbac/admin/forms.py` & `edx-rbac-1.9.0/edx_rbac/admin/forms.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/edx_rbac/decorators.py` & `edx-rbac-1.9.0/edx_rbac/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/edx_rbac/fields.py` & `edx-rbac-1.9.0/edx_rbac/fields.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/edx_rbac/mixins.py` & `edx-rbac-1.9.0/edx_rbac/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/edx_rbac/models.py` & `edx-rbac-1.9.0/edx_rbac/models.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/edx_rbac/templates/edx_rbac/base.html` & `edx-rbac-1.9.0/edx_rbac/templates/edx_rbac/base.html`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/edx_rbac/utils.py` & `edx-rbac-1.9.0/edx_rbac/utils.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/edx_rbac.egg-info/PKG-INFO` & `edx-rbac-1.9.0/edx_rbac.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: edx-rbac
-Version: 1.8.0
+Version: 1.9.0
 Summary: Library to help managing role based access controls for django apps
 Home-page: https://github.com/openedx/edx-rbac
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 License-File: LICENSE.txt
 License-File: AUTHORS
+Requires-Dist: Django
+Requires-Dist: django-crum
+Requires-Dist: django-model-utils
+Requires-Dist: edx-drf-extensions
+Requires-Dist: setuptools
+Requires-Dist: six
 
 edx-rbac
 =============================
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge|
 
@@ -58,15 +65,15 @@
 
 Issue report template should be automatically applied if you are sending it from github UI as well; otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-rbac/blob/master/.github/ISSUE_TEMPLATE.md>`_
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to this `list of resources`_ if you need any assistance.
 
@@ -110,14 +117,18 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 --------------------
 
+[1.9.0]
+-------
+* Add support for Python 3.11 & 3.12
+
 [1.8.0]
 -------
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 * Added support for Django 4.2
 
 [1.7.0]
```

### Comparing `edx-rbac-1.8.0/edx_rbac.egg-info/SOURCES.txt` & `edx-rbac-1.9.0/edx_rbac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/requirements/constraints.txt` & `edx-rbac-1.9.0/requirements/constraints.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,7 +9,11 @@
 # linking to it here is good.
 
 -c common_constraints.txt
 
 # diff-cover latest requires (pluggy>=0.13.1,<0.14.0) which conflicts with pytest which requires(pluggy>=0.12,<2.0.0)
 # Using the same version of diff-cover which is being used currently in edx-platform to avoid this conflict.
 diff-cover==4.0.0
+
+
+# Temporary to Support the python 3.11 Upgrade
+backports.zoneinfo;python_version<"3.9"  # Newer versions have zoneinfo available in the standard library
```

### Comparing `edx-rbac-1.8.0/setup.py` & `edx-rbac-1.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,16 +116,17 @@
     install_requires=load_requirements('requirements/base.in'),
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8'
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `edx-rbac-1.8.0/tests/test_fields.py` & `edx-rbac-1.9.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/tests/test_forms.py` & `edx-rbac-1.9.0/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/tests/test_mixins.py` & `edx-rbac-1.9.0/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `edx-rbac-1.8.0/tests/test_utils.py` & `edx-rbac-1.9.0/tests/test_utils.py`

 * *Files identical despite different names*

