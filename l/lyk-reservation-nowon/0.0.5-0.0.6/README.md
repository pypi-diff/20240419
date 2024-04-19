# Comparing `tmp/lyk-reservation-nowon-0.0.5.tar.gz` & `tmp/lyk-reservation-nowon-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyk-reservation-nowon-0.0.5.tar", last modified: Fri Apr 19 07:24:43 2024, max compression
+gzip compressed data, was "lyk-reservation-nowon-0.0.6.tar", last modified: Fri Apr 19 07:37:54 2024, max compression
```

## Comparing `lyk-reservation-nowon-0.0.5.tar` & `lyk-reservation-nowon-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 07:24:43.527818 lyk-reservation-nowon-0.0.5/
--rw-rw-rw-   0        0        0      525 2024-04-19 07:24:43.526819 lyk-reservation-nowon-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 07:24:43.521834 lyk-reservation-nowon-0.0.5/lyk_reservation_nowon.egg-info/
--rw-rw-rw-   0        0        0      525 2024-04-19 07:24:43.000000 lyk-reservation-nowon-0.0.5/lyk_reservation_nowon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-04-19 07:24:43.000000 lyk-reservation-nowon-0.0.5/lyk_reservation_nowon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 07:24:43.000000 lyk-reservation-nowon-0.0.5/lyk_reservation_nowon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-19 07:24:43.000000 lyk-reservation-nowon-0.0.5/lyk_reservation_nowon.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       37 2024-04-19 07:24:43.000000 lyk-reservation-nowon-0.0.5/lyk_reservation_nowon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 07:24:43.000000 lyk-reservation-nowon-0.0.5/lyk_reservation_nowon.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 07:24:43.525822 lyk-reservation-nowon-0.0.5/reservation/
--rw-rw-rw-   0        0        0       21 2024-04-19 07:24:30.000000 lyk-reservation-nowon-0.0.5/reservation/__init__.py
--rw-rw-rw-   0        0        0    10551 2024-04-19 04:52:07.000000 lyk-reservation-nowon-0.0.5/reservation/reservation.py
--rw-rw-rw-   0        0        0       42 2024-04-19 07:24:43.528813 lyk-reservation-nowon-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-04-19 07:24:26.000000 lyk-reservation-nowon-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:37:54.391685 lyk-reservation-nowon-0.0.6/
+-rw-rw-rw-   0        0        0      525 2024-04-19 07:37:54.391685 lyk-reservation-nowon-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 07:37:54.384702 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/
+-rw-rw-rw-   0        0        0      525 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-19 07:37:54.000000 lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 07:37:54.389690 lyk-reservation-nowon-0.0.6/reservation/
+-rw-rw-rw-   0        0        0       21 2024-04-19 07:37:12.000000 lyk-reservation-nowon-0.0.6/reservation/__init__.py
+-rw-rw-rw-   0        0        0    10551 2024-04-19 04:52:07.000000 lyk-reservation-nowon-0.0.6/reservation/reservation.py
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:37:54.392681 lyk-reservation-nowon-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      795 2024-04-19 07:36:58.000000 lyk-reservation-nowon-0.0.6/setup.py
```

### Comparing `lyk-reservation-nowon-0.0.5/PKG-INFO` & `lyk-reservation-nowon-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyk-reservation-nowon
-Version: 0.0.5
+Version: 0.0.6
 Summary: lyk-reservation-nowon
 Author: officeyongki
 Author-email: officeyongki@gmail.com
 Keywords: reservation,lyk,pypi
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lyk-reservation-nowon-0.0.5/lyk_reservation_nowon.egg-info/PKG-INFO` & `lyk-reservation-nowon-0.0.6/lyk_reservation_nowon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyk-reservation-nowon
-Version: 0.0.5
+Version: 0.0.6
 Summary: lyk-reservation-nowon
 Author: officeyongki
 Author-email: officeyongki@gmail.com
 Keywords: reservation,lyk,pypi
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lyk-reservation-nowon-0.0.5/reservation/reservation.py` & `lyk-reservation-nowon-0.0.6/reservation/reservation.py`

 * *Files identical despite different names*

### Comparing `lyk-reservation-nowon-0.0.5/setup.py` & `lyk-reservation-nowon-0.0.6/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lyk-reservation-nowon',
-    version='0.0.5',
+    version='0.0.6',
     description='lyk-reservation-nowon',
     author='officeyongki',
     author_email='officeyongki@gmail.com',
     install_requires=['pyperclip', 'selenium', 'webdriver_manager'],
-    packages=find_packages(exclude=[]),
+    packages=find_packages(include=['reservation', 'reservation.*']),
     keywords=['reservation', 'lyk', 'pypi'],
     python_requires='>=3.10',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

