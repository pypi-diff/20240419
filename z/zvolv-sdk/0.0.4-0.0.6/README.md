# Comparing `tmp/zvolv_sdk-0.0.4.tar.gz` & `tmp/zvolv_sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zvolv_sdk-0.0.4.tar", last modified: Fri Apr 19 05:22:39 2024, max compression
+gzip compressed data, was "zvolv_sdk-0.0.6.tar", last modified: Fri Apr 19 05:51:31 2024, max compression
```

## Comparing `zvolv_sdk-0.0.4.tar` & `zvolv_sdk-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.222741 zvolv_sdk-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.222741 zvolv_sdk-0.0.4/src/devide/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/src/devide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/src/devide/divide_by_three.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/src/zvolv_client/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/src/zvolv_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/src/zvolv_client/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/tests/test_divide_by_three.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/zvolv_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/common_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/server_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/user_defined_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/zvolv_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 05:22:39.000000 zvolv_sdk-0.0.4/zvolv_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-19 05:22:39.000000 zvolv_sdk-0.0.4/zvolv_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:22:39.000000 zvolv_sdk-0.0.4/zvolv_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 05:22:39.000000 zvolv_sdk-0.0.4/zvolv_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.291911 zvolv_sdk-0.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.291911 zvolv_sdk-0.0.6/src/devide/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/src/devide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/src/devide/divide_by_three.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.291911 zvolv_sdk-0.0.6/src/zvolv_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/src/zvolv_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/src/zvolv_client/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/tests/test_divide_by_three.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/zvolv_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/common_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/zvolv_sdk/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/modules/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/server_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/user_defined_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-19 05:51:21.000000 zvolv_sdk-0.0.6/zvolv_sdk/zvolv_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:51:31.295911 zvolv_sdk-0.0.6/zvolv_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 05:51:31.000000 zvolv_sdk-0.0.6/zvolv_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-19 05:51:31.000000 zvolv_sdk-0.0.6/zvolv_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:51:31.000000 zvolv_sdk-0.0.6/zvolv_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 05:51:31.000000 zvolv_sdk-0.0.6/zvolv_sdk.egg-info/top_level.txt
```

### Comparing `zvolv_sdk-0.0.4/LICENSE` & `zvolv_sdk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.4/PKG-INFO` & `zvolv_sdk-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zvolv_sdk
-Version: 0.0.4
+Version: 0.0.6
 Summary: The Zvolv API Platform SDK for Python
 Home-page: https://github.com/zvolvapi/python-zvolv-sdk
 Download-URL: https://github.com/zvolvapi/python-zvolv-sdk/archive/v_01.tar.gz
 Author: Akshay Jadhav
 Author-email: support@zvolv.com
 License: MIT
 Keywords: zvolv,zvolv-api,web-api,sdk,rest-api-client
```

### Comparing `zvolv_sdk-0.0.4/README.md` & `zvolv_sdk-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.4/setup.py` & `zvolv_sdk-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.4/src/zvolv_client/auth.py` & `zvolv_sdk-0.0.6/src/zvolv_client/auth.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.4/zvolv_sdk/client.py` & `zvolv_sdk-0.0.6/zvolv_sdk/client.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.4/zvolv_sdk/common_api.py` & `zvolv_sdk-0.0.6/zvolv_sdk/common_api.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.4/zvolv_sdk/server_configuration.py` & `zvolv_sdk-0.0.6/zvolv_sdk/server_configuration.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.4/zvolv_sdk/submission.py` & `zvolv_sdk-0.0.6/zvolv_sdk/submission.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.4/zvolv_sdk/user_defined_exceptions.py` & `zvolv_sdk-0.0.6/zvolv_sdk/user_defined_exceptions.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.4/zvolv_sdk.egg-info/PKG-INFO` & `zvolv_sdk-0.0.6/zvolv_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zvolv_sdk
-Version: 0.0.4
+Version: 0.0.6
 Summary: The Zvolv API Platform SDK for Python
 Home-page: https://github.com/zvolvapi/python-zvolv-sdk
 Download-URL: https://github.com/zvolvapi/python-zvolv-sdk/archive/v_01.tar.gz
 Author: Akshay Jadhav
 Author-email: support@zvolv.com
 License: MIT
 Keywords: zvolv,zvolv-api,web-api,sdk,rest-api-client
```

