# Comparing `tmp/x256offline-0.0.2.tar.gz` & `tmp/x256offline-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x256offline-0.0.2.tar", last modified: Fri Apr 19 13:18:18 2024, max compression
+gzip compressed data, was "x256offline-0.0.3.tar", last modified: Fri Apr 19 14:00:30 2024, max compression
```

## Comparing `x256offline-0.0.2.tar` & `x256offline-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 13:18:18.339105 x256offline-0.0.2/
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)     1063 2024-04-14 13:47:56.000000 x256offline-0.0.2/LICENSE
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)     2380 2024-04-19 13:18:18.319035 x256offline-0.0.2/PKG-INFO
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)      520 2024-04-15 02:10:20.000000 x256offline-0.0.2/README.rst
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)      895 2024-04-17 13:58:08.000000 x256offline-0.0.2/pyproject.toml
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)       38 2024-04-19 13:18:18.340107 x256offline-0.0.2/setup.cfg
-drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 13:18:17.114005 x256offline-0.0.2/src/
-drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 13:18:17.687747 x256offline-0.0.2/src/x256offline/
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)       58 2024-04-17 12:55:05.000000 x256offline-0.0.2/src/x256offline/__init__.py
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)     3359 2024-04-17 12:36:48.000000 x256offline-0.0.2/src/x256offline/x256.py
--rwxrwxrwx   0 elaina    (1000) elaina    (1000) 16777216 2024-04-17 12:39:45.000000 x256offline-0.0.2/src/x256offline/x256e.bin
--rwxrwxrwx   0 elaina    (1000) elaina    (1000) 16777216 2024-04-17 12:39:45.000000 x256offline-0.0.2/src/x256offline/x256w.bin
-drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 13:18:18.305085 x256offline-0.0.2/src/x256offline.egg-info/
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)     2380 2024-04-19 13:18:16.000000 x256offline-0.0.2/src/x256offline.egg-info/PKG-INFO
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)      293 2024-04-19 13:18:17.000000 x256offline-0.0.2/src/x256offline.egg-info/SOURCES.txt
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)        1 2024-04-19 13:18:16.000000 x256offline-0.0.2/src/x256offline.egg-info/dependency_links.txt
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)       12 2024-04-19 13:18:16.000000 x256offline-0.0.2/src/x256offline.egg-info/top_level.txt
+drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 14:00:30.035932 x256offline-0.0.3/
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)     1063 2024-04-14 13:47:56.000000 x256offline-0.0.3/LICENSE
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)     2380 2024-04-19 14:00:30.033883 x256offline-0.0.3/PKG-INFO
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)      520 2024-04-15 02:10:20.000000 x256offline-0.0.3/README.rst
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)      894 2024-04-19 13:59:43.000000 x256offline-0.0.3/pyproject.toml
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)       38 2024-04-19 14:00:30.044854 x256offline-0.0.3/setup.cfg
+drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 14:00:29.624517 x256offline-0.0.3/src/
+drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 14:00:29.795678 x256offline-0.0.3/src/x256offline/
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)       58 2024-04-19 13:19:19.000000 x256offline-0.0.3/src/x256offline/__init__.py
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)   573300 2024-04-19 13:58:13.000000 x256offline-0.0.3/src/x256offline/x256.bin
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)     3522 2024-04-19 13:58:35.000000 x256offline-0.0.3/src/x256offline/x256.py
+drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 14:00:30.013806 x256offline-0.0.3/src/x256offline.egg-info/
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)     2380 2024-04-19 14:00:29.000000 x256offline-0.0.3/src/x256offline.egg-info/PKG-INFO
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)      266 2024-04-19 14:00:29.000000 x256offline-0.0.3/src/x256offline.egg-info/SOURCES.txt
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)        1 2024-04-19 14:00:29.000000 x256offline-0.0.3/src/x256offline.egg-info/dependency_links.txt
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)       12 2024-04-19 14:00:29.000000 x256offline-0.0.3/src/x256offline.egg-info/top_level.txt
```

### Comparing `x256offline-0.0.2/LICENSE` & `x256offline-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `x256offline-0.0.2/PKG-INFO` & `x256offline-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x256offline
-Version: 0.0.2
+Version: 0.0.3
 Summary: quickly find the nearest xterm 256 color index of an RGB
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2024 Elaina
```

### Comparing `x256offline-0.0.2/README.rst` & `x256offline-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `x256offline-0.0.2/pyproject.toml` & `x256offline-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "x256offline"
-version = "0.0.2"
+version = "0.0.3"
 description = "quickly find the nearest xterm 256 color index of an RGB"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["x256", "xterm", "color"]
 
 authors = [
@@ -21,12 +21,12 @@
 
 [project.urls]
 "Homepage" = "https://github.com/userElaina/python-x256-offline"
 "Bug Reports" = "https://github.com/userElaina/python-x256-offline/issues"
 "Source" = "https://github.com/userElaina/python-x256-offline"
 
 [tool.setuptools]
-package-data = {"x256offline" = ["x256*.bin"]}
+package-data = {"x256offline" = ["x256.bin"]}
 
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `x256offline-0.0.2/src/x256offline/x256.py` & `x256offline-0.0.3/src/x256offline/x256.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import zlib
 
 X256_RGB = [
     0x000000, 0x800000, 0x008000, 0x808000, 0x000080, 0x800080, 0x008080, 0xc0c0c0,
     0x808080, 0xff0000, 0x00ff00, 0xffff00, 0x0000ff, 0xff00ff, 0x00ffff, 0xffffff,
     0x000000, 0x00005f, 0x000087, 0x0000af, 0x0000d7, 0x0000ff, 0x005f00, 0x005f5f,
     0x005f87, 0x005faf, 0x005fd7, 0x005fff, 0x008700, 0x00875f, 0x008787, 0x0087af,
     0x0087d7, 0x0087ff, 0x00af00, 0x00af5f, 0x00af87, 0x00afaf, 0x00afd7, 0x00afff,
@@ -41,17 +42,20 @@
 X256W = 'x256w'
 X256 = [X232E, X232W, X256E, X256W]
 
 DIRNAME = os.path.dirname(__file__)
 
 RGB_X256 = dict()
 
-for i in X256:
-    with open(os.path.join(DIRNAME, i + '.bin'), 'rb') as f:
-        RGB_X256[i] =  [j for j in f.read()]
+with open(os.path.join(DIRNAME, 'x256.bin'), 'rb') as f:
+    data = zlib.decompress(f.read())
+    RGB_X256[X232E] = data[:0x1000000]
+    RGB_X256[X232W] = data[0x1000000:0x2000000]
+    RGB_X256[X256E] = data[0x2000000:0x3000000]
+    RGB_X256[X256W] = data[0x3000000:]
 
 
 def from_rgb(
     r: int, g: int = -1, b: int = -1,
     weighted: bool = False,
     n_color: int = 232
 ) -> int:
```

### Comparing `x256offline-0.0.2/src/x256offline.egg-info/PKG-INFO` & `x256offline-0.0.3/src/x256offline.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x256offline
-Version: 0.0.2
+Version: 0.0.3
 Summary: quickly find the nearest xterm 256 color index of an RGB
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2024 Elaina
```

