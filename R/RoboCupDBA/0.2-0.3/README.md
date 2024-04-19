# Comparing `tmp/RoboCupDBA-0.2.tar.gz` & `tmp/RoboCupDBA-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RoboCupDBA-0.2.tar", last modified: Fri Apr 19 07:43:22 2024, max compression
+gzip compressed data, was "RoboCupDBA-0.3.tar", last modified: Fri Apr 19 07:57:21 2024, max compression
```

## Comparing `RoboCupDBA-0.2.tar` & `RoboCupDBA-0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-19 07:43:22.341998 RoboCupDBA-0.2/
--rw-r--r--   0 dev        (501) staff       (20)     1753 2024-04-19 07:43:22.341767 RoboCupDBA-0.2/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)     1355 2024-04-19 07:33:19.000000 RoboCupDBA-0.2/README.md
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-19 07:43:22.340720 RoboCupDBA-0.2/RoboCupDBA/
--rw-r--r--   0 dev        (501) staff       (20)       62 2024-04-19 07:02:15.000000 RoboCupDBA-0.2/RoboCupDBA/__init__.py
--rw-r--r--   0 dev        (501) staff       (20)      894 2024-04-19 06:59:48.000000 RoboCupDBA-0.2/RoboCupDBA/insert.py
--rw-r--r--   0 dev        (501) staff       (20)      493 2024-04-19 07:00:25.000000 RoboCupDBA-0.2/RoboCupDBA/query.py
-drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-19 07:43:22.341532 RoboCupDBA-0.2/RoboCupDBA.egg-info/
--rw-r--r--   0 dev        (501) staff       (20)     1753 2024-04-19 07:43:22.000000 RoboCupDBA-0.2/RoboCupDBA.egg-info/PKG-INFO
--rw-r--r--   0 dev        (501) staff       (20)      218 2024-04-19 07:43:22.000000 RoboCupDBA-0.2/RoboCupDBA.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (501) staff       (20)        1 2024-04-19 07:43:22.000000 RoboCupDBA-0.2/RoboCupDBA.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (501) staff       (20)       11 2024-04-19 07:43:22.000000 RoboCupDBA-0.2/RoboCupDBA.egg-info/top_level.txt
--rw-r--r--   0 dev        (501) staff       (20)       38 2024-04-19 07:43:22.342043 RoboCupDBA-0.2/setup.cfg
--rw-r--r--   0 dev        (501) staff       (20)      629 2024-04-19 07:43:11.000000 RoboCupDBA-0.2/setup.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-19 07:57:21.339981 RoboCupDBA-0.3/
+-rw-r--r--   0 dev        (501) staff       (20)     1824 2024-04-19 07:57:21.339737 RoboCupDBA-0.3/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)     1355 2024-04-19 07:33:19.000000 RoboCupDBA-0.3/README.md
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-19 07:57:21.338208 RoboCupDBA-0.3/RoboCupDBA/
+-rw-r--r--   0 dev        (501) staff       (20)       62 2024-04-19 07:02:15.000000 RoboCupDBA-0.3/RoboCupDBA/__init__.py
+-rw-r--r--   0 dev        (501) staff       (20)      894 2024-04-19 06:59:48.000000 RoboCupDBA-0.3/RoboCupDBA/insert.py
+-rw-r--r--   0 dev        (501) staff       (20)      493 2024-04-19 07:00:25.000000 RoboCupDBA-0.3/RoboCupDBA/query.py
+drwxr-xr-x   0 dev        (501) staff       (20)        0 2024-04-19 07:57:21.339413 RoboCupDBA-0.3/RoboCupDBA.egg-info/
+-rw-r--r--   0 dev        (501) staff       (20)     1824 2024-04-19 07:57:21.000000 RoboCupDBA-0.3/RoboCupDBA.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (501) staff       (20)      251 2024-04-19 07:57:21.000000 RoboCupDBA-0.3/RoboCupDBA.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (501) staff       (20)        1 2024-04-19 07:57:21.000000 RoboCupDBA-0.3/RoboCupDBA.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (501) staff       (20)       26 2024-04-19 07:57:21.000000 RoboCupDBA-0.3/RoboCupDBA.egg-info/requires.txt
+-rw-r--r--   0 dev        (501) staff       (20)       11 2024-04-19 07:57:21.000000 RoboCupDBA-0.3/RoboCupDBA.egg-info/top_level.txt
+-rw-r--r--   0 dev        (501) staff       (20)       38 2024-04-19 07:57:21.340046 RoboCupDBA-0.3/setup.cfg
+-rw-r--r--   0 dev        (501) staff       (20)      717 2024-04-19 07:57:00.000000 RoboCupDBA-0.3/setup.py
```

### Comparing `RoboCupDBA-0.2/PKG-INFO` & `RoboCupDBA-0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: RoboCupDBA
-Version: 0.2
+Version: 0.3
 Summary: A small example package MongoDB Robo
 Home-page: https://github.com/bluebox-dev/RoboCupDBA
 Author: blueboxdev
 Author-email: thanakorn.vsalab@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: dnspython
+Requires-Dist: install
+Requires-Dist: pymongo
 
 # RoboCupDBA
 ## Exmaple Insert RoboCupDBA
 ```
 import RoboCupDBA
 RoboCupDBA.Insert(link="mongodb://root:6yHnmju%26@localhost:27017/",db="data",collection="data",name="1",x=0.0,y=0.0,theta=0.0,typeObj="A")
 ```
```

### Comparing `RoboCupDBA-0.2/README.md` & `RoboCupDBA-0.3/README.md`

 * *Files identical despite different names*

### Comparing `RoboCupDBA-0.2/RoboCupDBA/insert.py` & `RoboCupDBA-0.3/RoboCupDBA/insert.py`

 * *Files identical despite different names*

### Comparing `RoboCupDBA-0.2/RoboCupDBA.egg-info/PKG-INFO` & `RoboCupDBA-0.3/RoboCupDBA.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: RoboCupDBA
-Version: 0.2
+Version: 0.3
 Summary: A small example package MongoDB Robo
 Home-page: https://github.com/bluebox-dev/RoboCupDBA
 Author: blueboxdev
 Author-email: thanakorn.vsalab@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Requires-Dist: dnspython
+Requires-Dist: install
+Requires-Dist: pymongo
 
 # RoboCupDBA
 ## Exmaple Insert RoboCupDBA
 ```
 import RoboCupDBA
 RoboCupDBA.Insert(link="mongodb://root:6yHnmju%26@localhost:27017/",db="data",collection="data",name="1",x=0.0,y=0.0,theta=0.0,typeObj="A")
 ```
```

