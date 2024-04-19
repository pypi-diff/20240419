# Comparing `tmp/jsonrpc_python_client_generator-1.0.1.tar.gz` & `tmp/jsonrpc_python_client_generator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc_python_client_generator-1.0.1.tar", last modified: Fri Apr 19 08:32:58 2024, max compression
+gzip compressed data, was "jsonrpc_python_client_generator-1.0.2.tar", last modified: Fri Apr 19 09:56:27 2024, max compression
```

## Comparing `jsonrpc_python_client_generator-1.0.1.tar` & `jsonrpc_python_client_generator-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vitalij    (501) staff       (20)        0 2024-04-19 08:32:58.234738 jsonrpc_python_client_generator-1.0.1/
--rw-r--r--   0 vitalij    (501) staff       (20)      563 2024-04-19 07:38:57.000000 jsonrpc_python_client_generator-1.0.1/LICENSE
--rw-r--r--   0 vitalij    (501) staff       (20)     1930 2024-04-19 08:32:58.234644 jsonrpc_python_client_generator-1.0.1/PKG-INFO
--rw-r--r--   0 vitalij    (501) staff       (20)     1372 2024-04-19 08:31:48.000000 jsonrpc_python_client_generator-1.0.1/README.md
-drwxr-xr-x   0 vitalij    (501) staff       (20)        0 2024-04-19 08:32:58.233296 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator/
--rw-r--r--   0 vitalij    (501) staff       (20)        0 2024-04-18 06:41:25.000000 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator/__init__.py
--rw-r--r--   0 vitalij    (501) staff       (20)      971 2024-04-19 08:24:28.000000 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator/client.py
--rw-r--r--   0 vitalij    (501) staff       (20)     4377 2024-04-19 07:57:09.000000 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator/generator.py
--rw-r--r--   0 vitalij    (501) staff       (20)      902 2024-04-18 12:13:05.000000 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator/response.py
-drwxr-xr-x   0 vitalij    (501) staff       (20)        0 2024-04-19 08:32:58.234327 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator.egg-info/
--rw-r--r--   0 vitalij    (501) staff       (20)     1930 2024-04-19 08:32:58.000000 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator.egg-info/PKG-INFO
--rw-r--r--   0 vitalij    (501) staff       (20)      485 2024-04-19 08:32:58.000000 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator.egg-info/SOURCES.txt
--rw-r--r--   0 vitalij    (501) staff       (20)        1 2024-04-19 08:32:58.000000 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator.egg-info/dependency_links.txt
--rw-r--r--   0 vitalij    (501) staff       (20)       17 2024-04-19 08:32:58.000000 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator.egg-info/requires.txt
--rw-r--r--   0 vitalij    (501) staff       (20)       32 2024-04-19 08:32:58.000000 jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator.egg-info/top_level.txt
--rw-r--r--   0 vitalij    (501) staff       (20)       38 2024-04-19 08:32:58.234973 jsonrpc_python_client_generator-1.0.1/setup.cfg
--rw-r--r--   0 vitalij    (501) staff       (20)      801 2024-04-19 08:15:24.000000 jsonrpc_python_client_generator-1.0.1/setup.py
+drwxr-xr-x   0 vitalij    (501) staff       (20)        0 2024-04-19 09:56:27.630200 jsonrpc_python_client_generator-1.0.2/
+-rw-r--r--   0 vitalij    (501) staff       (20)     1067 2024-04-19 08:39:47.000000 jsonrpc_python_client_generator-1.0.2/LICENSE
+-rw-r--r--   0 vitalij    (501) staff       (20)     1898 2024-04-19 09:56:27.630108 jsonrpc_python_client_generator-1.0.2/PKG-INFO
+-rw-r--r--   0 vitalij    (501) staff       (20)     1340 2024-04-19 08:37:33.000000 jsonrpc_python_client_generator-1.0.2/README.md
+drwxr-xr-x   0 vitalij    (501) staff       (20)        0 2024-04-19 09:56:27.628284 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator/
+-rw-r--r--   0 vitalij    (501) staff       (20)        0 2024-04-18 06:41:25.000000 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator/__init__.py
+-rw-r--r--   0 vitalij    (501) staff       (20)      971 2024-04-19 08:24:28.000000 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator/client.py
+-rw-r--r--   0 vitalij    (501) staff       (20)     4377 2024-04-19 07:57:09.000000 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator/generator.py
+-rw-r--r--   0 vitalij    (501) staff       (20)      902 2024-04-18 12:13:05.000000 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator/response.py
+drwxr-xr-x   0 vitalij    (501) staff       (20)        0 2024-04-19 09:56:27.629654 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator.egg-info/
+-rw-r--r--   0 vitalij    (501) staff       (20)     1898 2024-04-19 09:56:27.000000 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator.egg-info/PKG-INFO
+-rw-r--r--   0 vitalij    (501) staff       (20)      485 2024-04-19 09:56:27.000000 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 vitalij    (501) staff       (20)        1 2024-04-19 09:56:27.000000 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 vitalij    (501) staff       (20)       17 2024-04-19 09:56:27.000000 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator.egg-info/requires.txt
+-rw-r--r--   0 vitalij    (501) staff       (20)       32 2024-04-19 09:56:27.000000 jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator.egg-info/top_level.txt
+-rw-r--r--   0 vitalij    (501) staff       (20)       38 2024-04-19 09:56:27.630488 jsonrpc_python_client_generator-1.0.2/setup.cfg
+-rw-r--r--   0 vitalij    (501) staff       (20)      801 2024-04-19 08:53:36.000000 jsonrpc_python_client_generator-1.0.2/setup.py
```

### Comparing `jsonrpc_python_client_generator-1.0.1/PKG-INFO` & `jsonrpc_python_client_generator-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc_python_client_generator
-Version: 1.0.1
+Version: 1.0.2
 Summary: Jsonrpc Python Client Generator
 Home-page: https://github.com/vk1511work/jsonrpc-python-client-generator
 Author: vk1511work
 Author-email: vk1511work@gmail.com
 Keywords: jsonrpc 2.0 python client generator
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -68,8 +68,7 @@
 
 client = JsonRpcClient()
 client.checkLogin(login="your_login")
 ```
 
 ## Requirements
  * Python 3.10 and higher
- * PHP --with-curl installation
```

