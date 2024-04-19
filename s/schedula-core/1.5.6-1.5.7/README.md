# Comparing `tmp/schedula-core-1.5.6.tar.gz` & `tmp/schedula_core-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedula-core-1.5.6.tar", last modified: Wed Apr  3 14:57:09 2024, max compression
+gzip compressed data, was "schedula_core-1.5.7.tar", last modified: Fri Apr 19 10:49:42 2024, max compression
```

## Comparing `schedula-core-1.5.6.tar` & `schedula_core-1.5.7.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.907631 schedula-core-1.5.6/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2020-04-22 23:09:02.000000 schedula-core-1.5.6/AUTHORS.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2020-04-22 23:09:02.000000 schedula-core-1.5.6/LICENSE.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-04-03 14:57:09.907527 schedula-core-1.5.6/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-04-03 14:51:38.000000 schedula-core-1.5.6/README.rst
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.899767 schedula-core-1.5.6/schedula/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4300 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-04-03 14:51:38.000000 schedula-core-1.5.6/schedula/_version.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68892 2024-04-03 12:07:12.000000 schedula-core-1.5.6/schedula/dispatcher.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.903509 schedula-core-1.5.6/schedula/utils/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/__init__.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/alg.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.904348 schedula-core-1.5.6/schedula/utils/asy/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/asy/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/asy/executors.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/asy/factory.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    17367 2024-03-30 08:05:12.000000 schedula-core-1.5.6/schedula/utils/base.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/blue.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/cst.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/dsp.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/exc.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/gen.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/graph.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/imp.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/sol.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-03-14 10:25:40.000000 schedula-core-1.5.6/schedula/utils/utl.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.907155 schedula-core-1.5.6/schedula_core.egg-info/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-04-03 14:57:09.000000 schedula-core-1.5.6/schedula_core.egg-info/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      745 2024-04-03 14:57:09.000000 schedula-core-1.5.6/schedula_core.egg-info/SOURCES.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-04-03 14:57:09.000000 schedula-core-1.5.6/schedula_core.egg-info/dependency_links.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-04-03 14:57:09.000000 schedula-core-1.5.6/schedula_core.egg-info/top_level.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-04-03 14:57:09.908052 schedula-core-1.5.6/setup.cfg
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7084 2024-03-14 10:25:40.000000 schedula-core-1.5.6/setup.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:57:09.906831 schedula-core-1.5.6/tests/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-03-14 10:25:40.000000 schedula-core-1.5.6/tests/test_dispatcher.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-03-14 10:25:40.000000 schedula-core-1.5.6/tests/test_import.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-03-14 10:25:40.000000 schedula-core-1.5.6/tests/test_micropython.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-03-14 10:25:40.000000 schedula-core-1.5.6/tests/test_readme.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-03-14 10:25:40.000000 schedula-core-1.5.6/tests/test_setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.277184 schedula_core-1.5.7/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2024-04-12 16:17:27.000000 schedula_core-1.5.7/AUTHORS.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2024-04-12 16:17:27.000000 schedula_core-1.5.7/LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-04-19 10:49:42.277094 schedula_core-1.5.7/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-04-19 10:36:00.000000 schedula_core-1.5.7/README.rst
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.269435 schedula_core-1.5.7/schedula/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4309 2024-04-17 14:10:45.000000 schedula_core-1.5.7/schedula/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-04-19 10:36:00.000000 schedula_core-1.5.7/schedula/_version.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1267 2024-04-17 14:10:45.000000 schedula_core-1.5.7/schedula/cli.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68892 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/dispatcher.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.273668 schedula_core-1.5.7/schedula/utils/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/__init__.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/alg.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.274514 schedula_core-1.5.7/schedula/utils/asy/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/asy/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/asy/executors.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/asy/factory.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16000 2024-04-17 16:28:10.000000 schedula_core-1.5.7/schedula/utils/base.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/blue.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/cst.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/dsp.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/exc.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/gen.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/graph.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/imp.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/sol.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-04-12 16:17:27.000000 schedula_core-1.5.7/schedula/utils/utl.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.276847 schedula_core-1.5.7/schedula_core.egg-info/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4233 2024-04-19 10:49:42.000000 schedula_core-1.5.7/schedula_core.egg-info/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      761 2024-04-19 10:49:42.000000 schedula_core-1.5.7/schedula_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-04-19 10:49:42.000000 schedula_core-1.5.7/schedula_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-04-19 10:49:42.000000 schedula_core-1.5.7/schedula_core.egg-info/top_level.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-04-19 10:49:42.277574 schedula_core-1.5.7/setup.cfg
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7344 2024-04-19 10:12:23.000000 schedula_core-1.5.7/setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:49:42.276578 schedula_core-1.5.7/tests/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-04-12 16:17:27.000000 schedula_core-1.5.7/tests/test_dispatcher.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-04-12 16:17:27.000000 schedula_core-1.5.7/tests/test_import.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-04-12 16:17:27.000000 schedula_core-1.5.7/tests/test_micropython.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-04-12 16:17:27.000000 schedula_core-1.5.7/tests/test_readme.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-04-12 16:17:27.000000 schedula_core-1.5.7/tests/test_setup.py
```

### Comparing `schedula-core-1.5.6/LICENSE.txt` & `schedula_core-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/PKG-INFO` & `schedula_core-1.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula-core
-Version: 1.5.6
+Version: 1.5.7
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.6
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.7
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
```

### Comparing `schedula-core-1.5.6/README.rst` & `schedula_core-1.5.7/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 #######################################################################
 schedula: A smart function scheduler for dynamic flow-based programming
 #######################################################################
 |pypi_ver| |test_status| |cover_status| |docs_status| |downloads|
 |month_downloads| |github_issues| |python_ver| |proj_license| |binder|
 
