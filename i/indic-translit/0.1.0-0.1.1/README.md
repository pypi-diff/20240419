# Comparing `tmp/indic-translit-0.1.0.tar.gz` & `tmp/indic-translit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indic-translit-0.1.0.tar", last modified: Fri Apr 19 13:50:00 2024, max compression
+gzip compressed data, was "indic-translit-0.1.1.tar", last modified: Fri Apr 19 13:57:15 2024, max compression
```

## Comparing `indic-translit-0.1.0.tar` & `indic-translit-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 13:50:00.610030 indic-translit-0.1.0/
--rw-r--r--   0 chandana   (501) staff       (20)     1069 2024-04-19 08:08:03.000000 indic-translit-0.1.0/LICENSE
--rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 13:50:00.609832 indic-translit-0.1.0/PKG-INFO
--rw-r--r--   0 chandana   (501) staff       (20)     2936 2024-04-19 12:37:53.000000 indic-translit-0.1.0/README.md
-drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 13:50:00.609556 indic-translit-0.1.0/indic_translit.egg-info/
--rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 13:50:00.000000 indic-translit-0.1.0/indic_translit.egg-info/PKG-INFO
--rw-r--r--   0 chandana   (501) staff       (20)      178 2024-04-19 13:50:00.000000 indic-translit-0.1.0/indic_translit.egg-info/SOURCES.txt
--rw-r--r--   0 chandana   (501) staff       (20)        1 2024-04-19 13:50:00.000000 indic-translit-0.1.0/indic_translit.egg-info/dependency_links.txt
--rw-r--r--   0 chandana   (501) staff       (20)        9 2024-04-19 13:50:00.000000 indic-translit-0.1.0/indic_translit.egg-info/top_level.txt
--rw-r--r--   0 chandana   (501) staff       (20)       38 2024-04-19 13:50:00.610098 indic-translit-0.1.0/setup.cfg
--rw-r--r--   0 chandana   (501) staff       (20)     2698 2024-04-19 13:46:13.000000 indic-translit-0.1.0/setup.py
+drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 13:57:15.694793 indic-translit-0.1.1/
+-rw-r--r--   0 chandana   (501) staff       (20)     1069 2024-04-19 08:08:03.000000 indic-translit-0.1.1/LICENSE
+-rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 13:57:15.694376 indic-translit-0.1.1/PKG-INFO
+-rw-r--r--   0 chandana   (501) staff       (20)     2936 2024-04-19 12:37:53.000000 indic-translit-0.1.1/README.md
+drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 13:57:15.693793 indic-translit-0.1.1/indic_translit.egg-info/
+-rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 13:57:15.000000 indic-translit-0.1.1/indic_translit.egg-info/PKG-INFO
+-rw-r--r--   0 chandana   (501) staff       (20)      178 2024-04-19 13:57:15.000000 indic-translit-0.1.1/indic_translit.egg-info/SOURCES.txt
+-rw-r--r--   0 chandana   (501) staff       (20)        1 2024-04-19 13:57:15.000000 indic-translit-0.1.1/indic_translit.egg-info/dependency_links.txt
+-rw-r--r--   0 chandana   (501) staff       (20)       15 2024-04-19 13:57:15.000000 indic-translit-0.1.1/indic_translit.egg-info/top_level.txt
+-rw-r--r--   0 chandana   (501) staff       (20)       38 2024-04-19 13:57:15.694948 indic-translit-0.1.1/setup.cfg
+-rw-r--r--   0 chandana   (501) staff       (20)     2704 2024-04-19 13:54:34.000000 indic-translit-0.1.1/setup.py
```

### Comparing `indic-translit-0.1.0/LICENSE` & `indic-translit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `indic-translit-0.1.0/PKG-INFO` & `indic-translit-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indic-translit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transliterate to and from Indian languages. Currently supported Dravida languages - ಕతెമத.
 Home-page: https://github.com/Posterior-AI/dravida-transliterate
 Author: posteriorai
 Author-email: jaswanth@posterior.xyz
 License-File: LICENSE
```

### Comparing `indic-translit-0.1.0/README.md` & `indic-translit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `indic-translit-0.1.0/indic_translit.egg-info/PKG-INFO` & `indic-translit-0.1.1/indic_translit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indic-translit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transliterate to and from Indian languages. Currently supported Dravida languages - ಕతెമத.
 Home-page: https://github.com/Posterior-AI/dravida-transliterate
 Author: posteriorai
 Author-email: jaswanth@posterior.xyz
 License-File: LICENSE
```

### Comparing `indic-translit-0.1.0/setup.py` & `indic-translit-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-from translit import __version__
+from indic_translit import __version__
 
 setup(
     name='indic-translit',
     version=__version__,
 
     url='https://github.com/Posterior-AI/dravida-transliterate',
     owner="posteriorai",
```

