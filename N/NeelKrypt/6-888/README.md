# Comparing `tmp/NeelKrypt-6.tar.gz` & `tmp/NeelKrypt-888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeelKrypt-6.tar", last modified: Fri Apr 19 06:38:52 2024, max compression
+gzip compressed data, was "NeelKrypt-888.tar", last modified: Fri Apr 19 06:44:49 2024, max compression
```

## Comparing `NeelKrypt-6.tar` & `NeelKrypt-888.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 06:38:52.345853 NeelKrypt-6/
-drwxrwxrwx   0        0        0        0 2024-04-19 06:38:52.339765 NeelKrypt-6/NeelKrypt/
--rw-rw-rw-   0        0        0       17 2024-04-19 06:34:00.000000 NeelKrypt-6/NeelKrypt/__init__.py
--rw-rw-rw-   0        0        0     1565 2024-04-19 06:37:43.000000 NeelKrypt-6/NeelKrypt/b.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:38:52.343831 NeelKrypt-6/NeelKrypt.egg-info/
--rw-rw-rw-   0        0        0      390 2024-04-19 06:38:52.000000 NeelKrypt-6/NeelKrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-04-19 06:38:52.000000 NeelKrypt-6/NeelKrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 06:38:52.000000 NeelKrypt-6/NeelKrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-19 06:38:52.000000 NeelKrypt-6/NeelKrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-19 06:38:52.000000 NeelKrypt-6/NeelKrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      390 2024-04-19 06:38:52.344846 NeelKrypt-6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-19 06:38:52.345853 NeelKrypt-6/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-19 06:38:37.000000 NeelKrypt-6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:44:49.646248 NeelKrypt-888/
+drwxrwxrwx   0        0        0        0 2024-04-19 06:44:49.640110 NeelKrypt-888/NeelKrypt/
+-rw-rw-rw-   0        0        0       21 2024-04-19 06:42:39.000000 NeelKrypt-888/NeelKrypt/__init__.py
+-rw-rw-rw-   0        0        0     1565 2024-04-19 06:37:43.000000 NeelKrypt-888/NeelKrypt/b.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:44:49.644734 NeelKrypt-888/NeelKrypt.egg-info/
+-rw-rw-rw-   0        0        0      392 2024-04-19 06:44:49.000000 NeelKrypt-888/NeelKrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-19 06:44:49.000000 NeelKrypt-888/NeelKrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 06:44:49.000000 NeelKrypt-888/NeelKrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 06:44:49.000000 NeelKrypt-888/NeelKrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 06:44:49.000000 NeelKrypt-888/NeelKrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      392 2024-04-19 06:44:49.645741 NeelKrypt-888/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-19 06:44:49.646248 NeelKrypt-888/setup.cfg
+-rw-rw-rw-   0        0        0      924 2024-04-19 06:44:37.000000 NeelKrypt-888/setup.py
```

### Comparing `NeelKrypt-6/NeelKrypt/b.py` & `NeelKrypt-888/NeelKrypt/b.py`

 * *Files identical despite different names*

### Comparing `NeelKrypt-6/setup.py` & `NeelKrypt-888/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '6' 
+VERSION = '888' 
 DESCRIPTION = 'Text Enkryptor and Dekryptor using PKI'
 LONG_DESCRIPTION = 'USES DIFFIE HELLMAN @ CORE . KEY HANDLING AND CONVERSION IS THE ART HERE'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="NeelKrypt",
```

