# Comparing `tmp/CMDHelpMeTool-0.2.6.tar.gz` & `tmp/CMDHelpMeTool-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMDHelpMeTool-0.2.6.tar", last modified: Fri Apr 19 08:06:13 2024, max compression
+gzip compressed data, was "CMDHelpMeTool-0.2.7.tar", last modified: Fri Apr 19 08:11:21 2024, max compression
```

## Comparing `CMDHelpMeTool-0.2.6.tar` & `CMDHelpMeTool-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:06:13.287505 CMDHelpMeTool-0.2.6/
-drwxrwxrwx   0        0        0        0 2024-04-19 08:06:13.256290 CMDHelpMeTool-0.2.6/CMDHelpMeTool/
--rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.2.6/CMDHelpMeTool/__init__.py
--rw-rw-rw-   0        0        0     2046 2024-04-19 08:06:04.000000 CMDHelpMeTool-0.2.6/CMDHelpMeTool/cmd_tool.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:06:13.283488 CMDHelpMeTool-0.2.6/CMDHelpMeTool.egg-info/
--rw-rw-rw-   0        0        0      322 2024-04-19 08:06:13.000000 CMDHelpMeTool-0.2.6/CMDHelpMeTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-19 08:06:13.000000 CMDHelpMeTool-0.2.6/CMDHelpMeTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:06:13.000000 CMDHelpMeTool-0.2.6/CMDHelpMeTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-19 08:06:13.000000 CMDHelpMeTool-0.2.6/CMDHelpMeTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 08:06:13.000000 CMDHelpMeTool-0.2.6/CMDHelpMeTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 08:06:13.000000 CMDHelpMeTool-0.2.6/CMDHelpMeTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      322 2024-04-19 08:06:13.284487 CMDHelpMeTool-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-19 08:06:13.287505 CMDHelpMeTool-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-04-19 08:06:10.000000 CMDHelpMeTool-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:11:21.674352 CMDHelpMeTool-0.2.7/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:11:21.570123 CMDHelpMeTool-0.2.7/CMDHelpMeTool/
+-rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool/__init__.py
+-rw-rw-rw-   0        0        0     2360 2024-04-19 08:11:10.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool/cmd_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:11:21.669351 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 08:11:21.000000 CMDHelpMeTool-0.2.7/CMDHelpMeTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      322 2024-04-19 08:11:21.670353 CMDHelpMeTool-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:11:21.674352 CMDHelpMeTool-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      532 2024-04-19 08:11:18.000000 CMDHelpMeTool-0.2.7/setup.py
```

### Comparing `CMDHelpMeTool-0.2.6/CMDHelpMeTool/cmd_tool.py` & `CMDHelpMeTool-0.2.7/CMDHelpMeTool/cmd_tool.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
-import os
 import pyperclip
 
+exp1 = "If you can't upload your project's release to PyPI because you're hitting the upload file size limit, we can sometimes increase your limit. Make sure you've uploaded at least one release for the project that's under the limit (a developmental release version number is fine). Then, file an issue and tell us:\n\nA link to your project on PyPI (or Test PyPI)\nThe size of your release, in megabytes\nWhich index/indexes you need the increase for (PyPI, Test PyPI, or both)\nA brief description of your project, including the reason for the additional size."
+
 def create_file(filename):
     with open(filename, 'w') as file:
         file.write('Sample text in ' + filename)
 
 def read_file(filename):
     try:
         with open(filename, 'r') as file:
@@ -15,46 +16,41 @@
 
 def list_files():
     files = os.listdir('.')
     return '\n'.join(files)
 
 def copy_to_clipboard(text):
     pyperclip.copy(text)
-    print("Content copied to clipboard.")
 
-def copy_folder_content(folder_path):
-    for filename in os.listdir(folder_path):
-        file_path = os.path.join(folder_path, filename)
-        if os.path.isfile(file_path):
-            with open(file_path, 'r') as file:
-                content = file.read()
-                pyperclip.copy(content)
-                print(f"Content of {filename} copied to clipboard.")
+def copy_variable_to_clipboard(variable):
+    pyperclip.copy(variable)
+    print("Variable content copied to clipboard.")
 
 def main():
     parser = argparse.ArgumentParser(description='Command-line tool for file management and copying to clipboard.')
-    parser.add_argument('command', choices=['create', 'read', 'copy', 'ls', 'copy_folder', 'new_command'], help='Command to execute')
+    parser.add_argument('command', choices=['create', 'read', 'copy', 'ls', 'copy_variable', 'new_command'], help='Command to execute')
     parser.add_argument('filename', nargs='?', help='File name')
 
     args = parser.parse_args()
 
     if args.command == 'create':
         create_file(args.filename)
         print(f"File '{args.filename}' created successfully.")
     elif args.command == 'read':
         content = read_file(args.filename)
         print(content)
     elif args.command == 'copy':
         content = read_file(args.filename)
         copy_to_clipboard(content)
+        print("File content copied to clipboard.")
     elif args.command == 'ls':
         files_list = list_files()
         print("Files in current directory:")
         print(files_list)
-    elif args.command == 'copy_folder':
-        copy_folder_content(args.filename)
+    elif args.command == 'copy_variable':
+        copy_variable_to_clipboard(exp1)
     elif args.command == 'new_command':
         # Implement functionality for your new command here
         print("New command executed.")
 
 if __name__ == "__main__":
     main()
```

### Comparing `CMDHelpMeTool-0.2.6/LICENSE` & `CMDHelpMeTool-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.2.6/setup.py` & `CMDHelpMeTool-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CMDHelpMeTool',
-    version='0.2.6',
+    version='0.2.7',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'helpme = CMDHelpMeTool.cmd_tool:main'
         ]
     },
     install_requires=[
```

