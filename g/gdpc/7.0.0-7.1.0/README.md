# Comparing `tmp/gdpc-7.0.0.tar.gz` & `tmp/gdpc-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdpc-7.0.0.tar", last modified: Fri Mar 22 21:25:52 2024, max compression
+gzip compressed data, was "gdpc-7.1.0.tar", last modified: Fri Apr 19 20:44:48 2024, max compression
```

## Comparing `gdpc-7.0.0.tar` & `gdpc-7.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-03-22 21:25:52.031682 gdpc-7.0.0/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1157 2024-03-22 20:24:31.000000 gdpc-7.0.0/LICENSE
--rw-r--r--   0 arthur    (1000) arthur    (1000)     8890 2024-03-22 21:25:52.031682 gdpc-7.0.0/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7087 2024-03-22 21:08:39.000000 gdpc-7.0.0/README.md
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-03-22 21:25:52.031682 gdpc-7.0.0/gdpc/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1138 2024-03-22 20:56:34.000000 gdpc-7.0.0/gdpc/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4478 2023-03-24 01:05:49.000000 gdpc-7.0.0/gdpc/block.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7343 2023-02-01 16:21:53.000000 gdpc-7.0.0/gdpc/block_state_tools.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    24845 2024-03-21 18:31:25.000000 gdpc-7.0.0/gdpc/editor.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     6164 2024-03-21 18:28:03.000000 gdpc-7.0.0/gdpc/editor_tools.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      505 2023-02-01 00:45:52.000000 gdpc-7.0.0/gdpc/exceptions.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     9321 2023-03-24 01:05:49.000000 gdpc-7.0.0/gdpc/geometry.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    12964 2024-03-21 20:36:02.000000 gdpc-7.0.0/gdpc/interface.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)   121425 2024-03-11 15:00:48.000000 gdpc-7.0.0/gdpc/lookup.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     9748 2024-03-21 15:42:39.000000 gdpc-7.0.0/gdpc/minecraft_tools.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2575 2023-03-24 01:05:49.000000 gdpc-7.0.0/gdpc/model.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2042 2024-03-11 15:00:48.000000 gdpc-7.0.0/gdpc/nbt_tools.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7814 2024-03-20 21:29:37.000000 gdpc-7.0.0/gdpc/transform.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4536 2024-03-11 15:00:48.000000 gdpc-7.0.0/gdpc/utils.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    48614 2024-03-11 15:00:48.000000 gdpc-7.0.0/gdpc/vector_tools.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    14199 2024-03-11 15:00:48.000000 gdpc-7.0.0/gdpc/world_slice.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-03-22 21:25:52.031682 gdpc-7.0.0/gdpc.egg-info/
--rw-r--r--   0 arthur    (1000) arthur    (1000)     8890 2024-03-22 21:25:52.000000 gdpc-7.0.0/gdpc.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      498 2024-03-22 21:25:52.000000 gdpc-7.0.0/gdpc.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-03-22 21:25:52.000000 gdpc-7.0.0/gdpc.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-02-27 18:17:38.000000 gdpc-7.0.0/gdpc.egg-info/not-zip-safe
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      140 2024-03-22 21:25:52.000000 gdpc-7.0.0/gdpc.egg-info/requires.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        5 2024-03-22 21:25:52.000000 gdpc-7.0.0/gdpc.egg-info/top_level.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      104 2022-09-29 15:44:28.000000 gdpc-7.0.0/pyproject.toml
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2024-03-22 21:25:52.031682 gdpc-7.0.0/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2869 2024-03-11 15:00:48.000000 gdpc-7.0.0/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-04-19 20:44:48.611605 gdpc-7.1.0/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1157 2024-03-25 17:37:02.000000 gdpc-7.1.0/LICENSE
+-rw-r--r--   0 arthur    (1000) arthur    (1000)     8890 2024-04-19 20:44:48.611605 gdpc-7.1.0/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7087 2024-03-25 17:37:02.000000 gdpc-7.1.0/README.md
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-04-19 20:44:48.607605 gdpc-7.1.0/gdpc/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1138 2024-04-19 20:39:32.000000 gdpc-7.1.0/gdpc/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4478 2023-03-24 01:05:49.000000 gdpc-7.1.0/gdpc/block.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7343 2023-02-01 16:21:53.000000 gdpc-7.1.0/gdpc/block_state_tools.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    24845 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/editor.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     6164 2024-03-25 17:37:02.000000 gdpc-7.1.0/gdpc/editor_tools.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      505 2023-02-01 00:45:52.000000 gdpc-7.1.0/gdpc/exceptions.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     9321 2023-03-24 01:05:49.000000 gdpc-7.1.0/gdpc/geometry.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    13828 2024-04-19 20:36:27.000000 gdpc-7.1.0/gdpc/interface.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)   121425 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/lookup.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     9748 2024-03-25 17:37:02.000000 gdpc-7.1.0/gdpc/minecraft_tools.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2575 2023-03-24 01:05:49.000000 gdpc-7.1.0/gdpc/model.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2042 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/nbt_tools.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7814 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/transform.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4536 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/utils.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    48614 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/vector_tools.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    14199 2024-03-22 21:29:37.000000 gdpc-7.1.0/gdpc/world_slice.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-04-19 20:44:48.611605 gdpc-7.1.0/gdpc.egg-info/
+-rw-r--r--   0 arthur    (1000) arthur    (1000)     8890 2024-04-19 20:44:48.000000 gdpc-7.1.0/gdpc.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      498 2024-04-19 20:44:48.000000 gdpc-7.1.0/gdpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-04-19 20:44:48.000000 gdpc-7.1.0/gdpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-02-27 18:17:38.000000 gdpc-7.1.0/gdpc.egg-info/not-zip-safe
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      140 2024-04-19 20:44:48.000000 gdpc-7.1.0/gdpc.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        5 2024-04-19 20:44:48.000000 gdpc-7.1.0/gdpc.egg-info/top_level.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      104 2022-09-29 15:44:28.000000 gdpc-7.1.0/pyproject.toml
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2024-04-19 20:44:48.611605 gdpc-7.1.0/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2869 2024-03-22 21:29:37.000000 gdpc-7.1.0/setup.py
```

### Comparing `gdpc-7.0.0/LICENSE` & `gdpc-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/PKG-INFO` & `gdpc-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdpc
-Version: 7.0.0
+Version: 7.1.0
 Summary: The Generative Design Python Client (GDPC) is a Python-based interface for the Minecraft GDMC HTTP Interface mod.\nIt was created for use in the Generative Design in Minecraft Competition (GDMC).
 Home-page: https://github.com/avdstaaij/gdpc
 Author: Arthur van der Staaij, Blinkenlights, Nils Gawlik
 Author-email: arthurvanderstaaij@gmail.com, blinkenlights@pm.me, nilsgawlik@gmx.de
 Maintainer: Arthur van der Staaij
 Maintainer-email: arthurvanderstaaij@gmail.com
 License: MIT
