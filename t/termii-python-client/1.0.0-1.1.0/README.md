# Comparing `tmp/termii_python_client-1.0.0.tar.gz` & `tmp/termii_python_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termii_python_client-1.0.0.tar", last modified: Thu Apr 18 09:53:32 2024, max compression
+gzip compressed data, was "termii_python_client-1.1.0.tar", last modified: Thu Apr 18 19:00:11 2024, max compression
```

## Comparing `termii_python_client-1.0.0.tar` & `termii_python_client-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 09:53:32.612501 termii_python_client-1.0.0/
--rw-rw-rw-   0        0        0     1093 2024-04-18 09:23:17.000000 termii_python_client-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      672 2024-04-18 09:53:32.609511 termii_python_client-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       56 2024-04-18 09:24:30.000000 termii_python_client-1.0.0/README.md
--rw-rw-rw-   0        0        0      725 2024-04-18 09:52:47.000000 termii_python_client-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 09:53:32.612501 termii_python_client-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0    21754 2024-04-18 09:03:49.000000 termii_python_client-1.0.0/termii.py
-drwxrwxrwx   0        0        0        0 2024-04-18 09:53:32.606517 termii_python_client-1.0.0/termii_python_client.egg-info/
--rw-rw-rw-   0        0        0      672 2024-04-18 09:53:32.000000 termii_python_client-1.0.0/termii_python_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-04-18 09:53:32.000000 termii_python_client-1.0.0/termii_python_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 09:53:32.000000 termii_python_client-1.0.0/termii_python_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 09:53:32.000000 termii_python_client-1.0.0/termii_python_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 09:53:32.603525 termii_python_client-1.0.0/tests/
--rw-rw-rw-   0        0        0      921 2024-04-18 00:09:57.000000 termii_python_client-1.0.0/tests/test_contact.py
--rw-rw-rw-   0        0        0     1379 2024-04-18 09:03:34.000000 termii_python_client-1.0.0/tests/test_insights.py
--rw-rw-rw-   0        0        0     1687 2024-04-17 23:13:06.000000 termii_python_client-1.0.0/tests/test_messaging.py
--rw-rw-rw-   0        0        0     1192 2024-04-17 19:04:09.000000 termii_python_client-1.0.0/tests/test_number_api.py
--rw-rw-rw-   0        0        0     2222 2024-04-17 23:12:53.000000 termii_python_client-1.0.0/tests/test_phonebooks.py
--rw-rw-rw-   0        0        0      642 2024-04-17 06:41:14.000000 termii_python_client-1.0.0/tests/test_sender_id.py
--rw-rw-rw-   0        0        0     2185 2024-04-18 08:36:18.000000 termii_python_client-1.0.0/tests/test_token.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:00:11.207912 termii_python_client-1.1.0/
+-rw-rw-rw-   0        0        0     1093 2024-04-18 09:23:17.000000 termii_python_client-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5024 2024-04-18 19:00:11.175997 termii_python_client-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4410 2024-04-18 18:56:21.000000 termii_python_client-1.1.0/README.md
+-rw-rw-rw-   0        0        0      725 2024-04-18 18:59:46.000000 termii_python_client-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 19:00:11.207912 termii_python_client-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 19:00:11.173005 termii_python_client-1.1.0/termii_python_client.egg-info/
+-rw-rw-rw-   0        0        0     5024 2024-04-18 19:00:10.000000 termii_python_client-1.1.0/termii_python_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-18 19:00:10.000000 termii_python_client-1.1.0/termii_python_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 19:00:10.000000 termii_python_client-1.1.0/termii_python_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 19:00:10.000000 termii_python_client-1.1.0/termii_python_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 19:00:11.160044 termii_python_client-1.1.0/tests/
+-rw-rw-rw-   0        0        0      921 2024-04-18 00:09:57.000000 termii_python_client-1.1.0/tests/test_contact.py
+-rw-rw-rw-   0        0        0     1379 2024-04-18 09:03:34.000000 termii_python_client-1.1.0/tests/test_insights.py
+-rw-rw-rw-   0        0        0     1687 2024-04-17 23:13:06.000000 termii_python_client-1.1.0/tests/test_messaging.py
+-rw-rw-rw-   0        0        0     1192 2024-04-17 19:04:09.000000 termii_python_client-1.1.0/tests/test_number_api.py
+-rw-rw-rw-   0        0        0     2222 2024-04-17 23:12:53.000000 termii_python_client-1.1.0/tests/test_phonebooks.py
+-rw-rw-rw-   0        0        0      642 2024-04-17 06:41:14.000000 termii_python_client-1.1.0/tests/test_sender_id.py
+-rw-rw-rw-   0        0        0     2185 2024-04-18 18:56:32.000000 termii_python_client-1.1.0/tests/test_token.py
```

### Comparing `termii_python_client-1.0.0/LICENSE` & `termii_python_client-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.0.0/pyproject.toml` & `termii_python_client-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests>=2.31.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "termii-python-client"
-version = "1.0.0"
+version = "1.1.0"
 authors = [ { name="Gabriel Michael Ojomakpene [codewitgabi]", email="codewitgabi222@gmail.com" }, { name="Joshua Joseph", email="joshuajosephizzyjosh@gmail.com" },
 ]
 description = "Termii python package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `termii_python_client-1.0.0/tests/test_contact.py` & `termii_python_client-1.1.0/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.0.0/tests/test_insights.py` & `termii_python_client-1.1.0/tests/test_insights.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.0.0/tests/test_messaging.py` & `termii_python_client-1.1.0/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.0.0/tests/test_number_api.py` & `termii_python_client-1.1.0/tests/test_number_api.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.0.0/tests/test_phonebooks.py` & `termii_python_client-1.1.0/tests/test_phonebooks.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.0.0/tests/test_sender_id.py` & `termii_python_client-1.1.0/tests/test_sender_id.py`

 * *Files identical despite different names*

### Comparing `termii_python_client-1.0.0/tests/test_token.py` & `termii_python_client-1.1.0/tests/test_token.py`

 * *Files identical despite different names*

