# Comparing `tmp/CMDHelpMeTool-0.2.1.tar.gz` & `tmp/CMDHelpMeTool-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMDHelpMeTool-0.2.1.tar", last modified: Fri Apr 19 07:30:49 2024, max compression
+gzip compressed data, was "CMDHelpMeTool-0.2.2.tar", last modified: Fri Apr 19 07:31:56 2024, max compression
```

## Comparing `CMDHelpMeTool-0.2.1.tar` & `CMDHelpMeTool-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:30:49.541181 CMDHelpMeTool-0.2.1/
-drwxrwxrwx   0        0        0        0 2024-04-19 07:30:49.491238 CMDHelpMeTool-0.2.1/CMDHelpMeTool/
--rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.2.1/CMDHelpMeTool/__init__.py
--rw-rw-rw-   0        0        0     1721 2024-04-19 07:30:30.000000 CMDHelpMeTool-0.2.1/CMDHelpMeTool/cmd_tool.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:30:49.533105 CMDHelpMeTool-0.2.1/CMDHelpMeTool.egg-info/
--rw-rw-rw-   0        0        0      322 2024-04-19 07:30:49.000000 CMDHelpMeTool-0.2.1/CMDHelpMeTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-19 07:30:49.000000 CMDHelpMeTool-0.2.1/CMDHelpMeTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:30:49.000000 CMDHelpMeTool-0.2.1/CMDHelpMeTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-19 07:30:49.000000 CMDHelpMeTool-0.2.1/CMDHelpMeTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 07:30:49.000000 CMDHelpMeTool-0.2.1/CMDHelpMeTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 07:30:49.000000 CMDHelpMeTool-0.2.1/CMDHelpMeTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      322 2024-04-19 07:30:49.539169 CMDHelpMeTool-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-19 07:30:49.542181 CMDHelpMeTool-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-04-19 07:30:41.000000 CMDHelpMeTool-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:31:56.437588 CMDHelpMeTool-0.2.2/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:31:56.400189 CMDHelpMeTool-0.2.2/CMDHelpMeTool/
+-rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.2.2/CMDHelpMeTool/__init__.py
+-rw-rw-rw-   0        0        0     1721 2024-04-19 07:30:30.000000 CMDHelpMeTool-0.2.2/CMDHelpMeTool/cmd_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:31:56.434615 CMDHelpMeTool-0.2.2/CMDHelpMeTool.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-04-19 07:31:56.000000 CMDHelpMeTool-0.2.2/CMDHelpMeTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-19 07:31:56.000000 CMDHelpMeTool-0.2.2/CMDHelpMeTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:31:56.000000 CMDHelpMeTool-0.2.2/CMDHelpMeTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 07:31:56.000000 CMDHelpMeTool-0.2.2/CMDHelpMeTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 07:31:56.000000 CMDHelpMeTool-0.2.2/CMDHelpMeTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 07:31:56.000000 CMDHelpMeTool-0.2.2/CMDHelpMeTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      322 2024-04-19 07:31:56.437588 CMDHelpMeTool-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:31:56.438838 CMDHelpMeTool-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      532 2024-04-19 07:31:53.000000 CMDHelpMeTool-0.2.2/setup.py
```

### Comparing `CMDHelpMeTool-0.2.1/CMDHelpMeTool/cmd_tool.py` & `CMDHelpMeTool-0.2.2/CMDHelpMeTool/cmd_tool.py`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.2.1/LICENSE` & `CMDHelpMeTool-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.2.1/setup.py` & `CMDHelpMeTool-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CMDHelpMeTool',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'helpme = CMDHelpMeTool.cmd_tool:main'
         ]
     },
     install_requires=[
```

