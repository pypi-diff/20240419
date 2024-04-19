# Comparing `tmp/edds-1.1.tar.gz` & `tmp/edds-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edds-1.1.tar", last modified: Fri Apr 19 09:42:55 2024, max compression
+gzip compressed data, was "edds-1.2.tar", last modified: Fri Apr 19 09:57:29 2024, max compression
```

## Comparing `edds-1.1.tar` & `edds-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 09:42:55.575000 edds-1.1/
--rw-rw-rw-   0        0        0        0 2024-04-19 08:41:51.000000 edds-1.1/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-19 08:43:36.000000 edds-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2215 2024-04-19 09:42:55.543000 edds-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1667 2024-04-19 09:42:25.000000 edds-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 09:42:55.526000 edds-1.1/edds.egg-info/
--rw-rw-rw-   0        0        0     2215 2024-04-19 09:42:54.000000 edds-1.1/edds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-04-19 09:42:54.000000 edds-1.1/edds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 09:42:54.000000 edds-1.1/edds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 09:42:54.000000 edds-1.1/edds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 09:42:54.000000 edds-1.1/edds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 09:42:55.572000 edds-1.1/setup.cfg
--rw-rw-rw-   0        0        0      735 2024-04-19 09:42:43.000000 edds-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:57:29.157000 edds-1.2/
+-rw-rw-rw-   0        0        0        0 2024-04-19 08:41:51.000000 edds-1.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-19 08:43:36.000000 edds-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2236 2024-04-19 09:57:29.115000 edds-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1667 2024-04-19 09:42:25.000000 edds-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 09:57:29.070000 edds-1.2/edds.egg-info/
+-rw-rw-rw-   0        0        0     2236 2024-04-19 09:57:28.000000 edds-1.2/edds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2024-04-19 09:57:28.000000 edds-1.2/edds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:57:28.000000 edds-1.2/edds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-19 09:57:28.000000 edds-1.2/edds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:57:28.000000 edds-1.2/edds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:57:29.153000 edds-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      752 2024-04-19 09:50:46.000000 edds-1.2/setup.py
```

### Comparing `edds-1.1/PKG-INFO` & `edds-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: edds
-Version: 1.1
+Version: 1.2
 Summary: The Central Bank of the Republic of Türkiye Electronic Data Distribution System Data Access Package
 Home-page: https://github.com/altanalaybeyoglu/edds
 Author: Altan Alaybeyoğlu
 Author-email: altanalaybeyoglu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pandas
+Requires-Dist: json
 
 # edds - The Central Bank of the Republic of TÃ¼rkiye Electronic Data Distribution System Data Access Package
 
 This package provides easy-to-use functions to retrieve data from the Central Bank of the Republic of Turkey (TCMB) Economic Data Distribution System (EDDS) web service.
 
 # Features
```

### Comparing `edds-1.1/README.md` & `edds-1.2/README.md`

 * *Files identical despite different names*

### Comparing `edds-1.1/edds.egg-info/PKG-INFO` & `edds-1.2/edds.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: edds
-Version: 1.1
+Version: 1.2
 Summary: The Central Bank of the Republic of Türkiye Electronic Data Distribution System Data Access Package
 Home-page: https://github.com/altanalaybeyoglu/edds
 Author: Altan Alaybeyoğlu
 Author-email: altanalaybeyoglu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pandas
+Requires-Dist: json
 
 # edds - The Central Bank of the Republic of TÃ¼rkiye Electronic Data Distribution System Data Access Package
 
 This package provides easy-to-use functions to retrieve data from the Central Bank of the Republic of Turkey (TCMB) Economic Data Distribution System (EDDS) web service.
 
 # Features
```

### Comparing `edds-1.1/setup.py` & `edds-1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="edds",  
-    version="1.1",  
+    version="1.2",  
     author="Altan Alaybeyoğlu",
     author_email="altanalaybeyoglu@gmail.com",
     description="The Central Bank of the Republic of Türkiye Electronic Data Distribution System Data Access Package", 
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/altanalaybeyoglu/edds",  
     packages=find_packages(),
     install_requires=[
         "requests",
         "pandas",
+        "json",
     ],  
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

