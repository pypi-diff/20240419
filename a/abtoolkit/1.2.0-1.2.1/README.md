# Comparing `tmp/abtoolkit-1.2.0.tar.gz` & `tmp/abtoolkit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abtoolkit-1.2.0.tar", last modified: Fri Mar 29 12:30:41 2024, max compression
+gzip compressed data, was "abtoolkit-1.2.1.tar", last modified: Fri Apr 19 07:42:53 2024, max compression
```

## Comparing `abtoolkit-1.2.0.tar` & `abtoolkit-1.2.1.tar`

### file list

```diff
@@ -1,51 +1,61 @@
-drwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-29 12:30:41.202444 abtoolkit-1.2.0/
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     1062 2024-03-22 09:28:06.000000 abtoolkit-1.2.0/LICENSE
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     4833 2024-03-29 12:30:41.202137 abtoolkit-1.2.0/PKG-INFO
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     4103 2024-03-25 15:10:54.000000 abtoolkit-1.2.0/README.md
-drwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-29 12:30:41.191591 abtoolkit-1.2.0/abtoolkit/
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-23 05:39:11.000000 abtoolkit-1.2.0/abtoolkit/__init__.py
-drwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-29 12:30:41.193971 abtoolkit-1.2.0/abtoolkit/continuous/
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-22 09:33:10.000000 abtoolkit-1.2.0/abtoolkit/continuous/__init__.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     7637 2024-03-29 12:15:29.000000 abtoolkit-1.2.0/abtoolkit/continuous/simulation.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)    10878 2024-03-28 15:35:50.000000 abtoolkit-1.2.0/abtoolkit/continuous/stattests.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     3381 2024-03-29 11:44:42.000000 abtoolkit-1.2.0/abtoolkit/continuous/utils.py
-drwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-29 12:30:41.195044 abtoolkit-1.2.0/abtoolkit/discrete/
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-22 09:32:58.000000 abtoolkit-1.2.0/abtoolkit/discrete/__init__.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     2396 2024-03-29 12:15:29.000000 abtoolkit-1.2.0/abtoolkit/discrete/simulation.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     1609 2024-03-29 11:46:38.000000 abtoolkit-1.2.0/abtoolkit/discrete/stattests.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     1801 2024-03-29 12:07:16.000000 abtoolkit-1.2.0/abtoolkit/discrete/utils.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     6152 2024-03-29 11:56:12.000000 abtoolkit-1.2.0/abtoolkit/utils.py
-drwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-29 12:30:41.201781 abtoolkit-1.2.0/abtoolkit.egg-info/
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     4833 2024-03-29 12:30:41.000000 abtoolkit-1.2.0/abtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     1074 2024-03-29 12:30:41.000000 abtoolkit-1.2.0/abtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        1 2024-03-29 12:30:41.000000 abtoolkit-1.2.0/abtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)       93 2024-03-29 12:30:41.000000 abtoolkit-1.2.0/abtoolkit.egg-info/requires.txt
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)       42 2024-03-29 12:30:41.000000 abtoolkit-1.2.0/abtoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-29 12:30:41.195575 abtoolkit-1.2.0/examples/
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     1864 2024-03-29 08:48:35.000000 abtoolkit-1.2.0/examples/continuous_var_analysis.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     1479 2024-03-29 11:34:01.000000 abtoolkit-1.2.0/examples/discrete_var_analysis.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     1021 2024-03-29 12:29:44.000000 abtoolkit-1.2.0/pyproject.toml
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)       38 2024-03-29 12:30:41.202495 abtoolkit-1.2.0/setup.cfg
-drwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-29 12:30:41.197504 abtoolkit-1.2.0/tests/
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-22 08:45:06.000000 abtoolkit-1.2.0/tests/__init__.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     2727 2024-03-29 08:48:35.000000 abtoolkit-1.2.0/tests/test_continuous_simulation.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     5436 2024-03-29 08:48:35.000000 abtoolkit-1.2.0/tests/test_continuous_stattests.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      795 2024-03-25 10:43:06.000000 abtoolkit-1.2.0/tests/test_continuous_utils.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     2426 2024-03-29 10:20:21.000000 abtoolkit-1.2.0/tests/test_discrete_simulation.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      583 2024-03-29 09:29:26.000000 abtoolkit-1.2.0/tests/test_discrete_stattests.py
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      865 2024-03-29 10:35:15.000000 abtoolkit-1.2.0/tests/test_discrete_utils.py
-drwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-29 12:30:41.190314 abtoolkit-1.2.0/venv/
-drwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)        0 2024-03-29 12:30:41.201419 abtoolkit-1.2.0/venv/bin/
--rw-r--r--   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     1175 2024-03-22 08:53:42.000000 abtoolkit-1.2.0/venv/bin/activate_this.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      648 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2html.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      770 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)     1105 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      847 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      670 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2man.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      836 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      642 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      655 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      691 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      927 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      656 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 naltukhov (1397289063) COMPANY\Domain Users (359461530)      724 2024-03-22 14:05:07.000000 abtoolkit-1.2.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:42:53.258296 abtoolkit-1.2.1/
+-rw-r--r--   0 naltukhov (1397289063) 359461530       32 2024-03-22 14:05:39.000000 abtoolkit-1.2.1/.gitignore
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1062 2024-03-22 09:28:06.000000 abtoolkit-1.2.1/LICENSE
+-rw-r--r--   0 naltukhov (1397289063) 359461530      558 2024-03-23 09:48:31.000000 abtoolkit-1.2.1/Makefile
+-rw-r--r--   0 naltukhov (1397289063) 359461530     5786 2024-04-19 07:42:53.258009 abtoolkit-1.2.1/PKG-INFO
+-rw-r--r--   0 naltukhov (1397289063) 359461530     5056 2024-03-29 12:51:18.000000 abtoolkit-1.2.1/README.md
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:42:53.245571 abtoolkit-1.2.1/abtoolkit/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-23 05:39:11.000000 abtoolkit-1.2.1/abtoolkit/__init__.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:42:53.246989 abtoolkit-1.2.1/abtoolkit/continuous/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 09:33:10.000000 abtoolkit-1.2.1/abtoolkit/continuous/__init__.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     7637 2024-03-29 12:15:29.000000 abtoolkit-1.2.1/abtoolkit/continuous/simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530    10878 2024-03-29 13:46:05.000000 abtoolkit-1.2.1/abtoolkit/continuous/stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     3381 2024-03-29 11:44:42.000000 abtoolkit-1.2.1/abtoolkit/continuous/utils.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:42:53.247490 abtoolkit-1.2.1/abtoolkit/discrete/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 09:32:58.000000 abtoolkit-1.2.1/abtoolkit/discrete/__init__.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     2396 2024-03-29 12:15:29.000000 abtoolkit-1.2.1/abtoolkit/discrete/simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1609 2024-03-29 11:46:38.000000 abtoolkit-1.2.1/abtoolkit/discrete/stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1801 2024-03-29 12:07:16.000000 abtoolkit-1.2.1/abtoolkit/discrete/utils.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     6152 2024-03-29 11:56:12.000000 abtoolkit-1.2.1/abtoolkit/utils.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:42:53.257624 abtoolkit-1.2.1/abtoolkit.egg-info/
+-rw-r--r--   0 naltukhov (1397289063) 359461530     5786 2024-04-19 07:42:53.000000 abtoolkit-1.2.1/abtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1248 2024-04-19 07:42:53.000000 abtoolkit-1.2.1/abtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530        1 2024-04-19 07:42:53.000000 abtoolkit-1.2.1/abtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530       93 2024-04-19 07:42:53.000000 abtoolkit-1.2.1/abtoolkit.egg-info/requires.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530       42 2024-04-19 07:42:53.000000 abtoolkit-1.2.1/abtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:42:53.248063 abtoolkit-1.2.1/examples/
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1844 2024-03-29 14:11:25.000000 abtoolkit-1.2.1/examples/continuous_var_analysis.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1479 2024-03-29 11:34:01.000000 abtoolkit-1.2.1/examples/discrete_var_analysis.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      260 2024-03-23 09:42:57.000000 abtoolkit-1.2.1/pre-commit.bash
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1021 2024-04-19 07:42:15.000000 abtoolkit-1.2.1/pyproject.toml
+-rw-r--r--   0 naltukhov (1397289063) 359461530      110 2024-03-22 14:16:03.000000 abtoolkit-1.2.1/requirements.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530       38 2024-04-19 07:42:53.258354 abtoolkit-1.2.1/setup.cfg
+-rw-r--r--   0 naltukhov (1397289063) 359461530      256 2024-04-19 07:41:47.000000 abtoolkit-1.2.1/setup.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:42:53.250364 abtoolkit-1.2.1/static/
+-rw-r--r--   0 naltukhov (1397289063) 359461530    41812 2024-03-29 12:49:51.000000 abtoolkit-1.2.1/static/discrete-output-plot.png
+-rw-r--r--   0 naltukhov (1397289063) 359461530   135844 2024-03-29 12:50:41.000000 abtoolkit-1.2.1/static/discrete-p-value-plot.png
+-rw-r--r--   0 naltukhov (1397289063) 359461530   185112 2024-03-29 12:52:31.000000 abtoolkit-1.2.1/static/output-plot.png
+-rw-r--r--   0 naltukhov (1397289063) 359461530   205019 2024-03-22 08:45:06.000000 abtoolkit-1.2.1/static/p-value-plot.png
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:42:53.253471 abtoolkit-1.2.1/tests/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 08:45:06.000000 abtoolkit-1.2.1/tests/__init__.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     2727 2024-03-29 08:48:35.000000 abtoolkit-1.2.1/tests/test_continuous_simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     5436 2024-03-29 08:48:35.000000 abtoolkit-1.2.1/tests/test_continuous_stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530      795 2024-03-25 10:43:06.000000 abtoolkit-1.2.1/tests/test_continuous_utils.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     2426 2024-03-29 10:20:21.000000 abtoolkit-1.2.1/tests/test_discrete_simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530      583 2024-03-29 09:29:26.000000 abtoolkit-1.2.1/tests/test_discrete_stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530      865 2024-03-29 10:35:15.000000 abtoolkit-1.2.1/tests/test_discrete_utils.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:42:53.243615 abtoolkit-1.2.1/venv/
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:42:53.257306 abtoolkit-1.2.1/venv/bin/
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1175 2024-03-22 08:53:42.000000 abtoolkit-1.2.1/venv/bin/activate_this.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      648 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2html.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      770 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2html4.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530     1105 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2html5.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      847 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2latex.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      670 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2man.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      836 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2odt.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      642 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      655 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      691 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2s5.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      927 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      656 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rst2xml.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      724 2024-03-22 14:05:07.000000 abtoolkit-1.2.1/venv/bin/rstpep2html.py
```

### Comparing `abtoolkit-1.2.0/LICENSE` & `abtoolkit-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/PKG-INFO` & `abtoolkit-1.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,20 @@
-Metadata-Version: 2.1
-Name: abtoolkit
-Version: 1.2.0
-Summary: Package with tools for AB testing
-Author-email: Nikita Altukhov <altuxov.nikita@gmail.com>
-Project-URL: Homepage, https://github.com/nikitosl/abtoolkit
-Project-URL: Issues, https://github.com/nikitosl/abtoolkit/issues
-Keywords: ab_test,cuped,did,ttest
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas>=2.2.1
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: statsmodels>=0.14.1
-Requires-Dist: scipy>=1.12.0
-Requires-Dist: linearmodels>=5.4
-Requires-Dist: tqdm>=4.66.2
-
 # ABToolkit
 Set of tools for AA and AB tests, sample size estimation, confidence intervals estimation. 
 For continuous and discrete variables.
 
 ## Install using pip:
 ```pip install abtoolkit```
 
 ## Continuous variables analysis
 #### Sample size estimation:
 ```
-from abtoolkit.continuous.utils import calculate_sample_size_by_mde
-calculate_sample_size_by_mde(
+from abtoolkit.continuous.utils import estimate_sample_size_by_mde
+
+estimate_sample_size_by_mde(
     std=variable.std(),
     alpha=alpha_level, 
     power=power, 
     mde=mde,
     alternative="two-sided"
 )
 ```
