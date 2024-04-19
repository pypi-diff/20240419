# Comparing `tmp/tabletalk-0.0.2.tar.gz` & `tmp/tabletalk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabletalk-0.0.2.tar", last modified: Fri Apr 19 17:37:27 2024, max compression
+gzip compressed data, was "tabletalk-0.0.3.tar", last modified: Fri Apr 19 17:49:08 2024, max compression
```

## Comparing `tabletalk-0.0.2.tar` & `tabletalk-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:37:27.860997 tabletalk-0.0.2/
--rw-r--r--   0 vinceberry   (501) staff       (20)     1045 2024-04-19 17:08:20.000000 tabletalk-0.0.2/LICENSE
--rw-r--r--   0 vinceberry   (501) staff       (20)      597 2024-04-19 17:37:27.860792 tabletalk-0.0.2/PKG-INFO
--rw-r--r--   0 vinceberry   (501) staff       (20)       12 2024-04-19 16:52:19.000000 tabletalk-0.0.2/README.md
--rw-r--r--   0 vinceberry   (501) staff       (20)       38 2024-04-19 17:37:27.861039 tabletalk-0.0.2/setup.cfg
--rw-r--r--   0 vinceberry   (501) staff       (20)     1122 2024-04-19 17:33:36.000000 tabletalk-0.0.2/setup.py
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:37:27.859931 tabletalk-0.0.2/tabletalk/
--rw-r--r--   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:08:20.000000 tabletalk-0.0.2/tabletalk/__init__.py
--rw-r--r--   0 vinceberry   (501) staff       (20)     2805 2024-04-19 17:08:20.000000 tabletalk-0.0.2/tabletalk/talk.py
-drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:37:27.860616 tabletalk-0.0.2/tabletalk.egg-info/
--rw-r--r--   0 vinceberry   (501) staff       (20)      597 2024-04-19 17:37:27.000000 tabletalk-0.0.2/tabletalk.egg-info/PKG-INFO
--rw-r--r--   0 vinceberry   (501) staff       (20)      198 2024-04-19 17:37:27.000000 tabletalk-0.0.2/tabletalk.egg-info/SOURCES.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)        1 2024-04-19 17:37:27.000000 tabletalk-0.0.2/tabletalk.egg-info/dependency_links.txt
--rw-r--r--   0 vinceberry   (501) staff       (20)       10 2024-04-19 17:37:27.000000 tabletalk-0.0.2/tabletalk.egg-info/top_level.txt
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:49:08.865501 tabletalk-0.0.3/
+-rw-r--r--   0 vinceberry   (501) staff       (20)     1045 2024-04-19 17:08:20.000000 tabletalk-0.0.3/LICENSE
+-rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 17:49:08.865281 tabletalk-0.0.3/PKG-INFO
+-rw-r--r--   0 vinceberry   (501) staff       (20)       12 2024-04-19 16:52:19.000000 tabletalk-0.0.3/README.md
+-rw-r--r--   0 vinceberry   (501) staff       (20)       38 2024-04-19 17:49:08.865545 tabletalk-0.0.3/setup.cfg
+-rw-r--r--   0 vinceberry   (501) staff       (20)     1154 2024-04-19 17:47:19.000000 tabletalk-0.0.3/setup.py
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:49:08.864228 tabletalk-0.0.3/tabletalk/
+-rw-r--r--   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:08:20.000000 tabletalk-0.0.3/tabletalk/__init__.py
+-rw-r--r--   0 vinceberry   (501) staff       (20)     2805 2024-04-19 17:08:20.000000 tabletalk-0.0.3/tabletalk/talk.py
+drwxr-xr-x   0 vinceberry   (501) staff       (20)        0 2024-04-19 17:49:08.865041 tabletalk-0.0.3/tabletalk.egg-info/
+-rw-r--r--   0 vinceberry   (501) staff       (20)      667 2024-04-19 17:49:08.000000 tabletalk-0.0.3/tabletalk.egg-info/PKG-INFO
+-rw-r--r--   0 vinceberry   (501) staff       (20)      230 2024-04-19 17:49:08.000000 tabletalk-0.0.3/tabletalk.egg-info/SOURCES.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)        1 2024-04-19 17:49:08.000000 tabletalk-0.0.3/tabletalk.egg-info/dependency_links.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)       25 2024-04-19 17:49:08.000000 tabletalk-0.0.3/tabletalk.egg-info/requires.txt
+-rw-r--r--   0 vinceberry   (501) staff       (20)       10 2024-04-19 17:49:08.000000 tabletalk-0.0.3/tabletalk.egg-info/top_level.txt
```

### Comparing `tabletalk-0.0.2/LICENSE` & `tabletalk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tabletalk-0.0.2/PKG-INFO` & `tabletalk-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: tabletalk
-Version: 0.0.2
+Version: 0.0.3
 Summary: NL2SQL2RAG
 Author: Vince Berry
 Author-email: vincent.berry11@gmail.com
 Keywords: nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: sqlalchemy
+Requires-Dist: pandas
+Requires-Dist: openai
 
 
 # tabletalk
```

### Comparing `tabletalk-0.0.2/setup.py` & `tabletalk-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'NL2SQL2RAG'
 LONG_DESCRIPTION = 'TableTalk allows you ask query your tabular data with natural language, then produces a generated response.'
 
 setup(
     name="tabletalk",
     version=VERSION,
     author="Vince Berry",
     author_email="vincent.berry11@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=[],
+    install_requires=['sqlalchemy', 'pandas', 'openai'],
     keywords=['nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `tabletalk-0.0.2/tabletalk/talk.py` & `tabletalk-0.0.3/tabletalk/talk.py`

 * *Files identical despite different names*

### Comparing `tabletalk-0.0.2/tabletalk.egg-info/PKG-INFO` & `tabletalk-0.0.3/tabletalk.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: tabletalk
-Version: 0.0.2
+Version: 0.0.3
 Summary: NL2SQL2RAG
 Author: Vince Berry
 Author-email: vincent.berry11@gmail.com
 Keywords: nlp, rag, sql, natural language processing, table, tabular data, query, natural language, tabletalk
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: sqlalchemy
+Requires-Dist: pandas
+Requires-Dist: openai
 
 
 # tabletalk
```

