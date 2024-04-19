# Comparing `tmp/ftw.casauth-1.6.0.tar.gz` & `tmp/ftw.casauth-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftw.casauth-1.6.0.tar", last modified: Tue Aug 15 12:50:29 2023, max compression
+gzip compressed data, was "ftw.casauth-1.6.1.tar", last modified: Mon Sep 18 09:28:57 2023, max compression
```

## Comparing `ftw.casauth-1.6.0.tar` & `ftw.casauth-1.6.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-08-15 12:50:29.716258 ftw.casauth-1.6.0/
--rw-r--r--   0 tbu        (501) staff       (20)       97 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/MANIFEST.in
--rw-r--r--   0 tbu        (501) staff       (20)     3192 2023-08-15 12:50:29.715986 ftw.casauth-1.6.0/PKG-INFO
--rw-r--r--   0 tbu        (501) staff       (20)      867 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/README.rst
-drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-08-15 12:50:29.706979 ftw.casauth-1.6.0/docs/
--rw-r--r--   0 tbu        (501) staff       (20)     1644 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/docs/HISTORY.txt
--rw-r--r--   0 tbu        (501) staff       (20)    18092 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/docs/LICENSE.GPL
--rw-r--r--   0 tbu        (501) staff       (20)      722 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/docs/LICENSE.txt
-drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-08-15 12:50:29.707315 ftw.casauth-1.6.0/ftw/
--rw-r--r--   0 tbu        (501) staff       (20)       56 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/__init__.py
-drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-08-15 12:50:29.711389 ftw.casauth-1.6.0/ftw/casauth/
--rw-r--r--   0 tbu        (501) staff       (20)      587 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/__init__.py
--rw-r--r--   0 tbu        (501) staff       (20)     3377 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/cas.py
--rw-r--r--   0 tbu        (501) staff       (20)      386 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/configure.zcml
--rw-r--r--   0 tbu        (501) staff       (20)     6474 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/plugin.py
-drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-08-15 12:50:29.712224 ftw.casauth-1.6.0/ftw/casauth/restapi/
--rw-r--r--   0 tbu        (501) staff       (20)        0 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/restapi/__init__.py
--rw-r--r--   0 tbu        (501) staff       (20)     3180 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/restapi/caslogin.py
--rw-r--r--   0 tbu        (501) staff       (20)      351 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/restapi/configure.zcml
--rw-r--r--   0 tbu        (501) staff       (20)     1935 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/testing.py
-drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-08-15 12:50:29.714303 ftw.casauth-1.6.0/ftw/casauth/tests/
--rw-r--r--   0 tbu        (501) staff       (20)        1 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/tests/__init__.py
-drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-08-15 12:50:29.714946 ftw.casauth-1.6.0/ftw/casauth/tests/data/
--rw-r--r--   0 tbu        (501) staff       (20)      210 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/tests/data/service_validate_invalid_ticket.xml
--rw-r--r--   0 tbu        (501) staff       (20)      544 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/tests/data/service_validate_success.xml
--rw-r--r--   0 tbu        (501) staff       (20)     3134 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/tests/test_browser.py
--rw-r--r--   0 tbu        (501) staff       (20)     2513 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/tests/test_cas.py
--rw-r--r--   0 tbu        (501) staff       (20)     7152 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/tests/test_plugin.py
--rw-r--r--   0 tbu        (501) staff       (20)     6589 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/tests/test_restapi.py
--rw-r--r--   0 tbu        (501) staff       (20)      502 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/tests/utils.py
-drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-08-15 12:50:29.715569 ftw.casauth-1.6.0/ftw/casauth/www/
--rw-r--r--   0 tbu        (501) staff       (20)     1143 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/www/addPlugin.zpt
--rw-r--r--   0 tbu        (501) staff       (20)      900 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/ftw/casauth/www/config.zpt
-drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-08-15 12:50:29.709778 ftw.casauth-1.6.0/ftw.casauth.egg-info/
--rw-r--r--   0 tbu        (501) staff       (20)     3192 2023-08-15 12:50:29.000000 ftw.casauth-1.6.0/ftw.casauth.egg-info/PKG-INFO
--rw-r--r--   0 tbu        (501) staff       (20)      958 2023-08-15 12:50:29.000000 ftw.casauth-1.6.0/ftw.casauth.egg-info/SOURCES.txt
--rw-r--r--   0 tbu        (501) staff       (20)        1 2023-08-15 12:50:29.000000 ftw.casauth-1.6.0/ftw.casauth.egg-info/dependency_links.txt
--rw-r--r--   0 tbu        (501) staff       (20)       40 2023-08-15 12:50:29.000000 ftw.casauth-1.6.0/ftw.casauth.egg-info/entry_points.txt
--rw-r--r--   0 tbu        (501) staff       (20)        4 2023-08-15 12:50:29.000000 ftw.casauth-1.6.0/ftw.casauth.egg-info/namespace_packages.txt
--rw-r--r--   0 tbu        (501) staff       (20)        1 2023-08-15 12:50:29.000000 ftw.casauth-1.6.0/ftw.casauth.egg-info/not-zip-safe
--rw-r--r--   0 tbu        (501) staff       (20)      113 2023-08-15 12:50:29.000000 ftw.casauth-1.6.0/ftw.casauth.egg-info/requires.txt
--rw-r--r--   0 tbu        (501) staff       (20)        4 2023-08-15 12:50:29.000000 ftw.casauth-1.6.0/ftw.casauth.egg-info/top_level.txt
--rw-r--r--   0 tbu        (501) staff       (20)       38 2023-08-15 12:50:29.716341 ftw.casauth-1.6.0/setup.cfg
--rw-r--r--   0 tbu        (501) staff       (20)     1496 2023-08-15 12:50:28.000000 ftw.casauth-1.6.0/setup.py
+drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-09-18 09:28:57.665106 ftw.casauth-1.6.1/
+-rw-r--r--   0 tbu        (501) staff       (20)       97 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/MANIFEST.in
+-rw-r--r--   0 tbu        (501) staff       (20)     3377 2023-09-18 09:28:57.664709 ftw.casauth-1.6.1/PKG-INFO
+-rw-r--r--   0 tbu        (501) staff       (20)      867 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/README.rst
+drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-09-18 09:28:57.656494 ftw.casauth-1.6.1/docs/
+-rw-r--r--   0 tbu        (501) staff       (20)     1829 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/docs/HISTORY.txt
+-rw-r--r--   0 tbu        (501) staff       (20)    18092 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/docs/LICENSE.GPL
+-rw-r--r--   0 tbu        (501) staff       (20)      722 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/docs/LICENSE.txt
+drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-09-18 09:28:57.656798 ftw.casauth-1.6.1/ftw/
+-rw-r--r--   0 tbu        (501) staff       (20)       56 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/__init__.py
+drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-09-18 09:28:57.660562 ftw.casauth-1.6.1/ftw/casauth/
+-rw-r--r--   0 tbu        (501) staff       (20)      587 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/__init__.py
+-rw-r--r--   0 tbu        (501) staff       (20)     3377 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/cas.py
+-rw-r--r--   0 tbu        (501) staff       (20)      386 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/configure.zcml
+-rw-r--r--   0 tbu        (501) staff       (20)     6474 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/plugin.py
+drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-09-18 09:28:57.661365 ftw.casauth-1.6.1/ftw/casauth/restapi/
+-rw-r--r--   0 tbu        (501) staff       (20)        0 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/restapi/__init__.py
+-rw-r--r--   0 tbu        (501) staff       (20)     3202 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/restapi/caslogin.py
+-rw-r--r--   0 tbu        (501) staff       (20)      351 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/restapi/configure.zcml
+-rw-r--r--   0 tbu        (501) staff       (20)     1935 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/testing.py
+drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-09-18 09:28:57.663054 ftw.casauth-1.6.1/ftw/casauth/tests/
+-rw-r--r--   0 tbu        (501) staff       (20)        1 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/tests/__init__.py
+drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-09-18 09:28:57.663641 ftw.casauth-1.6.1/ftw/casauth/tests/data/
+-rw-r--r--   0 tbu        (501) staff       (20)      210 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/tests/data/service_validate_invalid_ticket.xml
+-rw-r--r--   0 tbu        (501) staff       (20)      544 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/tests/data/service_validate_success.xml
+-rw-r--r--   0 tbu        (501) staff       (20)     3134 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/tests/test_browser.py
+-rw-r--r--   0 tbu        (501) staff       (20)     2513 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/tests/test_cas.py
+-rw-r--r--   0 tbu        (501) staff       (20)     7152 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/tests/test_plugin.py
+-rw-r--r--   0 tbu        (501) staff       (20)     6589 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/tests/test_restapi.py
+-rw-r--r--   0 tbu        (501) staff       (20)      502 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/tests/utils.py
+drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-09-18 09:28:57.664309 ftw.casauth-1.6.1/ftw/casauth/www/
+-rw-r--r--   0 tbu        (501) staff       (20)     1143 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/www/addPlugin.zpt
+-rw-r--r--   0 tbu        (501) staff       (20)      900 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw/casauth/www/config.zpt
+drwxr-xr-x   0 tbu        (501) staff       (20)        0 2023-09-18 09:28:57.659183 ftw.casauth-1.6.1/ftw.casauth.egg-info/
+-rw-r--r--   0 tbu        (501) staff       (20)     3377 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw.casauth.egg-info/PKG-INFO
+-rw-r--r--   0 tbu        (501) staff       (20)      958 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw.casauth.egg-info/SOURCES.txt
+-rw-r--r--   0 tbu        (501) staff       (20)        1 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw.casauth.egg-info/dependency_links.txt
+-rw-r--r--   0 tbu        (501) staff       (20)       40 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw.casauth.egg-info/entry_points.txt
+-rw-r--r--   0 tbu        (501) staff       (20)        4 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw.casauth.egg-info/namespace_packages.txt
+-rw-r--r--   0 tbu        (501) staff       (20)        1 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw.casauth.egg-info/not-zip-safe
+-rw-r--r--   0 tbu        (501) staff       (20)      113 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw.casauth.egg-info/requires.txt
+-rw-r--r--   0 tbu        (501) staff       (20)        4 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/ftw.casauth.egg-info/top_level.txt
+-rw-r--r--   0 tbu        (501) staff       (20)       38 2023-09-18 09:28:57.665187 ftw.casauth-1.6.1/setup.cfg
+-rw-r--r--   0 tbu        (501) staff       (20)     1496 2023-09-18 09:28:57.000000 ftw.casauth-1.6.1/setup.py
```

### Comparing `ftw.casauth-1.6.0/PKG-INFO` & `ftw.casauth-1.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftw.casauth
-Version: 1.6.0
+Version: 1.6.1
 Summary: Plone PAS plugin for authentication against CAS.
 Home-page: https://github.com/4teamwork/ftw.casauth
 Author: Thomas Buchberger
 Author-email: mailto:t.buchberger@4teamwork.ch
 License: GPL2
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
@@ -52,14 +52,21 @@
 This package is copyright by `4teamwork <http://www.4teamwork.ch/>`_.
 
 ``ftw.casauth`` is licensed under GNU General Public License, version 2.
 
 Changelog
 =========
 
