# Comparing `tmp/lyk-reservation-nowon-0.0.1.tar.gz` & `tmp/lyk-reservation-nowon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyk-reservation-nowon-0.0.1.tar", last modified: Fri Apr 19 07:01:37 2024, max compression
+gzip compressed data, was "lyk-reservation-nowon-0.0.2.tar", last modified: Fri Apr 19 07:16:36 2024, max compression
```

## Comparing `lyk-reservation-nowon-0.0.1.tar` & `lyk-reservation-nowon-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:01:37.296331 lyk-reservation-nowon-0.0.1/
--rw-rw-rw-   0        0        0      525 2024-04-19 07:01:37.295333 lyk-reservation-nowon-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 07:01:37.288352 lyk-reservation-nowon-0.0.1/lyk_reservation_nowon.egg-info/
--rw-rw-rw-   0        0        0      525 2024-04-19 07:01:36.000000 lyk-reservation-nowon-0.0.1/lyk_reservation_nowon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-04-19 07:01:37.000000 lyk-reservation-nowon-0.0.1/lyk_reservation_nowon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:01:36.000000 lyk-reservation-nowon-0.0.1/lyk_reservation_nowon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-19 07:01:36.000000 lyk-reservation-nowon-0.0.1/lyk_reservation_nowon.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       61 2024-04-19 07:01:36.000000 lyk-reservation-nowon-0.0.1/lyk_reservation_nowon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 07:01:36.000000 lyk-reservation-nowon-0.0.1/lyk_reservation_nowon.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 07:01:37.293340 lyk-reservation-nowon-0.0.1/reservation/
--rw-rw-rw-   0        0        0       21 2024-04-19 06:02:26.000000 lyk-reservation-nowon-0.0.1/reservation/__init__.py
--rw-rw-rw-   0        0        0    10551 2024-04-19 04:52:07.000000 lyk-reservation-nowon-0.0.1/reservation/reservation.py
--rw-rw-rw-   0        0        0       42 2024-04-19 07:01:37.298324 lyk-reservation-nowon-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      798 2024-04-19 06:33:42.000000 lyk-reservation-nowon-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:36.711475 lyk-reservation-nowon-0.0.2/
+-rw-rw-rw-   0        0        0      525 2024-04-19 07:16:36.710478 lyk-reservation-nowon-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:36.704494 lyk-reservation-nowon-0.0.2/lyk_reservation_nowon.egg-info/
+-rw-rw-rw-   0        0        0      525 2024-04-19 07:16:36.000000 lyk-reservation-nowon-0.0.2/lyk_reservation_nowon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-04-19 07:16:36.000000 lyk-reservation-nowon-0.0.2/lyk_reservation_nowon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:16:36.000000 lyk-reservation-nowon-0.0.2/lyk_reservation_nowon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 07:16:36.000000 lyk-reservation-nowon-0.0.2/lyk_reservation_nowon.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       56 2024-04-19 07:16:36.000000 lyk-reservation-nowon-0.0.2/lyk_reservation_nowon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-19 07:16:36.000000 lyk-reservation-nowon-0.0.2/lyk_reservation_nowon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 07:16:36.708484 lyk-reservation-nowon-0.0.2/reservation/
+-rw-rw-rw-   0        0        0       21 2024-04-19 07:16:16.000000 lyk-reservation-nowon-0.0.2/reservation/__init__.py
+-rw-rw-rw-   0        0        0    10551 2024-04-19 04:52:07.000000 lyk-reservation-nowon-0.0.2/reservation/reservation.py
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:16:36.711475 lyk-reservation-nowon-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      790 2024-04-19 07:16:14.000000 lyk-reservation-nowon-0.0.2/setup.py
```

### Comparing `lyk-reservation-nowon-0.0.1/PKG-INFO` & `lyk-reservation-nowon-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyk-reservation-nowon
-Version: 0.0.1
+Version: 0.0.2
 Summary: lyk-reservation-nowon
 Author: officeyongki
 Author-email: officeyongki@gmail.com
 Keywords: reservation,lyk,pypi
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lyk-reservation-nowon-0.0.1/lyk_reservation_nowon.egg-info/PKG-INFO` & `lyk-reservation-nowon-0.0.2/lyk_reservation_nowon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyk-reservation-nowon
-Version: 0.0.1
+Version: 0.0.2
 Summary: lyk-reservation-nowon
 Author: officeyongki
 Author-email: officeyongki@gmail.com
 Keywords: reservation,lyk,pypi
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lyk-reservation-nowon-0.0.1/reservation/reservation.py` & `lyk-reservation-nowon-0.0.2/reservation/reservation.py`

 * *Files identical despite different names*

### Comparing `lyk-reservation-nowon-0.0.1/setup.py` & `lyk-reservation-nowon-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lyk-reservation-nowon',
-    version='0.0.1',
+    version='0.0.2',
     description='lyk-reservation-nowon',
     author='officeyongki',
     author_email='officeyongki@gmail.com',
-    install_requires=['datetime', 'time', 'pyperclip', 'threading', 'selenium', 'webdriver_manager'],
+    install_requires=['datetime', 'pyperclip', 'threading', 'selenium', 'webdriver_manager'],
     packages=find_packages(exclude=[]),
     keywords=['reservation', 'lyk', 'pypi'],
     python_requires='>=3.10',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
```

