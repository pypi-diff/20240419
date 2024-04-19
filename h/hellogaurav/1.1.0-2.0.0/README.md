# Comparing `tmp/hellogaurav-1.1.0.tar.gz` & `tmp/hellogaurav-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hellogaurav-1.1.0.tar", last modified: Fri Apr 19 11:08:57 2024, max compression
+gzip compressed data, was "dist\hellogaurav-2.0.0.tar", last modified: Fri Apr 19 11:07:45 2024, max compression
```

## Comparing `hellogaurav-1.1.0.tar` & `hellogaurav-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 11:08:57.835109 hellogaurav-1.1.0/
--rw-rw-rw-   0        0        0        0 2024-04-19 10:27:33.000000 hellogaurav-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      193 2024-04-19 11:08:57.832384 hellogaurav-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 10:27:45.000000 hellogaurav-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 11:08:57.774743 hellogaurav-1.1.0/hellogaurav/
--rw-rw-rw-   0        0        0        0 2024-04-19 10:26:21.000000 hellogaurav-1.1.0/hellogaurav/__init__.py
--rw-rw-rw-   0        0        0       14 2024-04-19 10:26:44.000000 hellogaurav-1.1.0/hellogaurav/hello.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:08:57.830306 hellogaurav-1.1.0/hellogaurav.egg-info/
--rw-rw-rw-   0        0        0      193 2024-04-19 11:08:57.000000 hellogaurav-1.1.0/hellogaurav.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-04-19 11:08:57.000000 hellogaurav-1.1.0/hellogaurav.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 11:08:57.000000 hellogaurav-1.1.0/hellogaurav.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-19 10:41:45.000000 hellogaurav-1.1.0/hellogaurav.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-04-19 11:08:57.000000 hellogaurav-1.1.0/hellogaurav.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 11:08:57.835109 hellogaurav-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      401 2024-04-19 11:08:40.000000 hellogaurav-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:07:45.135246 hellogaurav-2.0.0/
+-rw-rw-rw-   0        0        0        0 2024-04-19 10:27:33.000000 hellogaurav-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      193 2024-04-19 11:07:45.135246 hellogaurav-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 10:27:45.000000 hellogaurav-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 11:07:45.053506 hellogaurav-2.0.0/hellogaurav/
+-rw-rw-rw-   0        0        0        0 2024-04-19 10:26:21.000000 hellogaurav-2.0.0/hellogaurav/__init__.py
+-rw-rw-rw-   0        0        0       14 2024-04-19 10:26:44.000000 hellogaurav-2.0.0/hellogaurav/hello.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:07:45.133231 hellogaurav-2.0.0/hellogaurav.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-04-19 11:07:44.000000 hellogaurav-2.0.0/hellogaurav.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-04-19 11:07:45.000000 hellogaurav-2.0.0/hellogaurav.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 11:07:44.000000 hellogaurav-2.0.0/hellogaurav.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 10:41:45.000000 hellogaurav-2.0.0/hellogaurav.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-19 11:07:44.000000 hellogaurav-2.0.0/hellogaurav.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 11:07:45.135246 hellogaurav-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      401 2024-04-19 11:07:16.000000 hellogaurav-2.0.0/setup.py
```

