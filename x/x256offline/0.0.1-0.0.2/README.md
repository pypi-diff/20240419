# Comparing `tmp/x256offline-0.0.1.tar.gz` & `tmp/x256offline-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x256offline-0.0.1.tar", last modified: Mon Apr 15 09:48:49 2024, max compression
+gzip compressed data, was "x256offline-0.0.2.tar", last modified: Fri Apr 19 13:18:18 2024, max compression
```

## Comparing `x256offline-0.0.1.tar` & `x256offline-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-15 09:48:49.761922 x256offline-0.0.1/
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)     1063 2024-04-14 13:47:56.000000 x256offline-0.0.1/LICENSE
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)     2380 2024-04-15 09:48:49.746452 x256offline-0.0.1/PKG-INFO
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)      520 2024-04-15 02:10:20.000000 x256offline-0.0.1/README.rst
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)      891 2024-04-15 02:02:00.000000 x256offline-0.0.1/pyproject.toml
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)       38 2024-04-15 09:48:49.762911 x256offline-0.0.1/setup.cfg
-drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-15 09:48:48.714839 x256offline-0.0.1/src/
-drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-15 09:48:49.573565 x256offline-0.0.1/src/x256offline/
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)       58 2024-04-15 02:26:52.000000 x256offline-0.0.1/src/x256offline/__init__.py
--rwxrwxrwx   0 elaina    (1000) elaina    (1000) 16777216 2024-04-15 01:15:37.000000 x256offline-0.0.1/src/x256offline/euclidean_distance.bin
--rwxrwxrwx   0 elaina    (1000) elaina    (1000) 16777216 2024-04-15 01:15:37.000000 x256offline-0.0.1/src/x256offline/weighted_euclidean_distance.bin
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)     3367 2024-04-15 01:30:57.000000 x256offline-0.0.1/src/x256offline/x256.py
-drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-15 09:48:49.727816 x256offline-0.0.1/src/x256offline.egg-info/
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)     2380 2024-04-15 09:48:48.000000 x256offline-0.0.1/src/x256offline.egg-info/PKG-INFO
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)      328 2024-04-15 09:48:48.000000 x256offline-0.0.1/src/x256offline.egg-info/SOURCES.txt
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)        1 2024-04-15 09:48:48.000000 x256offline-0.0.1/src/x256offline.egg-info/dependency_links.txt
--rwxrwxrwx   0 elaina    (1000) elaina    (1000)       12 2024-04-15 09:48:48.000000 x256offline-0.0.1/src/x256offline.egg-info/top_level.txt
+drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 13:18:18.339105 x256offline-0.0.2/
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)     1063 2024-04-14 13:47:56.000000 x256offline-0.0.2/LICENSE
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)     2380 2024-04-19 13:18:18.319035 x256offline-0.0.2/PKG-INFO
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)      520 2024-04-15 02:10:20.000000 x256offline-0.0.2/README.rst
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)      895 2024-04-17 13:58:08.000000 x256offline-0.0.2/pyproject.toml
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)       38 2024-04-19 13:18:18.340107 x256offline-0.0.2/setup.cfg
+drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 13:18:17.114005 x256offline-0.0.2/src/
+drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 13:18:17.687747 x256offline-0.0.2/src/x256offline/
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)       58 2024-04-17 12:55:05.000000 x256offline-0.0.2/src/x256offline/__init__.py
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)     3359 2024-04-17 12:36:48.000000 x256offline-0.0.2/src/x256offline/x256.py
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000) 16777216 2024-04-17 12:39:45.000000 x256offline-0.0.2/src/x256offline/x256e.bin
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000) 16777216 2024-04-17 12:39:45.000000 x256offline-0.0.2/src/x256offline/x256w.bin
+drwxrwxrwx   0 elaina    (1000) elaina    (1000)        0 2024-04-19 13:18:18.305085 x256offline-0.0.2/src/x256offline.egg-info/
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)     2380 2024-04-19 13:18:16.000000 x256offline-0.0.2/src/x256offline.egg-info/PKG-INFO
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)      293 2024-04-19 13:18:17.000000 x256offline-0.0.2/src/x256offline.egg-info/SOURCES.txt
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)        1 2024-04-19 13:18:16.000000 x256offline-0.0.2/src/x256offline.egg-info/dependency_links.txt
+-rwxrwxrwx   0 elaina    (1000) elaina    (1000)       12 2024-04-19 13:18:16.000000 x256offline-0.0.2/src/x256offline.egg-info/top_level.txt
```

### Comparing `x256offline-0.0.1/LICENSE` & `x256offline-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `x256offline-0.0.1/PKG-INFO` & `x256offline-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x256offline
-Version: 0.0.1
+Version: 0.0.2
 Summary: quickly find the nearest xterm 256 color index of an RGB
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2024 Elaina
```

