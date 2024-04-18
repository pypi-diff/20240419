# Comparing `tmp/green-4.0.1.tar.gz` & `tmp/green-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green-4.0.1.tar", last modified: Thu Feb 15 16:39:02 2024, max compression
+gzip compressed data, was "green-4.0.2.tar", last modified: Thu Apr 18 23:54:15 2024, max compression
```

## Comparing `green-4.0.1.tar` & `green-4.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:02.101544 green-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-15 16:38:38.000000 green-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-15 16:38:38.000000 green-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-02-15 16:39:02.101544 green-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-15 16:38:38.000000 green-4.0.1/README-pypi.rst
--rw-r--r--   0 runner    (1001) docker     (127)    21609 2024-02-15 16:38:38.000000 green-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:02.093544 green-4.0.1/green/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-15 16:38:38.000000 green-4.0.1/green/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-15 16:38:38.000000 green-4.0.1/green/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-15 16:38:38.000000 green-4.0.1/green/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-02-15 16:38:38.000000 green-4.0.1/green/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-02-15 16:38:38.000000 green-4.0.1/green/command.py
--rw-r--r--   0 runner    (1001) docker     (127)    27762 2024-02-15 16:38:38.000000 green-4.0.1/green/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-02-15 16:38:38.000000 green-4.0.1/green/djangorunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-15 16:38:38.000000 green-4.0.1/green/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-15 16:38:38.000000 green-4.0.1/green/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-02-15 16:38:38.000000 green-4.0.1/green/junit.py
--rw-r--r--   0 runner    (1001) docker     (127)    22891 2024-02-15 16:38:38.000000 green-4.0.1/green/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-02-15 16:38:38.000000 green-4.0.1/green/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-02-15 16:38:38.000000 green-4.0.1/green/process.py
--rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-02-15 16:38:38.000000 green-4.0.1/green/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-02-15 16:38:38.000000 green-4.0.1/green/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-15 16:38:38.000000 green-4.0.1/green/shell_completion.sh
--rw-r--r--   0 runner    (1001) docker     (127)     9868 2024-02-15 16:38:38.000000 green-4.0.1/green/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:02.097544 green-4.0.1/green/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 16:38:38.000000 green-4.0.1/green/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    26112 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_djangorunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_junit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_load_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    32933 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    36877 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-15 16:38:38.000000 green-4.0.1/green/test/test_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-15 16:38:38.000000 green-4.0.1/green/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:39:02.097544 green-4.0.1/green.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-02-15 16:39:02.000000 green-4.0.1/green.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-02-15 16:39:02.000000 green-4.0.1/green.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 16:39:02.000000 green-4.0.1/green.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-15 16:39:02.000000 green-4.0.1/green.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-15 16:39:02.000000 green-4.0.1/green.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-15 16:39:02.000000 green-4.0.1/green.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-15 16:38:38.000000 green-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-15 16:38:38.000000 green-4.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-15 16:38:38.000000 green-4.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-02-15 16:39:02.101544 green-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-15 16:38:38.000000 green-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:54:15.914416 green-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-18 23:53:48.000000 green-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 23:53:48.000000 green-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-18 23:54:15.914416 green-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-18 23:53:48.000000 green-4.0.2/README-pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21609 2024-04-18 23:53:48.000000 green-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:54:15.906416 green-4.0.2/green/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 23:53:48.000000 green-4.0.2/green/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 23:53:48.000000 green-4.0.2/green/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 23:53:48.000000 green-4.0.2/green/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-18 23:53:48.000000 green-4.0.2/green/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-18 23:53:48.000000 green-4.0.2/green/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27762 2024-04-18 23:53:48.000000 green-4.0.2/green/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-18 23:53:48.000000 green-4.0.2/green/djangorunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-18 23:53:48.000000 green-4.0.2/green/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 23:53:48.000000 green-4.0.2/green/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-18 23:53:48.000000 green-4.0.2/green/junit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22891 2024-04-18 23:53:48.000000 green-4.0.2/green/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-04-18 23:53:48.000000 green-4.0.2/green/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-04-18 23:53:48.000000 green-4.0.2/green/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-04-18 23:53:48.000000 green-4.0.2/green/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-18 23:53:48.000000 green-4.0.2/green/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-18 23:53:48.000000 green-4.0.2/green/shell_completion.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     9868 2024-04-18 23:53:48.000000 green-4.0.2/green/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:54:15.910416 green-4.0.2/green/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 23:53:48.000000 green-4.0.2/green/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26112 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_djangorunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_junit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_load_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32933 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37216 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-18 23:53:48.000000 green-4.0.2/green/test/test_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-18 23:53:48.000000 green-4.0.2/green/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:54:15.910416 green-4.0.2/green.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-18 23:54:15.000000 green-4.0.2/green.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-18 23:54:15.000000 green-4.0.2/green.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 23:54:15.000000 green-4.0.2/green.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 23:54:15.000000 green-4.0.2/green.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 23:54:15.000000 green-4.0.2/green.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 23:54:15.000000 green-4.0.2/green.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 23:53:48.000000 green-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-18 23:53:48.000000 green-4.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 23:53:48.000000 green-4.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-18 23:54:15.914416 green-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-18 23:53:48.000000 green-4.0.2/setup.py
```

### Comparing `green-4.0.1/LICENSE` & `green-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `green-4.0.1/PKG-INFO` & `green-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green
-Version: 4.0.1
+Version: 4.0.2
 Summary: Green is a clean, colorful, fast python test runner.
 Home-page: https://github.com/CleanCut/green
 Author: Nathan Stocks
 Author-email: nathan.stocks@gmail.com
 Maintainer: Nathan Stocks
 License: 'MIT'
 Keywords: nose, nose2, trial, pytest, py.test, tox, green,,tdd, test, tests, functional, system, unit, unittest,,color, tabular, clean, red, rednose, regression, runner,,integration,smoke, white, black, box, incremental, end,,end-to-end, sanity, acceptance, load, stress, performance,,usability, install, uninstall, recovery, security,,comparison, alpha, beta, non-functional, destructive,,accessibility, internationalization, i18n, localization, l10n,,development, a/b, concurrent, conformance, verification,,validation, quality, assurance, ad-hoc, agile, api,,automated, all, pairs, pairwise, boundary, value, branch,,browser, condition, coverage, dynamic, exploratory,,equivalence, partitioning, fuzz, gui, glass, gorilla,,interface, keyword, penetration, retesting, risk, based,,scalability, soak, volume, vulnerability
```

