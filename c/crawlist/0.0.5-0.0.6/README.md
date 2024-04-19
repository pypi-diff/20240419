# Comparing `tmp/crawlist-0.0.5.tar.gz` & `tmp/crawlist-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlist-0.0.5.tar", last modified: Thu Apr 18 06:13:31 2024, max compression
+gzip compressed data, was "crawlist-0.0.6.tar", last modified: Fri Apr 19 06:17:32 2024, max compression
```

## Comparing `crawlist-0.0.5.tar` & `crawlist-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.630055 crawlist-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 06:13:27.000000 crawlist-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 06:13:27.000000 crawlist-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-18 06:13:31.630055 crawlist-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-18 06:13:27.000000 crawlist-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.626055 crawlist-0.0.5/crawlist/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.626055 crawlist-0.0.5/crawlist/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.626055 crawlist-0.0.5/crawlist/analyzers/pager/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/pager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/pager/dynamic_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/pager/pager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/pager/static_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/analyzers/valid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.630055 crawlist-0.0.5/crawlist/processings/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/processings/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-18 06:13:27.000000 crawlist-0.0.5/crawlist/processings/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:13:31.630055 crawlist-0.0.5/crawlist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-18 06:13:31.000000 crawlist-0.0.5/crawlist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-18 06:13:31.000000 crawlist-0.0.5/crawlist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:13:31.000000 crawlist-0.0.5/crawlist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 06:13:31.000000 crawlist-0.0.5/crawlist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 06:13:31.000000 crawlist-0.0.5/crawlist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:13:31.630055 crawlist-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-18 06:13:27.000000 crawlist-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.332104 crawlist-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-19 06:17:28.000000 crawlist-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 06:17:28.000000 crawlist-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-19 06:17:32.332104 crawlist-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-19 06:17:28.000000 crawlist-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.328104 crawlist-0.0.6/crawlist/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.332104 crawlist-0.0.6/crawlist/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.332104 crawlist-0.0.6/crawlist/analyzers/pager/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/pager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/pager/dynamic_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/pager/pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/pager/static_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/analyzers/valid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.332104 crawlist-0.0.6/crawlist/processings/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/processings/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-19 06:17:28.000000 crawlist-0.0.6/crawlist/processings/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:17:32.332104 crawlist-0.0.6/crawlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-19 06:17:32.000000 crawlist-0.0.6/crawlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 06:17:32.000000 crawlist-0.0.6/crawlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:17:32.000000 crawlist-0.0.6/crawlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 06:17:32.000000 crawlist-0.0.6/crawlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 06:17:32.000000 crawlist-0.0.6/crawlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 06:17:32.332104 crawlist-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-19 06:17:28.000000 crawlist-0.0.6/setup.py
```

### Comparing `crawlist-0.0.5/LICENSE` & `crawlist-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/PKG-INFO` & `crawlist-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.5
+Version: 0.0.6
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: parsel
 Requires-Dist: selenium>=4.0.0
 Requires-Dist: cssselect
 Requires-Dist: lxml
 Requires-Dist: requests
@@ -37,26 +37,25 @@
 A universal solution for web crawling lists
 <!-- prettier-ignore-end -->
 
 <p align="center">
   <a href="https://pypi.python.org/pypi/crawlist">
     <img src="https://img.shields.io/pypi/v/crawlist" alt="pypi">
   </a>
-  <img src="https://img.shields.io/badge/python-3.8.0+-blue" alt="python">
+  <img src="https://img.shields.io/badge/python-3.10.0+-blue" alt="python">
   <a href="https://github.com/WwwwwyDev/crawlist/stargazers"><img src="https://img.shields.io/github/stars/WwwwwyDev/crawlist" alt="GitHub stars"style="max-width: 100%;">
   </a>
   <br/>
 </p>
 </div>
 
 
 ## introduction
 
-You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.\
-Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
+You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
 
 ## installing
 You can use pip or pip3 to install the crawlist\
 `pip install crawlist` or `pip3 install crawlist`
 
 ## quickly start
 This is a static website demo. It does not use the JavaScript to load the data.
```

### Comparing `crawlist-0.0.5/README.md` & `crawlist-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,25 @@
 A universal solution for web crawling lists
 <!-- prettier-ignore-end -->
 
 <p align="center">
   <a href="https://pypi.python.org/pypi/crawlist">
     <img src="https://img.shields.io/pypi/v/crawlist" alt="pypi">
   </a>
