# Comparing `tmp/lusid_express-0.5.1.tar.gz` & `tmp/lusid_express-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-0.5.1.tar", last modified: Thu Apr 18 23:27:21 2024, max compression
+gzip compressed data, was "lusid_express-0.5.2.tar", last modified: Thu Apr 18 23:39:09 2024, max compression
```

## Comparing `lusid_express-0.5.1.tar` & `lusid_express-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:27:21.128394 lusid_express-0.5.1/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-18 23:27:18.000000 lusid_express-0.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-18 23:27:18.000000 lusid_express-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6548 2024-04-18 23:27:21.127394 lusid_express-0.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-18 23:27:18.000000 lusid_express-0.5.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 23:27:21.128394 lusid_express-0.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-18 23:27:18.000000 lusid_express-0.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:27:21.123394 lusid_express-0.5.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:27:21.125394 lusid_express-0.5.1/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-18 23:27:18.000000 lusid_express-0.5.1/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1941 2024-04-18 23:27:18.000000 lusid_express-0.5.1/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:27:21.126394 lusid_express-0.5.1/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-18 23:27:18.000000 lusid_express-0.5.1/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:27:21.127394 lusid_express-0.5.1/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-18 23:27:18.000000 lusid_express-0.5.1/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:27:21.127394 lusid_express-0.5.1/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-18 23:27:18.000000 lusid_express-0.5.1/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)     6589 2024-04-18 23:27:18.000000 lusid_express-0.5.1/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-18 23:27:18.000000 lusid_express-0.5.1/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:27:21.126394 lusid_express-0.5.1/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6548 2024-04-18 23:27:21.000000 lusid_express-0.5.1/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-18 23:27:21.000000 lusid_express-0.5.1/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 23:27:21.000000 lusid_express-0.5.1/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-18 23:27:21.000000 lusid_express-0.5.1/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-18 23:27:21.000000 lusid_express-0.5.1/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.552502 lusid_express-0.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-18 23:39:06.000000 lusid_express-0.5.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-18 23:39:06.000000 lusid_express-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-18 23:39:09.552502 lusid_express-0.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-18 23:39:06.000000 lusid_express-0.5.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 23:39:09.552502 lusid_express-0.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-18 23:39:06.000000 lusid_express-0.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.548502 lusid_express-0.5.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.550502 lusid_express-0.5.2/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2423 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.551502 lusid_express-0.5.2/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.551502 lusid_express-0.5.2/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.552502 lusid_express-0.5.2/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)     6589 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-18 23:39:06.000000 lusid_express-0.5.2/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 23:39:09.551502 lusid_express-0.5.2/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-18 23:39:09.000000 lusid_express-0.5.2/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-18 23:39:09.000000 lusid_express-0.5.2/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 23:39:09.000000 lusid_express-0.5.2/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-18 23:39:09.000000 lusid_express-0.5.2/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-18 23:39:09.000000 lusid_express-0.5.2/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-0.5.1/LICENSE` & `lusid_express-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.1/PKG-INFO` & `lusid_express-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 0.5.1
+Version: 0.5.2
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-0.5.1/README.md` & `lusid_express-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.1/setup.py` & `lusid_express-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='0.5.1',
+    version='0.5.2',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-0.5.1/src/lusid_express/__main__.py` & `lusid_express-0.5.2/src/lusid_express/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,25 +16,39 @@
     if os.path.exists(config_path):
         with open(config_path, 'r') as f:
             config = yaml.safe_load(f) or {}
     else:
         config = {'features': []}
 
     enabled_features = set(config.get('features', []))
-
+    show_msg = False
+    change_msg = "Configuration updated successfully! Changes will be applied after kernel restart."
     if args.enable:
+        diff = set(args.enable) - enabled_features
         enabled_features.update(args.enable)
+        if diff:
+            print(f"Enabling features: {', '.join(diff)}")
+            print(change_msg)
 
     if args.disable:
+        diff = set(args.disable) - enabled_features
+        for feature in args.disable:
+            if feature in enabled_features:
+                show_msg = True
         enabled_features.difference_update(args.disable)
+        if show_msg:
+            print(f"Disabling features: {', '.join(args.disable)}")
+            print(change_msg)
 
     config['features'] = list(enabled_features)
 
     with open(config_path, 'w') as f:
         yaml.safe_dump(config, f)
+    
+    
 
 
 def copy_startup_file():
     ipython_startup_dir = os.path.expanduser('~/.ipython/profile_default/startup/')
     target_file = os.path.join(ipython_startup_dir, '00-load_lusid_express.py')
     source_file = os.path.join(os.path.dirname(__file__), 'load.le')
 
@@ -51,11 +65,11 @@
         
         
         
 def main():
     args = parse_args()
     update_config(args)
     copy_startup_file()
-    print("Configuration updated successfully! Changes will be applied after kernel restart.")
+    
 
 if __name__ == "__main__":
     main()
```

### Comparing `lusid_express-0.5.1/src/lusid_express/apis/__init__.py` & `lusid_express-0.5.2/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.1/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-0.5.2/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.1/src/lusid_express/display/__init__.py` & `lusid_express-0.5.2/src/lusid_express/display/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.1/src/lusid_express/load.le` & `lusid_express-0.5.2/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-0.5.1/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-0.5.2/src/lusid_express.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 0.5.1
+Version: 0.5.2
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

