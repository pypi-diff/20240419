# Comparing `tmp/th-influx-sdk-1.0.0.tar.gz` & `tmp/th-influx-sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th-influx-sdk-1.0.0.tar", last modified: Fri Apr 19 07:06:54 2024, max compression
+gzip compressed data, was "th-influx-sdk-1.0.1.tar", last modified: Fri Apr 19 07:13:02 2024, max compression
```

## Comparing `th-influx-sdk-1.0.0.tar` & `th-influx-sdk-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:06:54.210985 th-influx-sdk-1.0.0/
--rw-rw-rw-   0        0        0      370 2024-04-19 07:06:54.209025 th-influx-sdk-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 07:06:54.200050 th-influx-sdk-1.0.0/ThInfluxSDK/
--rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.0/ThInfluxSDK/__init__.py
--rw-rw-rw-   0        0        0     6934 2024-04-19 05:42:36.000000 th-influx-sdk-1.0.0/ThInfluxSDK/influxSDK.py
--rw-rw-rw-   0        0        0       42 2024-04-19 07:06:54.210985 th-influx-sdk-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      519 2024-04-19 07:06:37.000000 th-influx-sdk-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 07:06:54.207993 th-influx-sdk-1.0.0/th_influx_sdk.egg-info/
--rw-rw-rw-   0        0        0      370 2024-04-19 07:06:54.000000 th-influx-sdk-1.0.0/th_influx_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-19 07:06:54.000000 th-influx-sdk-1.0.0/th_influx_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:06:54.000000 th-influx-sdk-1.0.0/th_influx_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-19 07:06:54.000000 th-influx-sdk-1.0.0/th_influx_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 07:06:54.000000 th-influx-sdk-1.0.0/th_influx_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 07:13:02.375416 th-influx-sdk-1.0.1/
+-rw-rw-rw-   0        0        0      377 2024-04-19 07:13:02.372419 th-influx-sdk-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       39 2024-04-19 06:33:19.000000 th-influx-sdk-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 07:13:02.363427 th-influx-sdk-1.0.1/ThInfluxSDK/
+-rw-rw-rw-   0        0        0       25 2024-04-19 05:50:15.000000 th-influx-sdk-1.0.1/ThInfluxSDK/__init__.py
+-rw-rw-rw-   0        0        0     6934 2024-04-19 05:42:36.000000 th-influx-sdk-1.0.1/ThInfluxSDK/influxSDK.py
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:13:02.375416 th-influx-sdk-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      526 2024-04-19 07:12:56.000000 th-influx-sdk-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:13:02.372419 th-influx-sdk-1.0.1/th_influx_sdk.egg-info/
+-rw-rw-rw-   0        0        0      377 2024-04-19 07:13:02.000000 th-influx-sdk-1.0.1/th_influx_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-19 07:13:02.000000 th-influx-sdk-1.0.1/th_influx_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:13:02.000000 th-influx-sdk-1.0.1/th_influx_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-19 07:13:02.000000 th-influx-sdk-1.0.1/th_influx_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-19 07:13:02.000000 th-influx-sdk-1.0.1/th_influx_sdk.egg-info/top_level.txt
```

### Comparing `th-influx-sdk-1.0.0/ThInfluxSDK/influxSDK.py` & `th-influx-sdk-1.0.1/ThInfluxSDK/influxSDK.py`

 * *Files identical despite different names*

### Comparing `th-influx-sdk-1.0.0/setup.py` & `th-influx-sdk-1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name='th-influx-sdk',
-    version='1.0.0',
+    version='1.0.1',
     description='A SDK for influxDb',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='xiongyi',
     author_email='15679191752@163.com',
     packages=find_packages(),
     install_requires=[
         'influxdb',
         'typing',
-        'dateutil',
+        'dateutil==2.9.0',
         'datetime',
         'collections',
         'json'
     ]
 )
```

