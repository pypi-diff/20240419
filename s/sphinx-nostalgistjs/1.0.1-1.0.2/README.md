# Comparing `tmp/sphinx-nostalgistjs-1.0.1.tar.gz` & `tmp/sphinx_nostalgistjs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-nostalgistjs-1.0.1.tar", last modified: Sun Mar 17 23:02:30 2024, max compression
+gzip compressed data, was "sphinx_nostalgistjs-1.0.2.tar", last modified: Fri Apr 19 21:37:34 2024, max compression
```

## Comparing `sphinx-nostalgistjs-1.0.1.tar` & `sphinx_nostalgistjs-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 camargo   (1000) camargo   (1000)        0 2024-03-17 23:02:30.892702 sphinx-nostalgistjs-1.0.1/
--rw-r--r--   0 camargo   (1000) camargo   (1000)     3087 2024-03-08 00:43:36.000000 sphinx-nostalgistjs-1.0.1/.gitignore
--rw-r--r--   0 camargo   (1000) camargo   (1000)    35149 2024-03-08 00:37:51.000000 sphinx-nostalgistjs-1.0.1/LICENSE
--rw-r--r--   0 camargo   (1000) camargo   (1000)     6638 2024-03-17 23:02:30.891702 sphinx-nostalgistjs-1.0.1/PKG-INFO
--rw-r--r--   0 camargo   (1000) camargo   (1000)     5521 2024-03-10 23:00:54.000000 sphinx-nostalgistjs-1.0.1/README.md
--rw-r--r--   0 camargo   (1000) camargo   (1000)     1363 2024-03-17 23:01:12.000000 sphinx-nostalgistjs-1.0.1/pyproject.toml
--rw-r--r--   0 camargo   (1000) camargo   (1000)       38 2024-03-17 23:02:30.892702 sphinx-nostalgistjs-1.0.1/setup.cfg
-drwxr-xr-x   0 camargo   (1000) camargo   (1000)        0 2024-03-17 23:02:30.890702 sphinx-nostalgistjs-1.0.1/src/
-drwxr-xr-x   0 camargo   (1000) camargo   (1000)        0 2024-03-17 23:02:30.891702 sphinx-nostalgistjs-1.0.1/src/sphinx_nostalgistjs/
--rw-r--r--   0 camargo   (1000) camargo   (1000)    12854 2024-03-17 22:52:02.000000 sphinx-nostalgistjs-1.0.1/src/sphinx_nostalgistjs/__init__.py
-drwxr-xr-x   0 camargo   (1000) camargo   (1000)        0 2024-03-17 23:02:30.891702 sphinx-nostalgistjs-1.0.1/src/sphinx_nostalgistjs.egg-info/
--rw-r--r--   0 camargo   (1000) camargo   (1000)     6638 2024-03-17 23:02:30.000000 sphinx-nostalgistjs-1.0.1/src/sphinx_nostalgistjs.egg-info/PKG-INFO
--rw-r--r--   0 camargo   (1000) camargo   (1000)      313 2024-03-17 23:02:30.000000 sphinx-nostalgistjs-1.0.1/src/sphinx_nostalgistjs.egg-info/SOURCES.txt
--rw-r--r--   0 camargo   (1000) camargo   (1000)        1 2024-03-17 23:02:30.000000 sphinx-nostalgistjs-1.0.1/src/sphinx_nostalgistjs.egg-info/dependency_links.txt
--rw-r--r--   0 camargo   (1000) camargo   (1000)       10 2024-03-17 23:02:30.000000 sphinx-nostalgistjs-1.0.1/src/sphinx_nostalgistjs.egg-info/requires.txt
--rw-r--r--   0 camargo   (1000) camargo   (1000)       20 2024-03-17 23:02:30.000000 sphinx-nostalgistjs-1.0.1/src/sphinx_nostalgistjs.egg-info/top_level.txt
+drwxr-xr-x   0 camargo   (1000) camargo   (1000)        0 2024-04-19 21:37:34.449791 sphinx_nostalgistjs-1.0.2/
+-rw-r--r--   0 camargo   (1000) camargo   (1000)     3104 2024-03-17 23:21:56.000000 sphinx_nostalgistjs-1.0.2/.gitignore
+-rw-r--r--   0 camargo   (1000) camargo   (1000)    35149 2024-03-08 00:37:51.000000 sphinx_nostalgistjs-1.0.2/LICENSE
+-rw-r--r--   0 camargo   (1000) camargo   (1000)     6722 2024-04-19 21:37:34.449791 sphinx_nostalgistjs-1.0.2/PKG-INFO
+-rw-r--r--   0 camargo   (1000) camargo   (1000)     5605 2024-03-17 23:17:47.000000 sphinx_nostalgistjs-1.0.2/README.md
+-rw-r--r--   0 camargo   (1000) camargo   (1000)     1363 2024-03-17 23:01:12.000000 sphinx_nostalgistjs-1.0.2/pyproject.toml
+-rw-r--r--   0 camargo   (1000) camargo   (1000)       38 2024-04-19 21:37:34.449791 sphinx_nostalgistjs-1.0.2/setup.cfg
+drwxr-xr-x   0 camargo   (1000) camargo   (1000)        0 2024-04-19 21:37:34.448791 sphinx_nostalgistjs-1.0.2/src/
+drwxr-xr-x   0 camargo   (1000) camargo   (1000)        0 2024-04-19 21:37:34.448791 sphinx_nostalgistjs-1.0.2/src/sphinx_nostalgistjs/
+-rw-r--r--   0 camargo   (1000) camargo   (1000)    12854 2024-04-19 21:35:03.000000 sphinx_nostalgistjs-1.0.2/src/sphinx_nostalgistjs/__init__.py
+drwxr-xr-x   0 camargo   (1000) camargo   (1000)        0 2024-04-19 21:37:34.449791 sphinx_nostalgistjs-1.0.2/src/sphinx_nostalgistjs.egg-info/
+-rw-r--r--   0 camargo   (1000) camargo   (1000)     6722 2024-04-19 21:37:34.000000 sphinx_nostalgistjs-1.0.2/src/sphinx_nostalgistjs.egg-info/PKG-INFO
+-rw-r--r--   0 camargo   (1000) camargo   (1000)      313 2024-04-19 21:37:34.000000 sphinx_nostalgistjs-1.0.2/src/sphinx_nostalgistjs.egg-info/SOURCES.txt
+-rw-r--r--   0 camargo   (1000) camargo   (1000)        1 2024-04-19 21:37:34.000000 sphinx_nostalgistjs-1.0.2/src/sphinx_nostalgistjs.egg-info/dependency_links.txt
+-rw-r--r--   0 camargo   (1000) camargo   (1000)       10 2024-04-19 21:37:34.000000 sphinx_nostalgistjs-1.0.2/src/sphinx_nostalgistjs.egg-info/requires.txt
+-rw-r--r--   0 camargo   (1000) camargo   (1000)       20 2024-04-19 21:37:34.000000 sphinx_nostalgistjs-1.0.2/src/sphinx_nostalgistjs.egg-info/top_level.txt
```

### Comparing `sphinx-nostalgistjs-1.0.1/.gitignore` & `sphinx_nostalgistjs-1.0.2/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -156,7 +156,9 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 .vscode
+
+release commands
```

### Comparing `sphinx-nostalgistjs-1.0.1/LICENSE` & `sphinx_nostalgistjs-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-nostalgistjs-1.0.1/PKG-INFO` & `sphinx_nostalgistjs-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-nostalgistjs
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sphinx extension for embeding Isso comments in documents
 Author: Lucas Pires Camargo
 Maintainer: Lucas Pires Camargo
 Project-URL: homepage, https://camargo.eng.br/projects/sphinx-nostalgistjs/README.html
 Project-URL: repository, https://github.com/lucaspcamargo/sphinx-nostalgistjs
 Project-URL: tracker, https://github.com/lucaspcamargo/sphinx-nostalgistjs/issues
 Keywords: documentation,sphinx,extension,nostalgistjs,emulation,games
