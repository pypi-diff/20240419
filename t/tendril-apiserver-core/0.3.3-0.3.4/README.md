# Comparing `tmp/tendril-apiserver-core-0.3.3.tar.gz` & `tmp/tendril_apiserver_core-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-apiserver-core-0.3.3.tar", last modified: Sun Feb  4 16:00:41 2024, max compression
+gzip compressed data, was "tendril_apiserver_core-0.3.4.tar", last modified: Thu Apr 18 22:06:12 2024, max compression
```

## Comparing `tendril-apiserver-core-0.3.3.tar` & `tendril_apiserver_core-0.3.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.326334 tendril-apiserver-core-0.3.3/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3630 2024-02-04 16:00:41.326334 tendril-apiserver-core-0.3.3/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2302 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/README.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-02-04 16:00:41.330334 tendril-apiserver-core-0.3.3/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3479 2023-08-10 00:50:44.000000 tendril-apiserver-core-0.3.3/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.314334 tendril-apiserver-core-0.3.3/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.318334 tendril-apiserver-core-0.3.3/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.318334 tendril-apiserver-core-0.3.3/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/src/tendril/apiserver/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       52 2023-02-18 23:08:41.000000 tendril-apiserver-core-0.3.3/src/tendril/apiserver/core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.322334 tendril-apiserver-core-0.3.3/src/tendril/apiserver/exceptions/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:26.000000 tendril-apiserver-core-0.3.3/src/tendril/apiserver/exceptions/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      428 2023-03-15 16:01:26.000000 tendril-apiserver-core-0.3.3/src/tendril/apiserver/exceptions/common.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.322334 tendril-apiserver-core-0.3.3/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 20:27:06.000000 tendril-apiserver-core-0.3.3/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2115 2024-02-04 15:59:51.000000 tendril-apiserver-core-0.3.3/src/tendril/apiserver/routers/diagnostics.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1075 2023-09-06 11:25:54.000000 tendril-apiserver-core-0.3.3/src/tendril/apiserver/routers/system.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5669 2023-09-06 12:16:17.000000 tendril-apiserver-core-0.3.3/src/tendril/apiserver/server.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.322334 tendril-apiserver-core-0.3.3/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril-apiserver-core-0.3.3/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.322334 tendril-apiserver-core-0.3.3/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:00:43.000000 tendril-apiserver-core-0.3.3/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      153 2022-11-28 19:36:13.000000 tendril-apiserver-core-0.3.3/src/tendril/authz/scopes/system.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.326334 tendril-apiserver-core-0.3.3/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:26.000000 tendril-apiserver-core-0.3.3/src/tendril/common/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       61 2023-03-15 16:01:26.000000 tendril-apiserver-core-0.3.3/src/tendril/common/exceptions.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.326334 tendril-apiserver-core-0.3.3/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3083 2023-03-16 05:14:37.000000 tendril-apiserver-core-0.3.3/src/tendril/config/server.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.326334 tendril-apiserver-core-0.3.3/src/tendril/resources/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1302 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/src/tendril/resources/test_certificate.pem
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/src/tendril/resources/test_key.pem
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-02-04 16:00:41.326334 tendril-apiserver-core-0.3.3/src/tendril_apiserver_core.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3630 2024-02-04 16:00:41.000000 tendril-apiserver-core-0.3.3/src/tendril_apiserver_core.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1052 2024-02-04 16:00:41.000000 tendril-apiserver-core-0.3.3/src/tendril_apiserver_core.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-02-04 16:00:41.000000 tendril-apiserver-core-0.3.3/src/tendril_apiserver_core.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2024-02-04 16:00:41.000000 tendril-apiserver-core-0.3.3/src/tendril_apiserver_core.egg-info/entry_points.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      772 2024-02-04 16:00:41.000000 tendril-apiserver-core-0.3.3/src/tendril_apiserver_core.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-02-04 16:00:41.000000 tendril-apiserver-core-0.3.3/src/tendril_apiserver_core.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      829 2022-11-25 15:34:14.000000 tendril-apiserver-core-0.3.3/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.267438 tendril_apiserver_core-0.3.4/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5911 2024-04-18 22:06:12.267438 tendril_apiserver_core-0.3.4/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2302 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/README.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-18 22:06:12.267438 tendril_apiserver_core-0.3.4/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3479 2023-08-10 00:50:44.000000 tendril_apiserver_core-0.3.4/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.247438 tendril_apiserver_core-0.3.4/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.251438 tendril_apiserver_core-0.3.4/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.251438 tendril_apiserver_core-0.3.4/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       52 2023-02-18 23:08:41.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.251438 tendril_apiserver_core-0.3.4/src/tendril/apiserver/exceptions/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:26.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/exceptions/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      428 2023-03-15 16:01:26.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/exceptions/common.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.255438 tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-12-09 20:27:06.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2115 2024-02-04 15:59:51.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/diagnostics.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1075 2023-09-06 11:25:54.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/system.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5669 2023-09-06 12:16:17.000000 tendril_apiserver_core-0.3.4/src/tendril/apiserver/server.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.255438 tendril_apiserver_core-0.3.4/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:36:13.000000 tendril_apiserver_core-0.3.4/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.255438 tendril_apiserver_core-0.3.4/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 21:00:43.000000 tendril_apiserver_core-0.3.4/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      153 2022-11-28 19:36:13.000000 tendril_apiserver_core-0.3.4/src/tendril/authz/scopes/system.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.255438 tendril_apiserver_core-0.3.4/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:26.000000 tendril_apiserver_core-0.3.4/src/tendril/common/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      143 2024-04-17 22:39:46.000000 tendril_apiserver_core-0.3.4/src/tendril/common/exceptions.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.255438 tendril_apiserver_core-0.3.4/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3083 2023-03-16 05:14:37.000000 tendril_apiserver_core-0.3.4/src/tendril/config/server.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.259438 tendril_apiserver_core-0.3.4/src/tendril/resources/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1302 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/src/tendril/resources/test_certificate.pem
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/src/tendril/resources/test_key.pem
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:06:12.259438 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5911 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1052 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/entry_points.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      772 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-18 22:06:12.000000 tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/top_level.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      829 2022-11-25 15:34:14.000000 tendril_apiserver_core-0.3.4/tox.ini
```

### Comparing `tendril-apiserver-core-0.3.3/.gitignore` & `tendril_apiserver_core-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/.readthedocs.yml` & `tendril_apiserver_core-0.3.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/.travis.yml` & `tendril_apiserver_core-0.3.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/LICENSE` & `tendril_apiserver_core-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/README.rst` & `tendril_apiserver_core-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/setup.py` & `tendril_apiserver_core-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/src/tendril/apiserver/routers/diagnostics.py` & `tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/diagnostics.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/src/tendril/apiserver/routers/system.py` & `tendril_apiserver_core-0.3.4/src/tendril/apiserver/routers/system.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/src/tendril/apiserver/server.py` & `tendril_apiserver_core-0.3.4/src/tendril/apiserver/server.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/src/tendril/config/__init__.py` & `tendril_apiserver_core-0.3.4/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/src/tendril/config/server.py` & `tendril_apiserver_core-0.3.4/src/tendril/config/server.py`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/src/tendril/resources/test_certificate.pem` & `tendril_apiserver_core-0.3.4/src/tendril/resources/test_certificate.pem`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/src/tendril/resources/test_key.pem` & `tendril_apiserver_core-0.3.4/src/tendril/resources/test_key.pem`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/src/tendril_apiserver_core.egg-info/SOURCES.txt` & `tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/src/tendril_apiserver_core.egg-info/requires.txt` & `tendril_apiserver_core-0.3.4/src/tendril_apiserver_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-apiserver-core-0.3.3/tox.ini` & `tendril_apiserver_core-0.3.4/tox.ini`

 * *Files identical despite different names*

