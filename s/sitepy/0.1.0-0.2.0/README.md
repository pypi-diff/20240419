# Comparing `tmp/sitepy-0.1.0.tar.gz` & `tmp/sitepy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.1.0.tar", last modified: Thu Apr 18 21:21:52 2024, max compression
+gzip compressed data, was "sitepy-0.2.0.tar", last modified: Thu Apr 18 22:07:27 2024, max compression
```

## Comparing `sitepy-0.1.0.tar` & `sitepy-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 21:21:52.889144 sitepy-0.1.0/
--rw-rw-rw-   0        0        0      566 2024-04-18 20:48:30.000000 sitepy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1810 2024-04-18 21:21:52.888144 sitepy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-04-18 18:57:48.000000 sitepy-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 21:21:52.890145 sitepy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1081 2024-04-18 21:21:44.000000 sitepy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 21:21:52.872139 sitepy-0.1.0/sitepy/
--rw-rw-rw-   0        0        0       88 2024-04-18 20:59:01.000000 sitepy-0.1.0/sitepy/__init__.py
--rw-rw-rw-   0        0        0     3540 2024-04-18 21:20:39.000000 sitepy-0.1.0/sitepy/core.py
--rw-rw-rw-   0        0        0      250 2024-04-18 20:08:02.000000 sitepy-0.1.0/sitepy/gpt.py
--rw-rw-rw-   0        0        0    28927 2024-04-18 21:14:00.000000 sitepy-0.1.0/sitepy/profanity.py
--rw-rw-rw-   0        0        0      343 2024-04-18 20:45:59.000000 sitepy-0.1.0/sitepy/recaptcha.py
-drwxrwxrwx   0        0        0        0 2024-04-18 21:21:52.884143 sitepy-0.1.0/sitepy.egg-info/
--rw-rw-rw-   0        0        0     1810 2024-04-18 21:21:52.000000 sitepy-0.1.0/sitepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-18 21:21:52.000000 sitepy-0.1.0/sitepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 21:21:52.000000 sitepy-0.1.0/sitepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 21:21:52.000000 sitepy-0.1.0/sitepy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 22:07:27.967702 sitepy-0.2.0/
+-rw-rw-rw-   0        0        0      566 2024-04-18 20:48:30.000000 sitepy-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1810 2024-04-18 22:07:27.966702 sitepy-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-04-18 18:57:48.000000 sitepy-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 22:07:27.968703 sitepy-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2024-04-18 22:07:17.000000 sitepy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:07:27.949696 sitepy-0.2.0/sitepy/
+-rw-rw-rw-   0        0        0       88 2024-04-18 20:59:01.000000 sitepy-0.2.0/sitepy/__init__.py
+-rw-rw-rw-   0        0        0    11705 2024-04-18 22:06:17.000000 sitepy-0.2.0/sitepy/core.py
+-rw-rw-rw-   0        0        0      250 2024-04-18 20:08:02.000000 sitepy-0.2.0/sitepy/gpt.py
+-rw-rw-rw-   0        0        0    28927 2024-04-18 21:14:00.000000 sitepy-0.2.0/sitepy/profanity.py
+-rw-rw-rw-   0        0        0      343 2024-04-18 20:45:59.000000 sitepy-0.2.0/sitepy/recaptcha.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:07:27.962701 sitepy-0.2.0/sitepy.egg-info/
+-rw-rw-rw-   0        0        0     1810 2024-04-18 22:07:27.000000 sitepy-0.2.0/sitepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-18 22:07:27.000000 sitepy-0.2.0/sitepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 22:07:27.000000 sitepy-0.2.0/sitepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 22:07:27.000000 sitepy-0.2.0/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.1.0/LICENSE` & `sitepy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sitepy-0.1.0/PKG-INFO` & `sitepy-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sitepy-0.1.0/README.md` & `sitepy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sitepy-0.1.0/setup.py` & `sitepy-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.1.0',
+    version='0.2.0',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
     license='Apache 2.0',
     packages=find_packages(),
     long_description=open('sitepy/README.md').read(),
```

### Comparing `sitepy-0.1.0/sitepy/profanity.py` & `sitepy-0.2.0/sitepy/profanity.py`

 * *Files identical despite different names*

### Comparing `sitepy-0.1.0/sitepy.egg-info/PKG-INFO` & `sitepy-0.2.0/sitepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