### Comparing `green-4.0.1/README-pypi.rst` & `green-4.0.2/README-pypi.rst`

 * *Files identical despite different names*

### Comparing `green-4.0.1/README.md` & `green-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/cmdline.py` & `green-4.0.2/green/cmdline.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/command.py` & `green-4.0.2/green/command.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/config.py` & `green-4.0.2/green/config.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/djangorunner.py` & `green-4.0.2/green/djangorunner.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/examples.py` & `green-4.0.2/green/examples.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/junit.py` & `green-4.0.2/green/junit.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/loader.py` & `green-4.0.2/green/loader.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/output.py` & `green-4.0.2/green/output.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/process.py` & `green-4.0.2/green/process.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/result.py` & `green-4.0.2/green/result.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -325,16 +325,16 @@
         self.finalize_callback = None
 
     def startTest(self, test: RunnableTestT) -> None:
         """
         Called before each test runs.
         """
         test = proto_test(test)
-        self.start_time = time.time()
         self.reinitialize()
+        self.start_time = time.time()
         if self.start_callback:
             self.start_callback(test)
 
     def stopTest(self, test: RunnableTestT) -> None:
         """
         Called after each test runs.
         """
```

### Comparing `green-4.0.1/green/runner.py` & `green-4.0.2/green/runner.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/shell_completion.sh` & `green-4.0.2/green/shell_completion.sh`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/suite.py` & `green-4.0.2/green/suite.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_cmdline.py` & `green-4.0.2/green/test/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_command.py` & `green-4.0.2/green/test/test_command.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_config.py` & `green-4.0.2/green/test/test_config.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_djangorunner.py` & `green-4.0.2/green/test/test_djangorunner.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_integration.py` & `green-4.0.2/green/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_junit.py` & `green-4.0.2/green/test/test_junit.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_load_tests.py` & `green-4.0.2/green/test/test_load_tests.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_loader.py` & `green-4.0.2/green/test/test_loader.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_output.py` & `green-4.0.2/green/test/test_output.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_process.py` & `green-4.0.2/green/test/test_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,18 +99,20 @@
                 def testPass(self):
                     pass
             """
             )
         )
         fh.close()
         module_name = basename + ".test_pool_runner_dotted.A.testPass"
-        result = Queue()
-        poolRunner(module_name, result, 1)
-        result.get()
-        self.assertEqual(len(result.get().passing), 1)
+        results = Queue()
+        poolRunner(module_name, results, 1)
+        results.get()
+        result = results.get()
+        self.assertEqual(len(result.passing), 1)
+        self.assertGreater(float(result.test_time), 0)
 
     def test_SyntaxErrorInUnitTest(self):
         """
         SyntaxError gets reported as an error loading the unit test
         """
         saved_coverage = process.coverage
         process.coverage = MagicMock()
```

