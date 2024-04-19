# Comparing `tmp/YnExchangePY-2.0.0.tar.gz` & `tmp/YnExchangePY-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YnExchangePY-2.0.0.tar", last modified: Thu Apr 11 14:31:22 2024, max compression
+gzip compressed data, was "YnExchangePY-2.5.2.tar", last modified: Fri Apr 19 14:53:39 2024, max compression
```

## Comparing `YnExchangePY-2.0.0.tar` & `YnExchangePY-2.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 14:31:22.903796 YnExchangePY-2.0.0/
--rw-rw-rw-   0        0        0     2047 2024-04-11 14:31:22.903796 YnExchangePY-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1678 2024-04-11 13:25:29.000000 YnExchangePY-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 14:31:22.872549 YnExchangePY-2.0.0/YnExchangePY.egg-info/
--rw-rw-rw-   0        0        0     2047 2024-04-11 14:31:22.000000 YnExchangePY-2.0.0/YnExchangePY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-11 14:31:22.000000 YnExchangePY-2.0.0/YnExchangePY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 14:31:22.000000 YnExchangePY-2.0.0/YnExchangePY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 14:31:22.000000 YnExchangePY-2.0.0/YnExchangePY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 14:31:22.000000 YnExchangePY-2.0.0/YnExchangePY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 14:31:22.903796 YnExchangePY-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      674 2024-04-11 14:31:05.000000 YnExchangePY-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:53:39.822461 YnExchangePY-2.5.2/
+-rw-rw-rw-   0        0        0     3732 2024-04-19 14:53:39.822461 YnExchangePY-2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3369 2024-04-19 14:49:08.000000 YnExchangePY-2.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 14:53:39.804345 YnExchangePY-2.5.2/YnExchangePY.egg-info/
+-rw-rw-rw-   0        0        0     3732 2024-04-19 14:53:38.000000 YnExchangePY-2.5.2/YnExchangePY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-19 14:53:38.000000 YnExchangePY-2.5.2/YnExchangePY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 14:53:38.000000 YnExchangePY-2.5.2/YnExchangePY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 14:53:38.000000 YnExchangePY-2.5.2/YnExchangePY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 14:53:38.000000 YnExchangePY-2.5.2/YnExchangePY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 14:53:39.822461 YnExchangePY-2.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      674 2024-04-19 14:46:26.000000 YnExchangePY-2.5.2/setup.py
```

### Comparing `YnExchangePY-2.0.0/setup.py` & `YnExchangePY-2.5.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '2.0.0'
+VERSION = '2.5.2'
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 
 # Setting up
```