@@ -25,14 +25,16 @@
 Requires-Dist: Sphinx>=4
 
 # sphinx-nostalgistjs
 
 Sphinx extension for embedding RetroArch in HTML documents, using [NostalgistJS](https://nostalgist.js.org/).
 Styling and layout depend on Bootstrap v5, not included.
 
+This package is released on [pypi](https://pypi.org/project/sphinx-nostalgistjs/).
+
 <!--ENGBR_SECTION
 ## Demo
 
 Click to start. Use the Z key to jump, and the Enter key to start.
 This is emulating "flappybird.nes" on the "FCEUmm" core in RetroArch.
 
 ```{nostalgistjs}
```

### Comparing `sphinx-nostalgistjs-1.0.1/README.md` & `sphinx_nostalgistjs-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # sphinx-nostalgistjs
 
 Sphinx extension for embedding RetroArch in HTML documents, using [NostalgistJS](https://nostalgist.js.org/).
 Styling and layout depend on Bootstrap v5, not included.
 
+This package is released on [pypi](https://pypi.org/project/sphinx-nostalgistjs/).
+
 <!--ENGBR_SECTION
 ## Demo
 
 Click to start. Use the Z key to jump, and the Enter key to start.
 This is emulating "flappybird.nes" on the "FCEUmm" core in RetroArch.
 
 ```{nostalgistjs}
```

### Comparing `sphinx-nostalgistjs-1.0.1/pyproject.toml` & `sphinx_nostalgistjs-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinx-nostalgistjs-1.0.1/src/sphinx_nostalgistjs/__init__.py` & `sphinx_nostalgistjs-1.0.2/src/sphinx_nostalgistjs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         # TODO setup kwargs according to config IF script needs it
         js_url = app.config.nostalgistjs_script_url
         app.add_js_file(js_url, **kwargs)
         logger.warning("Using NostalgistJS from "+js_url)
 
 def setup(app):
     for cfg in CONFIG_ITEMS:
-        app.add_config_value(cfg, None, {})
+        app.add_config_value(cfg, None, '')
     app.add_node(NostalgistJSNode, html=(NostalgistJSNode.visit, NostalgistJSNode.depart))
     app.add_directive('nostalgistjs', NostalgistJSDirective)
     app.connect('html-page-context', on_html_page_context)
 
     return {
         'version': '0.1',
         'parallel_read_safe': True,
```

### Comparing `sphinx-nostalgistjs-1.0.1/src/sphinx_nostalgistjs.egg-info/PKG-INFO` & `sphinx_nostalgistjs-1.0.2/src/sphinx_nostalgistjs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-nostalgistjs
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sphinx extension for embeding Isso comments in documents
 Author: Lucas Pires Camargo
 Maintainer: Lucas Pires Camargo
 Project-URL: homepage, https://camargo.eng.br/projects/sphinx-nostalgistjs/README.html
 Project-URL: repository, https://github.com/lucaspcamargo/sphinx-nostalgistjs
 Project-URL: tracker, https://github.com/lucaspcamargo/sphinx-nostalgistjs/issues
 Keywords: documentation,sphinx,extension,nostalgistjs,emulation,games
@@ -25,14 +25,16 @@
 Requires-Dist: Sphinx>=4
 
 # sphinx-nostalgistjs
 
 Sphinx extension for embedding RetroArch in HTML documents, using [NostalgistJS](https://nostalgist.js.org/).
 Styling and layout depend on Bootstrap v5, not included.
 
+This package is released on [pypi](https://pypi.org/project/sphinx-nostalgistjs/).
+
 <!--ENGBR_SECTION
 ## Demo
 
 Click to start. Use the Z key to jump, and the Enter key to start.
 This is emulating "flappybird.nes" on the "FCEUmm" core in RetroArch.
 
 ```{nostalgistjs}
```

