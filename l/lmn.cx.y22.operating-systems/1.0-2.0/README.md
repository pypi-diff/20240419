# Comparing `tmp/lmn_cx_y22_operating_systems-1.0.tar.gz` & `tmp/lmn_cx_y22_operating_systems-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmn_cx_y22_operating_systems-1.0.tar", last modified: Thu Apr 18 00:48:09 2024, max compression
+gzip compressed data, was "lmn_cx_y22_operating_systems-2.0.tar", last modified: Fri Apr 19 01:10:02 2024, max compression
```

## Comparing `lmn_cx_y22_operating_systems-1.0.tar` & `lmn_cx_y22_operating_systems-2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 00:48:09.626481 lmn_cx_y22_operating_systems-1.0/
--rw-rw-rw-   0        0        0     3383 2024-04-17 15:36:16.000000 lmn_cx_y22_operating_systems-1.0/.gitignore
--rw-rw-rw-   0        0        0      761 2024-04-17 23:30:48.000000 lmn_cx_y22_operating_systems-1.0/COPYING
--rw-rw-rw-   0        0        0      681 2024-04-17 23:51:44.000000 lmn_cx_y22_operating_systems-1.0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-18 00:48:09.578986 lmn_cx_y22_operating_systems-1.0/LICENSES/
--rw-rw-rw-   0        0        0      656 2024-04-17 23:47:39.000000 lmn_cx_y22_operating_systems-1.0/LICENSES/0BSD.txt
--rw-rw-rw-   0        0        0    11558 2024-04-17 14:21:46.000000 lmn_cx_y22_operating_systems-1.0/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0        0        0     7169 2024-04-17 15:09:19.000000 lmn_cx_y22_operating_systems-1.0/LICENSES/CC0-1.0.txt
--rw-rw-rw-   0        0        0     1099 2024-04-17 20:35:00.000000 lmn_cx_y22_operating_systems-1.0/LICENSES/MIT.txt
--rw-rw-rw-   0        0        0     1045 2024-04-18 00:48:09.626481 lmn_cx_y22_operating_systems-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      123 2024-04-17 15:35:59.000000 lmn_cx_y22_operating_systems-1.0/README.md
--rw-rw-rw-   0        0        0     1397 2024-04-17 23:39:05.000000 lmn_cx_y22_operating_systems-1.0/REUSE
--rw-rw-rw-   0        0        0     1771 2024-04-17 23:44:16.000000 lmn_cx_y22_operating_systems-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 00:48:09.626481 lmn_cx_y22_operating_systems-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 00:48:09.532628 lmn_cx_y22_operating_systems-1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 00:48:09.532628 lmn_cx_y22_operating_systems-1.0/src/lmn/
-drwxrwxrwx   0        0        0        0 2024-04-18 00:48:09.547526 lmn_cx_y22_operating_systems-1.0/src/lmn/cx/
-drwxrwxrwx   0        0        0        0 2024-04-18 00:48:09.547526 lmn_cx_y22_operating_systems-1.0/src/lmn/cx/y22/
-drwxrwxrwx   0        0        0        0 2024-04-18 00:48:09.610841 lmn_cx_y22_operating_systems-1.0/src/lmn/cx/y22/operating_systems/
--rw-rw-rw-   0        0        0      313 2024-04-18 00:33:46.000000 lmn_cx_y22_operating_systems-1.0/src/lmn/cx/y22/operating_systems/__init__.py
--rw-rw-rw-   0        0        0     2261 2024-04-18 00:34:23.000000 lmn_cx_y22_operating_systems-1.0/src/lmn/cx/y22/operating_systems/_operating_systems.py
-drwxrwxrwx   0        0        0        0 2024-04-18 00:48:09.610841 lmn_cx_y22_operating_systems-1.0/src/lmn.cx.y22.operating_systems.egg-info/
--rw-rw-rw-   0        0        0     1045 2024-04-18 00:48:09.000000 lmn_cx_y22_operating_systems-1.0/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2024-04-18 00:48:09.000000 lmn_cx_y22_operating_systems-1.0/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 00:48:09.000000 lmn_cx_y22_operating_systems-1.0/src/lmn.cx.y22.operating_systems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2024-04-18 00:48:09.000000 lmn_cx_y22_operating_systems-1.0/src/lmn.cx.y22.operating_systems.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-18 00:48:09.000000 lmn_cx_y22_operating_systems-1.0/src/lmn.cx.y22.operating_systems.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.678043 lmn_cx_y22_operating_systems-2.0/
+-rw-rw-rw-   0        0        0     3383 2024-04-17 15:36:16.000000 lmn_cx_y22_operating_systems-2.0/.gitignore
+-rw-rw-rw-   0        0        0      761 2024-04-17 23:30:48.000000 lmn_cx_y22_operating_systems-2.0/COPYING
+-rw-rw-rw-   0        0        0      681 2024-04-17 23:51:44.000000 lmn_cx_y22_operating_systems-2.0/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.649825 lmn_cx_y22_operating_systems-2.0/LICENSES/
+-rw-rw-rw-   0        0        0      656 2024-04-17 23:47:39.000000 lmn_cx_y22_operating_systems-2.0/LICENSES/0BSD.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-17 14:21:46.000000 lmn_cx_y22_operating_systems-2.0/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0        0        0     7169 2024-04-17 15:09:19.000000 lmn_cx_y22_operating_systems-2.0/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0        0        0     1099 2024-04-17 20:35:00.000000 lmn_cx_y22_operating_systems-2.0/LICENSES/MIT.txt
+-rw-rw-rw-   0        0        0     1045 2024-04-19 01:10:02.674028 lmn_cx_y22_operating_systems-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2024-04-17 15:35:59.000000 lmn_cx_y22_operating_systems-2.0/README.md
+-rw-rw-rw-   0        0        0     1397 2024-04-17 23:39:05.000000 lmn_cx_y22_operating_systems-2.0/REUSE
+-rw-rw-rw-   0        0        0     1771 2024-04-17 23:44:16.000000 lmn_cx_y22_operating_systems-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 01:10:02.678043 lmn_cx_y22_operating_systems-2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.545975 lmn_cx_y22_operating_systems-2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.545975 lmn_cx_y22_operating_systems-2.0/src/lmn/
+drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.545975 lmn_cx_y22_operating_systems-2.0/src/lmn/cx/
+drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.550404 lmn_cx_y22_operating_systems-2.0/src/lmn/cx/y22/
+drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.672017 lmn_cx_y22_operating_systems-2.0/src/lmn/cx/y22/operating_systems/
+-rw-rw-rw-   0        0        0      313 2024-04-18 00:33:46.000000 lmn_cx_y22_operating_systems-2.0/src/lmn/cx/y22/operating_systems/__init__.py
+-rw-rw-rw-   0        0        0     2907 2024-04-19 01:08:37.000000 lmn_cx_y22_operating_systems-2.0/src/lmn/cx/y22/operating_systems/_operating_systems.py
+drwxrwxrwx   0        0        0        0 2024-04-19 01:10:02.674028 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/
+-rw-rw-rw-   0        0        0     1045 2024-04-19 01:10:02.000000 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2024-04-19 01:10:02.000000 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 01:10:02.000000 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2024-04-19 01:10:02.000000 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-19 01:10:02.000000 lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/top_level.txt
```

### Comparing `lmn_cx_y22_operating_systems-1.0/.gitignore` & `lmn_cx_y22_operating_systems-2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-1.0/COPYING` & `lmn_cx_y22_operating_systems-2.0/COPYING`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-1.0/LICENSE` & `lmn_cx_y22_operating_systems-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-1.0/LICENSES/0BSD.txt` & `lmn_cx_y22_operating_systems-2.0/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-1.0/LICENSES/Apache-2.0.txt` & `lmn_cx_y22_operating_systems-2.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-1.0/LICENSES/CC0-1.0.txt` & `lmn_cx_y22_operating_systems-2.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-1.0/LICENSES/MIT.txt` & `lmn_cx_y22_operating_systems-2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-1.0/PKG-INFO` & `lmn_cx_y22_operating_systems-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmn.cx.y22.operating_systems
-Version: 1.0
+Version: 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zero-Clause BSD (0BSD)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `lmn_cx_y22_operating_systems-1.0/REUSE` & `lmn_cx_y22_operating_systems-2.0/REUSE`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-1.0/pyproject.toml` & `lmn_cx_y22_operating_systems-2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lmn_cx_y22_operating_systems-1.0/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO` & `lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmn.cx.y22.operating_systems
-Version: 1.0
+Version: 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Zero-Clause BSD (0BSD)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `lmn_cx_y22_operating_systems-1.0/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt` & `lmn_cx_y22_operating_systems-2.0/src/lmn.cx.y22.operating_systems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

