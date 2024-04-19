# Comparing `tmp/hsadev-kit-0.0.5.tar.gz` & `tmp/hsadev_kit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsadev-kit-0.0.5.tar", last modified: Fri Feb  9 06:07:55 2024, max compression
+gzip compressed data, was "hsadev_kit-0.0.6.tar", last modified: Fri Apr 19 01:26:26 2024, max compression
```

## Comparing `hsadev-kit-0.0.5.tar` & `hsadev_kit-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-09 06:07:55.437683 hsadev-kit-0.0.5/
--rw-rw-rw-   0        0        0        0 2024-02-08 07:02:19.000000 hsadev-kit-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      692 2024-02-09 06:07:55.435684 hsadev-kit-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      104 2024-02-09 06:05:30.000000 hsadev-kit-0.0.5/README.md
--rw-rw-rw-   0        0        0      108 2024-02-08 07:09:28.000000 hsadev-kit-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-09 06:07:55.437683 hsadev-kit-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      911 2024-02-09 06:06:14.000000 hsadev-kit-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-09 06:07:55.418693 hsadev-kit-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-02-09 06:07:55.427682 hsadev-kit-0.0.5/src/hsadev/
--rw-rw-rw-   0        0        0       23 2024-02-09 06:06:14.000000 hsadev-kit-0.0.5/src/hsadev/__init__.py
--rw-rw-rw-   0        0        0     1296 2023-08-25 02:10:16.000000 hsadev-kit-0.0.5/src/hsadev/logger.py
--rw-rw-rw-   0        0        0     3092 2024-02-09 06:06:58.000000 hsadev-kit-0.0.5/src/hsadev/request.py
--rw-rw-rw-   0        0        0     1476 2024-02-02 03:53:16.000000 hsadev-kit-0.0.5/src/hsadev/util.py
-drwxrwxrwx   0        0        0        0 2024-02-09 06:07:55.434682 hsadev-kit-0.0.5/src/hsadev_kit.egg-info/
--rw-rw-rw-   0        0        0      692 2024-02-09 06:07:55.000000 hsadev-kit-0.0.5/src/hsadev_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-02-09 06:07:55.000000 hsadev-kit-0.0.5/src/hsadev_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-09 06:07:55.000000 hsadev-kit-0.0.5/src/hsadev_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-02-09 06:07:55.000000 hsadev-kit-0.0.5/src/hsadev_kit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-09 06:07:55.000000 hsadev-kit-0.0.5/src/hsadev_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 01:26:26.311688 hsadev_kit-0.0.6/
+-rw-rw-rw-   0        0        0        0 2024-02-08 07:02:19.000000 hsadev_kit-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      725 2024-04-19 01:26:26.309976 hsadev_kit-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      135 2024-04-19 01:25:38.000000 hsadev_kit-0.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2024-02-08 07:09:28.000000 hsadev_kit-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 01:26:26.311688 hsadev_kit-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      911 2024-04-19 01:25:53.000000 hsadev_kit-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 01:26:26.290408 hsadev_kit-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 01:26:26.298425 hsadev_kit-0.0.6/src/hsadev/
+-rw-rw-rw-   0        0        0       23 2024-04-19 01:25:38.000000 hsadev_kit-0.0.6/src/hsadev/__init__.py
+-rw-rw-rw-   0        0        0     1296 2023-08-25 02:10:16.000000 hsadev_kit-0.0.6/src/hsadev/logger.py
+-rw-rw-rw-   0        0        0     3092 2024-04-19 01:24:02.000000 hsadev_kit-0.0.6/src/hsadev/request.py
+-rw-rw-rw-   0        0        0     1476 2024-02-02 03:53:16.000000 hsadev_kit-0.0.6/src/hsadev/util.py
+drwxrwxrwx   0        0        0        0 2024-04-19 01:26:26.308447 hsadev_kit-0.0.6/src/hsadev_kit.egg-info/
+-rw-rw-rw-   0        0        0      725 2024-04-19 01:26:26.000000 hsadev_kit-0.0.6/src/hsadev_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-04-19 01:26:26.000000 hsadev_kit-0.0.6/src/hsadev_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 01:26:26.000000 hsadev_kit-0.0.6/src/hsadev_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-19 01:26:26.000000 hsadev_kit-0.0.6/src/hsadev_kit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-19 01:26:26.000000 hsadev_kit-0.0.6/src/hsadev_kit.egg-info/top_level.txt
```

### Comparing `hsadev-kit-0.0.5/PKG-INFO` & `hsadev_kit-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsadev-kit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for personal
 Home-page: http://dev.secuman.com/secuman/hsadev_kit
 Author: secuman83
 Author-email: secuman83@outlook.com
 Project-URL: Bug Tracker, http://dev.secuman.com/secuman/hsadev_kit/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,9 +19,10 @@
 # hsadev_kit
 
 
 
 ## For personal use.
 
 ## Revision
-[0.0.4] Begin
+[0.0.4] Begin.  
 [0.0.5] Fixed encoding errors.
+[0.0.6] Fixed parsing error.
```

### Comparing `hsadev-kit-0.0.5/setup.py` & `hsadev_kit-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hsadev-kit",
-    version="0.0.5",
+    version="0.0.6",
     author="secuman83",
     author_email="secuman83@outlook.com",
     description="Package for personal",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://dev.secuman.com/secuman/hsadev_kit",
     project_urls={
```

### Comparing `hsadev-kit-0.0.5/src/hsadev/logger.py` & `hsadev_kit-0.0.6/src/hsadev/logger.py`

 * *Files identical despite different names*

### Comparing `hsadev-kit-0.0.5/src/hsadev/request.py` & `hsadev_kit-0.0.6/src/hsadev/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             raise Exception('Invalid response status: {}'.format(response.status_code))
 
         if 'Set-Cookie' in response.headers:
             set_cookie = response.headers.get('Set-Cookie')
             self.__headers['Cookie'] = set_cookie
 
         if 'Content-Type' in response.headers:
-            if response.headers.get('Content-Type') == 'text/html':
+            if 'text/html' in response.headers.get('Content-Type'):
                 response = BeautifulSoup(response.text.encode(response.encoding), 'html.parser')
 
         return response
 
     # public functions
     def set_header(self, headers, clear=True, save_cookie=False):
         if save_cookie and 'Cookie' in self.__headers:
```

### Comparing `hsadev-kit-0.0.5/src/hsadev/util.py` & `hsadev_kit-0.0.6/src/hsadev/util.py`

 * *Files identical despite different names*

### Comparing `hsadev-kit-0.0.5/src/hsadev_kit.egg-info/PKG-INFO` & `hsadev_kit-0.0.6/src/hsadev_kit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsadev-kit
-Version: 0.0.5
+Version: 0.0.6
 Summary: Package for personal
 Home-page: http://dev.secuman.com/secuman/hsadev_kit
 Author: secuman83
 Author-email: secuman83@outlook.com
 Project-URL: Bug Tracker, http://dev.secuman.com/secuman/hsadev_kit/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,9 +19,10 @@
 # hsadev_kit
 
 
 
 ## For personal use.
 
 ## Revision
-[0.0.4] Begin
+[0.0.4] Begin.  
 [0.0.5] Fixed encoding errors.
+[0.0.6] Fixed parsing error.
```

