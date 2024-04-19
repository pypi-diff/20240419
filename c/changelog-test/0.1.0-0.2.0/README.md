# Comparing `tmp/changelog_test-0.1.0.tar.gz` & `tmp/changelog_test-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelog_test-0.1.0.tar", last modified: Fri Apr 19 14:49:37 2024, max compression
+gzip compressed data, was "changelog_test-0.2.0.tar", last modified: Fri Apr 19 19:58:14 2024, max compression
```

## Comparing `changelog_test-0.1.0.tar` & `changelog_test-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.379840 changelog_test-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 14:49:25.000000 changelog_test-0.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.367840 changelog_test-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.371840 changelog_test-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-19 14:49:25.000000 changelog_test-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-19 14:49:25.000000 changelog_test-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 14:49:25.000000 changelog_test-0.1.0/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.371840 changelog_test-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-19 14:49:25.000000 changelog_test-0.1.0/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-19 14:49:25.000000 changelog_test-0.1.0/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-19 14:49:25.000000 changelog_test-0.1.0/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-19 14:49:25.000000 changelog_test-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 14:49:25.000000 changelog_test-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-19 14:49:25.000000 changelog_test-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-19 14:49:37.379840 changelog_test-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-19 14:49:25.000000 changelog_test-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.375840 changelog_test-0.1.0/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 14:49:25.000000 changelog_test-0.1.0/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 14:49:25.000000 changelog_test-0.1.0/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.375840 changelog_test-0.1.0/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.375840 changelog_test-0.1.0/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-19 14:49:25.000000 changelog_test-0.1.0/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-19 14:49:25.000000 changelog_test-0.1.0/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-19 14:49:25.000000 changelog_test-0.1.0/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-19 14:49:25.000000 changelog_test-0.1.0/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-19 14:49:25.000000 changelog_test-0.1.0/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-19 14:49:25.000000 changelog_test-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:49:37.379840 changelog_test-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 14:49:25.000000 changelog_test-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.371840 changelog_test-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.375840 changelog_test-0.1.0/src/changelog_test/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 14:49:25.000000 changelog_test-0.1.0/src/changelog_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.375840 changelog_test-0.1.0/src/changelog_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-19 14:49:37.000000 changelog_test-0.1.0/src/changelog_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 14:49:37.000000 changelog_test-0.1.0/src/changelog_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:49:37.000000 changelog_test-0.1.0/src/changelog_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 14:49:37.000000 changelog_test-0.1.0/src/changelog_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 14:49:37.000000 changelog_test-0.1.0/src/changelog_test.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:49:37.375840 changelog_test-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 14:49:25.000000 changelog_test-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-19 14:49:25.000000 changelog_test-0.1.0/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.560148 changelog_test-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 19:58:02.000000 changelog_test-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.552148 changelog_test-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.556148 changelog_test-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-19 19:58:02.000000 changelog_test-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-19 19:58:02.000000 changelog_test-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 19:58:02.000000 changelog_test-0.2.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.556148 changelog_test-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-19 19:58:02.000000 changelog_test-0.2.0/.github/workflows/init.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-19 19:58:02.000000 changelog_test-0.2.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-19 19:58:02.000000 changelog_test-0.2.0/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-19 19:58:02.000000 changelog_test-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-19 19:58:03.000000 changelog_test-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-19 19:58:02.000000 changelog_test-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-19 19:58:14.560148 changelog_test-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-19 19:58:02.000000 changelog_test-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.556148 changelog_test-0.2.0/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 19:58:02.000000 changelog_test-0.2.0/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-19 19:58:02.000000 changelog_test-0.2.0/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.556148 changelog_test-0.2.0/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.560148 changelog_test-0.2.0/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-19 19:58:02.000000 changelog_test-0.2.0/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-19 19:58:02.000000 changelog_test-0.2.0/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-19 19:58:02.000000 changelog_test-0.2.0/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-19 19:58:02.000000 changelog_test-0.2.0/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-19 19:58:02.000000 changelog_test-0.2.0/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-19 19:58:02.000000 changelog_test-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:58:14.560148 changelog_test-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 19:58:02.000000 changelog_test-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.552148 changelog_test-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.560148 changelog_test-0.2.0/src/changelog_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 19:58:02.000000 changelog_test-0.2.0/src/changelog_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.560148 changelog_test-0.2.0/src/changelog_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-19 19:58:14.000000 changelog_test-0.2.0/src/changelog_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-19 19:58:14.000000 changelog_test-0.2.0/src/changelog_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:58:14.000000 changelog_test-0.2.0/src/changelog_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 19:58:14.000000 changelog_test-0.2.0/src/changelog_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 19:58:14.000000 changelog_test-0.2.0/src/changelog_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:02.000000 changelog_test-0.2.0/test
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:14.560148 changelog_test-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 19:58:02.000000 changelog_test-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-19 19:58:02.000000 changelog_test-0.2.0/tests/test_example.py
```

### Comparing `changelog_test-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `changelog_test-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `changelog_test-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/.github/ISSUE_TEMPLATE/user-story.md` & `changelog_test-0.2.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/.github/workflows/init.yml` & `changelog_test-0.2.0/.github/workflows/init.yml`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/.github/workflows/tag_and_publish.yml` & `changelog_test-0.2.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/.github/workflows/test_and_lint.yml` & `changelog_test-0.2.0/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/.gitignore` & `changelog_test-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/LICENSE` & `changelog_test-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/PKG-INFO` & `changelog_test-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog_test
-Version: 0.1.0
+Version: 0.2.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `changelog_test-0.1.0/README.md` & `changelog_test-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/doc_template/Makefile` & `changelog_test-0.2.0/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/doc_template/make.bat` & `changelog_test-0.2.0/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/doc_template/source/_static/dark-logo.svg` & `changelog_test-0.2.0/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/doc_template/source/_static/favicon.ico` & `changelog_test-0.2.0/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/doc_template/source/_static/light-logo.svg` & `changelog_test-0.2.0/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/doc_template/source/conf.py` & `changelog_test-0.2.0/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/pyproject.toml` & `changelog_test-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `changelog_test-0.1.0/src/changelog_test.egg-info/PKG-INFO` & `changelog_test-0.2.0/src/changelog_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog_test
-Version: 0.1.0
+Version: 0.2.0
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `changelog_test-0.1.0/src/changelog_test.egg-info/SOURCES.txt` & `changelog_test-0.2.0/src/changelog_test.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .flake8
 .gitignore
 CHANGELOG.md
 LICENSE
 README.md
 pyproject.toml
 setup.py
+test
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/user-story.md
 .github/workflows/init.yml
 .github/workflows/tag_and_publish.yml
 .github/workflows/test_and_lint.yml
 doc_template/Makefile
```

