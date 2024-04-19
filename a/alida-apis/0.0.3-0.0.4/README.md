# Comparing `tmp/alida-apis-0.0.3.tar.gz` & `tmp/alida-apis-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alida-apis-0.0.3.tar", last modified: Tue Apr 16 16:19:53 2024, max compression
+gzip compressed data, was "dist/alida-apis-0.0.4.tar", last modified: Fri Apr 19 14:35:30 2024, max compression
```

## Comparing `alida-apis-0.0.3.tar` & `alida-apis-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:19:53.136446 alida-apis-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-16 16:19:53.136446 alida-apis-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-16 16:19:43.000000 alida-apis-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:19:53.135446 alida-apis-0.0.3/alida_apis.egg-info/
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-16 16:19:53.000000 alida-apis-0.0.3/alida_apis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      281 2024-04-16 16:19:53.000000 alida-apis-0.0.3/alida_apis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 16:19:53.000000 alida-apis-0.0.3/alida_apis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-16 16:19:53.000000 alida-apis-0.0.3/alida_apis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-16 16:19:53.000000 alida-apis-0.0.3/alida_apis.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:19:53.136446 alida-apis-0.0.3/alidaapis/
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-16 16:19:43.000000 alida-apis-0.0.3/alidaapis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10329 2024-04-16 16:19:43.000000 alida-apis-0.0.3/alidaapis/apis.py
--rw-rw-rw-   0 root         (0) root         (0)     4951 2024-04-16 16:19:43.000000 alida-apis-0.0.3/alidaapis/minio_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-16 16:19:43.000000 alida-apis-0.0.3/alidaapis/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-16 16:19:53.136446 alida-apis-0.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-04-16 16:19:43.000000 alida-apis-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:35:30.391206 alida-apis-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-19 14:35:30.391206 alida-apis-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-19 14:35:20.000000 alida-apis-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:35:30.391206 alida-apis-0.0.4/alida_apis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-19 14:35:30.000000 alida-apis-0.0.4/alida_apis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      364 2024-04-19 14:35:30.000000 alida-apis-0.0.4/alida_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 14:35:30.000000 alida-apis-0.0.4/alida_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-19 14:35:30.000000 alida-apis-0.0.4/alida_apis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-19 14:35:30.000000 alida-apis-0.0.4/alida_apis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:35:30.391206 alida-apis-0.0.4/alidaapis/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-19 14:35:20.000000 alida-apis-0.0.4/alidaapis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2024-04-19 14:35:20.000000 alida-apis-0.0.4/alidaapis/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2024-04-19 14:35:20.000000 alida-apis-0.0.4/alidaapis/bda.py
+-rw-rw-rw-   0 root         (0) root         (0)     4441 2024-04-19 14:35:20.000000 alida-apis-0.0.4/alidaapis/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-19 14:35:20.000000 alida-apis-0.0.4/alidaapis/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     4951 2024-04-19 14:35:20.000000 alida-apis-0.0.4/alidaapis/minio_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-04-19 14:35:20.000000 alida-apis-0.0.4/alidaapis/service.py
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-19 14:35:20.000000 alida-apis-0.0.4/alidaapis/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-04-19 14:35:30.392206 alida-apis-0.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-04-19 14:35:20.000000 alida-apis-0.0.4/setup.py
```

### Comparing `alida-apis-0.0.3/alidaapis/minio_utils.py` & `alida-apis-0.0.4/alidaapis/minio_utils.py`

 * *Files identical despite different names*

### Comparing `alida-apis-0.0.3/setup.py` & `alida-apis-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="alida-apis",
-    version="0.0.3",
+    version="0.0.4",
     author="Alida research team",
     author_email="salvatore.cipolla@eng.it",
     description="Python APIs for interaction with ALIDA backend.",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