### Comparing `jsonrpc_python_client_generator-1.0.1/README.md` & `jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: jsonrpc_python_client_generator
+Version: 1.0.2
+Summary: Jsonrpc Python Client Generator
+Home-page: https://github.com/vk1511work/jsonrpc-python-client-generator
+Author: vk1511work
+Author-email: vk1511work@gmail.com
+Keywords: jsonrpc 2.0 python client generator
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.25.1
+
 # Jsonrpc Python Client Generator
 
 ## Installation
 
 ```bash
 pip install jsonrpc-python-client-generator
 ```
@@ -52,8 +68,7 @@
 
 client = JsonRpcClient()
 client.checkLogin(login="your_login")
 ```
 
 ## Requirements
  * Python 3.10 and higher
- * PHP --with-curl installation
```

### Comparing `jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator/client.py` & `jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator/client.py`

 * *Files identical despite different names*

### Comparing `jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator/generator.py` & `jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator/generator.py`

 * *Files identical despite different names*

### Comparing `jsonrpc_python_client_generator-1.0.1/jsonrpc_python_client_generator/response.py` & `jsonrpc_python_client_generator-1.0.2/jsonrpc_python_client_generator/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc_python_client_generator-1.0.1/setup.py` & `jsonrpc_python_client_generator-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='jsonrpc_python_client_generator',
-  version='1.0.1',
+  version='1.0.2',
   author='vk1511work',
   author_email='vk1511work@gmail.com',
   description='Jsonrpc Python Client Generator',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/vk1511work/jsonrpc-python-client-generator',
   packages=find_packages(),
```