```

### Comparing `gdpc-7.0.0/README.md` & `gdpc-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/__init__.py` & `gdpc-7.1.0/gdpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __url__              = "https://github.com/avdstaaij/gdpc"
 __author__           = "Arthur van der Staaij, Blinkenlights, Nils Gawlik"
 __author_email__     = "arthurvanderstaaij@gmail.com, blinkenlights@pm.me, nilsgawlik@gmx.de"
 __maintainer__       = "Arthur van der Staaij"
 __maintainer_email__ = "arthurvanderstaaij@gmail.com"
 __license__          = "MIT"
 __copyright__        = "Copyright 2022-2024 Arthur van der Staaij, Copyright 2021-2022 Blinkenlights, Copyright 2020-2021 Nils Gawlik"
-__version__          = "7.0.0"
+__version__          = "7.1.0"
 
 
 from .vector_tools import Rect, Box
 from .transform import Transform
 from .block import Block
 from .world_slice import WorldSlice
 from .editor import Editor
```

### Comparing `gdpc-7.0.0/gdpc/block.py` & `gdpc-7.1.0/gdpc/block.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/block_state_tools.py` & `gdpc-7.1.0/gdpc/block_state_tools.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/editor.py` & `gdpc-7.1.0/gdpc/editor.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/editor_tools.py` & `gdpc-7.1.0/gdpc/editor_tools.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/geometry.py` & `gdpc-7.1.0/gdpc/geometry.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/interface.py` & `gdpc-7.1.0/gdpc/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -315,10 +315,32 @@
     }
     headers = {'Accept-Encoding': 'gzip'} if returnCompressed is True else None
 
     response = _request(method="GET", url=url, params=parameters, headers=headers, retries=retries, timeout=timeout)
     return response.content
 
 
+def getEntities(selector: Optional[str] = None, includeData: bool = True, dimension: Optional[str] = None, retries=0, timeout=None, host=DEFAULT_HOST):
+    url = f'{host}/entities'
+    parameters = {
+        'selector': selector,
+        'dimension': dimension,
+        'includeData': includeData,
+    }
+    response = _request(method='GET', url=url, params=parameters, retries=retries, timeout=timeout)
+    return response.json()
+
+
+def getPlayers(selector: Optional[str] = None, includeData: bool = True, dimension: Optional[str] = None, retries=0, timeout=None, host=DEFAULT_HOST):
+    url = f'{host}/players'
+    parameters = {
+        'selector': selector,
+        'dimension': dimension,
+        'includeData': includeData,
+    }
+    response = _request(method='GET', url=url, params=parameters, retries=retries, timeout=timeout)
+    return response.json()
+
+
 def getVersion(retries=0, timeout=None, host=DEFAULT_HOST):
     """Returns the Minecraft version as a string."""
     return _request("GET", f"{host}/version", retries=retries, timeout=timeout).text
```

### Comparing `gdpc-7.0.0/gdpc/lookup.py` & `gdpc-7.1.0/gdpc/lookup.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/minecraft_tools.py` & `gdpc-7.1.0/gdpc/minecraft_tools.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/model.py` & `gdpc-7.1.0/gdpc/model.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/nbt_tools.py` & `gdpc-7.1.0/gdpc/nbt_tools.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/transform.py` & `gdpc-7.1.0/gdpc/transform.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/utils.py` & `gdpc-7.1.0/gdpc/utils.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/vector_tools.py` & `gdpc-7.1.0/gdpc/vector_tools.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc/world_slice.py` & `gdpc-7.1.0/gdpc/world_slice.py`

 * *Files identical despite different names*

### Comparing `gdpc-7.0.0/gdpc.egg-info/PKG-INFO` & `gdpc-7.1.0/gdpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdpc
-Version: 7.0.0
+Version: 7.1.0
 Summary: The Generative Design Python Client (GDPC) is a Python-based interface for the Minecraft GDMC HTTP Interface mod.\nIt was created for use in the Generative Design in Minecraft Competition (GDMC).
 Home-page: https://github.com/avdstaaij/gdpc
 Author: Arthur van der Staaij, Blinkenlights, Nils Gawlik
 Author-email: arthurvanderstaaij@gmail.com, blinkenlights@pm.me, nilsgawlik@gmx.de
 Maintainer: Arthur van der Staaij
 Maintainer-email: arthurvanderstaaij@gmail.com
 License: MIT
```

### Comparing `gdpc-7.0.0/setup.py` & `gdpc-7.1.0/setup.py`

 * *Files identical despite different names*

