# Comparing `tmp/CMDHelpMeTool-0.3.4.tar.gz` & `tmp/CMDHelpMeTool-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMDHelpMeTool-0.3.4.tar", last modified: Fri Apr 19 09:13:24 2024, max compression
+gzip compressed data, was "CMDHelpMeTool-0.3.5.tar", last modified: Fri Apr 19 09:17:41 2024, max compression
```

## Comparing `CMDHelpMeTool-0.3.4.tar` & `CMDHelpMeTool-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 09:13:24.593345 CMDHelpMeTool-0.3.4/
-drwxrwxrwx   0        0        0        0 2024-04-19 09:13:24.547307 CMDHelpMeTool-0.3.4/CMDHelpMeTool/
--rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.3.4/CMDHelpMeTool/__init__.py
--rw-rw-rw-   0        0        0      870 2024-04-19 08:48:03.000000 CMDHelpMeTool-0.3.4/CMDHelpMeTool/cmd_tool.py
--rw-rw-rw-   0        0        0    31374 2024-04-19 08:37:12.000000 CMDHelpMeTool-0.3.4/CMDHelpMeTool/experiments.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:13:24.588182 CMDHelpMeTool-0.3.4/CMDHelpMeTool.egg-info/
--rw-rw-rw-   0        0        0      322 2024-04-19 09:13:24.000000 CMDHelpMeTool-0.3.4/CMDHelpMeTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-19 09:13:24.000000 CMDHelpMeTool-0.3.4/CMDHelpMeTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 09:13:24.000000 CMDHelpMeTool-0.3.4/CMDHelpMeTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-19 09:13:24.000000 CMDHelpMeTool-0.3.4/CMDHelpMeTool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 09:13:24.000000 CMDHelpMeTool-0.3.4/CMDHelpMeTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 09:13:24.000000 CMDHelpMeTool-0.3.4/CMDHelpMeTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.3.4/LICENSE
--rw-rw-rw-   0        0        0      322 2024-04-19 09:13:24.591182 CMDHelpMeTool-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      528 2024-04-19 09:04:10.000000 CMDHelpMeTool-0.3.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 09:13:24.593345 CMDHelpMeTool-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-04-19 09:13:21.000000 CMDHelpMeTool-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:41.293981 CMDHelpMeTool-0.3.5/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:41.257838 CMDHelpMeTool-0.3.5/CMDHelpMeTool/
+-rw-rw-rw-   0        0        0       26 2024-04-19 07:12:47.000000 CMDHelpMeTool-0.3.5/CMDHelpMeTool/__init__.py
+-rw-rw-rw-   0        0        0      870 2024-04-19 08:48:03.000000 CMDHelpMeTool-0.3.5/CMDHelpMeTool/cmd_tool.py
+-rw-rw-rw-   0        0        0    31374 2024-04-19 08:37:12.000000 CMDHelpMeTool-0.3.5/CMDHelpMeTool/experiments.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:17:41.286930 CMDHelpMeTool-0.3.5/CMDHelpMeTool.egg-info/
+-rw-rw-rw-   0        0        0      884 2024-04-19 09:17:41.000000 CMDHelpMeTool-0.3.5/CMDHelpMeTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-19 09:17:41.000000 CMDHelpMeTool-0.3.5/CMDHelpMeTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:17:41.000000 CMDHelpMeTool-0.3.5/CMDHelpMeTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 09:17:41.000000 CMDHelpMeTool-0.3.5/CMDHelpMeTool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 09:17:41.000000 CMDHelpMeTool-0.3.5/CMDHelpMeTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 09:17:41.000000 CMDHelpMeTool-0.3.5/CMDHelpMeTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1073 2024-04-19 06:07:39.000000 CMDHelpMeTool-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0      884 2024-04-19 09:17:41.289939 CMDHelpMeTool-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2024-04-19 09:04:10.000000 CMDHelpMeTool-0.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:17:41.293981 CMDHelpMeTool-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-04-19 09:17:38.000000 CMDHelpMeTool-0.3.5/setup.py
```

### Comparing `CMDHelpMeTool-0.3.4/CMDHelpMeTool/cmd_tool.py` & `CMDHelpMeTool-0.3.5/CMDHelpMeTool/cmd_tool.py`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.3.4/CMDHelpMeTool/experiments.py` & `CMDHelpMeTool-0.3.5/CMDHelpMeTool/experiments.py`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.3.4/LICENSE` & `CMDHelpMeTool-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.3.4/README.md` & `CMDHelpMeTool-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `CMDHelpMeTool-0.3.4/setup.py` & `CMDHelpMeTool-0.3.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name='CMDHelpMeTool',
-    version='0.3.4',
+    version='0.3.5',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'helpme = CMDHelpMeTool.cmd_tool:main'
         ]
     },
     install_requires=[
         'pyperclip'
     ],
     author='Abhi-vish',
     author_email='iamabhishekvishwakarma7@gmail.com',
     description='A command-line tool for file management and copying to clipboard.',
+    long_description=long_description,
+    long_description_content_type="text/markdown",  # Specify content type as Markdown
     license='MIT',
     keywords='command-line tool'
 )
```

