# Comparing `tmp/proxybandit-1.0.0.tar.gz` & `tmp/proxybandit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxybandit-1.0.0.tar", last modified: Fri Apr 19 09:12:37 2024, max compression
+gzip compressed data, was "proxybandit-1.0.1.tar", last modified: Fri Apr 19 09:42:16 2024, max compression
```

## Comparing `proxybandit-1.0.0.tar` & `proxybandit-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 09:12:37.469907 proxybandit-1.0.0/
--rw-rw-rw-   0        0        0     1089 2024-04-19 08:53:22.000000 proxybandit-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      157 2024-04-19 09:12:37.467425 proxybandit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5207 2024-04-19 08:53:22.000000 proxybandit-1.0.0/README.md
--rw-rw-rw-   0        0        0      208 2024-04-19 09:12:29.000000 proxybandit-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 09:12:37.469907 proxybandit-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 09:12:37.419250 proxybandit-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 09:12:37.441956 proxybandit-1.0.0/src/proxybandit/
--rw-rw-rw-   0        0        0      123 2024-04-19 08:53:22.000000 proxybandit-1.0.0/src/proxybandit/__init__.py
--rw-rw-rw-   0        0        0     1009 2024-04-19 08:53:22.000000 proxybandit-1.0.0/src/proxybandit/core.py
--rw-rw-rw-   0        0        0     2988 2024-04-19 08:53:22.000000 proxybandit-1.0.0/src/proxybandit/gatherer.py
--rw-rw-rw-   0        0        0     1446 2024-04-19 08:53:22.000000 proxybandit-1.0.0/src/proxybandit/proxy.py
--rw-rw-rw-   0        0        0     1135 2024-04-19 08:53:22.000000 proxybandit-1.0.0/src/proxybandit/proxylist.py
-drwxrwxrwx   0        0        0        0 2024-04-19 09:12:37.467425 proxybandit-1.0.0/src/proxybandit.egg-info/
--rw-rw-rw-   0        0        0      157 2024-04-19 09:12:37.000000 proxybandit-1.0.0/src/proxybandit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-04-19 09:12:37.000000 proxybandit-1.0.0/src/proxybandit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 09:12:37.000000 proxybandit-1.0.0/src/proxybandit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-19 09:12:37.000000 proxybandit-1.0.0/src/proxybandit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 09:12:37.000000 proxybandit-1.0.0/src/proxybandit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 09:12:37.466328 proxybandit-1.0.0/tests/
--rw-rw-rw-   0        0        0      184 2024-04-19 08:53:22.000000 proxybandit-1.0.0/tests/test_core.py
--rw-rw-rw-   0        0        0      210 2024-04-19 08:53:22.000000 proxybandit-1.0.0/tests/test_gatherer.py
--rw-rw-rw-   0        0        0     1052 2024-04-19 08:53:22.000000 proxybandit-1.0.0/tests/test_proxy.py
--rw-rw-rw-   0        0        0      699 2024-04-19 08:53:22.000000 proxybandit-1.0.0/tests/test_proxylist.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:42:16.206885 proxybandit-1.0.1/
+-rw-rw-rw-   0        0        0     1089 2024-04-19 08:53:22.000000 proxybandit-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       35 2024-04-19 09:35:12.000000 proxybandit-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      157 2024-04-19 09:42:16.206885 proxybandit-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5207 2024-04-19 08:53:22.000000 proxybandit-1.0.1/README.md
+-rw-rw-rw-   0        0        0      310 2024-04-19 09:41:46.000000 proxybandit-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:42:16.206885 proxybandit-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 09:42:16.176706 proxybandit-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:42:16.187004 proxybandit-1.0.1/src/proxybandit/
+-rw-rw-rw-   0        0        0      123 2024-04-19 08:53:22.000000 proxybandit-1.0.1/src/proxybandit/__init__.py
+-rw-rw-rw-   0        0        0     1009 2024-04-19 08:53:22.000000 proxybandit-1.0.1/src/proxybandit/core.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:42:16.199360 proxybandit-1.0.1/src/proxybandit/data/
+-rw-rw-rw-   0        0        0      367 2024-04-19 08:53:22.000000 proxybandit-1.0.1/src/proxybandit/data/sources.json
+-rw-rw-rw-   0        0        0     2988 2024-04-19 08:53:22.000000 proxybandit-1.0.1/src/proxybandit/gatherer.py
+-rw-rw-rw-   0        0        0     1446 2024-04-19 08:53:22.000000 proxybandit-1.0.1/src/proxybandit/proxy.py
+-rw-rw-rw-   0        0        0     1135 2024-04-19 08:53:22.000000 proxybandit-1.0.1/src/proxybandit/proxylist.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:42:16.205792 proxybandit-1.0.1/src/proxybandit.egg-info/
+-rw-rw-rw-   0        0        0      157 2024-04-19 09:42:16.000000 proxybandit-1.0.1/src/proxybandit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2024-04-19 09:42:16.000000 proxybandit-1.0.1/src/proxybandit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:42:16.000000 proxybandit-1.0.1/src/proxybandit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-19 09:42:16.000000 proxybandit-1.0.1/src/proxybandit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-19 09:42:16.000000 proxybandit-1.0.1/src/proxybandit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 09:42:16.204688 proxybandit-1.0.1/tests/
+-rw-rw-rw-   0        0        0      184 2024-04-19 08:53:22.000000 proxybandit-1.0.1/tests/test_core.py
+-rw-rw-rw-   0        0        0      210 2024-04-19 08:53:22.000000 proxybandit-1.0.1/tests/test_gatherer.py
+-rw-rw-rw-   0        0        0     1052 2024-04-19 08:53:22.000000 proxybandit-1.0.1/tests/test_proxy.py
+-rw-rw-rw-   0        0        0      699 2024-04-19 08:53:22.000000 proxybandit-1.0.1/tests/test_proxylist.py
```

### Comparing `proxybandit-1.0.0/LICENSE` & `proxybandit-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proxybandit-1.0.0/README.md` & `proxybandit-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `proxybandit-1.0.0/src/proxybandit/core.py` & `proxybandit-1.0.1/src/proxybandit/core.py`

 * *Files identical despite different names*

### Comparing `proxybandit-1.0.0/src/proxybandit/gatherer.py` & `proxybandit-1.0.1/src/proxybandit/gatherer.py`

 * *Files identical despite different names*

### Comparing `proxybandit-1.0.0/src/proxybandit/proxy.py` & `proxybandit-1.0.1/src/proxybandit/proxy.py`

 * *Files identical despite different names*

### Comparing `proxybandit-1.0.0/src/proxybandit/proxylist.py` & `proxybandit-1.0.1/src/proxybandit/proxylist.py`

 * *Files identical despite different names*

### Comparing `proxybandit-1.0.0/tests/test_proxy.py` & `proxybandit-1.0.1/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `proxybandit-1.0.0/tests/test_proxylist.py` & `proxybandit-1.0.1/tests/test_proxylist.py`

 * *Files identical despite different names*

