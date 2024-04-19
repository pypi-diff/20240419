# Comparing `tmp/python-blockbee-2.0.0.tar.gz` & `tmp/python-blockbee-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-blockbee-2.0.0.tar", last modified: Mon Mar 18 20:46:29 2024, max compression
+gzip compressed data, was "python-blockbee-2.0.1.tar", last modified: Fri Apr 19 08:40:49 2024, max compression
```

## Comparing `python-blockbee-2.0.0.tar` & `python-blockbee-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-03-18 20:46:29.427358 python-blockbee-2.0.0/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1075 2023-01-13 17:33:47.000000 python-blockbee-2.0.0/LICENSE
--rw-r--r--   0 arianoangelo   (501) staff       (20)    25137 2024-03-18 20:46:29.427193 python-blockbee-2.0.0/PKG-INFO
--rw-r--r--   0 arianoangelo   (501) staff       (20)    24481 2024-03-18 11:03:24.000000 python-blockbee-2.0.0/README.md
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-03-18 20:46:29.426031 python-blockbee-2.0.0/blockbee/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     8790 2024-03-18 11:03:24.000000 python-blockbee-2.0.0/blockbee/BlockBee.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     3244 2024-03-18 10:36:06.000000 python-blockbee-2.0.0/blockbee/BlockBeeCheckout.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)       89 2024-03-14 16:00:34.000000 python-blockbee-2.0.0/blockbee/__init__.py
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-03-18 20:46:29.426966 python-blockbee-2.0.0/python_blockbee.egg-info/
--rw-r--r--   0 arianoangelo   (501) staff       (20)    25137 2024-03-18 20:46:29.000000 python-blockbee-2.0.0/python_blockbee.egg-info/PKG-INFO
--rw-r--r--   0 arianoangelo   (501) staff       (20)      329 2024-03-18 20:46:29.000000 python-blockbee-2.0.0/python_blockbee.egg-info/SOURCES.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2024-03-18 20:46:29.000000 python-blockbee-2.0.0/python_blockbee.egg-info/dependency_links.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-13 17:38:51.000000 python-blockbee-2.0.0/python_blockbee.egg-info/not-zip-safe
--rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2024-03-18 20:46:29.000000 python-blockbee-2.0.0/python_blockbee.egg-info/requires.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2024-03-18 20:46:29.000000 python-blockbee-2.0.0/python_blockbee.egg-info/top_level.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2024-03-18 20:46:29.427407 python-blockbee-2.0.0/setup.cfg
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1026 2024-03-18 11:03:24.000000 python-blockbee-2.0.0/setup.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-19 08:40:49.082203 python-blockbee-2.0.1/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1075 2023-01-13 17:33:47.000000 python-blockbee-2.0.1/LICENSE
+-rw-r--r--   0 arianoangelo   (501) staff       (20)    25166 2024-04-19 08:40:49.082034 python-blockbee-2.0.1/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)    24510 2024-04-19 08:33:28.000000 python-blockbee-2.0.1/README.md
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-19 08:40:49.080728 python-blockbee-2.0.1/blockbee/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     8787 2024-04-19 08:33:28.000000 python-blockbee-2.0.1/blockbee/BlockBee.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     3244 2024-03-18 10:36:06.000000 python-blockbee-2.0.1/blockbee/BlockBeeCheckout.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       89 2024-03-14 16:00:34.000000 python-blockbee-2.0.1/blockbee/__init__.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2024-04-19 08:40:49.081806 python-blockbee-2.0.1/python_blockbee.egg-info/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)    25166 2024-04-19 08:40:49.000000 python-blockbee-2.0.1/python_blockbee.egg-info/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      329 2024-04-19 08:40:49.000000 python-blockbee-2.0.1/python_blockbee.egg-info/SOURCES.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2024-04-19 08:40:49.000000 python-blockbee-2.0.1/python_blockbee.egg-info/dependency_links.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-13 17:38:51.000000 python-blockbee-2.0.1/python_blockbee.egg-info/not-zip-safe
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2024-04-19 08:40:49.000000 python-blockbee-2.0.1/python_blockbee.egg-info/requires.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2024-04-19 08:40:49.000000 python-blockbee-2.0.1/python_blockbee.egg-info/top_level.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2024-04-19 08:40:49.082254 python-blockbee-2.0.1/setup.cfg
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1026 2024-04-19 08:33:28.000000 python-blockbee-2.0.1/setup.py
```

### Comparing `python-blockbee-2.0.0/LICENSE` & `python-blockbee-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-blockbee-2.0.0/PKG-INFO` & `python-blockbee-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-blockbee
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python Library for BlockBee payment gateway
 Home-page: https://github.com/blockbee-io/python-blockbee
 Author: BlockBee
 Author-email: info@blockbee.io
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -611,11 +611,14 @@
 * Minor bugfixes
 
 #### 2.0.0
 * Automated Payouts
 * Support to BlockBee Checkout page
 * Various improvements
 
+#### 2.0.1
+* Minor bugfixes
+
 ### Breaking Changes
 
 #### 2.0.0
 * `create_payout` parameters were changed and will require you to update your code.
```

### Comparing `python-blockbee-2.0.0/README.md` & `python-blockbee-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -592,11 +592,14 @@
 * Minor bugfixes
 
 #### 2.0.0
 * Automated Payouts
 * Support to BlockBee Checkout page
 * Various improvements
 
+#### 2.0.1
+* Minor bugfixes
+
 ### Breaking Changes
 
 #### 2.0.0
 * `create_payout` parameters were changed and will require you to update your code.
```

### Comparing `python-blockbee-2.0.0/blockbee/BlockBee.py` & `python-blockbee-2.0.1/blockbee/BlockBee.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     def list_payouts(coin, status = 'all', page = 1, api_key = '', payout_request=False):
         if not api_key:
             return None
 
         params = {
             'apikey': api_key,
             'status': status,
-            'page': page
+            'p': page
         }
 
         endpoint = 'payout/list'
 
         if payout_request:
             endpoint = 'payout/request/list'
```

### Comparing `python-blockbee-2.0.0/blockbee/BlockBeeCheckout.py` & `python-blockbee-2.0.1/blockbee/BlockBeeCheckout.py`

 * *Files identical despite different names*

### Comparing `python-blockbee-2.0.0/python_blockbee.egg-info/PKG-INFO` & `python-blockbee-2.0.1/python_blockbee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-blockbee
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python Library for BlockBee payment gateway
 Home-page: https://github.com/blockbee-io/python-blockbee
 Author: BlockBee
 Author-email: info@blockbee.io
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -611,11 +611,14 @@
 * Minor bugfixes
 
 #### 2.0.0
 * Automated Payouts
 * Support to BlockBee Checkout page
 * Various improvements
 
+#### 2.0.1
+* Minor bugfixes
+
 ### Breaking Changes
 
 #### 2.0.0
 * `create_payout` parameters were changed and will require you to update your code.
```

### Comparing `python-blockbee-2.0.0/setup.py` & `python-blockbee-2.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
 
     name='python-blockbee',
 
-    version='2.0.0',
+    version='2.0.1',
 
     packages=find_packages(),
 
     author="BlockBee",
 
     author_email="info@blockbee.io",
     install_requires=[
```

