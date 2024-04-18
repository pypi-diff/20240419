# Comparing `tmp/eirStru-0.2.98.tar.gz` & `tmp/eirStru-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.2.98.tar", last modified: Mon Apr 15 09:07:34 2024, max compression
+gzip compressed data, was "eirStru-0.2.99.tar", last modified: Mon Apr 15 09:38:10 2024, max compression
```

## Comparing `eirStru-0.2.98.tar` & `eirStru-0.2.99.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:07:34.641121 eirStru-0.2.98/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.98/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.98/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 09:07:34.640851 eirStru-0.2.98/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.98/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:07:34.640148 eirStru-0.2.98/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.98/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.98/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.98/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    18149 2024-04-15 09:07:32.000000 eirStru-0.2.98/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.98/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     5936 2024-04-15 08:37:49.000000 eirStru-0.2.98/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.98/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.98/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.98/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.98/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:07:34.640617 eirStru-0.2.98/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 09:07:34.000000 eirStru-0.2.98/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-15 09:07:34.000000 eirStru-0.2.98/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-15 09:07:34.000000 eirStru-0.2.98/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-15 09:07:34.000000 eirStru-0.2.98/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-15 09:07:34.641172 eirStru-0.2.98/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-04-15 09:07:32.000000 eirStru-0.2.98/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:38:10.604345 eirStru-0.2.99/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.99/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.99/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 09:38:10.604060 eirStru-0.2.99/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.99/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:38:10.603037 eirStru-0.2.99/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.99/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.99/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.99/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    18149 2024-04-15 09:07:32.000000 eirStru-0.2.99/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.99/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     5936 2024-04-15 08:37:49.000000 eirStru-0.2.99/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.99/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.99/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.99/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.99/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:38:10.603749 eirStru-0.2.99/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 09:38:10.000000 eirStru-0.2.99/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-15 09:38:10.000000 eirStru-0.2.99/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-15 09:38:10.000000 eirStru-0.2.99/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-15 09:38:10.000000 eirStru-0.2.99/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-15 09:38:10.604392 eirStru-0.2.99/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-04-15 09:38:08.000000 eirStru-0.2.99/setup.py
```

### Comparing `eirStru-0.2.98/LICENSE` & `eirStru-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.98/PKG-INFO` & `eirStru-0.2.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.98
+Version: 0.2.99
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.98/README.md` & `eirStru-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.98/eirStru/aiomysql_helper.py` & `eirStru-0.2.99/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.98/eirStru/common.py` & `eirStru-0.2.99/eirStru/common.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.98/eirStru/eirjob_intf.py` & `eirStru-0.2.99/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.98/eirStru/eirlogin_intf.py` & `eirStru-0.2.99/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.98/eirStru/redis_utils.py` & `eirStru-0.2.99/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.98/eirStru/utils.py` & `eirStru-0.2.99/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.98/eirStru/wx_push.py` & `eirStru-0.2.99/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.98/eirStru.egg-info/PKG-INFO` & `eirStru-0.2.99/eirStru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.98
+Version: 0.2.99
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.98/setup.py` & `eirStru-0.2.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'eirStru'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.98'
+VERSION = '0.2.99'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