### Comparing `x256offline-0.0.1/README.rst` & `x256offline-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `x256offline-0.0.1/pyproject.toml` & `x256offline-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "x256offline"
-version = "0.0.1"
+version = "0.0.2"
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
-package-data = {"x256offline" = ["*.bin"]}
+package-data = {"x256offline" = ["x256*.bin"]}
 
 [build-system]
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `x256offline-0.0.1/src/x256offline/euclidean_distance.bin` & `x256offline-0.0.2/src/x256offline/x256e.bin`

 * *Files identical despite different names*

### Comparing `x256offline-0.0.1/src/x256offline/weighted_euclidean_distance.bin` & `x256offline-0.0.2/src/x256offline/x256w.bin`

 * *Files identical despite different names*

### Comparing `x256offline-0.0.1/src/x256offline/x256.py` & `x256offline-0.0.2/src/x256offline/x256.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,31 +31,34 @@
     0xffaf87, 0xffafaf, 0xffafd7, 0xffafff, 0xffd700, 0xffd75f, 0xffd787, 0xffd7af,
     0xffd7d7, 0xffd7ff, 0xffff00, 0xffff5f, 0xffff87, 0xffffaf, 0xffffd7, 0xffffff,
     0x080808, 0x121212, 0x1c1c1c, 0x262626, 0x303030, 0x3a3a3a, 0x444444, 0x4e4e4e,
     0x585858, 0x606060, 0x666666, 0x767676, 0x808080, 0x8a8a8a, 0x949494, 0x9e9e9e,
     0xa8a8a8, 0xb2b2b2, 0xbcbcbc, 0xc6c6c6, 0xd0d0d0, 0xdadada, 0xe4e4e4, 0xeeeeee
 ]
 
-WED = 'weighted_euclidean_distance'
-ED = 'euclidean_distance'
+X232E = 'x232e'
+X232W = 'x232w'
+X256E = 'x256e'
+X256W = 'x256w'
+X256 = [X232E, X232W, X256E, X256W]
 
 DIRNAME = os.path.dirname(__file__)
 
-WED_BIN = os.path.join(DIRNAME, WED + '.bin')
-ED_BIN = os.path.join(DIRNAME, ED + '.bin')
-
 RGB_X256 = dict()
 
-with open(WED_BIN, 'rb') as f:
-    RGB_X256[WED] = [i for i in f.read()]
-
-with open(ED_BIN, 'rb') as f:
-    RGB_X256[ED] = [i for i in f.read()]
+for i in X256:
+    with open(os.path.join(DIRNAME, i + '.bin'), 'rb') as f:
+        RGB_X256[i] =  [j for j in f.read()]
 
 
-def from_rgb(r: int, g: int = -1, b: int = -1, weighted: bool = False) -> int:
+def from_rgb(
+    r: int, g: int = -1, b: int = -1,
+    weighted: bool = False,
+    n_color: int = 232
+) -> int:
     rgb = r if g == -1 else (r*0x10000 + g*0x100 + b)
-    return RGB_X256[WED if weighted else ED][rgb]
+    x = 'x%d%s' % (n_color, 'w' if weighted else 'e')
+    return RGB_X256[x][rgb]
 
 
 def to_rgb(x: int) -> int:
     return X256_RGB[x]
```

### Comparing `x256offline-0.0.1/src/x256offline.egg-info/PKG-INFO` & `x256offline-0.0.2/src/x256offline.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x256offline
-Version: 0.0.1
+Version: 0.0.2
 Summary: quickly find the nearest xterm 256 color index of an RGB
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2024 Elaina
```

