# Comparing `tmp/abtoolkit-1.2.2.tar.gz` & `tmp/abtoolkit-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abtoolkit-1.2.2.tar", last modified: Fri Apr 19 07:49:45 2024, max compression
+gzip compressed data, was "abtoolkit-1.2.3.tar", last modified: Fri Apr 19 07:53:44 2024, max compression
```

## Comparing `abtoolkit-1.2.2.tar` & `abtoolkit-1.2.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:49:45.751397 abtoolkit-1.2.2/
--rw-r--r--   0 naltukhov (1397289063) 359461530       32 2024-03-22 14:05:39.000000 abtoolkit-1.2.2/.gitignore
--rw-r--r--   0 naltukhov (1397289063) 359461530     1062 2024-03-22 09:28:06.000000 abtoolkit-1.2.2/LICENSE
--rw-r--r--   0 naltukhov (1397289063) 359461530      558 2024-03-23 09:48:31.000000 abtoolkit-1.2.2/Makefile
--rw-r--r--   0 naltukhov (1397289063) 359461530     5986 2024-04-19 07:49:45.751178 abtoolkit-1.2.2/PKG-INFO
--rw-r--r--   0 naltukhov (1397289063) 359461530     5256 2024-04-19 07:49:08.000000 abtoolkit-1.2.2/README.md
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:49:45.736608 abtoolkit-1.2.2/abtoolkit/
--rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-23 05:39:11.000000 abtoolkit-1.2.2/abtoolkit/__init__.py
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:49:45.737856 abtoolkit-1.2.2/abtoolkit/continuous/
--rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 09:33:10.000000 abtoolkit-1.2.2/abtoolkit/continuous/__init__.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     7637 2024-03-29 12:15:29.000000 abtoolkit-1.2.2/abtoolkit/continuous/simulation.py
--rw-r--r--   0 naltukhov (1397289063) 359461530    10878 2024-03-29 13:46:05.000000 abtoolkit-1.2.2/abtoolkit/continuous/stattests.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     3381 2024-03-29 11:44:42.000000 abtoolkit-1.2.2/abtoolkit/continuous/utils.py
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:49:45.738349 abtoolkit-1.2.2/abtoolkit/discrete/
--rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 09:32:58.000000 abtoolkit-1.2.2/abtoolkit/discrete/__init__.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     2396 2024-03-29 12:15:29.000000 abtoolkit-1.2.2/abtoolkit/discrete/simulation.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     1609 2024-03-29 11:46:38.000000 abtoolkit-1.2.2/abtoolkit/discrete/stattests.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     1801 2024-03-29 12:07:16.000000 abtoolkit-1.2.2/abtoolkit/discrete/utils.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     6152 2024-03-29 11:56:12.000000 abtoolkit-1.2.2/abtoolkit/utils.py
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:49:45.750908 abtoolkit-1.2.2/abtoolkit.egg-info/
--rw-r--r--   0 naltukhov (1397289063) 359461530     5986 2024-04-19 07:49:45.000000 abtoolkit-1.2.2/abtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 naltukhov (1397289063) 359461530     1248 2024-04-19 07:49:45.000000 abtoolkit-1.2.2/abtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 naltukhov (1397289063) 359461530        1 2024-04-19 07:49:45.000000 abtoolkit-1.2.2/abtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 naltukhov (1397289063) 359461530       93 2024-04-19 07:49:45.000000 abtoolkit-1.2.2/abtoolkit.egg-info/requires.txt
--rw-r--r--   0 naltukhov (1397289063) 359461530       42 2024-04-19 07:49:45.000000 abtoolkit-1.2.2/abtoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:49:45.738793 abtoolkit-1.2.2/examples/
--rw-r--r--   0 naltukhov (1397289063) 359461530     1844 2024-03-29 14:11:25.000000 abtoolkit-1.2.2/examples/continuous_var_analysis.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     1479 2024-03-29 11:34:01.000000 abtoolkit-1.2.2/examples/discrete_var_analysis.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      260 2024-03-23 09:42:57.000000 abtoolkit-1.2.2/pre-commit.bash
--rw-r--r--   0 naltukhov (1397289063) 359461530     1021 2024-04-19 07:49:40.000000 abtoolkit-1.2.2/pyproject.toml
--rw-r--r--   0 naltukhov (1397289063) 359461530      110 2024-03-22 14:16:03.000000 abtoolkit-1.2.2/requirements.txt
--rw-r--r--   0 naltukhov (1397289063) 359461530       38 2024-04-19 07:49:45.751446 abtoolkit-1.2.2/setup.cfg
--rw-r--r--   0 naltukhov (1397289063) 359461530      256 2024-04-19 07:41:47.000000 abtoolkit-1.2.2/setup.py
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:49:45.744654 abtoolkit-1.2.2/static/
--rw-r--r--   0 naltukhov (1397289063) 359461530    41812 2024-03-29 12:49:51.000000 abtoolkit-1.2.2/static/discrete-output-plot.png
--rw-r--r--   0 naltukhov (1397289063) 359461530   135844 2024-03-29 12:50:41.000000 abtoolkit-1.2.2/static/discrete-p-value-plot.png
--rw-r--r--   0 naltukhov (1397289063) 359461530   185112 2024-03-29 12:52:31.000000 abtoolkit-1.2.2/static/output-plot.png
--rw-r--r--   0 naltukhov (1397289063) 359461530   205019 2024-03-22 08:45:06.000000 abtoolkit-1.2.2/static/p-value-plot.png
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:49:45.746973 abtoolkit-1.2.2/tests/
--rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 08:45:06.000000 abtoolkit-1.2.2/tests/__init__.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     2727 2024-03-29 08:48:35.000000 abtoolkit-1.2.2/tests/test_continuous_simulation.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     5436 2024-03-29 08:48:35.000000 abtoolkit-1.2.2/tests/test_continuous_stattests.py
--rw-r--r--   0 naltukhov (1397289063) 359461530      795 2024-03-25 10:43:06.000000 abtoolkit-1.2.2/tests/test_continuous_utils.py
--rw-r--r--   0 naltukhov (1397289063) 359461530     2426 2024-03-29 10:20:21.000000 abtoolkit-1.2.2/tests/test_discrete_simulation.py
--rw-r--r--   0 naltukhov (1397289063) 359461530      583 2024-03-29 09:29:26.000000 abtoolkit-1.2.2/tests/test_discrete_stattests.py
--rw-r--r--   0 naltukhov (1397289063) 359461530      865 2024-03-29 10:35:15.000000 abtoolkit-1.2.2/tests/test_discrete_utils.py
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:49:45.734679 abtoolkit-1.2.2/venv/
-drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:49:45.750585 abtoolkit-1.2.2/venv/bin/
--rw-r--r--   0 naltukhov (1397289063) 359461530     1175 2024-03-22 08:53:42.000000 abtoolkit-1.2.2/venv/bin/activate_this.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      648 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2html.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      770 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2html4.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530     1105 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2html5.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      847 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2latex.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      670 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2man.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      836 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2odt.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      642 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      655 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      691 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2s5.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      927 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2xetex.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      656 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rst2xml.py
--rwxr-xr-x   0 naltukhov (1397289063) 359461530      724 2024-03-22 14:05:07.000000 abtoolkit-1.2.2/venv/bin/rstpep2html.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:53:44.107817 abtoolkit-1.2.3/
+-rw-r--r--   0 naltukhov (1397289063) 359461530       32 2024-03-22 14:05:39.000000 abtoolkit-1.2.3/.gitignore
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1062 2024-03-22 09:28:06.000000 abtoolkit-1.2.3/LICENSE
+-rw-r--r--   0 naltukhov (1397289063) 359461530      558 2024-03-23 09:48:31.000000 abtoolkit-1.2.3/Makefile
+-rw-r--r--   0 naltukhov (1397289063) 359461530     6026 2024-04-19 07:53:44.107589 abtoolkit-1.2.3/PKG-INFO
+-rw-r--r--   0 naltukhov (1397289063) 359461530     5296 2024-04-19 07:52:57.000000 abtoolkit-1.2.3/README.md
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:53:44.096016 abtoolkit-1.2.3/abtoolkit/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-23 05:39:11.000000 abtoolkit-1.2.3/abtoolkit/__init__.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:53:44.097203 abtoolkit-1.2.3/abtoolkit/continuous/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 09:33:10.000000 abtoolkit-1.2.3/abtoolkit/continuous/__init__.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     7637 2024-03-29 12:15:29.000000 abtoolkit-1.2.3/abtoolkit/continuous/simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530    10878 2024-03-29 13:46:05.000000 abtoolkit-1.2.3/abtoolkit/continuous/stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     3381 2024-03-29 11:44:42.000000 abtoolkit-1.2.3/abtoolkit/continuous/utils.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:53:44.097900 abtoolkit-1.2.3/abtoolkit/discrete/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 09:32:58.000000 abtoolkit-1.2.3/abtoolkit/discrete/__init__.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     2396 2024-03-29 12:15:29.000000 abtoolkit-1.2.3/abtoolkit/discrete/simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1609 2024-03-29 11:46:38.000000 abtoolkit-1.2.3/abtoolkit/discrete/stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1801 2024-03-29 12:07:16.000000 abtoolkit-1.2.3/abtoolkit/discrete/utils.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     6152 2024-03-29 11:56:12.000000 abtoolkit-1.2.3/abtoolkit/utils.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:53:44.107267 abtoolkit-1.2.3/abtoolkit.egg-info/
+-rw-r--r--   0 naltukhov (1397289063) 359461530     6026 2024-04-19 07:53:44.000000 abtoolkit-1.2.3/abtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1248 2024-04-19 07:53:44.000000 abtoolkit-1.2.3/abtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530        1 2024-04-19 07:53:44.000000 abtoolkit-1.2.3/abtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530       93 2024-04-19 07:53:44.000000 abtoolkit-1.2.3/abtoolkit.egg-info/requires.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530       42 2024-04-19 07:53:44.000000 abtoolkit-1.2.3/abtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:53:44.098365 abtoolkit-1.2.3/examples/
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1844 2024-03-29 14:11:25.000000 abtoolkit-1.2.3/examples/continuous_var_analysis.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1479 2024-03-29 11:34:01.000000 abtoolkit-1.2.3/examples/discrete_var_analysis.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      260 2024-03-23 09:42:57.000000 abtoolkit-1.2.3/pre-commit.bash
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1021 2024-04-19 07:53:14.000000 abtoolkit-1.2.3/pyproject.toml
+-rw-r--r--   0 naltukhov (1397289063) 359461530      110 2024-03-22 14:16:03.000000 abtoolkit-1.2.3/requirements.txt
+-rw-r--r--   0 naltukhov (1397289063) 359461530       38 2024-04-19 07:53:44.107867 abtoolkit-1.2.3/setup.cfg
+-rw-r--r--   0 naltukhov (1397289063) 359461530      256 2024-04-19 07:41:47.000000 abtoolkit-1.2.3/setup.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:53:44.100774 abtoolkit-1.2.3/static/
+-rw-r--r--   0 naltukhov (1397289063) 359461530    41812 2024-03-29 12:49:51.000000 abtoolkit-1.2.3/static/discrete-output-plot.png
+-rw-r--r--   0 naltukhov (1397289063) 359461530   135844 2024-03-29 12:50:41.000000 abtoolkit-1.2.3/static/discrete-p-value-plot.png
+-rw-r--r--   0 naltukhov (1397289063) 359461530   185112 2024-03-29 12:52:31.000000 abtoolkit-1.2.3/static/output-plot.png
+-rw-r--r--   0 naltukhov (1397289063) 359461530   205019 2024-03-22 08:45:06.000000 abtoolkit-1.2.3/static/p-value-plot.png
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:53:44.103367 abtoolkit-1.2.3/tests/
+-rw-r--r--   0 naltukhov (1397289063) 359461530        0 2024-03-22 08:45:06.000000 abtoolkit-1.2.3/tests/__init__.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     2727 2024-03-29 08:48:35.000000 abtoolkit-1.2.3/tests/test_continuous_simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     5436 2024-03-29 08:48:35.000000 abtoolkit-1.2.3/tests/test_continuous_stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530      795 2024-03-25 10:43:06.000000 abtoolkit-1.2.3/tests/test_continuous_utils.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530     2426 2024-03-29 10:20:21.000000 abtoolkit-1.2.3/tests/test_discrete_simulation.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530      583 2024-03-29 09:29:26.000000 abtoolkit-1.2.3/tests/test_discrete_stattests.py
+-rw-r--r--   0 naltukhov (1397289063) 359461530      865 2024-03-29 10:35:15.000000 abtoolkit-1.2.3/tests/test_discrete_utils.py
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:53:44.094440 abtoolkit-1.2.3/venv/
+drwxr-xr-x   0 naltukhov (1397289063) 359461530        0 2024-04-19 07:53:44.106949 abtoolkit-1.2.3/venv/bin/
+-rw-r--r--   0 naltukhov (1397289063) 359461530     1175 2024-03-22 08:53:42.000000 abtoolkit-1.2.3/venv/bin/activate_this.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      648 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2html.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      770 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2html4.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530     1105 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2html5.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      847 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2latex.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      670 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2man.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      836 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2odt.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      642 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      655 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      691 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2s5.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      927 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      656 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rst2xml.py
+-rwxr-xr-x   0 naltukhov (1397289063) 359461530      724 2024-03-22 14:05:07.000000 abtoolkit-1.2.3/venv/bin/rstpep2html.py
```

### Comparing `abtoolkit-1.2.2/LICENSE` & `abtoolkit-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/Makefile` & `abtoolkit-1.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/PKG-INFO` & `abtoolkit-1.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abtoolkit
-Version: 1.2.2
+Version: 1.2.3
 Summary: Package with tools for AB testing
 Author-email: Nikita Altukhov <altuxov.nikita@gmail.com>
 Project-URL: Homepage, https://github.com/nikitosl/abtoolkit
 Project-URL: Issues, https://github.com/nikitosl/abtoolkit/issues
 Keywords: ab_test,cuped,did,ttest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -65,16 +65,16 @@
         additional_vars=[previous_value],
     )
 simulation.run()  # Run simulation
 simulation.print_results()  # Print results of simulation
 simulation.plot_p_values()  # Plot p-values distribution
 ```
 Output:
-![output-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Foutput-plot.png)
-![p-value-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Fp-value-plot.png)
+![output-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Foutput-plot.png)
+![p-value-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Fp-value-plot.png)
 
 Full example of usage you can find in ```examples/continuous_var_analysis.py``` script.
 
 #### Next stat tests implemented for treatment effect estimation:
 - ***T-Test*** - estimates treatment effect by comparing variables between test and control groups.
 - ***Difference T-Test*** - estimates treatment effect by comparing difference between actual and previous values 
 of variables in test and control groups.
@@ -123,15 +123,15 @@
         alpha_level=alpha_level,  # Fix alpha level on 5%
     )
     info = sim.run()  # Get dictionary with information about tests
     sim.print_results()  # Print results of simulation
     sim.plot_p_values()  # Plot p-values distribution
 ```
 Output:
-![discrete-output-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Fdiscrete-output-plot.png)
-![discrete-p-value-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Fdiscrete-p-value-plot.png)
+![discrete-output-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Fdiscrete-output-plot.png)
+![discrete-p-value-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Fdiscrete-p-value-plot.png)
 
 #### Next stat tests implemented for treatment effect estimation:
 - ***Conversion Z-Test*** estimates treatment effect on conversion variable using z-test
 
 ---
 You can find examples of toolkit usage in [examples/](https://github.com/nikitosl/abtoolkit/tree/master/examples) directory.
```

### Comparing `abtoolkit-1.2.2/README.md` & `abtoolkit-1.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         additional_vars=[previous_value],
     )
 simulation.run()  # Run simulation
 simulation.print_results()  # Print results of simulation
 simulation.plot_p_values()  # Plot p-values distribution
 ```
 Output:
-![output-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Foutput-plot.png)
-![p-value-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Fp-value-plot.png)
+![output-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Foutput-plot.png)
+![p-value-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Fp-value-plot.png)
 
 Full example of usage you can find in ```examples/continuous_var_analysis.py``` script.
 
 #### Next stat tests implemented for treatment effect estimation:
 - ***T-Test*** - estimates treatment effect by comparing variables between test and control groups.
 - ***Difference T-Test*** - estimates treatment effect by comparing difference between actual and previous values 
 of variables in test and control groups.
@@ -102,15 +102,15 @@
         alpha_level=alpha_level,  # Fix alpha level on 5%
     )
     info = sim.run()  # Get dictionary with information about tests
     sim.print_results()  # Print results of simulation
     sim.plot_p_values()  # Plot p-values distribution
 ```
 Output:
-![discrete-output-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Fdiscrete-output-plot.png)
-![discrete-p-value-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Fdiscrete-p-value-plot.png)
+![discrete-output-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Fdiscrete-output-plot.png)
+![discrete-p-value-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Fdiscrete-p-value-plot.png)
 
 #### Next stat tests implemented for treatment effect estimation:
 - ***Conversion Z-Test*** estimates treatment effect on conversion variable using z-test
 
 ---
 You can find examples of toolkit usage in [examples/](https://github.com/nikitosl/abtoolkit/tree/master/examples) directory.
```

### Comparing `abtoolkit-1.2.2/abtoolkit/continuous/simulation.py` & `abtoolkit-1.2.3/abtoolkit/continuous/simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/abtoolkit/continuous/stattests.py` & `abtoolkit-1.2.3/abtoolkit/continuous/stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/abtoolkit/continuous/utils.py` & `abtoolkit-1.2.3/abtoolkit/continuous/utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/abtoolkit/discrete/simulation.py` & `abtoolkit-1.2.3/abtoolkit/discrete/simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/abtoolkit/discrete/stattests.py` & `abtoolkit-1.2.3/abtoolkit/discrete/stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/abtoolkit/discrete/utils.py` & `abtoolkit-1.2.3/abtoolkit/discrete/utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/abtoolkit/utils.py` & `abtoolkit-1.2.3/abtoolkit/utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/abtoolkit.egg-info/PKG-INFO` & `abtoolkit-1.2.3/abtoolkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abtoolkit
-Version: 1.2.2
+Version: 1.2.3
 Summary: Package with tools for AB testing
 Author-email: Nikita Altukhov <altuxov.nikita@gmail.com>
 Project-URL: Homepage, https://github.com/nikitosl/abtoolkit
 Project-URL: Issues, https://github.com/nikitosl/abtoolkit/issues
 Keywords: ab_test,cuped,did,ttest
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -65,16 +65,16 @@
         additional_vars=[previous_value],
     )
 simulation.run()  # Run simulation
 simulation.print_results()  # Print results of simulation
 simulation.plot_p_values()  # Plot p-values distribution
 ```
 Output:
-![output-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Foutput-plot.png)
-![p-value-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Fp-value-plot.png)
+![output-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Foutput-plot.png)
+![p-value-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Fp-value-plot.png)
 
 Full example of usage you can find in ```examples/continuous_var_analysis.py``` script.
 
 #### Next stat tests implemented for treatment effect estimation:
 - ***T-Test*** - estimates treatment effect by comparing variables between test and control groups.
 - ***Difference T-Test*** - estimates treatment effect by comparing difference between actual and previous values 
 of variables in test and control groups.
@@ -123,15 +123,15 @@
         alpha_level=alpha_level,  # Fix alpha level on 5%
     )
     info = sim.run()  # Get dictionary with information about tests
     sim.print_results()  # Print results of simulation
     sim.plot_p_values()  # Plot p-values distribution
 ```
 Output:
-![discrete-output-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Fdiscrete-output-plot.png)
-![discrete-p-value-plot.png](https://github.com/nikitosl/abtoolkit/blob/master/static%2Fdiscrete-p-value-plot.png)
+![discrete-output-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Fdiscrete-output-plot.png)
+![discrete-p-value-plot.png](https://raw.githubusercontent.com/nikitosl/abtoolkit/master/static%2Fdiscrete-p-value-plot.png)
 
 #### Next stat tests implemented for treatment effect estimation:
 - ***Conversion Z-Test*** estimates treatment effect on conversion variable using z-test
 
 ---
 You can find examples of toolkit usage in [examples/](https://github.com/nikitosl/abtoolkit/tree/master/examples) directory.
```

### Comparing `abtoolkit-1.2.2/abtoolkit.egg-info/SOURCES.txt` & `abtoolkit-1.2.3/abtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/examples/continuous_var_analysis.py` & `abtoolkit-1.2.3/examples/continuous_var_analysis.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/examples/discrete_var_analysis.py` & `abtoolkit-1.2.3/examples/discrete_var_analysis.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/pyproject.toml` & `abtoolkit-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "abtoolkit"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Nikita Altukhov", email="altuxov.nikita@gmail.com" },
 ]
 description = "Package with tools for AB testing"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `abtoolkit-1.2.2/static/discrete-output-plot.png` & `abtoolkit-1.2.3/static/discrete-output-plot.png`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/static/discrete-p-value-plot.png` & `abtoolkit-1.2.3/static/discrete-p-value-plot.png`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/static/output-plot.png` & `abtoolkit-1.2.3/static/output-plot.png`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/static/p-value-plot.png` & `abtoolkit-1.2.3/static/p-value-plot.png`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/tests/test_continuous_simulation.py` & `abtoolkit-1.2.3/tests/test_continuous_simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/tests/test_continuous_stattests.py` & `abtoolkit-1.2.3/tests/test_continuous_stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/tests/test_continuous_utils.py` & `abtoolkit-1.2.3/tests/test_continuous_utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/tests/test_discrete_simulation.py` & `abtoolkit-1.2.3/tests/test_discrete_simulation.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/tests/test_discrete_stattests.py` & `abtoolkit-1.2.3/tests/test_discrete_stattests.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/tests/test_discrete_utils.py` & `abtoolkit-1.2.3/tests/test_discrete_utils.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/activate_this.py` & `abtoolkit-1.2.3/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2html.py` & `abtoolkit-1.2.3/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2html4.py` & `abtoolkit-1.2.3/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2html5.py` & `abtoolkit-1.2.3/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2latex.py` & `abtoolkit-1.2.3/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2man.py` & `abtoolkit-1.2.3/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2odt.py` & `abtoolkit-1.2.3/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2odt_prepstyles.py` & `abtoolkit-1.2.3/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2pseudoxml.py` & `abtoolkit-1.2.3/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2s5.py` & `abtoolkit-1.2.3/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2xetex.py` & `abtoolkit-1.2.3/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rst2xml.py` & `abtoolkit-1.2.3/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `abtoolkit-1.2.2/venv/bin/rstpep2html.py` & `abtoolkit-1.2.3/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