### Comparing `green-4.0.1/green/test/test_result.py` & `green-4.0.2/green/test/test_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,25 @@
         pt = ProtoTest()
         btr.stderr_errput[pt] = noise
         btr.displayStderr(pt)
         self.assertIn(noise, stream.getvalue())
 
 
 class TestProtoTestResult(unittest.TestCase):
+    def test_startStop(self):
+        """
+        startTest/stopTest work correctly
+        """
+        ptr = ProtoTestResult()
+        test = proto_test(MagicMock())
+        with patch("time.time", side_effect=[101, 123]):
+            ptr.startTest(test)
+            ptr.stopTest(test)
+        self.assertEqual(float(ptr.test_time), 22)
+
     def test_addSuccess(self):
         """
         addSuccess adds a test correctly
         """
         ptr = ProtoTestResult()
         test = proto_test(MagicMock())
         ptr.addSuccess(test)
```

### Comparing `green-4.0.1/green/test/test_runner.py` & `green-4.0.2/green/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_suite.py` & `green-4.0.2/green/test/test_suite.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_version.py` & `green-4.0.2/green/test/test_version.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/test/test_windows.py` & `green-4.0.2/green/test/test_windows.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green/version.py` & `green-4.0.2/green/version.py`

 * *Files identical despite different names*

### Comparing `green-4.0.1/green.egg-info/PKG-INFO` & `green-4.0.2/green.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green
-Version: 4.0.1
+Version: 4.0.2
 Summary: Green is a clean, colorful, fast python test runner.
 Home-page: https://github.com/CleanCut/green
 Author: Nathan Stocks
 Author-email: nathan.stocks@gmail.com
 Maintainer: Nathan Stocks
 License: 'MIT'
 Keywords: nose, nose2, trial, pytest, py.test, tox, green,,tdd, test, tests, functional, system, unit, unittest,,color, tabular, clean, red, rednose, regression, runner,,integration,smoke, white, black, box, incremental, end,,end-to-end, sanity, acceptance, load, stress, performance,,usability, install, uninstall, recovery, security,,comparison, alpha, beta, non-functional, destructive,,accessibility, internationalization, i18n, localization, l10n,,development, a/b, concurrent, conformance, verification,,validation, quality, assurance, ad-hoc, agile, api,,automated, all, pairs, pairwise, boundary, value, branch,,browser, condition, coverage, dynamic, exploratory,,equivalence, partitioning, fuzz, gui, glass, gorilla,,interface, keyword, penetration, retesting, risk, based,,scalability, soak, volume, vulnerability
```

### Comparing `green-4.0.1/green.egg-info/SOURCES.txt` & `green-4.0.2/green.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `green-4.0.1/pyproject.toml` & `green-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `green-4.0.1/setup.cfg` & `green-4.0.2/setup.cfg`

 * *Files identical despite different names*

