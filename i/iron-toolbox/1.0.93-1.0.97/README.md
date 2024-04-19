# Comparing `tmp/iron_toolbox-1.0.93.tar.gz` & `tmp/iron_toolbox-1.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iron_toolbox-1.0.93.tar", last modified: Thu Mar 28 13:54:35 2024, max compression
+gzip compressed data, was "iron_toolbox-1.0.97.tar", last modified: Fri Apr 19 16:21:54 2024, max compression
```

## Comparing `iron_toolbox-1.0.93.tar` & `iron_toolbox-1.0.97.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:54:35.719669 iron_toolbox-1.0.93/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-28 13:54:29.000000 iron_toolbox-1.0.93/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-28 13:54:35.719669 iron_toolbox-1.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-28 13:54:29.000000 iron_toolbox-1.0.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:54:35.715669 iron_toolbox-1.0.93/iron_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-28 13:54:29.000000 iron_toolbox-1.0.93/iron_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-03-28 13:54:29.000000 iron_toolbox-1.0.93/iron_toolbox/aws_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-03-28 13:54:29.000000 iron_toolbox-1.0.93/iron_toolbox/domo_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-03-28 13:54:29.000000 iron_toolbox-1.0.93/iron_toolbox/iron_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)   108913 2024-03-28 13:54:29.000000 iron_toolbox-1.0.93/iron_toolbox/mongo_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-03-28 13:54:29.000000 iron_toolbox-1.0.93/iron_toolbox/sftp_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:54:35.719669 iron_toolbox-1.0.93/iron_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-28 13:54:35.000000 iron_toolbox-1.0.93/iron_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-28 13:54:35.000000 iron_toolbox-1.0.93/iron_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:54:35.000000 iron_toolbox-1.0.93/iron_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 13:54:35.000000 iron_toolbox-1.0.93/iron_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-28 13:54:35.000000 iron_toolbox-1.0.93/iron_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-28 13:54:35.719669 iron_toolbox-1.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-28 13:54:29.000000 iron_toolbox-1.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:21:54.112581 iron_toolbox-1.0.97/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 16:21:48.000000 iron_toolbox-1.0.97/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-19 16:21:54.112581 iron_toolbox-1.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-19 16:21:48.000000 iron_toolbox-1.0.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:21:54.112581 iron_toolbox-1.0.97/iron_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 16:21:48.000000 iron_toolbox-1.0.97/iron_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-19 16:21:48.000000 iron_toolbox-1.0.97/iron_toolbox/aws_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-19 16:21:48.000000 iron_toolbox-1.0.97/iron_toolbox/domo_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-04-19 16:21:48.000000 iron_toolbox-1.0.97/iron_toolbox/iron_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108913 2024-04-19 16:21:48.000000 iron_toolbox-1.0.97/iron_toolbox/mongo_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-19 16:21:48.000000 iron_toolbox-1.0.97/iron_toolbox/sftp_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:21:54.112581 iron_toolbox-1.0.97/iron_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-19 16:21:54.000000 iron_toolbox-1.0.97/iron_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-19 16:21:54.000000 iron_toolbox-1.0.97/iron_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:21:54.000000 iron_toolbox-1.0.97/iron_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 16:21:54.000000 iron_toolbox-1.0.97/iron_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 16:21:54.000000 iron_toolbox-1.0.97/iron_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 16:21:54.112581 iron_toolbox-1.0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-19 16:21:48.000000 iron_toolbox-1.0.97/setup.py
```

### Comparing `iron_toolbox-1.0.93/LICENSE.txt` & `iron_toolbox-1.0.97/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.93/PKG-INFO` & `iron_toolbox-1.0.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iron_toolbox
-Version: 1.0.93
+Version: 1.0.97
 Summary: Functions to be used by Iron Data Analytics Team
 Home-page: https://github.com/IronTrainers/iron_data_toolbox
 Download-URL: https://github.com/IronTrainers/iron_data_toolbox/archive/refs/tags/iron_data_toolboox.tar.gz
 Author: Luciano Siqueira
 Author-email: lucianosiqueira@iron.fit
 License: MIT
 Project-URL: Bug Tracker, https://github.com/IronTrainers/iron_data_toolbox/issues
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: DateTime==5.1
 Requires-Dist: duckdb==0.7.1
 Requires-Dist: fsspec==2022.7.1
 Requires-Dist: paramiko
 Requires-Dist: pydomo==0.3.0.9