+1.6.1 (2023-09-18)
+------------------
+
+- Fix again login with invalid ticket using REST API, which could lead to
+  authenticate the wrong user. Bug was reintroduced in 1.6.0. [buchi]
+
+
 1.6.0 (2023-08-15)
 ------------------
 
 - Lookup users by username (login) instead of userid. [buchi]
 
 
 1.5.0 (2023-01-23)
```

### Comparing `ftw.casauth-1.6.0/README.rst` & `ftw.casauth-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/docs/HISTORY.txt` & `ftw.casauth-1.6.1/docs/HISTORY.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+1.6.1 (2023-09-18)
+------------------
+
+- Fix again login with invalid ticket using REST API, which could lead to
+  authenticate the wrong user. Bug was reintroduced in 1.6.0. [buchi]
+
+
 1.6.0 (2023-08-15)
 ------------------
 
 - Lookup users by username (login) instead of userid. [buchi]
 
 
 1.5.0 (2023-01-23)
```

### Comparing `ftw.casauth-1.6.0/docs/LICENSE.GPL` & `ftw.casauth-1.6.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/docs/LICENSE.txt` & `ftw.casauth-1.6.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/__init__.py` & `ftw.casauth-1.6.1/ftw/casauth/__init__.py`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/cas.py` & `ftw.casauth-1.6.1/ftw/casauth/cas.py`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/plugin.py` & `ftw.casauth-1.6.1/ftw/casauth/plugin.py`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/restapi/caslogin.py` & `ftw.casauth-1.6.1/ftw/casauth/restapi/caslogin.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                 message='JWT authentication plugin not installed.'))
 
         username = validate_ticket(
             data['ticket'],
             cas_plugin.cas_server_url,
             service,
         )
-        info = uf._verifyUser(uf.plugins, login=username)
+        info = uf._verifyUser(uf.plugins, login=username) if username else None
         if info is None:
             self.request.response.setStatus(401)
             return dict(error=dict(
                 type='Login failed',
                 message='User with username {} not found.'.format(username)))
 
         userid = info['id']
```

