# Comparing `tmp/CMDHelpMeTool-0.2.7.tar.gz` & `tmp/CMDHelpMeTool-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMDHelpMeTool-0.2.7.tar", last modified: Fri Apr 19 08:11:21 2024, max compression
+gzip compressed data, was "CMDHelpMeTool-0.3.1.tar", last modified: Fri Apr 19 08:37:27 2024, max compression
```

## Comparing `CMDHelpMeTool-0.2.7.tar` & `CMDHelpMeTool-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:11:21.674352 CMDHelpMeTool-0.2.7/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:11:21.570123 CMDHelpMeTool-0.2.7/CMDHelpMeTool/
--rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool/__init__.py
--rw-rw-rw-   0        0        0     2360 2024-04-19 08:11:10.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool/cmd_tool.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:11:21.669351 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/
--rw-rw-rw-   0        0        0      322 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.2.7/LICENSE
--rw-rw-rw-   0        0        0      322 2024-04-19 08:11:21.670353 CMDHelpMeTool-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-19 08:11:21.674352 CMDHelpMeTool-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-04-19 08:11:18.000000 CMDHelpMeTool-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:37:27.126608 CMDHelpMeTool-0.3.1/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:37:27.083943 CMDHelpMeTool-0.3.1/CMDHelpMeTool/
+-rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool/__init__.py
+-rw-rw-rw-   0        0        0      931 2024-04-19 08:20:10.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool/cmd_tool.py
+-rw-rw-rw-   0        0        0    31374 2024-04-19 08:37:12.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool/experiments.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:37:27.124606 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-04-19 08:37:26.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-04-19 08:37:27.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:37:26.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 08:37:26.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 08:37:26.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 08:37:26.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      322 2024-04-19 08:37:27.125605 CMDHelpMeTool-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:37:27.126608 CMDHelpMeTool-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      532 2024-04-19 08:37:23.000000 CMDHelpMeTool-0.3.1/setup.py
```

### Comparing `CMDHelpMeTool-0.2.7/LICENSE` & `CMDHelpMeTool-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.2.7/setup.py` & `CMDHelpMeTool-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CMDHelpMeTool',
-    version='0.2.7',
+    version='0.3.1',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'helpme = CMDHelpMeTool.cmd_tool:main'
         ]
     },
     install_requires=[
```

