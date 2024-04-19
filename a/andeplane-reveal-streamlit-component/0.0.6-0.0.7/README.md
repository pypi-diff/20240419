# Comparing `tmp/andeplane_reveal_streamlit_component-0.0.6.tar.gz` & `tmp/andeplane_reveal_streamlit_component-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andeplane_reveal_streamlit_component-0.0.6.tar", last modified: Thu Apr 18 20:26:58 2024, max compression
+gzip compressed data, was "andeplane_reveal_streamlit_component-0.0.7.tar", last modified: Thu Apr 18 20:27:53 2024, max compression
```

## Comparing `andeplane_reveal_streamlit_component-0.0.6.tar` & `andeplane_reveal_streamlit_component-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:26:58.143036 andeplane_reveal_streamlit_component-0.0.6/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1897 2024-04-18 20:26:58.142583 andeplane_reveal_streamlit_component-0.0.6/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1248 2024-04-18 20:05:24.000000 andeplane_reveal_streamlit_component-0.0.6/README.md
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:26:58.141784 andeplane_reveal_streamlit_component-0.0.6/andeplane_reveal_streamlit_component.egg-info/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1897 2024-04-18 20:26:58.000000 andeplane_reveal_streamlit_component-0.0.6/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)      451 2024-04-18 20:26:58.000000 andeplane_reveal_streamlit_component-0.0.6/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 20:26:58.000000 andeplane_reveal_streamlit_component-0.0.6/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 20:26:58.000000 andeplane_reveal_streamlit_component-0.0.6/andeplane_reveal_streamlit_component.egg-info/requires.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-04-18 20:26:58.000000 andeplane_reveal_streamlit_component-0.0.6/andeplane_reveal_streamlit_component.egg-info/top_level.txt
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:26:58.140893 andeplane_reveal_streamlit_component-0.0.6/reveal/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3715 2024-04-18 20:23:59.000000 andeplane_reveal_streamlit_component-0.0.6/reveal/__init__.py
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:26:58.139482 andeplane_reveal_streamlit_component-0.0.6/reveal/frontend/
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:26:58.141549 andeplane_reveal_streamlit_component-0.0.6/reveal/frontend/build/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1693 2024-04-18 20:26:40.000000 andeplane_reveal_streamlit_component-0.0.6/reveal/frontend/build/asset-manifest.json
--rw-r--r--   0 kvakkefly   (501) staff       (20)   197459 2024-04-18 20:25:58.000000 andeplane_reveal_streamlit_component-0.0.6/reveal/frontend/build/bootstrap.min.css
--rw-r--r--   0 kvakkefly   (501) staff       (20)      553 2024-04-18 20:26:40.000000 andeplane_reveal_streamlit_component-0.0.6/reveal/frontend/build/index.html
--rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 20:26:58.143114 andeplane_reveal_streamlit_component-0.0.6/setup.cfg
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1125 2024-04-18 20:26:55.000000 andeplane_reveal_streamlit_component-0.0.6/setup.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:27:53.417587 andeplane_reveal_streamlit_component-0.0.7/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1897 2024-04-18 20:27:53.417321 andeplane_reveal_streamlit_component-0.0.7/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1248 2024-04-18 20:05:24.000000 andeplane_reveal_streamlit_component-0.0.7/README.md
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:27:53.416653 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1897 2024-04-18 20:27:53.000000 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      451 2024-04-18 20:27:53.000000 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 20:27:53.000000 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 20:27:53.000000 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/requires.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-04-18 20:27:53.000000 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/top_level.txt
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:27:53.415469 andeplane_reveal_streamlit_component-0.0.7/reveal/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3714 2024-04-18 20:27:28.000000 andeplane_reveal_streamlit_component-0.0.7/reveal/__init__.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:27:53.414064 andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:27:53.416302 andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1693 2024-04-18 20:26:40.000000 andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/asset-manifest.json
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   197459 2024-04-18 20:25:58.000000 andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/bootstrap.min.css
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      553 2024-04-18 20:26:40.000000 andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/index.html
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 20:27:53.417634 andeplane_reveal_streamlit_component-0.0.7/setup.cfg
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1125 2024-04-18 20:27:30.000000 andeplane_reveal_streamlit_component-0.0.7/setup.py
```

### Comparing `andeplane_reveal_streamlit_component-0.0.6/PKG-INFO` & `andeplane_reveal_streamlit_component-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andeplane_reveal_streamlit_component
-Version: 0.0.6
+Version: 0.0.7
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
 Provides-Extra: devel
```

### Comparing `andeplane_reveal_streamlit_component-0.0.6/README.md` & `andeplane_reveal_streamlit_component-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.0.6/andeplane_reveal_streamlit_component.egg-info/PKG-INFO` & `andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andeplane_reveal_streamlit_component
-Version: 0.0.6
+Version: 0.0.7
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
 Provides-Extra: devel
```

### Comparing `andeplane_reveal_streamlit_component-0.0.6/reveal/__init__.py` & `andeplane_reveal_streamlit_component-0.0.7/reveal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import streamlit.components.v1 as components
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
```

### Comparing `andeplane_reveal_streamlit_component-0.0.6/reveal/frontend/build/asset-manifest.json` & `andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.0.6/reveal/frontend/build/bootstrap.min.css` & `andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.0.6/reveal/frontend/build/index.html` & `andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.0.6/setup.py` & `andeplane_reveal_streamlit_component-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="andeplane_reveal_streamlit_component",
-    version="0.0.6",
+    version="0.0.7",
     author="John Smith",
     author_email="john@example.com",
     description="Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     package_data={'': ['frontend/build/*']},
```

