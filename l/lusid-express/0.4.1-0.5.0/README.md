# Comparing `tmp/lusid_express-0.4.1.tar.gz` & `tmp/lusid_express-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-0.4.1.tar", last modified: Wed Apr 17 21:16:17 2024, max compression
+gzip compressed data, was "lusid_express-0.5.0.tar", last modified: Thu Apr 18 15:19:45 2024, max compression
```

## Comparing `lusid_express-0.4.1.tar` & `lusid_express-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.890872 lusid_express-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-17 21:16:15.000000 lusid_express-0.4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-17 21:16:15.000000 lusid_express-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6548 2024-04-17 21:16:17.890872 lusid_express-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-17 21:16:15.000000 lusid_express-0.4.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 21:16:17.890872 lusid_express-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-17 21:16:15.000000 lusid_express-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.886872 lusid_express-0.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.888872 lusid_express-0.4.1/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.889872 lusid_express-0.4.1/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.889872 lusid_express-0.4.1/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.889872 lusid_express-0.4.1/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)     5995 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2024-04-17 21:16:15.000000 lusid_express-0.4.1/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 21:16:17.889872 lusid_express-0.4.1/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6548 2024-04-17 21:16:17.000000 lusid_express-0.4.1/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-17 21:16:17.000000 lusid_express-0.4.1/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 21:16:17.000000 lusid_express-0.4.1/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-17 21:16:17.000000 lusid_express-0.4.1/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-17 21:16:17.000000 lusid_express-0.4.1/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:19:45.358035 lusid_express-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-18 15:19:42.000000 lusid_express-0.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-18 15:19:42.000000 lusid_express-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-18 15:19:45.357035 lusid_express-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-18 15:19:42.000000 lusid_express-0.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 15:19:45.358035 lusid_express-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-18 15:19:42.000000 lusid_express-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:19:45.353035 lusid_express-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:19:45.355035 lusid_express-0.5.0/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-18 15:19:42.000000 lusid_express-0.5.0/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1941 2024-04-18 15:19:42.000000 lusid_express-0.5.0/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:19:45.356035 lusid_express-0.5.0/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-18 15:19:42.000000 lusid_express-0.5.0/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:19:45.356035 lusid_express-0.5.0/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-18 15:19:42.000000 lusid_express-0.5.0/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:19:45.356035 lusid_express-0.5.0/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-18 15:19:42.000000 lusid_express-0.5.0/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)     5995 2024-04-18 15:19:42.000000 lusid_express-0.5.0/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-18 15:19:42.000000 lusid_express-0.5.0/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:19:45.356035 lusid_express-0.5.0/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6548 2024-04-18 15:19:45.000000 lusid_express-0.5.0/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-18 15:19:45.000000 lusid_express-0.5.0/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 15:19:45.000000 lusid_express-0.5.0/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-18 15:19:45.000000 lusid_express-0.5.0/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-18 15:19:45.000000 lusid_express-0.5.0/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-0.4.1/LICENSE` & `lusid_express-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.1/PKG-INFO` & `lusid_express-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 0.4.1
+Version: 0.5.0
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-0.4.1/README.md` & `lusid_express-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.1/setup.py` & `lusid_express-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='0.4.1',
+    version='0.5.0',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-0.4.1/src/lusid_express/__main__.py` & `lusid_express-0.5.0/src/lusid_express/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import yaml
 import os
 import shutil
 
 def parse_args():
     
     parser = argparse.ArgumentParser(description="Configure lusid_express settings.")
-    parser.add_argument('-e','--enable', nargs='+', type=str, choices=['vars', 'magic'], help='Enable feature(s).')
-    parser.add_argument('-d','--disable', nargs='+', type=str, choices=['vars', 'magic'], help='Disable feature(s).')
+    parser.add_argument('-e','--enable', nargs='+', type=str, choices=['vars', 'magic','format'], help='Enable feature(s).')
+    parser.add_argument('-d','--disable', nargs='+', type=str, choices=['vars', 'magic','format'], help='Disable feature(s).')
+    
     return parser.parse_args()
 
 def update_config(args):
     config_path = os.path.join(os.path.dirname(__file__), 'config.yaml')
     if os.path.exists(config_path):
         with open(config_path, 'r') as f:
             config = yaml.safe_load(f) or {}
```

### Comparing `lusid_express-0.4.1/src/lusid_express/apis/__init__.py` & `lusid_express-0.5.0/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.1/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-0.5.0/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.1/src/lusid_express/display/__init__.py` & `lusid_express-0.5.0/src/lusid_express/display/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.4.1/src/lusid_express/load.le` & `lusid_express-0.5.0/src/lusid_express/load.le`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict, List
 
 def initialize_ipython(config:Dict[str,List[str]]):
     
     features = config.get('features', [])
     do_vars = 'vars' in features
     do_magic = 'magic' in features
+    do_format = 'format' in features
     if do_vars:
         from IPython import get_ipython
         ipython = get_ipython()
         
         # Perform imports and assign them to variables
         import lusid as lu
         import lusid.models as lm
@@ -18,26 +19,32 @@
         ipython.user_ns['lu'] = lu
         ipython.user_ns['lm'] = lm
         ipython.user_ns['apis'] = apis
     if do_magic:
         from IPython.core.magic import register_line_cell_magic
         import os
         from lumipy.client import Client
-
         @register_line_cell_magic
         def luminesce(line, cell=None):
             query = cell if cell is not None else line
             lm_client = Client(api_secrets_filename=os.environ.get('FBN_SECRETS_PATH',None))
             df = lm_client.query_and_fetch(query)
             return df
 
         def load_ipython_extension(ipython):
             ipython.register_magic_function(luminesce, 'line_cell', 'luminesce')
 
-        del luminesce 
+        del luminesce
+        
+    if do_format:
+        from lusid_express.display import render_html,STYLES
+        for k in STYLES:
+            render_html(STYLES[k])
+
+
     
 try:
     from lusid_express.config import load
     config = load()
     if config is None:
         pass
     else:
```

### Comparing `lusid_express-0.4.1/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-0.5.0/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 0.4.1
+Version: 0.5.0
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