### Comparing `ftw.casauth-1.6.0/ftw/casauth/testing.py` & `ftw.casauth-1.6.1/ftw/casauth/testing.py`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/tests/data/service_validate_success.xml` & `ftw.casauth-1.6.1/ftw/casauth/tests/data/service_validate_success.xml`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/tests/test_browser.py` & `ftw.casauth-1.6.1/ftw/casauth/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/tests/test_cas.py` & `ftw.casauth-1.6.1/ftw/casauth/tests/test_cas.py`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/tests/test_plugin.py` & `ftw.casauth-1.6.1/ftw/casauth/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/tests/test_restapi.py` & `ftw.casauth-1.6.1/ftw/casauth/tests/test_restapi.py`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/www/addPlugin.zpt` & `ftw.casauth-1.6.1/ftw/casauth/www/addPlugin.zpt`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw/casauth/www/config.zpt` & `ftw.casauth-1.6.1/ftw/casauth/www/config.zpt`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/ftw.casauth.egg-info/PKG-INFO` & `ftw.casauth-1.6.1/ftw.casauth.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftw.casauth
-Version: 1.6.0
+Version: 1.6.1
 Summary: Plone PAS plugin for authentication against CAS.
 Home-page: https://github.com/4teamwork/ftw.casauth
 Author: Thomas Buchberger
 Author-email: mailto:t.buchberger@4teamwork.ch
 License: GPL2
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
@@ -52,14 +52,21 @@
 This package is copyright by `4teamwork <http://www.4teamwork.ch/>`_.
 
 ``ftw.casauth`` is licensed under GNU General Public License, version 2.
 
 Changelog
 =========
 
+1.6.1 (2023-09-18)
+------------------
+
+- Fix again login with invalid ticket using REST API, which could lead to
+  authenticate the wrong user. Bug was reintroduced in 1.6.0. [buchi]
+
+
 1.6.0 (2023-08-15)
 ------------------
 
 - Lookup users by username (login) instead of userid. [buchi]
 
 
 1.5.0 (2023-01-23)
```

### Comparing `ftw.casauth-1.6.0/ftw.casauth.egg-info/SOURCES.txt` & `ftw.casauth-1.6.1/ftw.casauth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ftw.casauth-1.6.0/setup.py` & `ftw.casauth-1.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = '1.6.0'
+version = '1.6.1'
 
 tests_require = [
     'plone.api',
     'plone.app.testing',
     'plone.restapi',
     'mock',
     'ftw.testbrowser',
```

