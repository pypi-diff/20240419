# Comparing `tmp/lyk-reservation-nowon-0.0.6.tar.gz` & `tmp/lyk-reservation-nowon-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyk-reservation-nowon-0.0.6.tar", last modified: Fri Apr 19 07:37:54 2024, max compression
+gzip compressed data, was "lyk-reservation-nowon-0.0.7.tar", last modified: Fri Apr 19 07:41:42 2024, max compression
```

## Comparing `lyk-reservation-nowon-0.0.6.tar` & `lyk-reservation-nowon-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:37:54.391685 lyk-reservation-nowon-0.0.6/
--rw-rw-rw-   0        0        0      525 2024-04-19 07:37:54.391685 lyk-reservation-nowon-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 07:37:54.384702 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/
--rw-rw-rw-   0        0        0      525 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       37 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 07:37:54.389690 lyk-reservation-nowon-0.0.6/reservation/
--rw-rw-rw-   0        0        0       21 2024-04-19 07:37:12.000000 lyk-reservation-nowon-0.0.6/reservation/__init__.py
--rw-rw-rw-   0        0        0    10551 2024-04-19 04:52:07.000000 lyk-reservation-nowon-0.0.6/reservation/reservation.py
--rw-rw-rw-   0        0        0       42 2024-04-19 07:37:54.392681 lyk-reservation-nowon-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      795 2024-04-19 07:36:58.000000 lyk-reservation-nowon-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:41:42.047907 lyk-reservation-nowon-0.0.7/
+-rw-rw-rw-   0        0        0      525 2024-04-19 07:41:42.045912 lyk-reservation-nowon-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 07:41:42.041922 lyk-reservation-nowon-0.0.7/lyk_reservation_nowon.egg-info/
+-rw-rw-rw-   0        0        0      525 2024-04-19 07:41:41.000000 lyk-reservation-nowon-0.0.7/lyk_reservation_nowon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-19 07:41:41.000000 lyk-reservation-nowon-0.0.7/lyk_reservation_nowon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:41:41.000000 lyk-reservation-nowon-0.0.7/lyk_reservation_nowon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 07:41:41.000000 lyk-reservation-nowon-0.0.7/lyk_reservation_nowon.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2024-04-19 07:41:41.000000 lyk-reservation-nowon-0.0.7/lyk_reservation_nowon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:41:41.000000 lyk-reservation-nowon-0.0.7/lyk_reservation_nowon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:41:42.047907 lyk-reservation-nowon-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      795 2024-04-19 07:41:33.000000 lyk-reservation-nowon-0.0.7/setup.py
```

### Comparing `lyk-reservation-nowon-0.0.6/PKG-INFO` & `lyk-reservation-nowon-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyk-reservation-nowon
-Version: 0.0.6
+Version: 0.0.7
 Summary: lyk-reservation-nowon
 Author: officeyongki
 Author-email: officeyongki@gmail.com
 Keywords: reservation,lyk,pypi
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/PKG-INFO` & `lyk-reservation-nowon-0.0.7/lyk_reservation_nowon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyk-reservation-nowon
-Version: 0.0.6
+Version: 0.0.7
 Summary: lyk-reservation-nowon
 Author: officeyongki
 Author-email: officeyongki@gmail.com
 Keywords: reservation,lyk,pypi
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lyk-reservation-nowon-0.0.6/setup.py` & `lyk-reservation-nowon-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lyk-reservation-nowon',
-    version='0.0.6',
+    version='0.0.7',
     description='lyk-reservation-nowon',
     author='officeyongki',
     author_email='officeyongki@gmail.com',
     install_requires=['pyperclip', 'selenium', 'webdriver_manager'],
     packages=find_packages(include=['reservation', 'reservation.*']),
     keywords=['reservation', 'lyk', 'pypi'],
     python_requires='>=3.10',
```

