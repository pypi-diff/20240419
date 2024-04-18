# Comparing `tmp/netskopesdk-0.0.8.tar.gz` & `tmp/netskopesdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/brajendran/NetSkope/repositories/restsdk/dist/tmpe1vi2lr8/netskopesdk-0.0.8.tar", last modified: Tue May 17 19:29:34 2022, max compression
+gzip compressed data, was "/Users/brajendran/NetSkope/repositories/restsdk/dist/tmp74eleaz4/netskopesdk-0.0.9.tar", last modified: Tue May 17 19:36:42 2022, max compression
```

## Comparing `netskopesdk-0.0.8.tar` & `netskopesdk-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/
--rw-r--r--   0 brajendran   (501) staff       (20)     1516 2022-05-17 19:28:56.000000 netskopesdk-0.0.8/LICENSE
--rw-r--r--   0 brajendran   (501) staff       (20)     2402 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/PKG-INFO
--rw-r--r--   0 brajendran   (501) staff       (20)     1921 2022-05-17 19:22:39.000000 netskopesdk-0.0.8/README.md
--rw-r--r--   0 brajendran   (501) staff       (20)       84 2022-04-27 21:41:22.000000 netskopesdk-0.0.8/pyproject.toml
--rw-r--r--   0 brajendran   (501) staff       (20)       38 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/setup.cfg
--rw-r--r--   0 brajendran   (501) staff       (20)      918 2022-05-17 19:29:17.000000 netskopesdk-0.0.8/setup.py
-drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/src/
-drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/src/netskope/
--rw-r--r--   0 brajendran   (501) staff       (20)        1 2022-04-12 23:10:22.000000 netskopesdk-0.0.8/src/netskope/__init__.py
-drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/src/netskope/api/
--rw-r--r--   0 brajendran   (501) staff       (20)        1 2022-04-12 23:10:22.000000 netskopesdk-0.0.8/src/netskope/api/__init__.py
-drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/src/netskope/api/iterator/
--rw-r--r--   0 brajendran   (501) staff       (20)        1 2022-04-12 23:10:22.000000 netskopesdk-0.0.8/src/netskope/api/iterator/__init__.py
--rw-r--r--   0 brajendran   (501) staff       (20)      388 2022-05-10 01:35:01.000000 netskopesdk-0.0.8/src/netskope/api/iterator/const.py
--rwxr-xr-x   0 brajendran   (501) staff       (20)     2907 2022-04-28 19:01:34.000000 netskopesdk-0.0.8/src/netskope/api/iterator/netskope_iterator.py
--rwxr-xr-x   0 brajendran   (501) staff       (20)     3045 2022-05-09 15:36:00.000000 netskopesdk-0.0.8/src/netskope/api/iterator/netskope_iterator_client.py
--rw-r--r--   0 brajendran   (501) staff       (20)      244 2022-04-27 22:15:53.000000 netskopesdk-0.0.8/src/netskope/api/iterator/operation.py
-drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/src/netskopesdk.egg-info/
--rw-r--r--   0 brajendran   (501) staff       (20)     2402 2022-05-17 19:29:33.000000 netskopesdk-0.0.8/src/netskopesdk.egg-info/PKG-INFO
--rw-r--r--   0 brajendran   (501) staff       (20)      502 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/src/netskopesdk.egg-info/SOURCES.txt
--rw-r--r--   0 brajendran   (501) staff       (20)        1 2022-05-17 19:29:33.000000 netskopesdk-0.0.8/src/netskopesdk.egg-info/dependency_links.txt
--rw-r--r--   0 brajendran   (501) staff       (20)       17 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/src/netskopesdk.egg-info/requires.txt
--rw-r--r--   0 brajendran   (501) staff       (20)        9 2022-05-17 19:29:34.000000 netskopesdk-0.0.8/src/netskopesdk.egg-info/top_level.txt
+drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/
+-rw-r--r--   0 brajendran   (501) staff       (20)     1516 2022-05-17 19:28:56.000000 netskopesdk-0.0.9/LICENSE
+-rw-r--r--   0 brajendran   (501) staff       (20)     2351 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/PKG-INFO
+-rw-r--r--   0 brajendran   (501) staff       (20)     1921 2022-05-17 19:22:39.000000 netskopesdk-0.0.9/README.md
+-rw-r--r--   0 brajendran   (501) staff       (20)       84 2022-04-27 21:41:22.000000 netskopesdk-0.0.9/pyproject.toml
+-rw-r--r--   0 brajendran   (501) staff       (20)       38 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/setup.cfg
+-rw-r--r--   0 brajendran   (501) staff       (20)      867 2022-05-17 19:36:26.000000 netskopesdk-0.0.9/setup.py
+drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/src/
+drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/src/netskope/
+-rw-r--r--   0 brajendran   (501) staff       (20)        1 2022-04-12 23:10:22.000000 netskopesdk-0.0.9/src/netskope/__init__.py
+drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/src/netskope/api/
+-rw-r--r--   0 brajendran   (501) staff       (20)        1 2022-04-12 23:10:22.000000 netskopesdk-0.0.9/src/netskope/api/__init__.py
+drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/src/netskope/api/iterator/
+-rw-r--r--   0 brajendran   (501) staff       (20)        1 2022-04-12 23:10:22.000000 netskopesdk-0.0.9/src/netskope/api/iterator/__init__.py
+-rw-r--r--   0 brajendran   (501) staff       (20)      388 2022-05-10 01:35:01.000000 netskopesdk-0.0.9/src/netskope/api/iterator/const.py
+-rwxr-xr-x   0 brajendran   (501) staff       (20)     2907 2022-04-28 19:01:34.000000 netskopesdk-0.0.9/src/netskope/api/iterator/netskope_iterator.py
+-rwxr-xr-x   0 brajendran   (501) staff       (20)     3045 2022-05-09 15:36:00.000000 netskopesdk-0.0.9/src/netskope/api/iterator/netskope_iterator_client.py
+-rw-r--r--   0 brajendran   (501) staff       (20)      244 2022-04-27 22:15:53.000000 netskopesdk-0.0.9/src/netskope/api/iterator/operation.py
+drwxr-xr-x   0 brajendran   (501) staff       (20)        0 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/src/netskopesdk.egg-info/
+-rw-r--r--   0 brajendran   (501) staff       (20)     2351 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/src/netskopesdk.egg-info/PKG-INFO
+-rw-r--r--   0 brajendran   (501) staff       (20)      502 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/src/netskopesdk.egg-info/SOURCES.txt
+-rw-r--r--   0 brajendran   (501) staff       (20)        1 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/src/netskopesdk.egg-info/dependency_links.txt
+-rw-r--r--   0 brajendran   (501) staff       (20)       17 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/src/netskopesdk.egg-info/requires.txt
+-rw-r--r--   0 brajendran   (501) staff       (20)        9 2022-05-17 19:36:42.000000 netskopesdk-0.0.9/src/netskopesdk.egg-info/top_level.txt
```

### Comparing `netskopesdk-0.0.8/LICENSE` & `netskopesdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netskopesdk-0.0.8/PKG-INFO` & `netskopesdk-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: netskopesdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK to download the Netskope Events
 Home-page: http://www.netskope.com/
 Author: Bharath Rajendran
 Author-email: bharath@netskope.com
 Project-URL: Bug Tracker, http://www.netskope.com/
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Netskope SDK
```

### Comparing `netskopesdk-0.0.8/README.md` & `netskopesdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `netskopesdk-0.0.8/setup.py` & `netskopesdk-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="netskopesdk",
-    version="0.0.8",
+    version="0.0.9",
     author="Bharath Rajendran",
     author_email="bharath@netskope.com",
     description="SDK to download the Netskope Events",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://www.netskope.com/",
     project_urls={
         "Bug Tracker": "http://www.netskope.com/",
     },
 
     include_package_data = True,
 
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
+        "Operating System :: OS Independent"
     ],
     package_dir = { '' : 'src' },
     packages    = find_packages(where='src'),
 
     python_requires=">=3.6",
 
     install_requires = [
```

### Comparing `netskopesdk-0.0.8/src/netskope/api/iterator/netskope_iterator.py` & `netskopesdk-0.0.9/src/netskope/api/iterator/netskope_iterator.py`

 * *Files identical despite different names*

### Comparing `netskopesdk-0.0.8/src/netskope/api/iterator/netskope_iterator_client.py` & `netskopesdk-0.0.9/src/netskope/api/iterator/netskope_iterator_client.py`

 * *Files identical despite different names*

### Comparing `netskopesdk-0.0.8/src/netskopesdk.egg-info/PKG-INFO` & `netskopesdk-0.0.9/src/netskopesdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: netskopesdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK to download the Netskope Events
 Home-page: http://www.netskope.com/
 Author: Bharath Rajendran
 Author-email: bharath@netskope.com
 Project-URL: Bug Tracker, http://www.netskope.com/
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Netskope SDK
```