-  <img src="https://img.shields.io/badge/python-3.8.0+-blue" alt="python">
+  <img src="https://img.shields.io/badge/python-3.10.0+-blue" alt="python">
   <a href="https://github.com/WwwwwyDev/crawlist/stargazers"><img src="https://img.shields.io/github/stars/WwwwwyDev/crawlist" alt="GitHub stars"style="max-width: 100%;">
   </a>
   <br/>
 </p>
 </div>
 
 
 ## introduction
 
-You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.\
-Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
+You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
 
 ## installing
 You can use pip or pip3 to install the crawlist\
 `pip install crawlist` or `pip3 install crawlist`
 
 ## quickly start
 This is a static website demo. It does not use the JavaScript to load the data.
@@ -85,8 +84,8 @@
 ```
 
 ## Documenting
 If you are interested and would like to see more detailed documentation, please click on the picture below.\
  <a href="https://wwydev.gitbook.io/crawlist/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:220px; height:100px" ></a>
 
 ## Contributing
-Please submit pull requests to the develop branch
+Please submit pull requests to the develop branch
```

### Comparing `crawlist-0.0.5/crawlist/analyzers/analyzer.py` & `crawlist-0.0.6/crawlist/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/analyzers/driver.py` & `crawlist-0.0.6/crawlist/analyzers/driver.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/analyzers/pager/dynamic_pager.py` & `crawlist-0.0.6/crawlist/analyzers/pager/dynamic_pager.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/analyzers/pager/pager.py` & `crawlist-0.0.6/crawlist/analyzers/pager/pager.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/analyzers/pager/static_pager.py` & `crawlist-0.0.6/crawlist/analyzers/pager/static_pager.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/analyzers/request.py` & `crawlist-0.0.6/crawlist/analyzers/request.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/analyzers/selector.py` & `crawlist-0.0.6/crawlist/analyzers/selector.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/analyzers/trie.py` & `crawlist-0.0.6/crawlist/analyzers/trie.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/analyzers/valid.py` & `crawlist-0.0.6/crawlist/analyzers/valid.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/annotation.py` & `crawlist-0.0.6/crawlist/annotation.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/processings/action.py` & `crawlist-0.0.6/crawlist/processings/action.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist/processings/script.py` & `crawlist-0.0.6/crawlist/processings/script.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/crawlist.egg-info/PKG-INFO` & `crawlist-0.0.6/crawlist.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: crawlist
-Version: 0.0.5
+Version: 0.0.6
 Summary: A universal solution for web crawling lists
 Home-page: https://github.com/WwwwwyDev/crawlist
 Author: WwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: parsel
 Requires-Dist: selenium>=4.0.0
 Requires-Dist: cssselect
 Requires-Dist: lxml
 Requires-Dist: requests
@@ -37,26 +37,25 @@
 A universal solution for web crawling lists
 <!-- prettier-ignore-end -->
 
 <p align="center">
   <a href="https://pypi.python.org/pypi/crawlist">
     <img src="https://img.shields.io/pypi/v/crawlist" alt="pypi">
   </a>
-  <img src="https://img.shields.io/badge/python-3.8.0+-blue" alt="python">
+  <img src="https://img.shields.io/badge/python-3.10.0+-blue" alt="python">
   <a href="https://github.com/WwwwwyDev/crawlist/stargazers"><img src="https://img.shields.io/github/stars/WwwwwyDev/crawlist" alt="GitHub stars"style="max-width: 100%;">
   </a>
   <br/>
 </p>
 </div>
 
 
 ## introduction
 
-You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.\
-Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
+You can use Crawlist to crawl websites containing lists, and with some simple configurations, you can obtain all the list data.Of course, in the face of some special websites that cannot be crawled, you can also customize the configuration of that website.
 
 ## installing
 You can use pip or pip3 to install the crawlist\
 `pip install crawlist` or `pip3 install crawlist`
 
 ## quickly start
 This is a static website demo. It does not use the JavaScript to load the data.
```

### Comparing `crawlist-0.0.5/crawlist.egg-info/SOURCES.txt` & `crawlist-0.0.6/crawlist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.5/setup.py` & `crawlist-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 # Package meta-data.
 NAME = 'crawlist'
 DESCRIPTION = 'A universal solution for web crawling lists'
 URL = 'https://github.com/WwwwwyDev/crawlist'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwyDev'
-REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.5'
+REQUIRES_PYTHON = '>=3.10.0'
+VERSION = '0.0.6'
 # What packages are required for this module to be executed?
 REQUIRED = [
     'parsel', 'selenium>=4.0.0', 'cssselect', 'lxml', 'requests', 'webdriver-manager'
 ]
 
 # What packages are optional?
 EXTRAS = {
@@ -115,15 +115,15 @@
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
```