@@ -94,21 +74,43 @@
 of treatment impact.
 ```y = bias + w0 * treated + w1 * additional_variable1 + w2 * additional_variable2 + ...```
 
 
 ## Discrete variables analysis
 #### Sample size estimation:
 ```
-from abtoolkit.discrete.utils import estimate_ci_binomial
-estimate_ci_binomial(
+from abtoolkit.discrete.utils import estimate_sample_size_by_mde
+
+estimate_sample_size_by_mde(
     p, 
     sample_size, 
-    alpha=0.05
+    alpha=0.05,
+    alternative="two-sided"
 )
 ```
 #### AA and AB tests simulation:
-To Be Done
+```
+from abtoolkit.discrete.simulation import StatTestsSimulation
+
+sim = StatTestsSimulation(
+        count=variable.sum(),
+        objects_num=variable.count(),
+        stattests_list=["conversion_ztest"],
+        alternative=alternative,
+        experiments_num=experiments_num,  # Run each stattest 10 times
+        sample_size=sample_size,  # Take 50 samples from variables
+        mde=mde,  # Trying to detect this effect (very big for our simulated data)
+        alpha_level=alpha_level,  # Fix alpha level on 5%
+    )
+    info = sim.run()  # Get dictionary with information about tests
+    sim.print_results()  # Print results of simulation
+    sim.plot_p_values()  # Plot p-values distribution
+```
+Output:
+![discrete-output-plot.png](static%2Fdiscrete-output-plot.png)
+![discrete-p-value-plot.png](static%2Fdiscrete-p-value-plot.png)
+
 #### Next stat tests implemented for treatment effect estimation:
