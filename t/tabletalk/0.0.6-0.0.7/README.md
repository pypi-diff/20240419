# Comparing `tmp/tabletalk-0.0.6.tar.gz` & `tmp/tabletalk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabletalk-0.0.6.tar", last modified: Fri Apr 19 20:03:18 2024, max compression
+gzip compressed data, was "tabletalk-0.0.7.tar", last modified: Fri Apr 19 20:16:35 2024, max compression
```

## Comparing `tabletalk-0.0.6.tar` & `tabletalk-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 20:03:18.529873 tabletalk-0.0.6/
--rw-r--r--   0 vinceberry   (501) staff       (20)     1045 2024-04-19 17:08:20.000000 tabletalk-0.0.6/LICENSE
--rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 20:03:18.529624 tabletalk-0.0.6/PKG-INFO
--rw-r--r--   0 vinceberry   (501) staff       (20)       12 2024-04-19 16:52:19.000000 tabletalk-0.0.6/README.md
--rw-r--r--   0 vinceberry   (501) staff       (20)       38 2024-04-19 20:03:18.529925 tabletalk-0.0.6/setup.cfg
--rw-r--r--   0 vinceberry   (501) staff       (20)     1154 2024-04-19 20:03:04.000000 tabletalk-0.0.6/setup.py
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 20:03:18.528454 tabletalk-0.0.6/tabletalk/
--rw-r--r--   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:08:20.000000 tabletalk-0.0.6/tabletalk/__init__.py
--rw-r--r--   0 vinceberry   (501) staff       (20)     3400 2024-04-19 19:55:39.000000 tabletalk-0.0.6/tabletalk/talk.py
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 20:03:18.529358 tabletalk-0.0.6/tabletalk.egg-info/
--rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 20:03:18.000000 tabletalk-0.0.6/tabletalk.egg-info/PKG-INFO
--rw-r--r--   0 vinceberry   (501) staff       (20)      230 2024-04-19 20:03:18.000000 tabletalk-0.0.6/tabletalk.egg-info/SOURCES.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)        1 2024-04-19 20:03:18.000000 tabletalk-0.0.6/tabletalk.egg-info/dependency_links.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)       25 2024-04-19 20:03:18.000000 tabletalk-0.0.6/tabletalk.egg-info/requires.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)       10 2024-04-19 20:03:18.000000 tabletalk-0.0.6/tabletalk.egg-info/top_level.txt
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 20:16:35.933337 tabletalk-0.0.7/
+-rw-r--r--   0 vinceberry   (501) staff       (20)     1045 2024-04-19 17:08:20.000000 tabletalk-0.0.7/LICENSE
+-rw-r--r--   0 vinceberry   (501) staff       (20)      688 2024-04-19 20:16:35.933103 tabletalk-0.0.7/PKG-INFO
+-rw-r--r--   0 vinceberry   (501) staff       (20)       12 2024-04-19 16:52:19.000000 tabletalk-0.0.7/README.md
+-rw-r--r--   0 vinceberry   (501) staff       (20)       38 2024-04-19 20:16:35.933384 tabletalk-0.0.7/setup.cfg
+-rw-r--r--   0 vinceberry   (501) staff       (20)     1182 2024-04-19 20:15:30.000000 tabletalk-0.0.7/setup.py
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 20:16:35.931895 tabletalk-0.0.7/tabletalk/
+-rw-r--r--   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:08:20.000000 tabletalk-0.0.7/tabletalk/__init__.py
+-rw-r--r--   0 vinceberry   (501) staff       (20)     3400 2024-04-19 19:55:39.000000 tabletalk-0.0.7/tabletalk/talk.py
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 20:16:35.932867 tabletalk-0.0.7/tabletalk.egg-info/
+-rw-r--r--   0 vinceberry   (501) staff       (20)      688 2024-04-19 20:16:35.000000 tabletalk-0.0.7/tabletalk.egg-info/PKG-INFO
+-rw-r--r--   0 vinceberry   (501) staff       (20)      230 2024-04-19 20:16:35.000000 tabletalk-0.0.7/tabletalk.egg-info/SOURCES.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)        1 2024-04-19 20:16:35.000000 tabletalk-0.0.7/tabletalk.egg-info/dependency_links.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)       25 2024-04-19 20:16:35.000000 tabletalk-0.0.7/tabletalk.egg-info/requires.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)       10 2024-04-19 20:16:35.000000 tabletalk-0.0.7/tabletalk.egg-info/top_level.txt
```

### Comparing `tabletalk-0.0.6/LICENSE` & `tabletalk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tabletalk-0.0.6/PKG-INFO` & `tabletalk-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: tabletalk
-Version: 0.0.6
+Version: 0.0.7
 Summary: NL2SQL2RAG
 Author: Vince Berry
 Author-email: vincent.berry11@gmail.com
+License: proprietary
 Keywords: nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `tabletalk-0.0.6/tabletalk/talk.py` & `tabletalk-0.0.7/tabletalk/talk.py`

 * *Files identical despite different names*

### Comparing `tabletalk-0.0.6/tabletalk.egg-info/PKG-INFO` & `tabletalk-0.0.7/tabletalk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: tabletalk
-Version: 0.0.6
+Version: 0.0.7
 Summary: NL2SQL2RAG
 Author: Vince Berry
 Author-email: vincent.berry11@gmail.com
+License: proprietary
 Keywords: nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

