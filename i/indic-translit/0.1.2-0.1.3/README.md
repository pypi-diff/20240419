# Comparing `tmp/indic-translit-0.1.2.tar.gz` & `tmp/indic_translit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indic-translit-0.1.2.tar", last modified: Fri Apr 19 13:59:07 2024, max compression
+gzip compressed data, was "indic_translit-0.1.3.tar", last modified: Fri Apr 19 14:31:47 2024, max compression
```

## Comparing `indic-translit-0.1.2.tar` & `indic_translit-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 13:59:07.645221 indic-translit-0.1.2/
--rw-r--r--   0 chandana   (501) staff       (20)     1069 2024-04-19 08:08:03.000000 indic-translit-0.1.2/LICENSE
--rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 13:59:07.644883 indic-translit-0.1.2/PKG-INFO
--rw-r--r--   0 chandana   (501) staff       (20)     2936 2024-04-19 12:37:53.000000 indic-translit-0.1.2/README.md
-drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 13:59:07.644400 indic-translit-0.1.2/indic_translit.egg-info/
--rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 13:59:07.000000 indic-translit-0.1.2/indic_translit.egg-info/PKG-INFO
--rw-r--r--   0 chandana   (501) staff       (20)      178 2024-04-19 13:59:07.000000 indic-translit-0.1.2/indic_translit.egg-info/SOURCES.txt
--rw-r--r--   0 chandana   (501) staff       (20)        1 2024-04-19 13:59:07.000000 indic-translit-0.1.2/indic_translit.egg-info/dependency_links.txt
--rw-r--r--   0 chandana   (501) staff       (20)       15 2024-04-19 13:59:07.000000 indic-translit-0.1.2/indic_translit.egg-info/top_level.txt
--rw-r--r--   0 chandana   (501) staff       (20)       38 2024-04-19 13:59:07.645334 indic-translit-0.1.2/setup.cfg
--rw-r--r--   0 chandana   (501) staff       (20)     2704 2024-04-19 13:58:09.000000 indic-translit-0.1.2/setup.py
+drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 14:31:47.485735 indic_translit-0.1.3/
+-rw-r--r--   0 chandana   (501) staff       (20)     1069 2024-04-19 08:08:03.000000 indic_translit-0.1.3/LICENSE
+-rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 14:31:47.485343 indic_translit-0.1.3/PKG-INFO
+-rw-r--r--   0 chandana   (501) staff       (20)     2936 2024-04-19 12:37:53.000000 indic_translit-0.1.3/README.md
+drwxr-xr-x   0 chandana   (501) staff       (20)        0 2024-04-19 14:31:47.484912 indic_translit-0.1.3/indic_translit.egg-info/
+-rw-r--r--   0 chandana   (501) staff       (20)     2530 2024-04-19 14:31:47.000000 indic_translit-0.1.3/indic_translit.egg-info/PKG-INFO
+-rw-r--r--   0 chandana   (501) staff       (20)      178 2024-04-19 14:31:47.000000 indic_translit-0.1.3/indic_translit.egg-info/SOURCES.txt
+-rw-r--r--   0 chandana   (501) staff       (20)        1 2024-04-19 14:31:47.000000 indic_translit-0.1.3/indic_translit.egg-info/dependency_links.txt
+-rw-r--r--   0 chandana   (501) staff       (20)       15 2024-04-19 14:31:47.000000 indic_translit-0.1.3/indic_translit.egg-info/top_level.txt
+-rw-r--r--   0 chandana   (501) staff       (20)       38 2024-04-19 14:31:47.485858 indic_translit-0.1.3/setup.cfg
+-rw-r--r--   0 chandana   (501) staff       (20)     2703 2024-04-19 14:09:56.000000 indic_translit-0.1.3/setup.py
```

### Comparing `indic-translit-0.1.2/LICENSE` & `indic_translit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indic-translit-0.1.2/PKG-INFO` & `indic_translit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: indic-translit
-Version: 0.1.2
+Name: indic_translit
+Version: 0.1.3
 Summary: Transliterate to and from Indian languages. Currently supported Dravida languages - ಕతెമத.
 Home-page: https://github.com/Posterior-AI/dravida-transliterate
 Author: posteriorai
 Author-email: jaswanth@posterior.xyz
 License-File: LICENSE
```

### Comparing `indic-translit-0.1.2/README.md` & `indic_translit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `indic-translit-0.1.2/indic_translit.egg-info/PKG-INFO` & `indic_translit-0.1.3/indic_translit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indic-translit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Transliterate to and from Indian languages. Currently supported Dravida languages - ಕతెമத.
 Home-page: https://github.com/Posterior-AI/dravida-transliterate
 Author: posteriorai
 Author-email: jaswanth@posterior.xyz
 License-File: LICENSE
```

### Comparing `indic-translit-0.1.2/setup.py` & `indic_translit-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 from indic_translit import __version__
 
 setup(
-    name='indic-translit',
+    name='indic_translit',
     version=__version__,
 
     url='https://github.com/Posterior-AI/dravida-transliterate',
     owner="posteriorai",
     author='posteriorai',
     author_email='jaswanth@posterior.xyz',
     description="Transliterate to and from Indian languages. Currently supported Dravida languages - ಕతెമத.",
@@ -71,9 +71,9 @@
 
 License
 -------
 
 MIT
 """,
 
-    py_modules=find_packages(),
+    py_modules=find_packages()
 )
```

