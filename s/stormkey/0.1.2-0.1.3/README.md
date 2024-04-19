# Comparing `tmp/stormkey-0.1.2.tar.gz` & `tmp/stormkey-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stormkey-0.1.2.tar", last modified: Fri Apr 19 19:42:07 2024, max compression
+gzip compressed data, was "stormkey-0.1.3.tar", last modified: Fri Apr 19 20:44:55 2024, max compression
```

## Comparing `stormkey-0.1.2.tar` & `stormkey-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:07.721714 stormkey-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 19:41:51.000000 stormkey-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-19 19:42:07.721714 stormkey-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 19:41:51.000000 stormkey-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:42:07.721714 stormkey-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 19:41:51.000000 stormkey-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:07.721714 stormkey-0.1.2/stormkey/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 19:41:51.000000 stormkey-0.1.2/stormkey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-19 19:41:51.000000 stormkey-0.1.2/stormkey/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:42:07.721714 stormkey-0.1.2/stormkey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-19 19:42:07.000000 stormkey-0.1.2/stormkey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 19:42:07.000000 stormkey-0.1.2/stormkey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:42:07.000000 stormkey-0.1.2/stormkey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 19:42:07.000000 stormkey-0.1.2/stormkey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:44:55.688301 stormkey-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 20:44:39.000000 stormkey-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-19 20:44:55.688301 stormkey-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 20:44:39.000000 stormkey-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:44:55.688301 stormkey-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-19 20:44:39.000000 stormkey-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:44:55.688301 stormkey-0.1.3/stormkey/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 20:44:39.000000 stormkey-0.1.3/stormkey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-19 20:44:39.000000 stormkey-0.1.3/stormkey/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:44:55.688301 stormkey-0.1.3/stormkey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-19 20:44:55.000000 stormkey-0.1.3/stormkey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 20:44:55.000000 stormkey-0.1.3/stormkey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:44:55.000000 stormkey-0.1.3/stormkey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 20:44:55.000000 stormkey-0.1.3/stormkey.egg-info/top_level.txt
```

### Comparing `stormkey-0.1.2/LICENSE` & `stormkey-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stormkey-0.1.2/PKG-INFO` & `stormkey-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormkey
-Version: 0.1.2
+Version: 0.1.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Stormkey
 
 ## Introduction
```

### Comparing `stormkey-0.1.2/README.md` & `stormkey-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `stormkey-0.1.2/stormkey.egg-info/PKG-INFO` & `stormkey-0.1.3/stormkey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormkey
-Version: 0.1.2
+Version: 0.1.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Stormkey
 
 ## Introduction
```

