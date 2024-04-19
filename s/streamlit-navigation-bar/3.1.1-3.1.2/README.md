# Comparing `tmp/streamlit-navigation-bar-3.1.1.tar.gz` & `tmp/streamlit-navigation-bar-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-navigation-bar-3.1.1.tar", last modified: Sat Apr  6 16:45:11 2024, max compression
+gzip compressed data, was "streamlit-navigation-bar-3.1.2.tar", last modified: Fri Apr 19 17:36:36 2024, max compression
```

## Comparing `streamlit-navigation-bar-3.1.1.tar` & `streamlit-navigation-bar-3.1.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.630179 streamlit-navigation-bar-3.1.1/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-01-27 21:14:24.000000 streamlit-navigation-bar-3.1.1/LICENSE
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       59 2024-03-03 21:06:11.000000 streamlit-navigation-bar-3.1.1/MANIFEST.in
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13521 2024-04-06 16:45:11.630022 streamlit-navigation-bar-3.1.1/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13004 2024-04-06 16:17:40.000000 streamlit-navigation-bar-3.1.1/README.md
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-04-06 16:45:11.630222 streamlit-navigation-bar-3.1.1/setup.cfg
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1024 2024-04-06 16:42:42.000000 streamlit-navigation-bar-3.1.1/setup.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.627717 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    17101 2024-04-06 16:44:33.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/__init__.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     8452 2024-04-06 13:59:37.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/errors.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      680 2024-03-30 14:23:08.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/example.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.625796 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.628676 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.629751 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/assets/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)   241380 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1150 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      683 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/index.html
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     8267 2024-03-27 17:37:32.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/match_navbar.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-06 16:45:11.628546 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13521 2024-04-06 16:45:11.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      605 2024-04-06 16:45:11.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/SOURCES.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-04-06 16:45:11.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/dependency_links.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       43 2024-04-06 16:45:11.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/requires.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       25 2024-04-06 16:45:11.000000 streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/top_level.txt
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.672514 streamlit-navigation-bar-3.1.2/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-01-27 21:14:24.000000 streamlit-navigation-bar-3.1.2/LICENSE
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       59 2024-03-03 21:06:11.000000 streamlit-navigation-bar-3.1.2/MANIFEST.in
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    15103 2024-04-19 17:36:36.672321 streamlit-navigation-bar-3.1.2/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    13316 2024-04-09 19:20:43.000000 streamlit-navigation-bar-3.1.2/README.md
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-04-19 17:36:36.672563 streamlit-navigation-bar-3.1.2/setup.cfg
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     2474 2024-04-19 17:33:41.000000 streamlit-navigation-bar-3.1.2/setup.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.669415 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    17362 2024-04-09 19:02:56.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/__init__.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       77 2024-04-19 17:15:50.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/__main__.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     8452 2024-04-06 13:59:37.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/errors.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      680 2024-04-19 17:10:51.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/example.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.667314 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.670659 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.672064 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/assets/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)   241380 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1150 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      683 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/index.html
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     8267 2024-03-27 17:37:32.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/match_navbar.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.670538 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    15103 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      693 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       85 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/entry_points.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       43 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/requires.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       25 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/top_level.txt
```

### Comparing `streamlit-navigation-bar-3.1.1/LICENSE` & `streamlit-navigation-bar-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.1/PKG-INFO` & `streamlit-navigation-bar-3.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: streamlit-navigation-bar
-Version: 3.1.1
-Summary: A component that allows you to place a navigation bar in your Streamlit app.
-Home-page: https://github.com/gabrieltempass/streamlit-navigation-bar
-Author: Gabriel Tem Pass
-Author-email: redo_hint_0x@icloud.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Downloads](https://static.pepy.tech/badge/streamlit-navigation-bar/month)](https://pepy.tech/project/streamlit-navigation-bar)
 
 # Streamlit Navigation Bar
 
 A component that allows you to place a navigation bar in your
 Streamlit app.
 
@@ -364,14 +349,18 @@
 multiple ways to contribute, such as [reporting a bug](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=bug&projects=&template=bug_report.yml)
 or [requesting a feature](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=enhancement&projects=&template=feature_request.yml).
 You can also just [ask a question](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=question&projects=&template=ask_question.yml),
 if you want. To submit code for a pull request, make sure to read the [guide on how to contribute](https://github.com/gabrieltempass/streamlit-navigation-bar/blob/main/CONTRIBUTING.md).
 
 ## References
 
-This Streamlit component is based on:
-* The [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template)
-  repository, by [@gabrieltempass](https://github.com/gabrieltempass)
+The Streamlit Navigation Bar was made with:
+* The [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template),
+  by [@gabrieltempass](https://github.com/gabrieltempass)
+* The [streamlit-theme](https://github.com/gabrieltempass/streamlit-theme)
+  component, by [@gabrieltempass](https://github.com/gabrieltempass)
+
+And based on:
 * The [streamlit-option-menu](https://github.com/victoryhb/streamlit-option-menu/tree/master)
   component, by [@victoryhb](https://github.com/victoryhb)
-
-
+* The [styleable container](https://arnaudmiribel.github.io/streamlit-extras/extras/stylable_container/),
+  by [@LukasMasuch](https://github.com/LukasMasuch)
```

### Comparing `streamlit-navigation-bar-3.1.1/README.md` & `streamlit-navigation-bar-3.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: streamlit-navigation-bar
+Version: 3.1.2
+Summary: A component that allows you to place a navigation bar in your Streamlit app.
+Home-page: https://github.com/gabrieltempass/streamlit-navigation-bar
+Author: Gabriel Tem Pass
+Author-email: redo_hint_0x@icloud.com
+License: MIT License
+Project-URL: Source Code, https://github.com/gabrieltempass/streamlit-navigation-bar
+Project-URL: Bug Tracker, https://github.com/gabrieltempass/streamlit-navigation-bar/issues
+Project-URL: Release notes, https://github.com/gabrieltempass/streamlit-navigation-bar/releases
+Project-URL: Documentation, https://github.com/gabrieltempass/streamlit-navigation-bar/wiki
+Project-URL: Community, https://discuss.streamlit.io/t/new-component-streamlit-navigation-bar/66032
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Widget Sets
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Downloads](https://static.pepy.tech/badge/streamlit-navigation-bar/month)](https://pepy.tech/project/streamlit-navigation-bar)
 
 # Streamlit Navigation Bar
 
 A component that allows you to place a navigation bar in your
 Streamlit app.
 
@@ -349,12 +384,20 @@
 multiple ways to contribute, such as [reporting a bug](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=bug&projects=&template=bug_report.yml)
 or [requesting a feature](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=enhancement&projects=&template=feature_request.yml).
 You can also just [ask a question](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=question&projects=&template=ask_question.yml),
 if you want. To submit code for a pull request, make sure to read the [guide on how to contribute](https://github.com/gabrieltempass/streamlit-navigation-bar/blob/main/CONTRIBUTING.md).
 
 ## References
 
-This Streamlit component is based on:
-* The [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template)
-  repository, by [@gabrieltempass](https://github.com/gabrieltempass)
+The Streamlit Navigation Bar was made with:
+* The [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template),
+  by [@gabrieltempass](https://github.com/gabrieltempass)
+* The [streamlit-theme](https://github.com/gabrieltempass/streamlit-theme)
+  component, by [@gabrieltempass](https://github.com/gabrieltempass)
+
+And based on:
 * The [streamlit-option-menu](https://github.com/victoryhb/streamlit-option-menu/tree/master)
   component, by [@victoryhb](https://github.com/victoryhb)
+* The [styleable container](https://arnaudmiribel.github.io/streamlit-extras/extras/stylable_container/),
+  by [@LukasMasuch](https://github.com/LukasMasuch)
+
+
```

### Comparing `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/__init__.py` & `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import base64
+from importlib.metadata import version as _version
 
 import streamlit as st
 import streamlit.components.v1 as components
 from jinja2 import FileSystemLoader, Environment
 
 from streamlit_navigation_bar.match_navbar import MatchNavbar
 from streamlit_navigation_bar.errors import (
@@ -31,14 +32,20 @@
     build_dir = os.path.join(parent_dir, "frontend/dist")
     _st_navbar = components.declare_component(
         "st_navbar",
         path=build_dir,
     )
 
 
+def print_version():
+    """Show the installed version of the Streamlit Navigation Bar package."""
+    version = _version("streamlit-navigation-bar")
+    print(f"Streamlit Navigation Bar, version {version}")
+
+
 def _encode_svg(path):
     """Encode an SVG to base64, from an absolute path."""
     svg = open(path).read()
     return base64.b64encode(svg.encode("utf-8")).decode("utf-8")
 
 
 def _prepare_urls(urls, pages):
```

### Comparing `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/errors.py` & `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/example.py` & `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/example.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js` & `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css` & `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/frontend/dist/index.html` & `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar/match_navbar.py` & `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/match_navbar.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/PKG-INFO` & `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,38 @@
 Metadata-Version: 2.1
 Name: streamlit-navigation-bar
-Version: 3.1.1
+Version: 3.1.2
 Summary: A component that allows you to place a navigation bar in your Streamlit app.
 Home-page: https://github.com/gabrieltempass/streamlit-navigation-bar
 Author: Gabriel Tem Pass
 Author-email: redo_hint_0x@icloud.com
-License: UNKNOWN
+License: MIT License
+Project-URL: Source Code, https://github.com/gabrieltempass/streamlit-navigation-bar
+Project-URL: Bug Tracker, https://github.com/gabrieltempass/streamlit-navigation-bar/issues
+Project-URL: Release notes, https://github.com/gabrieltempass/streamlit-navigation-bar/releases
+Project-URL: Documentation, https://github.com/gabrieltempass/streamlit-navigation-bar/wiki
+Project-URL: Community, https://discuss.streamlit.io/t/new-component-streamlit-navigation-bar/66032
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Downloads](https://static.pepy.tech/badge/streamlit-navigation-bar/month)](https://pepy.tech/project/streamlit-navigation-bar)
 
 # Streamlit Navigation Bar
@@ -364,14 +384,20 @@
 multiple ways to contribute, such as [reporting a bug](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=bug&projects=&template=bug_report.yml)
 or [requesting a feature](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=enhancement&projects=&template=feature_request.yml).
 You can also just [ask a question](https://github.com/gabrieltempass/streamlit-navigation-bar/issues/new?assignees=&labels=question&projects=&template=ask_question.yml),
 if you want. To submit code for a pull request, make sure to read the [guide on how to contribute](https://github.com/gabrieltempass/streamlit-navigation-bar/blob/main/CONTRIBUTING.md).
 
 ## References
 
-This Streamlit component is based on:
-* The [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template)
-  repository, by [@gabrieltempass](https://github.com/gabrieltempass)
+The Streamlit Navigation Bar was made with:
+* The [streamlit-component-vue-vite-template](https://github.com/gabrieltempass/streamlit-component-vue-vite-template),
+  by [@gabrieltempass](https://github.com/gabrieltempass)
+* The [streamlit-theme](https://github.com/gabrieltempass/streamlit-theme)
+  component, by [@gabrieltempass](https://github.com/gabrieltempass)
+
+And based on:
 * The [streamlit-option-menu](https://github.com/victoryhb/streamlit-option-menu/tree/master)
   component, by [@victoryhb](https://github.com/victoryhb)
+* The [styleable container](https://arnaudmiribel.github.io/streamlit-extras/extras/stylable_container/),
+  by [@LukasMasuch](https://github.com/LukasMasuch)
```

### Comparing `streamlit-navigation-bar-3.1.1/streamlit_navigation_bar.egg-info/SOURCES.txt` & `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 streamlit_navigation_bar/__init__.py
+streamlit_navigation_bar/__main__.py
 streamlit_navigation_bar/errors.py
 streamlit_navigation_bar/example.py
 streamlit_navigation_bar/match_navbar.py
 streamlit_navigation_bar.egg-info/PKG-INFO
 streamlit_navigation_bar.egg-info/SOURCES.txt
 streamlit_navigation_bar.egg-info/dependency_links.txt
+streamlit_navigation_bar.egg-info/entry_points.txt
 streamlit_navigation_bar.egg-info/requires.txt
 streamlit_navigation_bar.egg-info/top_level.txt
 streamlit_navigation_bar/frontend/dist/index.html
 streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js
 streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css
```