-To Be Done
+- ***Conversion Z-Test*** estimates treatment effect on conversion variable using z-test
 
 ---
-You can find examples of toolkit usage in [examples/](https://github.com/nikitosl/abtoolkit/tree/master/examples) directory.
+You can find examples of toolkit usage in [examples/](https://github.com/nikitosl/abtoolkit/tree/master/examples) directory.
```

### Comparing `abtoolkit-1.2.0/README.md` & `abtoolkit-1.2.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,41 @@
+Metadata-Version: 2.1
+Name: abtoolkit
+Version: 1.2.1
+Summary: Package with tools for AB testing
+Author-email: Nikita Altukhov <altuxov.nikita@gmail.com>
+Project-URL: Homepage, https://github.com/nikitosl/abtoolkit
+Project-URL: Issues, https://github.com/nikitosl/abtoolkit/issues
+Keywords: ab_test,cuped,did,ttest
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas>=2.2.1
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: statsmodels>=0.14.1
+Requires-Dist: scipy>=1.12.0
+Requires-Dist: linearmodels>=5.4
+Requires-Dist: tqdm>=4.66.2
+
 # ABToolkit
 Set of tools for AA and AB tests, sample size estimation, confidence intervals estimation. 
 For continuous and discrete variables.
 
 ## Install using pip:
 ```pip install abtoolkit```
 
 ## Continuous variables analysis
 #### Sample size estimation:
 ```
-from abtoolkit.continuous.utils import calculate_sample_size_by_mde
-calculate_sample_size_by_mde(
+from abtoolkit.continuous.utils import estimate_sample_size_by_mde
+
+estimate_sample_size_by_mde(
     std=variable.std(),
     alpha=alpha_level, 
     power=power, 
     mde=mde,
     alternative="two-sided"
 )
 ```
@@ -73,21 +95,43 @@
 of treatment impact.
 ```y = bias + w0 * treated + w1 * additional_variable1 + w2 * additional_variable2 + ...```
 
 
 ## Discrete variables analysis
 #### Sample size estimation:
 ```
-from abtoolkit.discrete.utils import estimate_ci_binomial
-estimate_ci_binomial(
+from abtoolkit.discrete.utils import estimate_sample_size_by_mde
+
+estimate_sample_size_by_mde(
     p, 
     sample_size, 
-    alpha=0.05
+    alpha=0.05,
+    alternative="two-sided"
 )
 ```
 #### AA and AB tests simulation:
-To Be Done
+```
+from abtoolkit.discrete.simulation import StatTestsSimulation
+
+sim = StatTestsSimulation(
+        count=variable.sum(),
+        objects_num=variable.count(),
+        stattests_list=["conversion_ztest"],
+        alternative=alternative,
+        experiments_num=experiments_num,  # Run each stattest 10 times
+        sample_size=sample_size,  # Take 50 samples from variables
+        mde=mde,  # Trying to detect this effect (very big for our simulated data)
+        alpha_level=alpha_level,  # Fix alpha level on 5%
+    )
+    info = sim.run()  # Get dictionary with information about tests
+    sim.print_results()  # Print results of simulation
+    sim.plot_p_values()  # Plot p-values distribution
+```
+Output:
+![discrete-output-plot.png](static%2Fdiscrete-output-plot.png)
+![discrete-p-value-plot.png](static%2Fdiscrete-p-value-plot.png)
+
 #### Next stat tests implemented for treatment effect estimation:
-To Be Done
+- ***Conversion Z-Test*** estimates treatment effect on conversion variable using z-test
 
 ---
-You can find examples of toolkit usage in [examples/](https://github.com/nikitosl/abtoolkit/tree/master/examples) directory.
+You can find examples of toolkit usage in [examples/](https://github.com/nikitosl/abtoolkit/tree/master/examples) directory.
```

### Comparing `abtoolkit-1.2.0/abtoolkit/continuous/simulation.py` & `abtoolkit-1.2.1/abtoolkit/continuous/simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/abtoolkit/continuous/stattests.py` & `abtoolkit-1.2.1/abtoolkit/continuous/stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/abtoolkit/continuous/utils.py` & `abtoolkit-1.2.1/abtoolkit/continuous/utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/abtoolkit/discrete/simulation.py` & `abtoolkit-1.2.1/abtoolkit/discrete/simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/abtoolkit/discrete/stattests.py` & `abtoolkit-1.2.1/abtoolkit/discrete/stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/abtoolkit/discrete/utils.py` & `abtoolkit-1.2.1/abtoolkit/discrete/utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/abtoolkit/utils.py` & `abtoolkit-1.2.1/abtoolkit/utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/abtoolkit.egg-info/PKG-INFO` & `abtoolkit-1.2.1/abtoolkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abtoolkit
-Version: 1.2.0
+Version: 1.2.1
 Summary: Package with tools for AB testing
 Author-email: Nikita Altukhov <altuxov.nikita@gmail.com>
 Project-URL: Homepage, https://github.com/nikitosl/abtoolkit
 Project-URL: Issues, https://github.com/nikitosl/abtoolkit/issues
 Keywords: ab_test,cuped,did,ttest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,16 +25,17 @@
 
 ## Install using pip:
 ```pip install abtoolkit```
 
 ## Continuous variables analysis
 #### Sample size estimation:
 ```
-from abtoolkit.continuous.utils import calculate_sample_size_by_mde
-calculate_sample_size_by_mde(
+from abtoolkit.continuous.utils import estimate_sample_size_by_mde
+
+estimate_sample_size_by_mde(
     std=variable.std(),
     alpha=alpha_level, 
     power=power, 
     mde=mde,
     alternative="two-sided"
 )
 ```
@@ -94,21 +95,43 @@
 of treatment impact.
 ```y = bias + w0 * treated + w1 * additional_variable1 + w2 * additional_variable2 + ...```
 
 
 ## Discrete variables analysis
 #### Sample size estimation:
 ```
-from abtoolkit.discrete.utils import estimate_ci_binomial
-estimate_ci_binomial(
+from abtoolkit.discrete.utils import estimate_sample_size_by_mde
+
+estimate_sample_size_by_mde(
     p, 
     sample_size, 
-    alpha=0.05
+    alpha=0.05,
+    alternative="two-sided"
 )
 ```
 #### AA and AB tests simulation:
-To Be Done
+```
+from abtoolkit.discrete.simulation import StatTestsSimulation
+
+sim = StatTestsSimulation(
+        count=variable.sum(),
+        objects_num=variable.count(),
+        stattests_list=["conversion_ztest"],
+        alternative=alternative,
+        experiments_num=experiments_num,  # Run each stattest 10 times
+        sample_size=sample_size,  # Take 50 samples from variables
+        mde=mde,  # Trying to detect this effect (very big for our simulated data)
+        alpha_level=alpha_level,  # Fix alpha level on 5%
+    )
+    info = sim.run()  # Get dictionary with information about tests
+    sim.print_results()  # Print results of simulation
+    sim.plot_p_values()  # Plot p-values distribution
+```
+Output:
+![discrete-output-plot.png](static%2Fdiscrete-output-plot.png)
+![discrete-p-value-plot.png](static%2Fdiscrete-p-value-plot.png)
+
 #### Next stat tests implemented for treatment effect estimation:
-To Be Done
+- ***Conversion Z-Test*** estimates treatment effect on conversion variable using z-test
 
 ---
 You can find examples of toolkit usage in [examples/](https://github.com/nikitosl/abtoolkit/tree/master/examples) directory.
```

### Comparing `abtoolkit-1.2.0/abtoolkit.egg-info/SOURCES.txt` & `abtoolkit-1.2.1/abtoolkit.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+.gitignore
 LICENSE
+Makefile
 README.md
+pre-commit.bash
 pyproject.toml
+requirements.txt
+setup.py
 abtoolkit/__init__.py
 abtoolkit/utils.py
 abtoolkit.egg-info/PKG-INFO
 abtoolkit.egg-info/SOURCES.txt
 abtoolkit.egg-info/dependency_links.txt
 abtoolkit.egg-info/requires.txt
 abtoolkit.egg-info/top_level.txt
@@ -14,14 +19,18 @@
 abtoolkit/continuous/utils.py
 abtoolkit/discrete/__init__.py
 abtoolkit/discrete/simulation.py
 abtoolkit/discrete/stattests.py
 abtoolkit/discrete/utils.py
 examples/continuous_var_analysis.py
 examples/discrete_var_analysis.py
+static/discrete-output-plot.png
+static/discrete-p-value-plot.png
+static/output-plot.png
+static/p-value-plot.png
 tests/__init__.py
 tests/test_continuous_simulation.py
 tests/test_continuous_stattests.py
 tests/test_continuous_utils.py
 tests/test_discrete_simulation.py
 tests/test_discrete_stattests.py
 tests/test_discrete_utils.py
```

### Comparing `abtoolkit-1.2.0/examples/continuous_var_analysis.py` & `abtoolkit-1.2.1/examples/continuous_var_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import numpy as np
-
 from abtoolkit.continuous.simulation import StatTestsSimulation
 from abtoolkit.continuous.utils import estimate_sample_size_by_mde
 from abtoolkit.utils import generate_data
 
 
 if __name__ == '__main__':
     # Fix global params
```

### Comparing `abtoolkit-1.2.0/examples/discrete_var_analysis.py` & `abtoolkit-1.2.1/examples/discrete_var_analysis.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/pyproject.toml` & `abtoolkit-1.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "abtoolkit"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Nikita Altukhov", email="altuxov.nikita@gmail.com" },
 ]
 description = "Package with tools for AB testing"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `abtoolkit-1.2.0/tests/test_continuous_simulation.py` & `abtoolkit-1.2.1/tests/test_continuous_simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/tests/test_continuous_stattests.py` & `abtoolkit-1.2.1/tests/test_continuous_stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/tests/test_continuous_utils.py` & `abtoolkit-1.2.1/tests/test_continuous_utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/tests/test_discrete_simulation.py` & `abtoolkit-1.2.1/tests/test_discrete_simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/tests/test_discrete_stattests.py` & `abtoolkit-1.2.1/tests/test_discrete_stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/tests/test_discrete_utils.py` & `abtoolkit-1.2.1/tests/test_discrete_utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/activate_this.py` & `abtoolkit-1.2.1/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2html.py` & `abtoolkit-1.2.1/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2html4.py` & `abtoolkit-1.2.1/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2html5.py` & `abtoolkit-1.2.1/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2latex.py` & `abtoolkit-1.2.1/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2man.py` & `abtoolkit-1.2.1/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2odt.py` & `abtoolkit-1.2.1/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2odt_prepstyles.py` & `abtoolkit-1.2.1/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2pseudoxml.py` & `abtoolkit-1.2.1/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2s5.py` & `abtoolkit-1.2.1/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2xetex.py` & `abtoolkit-1.2.1/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rst2xml.py` & `abtoolkit-1.2.1/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.0/venv/bin/rstpep2html.py` & `abtoolkit-1.2.1/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