-Requires-Dist: pymongo==4.3.3
+Requires-Dist: pymongo==4.6.3
 Requires-Dist: s3fs==2022.7.1
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: Unidecode==1.3.6
 Requires-Dist: pysftp==0.2.9
 
 # Iron Toolbox
 ### Utilização da Biblioteca
```

### Comparing `iron_toolbox-1.0.93/README.md` & `iron_toolbox-1.0.97/README.md`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.93/iron_toolbox/aws_functions.py` & `iron_toolbox-1.0.97/iron_toolbox/aws_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.93/iron_toolbox/domo_functions.py` & `iron_toolbox-1.0.97/iron_toolbox/domo_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.93/iron_toolbox/iron_functions.py` & `iron_toolbox-1.0.97/iron_toolbox/iron_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.93/iron_toolbox/mongo_functions.py` & `iron_toolbox-1.0.97/iron_toolbox/mongo_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.93/iron_toolbox/sftp_functions.py` & `iron_toolbox-1.0.97/iron_toolbox/sftp_functions.py`

 * *Files identical despite different names*

### Comparing `iron_toolbox-1.0.93/iron_toolbox.egg-info/PKG-INFO` & `iron_toolbox-1.0.97/iron_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iron_toolbox
-Version: 1.0.93
+Version: 1.0.97
 Summary: Functions to be used by Iron Data Analytics Team
 Home-page: https://github.com/IronTrainers/iron_data_toolbox
 Download-URL: https://github.com/IronTrainers/iron_data_toolbox/archive/refs/tags/iron_data_toolboox.tar.gz
 Author: Luciano Siqueira
 Author-email: lucianosiqueira@iron.fit
 License: MIT
 Project-URL: Bug Tracker, https://github.com/IronTrainers/iron_data_toolbox/issues
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: DateTime==5.1
 Requires-Dist: duckdb==0.7.1
 Requires-Dist: fsspec==2022.7.1
 Requires-Dist: paramiko
 Requires-Dist: pydomo==0.3.0.9
-Requires-Dist: pymongo==4.3.3
+Requires-Dist: pymongo==4.6.3
 Requires-Dist: s3fs==2022.7.1
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: Unidecode==1.3.6
 Requires-Dist: pysftp==0.2.9
 
 # Iron Toolbox
 ### Utilização da Biblioteca
```

### Comparing `iron_toolbox-1.0.93/setup.py` & `iron_toolbox-1.0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='iron_toolbox',
     packages=['iron_toolbox'],
-    version='1.0.93',
+    version='1.0.97',
     license='MIT',
     description='Functions to be used by Iron Data Analytics Team',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Luciano Siqueira',
     author_email='lucianosiqueira@iron.fit',
     url='https://github.com/IronTrainers/iron_data_toolbox',
     project_urls={"Bug Tracker": "https://github.com/IronTrainers/iron_data_toolbox/issues"},
     install_requires=['DateTime==5.1',
                       'duckdb==0.7.1',
                       'fsspec==2022.7.1',
                       'paramiko',
                       'pydomo==0.3.0.9',
-                      'pymongo==4.3.3',
+                      'pymongo==4.6.3',
                       's3fs==2022.7.1',
                       'tqdm==4.65.0',
                       'Unidecode==1.3.6',
                       'pysftp==0.2.9'],
     keywords=['python',
               'mongodb',
               'aws',
```

