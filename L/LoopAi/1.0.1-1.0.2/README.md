# Comparing `tmp/LoopAi-1.0.1.tar.gz` & `tmp/LoopAi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LoopAi-1.0.1.tar", last modified: Thu Apr 18 19:56:59 2024, max compression
+gzip compressed data, was "LoopAi-1.0.2.tar", last modified: Thu Apr 18 20:43:13 2024, max compression
```

## Comparing `LoopAi-1.0.1.tar` & `LoopAi-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:56:59.828822 LoopAi-1.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:56:59.824823 LoopAi-1.0.1/LoopAi/
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-18 19:17:58.000000 LoopAi-1.0.1/LoopAi/LoopAi.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-18 19:53:35.000000 LoopAi-1.0.1/LoopAi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 19:56:59.828822 LoopAi-1.0.1/LoopAi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      636 2024-04-18 19:56:59.000000 LoopAi-1.0.1/LoopAi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      193 2024-04-18 19:56:59.000000 LoopAi-1.0.1/LoopAi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 19:56:59.000000 LoopAi-1.0.1/LoopAi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-18 19:56:59.000000 LoopAi-1.0.1/LoopAi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-18 19:56:59.000000 LoopAi-1.0.1/LoopAi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      636 2024-04-18 19:56:59.828822 LoopAi-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 19:56:59.828822 LoopAi-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      795 2024-04-18 19:55:58.000000 LoopAi-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:43:13.023388 LoopAi-1.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:43:13.023388 LoopAi-1.0.2/LoopAi/
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-18 20:42:25.000000 LoopAi-1.0.2/LoopAi/LoopAi.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-18 19:53:35.000000 LoopAi-1.0.2/LoopAi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:43:13.023388 LoopAi-1.0.2/LoopAi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      636 2024-04-18 20:43:12.000000 LoopAi-1.0.2/LoopAi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      193 2024-04-18 20:43:12.000000 LoopAi-1.0.2/LoopAi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 20:43:12.000000 LoopAi-1.0.2/LoopAi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-18 20:43:12.000000 LoopAi-1.0.2/LoopAi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-18 20:43:12.000000 LoopAi-1.0.2/LoopAi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      636 2024-04-18 20:43:13.023388 LoopAi-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 20:43:13.023388 LoopAi-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      795 2024-04-18 20:41:13.000000 LoopAi-1.0.2/setup.py
```

### Comparing `LoopAi-1.0.1/LoopAi/LoopAi.py` & `LoopAi-1.0.2/LoopAi/LoopAi.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,20 @@
         else:
             return f"Error: {response.status_code}"
     
     def gemini(self, query):
         return self.make_request("Gemini.php", query)
     
     def worm(self, query):
-        return self.make_request("WormGpt.php", query)
+        return self.make_request("Wormgpt.php", query)
     
     def loop(self, query):
         return self.make_request("LoopGpt.php", query)
     
     def blackbox(self, mode, query):
         mode = mode.lower()
         modes = ["python", "java", "html", "android", "flutter", "javascript"]
         if mode not in modes:
             return "Unknown mode"
         
-        endpoint = f"BlackBoxAi.php?mode={mode}&message="
-        return self.make_request(endpoint, query)
+        endpoint = f"BlackBoxai.php?mode={mode}&message="
+        return self.make_request(endpoint, query)
```

### Comparing `LoopAi-1.0.1/LoopAi.egg-info/PKG-INFO` & `LoopAi-1.0.2/LoopAi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LoopAi
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python libary that gives you access to a set of Ai models including WormGpt , Gemini , blackbox and more
 Home-page: UNKNOWN
 Author: DarkLoop (Organisation)
 Author-email: <private.e.m.a.i.l.0.0.0.1.0.1.0.0.0.1@gmail.com>
 License: UNKNOWN
 Keywords: python,Ai,Text_Models
 Platform: UNKNOWN
```

### Comparing `LoopAi-1.0.1/PKG-INFO` & `LoopAi-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LoopAi
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python libary that gives you access to a set of Ai models including WormGpt , Gemini , blackbox and more
 Home-page: UNKNOWN
 Author: DarkLoop (Organisation)
 Author-email: <private.e.m.a.i.l.0.0.0.1.0.1.0.0.0.1@gmail.com>
 License: UNKNOWN
 Keywords: python,Ai,Text_Models
 Platform: UNKNOWN
```

### Comparing `LoopAi-1.0.1/setup.py` & `LoopAi-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'A python libary that gives you access to a set of Ai models including WormGpt , Gemini , blackbox and more'
 
 # Setting up
 setup(
     name="LoopAi",
     version=VERSION,
     author="DarkLoop (Organisation)",
```

