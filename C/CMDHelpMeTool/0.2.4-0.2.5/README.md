# Comparing `tmp/CMDHelpMeTool-0.2.4.tar.gz` & `tmp/CMDHelpMeTool-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMDHelpMeTool-0.2.4.tar", last modified: Fri Apr 19 07:39:17 2024, max compression
+gzip compressed data, was "CMDHelpMeTool-0.2.5.tar", last modified: Fri Apr 19 07:43:27 2024, max compression
```

## Comparing `CMDHelpMeTool-0.2.4.tar` & `CMDHelpMeTool-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:39:17.189376 CMDHelpMeTool-0.2.4/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:39:17.140610 CMDHelpMeTool-0.2.4/CMDHelpMeTool/
--rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.2.4/CMDHelpMeTool/__init__.py
--rw-rw-rw-   0        0        0     1574 2024-04-19 07:38:26.000000 CMDHelpMeTool-0.2.4/CMDHelpMeTool/cmd_tool.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:39:17.186115 CMDHelpMeTool-0.2.4/CMDHelpMeTool.egg-info/
--rw-rw-rw-   0        0        0      322 2024-04-19 07:39:17.000000 CMDHelpMeTool-0.2.4/CMDHelpMeTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-19 07:39:17.000000 CMDHelpMeTool-0.2.4/CMDHelpMeTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:39:17.000000 CMDHelpMeTool-0.2.4/CMDHelpMeTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-19 07:39:17.000000 CMDHelpMeTool-0.2.4/CMDHelpMeTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 07:39:17.000000 CMDHelpMeTool-0.2.4/CMDHelpMeTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 07:39:17.000000 CMDHelpMeTool-0.2.4/CMDHelpMeTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      322 2024-04-19 07:39:17.187364 CMDHelpMeTool-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-19 07:39:17.189376 CMDHelpMeTool-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-04-19 07:39:14.000000 CMDHelpMeTool-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:43:27.184138 CMDHelpMeTool-0.2.5/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:43:27.142394 CMDHelpMeTool-0.2.5/CMDHelpMeTool/
+-rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.2.5/CMDHelpMeTool/__init__.py
+-rw-rw-rw-   0        0        0     1574 2024-04-19 07:38:26.000000 CMDHelpMeTool-0.2.5/CMDHelpMeTool/cmd_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:43:27.179750 CMDHelpMeTool-0.2.5/CMDHelpMeTool.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-04-19 07:43:27.000000 CMDHelpMeTool-0.2.5/CMDHelpMeTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-19 07:43:27.000000 CMDHelpMeTool-0.2.5/CMDHelpMeTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:43:27.000000 CMDHelpMeTool-0.2.5/CMDHelpMeTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 07:43:27.000000 CMDHelpMeTool-0.2.5/CMDHelpMeTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 07:43:27.000000 CMDHelpMeTool-0.2.5/CMDHelpMeTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 07:43:27.000000 CMDHelpMeTool-0.2.5/CMDHelpMeTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      322 2024-04-19 07:43:27.183130 CMDHelpMeTool-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:43:27.185140 CMDHelpMeTool-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      532 2024-04-19 07:43:14.000000 CMDHelpMeTool-0.2.5/setup.py
```

### Comparing `CMDHelpMeTool-0.2.4/CMDHelpMeTool/cmd_tool.py` & `CMDHelpMeTool-0.2.5/CMDHelpMeTool/cmd_tool.py`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.2.4/LICENSE` & `CMDHelpMeTool-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.2.4/setup.py` & `CMDHelpMeTool-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CMDHelpMeTool',
-    version='0.2.4',
+    version='0.2.5',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'helpme = CMDHelpMeTool.cmd_tool:main'
         ]
     },
     install_requires=[
```

