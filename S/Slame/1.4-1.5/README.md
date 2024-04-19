# Comparing `tmp/Slame-1.4.tar.gz` & `tmp/Slame-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slame-1.4.tar", last modified: Wed Mar 27 12:44:36 2024, max compression
+gzip compressed data, was "Slame-1.5.tar", last modified: Fri Apr 19 09:33:32 2024, max compression
```

## Comparing `Slame-1.4.tar` & `Slame-1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)        0 2024-03-27 12:44:36.254405 Slame-1.4/
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)      893 2024-03-27 12:44:36.254405 Slame-1.4/PKG-INFO
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.4/README.md
-drwxrwxr-x   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)        0 2024-03-27 12:44:36.254405 Slame-1.4/Slame/
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)      394 2024-03-27 12:44:14.000000 Slame-1.4/Slame/__init__.py
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)    12287 2024-03-27 12:44:02.000000 Slame-1.4/Slame/slame.py
-drwxrwxr-x   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)        0 2024-03-27 12:44:36.254405 Slame-1.4/Slame.egg-info/
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)      893 2024-03-27 12:44:36.000000 Slame-1.4/Slame.egg-info/PKG-INFO
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)      205 2024-03-27 12:44:36.000000 Slame-1.4/Slame.egg-info/SOURCES.txt
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)        1 2024-03-27 12:44:36.000000 Slame-1.4/Slame.egg-info/dependency_links.txt
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)       20 2024-03-27 12:44:36.000000 Slame-1.4/Slame.egg-info/requires.txt
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)        6 2024-03-27 12:44:36.000000 Slame-1.4/Slame.egg-info/top_level.txt
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)       38 2024-03-27 12:44:36.254405 Slame-1.4/setup.cfg
--rw-rw-r--   0 zhrxxgroup-dev  (1000) zhrxxgroup-dev  (1000)     1252 2024-03-27 11:27:43.000000 Slame-1.4/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-19 09:33:32.574571 Slame-1.5/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      893 2024-04-19 09:33:32.574571 Slame-1.5/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)     2112 2024-03-24 11:40:44.000000 Slame-1.5/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-19 09:33:32.574571 Slame-1.5/Slame/
+-rw-r--r--   0 dev       (1000) dev       (1000)      393 2024-04-16 18:25:06.000000 Slame-1.5/Slame/__init__.py
+-rw-r--r--   0 dev       (1000) dev       (1000)        0 2024-03-27 12:15:44.000000 Slame-1.5/Slame/menu.py
+-rw-r--r--   0 dev       (1000) dev       (1000)    12287 2024-03-27 12:44:02.000000 Slame-1.5/Slame/slame.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2024-04-19 09:33:32.574571 Slame-1.5/Slame.egg-info/
+-rw-r--r--   0 dev       (1000) dev       (1000)      893 2024-04-19 09:33:32.000000 Slame-1.5/Slame.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)      219 2024-04-19 09:33:32.000000 Slame-1.5/Slame.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        1 2024-04-19 09:33:32.000000 Slame-1.5/Slame.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       20 2024-04-19 09:33:32.000000 Slame-1.5/Slame.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        6 2024-04-19 09:33:32.000000 Slame-1.5/Slame.egg-info/top_level.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       38 2024-04-19 09:33:32.574571 Slame-1.5/setup.cfg
+-rw-r--r--   0 dev       (1000) dev       (1000)     1252 2024-04-16 18:25:43.000000 Slame-1.5/setup.py
```

### Comparing `Slame-1.4/PKG-INFO` & `Slame-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.4
+Version: 1.5
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.4/README.md` & `Slame-1.5/README.md`

 * *Files identical despite different names*

### Comparing `Slame-1.4/Slame/slame.py` & `Slame-1.5/Slame/slame.py`

 * *Files identical despite different names*

### Comparing `Slame-1.4/Slame.egg-info/PKG-INFO` & `Slame-1.5/Slame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Slame
-Version: 1.4
+Version: 1.5
 Summary: Python module for serving a web server and more
 Home-page: https://github.com/zhrexx/Slame/
 Author: ZHRXXgroup
 Author-email: info@zhrxxgroup.com
 License: MIT License, see LICENSE file
 Download-URL: https://zhrxxgroup.com/slame/download.php?file=Slame-1.3.tar.gz
 Platform: UNKNOWN
```

### Comparing `Slame-1.4/setup.py` & `Slame-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 """
 :authors: ZHRXXgroup
 :license: MIT License, see LICENSE file
 :copyright: (c) 2024 ZHRXXgroup
 """
 
-version = '1.4'
+version = '1.5'
 
 long_description  = "Slame is an Python Module for serving a webserver and in 1.2 we added Plugins you can use your own plugins in Slame or you can download plugins from other Peoples at https://zhrxxgroup.com/slame/spm/. SLAME DOCS: https://zhrxxgroup.com/slame or https://github.com/zhrexx/Slame, OUR WEBSITE: https://zhrxxgroup.com"
 
 
 
 setup(
     name="Slame",
```

