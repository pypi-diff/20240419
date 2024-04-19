# Comparing `tmp/CMDHelpMeTool-0.3.2.tar.gz` & `tmp/CMDHelpMeTool-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMDHelpMeTool-0.3.2.tar", last modified: Fri Apr 19 08:43:46 2024, max compression
+gzip compressed data, was "CMDHelpMeTool-0.3.3.tar", last modified: Fri Apr 19 09:06:00 2024, max compression
```

## Comparing `CMDHelpMeTool-0.3.2.tar` & `CMDHelpMeTool-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:43:46.855012 CMDHelpMeTool-0.3.2/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:43:46.819982 CMDHelpMeTool-0.3.2/CMDHelpMeTool/
--rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool/__init__.py
--rw-rw-rw-   0        0        0      877 2024-04-19 08:43:34.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool/cmd_tool.py
--rw-rw-rw-   0        0        0    31374 2024-04-19 08:37:12.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool/experiments.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:43:46.853012 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/
--rw-rw-rw-   0        0        0      322 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.3.2/LICENSE
--rw-rw-rw-   0        0        0      322 2024-04-19 08:43:46.855012 CMDHelpMeTool-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-19 08:43:46.856013 CMDHelpMeTool-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-04-19 08:43:43.000000 CMDHelpMeTool-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:06:00.190578 CMDHelpMeTool-0.3.3/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:06:00.153530 CMDHelpMeTool-0.3.3/CMDHelpMeTool/
+-rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.3.3/CMDHelpMeTool/__init__.py
+-rw-rw-rw-   0        0        0      870 2024-04-19 08:48:03.000000 CMDHelpMeTool-0.3.3/CMDHelpMeTool/cmd_tool.py
+-rw-rw-rw-   0        0        0    31374 2024-04-19 08:37:12.000000 CMDHelpMeTool-0.3.3/CMDHelpMeTool/experiments.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:06:00.188578 CMDHelpMeTool-0.3.3/CMDHelpMeTool.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-04-19 09:06:00.000000 CMDHelpMeTool-0.3.3/CMDHelpMeTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-04-19 09:06:00.000000 CMDHelpMeTool-0.3.3/CMDHelpMeTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:06:00.000000 CMDHelpMeTool-0.3.3/CMDHelpMeTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 09:06:00.000000 CMDHelpMeTool-0.3.3/CMDHelpMeTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 09:06:00.000000 CMDHelpMeTool-0.3.3/CMDHelpMeTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 09:06:00.000000 CMDHelpMeTool-0.3.3/CMDHelpMeTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0      322 2024-04-19 09:06:00.189578 CMDHelpMeTool-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:06:00.193577 CMDHelpMeTool-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      532 2024-04-19 09:05:52.000000 CMDHelpMeTool-0.3.3/setup.py
```

### Comparing `CMDHelpMeTool-0.3.2/CMDHelpMeTool/cmd_tool.py` & `CMDHelpMeTool-0.3.3/CMDHelpMeTool/cmd_tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import pyperclip
 from .experiments import *  # Import all variables from experiments.py
 
 def copy_variable_to_clipboard(variable):
     pyperclip.copy(variable)
-    print(f"Content copied to clipboard: {variable}")
+    print("File content copied to clipboard.")
 
 def main():
     parser = argparse.ArgumentParser(description='Command-line tool for copying variable content to clipboard.')
     parser.add_argument('command', choices=['copy_experiment'], help='Command to execute')
     parser.add_argument('variable_name', help='Name of the variable to copy')
 
     args = parser.parse_args()
```

### Comparing `CMDHelpMeTool-0.3.2/CMDHelpMeTool/experiments.py` & `CMDHelpMeTool-0.3.3/CMDHelpMeTool/experiments.py`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.3.2/LICENSE` & `CMDHelpMeTool-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.3.2/setup.py` & `CMDHelpMeTool-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CMDHelpMeTool',
-    version='0.3.2',
+    version='0.3.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'helpme = CMDHelpMeTool.cmd_tool:main'
         ]
     },
     install_requires=[
```

