# Comparing `tmp/lusid_express-0.5.2.tar.gz` & `tmp/lusid_express-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-0.5.2.tar", last modified: Thu Apr 18 23:39:09 2024, max compression
+gzip compressed data, was "lusid_express-0.5.3.tar", last modified: Thu Apr 18 23:47:49 2024, max compression
```

## Comparing `lusid_express-0.5.2.tar` & `lusid_express-0.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.552502 lusid_express-0.5.2/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-18 23:39:06.000000 lusid_express-0.5.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-18 23:39:06.000000 lusid_express-0.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6548 2024-04-18 23:39:09.552502 lusid_express-0.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-18 23:39:06.000000 lusid_express-0.5.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 23:39:09.552502 lusid_express-0.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-18 23:39:06.000000 lusid_express-0.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.548502 lusid_express-0.5.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.550502 lusid_express-0.5.2/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2423 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.551502 lusid_express-0.5.2/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.551502 lusid_express-0.5.2/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.552502 lusid_express-0.5.2/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)     6589 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.551502 lusid_express-0.5.2/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6548 2024-04-18 23:39:09.000000 lusid_express-0.5.2/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-18 23:39:09.000000 lusid_express-0.5.2/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 23:39:09.000000 lusid_express-0.5.2/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-18 23:39:09.000000 lusid_express-0.5.2/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-18 23:39:09.000000 lusid_express-0.5.2/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:47:49.297144 lusid_express-0.5.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-18 23:47:46.000000 lusid_express-0.5.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-18 23:47:46.000000 lusid_express-0.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-18 23:47:49.297144 lusid_express-0.5.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-18 23:47:46.000000 lusid_express-0.5.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 23:47:49.297144 lusid_express-0.5.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-18 23:47:46.000000 lusid_express-0.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:47:49.293145 lusid_express-0.5.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:47:49.295144 lusid_express-0.5.3/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-18 23:47:46.000000 lusid_express-0.5.3/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2423 2024-04-18 23:47:46.000000 lusid_express-0.5.3/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:47:49.296144 lusid_express-0.5.3/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-18 23:47:46.000000 lusid_express-0.5.3/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:47:49.296144 lusid_express-0.5.3/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-18 23:47:46.000000 lusid_express-0.5.3/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:47:49.296144 lusid_express-0.5.3/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-18 23:47:46.000000 lusid_express-0.5.3/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)     6591 2024-04-18 23:47:46.000000 lusid_express-0.5.3/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-18 23:47:46.000000 lusid_express-0.5.3/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:47:49.296144 lusid_express-0.5.3/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-18 23:47:49.000000 lusid_express-0.5.3/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-18 23:47:49.000000 lusid_express-0.5.3/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 23:47:49.000000 lusid_express-0.5.3/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-18 23:47:49.000000 lusid_express-0.5.3/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-18 23:47:49.000000 lusid_express-0.5.3/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-0.5.2/LICENSE` & `lusid_express-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.2/PKG-INFO` & `lusid_express-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 0.5.2
+Version: 0.5.3
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-0.5.2/README.md` & `lusid_express-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.2/setup.py` & `lusid_express-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='0.5.2',
+    version='0.5.3',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-0.5.2/src/lusid_express/__main__.py` & `lusid_express-0.5.3/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.2/src/lusid_express/apis/__init__.py` & `lusid_express-0.5.3/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.2/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-0.5.3/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.2/src/lusid_express/display/__init__.py` & `lusid_express-0.5.3/src/lusid_express/display/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,23 @@
 <style>
 @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&display=swap');
 
 :root {
     --main-color: #00B6DA; /* Light theme color */
     --table-color: #065F82; /* Light theme table color */
     --accent-color: #FF5500; /* Light theme accent color */
-    --foreground-color: #121212; /* Light theme background */
+    --foreground-color: #777777; /* Light theme background */
 }
 
 @media (prefers-color-scheme: dark) {
     :root {
         --main-color: #0094AC; /* Dark theme color */
         --table-color: #043A4A; /* Dark theme table color */
         --accent-color: #E76F00; /* Dark theme accent color */
-        --foreground-color: white; /* Dark theme background */
+        --foreground-color: #777777; /* Dark theme background */
     }
 }
 
 body, h1, h2, h3, p {
     font-family: 'Montserrat';
 }
 table {
```

### Comparing `lusid_express-0.5.2/src/lusid_express/load.le` & `lusid_express-0.5.3/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.2/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-0.5.3/src/lusid_express.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 0.5.2
+Version: 0.5.3
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

