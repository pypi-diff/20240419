# Comparing `tmp/indic-translit-0.1.1.tar.gz` & `tmp/indic-translit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indic-translit-0.1.1.tar", last modified: Fri Apr 19 13:57:15 2024, max compression
+gzip compressed data, was "indic-translit-0.1.2.tar", last modified: Fri Apr 19 13:59:07 2024, max compression
```

## Comparing `indic-translit-0.1.1.tar` & `indic-translit-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 13:57:15.694793 indic-translit-0.1.1/
--rw-r--r--   0 chandana   (501) staff       (20)     1069 2024-04-19 08:08:03.000000 indic-translit-0.1.1/LICENSE
--rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 13:57:15.694376 indic-translit-0.1.1/PKG-INFO
--rw-r--r--   0 chandana   (501) staff       (20)     2936 2024-04-19 12:37:53.000000 indic-translit-0.1.1/README.md
-drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 13:57:15.693793 indic-translit-0.1.1/indic_translit.egg-info/
--rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 13:57:15.000000 indic-translit-0.1.1/indic_translit.egg-info/PKG-INFO
--rw-r--r--   0 chandana   (501) staff       (20)      178 2024-04-19 13:57:15.000000 indic-translit-0.1.1/indic_translit.egg-info/SOURCES.txt
--rw-r--r--   0 chandana   (501) staff       (20)        1 2024-04-19 13:57:15.000000 indic-translit-0.1.1/indic_translit.egg-info/dependency_links.txt
--rw-r--r--   0 chandana   (501) staff       (20)       15 2024-04-19 13:57:15.000000 indic-translit-0.1.1/indic_translit.egg-info/top_level.txt
--rw-r--r--   0 chandana   (501) staff       (20)       38 2024-04-19 13:57:15.694948 indic-translit-0.1.1/setup.cfg
--rw-r--r--   0 chandana   (501) staff       (20)     2704 2024-04-19 13:54:34.000000 indic-translit-0.1.1/setup.py
+drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 13:59:07.645221 indic-translit-0.1.2/
+-rw-r--r--   0 chandana   (501) staff       (20)     1069 2024-04-19 08:08:03.000000 indic-translit-0.1.2/LICENSE
+-rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 13:59:07.644883 indic-translit-0.1.2/PKG-INFO
+-rw-r--r--   0 chandana   (501) staff       (20)     2936 2024-04-19 12:37:53.000000 indic-translit-0.1.2/README.md
+drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 13:59:07.644400 indic-translit-0.1.2/indic_translit.egg-info/
+-rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 13:59:07.000000 indic-translit-0.1.2/indic_translit.egg-info/PKG-INFO
+-rw-r--r--   0 chandana   (501) staff       (20)      178 2024-04-19 13:59:07.000000 indic-translit-0.1.2/indic_translit.egg-info/SOURCES.txt
+-rw-r--r--   0 chandana   (501) staff       (20)        1 2024-04-19 13:59:07.000000 indic-translit-0.1.2/indic_translit.egg-info/dependency_links.txt
+-rw-r--r--   0 chandana   (501) staff       (20)       15 2024-04-19 13:59:07.000000 indic-translit-0.1.2/indic_translit.egg-info/top_level.txt
+-rw-r--r--   0 chandana   (501) staff       (20)       38 2024-04-19 13:59:07.645334 indic-translit-0.1.2/setup.cfg
+-rw-r--r--   0 chandana   (501) staff       (20)     2704 2024-04-19 13:58:09.000000 indic-translit-0.1.2/setup.py
```

### Comparing `indic-translit-0.1.1/LICENSE` & `indic-translit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indic-translit-0.1.1/PKG-INFO` & `indic-translit-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indic-translit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transliterate to and from Indian languages. Currently supported Dravida languages - ಕతెമத.
 Home-page: https://github.com/Posterior-AI/dravida-transliterate
 Author: posteriorai
 Author-email: jaswanth@posterior.xyz
 License-File: LICENSE
```

### Comparing `indic-translit-0.1.1/README.md` & `indic-translit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `indic-translit-0.1.1/indic_translit.egg-info/PKG-INFO` & `indic-translit-0.1.2/indic_translit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indic-translit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transliterate to and from Indian languages. Currently supported Dravida languages - ಕతెമத.
 Home-page: https://github.com/Posterior-AI/dravida-transliterate
 Author: posteriorai
 Author-email: jaswanth@posterior.xyz
 License-File: LICENSE
```

### Comparing `indic-translit-0.1.1/setup.py` & `indic-translit-0.1.2/setup.py`

 * *Files identical despite different names*

