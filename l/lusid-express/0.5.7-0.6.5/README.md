# Comparing `tmp/lusid_express-0.5.7.tar.gz` & `tmp/lusid_express-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-0.5.7.tar", last modified: Fri Apr 19 15:59:21 2024, max compression
+gzip compressed data, was "lusid_express-0.6.5.tar", last modified: Fri Apr 19 21:54:28 2024, max compression
```

## Comparing `lusid_express-0.5.7.tar` & `lusid_express-0.6.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:59:21.887602 lusid_express-0.5.7/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-19 15:59:19.000000 lusid_express-0.5.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-19 15:59:19.000000 lusid_express-0.5.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6548 2024-04-19 15:59:21.887602 lusid_express-0.5.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-19 15:59:19.000000 lusid_express-0.5.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 15:59:21.887602 lusid_express-0.5.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-19 15:59:19.000000 lusid_express-0.5.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:59:21.883602 lusid_express-0.5.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:59:21.885602 lusid_express-0.5.7/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-19 15:59:19.000000 lusid_express-0.5.7/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2418 2024-04-19 15:59:19.000000 lusid_express-0.5.7/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:59:21.886602 lusid_express-0.5.7/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-19 15:59:19.000000 lusid_express-0.5.7/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:59:21.886602 lusid_express-0.5.7/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-19 15:59:19.000000 lusid_express-0.5.7/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:59:21.886602 lusid_express-0.5.7/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-19 15:59:19.000000 lusid_express-0.5.7/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)     6591 2024-04-19 15:59:19.000000 lusid_express-0.5.7/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-19 15:59:19.000000 lusid_express-0.5.7/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:59:21.886602 lusid_express-0.5.7/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6548 2024-04-19 15:59:21.000000 lusid_express-0.5.7/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-19 15:59:21.000000 lusid_express-0.5.7/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 15:59:21.000000 lusid_express-0.5.7/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-19 15:59:21.000000 lusid_express-0.5.7/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-19 15:59:21.000000 lusid_express-0.5.7/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 21:54:28.041089 lusid_express-0.6.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-19 21:53:48.000000 lusid_express-0.6.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-19 21:53:48.000000 lusid_express-0.6.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-19 21:54:28.041089 lusid_express-0.6.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-19 21:53:48.000000 lusid_express-0.6.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 21:54:28.042089 lusid_express-0.6.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-19 21:53:48.000000 lusid_express-0.6.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 21:54:28.035089 lusid_express-0.6.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 21:54:28.037089 lusid_express-0.6.5/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-19 21:53:48.000000 lusid_express-0.6.5/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2024-04-19 21:53:48.000000 lusid_express-0.6.5/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 21:54:28.039089 lusid_express-0.6.5/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2219940 2024-04-19 21:54:27.000000 lusid_express-0.6.5/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 21:54:28.041089 lusid_express-0.6.5/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-19 21:53:48.000000 lusid_express-0.6.5/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 21:54:28.041089 lusid_express-0.6.5/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-19 21:53:48.000000 lusid_express-0.6.5/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)     6591 2024-04-19 21:53:48.000000 lusid_express-0.6.5/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-19 21:53:48.000000 lusid_express-0.6.5/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 21:54:28.038089 lusid_express-0.6.5/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-19 21:54:28.000000 lusid_express-0.6.5/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-19 21:54:28.000000 lusid_express-0.6.5/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 21:54:28.000000 lusid_express-0.6.5/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-19 21:54:28.000000 lusid_express-0.6.5/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-19 21:54:28.000000 lusid_express-0.6.5/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-0.5.7/LICENSE` & `lusid_express-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.7/PKG-INFO` & `lusid_express-0.6.5/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lusid_express
-Version: 0.5.7
+Name: lusid-express
+Version: 0.6.5
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-0.5.7/README.md` & `lusid_express-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.7/setup.py` & `lusid_express-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='0.5.7',
+    version='0.6.5',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-0.5.7/src/lusid_express/__main__.py` & `lusid_express-0.6.5/src/lusid_express/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,17 +56,15 @@
     target_file = os.path.join(ipython_startup_dir, '00-load_lusid_express.py')
     source_file = os.path.join(os.path.dirname(__file__), 'load.le')
 
     # Ensure the IPython startup directory exists
     os.makedirs(ipython_startup_dir, exist_ok=True)
 
     # Copy the load.py file if it does not already exist
-    if not os.path.exists(target_file):
-        shutil.copy(source_file, target_file)
-        print(f"File {source_file} copied to {target_file}")
+    shutil.copy(source_file, target_file)
         
         
         
         
 def main():
     args = parse_args()
     update_config(args)
```

### Comparing `lusid_express-0.5.7/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-0.6.5/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.7/src/lusid_express/display/__init__.py` & `lusid_express-0.6.5/src/lusid_express/display/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.7/src/lusid_express/load.le` & `lusid_express-0.6.5/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.7/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lusid-express
-Version: 0.5.7
+Name: lusid_express
+Version: 0.6.5
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