-:release:       1.5.6
-:date:          2024-04-03 15:00:00
+:release:       1.5.7
+:date:          2024-04-19 12:30:00
 :repository:    https://github.com/vinci1it2000/schedula
 :pypi-repo:     https://pypi.org/project/schedula/
 :docs:          https://schedula.readthedocs.io/
 :wiki:          https://github.com/vinci1it2000/schedula/wiki/
 :download:      https://github.com/vinci1it2000/schedula/releases/
 :keywords:      flow-based programming, dataflow, parallel, async, scheduling,
                 dispatch, functional programming, dataflow programming
```

### Comparing `schedula-core-1.5.6/schedula/__init__.py` & `schedula_core-1.5.7/schedula/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .. autosummary::
     :nosignatures:
     :toctree: toctree/schedula
 
     ~dispatcher
     ~utils
     ~ext
+    ~cli
 """
 import os
 import sys
 from ._version import *
 
 _all = {
     'Dispatcher': '.dispatcher',
```

### Comparing `schedula-core-1.5.6/schedula/dispatcher.py` & `schedula_core-1.5.7/schedula/dispatcher.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/__init__.py` & `schedula_core-1.5.7/schedula/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/alg.py` & `schedula_core-1.5.7/schedula/utils/alg.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/asy/__init__.py` & `schedula_core-1.5.7/schedula/utils/asy/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/asy/executors.py` & `schedula_core-1.5.7/schedula/utils/asy/executors.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/asy/factory.py` & `schedula_core-1.5.7/schedula/utils/asy/factory.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/base.py` & `schedula_core-1.5.7/schedula/utils/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,17 +113,14 @@
             sites.add(webmap.site(view=run))
         elif run:
             return webmap.site(view=run)
         return webmap
 
     def form(self, depth=1, node_data=NONE, node_function=NONE, directory=None,
              sites=None, run=True, view=True, get_context=NONE, get_data=NONE,
-             edit_on_change='static/schedula/onChange/*.js',
-             pre_submit='static/schedula/preSubmit/*.js',
-             post_submit='static/schedula/postSubmit/*.js',
              subsite_idle_timeout=600, basic_app_config=None,
              stripe_event_handler=lambda event: None):
         """
         Creates a dispatcher Form Flask app.
 
         :param depth:
             Depth of sub-dispatch API. If negative all levels are configured.
@@ -158,26 +155,14 @@
             Function to pass extra data as form context.
         :type get_context: function | dict, optional
 
         :param get_data:
             Function to initialize the formdata.
         :type get_data: function | dict, optional
 
-        :param edit_on_change:
-            JS function to edit on the browser the formdata when value change.
-        :type edit_on_change: str | dict[str], optional
-
-        :param pre_submit:
-            JS function to edit on the browser the formdata before submitting.
-        :type pre_submit: str | dict[str], optional
-
-        :param post_submit:
-            JS function to edit on the browser server response after submision.
-        :type post_submit: str | dict[str], optional
-
         :param subsite_idle_timeout:
             Idle timeout of a debug subsite in seconds.
         :type subsite_idle_timeout: int, optional
 
         :param basic_app_config:
             Flask app config object.
         :type basic_app_config: object, optional
@@ -201,33 +186,17 @@
         formmap = FormMap()
         formmap.add_items(obj, workflow=False, depth=depth, **options)
         formmap.directory = directory
         formmap.idle_timeout = subsite_idle_timeout
         formmap.basic_app_config = basic_app_config
         formmap.stripe_event_handler = stripe_event_handler
         methods = {
-            'get_edit_on_change_func': edit_on_change,
-            'get_pre_submit_func': pre_submit,
-            'get_post_submit_func': post_submit
-        }
-        for k, v in methods.items():
-            if isinstance(v, str):
-                methods[k] = d = {}
-                v = osp.join(directory or '.', *v.replace('\\', '/').split('/'))
-                for fpath in glob.glob(v):
-                    with open(fpath) as f:
-                        d[f'/{osp.splitext(osp.basename(fpath))[0]}'] = f.read()
-                if '/' not in d and '/index' in d:
-                    d['/'] = d['/index']
-                elif not d:
-                    methods[k] = NONE
-        methods.update({
             'get_form_context': get_context,
             'get_form_data': get_data
-        })
+        }
         for k, v in methods.items():
             if v is not NONE:
                 setattr(formmap, f'_{k}', v)
         if sites is not None or run or view:
             site = formmap.site(view=view)
             site = run and not view and site.run() or site
             if sites is None:
```

### Comparing `schedula-core-1.5.6/schedula/utils/blue.py` & `schedula_core-1.5.7/schedula/utils/blue.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/cst.py` & `schedula_core-1.5.7/schedula/utils/cst.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/dsp.py` & `schedula_core-1.5.7/schedula/utils/dsp.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/exc.py` & `schedula_core-1.5.7/schedula/utils/exc.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/gen.py` & `schedula_core-1.5.7/schedula/utils/gen.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/graph.py` & `schedula_core-1.5.7/schedula/utils/graph.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/imp.py` & `schedula_core-1.5.7/schedula/utils/imp.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/sol.py` & `schedula_core-1.5.7/schedula/utils/sol.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula/utils/utl.py` & `schedula_core-1.5.7/schedula/utils/utl.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/schedula_core.egg-info/PKG-INFO` & `schedula_core-1.5.7/schedula_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula-core
-Version: 1.5.6
+Version: 1.5.7
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.6
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.7
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
```

### Comparing `schedula-core-1.5.6/schedula_core.egg-info/SOURCES.txt` & `schedula_core-1.5.7/schedula_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 AUTHORS.rst
 LICENSE.txt
 README.rst
 setup.cfg
 setup.py
 schedula/__init__.py
 schedula/_version.py
+schedula/cli.py
 schedula/dispatcher.py
 schedula/utils/__init__.py
 schedula/utils/alg.py
 schedula/utils/base.py
 schedula/utils/blue.py
 schedula/utils/cst.py
 schedula/utils/dsp.py
```

### Comparing `schedula-core-1.5.6/setup.py` & `schedula_core-1.5.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,41 +87,49 @@
             'requests', 'graphviz>=0.17', 'regex', 'flask', 'Pygments',
             'jinja2', 'docutils'
         ]
     }
     extras['form'] = extras['web'] + [
         'itsdangerous', 'rst2txt', 'flask-sqlalchemy', 'sqlalchemy', 'docutils',
         'flask-babel', 'flask-wtf', 'flask-principal', 'flask-security-too',
-        'flask-mail', 'stripe'
+        'flask-mail', 'stripe', 'click', 'click_log', 'gunicorn'
     ]
     extras['sphinx'] = ['sphinx>=7.2'] + extras['plot']
     extras['all'] = sorted(functools.reduce(set.union, extras.values(), set()))
     extras['dev'] = extras['all'] + [
         'wheel', 'sphinx>=7.2', 'gitchangelog', 'mako', 'sphinx_rtd_theme',
         'setuptools>=36.0.1', 'sphinxcontrib-restbuilder', 'coveralls', 'polib',
         'requests', 'readthedocs-sphinx-ext', 'twine', 'ddt', 'translators',
+        'livereload>=2.6.3'
     ]
     exclude = [
         'doc', 'doc.*',
         'tests', 'tests.*',
         'examples', 'examples.*',
         'micropython', 'micropython.*',
         'requirements', 'binder', 'bin'
     ]
+    kw = {'entry_points': {
+        'console_scripts': [
+            '%(p)s = %(p)s.cli:cli' % {'p': name},
+        ]
+    }}
     if core:
         exclude.extend([
             'schedula.ext', 'schedula.ext.*',
             'schedula.utils.io', 'schedula.utils.io.*',
             'schedula.utils.drw', 'schedula.utils.drw.*',
             'schedula.utils.web', 'schedula.utils.web.*',
             'schedula.utils.form', 'schedula.utils.form.*',
             'schedula.utils.des', 'schedula.utils.des.*',
+            'schedula.cli',
         ])
         name = '%s-core' % name
         extras = {}
+        kw.pop('entry_points')
     long_description = ''
     if os.environ.get('ENABLE_SETUP_LONG_DESCRIPTION') == 'TRUE':
         try:
             long_description = get_long_description(core=core)
             print('LONG DESCRIPTION ENABLED!')
         except Exception as ex:
             print('LONG DESCRIPTION ERROR:\n %r', ex)
@@ -179,9 +187,10 @@
                 'templates/schedula/*', 'static/schedula/js/*.js.gz',
                 'static/schedula/css/*.css.gz',
                 'static/schedula/media/*.gz',
                 'static/schedula/forms/*',
                 'templates/schedula/*',
                 'templates/schedula/email/*'
             ]
-        }
+        },
+        **kw
     )
```

### Comparing `schedula-core-1.5.6/tests/test_dispatcher.py` & `schedula_core-1.5.7/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/tests/test_import.py` & `schedula_core-1.5.7/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/tests/test_micropython.py` & `schedula_core-1.5.7/tests/test_micropython.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/tests/test_readme.py` & `schedula_core-1.5.7/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `schedula-core-1.5.6/tests/test_setup.py` & `schedula_core-1.5.7/tests/test_setup.py`

 * *Files identical despite different names*

