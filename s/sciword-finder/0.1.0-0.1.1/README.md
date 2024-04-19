# Comparing `tmp/sciword_finder-0.1.0.tar.gz` & `tmp/sciword_finder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciword_finder-0.1.0.tar", last modified: Fri Apr 19 06:18:06 2024, max compression
+gzip compressed data, was "sciword_finder-0.1.1.tar", last modified: Fri Apr 19 06:34:25 2024, max compression
```

## Comparing `sciword_finder-0.1.0.tar` & `sciword_finder-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 06:18:06.952516 sciword_finder-0.1.0/
--rw-rw-rw-   0        0        0      373 2024-04-19 06:18:06.948134 sciword_finder-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 06:18:06.941680 sciword_finder-0.1.0/sciword-finder/
--rw-rw-rw-   0        0        0      974 2024-04-18 17:31:41.000000 sciword_finder-0.1.0/sciword-finder/__init__.py
--rw-rw-rw-   0        0        0     1925 2024-04-19 06:12:47.000000 sciword_finder-0.1.0/sciword-finder/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:18:06.948134 sciword_finder-0.1.0/sciword_finder.egg-info/
--rw-rw-rw-   0        0        0      373 2024-04-19 06:18:06.000000 sciword_finder-0.1.0/sciword_finder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-19 06:18:06.000000 sciword_finder-0.1.0/sciword_finder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 06:18:06.000000 sciword_finder-0.1.0/sciword_finder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-19 06:18:06.000000 sciword_finder-0.1.0/sciword_finder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 06:18:06.952516 sciword_finder-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      497 2024-04-18 17:38:16.000000 sciword_finder-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:34:25.931896 sciword_finder-0.1.1/
+-rw-rw-rw-   0        0        0      373 2024-04-19 06:34:25.927325 sciword_finder-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 06:34:25.917489 sciword_finder-0.1.1/sciword-finder/
+-rw-rw-rw-   0        0        0      974 2024-04-18 17:31:41.000000 sciword_finder-0.1.1/sciword-finder/__init__.py
+-rw-rw-rw-   0        0        0     1925 2024-04-19 06:12:47.000000 sciword_finder-0.1.1/sciword-finder/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:34:25.927325 sciword_finder-0.1.1/sciword_finder.egg-info/
+-rw-rw-rw-   0        0        0      373 2024-04-19 06:34:25.000000 sciword_finder-0.1.1/sciword_finder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-19 06:34:25.000000 sciword_finder-0.1.1/sciword_finder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 06:34:25.000000 sciword_finder-0.1.1/sciword_finder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-19 06:34:25.000000 sciword_finder-0.1.1/sciword_finder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-19 06:34:25.000000 sciword_finder-0.1.1/sciword_finder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 06:34:25.931896 sciword_finder-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      618 2024-04-19 06:32:22.000000 sciword_finder-0.1.1/setup.py
```

### Comparing `sciword_finder-0.1.0/sciword-finder/__init__.py` & `sciword_finder-0.1.1/sciword-finder/__init__.py`

 * *Files identical despite different names*

### Comparing `sciword_finder-0.1.0/sciword-finder/__main__.py` & `sciword_finder-0.1.1/sciword-finder/__main__.py`

 * *Files identical despite different names*

