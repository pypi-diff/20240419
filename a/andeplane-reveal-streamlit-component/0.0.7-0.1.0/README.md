# Comparing `tmp/andeplane_reveal_streamlit_component-0.0.7.tar.gz` & `tmp/andeplane_reveal_streamlit_component-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andeplane_reveal_streamlit_component-0.0.7.tar", last modified: Thu Apr 18 20:27:53 2024, max compression
+gzip compressed data, was "andeplane_reveal_streamlit_component-0.1.0.tar", last modified: Fri Apr 19 11:34:09 2024, max compression
```

## Comparing `andeplane_reveal_streamlit_component-0.0.7.tar` & `andeplane_reveal_streamlit_component-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,43 @@
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:27:53.417587 andeplane_reveal_streamlit_component-0.0.7/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1897 2024-04-18 20:27:53.417321 andeplane_reveal_streamlit_component-0.0.7/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1248 2024-04-18 20:05:24.000000 andeplane_reveal_streamlit_component-0.0.7/README.md
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:27:53.416653 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1897 2024-04-18 20:27:53.000000 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)      451 2024-04-18 20:27:53.000000 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 20:27:53.000000 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 20:27:53.000000 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/requires.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-04-18 20:27:53.000000 andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/top_level.txt
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:27:53.415469 andeplane_reveal_streamlit_component-0.0.7/reveal/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3714 2024-04-18 20:27:28.000000 andeplane_reveal_streamlit_component-0.0.7/reveal/__init__.py
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:27:53.414064 andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 20:27:53.416302 andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1693 2024-04-18 20:26:40.000000 andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/asset-manifest.json
--rw-r--r--   0 kvakkefly   (501) staff       (20)   197459 2024-04-18 20:25:58.000000 andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/bootstrap.min.css
--rw-r--r--   0 kvakkefly   (501) staff       (20)      553 2024-04-18 20:26:40.000000 andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/index.html
--rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 20:27:53.417634 andeplane_reveal_streamlit_component-0.0.7/setup.cfg
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1125 2024-04-18 20:27:30.000000 andeplane_reveal_streamlit_component-0.0.7/setup.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 11:34:09.889833 andeplane_reveal_streamlit_component-0.1.0/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     2433 2024-04-19 11:34:09.889544 andeplane_reveal_streamlit_component-0.1.0/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1772 2024-04-19 10:15:54.000000 andeplane_reveal_streamlit_component-0.1.0/README.md
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 11:34:09.888734 andeplane_reveal_streamlit_component-0.1.0/andeplane_reveal_streamlit_component.egg-info/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     2433 2024-04-19 11:34:09.000000 andeplane_reveal_streamlit_component-0.1.0/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1688 2024-04-19 11:34:09.000000 andeplane_reveal_streamlit_component-0.1.0/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-19 11:34:09.000000 andeplane_reveal_streamlit_component-0.1.0/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-19 11:34:09.000000 andeplane_reveal_streamlit_component-0.1.0/andeplane_reveal_streamlit_component.egg-info/requires.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-04-19 11:34:09.000000 andeplane_reveal_streamlit_component-0.1.0/andeplane_reveal_streamlit_component.egg-info/top_level.txt
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 11:34:09.866461 andeplane_reveal_streamlit_component-0.1.0/reveal/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3653 2024-04-19 11:17:50.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/__init__.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 11:34:09.864734 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 11:34:09.867409 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1693 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/asset-manifest.json
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   197459 2024-04-19 11:33:38.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/bootstrap.min.css
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      553 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/index.html
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 11:34:09.865107 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 11:34:09.868056 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/css/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   331112 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/css/main.c81cb3cf.css
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   461776 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/css/main.c81cb3cf.css.map
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 11:34:09.875247 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3941 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/114.e0ebff55.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3959 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/142.e332c9ad.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     5176 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/211.ee14119e.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3976 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/413.5c9588ac.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4033 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/463.ad8fb302.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3940 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/690.16ab8bc4.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4753 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/797.fb53d4d2.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4270 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/809.14863d52.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3589 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/82.2b5d6c2f.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3822 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/913.b1b6282c.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3882 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/974.691b1718.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)  5725188 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/main.c4c0dc31.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     5906 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/main.c4c0dc31.js.LICENSE.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20) 16427503 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/js/main.c4c0dc31.js.map
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 11:34:09.888393 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/media/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   106140 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   104332 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   105924 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)    98868 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   105804 2024-04-19 11:34:05.000000 andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-19 11:34:09.889882 andeplane_reveal_streamlit_component-0.1.0/setup.cfg
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1140 2024-04-19 11:33:53.000000 andeplane_reveal_streamlit_component-0.1.0/setup.py
```

### Comparing `andeplane_reveal_streamlit_component-0.0.7/PKG-INFO` & `andeplane_reveal_streamlit_component-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: andeplane_reveal_streamlit_component
-Version: 0.0.7
+Version: 0.1.0
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
+Home-page: 
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
 Provides-Extra: devel
 Requires-Dist: wheel; extra == "devel"
