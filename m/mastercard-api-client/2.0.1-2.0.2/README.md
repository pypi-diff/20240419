# Comparing `tmp/mastercard_api_client-2.0.1.tar.gz` & `tmp/mastercard_api_client-2.0.2.tar.gz`

## Comparing `mastercard_api_client-2.0.1.tar` & `mastercard_api_client-2.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/_version.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/core/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/core/baseobject.py
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/core/config.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/core/constants.py
--rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/core/controller.py
--rw-r--r--   0        0        0     8777 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/core/exceptions.py
--rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/core/model.py
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/core/util.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/security/__init__.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/security/authentication.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/security/oauth.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/mastercardapicore/security/util.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/README.md
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/_version.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/__init__.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/baseobject.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/config.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/constants.py
+-rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/controller.py
+-rw-r--r--   0        0        0     8777 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/exceptions.py
+-rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/model.py
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/core/util.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/security/__init__.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/security/authentication.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/security/oauth.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/mastercardapicore/security/util.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/.gitignore
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/README.md
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.2/PKG-INFO
```

### Comparing `mastercard_api_client-2.0.1/.github/workflows/publish.yaml` & `mastercard_api_client-2.0.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/mastercardapicore/core/baseobject.py` & `mastercard_api_client-2.0.2/mastercardapicore/core/baseobject.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/mastercardapicore/core/config.py` & `mastercard_api_client-2.0.2/mastercardapicore/core/config.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/mastercardapicore/core/constants.py` & `mastercard_api_client-2.0.2/mastercardapicore/core/constants.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/mastercardapicore/core/controller.py` & `mastercard_api_client-2.0.2/mastercardapicore/core/controller.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/mastercardapicore/core/exceptions.py` & `mastercard_api_client-2.0.2/mastercardapicore/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/mastercardapicore/core/model.py` & `mastercard_api_client-2.0.2/mastercardapicore/core/model.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/mastercardapicore/core/util.py` & `mastercard_api_client-2.0.2/mastercardapicore/core/util.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/mastercardapicore/security/authentication.py` & `mastercard_api_client-2.0.2/mastercardapicore/security/authentication.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/mastercardapicore/security/oauth.py` & `mastercard_api_client-2.0.2/mastercardapicore/security/oauth.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/mastercardapicore/security/util.py` & `mastercard_api_client-2.0.2/mastercardapicore/security/util.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/.gitignore` & `mastercard_api_client-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.1/pyproject.toml` & `mastercard_api_client-2.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,16 +23,15 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "requests>=2.31.0",
   "future>=0.18.3",
-  "cryptography>=41.0.7",
-  "pyopenssl>=24.1.0",
+  "cryptography>=42.0.5",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "_version.py"
```

### Comparing `mastercard_api_client-2.0.1/PKG-INFO` & `mastercard_api_client-2.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.3
 Name: mastercard-api-client
-Version: 2.0.1
+Version: 2.0.2
 Summary: MasterCard API Python Core SDK, fork of the mastercard-api-core library.
 Author-email: Twisto Platform <platform@twisto.cz>
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: cryptography>=41.0.7
+Requires-Dist: cryptography>=42.0.5
 Requires-Dist: future>=0.18.3
-Requires-Dist: pyopenssl>=24.1.0
 Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
-# mastercard-api-core
+# MasterCard API Core
 
 MasterCard API Python Core SDK, fork of the [mastercard-api-core](https://pypi.org/project/mastercard-api-core/) library.
+
+## Installation
+
+```bash
+pip install mastercard-api-client
+```
```

