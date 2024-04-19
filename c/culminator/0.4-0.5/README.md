# Comparing `tmp/culminator-0.4.tar.gz` & `tmp/culminator-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "culminator-0.4.tar", last modified: Thu Apr 18 08:45:50 2024, max compression
+gzip compressed data, was "culminator-0.5.tar", last modified: Thu Apr 18 23:38:03 2024, max compression
```

## Comparing `culminator-0.4.tar` & `culminator-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 08:45:50.476888 culminator-0.4/
--rw-rw-rw-   0        0        0     3015 2024-04-18 08:45:50.475888 culminator-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2870 2024-04-18 08:42:42.000000 culminator-0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 08:45:50.463076 culminator-0.4/culminator/
--rw-rw-rw-   0        0        0      197 2024-04-18 04:27:17.000000 culminator-0.4/culminator/__init__.py
--rw-rw-rw-   0        0        0     4241 2024-04-18 07:59:37.000000 culminator-0.4/culminator/classification.py
--rw-rw-rw-   0        0        0     4743 2024-04-18 07:59:43.000000 culminator-0.4/culminator/clustering.py
--rw-rw-rw-   0        0        0     7456 2024-04-18 07:18:31.000000 culminator-0.4/culminator/regression.py
-drwxrwxrwx   0        0        0        0 2024-04-18 08:45:50.473876 culminator-0.4/culminator.egg-info/
--rw-rw-rw-   0        0        0     3015 2024-04-18 08:45:50.000000 culminator-0.4/culminator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-04-18 08:45:50.000000 culminator-0.4/culminator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 08:45:50.000000 culminator-0.4/culminator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 08:45:50.000000 culminator-0.4/culminator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-18 08:45:50.000000 culminator-0.4/culminator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 08:45:50.476888 culminator-0.4/setup.cfg
--rw-rw-rw-   0        0        0      352 2024-04-18 08:45:28.000000 culminator-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:38:03.456005 culminator-0.5/
+-rw-rw-rw-   0        0        0     3015 2024-04-18 23:38:03.455004 culminator-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2870 2024-04-18 08:42:42.000000 culminator-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 23:38:03.422613 culminator-0.5/culminator/
+-rw-rw-rw-   0        0        0       87 2024-04-18 23:36:58.000000 culminator-0.5/culminator/__init__.py
+-rw-rw-rw-   0        0        0     4241 2024-04-18 07:59:37.000000 culminator-0.5/culminator/classif.py
+-rw-rw-rw-   0        0        0     4743 2024-04-18 07:59:43.000000 culminator-0.5/culminator/clus.py
+-rw-rw-rw-   0        0        0     7456 2024-04-18 07:18:31.000000 culminator-0.5/culminator/reg.py
+drwxrwxrwx   0        0        0        0 2024-04-18 23:38:03.450895 culminator-0.5/culminator.egg-info/
+-rw-rw-rw-   0        0        0     3015 2024-04-18 23:38:03.000000 culminator-0.5/culminator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-04-18 23:38:03.000000 culminator-0.5/culminator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 23:38:03.000000 culminator-0.5/culminator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-18 23:38:03.000000 culminator-0.5/culminator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-18 23:38:03.000000 culminator-0.5/culminator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 23:38:03.456005 culminator-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      352 2024-04-18 23:37:47.000000 culminator-0.5/setup.py
```

### Comparing `culminator-0.4/PKG-INFO` & `culminator-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: culminator
-Version: 0.4
+Version: 0.5
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 
 # Culminator
 Culminator is a Python package designed to facilitate regression, classification, and clustering. It provides functionalities for data loading, preprocessing,  training, and predicting. This README file serves as a guide to understand and utilize the package effectively.
```

### Comparing `culminator-0.4/README.md` & `culminator-0.5/README.md`

 * *Files identical despite different names*

### Comparing `culminator-0.4/culminator/classification.py` & `culminator-0.5/culminator/classif.py`

 * *Files identical despite different names*

### Comparing `culminator-0.4/culminator/clustering.py` & `culminator-0.5/culminator/clus.py`

 * *Files identical despite different names*

### Comparing `culminator-0.4/culminator/regression.py` & `culminator-0.5/culminator/reg.py`

 * *Files identical despite different names*

### Comparing `culminator-0.4/culminator.egg-info/PKG-INFO` & `culminator-0.5/culminator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: culminator
-Version: 0.4
+Version: 0.5
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 
 # Culminator
 Culminator is a Python package designed to facilitate regression, classification, and clustering. It provides functionalities for data loading, preprocessing,  training, and predicting. This README file serves as a guide to understand and utilize the package effectively.
```

