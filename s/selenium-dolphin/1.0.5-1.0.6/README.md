# Comparing `tmp/selenium_dolphin-1.0.5.tar.gz` & `tmp/selenium_dolphin-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_dolphin-1.0.5.tar", last modified: Tue Apr  2 05:34:29 2024, max compression
+gzip compressed data, was "selenium_dolphin-1.0.6.tar", last modified: Fri Apr 19 11:24:46 2024, max compression
```

## Comparing `selenium_dolphin-1.0.5.tar` & `selenium_dolphin-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 05:34:29.831496 selenium_dolphin-1.0.5/
--rw-rw-rw-   0        0        0     1080 2024-04-02 05:03:25.000000 selenium_dolphin-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      102 2024-04-02 05:28:19.000000 selenium_dolphin-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6661 2024-04-02 05:34:29.830499 selenium_dolphin-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5804 2024-04-02 05:03:25.000000 selenium_dolphin-1.0.5/README.MD
-drwxrwxrwx   0        0        0        0 2024-04-02 05:34:29.827507 selenium_dolphin-1.0.5/selenium_dolphin/
--rw-rw-rw-   0        0        0       83 2024-04-02 05:03:25.000000 selenium_dolphin-1.0.5/selenium_dolphin/__init__.py
--rw-rw-rw-   0        0        0     8144 2024-04-02 05:29:06.000000 selenium_dolphin-1.0.5/selenium_dolphin/api.py
--rw-rw-rw-   0        0        0     6395 2024-04-02 05:28:00.000000 selenium_dolphin-1.0.5/selenium_dolphin/selenium_dolphin.py
--rw-rw-rw-   0        0        0     1398 2024-04-02 05:32:35.000000 selenium_dolphin-1.0.5/selenium_dolphin/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 05:34:29.830499 selenium_dolphin-1.0.5/selenium_dolphin.egg-info/
--rw-rw-rw-   0        0        0     6661 2024-04-02 05:34:29.000000 selenium_dolphin-1.0.5/selenium_dolphin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-04-02 05:34:29.000000 selenium_dolphin-1.0.5/selenium_dolphin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 05:34:29.000000 selenium_dolphin-1.0.5/selenium_dolphin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-02 05:34:29.000000 selenium_dolphin-1.0.5/selenium_dolphin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-02 05:34:29.000000 selenium_dolphin-1.0.5/selenium_dolphin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 05:34:29.831496 selenium_dolphin-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1243 2024-04-02 05:33:20.000000 selenium_dolphin-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:24:46.507123 selenium_dolphin-1.0.6/
+-rw-rw-rw-   0        0        0     1080 2024-04-19 11:23:17.000000 selenium_dolphin-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      102 2024-04-19 11:23:17.000000 selenium_dolphin-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6661 2024-04-19 11:24:46.507123 selenium_dolphin-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5804 2024-04-19 11:23:17.000000 selenium_dolphin-1.0.6/README.MD
+drwxrwxrwx   0        0        0        0 2024-04-19 11:24:46.503144 selenium_dolphin-1.0.6/selenium_dolphin/
+-rw-rw-rw-   0        0        0       83 2024-04-19 11:23:17.000000 selenium_dolphin-1.0.6/selenium_dolphin/__init__.py
+-rw-rw-rw-   0        0        0     8144 2024-04-19 11:23:17.000000 selenium_dolphin-1.0.6/selenium_dolphin/api.py
+-rw-rw-rw-   0        0        0     6395 2024-04-19 11:23:17.000000 selenium_dolphin-1.0.6/selenium_dolphin/selenium_dolphin.py
+-rw-rw-rw-   0        0        0     1459 2024-04-19 11:23:55.000000 selenium_dolphin-1.0.6/selenium_dolphin/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:24:46.506126 selenium_dolphin-1.0.6/selenium_dolphin.egg-info/
+-rw-rw-rw-   0        0        0     6661 2024-04-19 11:24:46.000000 selenium_dolphin-1.0.6/selenium_dolphin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-04-19 11:24:46.000000 selenium_dolphin-1.0.6/selenium_dolphin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 11:24:46.000000 selenium_dolphin-1.0.6/selenium_dolphin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-19 11:24:46.000000 selenium_dolphin-1.0.6/selenium_dolphin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-19 11:24:46.000000 selenium_dolphin-1.0.6/selenium_dolphin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 11:24:46.507123 selenium_dolphin-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1243 2024-04-19 11:24:08.000000 selenium_dolphin-1.0.6/setup.py
```

### Comparing `selenium_dolphin-1.0.5/LICENSE` & `selenium_dolphin-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_dolphin-1.0.5/PKG-INFO` & `selenium_dolphin-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_dolphin
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python module for controlling Dolphin browser profiles using Selenium/Pyppeteer. It also has a Dolphin API for creating, editing, and deleting profiles.
 Home-page: https://github.com/DedInc/selenium_dolphin
 Author: Maehdakvan
 Author-email: visitanimation@google.com
 Project-URL: Bug Tracker, https://github.com/DedInc/selenium_dolphin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `selenium_dolphin-1.0.5/README.MD` & `selenium_dolphin-1.0.6/README.MD`

 * *Files identical despite different names*

### Comparing `selenium_dolphin-1.0.5/selenium_dolphin/api.py` & `selenium_dolphin-1.0.6/selenium_dolphin/api.py`

 * *Files identical despite different names*

### Comparing `selenium_dolphin-1.0.5/selenium_dolphin/selenium_dolphin.py` & `selenium_dolphin-1.0.6/selenium_dolphin/selenium_dolphin.py`

 * *Files identical despite different names*

### Comparing `selenium_dolphin-1.0.5/selenium_dolphin/utils.py` & `selenium_dolphin-1.0.6/selenium_dolphin/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,18 @@
         return os.path.expanduser('~/Library/Application Support/dolphin_anty/browser_profiles')
     else:
         return os.path.expanduser('~/.config/dolphin_anty/browser_profiles')
 
 
 def clean_if_exists(dir_to_clean):
     if os.path.exists(dir_to_clean):
-        shutil.rmtree(dir_to_clean)
+        try:
+            shutil.rmtree(dir_to_clean)
+        except OSError:
+            pass
 
 
 def collect_garbage(api=None, profile_id=None):
     profile_folder = get_profile_folder()
 
     if api is not None:
         api_profiles = []
```

### Comparing `selenium_dolphin-1.0.5/selenium_dolphin.egg-info/PKG-INFO` & `selenium_dolphin-1.0.6/selenium_dolphin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_dolphin
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python module for controlling Dolphin browser profiles using Selenium/Pyppeteer. It also has a Dolphin API for creating, editing, and deleting profiles.
 Home-page: https://github.com/DedInc/selenium_dolphin
 Author: Maehdakvan
 Author-email: visitanimation@google.com
 Project-URL: Bug Tracker, https://github.com/DedInc/selenium_dolphin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `selenium_dolphin-1.0.5/setup.py` & `selenium_dolphin-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 install_requires = ['requests', 'selenium', 'pyppeteer'] 
 if sys.platform == 'win32':
     install_requires.append('pywinauto')
 
 setup(
     name='selenium_dolphin',
-    version='1.0.5',
+    version='1.0.6',
     author='Maehdakvan',
     author_email='visitanimation@google.com',
     description='A Python module for controlling Dolphin browser profiles using Selenium/Pyppeteer. It also has a Dolphin API for creating, editing, and deleting profiles.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DedInc/selenium_dolphin',
     project_urls={
```