@@ -64,7 +65,20 @@
 
 Open repo folder in another terminal. Install this package as development package
 `pip install -e .`
 
 Extract a token from Fusion, and start with
 
 `COGNITE_TOKEN="TOKEN" streamlit run examples/example.py`
+
+### Local development in fusion stlite
+
+Make sure you have set (reveal/**init**.py:8)[reveal/__init__.py:8] to `_RELEASE = True`.
+
+Step 1) Build front end component with `cd reveal/frontend && yarn && yarn build`
+Step 2) Build streamlit component with `python -m build`
+Step 3) Start local server `python server.py`
+
+Open Fusion, create a Streamlit app and add the following the installed package
+`http://localhost:8000/dist/reveal_streamlit_component-0.0.1-py3-none-any.whl`
+
+It will then load successfully inside Stlite.
```

### Comparing `andeplane_reveal_streamlit_component-0.0.7/README.md` & `andeplane_reveal_streamlit_component-0.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -47,7 +47,20 @@
 
 Open repo folder in another terminal. Install this package as development package
 `pip install -e .`
 
 Extract a token from Fusion, and start with
 
 `COGNITE_TOKEN="TOKEN" streamlit run examples/example.py`
+
+### Local development in fusion stlite
+
+Make sure you have set (reveal/**init**.py:8)[reveal/__init__.py:8] to `_RELEASE = True`.
+
+Step 1) Build front end component with `cd reveal/frontend && yarn && yarn build`
+Step 2) Build streamlit component with `python -m build`
+Step 3) Start local server `python server.py`
+
+Open Fusion, create a Streamlit app and add the following the installed package
+`http://localhost:8000/dist/reveal_streamlit_component-0.0.1-py3-none-any.whl`
+
+It will then load successfully inside Stlite.
```

### Comparing `andeplane_reveal_streamlit_component-0.0.7/andeplane_reveal_streamlit_component.egg-info/PKG-INFO` & `andeplane_reveal_streamlit_component-0.1.0/andeplane_reveal_streamlit_component.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: andeplane_reveal_streamlit_component
-Version: 0.0.7
+Version: 0.1.0
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
+Home-page: 
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
 Provides-Extra: devel
 Requires-Dist: wheel; extra == "devel"
@@ -64,7 +65,20 @@
 
 Open repo folder in another terminal. Install this package as development package
 `pip install -e .`
 
 Extract a token from Fusion, and start with
 
 `COGNITE_TOKEN="TOKEN" streamlit run examples/example.py`
+
+### Local development in fusion stlite
+
+Make sure you have set (reveal/**init**.py:8)[reveal/__init__.py:8] to `_RELEASE = True`.
+
+Step 1) Build front end component with `cd reveal/frontend && yarn && yarn build`
+Step 2) Build streamlit component with `python -m build`
+Step 3) Start local server `python server.py`
+
+Open Fusion, create a Streamlit app and add the following the installed package
+`http://localhost:8000/dist/reveal_streamlit_component-0.0.1-py3-none-any.whl`
+
+It will then load successfully inside Stlite.
```

### Comparing `andeplane_reveal_streamlit_component-0.0.7/reveal/__init__.py` & `andeplane_reveal_streamlit_component-0.1.0/reveal/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,41 +23,37 @@
         # We give the component a simple, descriptive name ("my_component"
         # does not fit this bill, so please choose something better for your
         # own component :)
         "reveal",
         # Pass `url` here to tell Streamlit that the component will be served
         # by the local dev server that you run via `npm run start`.
         # (This is useful while your component is in development.)
-        url="http://localhost:3001",
+        # url="http://localhost:3001",
+        url="https://localhost:3001/",
     )
 else:
     # When we're distributing a production version of the component, we'll
     # replace the `url` param with `path`, and point it to the component's
     # build directory:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component("reveal", path=build_dir)
 
 
-# Create a wrapper function for the component. This is an optional
-# best practice - we could simply expose the component function returned by
-# `declare_component` and call it done. The wrapper allows us to customize
-# our component's API: we can pre-process its input args, post-process its
-# output value, and add a docstring for users.
-def reveal(client, model_id, revision_id, key=None):
-    """Create a new instance of "my_component".
+def reveal(client, scene_external_id, scene_space, key=None):
+    """Create a new instance of Reveal.
 
     Parameters
     ----------
     client: CogniteClient
         The CogniteClient to use
-    model_id: int
-        The model id of the 3D model
-    revision_id: int
-        The revision id of the 3D model
+    scene_external_id: string
+        External id of the 3D scene
+    scene_space: string
+        Space id of the 3D scene
     key: str or None
         An optional key that uniquely identifies this component. If this is
         None, and the component's arguments are changed, the component will
         be re-mounted in the Streamlit frontend and lose its current state.
 
     Returns
     -------
@@ -69,15 +65,25 @@
     """
     # Call through to our private component function. Arguments we pass here
     # will be sent to the frontend, where they'll be available in an "args"
     # dictionary.
     #
     # "default" is a special argument that specifies the initial return
     # value of the component before the user has interacted with it.
-    base_url = client.config.base_url
-    project = client.config.project
-    _, token = client.config.credentials.authorization_header()
-    component_value = _component_func(model_id=model_id, revision_id=revision_id, token=token, base_url=base_url, project=project, key=key, default=0)
-    
+    client_config = {
+        # TODO replace this with a callback that refeshes token
+        # Also; can we get rid of the Bearer evilness?
+        "token": client.config.credentials.authorization_header()[1].replace("Bearer ", ""),
+        "project": client.config.project,
+        "baseUrl": client.config.base_url
+    }
+    component_value = _component_func(
+        client_config=client_config, 
+        scene_external_id=scene_external_id, 
+        scene_space=scene_space, 
+        key=key, 
+        default=0
+    )
+
     # We could modify the value returned from the component if we wanted.
     # There's no need to do this in our simple example - but it's an option.
     return component_value
```

### Comparing `andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/asset-manifest.json` & `andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/asset-manifest.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8049242424242424%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.c4c0dc31.js')], delete: [1]}",*

 * * "'files'": "{'main.js': './static/js/main.c4c0dc31.js', 'main.c4c0dc31.js.map': "*

 * *            "'./static/js/main.c4c0dc31.js.map', delete: ['main.c3bf608e.js.map']}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "entrypoints": [
         "static/css/main.c81cb3cf.css",
-        "static/js/main.c3bf608e.js"
+        "static/js/main.c4c0dc31.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.c3bf608e.js.map": "./static/js/main.c3bf608e.js.map",
+        "main.c4c0dc31.js.map": "./static/js/main.c4c0dc31.js.map",
         "main.c81cb3cf.css.map": "./static/css/main.c81cb3cf.css.map",
         "main.css": "./static/css/main.c81cb3cf.css",
-        "main.js": "./static/js/main.c3bf608e.js",
+        "main.js": "./static/js/main.c4c0dc31.js",
         "static/js/114.e0ebff55.chunk.js": "./static/js/114.e0ebff55.chunk.js",
         "static/js/142.e332c9ad.chunk.js": "./static/js/142.e332c9ad.chunk.js",
         "static/js/211.ee14119e.chunk.js": "./static/js/211.ee14119e.chunk.js",
         "static/js/413.5c9588ac.chunk.js": "./static/js/413.5c9588ac.chunk.js",
         "static/js/463.ad8fb302.chunk.js": "./static/js/463.ad8fb302.chunk.js",
         "static/js/690.16ab8bc4.chunk.js": "./static/js/690.16ab8bc4.chunk.js",
         "static/js/797.fb53d4d2.chunk.js": "./static/js/797.fb53d4d2.chunk.js",
```

### Comparing `andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/bootstrap.min.css` & `andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.0.7/reveal/frontend/build/index.html` & `andeplane_reveal_streamlit_component-0.1.0/reveal/frontend/build/index.html`

 * *Files 25% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><script defer="defer" src="./static/js/main.c3bf608e.js"></script><link href="./static/css/main.c81cb3cf.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><script defer="defer" src="./static/js/main.c4c0dc31.js"></script><link href="./static/css/main.c81cb3cf.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `andeplane_reveal_streamlit_component-0.0.7/setup.py` & `andeplane_reveal_streamlit_component-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="andeplane_reveal_streamlit_component",
-    version="0.0.7",
+    version="0.1.0",
     author="John Smith",
     author_email="john@example.com",
     description="Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    url="",
     packages=setuptools.find_packages(),
-    package_data={'': ['frontend/build/*']},
+    package_data={'': ['frontend/build/**/*']},
     include_package_data=True,
     classifiers=[],
     python_requires=">=3.7",
     install_requires=[
         # By definition, a Custom Component depends on Streamlit.
         # If your component has other Python dependencies, list
         # them here.
```

