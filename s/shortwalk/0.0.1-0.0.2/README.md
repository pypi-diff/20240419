# Comparing `tmp/shortwalk-0.0.1.tar.gz` & `tmp/shortwalk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortwalk-0.0.1.tar", last modified: Thu Apr 18 14:46:23 2024, max compression
+gzip compressed data, was "shortwalk-0.0.2.tar", last modified: Fri Apr 19 15:30:07 2024, max compression
```

## Comparing `shortwalk-0.0.1.tar` & `shortwalk-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 14:46:23.952189 shortwalk-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-04-18 14:44:29.000000 shortwalk-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      277 2024-04-18 14:46:23.949197 shortwalk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-18 14:46:23.952508 shortwalk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      668 2024-04-18 13:53:33.000000 shortwalk-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:46:23.919274 shortwalk-0.0.1/shortwalk/
--rw-rw-rw-   0        0        0     2044 2024-04-18 13:41:12.000000 shortwalk-0.0.1/shortwalk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:46:23.946202 shortwalk-0.0.1/shortwalk.egg-info/
--rw-rw-rw-   0        0        0      277 2024-04-18 14:46:23.000000 shortwalk-0.0.1/shortwalk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2024-04-18 14:46:23.000000 shortwalk-0.0.1/shortwalk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 14:46:23.000000 shortwalk-0.0.1/shortwalk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 14:46:23.000000 shortwalk-0.0.1/shortwalk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 15:30:07.109231 shortwalk-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-18 14:44:29.000000 shortwalk-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      277 2024-04-19 15:30:07.103250 shortwalk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-19 15:30:07.110283 shortwalk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      668 2024-04-19 15:27:07.000000 shortwalk-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:30:07.041279 shortwalk-0.0.2/shortwalk/
+-rw-rw-rw-   0        0        0     2044 2024-04-19 11:11:12.000000 shortwalk-0.0.2/shortwalk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:30:07.099261 shortwalk-0.0.2/shortwalk.egg-info/
+-rw-rw-rw-   0        0        0      277 2024-04-19 15:30:05.000000 shortwalk-0.0.2/shortwalk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2024-04-19 15:30:06.000000 shortwalk-0.0.2/shortwalk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 15:30:05.000000 shortwalk-0.0.2/shortwalk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 15:30:05.000000 shortwalk-0.0.2/shortwalk.egg-info/top_level.txt
```

### Comparing `shortwalk-0.0.1/LICENSE` & `shortwalk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shortwalk-0.0.1/setup.py` & `shortwalk-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         long_description = f.read()
 except FileNotFoundError:
     long_description = ''
 
 setup(
     packages = find_packages(),
     name = 'shortwalk',
-    version='0.0.1',
+    version='0.0.2',
     author="Stanislav Doronin",
     author_email="mugisbrows@gmail.com",
     url='https://github.com/mugiseyebrows/shortwalk',
     description='os.walk with maxdepth option',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     install_requires = []
```

### Comparing `shortwalk-0.0.1/shortwalk/__init__.py` & `shortwalk-0.0.2/shortwalk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 def walk(top, maxdepth=0, topdown=True, onerror=None, followlinks=False):
-    return _walk(os.fspath(top), topdown, onerror, followlinks, maxdepth)
+    return _walk(os.fspath(top), maxdepth, topdown, onerror, followlinks)
 
 def _walk(top, maxdepth, topdown, onerror, followlinks):
     dirs = []
     nondirs = []
     walk_dirs = []
     try:
         scandir_it = os.scandir(top)
@@ -57,12 +57,12 @@
         yield top, dirs, nondirs
         if maxdepth == 0:
             return
         islink, join = os.path.islink, os.path.join
         for dirname in dirs:
             new_path = join(top, dirname)
             if followlinks or not islink(new_path):
-                yield from _walk(new_path, topdown, onerror, followlinks, maxdepth)
+                yield from _walk(new_path, maxdepth, topdown, onerror, followlinks)
     else:
         for new_path in walk_dirs:
-            yield from _walk(new_path, topdown, onerror, followlinks, maxdepth)
+            yield from _walk(new_path, maxdepth, topdown, onerror, followlinks)
         yield top, dirs, nondirs
```

