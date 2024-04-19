# Comparing `tmp/ncapybaralib-0.0.1.tar.gz` & `tmp/ncapybaralib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncapybaralib-0.0.1.tar", last modified: Fri Apr 19 15:32:42 2024, max compression
+gzip compressed data, was "ncapybaralib-0.0.2.tar", last modified: Fri Apr 19 18:02:24 2024, max compression
```

## Comparing `ncapybaralib-0.0.1.tar` & `ncapybaralib-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 15:32:42.614104 ncapybaralib-0.0.1/
--rw-rw-rw-   0        0        0      603 2024-04-19 15:32:42.612110 ncapybaralib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-04-19 14:38:32.000000 ncapybaralib-0.0.1/README.md
--rw-rw-rw-   0        0        0      520 2024-04-19 15:25:56.000000 ncapybaralib-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 15:32:42.614104 ncapybaralib-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 15:32:42.586103 ncapybaralib-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 15:32:42.592101 ncapybaralib-0.0.1/src/NCapybaraLib/
--rw-rw-rw-   0        0        0       59 2024-04-19 15:16:11.000000 ncapybaralib-0.0.1/src/NCapybaraLib/__init__.py
--rw-rw-rw-   0        0        0       36 2024-04-19 15:21:36.000000 ncapybaralib-0.0.1/src/NCapybaraLib/__init__.pyi
-drwxrwxrwx   0        0        0        0 2024-04-19 15:32:42.609099 ncapybaralib-0.0.1/src/NCapybaraLib.egg-info/
--rw-rw-rw-   0        0        0      603 2024-04-19 15:32:42.000000 ncapybaralib-0.0.1/src/NCapybaraLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-19 15:32:42.000000 ncapybaralib-0.0.1/src/NCapybaraLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 15:32:42.000000 ncapybaralib-0.0.1/src/NCapybaraLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-19 15:32:42.000000 ncapybaralib-0.0.1/src/NCapybaraLib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 18:02:24.390127 ncapybaralib-0.0.2/
+-rw-rw-rw-   0        0        0      964 2024-04-19 18:02:24.388128 ncapybaralib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2024-04-19 16:03:59.000000 ncapybaralib-0.0.2/README.md
+-rw-rw-rw-   0        0        0      667 2024-04-19 16:20:44.000000 ncapybaralib-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 18:02:24.391129 ncapybaralib-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 18:02:24.304129 ncapybaralib-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 18:02:24.341132 ncapybaralib-0.0.2/src/NCapybaraLib/
+-rw-rw-rw-   0        0        0      616 2024-04-19 16:30:29.000000 ncapybaralib-0.0.2/src/NCapybaraLib/String.py
+-rw-rw-rw-   0        0        0     1038 2024-04-19 17:55:43.000000 ncapybaralib-0.0.2/src/NCapybaraLib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 18:02:24.377129 ncapybaralib-0.0.2/src/NCapybaraLib.egg-info/
+-rw-rw-rw-   0        0        0      964 2024-04-19 18:02:24.000000 ncapybaralib-0.0.2/src/NCapybaraLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-04-19 18:02:24.000000 ncapybaralib-0.0.2/src/NCapybaraLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 18:02:24.000000 ncapybaralib-0.0.2/src/NCapybaraLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 18:02:24.000000 ncapybaralib-0.0.2/src/NCapybaraLib.egg-info/top_level.txt
```

