# Comparing `tmp/CMDHelpMeTool-0.3.1.tar.gz` & `tmp/CMDHelpMeTool-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMDHelpMeTool-0.3.1.tar", last modified: Fri Apr 19 08:37:27 2024, max compression
+gzip compressed data, was "CMDHelpMeTool-0.3.2.tar", last modified: Fri Apr 19 08:43:46 2024, max compression
```

## Comparing `CMDHelpMeTool-0.3.1.tar` & `CMDHelpMeTool-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:37:27.126608 CMDHelpMeTool-0.3.1/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:37:27.083943 CMDHelpMeTool-0.3.1/CMDHelpMeTool/
--rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool/__init__.py
--rw-rw-rw-   0        0        0      931 2024-04-19 08:20:10.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool/cmd_tool.py
--rw-rw-rw-   0        0        0    31374 2024-04-19 08:37:12.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool/experiments.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:37:27.124606 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/
--rw-rw-rw-   0        0        0      322 2024-04-19 08:37:26.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2024-04-19 08:37:27.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:37:26.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-19 08:37:26.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 08:37:26.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 08:37:26.000000 CMDHelpMeTool-0.3.1/CMDHelpMeTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      322 2024-04-19 08:37:27.125605 CMDHelpMeTool-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-19 08:37:27.126608 CMDHelpMeTool-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-04-19 08:37:23.000000 CMDHelpMeTool-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:43:46.855012 CMDHelpMeTool-0.3.2/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:43:46.819982 CMDHelpMeTool-0.3.2/CMDHelpMeTool/
+-rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool/__init__.py
+-rw-rw-rw-   0        0        0      877 2024-04-19 08:43:34.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool/cmd_tool.py
+-rw-rw-rw-   0        0        0    31374 2024-04-19 08:37:12.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool/experiments.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:43:46.853012 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 08:43:46.000000 CMDHelpMeTool-0.3.2/CMDHelpMeTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0      322 2024-04-19 08:43:46.855012 CMDHelpMeTool-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:43:46.856013 CMDHelpMeTool-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      532 2024-04-19 08:43:43.000000 CMDHelpMeTool-0.3.2/setup.py
```

### Comparing `CMDHelpMeTool-0.3.1/CMDHelpMeTool/cmd_tool.py` & `CMDHelpMeTool-0.3.2/CMDHelpMeTool/cmd_tool.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import argparse
 import pyperclip
-import experiments  # Import the experiments module
+from .experiments import *  # Import all variables from experiments.py
 
-def copy_variable_to_clipboard(variable_name):
-    # Get the variable value based on the variable name
-    variable = getattr(experiments, variable_name, None)
-    if variable is not None:
-        pyperclip.copy(variable)
-        print(f"Content of '{variable_name}' copied to clipboard.")
-    else:
-        print(f"Variable '{variable_name}' not found.")
+def copy_variable_to_clipboard(variable):
+    pyperclip.copy(variable)
+    print(f"Content copied to clipboard: {variable}")
 
 def main():
     parser = argparse.ArgumentParser(description='Command-line tool for copying variable content to clipboard.')
     parser.add_argument('command', choices=['copy_experiment'], help='Command to execute')
     parser.add_argument('variable_name', help='Name of the variable to copy')
 
     args = parser.parse_args()
 
     if args.command == 'copy_experiment':
-        copy_variable_to_clipboard(args.variable_name)
+        variable = globals().get(args.variable_name)
+        if variable is not None:
+            copy_variable_to_clipboard(variable)
+        else:
+            print(f"Variable '{args.variable_name}' not found.")
 
 if __name__ == "__main__":
     main()
```

### Comparing `CMDHelpMeTool-0.3.1/CMDHelpMeTool/experiments.py` & `CMDHelpMeTool-0.3.2/CMDHelpMeTool/experiments.py`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.3.1/LICENSE` & `CMDHelpMeTool-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.3.1/setup.py` & `CMDHelpMeTool-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CMDHelpMeTool',
-    version='0.3.1',
+    version='0.3.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'helpme = CMDHelpMeTool.cmd_tool:main'
         ]
     },
     install_requires=[
```

