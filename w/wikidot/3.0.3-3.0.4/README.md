# Comparing `tmp/wikidot-3.0.3.tar.gz` & `tmp/wikidot-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikidot-3.0.3.tar", last modified: Tue Apr 16 10:01:01 2024, max compression
+gzip compressed data, was "wikidot-3.0.4.tar", last modified: Fri Apr 19 01:53:09 2024, max compression
```

## Comparing `wikidot-3.0.3.tar` & `wikidot-3.0.4.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 10:01:01.369151 wikidot-3.0.3/
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1070 2024-04-11 05:41:21.000000 wikidot-3.0.3/LICENSE
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3121 2024-04-16 10:01:01.368928 wikidot-3.0.3/PKG-INFO
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2339 2024-04-15 07:24:27.000000 wikidot-3.0.3/README.md
--rw-r--r--   0 ukwhatn    (501) staff       (20)      732 2024-04-16 10:00:47.000000 wikidot-3.0.3/pyproject.toml
--rw-r--r--   0 ukwhatn    (501) staff       (20)       38 2024-04-16 10:01:01.369198 wikidot-3.0.3/setup.cfg
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 10:01:01.361359 wikidot-3.0.3/wikidot/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       34 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/__init__.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 10:01:01.363432 wikidot-3.0.3/wikidot/common/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       40 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/common/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      998 2024-04-15 07:24:27.000000 wikidot-3.0.3/wikidot/common/decorators.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2517 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/common/exceptions.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      450 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/common/logger.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 10:01:01.364020 wikidot-3.0.3/wikidot/connector/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/connector/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)    10788 2024-04-15 07:24:27.000000 wikidot-3.0.3/wikidot/connector/ajax.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      261 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/connector/api.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 10:01:01.366795 wikidot-3.0.3/wikidot/module/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/module/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2091 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/module/auth.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     6407 2024-04-15 07:24:27.000000 wikidot-3.0.3/wikidot/module/client.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)    16496 2024-04-16 09:41:04.000000 wikidot-3.0.3/wikidot/module/page.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3602 2024-04-16 06:41:50.000000 wikidot-3.0.3/wikidot/module/page_revision.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      194 2024-04-15 07:34:32.000000 wikidot-3.0.3/wikidot/module/page_source.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      548 2024-04-16 07:55:57.000000 wikidot-3.0.3/wikidot/module/page_votes.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     8665 2024-04-16 06:41:50.000000 wikidot-3.0.3/wikidot/module/private_message.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     6742 2024-04-16 06:21:58.000000 wikidot-3.0.3/wikidot/module/site.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3053 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/module/site_application.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     7868 2024-04-16 06:41:50.000000 wikidot-3.0.3/wikidot/module/user.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 10:01:01.367499 wikidot-3.0.3/wikidot/util/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/util/__init__.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 10:01:01.367949 wikidot-3.0.3/wikidot/util/parser/
--rw-r--r--   0 ukwhatn    (501) staff       (20)       77 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/util/parser/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)      752 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/util/parser/odate.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2038 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/util/parser/user.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     2635 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/util/quick_module.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1869 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/util/requestutil.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     1477 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/util/stringutil.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 10:01:01.368208 wikidot-3.0.3/wikidot/util/table/
--rw-r--r--   0 ukwhatn    (501) staff       (20)        0 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/util/table/__init__.py
--rw-r--r--   0 ukwhatn    (501) staff       (20)     7128 2024-04-11 05:41:21.000000 wikidot-3.0.3/wikidot/util/table/char_table.py
-drwxr-xr-x   0 ukwhatn    (501) staff       (20)        0 2024-04-16 10:01:01.368521 wikidot-3.0.3/wikidot.egg-info/
--rw-r--r--   0 ukwhatn    (501) staff       (20)     3121 2024-04-16 10:01:01.000000 wikidot-3.0.3/wikidot.egg-info/PKG-INFO
--rw-r--r--   0 ukwhatn    (501) staff       (20)      963 2024-04-16 10:01:01.000000 wikidot-3.0.3/wikidot.egg-info/SOURCES.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)        1 2024-04-16 10:01:01.000000 wikidot-3.0.3/wikidot.egg-info/dependency_links.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)       68 2024-04-16 10:01:01.000000 wikidot-3.0.3/wikidot.egg-info/requires.txt
--rw-r--r--   0 ukwhatn    (501) staff       (20)        8 2024-04-16 10:01:01.000000 wikidot-3.0.3/wikidot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 01:52:49.000000 wikidot-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 01:52:49.000000 wikidot-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-19 01:53:09.006564 wikidot-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-19 01:52:49.000000 wikidot-3.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 01:52:49.000000 wikidot-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:53:09.006564 wikidot-3.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:08.998564 wikidot-3.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.002564 wikidot-3.0.4/src/wikidot/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.002564 wikidot-3.0.4/src/wikidot/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/common/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.002564 wikidot-3.0.4/src/wikidot/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/connector/ajax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/connector/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/src/wikidot/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/page_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/page_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/page_votes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/site_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/module/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/src/wikidot/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/src/wikidot/util/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/parser/odate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/parser/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/quick_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/requestutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/stringutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/src/wikidot/util/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-19 01:52:49.000000 wikidot-3.0.4/src/wikidot/util/table/char_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:53:09.006564 wikidot-3.0.4/src/wikidot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-19 01:53:08.000000 wikidot-3.0.4/src/wikidot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-19 01:53:08.000000 wikidot-3.0.4/src/wikidot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:53:08.000000 wikidot-3.0.4/src/wikidot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 01:53:08.000000 wikidot-3.0.4/src/wikidot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 01:53:08.000000 wikidot-3.0.4/src/wikidot.egg-info/top_level.txt
```

### Comparing `wikidot-3.0.3/LICENSE` & `wikidot-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.3/PKG-INFO` & `wikidot-3.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: wikidot
-Version: 3.0.3
+Version: 3.0.4
 Summary: Wikidot Utility Library
 Author-email: ukwhatn <ukwhatn@gmail.com>
 Project-URL: Homepage, https://github.com/ukwhatn/wikidot.py
 Project-URL: Bug Tracker, https://github.com/ukwhatn/wikidot.py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx~=0.25.0
+Requires-Dist: httpx<0.28,>=0.25
 Requires-Dist: beautifulsoup4~=4.12.2
-Requires-Dist: lxml~=4.9.3
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
+Requires-Dist: lxml<5.3.0,>=4.9.3
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Requires-Dist: twine; extra == "build"
+Provides-Extra: lint
+Requires-Dist: flake8; extra == "lint"
+Requires-Dist: mypy; extra == "lint"
+Requires-Dist: isort; extra == "lint"
+Provides-Extra: format
+Requires-Dist: black; extra == "format"
+Requires-Dist: isort; extra == "format"
 
 # wikidot.py - A Python library for making requests to the Wikidot sites.
 
 ## Installation
 ```bash
 pip install wikidot
 ```
```

### Comparing `wikidot-3.0.3/README.md` & `wikidot-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.3/pyproject.toml` & `wikidot-3.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 [project]
 name = "wikidot"
-version = "3.0.3"
+version = "3.0.4"
 authors = [{ name = "ukwhatn", email = "ukwhatn@gmail.com" }]
 description = "Wikidot Utility Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
 ]
 
 dependencies = [
-    "httpx ~= 0.25.0",
+    "httpx >= 0.25,< 0.28",
     "beautifulsoup4 ~= 4.12.2",
-    "lxml ~= 4.9.3",
+    "lxml >= 4.9.3,< 5.3.0",
 ]
 
 [project.optional-dependencies]
-dev = [
+build = [
     "build",
     "twine",
 ]
+lint = [
+    "flake8",
+    "mypy",
+    "isort",
+]
+format = [
+    "black",
+    "isort",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/ukwhatn/wikidot.py"
 "Bug Tracker" = "https://github.com/ukwhatn/wikidot.py/issues"
```

### Comparing `wikidot-3.0.3/wikidot/common/decorators.py` & `wikidot-3.0.4/src/wikidot/common/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,29 +7,30 @@
     関数のパラメータに存在するclientを取得し、ログインしていない場合は例外を送出する
     clientはパラメータ、もしくはself.clientで取得できる
     """
 
     @wraps(func)
     def wrapper(*args, **kwargs):
         client = None
-        if 'client' in kwargs:
-            client = kwargs['client']
+        if "client" in kwargs:
+            client = kwargs["client"]
         else:
             from wikidot.module.client import Client
+
             for arg in args:
                 if isinstance(arg, Client):
                     client = arg
                     break
 
             # selfに存在するか？
             if client is None:
-                if hasattr(args[0], 'client'):
+                if hasattr(args[0], "client"):
                     client = args[0].client
 
         if client is None:
-            raise ValueError('Client is not found')
+            raise ValueError("Client is not found")
 
         client.login_check()
 
         return func(*args, **kwargs)
 
     return wrapper
```

### Comparing `wikidot-3.0.3/wikidot/common/exceptions.py` & `wikidot-3.0.4/src/wikidot/common/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # ---
 # 基底クラス
 # ---
 
+
 class WikidotException(Exception):
     """独自例外の基底クラス"""
 
     def __init__(self, message):
         super().__init__(message)
 
 
 # ---
 # ワイルドカード
 # ---
 
+
 class UnexpectedException(WikidotException):
     """予期せぬ例外が発生したときの例外"""
 
     def __init__(self, message):
         super().__init__(message)
 
 
 # ---
 # セッション関連
 # ---
 
+
 class SessionCreateException(WikidotException):
     """セッションの作成に失敗したときの例外"""
 
     def __init__(self, message):
         super().__init__(message)
 
 
@@ -74,14 +77,15 @@
         super().__init__(message)
 
 
 # ---
 # ターゲットエラー関連
 # ---
 
+
 class NotFoundException(WikidotException):
     """サイトやページ・ユーザが見つからなかったときの例外"""
 
     def __init__(self, message):
         super().__init__(message)
```

### Comparing `wikidot-3.0.3/wikidot/connector/ajax.py` & `wikidot-3.0.4/src/wikidot/connector/ajax.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,45 +2,53 @@
 import json.decoder
 from dataclasses import dataclass
 from typing import Any
 
 import httpx
 
 from ..common import wd_logger
-from ..common.exceptions import NotFoundException, AMCHttpStatusCodeException, ResponseDataException, \
-    WikidotStatusCodeException
+from ..common.exceptions import (
+    AMCHttpStatusCodeException,
+    NotFoundException,
+    ResponseDataException,
+    WikidotStatusCodeException,
+)
 
 
 class AjaxRequestHeader:
     """ajax-module-connector.phpへのリクエスト時に利用するヘッダの構築用クラス"""
 
-    def __init__(self,
-                 content_type: str | None = None,
-                 user_agent: str | None = None,
-                 referer: str | None = None,
-                 cookie: dict | None = None):
+    def __init__(
+        self,
+        content_type: str | None = None,
+        user_agent: str | None = None,
+        referer: str | None = None,
+        cookie: dict | None = None,
+    ):
         """AjaxRequestHeaderオブジェクトの初期化
 
         Parameters
         ----------
         content_type: str | None
             Content-Type
         user_agent: str | None
             User-Agent
         referer: str | None
             Referer
         cookie: dict | None
             Cookie
         """
-        self.content_type: str = "application/x-www-form-urlencoded; charset=UTF-8" if content_type is None else content_type
+        self.content_type: str = (
+            "application/x-www-form-urlencoded; charset=UTF-8"
+            if content_type is None
+            else content_type
+        )
         self.user_agent: str = "WikidotPy" if user_agent is None else user_agent
         self.referer: str = "https://www.wikidot.com/" if referer is None else referer
-        self.cookie: dict[str, any] = {
-            "wikidot_token7": 123456
-        }
+        self.cookie: dict[str, Any] = {"wikidot_token7": 123456}
         if cookie is not None:
             self.cookie.update(cookie)
         return
 
     def set_cookie(self, name, value) -> None:
         """Cookieを設定する
 
@@ -73,15 +81,17 @@
         dict
             ヘッダ
         """
         return {
             "Content-Type": self.content_type,
             "User-Agent": self.user_agent,
             "Referer": self.referer,
-            "Cookie": "".join([f'{name}={value};' for name, value in self.cookie.items()])
+            "Cookie": "".join(
+                [f"{name}={value};" for name, value in self.cookie.items()]
+            ),
         }
 
 
 @dataclass
 class AjaxModuleConnectorConfig:
     """ajax-module-connector.phpへのリクエストを行う際の設定
 
@@ -92,68 +102,74 @@
     attempt_limit: int
         リクエストの試行回数上限
     retry_interval: int
         リクエスト失敗時のリトライ間隔
     semaphore_limit: int
         セマフォの上限
     """
+
     request_timeout: int = 20
     attempt_limit: int = 3
     retry_interval: int = 5
     semaphore_limit: int = 10
 
 
 class AjaxModuleConnectorClient:
     """ajax-module-connector.phpへのリクエストを行うクライアント"""
 
     def __init__(
-            self,
-            site_name: str | None = None,
-            config: AjaxModuleConnectorConfig | None = None
+        self,
+        site_name: str | None = None,
+        config: AjaxModuleConnectorConfig | None = None,
     ):
         """AjaxModuleConnectorClientオブジェクトの初期化
 
         Parameters
         ----------
         config: AjaxModuleConnectorConfig
             設定
         """
-        self.site_name: str = site_name if site_name is not None else 'www'
-        self.config: AjaxModuleConnectorConfig = config if config is not None else AjaxModuleConnectorConfig()
+        self.site_name: str = site_name if site_name is not None else "www"
+        self.config: AjaxModuleConnectorConfig = (
+            config if config is not None else AjaxModuleConnectorConfig()
+        )
 
         # ssl対応チェック
         self.ssl_supported: bool = self._check_existence_and_ssl()
 
         # ヘッダの初期化
         self.header: AjaxRequestHeader = AjaxRequestHeader()
 
     def _check_existence_and_ssl(self):
         """実際にアクセスしてみてサイトの存在とSSL対応をチェック"""
 
         # wwwは常にSSL対応
-        if self.site_name == 'www':
+        if self.site_name == "www":
             return True
 
         # それ以外のサイトはhttpsにリダイレクトされるかどうかで判断
-        response = httpx.get(f'http://{self.site_name}.wikidot.com')
+        response = httpx.get(f"http://{self.site_name}.wikidot.com")
 
         # 存在しなければ例外送出
         if response.status_code == httpx.codes.NOT_FOUND:
-            raise NotFoundException(f'Site is not found: {self.site_name}.wikidot.com')
+            raise NotFoundException(f"Site is not found: {self.site_name}.wikidot.com")
 
         # httpsにリダイレクトされているかどうかで判断
-        return response.status_code == httpx.codes.MOVED_PERMANENTLY and 'Location' in response.headers and \
-            response.headers['Location'].startswith('https')
+        return (
+            response.status_code == httpx.codes.MOVED_PERMANENTLY
+            and "Location" in response.headers
+            and response.headers["Location"].startswith("https")
+        )
 
     def request(
-            self,
-            bodies: list[dict[str, any]],
-            return_exceptions: bool = False,
-            site_name: str | None = None,
-            site_ssl_supported: bool | None = None
+        self,
+        bodies: list[dict[str, Any]],
+        return_exceptions: bool = False,
+        site_name: str | None = None,
+        site_ssl_supported: bool | None = None,
     ) -> tuple[BaseException | Any]:
         """ajax-module-connector.phpへのリクエストを行う
 
         Parameters
         ----------
         bodies: list[dict]
             リクエストボディのリスト
@@ -184,92 +200,112 @@
         ResponseDataException
             AMCから返却されたデータが不正だったときの例外
             JSONデータとしてパースできなかった場合や空だった場合に投げる
         """
         semaphore_instance = asyncio.Semaphore(self.config.semaphore_limit)
 
         site_name = site_name if site_name is not None else self.site_name
-        site_ssl_supported = site_ssl_supported if site_ssl_supported is not None else self.ssl_supported
+        site_ssl_supported = (
+            site_ssl_supported if site_ssl_supported is not None else self.ssl_supported
+        )
 
-        async def _request(
-                _body: dict[str, any]
-        ) -> httpx.Response:
+        async def _request(_body: dict[str, Any]) -> httpx.Response:
             retry_count = 0
 
             while True:
 
                 # リクエスト実行
                 try:
                     # Semaphoreで同時実行数制御
                     async with semaphore_instance:
                         async with httpx.AsyncClient() as client:
                             url = (
                                 f'http{"s" if site_ssl_supported else ""}://{site_name}.wikidot.com/'
-                                f'ajax-module-connector.php')
-                            _body['wikidot_token7'] = 123456
-                            wd_logger.debug(f'Ajax Request: {url} -> {_body}')
+                                f"ajax-module-connector.php"
+                            )
+                            _body["wikidot_token7"] = 123456
+                            wd_logger.debug(f"Ajax Request: {url} -> {_body}")
                             response = await client.post(
                                 url,
                                 headers=self.header.get_header(),
                                 data=_body,
-                                timeout=self.config.request_timeout
+                                timeout=self.config.request_timeout,
                             )
                             response.raise_for_status()
                 except (httpx.HTTPStatusError, httpx.TimeoutException) as e:
                     # HTTPステータスエラーまたはタイムアウトの場合はリトライ
                     retry_count += 1
 
                     # リトライ回数上限に達した場合は例外送出
                     if retry_count >= self.config.attempt_limit:
-                        wd_logger.error(f'AMC is respond HTTP error code: {response.status_code} -> {_body}')
+                        wd_logger.error(
+                            f"AMC is respond HTTP error code: {response.status_code} -> {_body}"
+                        )
                         raise AMCHttpStatusCodeException(
-                            f'AMC is respond HTTP error code: {response.status_code}',
-                            response.status_code
+                            f"AMC is respond HTTP error code: {response.status_code}",
+                            response.status_code,
                         ) from e
 
                     # 間隔を空けてリトライ
-                    wd_logger.info(f'AMC is respond status: {response.status_code} (retry: {retry_count}) -> {_body}')
+                    wd_logger.info(
+                        f"AMC is respond status: {response.status_code} (retry: {retry_count}) -> {_body}"
+                    )
                     await asyncio.sleep(self.config.retry_interval)
                     continue
 
                 # bodyをJSONデータとしてパース
                 try:
                     _response_body = response.json()
                 except json.decoder.JSONDecodeError as e:
                     # パースできなかったらエラーとして扱う
-                    wd_logger.error(f'AMC is respond non-json data: "{response.text}" -> {_body}')
-                    raise ResponseDataException(f'AMC is respond non-json data: "{response.text}"') from e
+                    wd_logger.error(
+                        f'AMC is respond non-json data: "{response.text}" -> {_body}'
+                    )
+                    raise ResponseDataException(
+                        f'AMC is respond non-json data: "{response.text}"'
+                    ) from e
 
                 # レスポンスが空だったらエラーとして扱う
                 if _response_body is None or len(_response_body) == 0:
-                    wd_logger.error(f'AMC is respond empty data -> {_body}')
-                    raise ResponseDataException(f'AMC is respond empty data')
+                    wd_logger.error(f"AMC is respond empty data -> {_body}")
+                    raise ResponseDataException("AMC is respond empty data")
 
                 # 中身のstatusがokでなかったらエラーとして扱う
-                if 'status' in _response_body:
+                if "status" in _response_body:
                     # statusがtry_againの場合はリトライ
-                    if _response_body['status'] == 'try_again':
+                    if _response_body["status"] == "try_again":
                         retry_count += 1
                         if retry_count >= self.config.attempt_limit:
-                            wd_logger.error(f'AMC is respond status: "try_again" -> {_body}')
-                            raise WikidotStatusCodeException(f'AMC is respond status: "try_again"', 'try_again')
+                            wd_logger.error(
+                                f'AMC is respond status: "try_again" -> {_body}'
+                            )
+                            raise WikidotStatusCodeException(
+                                'AMC is respond status: "try_again"', "try_again"
+                            )
 
-                        wd_logger.info(f'AMC is respond status: "try_again" (retry: {retry_count})')
+                        wd_logger.info(
+                            f'AMC is respond status: "try_again" (retry: {retry_count})'
+                        )
                         await asyncio.sleep(self.config.retry_interval)
                         continue
 
                     # それ以外でstatusがokでない場合はエラーとして扱う
-                    elif _response_body['status'] != 'ok':
-                        wd_logger.error(f'AMC is respond error status: "{_response_body["status"]}" -> {_body}')
+                    elif _response_body["status"] != "ok":
+                        wd_logger.error(
+                            f'AMC is respond error status: "{_response_body["status"]}" -> {_body}'
+                        )
                         raise WikidotStatusCodeException(
                             f'AMC is respond error status: "{_response_body["status"]}"',
-                            _response_body['status']
+                            _response_body["status"],
                         )
 
                 # レスポンスを返す
                 return response
 
         async def _execute_requests():
-            return await asyncio.gather(*[_request(body) for body in bodies], return_exceptions=return_exceptions)
+            return await asyncio.gather(
+                *[_request(body) for body in bodies],
+                return_exceptions=return_exceptions,
+            )
 
         # 処理を実行
         return asyncio.run(_execute_requests())
```

### Comparing `wikidot-3.0.3/wikidot/module/auth.py` & `wikidot-3.0.4/src/wikidot/module/auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,63 +7,69 @@
 if TYPE_CHECKING:
     from wikidot.module.client import Client
 
 
 class HTTPAuthentication:
     @staticmethod
     def login(
-            client: 'Client',
-            username: str,
-            password: str,
+        client: "Client",
+        username: str,
+        password: str,
     ):
         """ユーザー名とパスワードでログインする
 
         Parameters
         ----------
         client: Client
             クライアント
         username: str
             ユーザー名
         password: str
             パスワード
         """
         # ログインリクエスト実行
         response = httpx.post(
-            url='https://www.wikidot.com/default--flow/login__LoginPopupScreen',
+            url="https://www.wikidot.com/default--flow/login__LoginPopupScreen",
             data={
-                'login': username,
-                'password': password,
-                'action': 'Login2Action',
-                'event': 'login'
+                "login": username,
+                "password": password,
+                "action": "Login2Action",
+                "event": "login",
             },
             headers=client.amc_client.header.get_header(),
-            timeout=20
+            timeout=20,
         )
 
         # Check status code
         if response.status_code != httpx.codes.OK:
             raise SessionCreateException(
-                'Login attempt is failed due to HTTP status code: ' + str(response.status_code))
+                "Login attempt is failed due to HTTP status code: "
+                + str(response.status_code)
+            )
 
         # Check body
-        if 'The login and password do not match' in response.text:
-            raise SessionCreateException('Login attempt is failed due to invalid username or password')
+        if "The login and password do not match" in response.text:
+            raise SessionCreateException(
+                "Login attempt is failed due to invalid username or password"
+            )
 
         # Check cookies
-        if 'WIKIDOT_SESSION_ID' not in response.cookies:
-            raise SessionCreateException('Login attempt is failed due to invalid cookies')
+        if "WIKIDOT_SESSION_ID" not in response.cookies:
+            raise SessionCreateException(
+                "Login attempt is failed due to invalid cookies"
+            )
 
         # Set cookies
-        client.amc_client.header.set_cookie('WIKIDOT_SESSION_ID', response.cookies['WIKIDOT_SESSION_ID'])
+        client.amc_client.header.set_cookie(
+            "WIKIDOT_SESSION_ID", response.cookies["WIKIDOT_SESSION_ID"]
+        )
 
     @staticmethod
-    def logout(client: 'Client'):
+    def logout(client: "Client"):
         try:
-            client.amc_client.request([{
-                'action': 'Login2Action',
-                'event': 'logout',
-                'moduleName': 'Empty'
-            }])
+            client.amc_client.request(
+                [{"action": "Login2Action", "event": "logout", "moduleName": "Empty"}]
+            )
         except Exception:
             pass
 
-        client.amc_client.header.delete_cookie('WIKIDOT_SESSION_ID')
+        client.amc_client.header.delete_cookie("WIKIDOT_SESSION_ID")
```

### Comparing `wikidot-3.0.3/wikidot/module/client.py` & `wikidot-3.0.4/src/wikidot/module/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from wikidot.common import wd_logger
 from wikidot.common.exceptions import LoginRequiredException
 from wikidot.connector.ajax import AjaxModuleConnectorClient, AjaxModuleConnectorConfig
 from wikidot.module.auth import HTTPAuthentication
-from wikidot.module.private_message import PrivateMessage, PrivateMessageInbox, \
-    PrivateMessageSentBox, PrivateMessageCollection
+from wikidot.module.private_message import (
+    PrivateMessage,
+    PrivateMessageCollection,
+    PrivateMessageInbox,
+    PrivateMessageSentBox,
+)
 from wikidot.module.site import Site
 from wikidot.module.user import User, UserCollection
 
 
 class ClientUserMethods:
-    def __init__(self, client: 'Client'):
+    def __init__(self, client: "Client"):
         self.client = client
 
-    def get(
-            self,
-            name: str,
-            raise_when_not_found: bool = False
-    ) -> User:
+    def get(self, name: str, raise_when_not_found: bool = False) -> User:
         """ユーザー名からユーザーオブジェクトを取得する
 
         Parameters
         ----------
         name: str
             ユーザー名
 
@@ -32,17 +32,15 @@
         -------
         User
             ユーザーオブジェクト
         """
         return User.from_name(self.client, name, raise_when_not_found)
 
     def get_bulk(
-            self,
-            names: list[str],
-            raise_when_not_found: bool = False
+        self, names: list[str], raise_when_not_found: bool = False
     ) -> list[User]:
         """ユーザー名からユーザーオブジェクトを取得する
 
         Parameters
         ----------
         names: list[str]
             ユーザー名のリスト
@@ -55,23 +53,18 @@
         list[User]
             ユーザーオブジェクトのリスト
         """
         return UserCollection.from_names(self.client, names, raise_when_not_found)
 
 
 class ClientPrivateMessageMethods:
-    def __init__(self, client: 'Client'):
+    def __init__(self, client: "Client"):
         self.client = client
 
-    def send(
-            self,
-            recipient: User,
-            subject: str,
-            body: str
-    ) -> None:
+    def send(self, recipient: User, subject: str, body: str) -> None:
         """メッセージを送信する
 
         Parameters
         ----------
         recipient: User
             受信者
         subject: str
@@ -129,18 +122,18 @@
         PrivateMessage
             メッセージ
         """
         return PrivateMessage.from_id(self.client, message_id)
 
 
 class ClientSiteMethods:
-    def __init__(self, client: 'Client'):
+    def __init__(self, client: "Client"):
         self.client = client
 
-    def get(self, unix_name: str) -> 'Site':
+    def get(self, unix_name: str) -> "Site":
         """UNIX名からサイトオブジェクトを取得する
 
         Parameters
         ----------
         unix_name: str
             サイトのUNIX名
 
@@ -152,19 +145,19 @@
         return Site.from_unix_name(self.client, unix_name)
 
 
 class Client:
     """基幹クライアント"""
 
     def __init__(
-            self,
-            username: str | None = None,
-            password: str | None = None,
-            amc_config: AjaxModuleConnectorConfig | None = None,
-            logging_level: str = "WARNING"
+        self,
+        username: str | None = None,
+        password: str | None = None,
+        amc_config: AjaxModuleConnectorConfig | None = None,
+        logging_level: str = "WARNING",
     ):
         """Wikidot Client
 
         Parameters
         ----------
         username: str | None
             ユーザー名
@@ -175,18 +168,15 @@
         logging_level: str
             ロギングレベル
         """
         # 最初にロギングレベルを決定する
         wd_logger.setLevel(logging_level)
 
         # AMCClientを初期化
-        self.amc_client = AjaxModuleConnectorClient(
-            site_name=None,
-            config=amc_config
-        )
+        self.amc_client = AjaxModuleConnectorClient(site_name=None, config=amc_config)
 
         # セッション関連変数の初期化
         self.is_logged_in = False
         self.username = None
 
         # usernameとpasswordが指定されていればログインする
         if username is not None and password is not None:
@@ -222,9 +212,9 @@
         return
 
     def __str__(self):
         return f"Client(username={self.username}, is_logged_in={self.is_logged_in})"
 
     def login_check(self) -> None:
         if not self.is_logged_in:
-            raise LoginRequiredException('Login is required to execute this function')
+            raise LoginRequiredException("Login is required to execute this function")
         return
```

### Comparing `wikidot-3.0.3/wikidot/module/page.py` & `wikidot-3.0.4/src/wikidot/module/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import re
 from collections.abc import Iterator
-from dataclasses import dataclass, asdict
+from dataclasses import asdict, dataclass
 from datetime import datetime
-from typing import TYPE_CHECKING, Optional, Union, Any
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from bs4 import BeautifulSoup
 
 from wikidot.common import exceptions
 from wikidot.module.page_revision import PageRevision, PageRevisionCollection
 from wikidot.module.page_source import PageSource
 from wikidot.module.page_votes import PageVote, PageVoteCollection
-from wikidot.util.parser import user as user_parser, odate as odate_parser
+from wikidot.util.parser import odate as odate_parser
+from wikidot.util.parser import user as user_parser
 from wikidot.util.requestutil import RequestUtil
 
 if TYPE_CHECKING:
     from wikidot.module.site import Site
     from wikidot.module.user import User
 
 DEFAULT_MODULE_BODY = [
@@ -47,15 +48,15 @@
     pagetype: Optional[str] = "*"
     category: Optional[str] = "*"
     tags: Optional[str | list[str]] = None
     parent: Optional[str] = None
     link_to: Optional[str] = None
     created_at: Optional[str] = None
     updated_at: Optional[str] = None
-    created_by: Optional[Union['User', str]] = None
+    created_by: Optional[Union["User", str]] = None
     rating: Optional[str] = None
     votes: Optional[str] = None
     name: Optional[str] = None
     fullname: Optional[str] = None
     range: Optional[str] = None
 
     # ordering
@@ -72,35 +73,38 @@
     def as_dict(self) -> dict[str, Any]:
         res = {k: v for k, v in asdict(self).items() if v is not None}
         if "tags" in res and isinstance(res["tags"], list):
             res["tags"] = " ".join(res["tags"])
         return res
 
 
-class PageCollection(list['Page']):
-    def __init__(self, site: 'Site' = None, pages: list['Page'] = None):
+class PageCollection(list["Page"]):
+    def __init__(self, site: "Site" = None, pages: list["Page"] = None):
         super().__init__(pages or [])
 
         if site is not None:
             self.site = site
         else:
             self.site = self[0].site
 
-    def __iter__(self) -> Iterator['Page']:
+    def __iter__(self) -> Iterator["Page"]:
         return super().__iter__()
 
     @staticmethod
-    def _parse(site: 'Site', html_body: BeautifulSoup):
+    def _parse(site: "Site", html_body: BeautifulSoup):
         pages = []
 
         for page_element in html_body.select("span.page"):
             page_params = {}
 
             # レーティング方式を判定
-            is_5star_rating = page_element.select_one("span.rating span.page-rate-list-pages-start") is not None
+            is_5star_rating = (
+                page_element.select_one("span.rating span.page-rate-list-pages-start")
+                is not None
+            )
 
             # 各値を取得
             for set_element in page_element.select("span.set"):
                 key = set_element.select_one("span.name").text.strip()
                 value_element = set_element.select_one("span.value")
 
                 if value_element is None:
@@ -109,15 +113,19 @@
                 elif key in ["created_at", "updated_at", "commented_at"]:
                     odate_element = value_element.select_one("span.odate")
                     if odate_element is None:
                         value = None
                     else:
                         value = odate_parser(odate_element)
 
-                elif key in ["created_by_linked", "updated_by_linked", "commented_by_linked"]:
+                elif key in [
+                    "created_by_linked",
+                    "updated_by_linked",
+                    "commented_by_linked",
+                ]:
                     printuser_element = value_element.select_one("span.printuser")
                     if printuser_element is None:
                         value = None
                     else:
                         value = user_parser(site.client, printuser_element)
 
                 elif key in ["tags", "_tags"]:
@@ -161,175 +169,200 @@
 
             # ページオブジェクトを作成
             pages.append(Page(site, **page_params))
 
         return PageCollection(site, pages)
 
     @staticmethod
-    def search_pages(
-            site: 'Site',
-            query: SearchPagesQuery = SearchPagesQuery()
-    ):
+    def search_pages(site: "Site", query: SearchPagesQuery = SearchPagesQuery()):
         # 初回実行
         query_dict = query.as_dict()
         query_dict["moduleName"] = "list/ListPagesModule"
-        query_dict["module_body"] = '[[span class="page"]]' + "".join(
-            [
-                f'[[span class="set {key}"]]'
-                f'[[span class="name"]] {key} [[/span]]'
-                f'[[span class="value"]] %%{key}%% [[/span]]'
-                f'[[/span]]'
-                for key in DEFAULT_MODULE_BODY
-            ]
-        ) + "[[/span]]"
+        query_dict["module_body"] = (
+            '[[span class="page"]]'
+            + "".join(
+                [
+                    f'[[span class="set {key}"]]'
+                    f'[[span class="name"]] {key} [[/span]]'
+                    f'[[span class="value"]] %%{key}%% [[/span]]'
+                    f"[[/span]]"
+                    for key in DEFAULT_MODULE_BODY
+                ]
+            )
+            + "[[/span]]"
+        )
 
         try:
             response = site.amc_request([query_dict])[0]
         except exceptions.WikidotStatusCodeException as e:
             if e.status_code == "not_ok":
-                raise exceptions.ForbiddenException("Failed to get pages, target site may be private") from e
+                raise exceptions.ForbiddenException(
+                    "Failed to get pages, target site may be private"
+                ) from e
             raise e
 
         body = response.json()["body"]
 
         first_page_html_body = BeautifulSoup(body, "lxml")
 
         total = 1
         html_bodies = [first_page_html_body]
         # pagerが存在する
         if first_page_html_body.select_one("div.pager") is not None:
             # span.target[-2] > a から最大ページ数を取得
-            total = int(first_page_html_body.select("div.pager span.target")[-2].select_one("a").text)
+            total = int(
+                first_page_html_body.select("div.pager span.target")[-2]
+                .select_one("a")
+                .text
+            )
 
         if total > 1:
             request_bodies = []
             for i in range(1, total):
                 _query_dict = query_dict.copy()
                 _query_dict["offset"] = i * query.perPage
                 request_bodies.append(_query_dict)
 
             responses = site.amc_request(request_bodies)
-            html_bodies.extend([BeautifulSoup(response.json()["body"], "lxml") for response in responses])
+            html_bodies.extend(
+                [
+                    BeautifulSoup(response.json()["body"], "lxml")
+                    for response in responses
+                ]
+            )
 
         pages = []
         for html_body in html_bodies:
             pages.extend(PageCollection._parse(site, html_body))
 
         return PageCollection(site, pages)
 
     @staticmethod
-    def _acquire_page_ids(
-            site: 'Site',
-            pages: list['Page']
-    ):
+    def _acquire_page_ids(site: "Site", pages: list["Page"]):
         # pagesからidが設定されていないものを抽出
         target_pages = [page for page in pages if not page.is_id_acquired()]
 
         # なければ終了
         if len(target_pages) == 0:
             return pages
 
         # norender, noredirectでアクセス
         responses = RequestUtil.request(
             site.client,
             "GET",
-            [f"{page.get_url()}/norender/true/noredirect/true" for page in target_pages]
+            [
+                f"{page.get_url()}/norender/true/noredirect/true"
+                for page in target_pages
+            ],
         )
 
         # "WIKIREQUEST.info.pageId = xxx;"の値をidに設定
         for index, response in enumerate(responses):
             source = response.text
 
-            id_match = re.search(r'WIKIREQUEST\.info\.pageId = (\d+);', source)
+            id_match = re.search(r"WIKIREQUEST\.info\.pageId = (\d+);", source)
             if id_match is None:
-                raise exceptions.UnexpectedException(f'Cannot find page id: {target_pages[index].fullname}')
+                raise exceptions.UnexpectedException(
+                    f"Cannot find page id: {target_pages[index].fullname}"
+                )
             target_pages[index].id = int(id_match.group(1))
 
         return pages
 
     def get_page_ids(self):
         return PageCollection._acquire_page_ids(self.site, self)
 
     @staticmethod
-    def _acquire_page_sources(
-            site: 'Site',
-            pages: list['Page']
-    ):
+    def _acquire_page_sources(site: "Site", pages: list["Page"]):
         if len(pages) == 0:
             return pages
 
-        responses = site.amc_request([{
-            "moduleName": "viewsource/ViewSourceModule",
-            "page_id": page.id
-        } for page in pages])
+        responses = site.amc_request(
+            [
+                {"moduleName": "viewsource/ViewSourceModule", "page_id": page.id}
+                for page in pages
+            ]
+        )
 
         for page, responses in zip(pages, responses):
             body = responses.json()["body"]
-            source = BeautifulSoup(body, "lxml").select_one("div.page-source").text.strip().removeprefix("\t")
+            source = (
+                BeautifulSoup(body, "lxml")
+                .select_one("div.page-source")
+                .text.strip()
+                .removeprefix("\t")
+            )
             page.source = PageSource(page, source)
         return pages
 
     def get_page_sources(self):
         return PageCollection._acquire_page_sources(self.site, self)
 
     @staticmethod
-    def _acquire_page_revisions(
-            site: 'Site',
-            pages: list['Page']
-    ):
+    def _acquire_page_revisions(site: "Site", pages: list["Page"]):
         if len(pages) == 0:
             return pages
 
-        responses = site.amc_request([{
-            "moduleName": "history/PageRevisionListModule",
-            "page_id": page.id,
-            "options": {"all": True},
-            "perpage": 100000000  # pagerを使わずに全て取得
-        } for page in pages])
+        responses = site.amc_request(
+            [
+                {
+                    "moduleName": "history/PageRevisionListModule",
+                    "page_id": page.id,
+                    "options": {"all": True},
+                    "perpage": 100000000,  # pagerを使わずに全て取得
+                }
+                for page in pages
+            ]
+        )
 
         for page, response in zip(pages, responses):
             body = response.json()["body"]
             revs = []
             body_html = BeautifulSoup(body, "lxml")
-            for rev_element in body_html.select('table.page-history > tr[id^=revision-row-]'):
+            for rev_element in body_html.select(
+                "table.page-history > tr[id^=revision-row-]"
+            ):
                 rev_id = int(rev_element["id"].removeprefix("revision-row-"))
 
                 tds = rev_element.select("td")
                 rev_no = int(tds[0].text.strip().removesuffix("."))
-                created_by = user_parser(page.site.client, tds[4].select_one("span.printuser"))
+                created_by = user_parser(
+                    page.site.client, tds[4].select_one("span.printuser")
+                )
                 created_at = odate_parser(tds[5].select_one("span.odate"))
                 comment = tds[6].text.strip()
 
-                revs.append(PageRevision(
-                    page=page,
-                    id=rev_id,
-                    rev_no=rev_no,
-                    created_by=created_by,
-                    created_at=created_at,
-                    comment=comment
-                ))
+                revs.append(
+                    PageRevision(
+                        page=page,
+                        id=rev_id,
+                        rev_no=rev_no,
+                        created_by=created_by,
+                        created_at=created_at,
+                        comment=comment,
+                    )
+                )
             page.revisions = revs
 
         return pages
 
     def get_page_revisions(self):
         return PageCollection._acquire_page_revisions(self.site, self)
 
     @staticmethod
-    def _acquire_page_votes(
-            site: 'Site',
-            pages: list['Page']
-    ):
+    def _acquire_page_votes(site: "Site", pages: list["Page"]):
         if len(pages) == 0:
             return pages
 
-        responses = site.amc_request([{
-            "moduleName": "pagerate/WhoRatedPageModule",
-            "pageId": page.id
-        } for page in pages])
+        responses = site.amc_request(
+            [
+                {"moduleName": "pagerate/WhoRatedPageModule", "pageId": page.id}
+                for page in pages
+            ]
+        )
 
         for page, response in zip(pages, responses):
             body = response.json()["body"]
             html = BeautifulSoup(body, "lxml")
             user_elems = html.select("span.printuser")
             value_elems = html.select("span[style^='color']")
 
@@ -343,17 +376,15 @@
                 if value == "+":
                     values.append(1)
                 elif value == "-":
                     values.append(-1)
                 else:
                     values.append(int(value))
 
-            votes = [
-                PageVote(page, user, vote) for user, vote in zip(users, values)
-            ]
+            votes = [PageVote(page, user, vote) for user, vote in zip(users, values)]
             page._votes = PageVoteCollection(page.site, votes)
 
         return pages
 
     def get_page_votes(self):
         return PageCollection._acquire_page_votes(self.site, self)
 
@@ -403,37 +434,38 @@
     commented_by: Optional[User]
         コメントしたユーザ
     commented_at: datetime
         コメント日時
     _id: int
         ページID
     """
-    site: 'Site'
+
+    site: "Site"
     fullname: str
     name: str
     category: str
     title: str
     children_count: int
     comments_count: int
     size: int
     rating: int | float
     votes_count: int
     rating_percent: float
     revisions_count: int
     parent_fullname: str | None
     tags: list[str]
-    created_by: 'User'
+    created_by: "User"
     created_at: datetime
-    updated_by: 'User'
+    updated_by: "User"
     updated_at: datetime
-    commented_by: Optional['User']
+    commented_by: Optional["User"]
     commented_at: datetime
     _id: int = None
     _source: Optional[PageSource] = None
-    _revisions: list['PageRevision'] = None
+    _revisions: list["PageRevision"] = None
     _votes: PageVoteCollection = None
 
     def get_url(self) -> str:
         return f"{self.site.get_url()}/{self.fullname}"
 
     @property
     def id(self) -> int:
@@ -462,21 +494,23 @@
         return self._source
 
     @source.setter
     def source(self, value: PageSource):
         self._source = value
 
     @property
-    def revisions(self) -> PageRevisionCollection['PageRevision']:
+    def revisions(self) -> PageRevisionCollection["PageRevision"]:
         if self._revisions is None:
             PageCollection(self.site, [self]).get_page_revisions()
         return PageRevisionCollection(self, self._revisions)
 
     @revisions.setter
-    def revisions(self, value: list['PageRevision'] | PageRevisionCollection['PageRevision']):
+    def revisions(
+        self, value: list["PageRevision"] | PageRevisionCollection["PageRevision"]
+    ):
         self._revisions = value
 
     @property
     def latest_revision(self) -> PageRevision:
         # revision_countとrev_noが一致するものを取得
         for revision in self.revisions:
             if revision.rev_no == self.revisions_count:
@@ -492,13 +526,17 @@
 
     @votes.setter
     def votes(self, value: PageVoteCollection):
         self._votes = value
 
     def destroy(self):
         self.site.client.login_check()
-        self.site.amc_request([{
-            "action": "WikiPageAction",
-            "event": "deletePage",
-            "page_id": self.id,
-            "moduleName": "Empty"
-        }])
+        self.site.amc_request(
+            [
+                {
+                    "action": "WikiPageAction",
+                    "event": "deletePage",
+                    "page_id": self.id,
+                    "moduleName": "Empty",
+                }
+            ]
+        )
```

### Comparing `wikidot-3.0.3/wikidot/module/page_revision.py` & `wikidot-3.0.4/src/wikidot/module/page_revision.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,103 +8,109 @@
 from wikidot.module.page_source import PageSource
 
 if TYPE_CHECKING:
     from wikidot.module.page import Page
     from wikidot.module.user import AbstractUser
 
 
-class PageRevisionCollection(list['PageRevision']):
-    def __init__(self, page: 'Page' = None, revisions: list['PageRevision'] = None):
+class PageRevisionCollection(list["PageRevision"]):
+    def __init__(self, page: "Page" = None, revisions: list["PageRevision"] = None):
         super().__init__(revisions or [])
         self.page = page or revisions[0].page
 
-    def __iter__(self) -> Iterator['PageRevision']:
+    def __iter__(self) -> Iterator["PageRevision"]:
         return super().__iter__()
 
     @staticmethod
-    def _acquire_sources(page, revisions: list['PageRevision']):
-        target_revisions = [revision for revision in revisions if not revision.is_source_acquired()]
+    def _acquire_sources(page, revisions: list["PageRevision"]):
+        target_revisions = [
+            revision for revision in revisions if not revision.is_source_acquired()
+        ]
 
         if len(target_revisions) == 0:
             return revisions
 
         responses = page.site.amc_request(
-            [{
-                'moduleName': 'history/PageSourceModule',
-                'revision_id': revision.id
-            } for revision in target_revisions]
+            [
+                {"moduleName": "history/PageSourceModule", "revision_id": revision.id}
+                for revision in target_revisions
+            ]
         )
 
         for revision, response in zip(target_revisions, responses):
-            body = response.json()['body']
-            body_html = BeautifulSoup(body, 'lxml')
+            body = response.json()["body"]
+            body_html = BeautifulSoup(body, "lxml")
             revision.source = PageSource(
                 page=page,
-                wiki_text=body_html.select_one("div.page-source").text.strip()
+                wiki_text=body_html.select_one("div.page-source").text.strip(),
             )
 
         return revisions
 
     def get_sources(self):
         return self._acquire_sources(self.page, self)
 
     @staticmethod
-    def _acquire_htmls(page, revisions: list['PageRevision']):
-        target_revisions = [revision for revision in revisions if not revision.is_html_acquired()]
+    def _acquire_htmls(page, revisions: list["PageRevision"]):
+        target_revisions = [
+            revision for revision in revisions if not revision.is_html_acquired()
+        ]
 
         if len(target_revisions) == 0:
             return revisions
 
         responses = page.site.amc_request(
-            [{
-                'moduleName': 'history/PageVersionModule',
-                'revision_id': revision.id
-            } for revision in target_revisions]
+            [
+                {"moduleName": "history/PageVersionModule", "revision_id": revision.id}
+                for revision in target_revisions
+            ]
         )
 
         for revision, response in zip(target_revisions, responses):
-            body = response.json()['body']
+            body = response.json()["body"]
             # onclick="document.getElementById('page-version-info').style.display='none'">(.*?)</a>\n\t</div>\n\n\n\n
             # 以降をソースとして取得
-            source = body.split('onclick="document.getElementById(\'page-version-info\').style.display=\'none\'">',
-                                maxsplit=1)[1]
-            source = source.split('</a>\n\t</div>\n\n\n\n', maxsplit=1)[1]
+            source = body.split(
+                "onclick=\"document.getElementById('page-version-info').style.display='none'\">",
+                maxsplit=1,
+            )[1]
+            source = source.split("</a>\n\t</div>\n\n\n\n", maxsplit=1)[1]
             revision._html = source
 
         return revisions
 
     def get_htmls(self):
         return self._acquire_htmls(self.page, self)
 
 
 @dataclass
 class PageRevision:
-    page: 'Page'
+    page: "Page"
     id: int
     rev_no: int
-    created_by: 'AbstractUser'
+    created_by: "AbstractUser"
     created_at: datetime
     comment: str
-    _source: Optional['PageSource'] = None
+    _source: Optional["PageSource"] = None
     _html: Optional[str] = None
 
     def is_source_acquired(self) -> bool:
         return self._source is not None
 
     def is_html_acquired(self) -> bool:
         return self._html is not None
 
     @property
-    def source(self) -> 'PageSource':
+    def source(self) -> "PageSource":
         if not self.is_source_acquired():
             PageRevisionCollection(self.page, [self]).get_sources()
         return self._source
 
     @source.setter
-    def source(self, value: 'PageSource'):
+    def source(self, value: "PageSource"):
         self._source = value
 
     @property
     def html(self) -> str:
         if not self.is_html_acquired():
             PageRevisionCollection(self.page, [self]).get_htmls()
         return self._html
```

### Comparing `wikidot-3.0.3/wikidot/module/private_message.py` & `wikidot-3.0.4/src/wikidot/module/private_message.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,37 @@
+from collections.abc import Iterator
 from dataclasses import dataclass
 from datetime import datetime
 from typing import TYPE_CHECKING
-from collections.abc import Iterator
 
 import httpx
-from bs4 import BeautifulSoup, Tag, ResultSet
+from bs4 import BeautifulSoup, ResultSet, Tag
 
 from wikidot.common import exceptions
 from wikidot.common.decorators import login_required
-from wikidot.util.parser import odate as odate_parser, user as user_parser
+from wikidot.util.parser import odate as odate_parser
+from wikidot.util.parser import user as user_parser
 
 if TYPE_CHECKING:
-    from wikidot.module.user import AbstractUser, User
     from wikidot.module.client import Client
+    from wikidot.module.user import AbstractUser, User
 
 
-class PrivateMessageCollection(list['PrivateMessage']):
+class PrivateMessageCollection(list["PrivateMessage"]):
     def __str__(self):
-        return f'{self.__class__.__name__}({len(self)} messages)'
+        return f"{self.__class__.__name__}({len(self)} messages)"
 
-    def __iter__(self) -> Iterator['PrivateMessage']:
+    def __iter__(self) -> Iterator["PrivateMessage"]:
         return super().__iter__()
 
     @staticmethod
     @login_required
     def from_ids(
-            client: 'Client',
-            message_ids: list[int]
-    ) -> 'PrivateMessageCollection':
+        client: "Client", message_ids: list[int]
+    ) -> "PrivateMessageCollection":
         """メッセージIDのリストからメッセージオブジェクトのリストを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
         message_ids: list[int]
@@ -41,52 +41,60 @@
         -------
         PrivateMessageCollection
             メッセージオブジェクトのリスト
         """
         bodies = []
 
         for message_id in message_ids:
-            bodies.append({
-                'item': message_id,
-                'moduleName': 'dashboard/messages/DMViewMessageModule'
-            })
+            bodies.append(
+                {
+                    "item": message_id,
+                    "moduleName": "dashboard/messages/DMViewMessageModule",
+                }
+            )
 
-        responses: [httpx.Response | Exception] = client.amc_client.request(bodies, return_exceptions=True)
+        responses: [httpx.Response | Exception] = client.amc_client.request(
+            bodies, return_exceptions=True
+        )
 
         messages = []
 
         for index, response in enumerate(responses):
             if isinstance(response, exceptions.WikidotStatusCodeException):
                 if response.status_code == "no_message":
-                    raise exceptions.ForbiddenException(f'Failed to get message: {message_ids[index]}') from response
+                    raise exceptions.ForbiddenException(
+                        f"Failed to get message: {message_ids[index]}"
+                    ) from response
 
             if isinstance(response, Exception):
                 raise response
 
-            html = BeautifulSoup(response.json()['body'], 'lxml')
+            html = BeautifulSoup(response.json()["body"], "lxml")
 
-            sender, recipient = html.select('div.pmessage div.header span.printuser')
+            sender, recipient = html.select("div.pmessage div.header span.printuser")
 
             messages.append(
                 PrivateMessage(
                     client=client,
                     id=message_ids[index],
                     sender=user_parser(client, sender),
                     recipient=user_parser(client, recipient),
-                    subject=html.select_one('div.pmessage div.header span.subject').get_text(),
-                    body=html.select_one('div.pmessage div.body').get_text(),
-                    created_at=odate_parser(html.select_one('div.header span.odate'))
+                    subject=html.select_one(
+                        "div.pmessage div.header span.subject"
+                    ).get_text(),
+                    body=html.select_one("div.pmessage div.body").get_text(),
+                    created_at=odate_parser(html.select_one("div.header span.odate")),
                 )
             )
 
         return PrivateMessageCollection(messages)
 
     @staticmethod
     @login_required
-    def _acquire(client: 'Client', module_name: str):
+    def _acquire(client: "Client", module_name: str):
         """受信・送信箱のメッセージを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
         module_name: str
@@ -94,121 +102,129 @@
 
         Returns
         -------
         PrivateMessageCollection
             受信箱のメッセージ
         """
         # pager取得
-        response = client.amc_client.request([{
-            'moduleName': module_name
-        }])[0]
+        response = client.amc_client.request([{"moduleName": module_name}])[0]
 
-        html = BeautifulSoup(response.json()['body'], 'lxml')
+        html = BeautifulSoup(response.json()["body"], "lxml")
         # pagerの最後から2番目の要素を取得
         # pageが存在しない場合は1ページのみ
-        pager: ResultSet[Tag] = html.select('div.pager span.target')
+        pager: ResultSet[Tag] = html.select("div.pager span.target")
         max_page: int = int(pager[-2].get_text()) if len(pager) > 2 else 1
 
         if max_page > 1:
             # メッセージ取得
-            bodies = [{
-                'page': page,
-                'moduleName': module_name
-            } for page in range(1, max_page + 1)]
+            bodies = [
+                {"page": page, "moduleName": module_name}
+                for page in range(1, max_page + 1)
+            ]
 
-            responses: [httpx.Response | Exception] = client.amc_client.request(bodies, return_exceptions=False)
+            responses: [httpx.Response | Exception] = client.amc_client.request(
+                bodies, return_exceptions=False
+            )
         else:
             responses = [response]
 
         message_ids = []
         for response in responses:
-            html = BeautifulSoup(response.json()['body'], 'lxml')
+            html = BeautifulSoup(response.json()["body"], "lxml")
             # tr.messageのdata-href末尾の数字を取得
-            message_ids.extend([int(tr['data-href'].split('/')[-1]) for tr in html.select('tr.message')])
+            message_ids.extend(
+                [
+                    int(tr["data-href"].split("/")[-1])
+                    for tr in html.select("tr.message")
+                ]
+            )
 
         return PrivateMessageCollection.from_ids(client, message_ids)
 
 
 class PrivateMessageInbox(PrivateMessageCollection):
     @staticmethod
-    def from_ids(
-            client: 'Client',
-            message_ids: list[int]
-    ) -> 'PrivateMessageInbox':
+    def from_ids(client: "Client", message_ids: list[int]) -> "PrivateMessageInbox":
         """メッセージIDのリストから受信箱のメッセージオブジェクトのリストを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
         message_ids: list[int]
             メッセージIDのリスト
 
         Returns
         -------
         PrivateMessageInbox
             受信箱のメッセージオブジェクトのリスト
         """
-        return PrivateMessageInbox(PrivateMessageCollection.from_ids(client, message_ids))
+        return PrivateMessageInbox(
+            PrivateMessageCollection.from_ids(client, message_ids)
+        )
 
     @staticmethod
-    def acquire(client: 'Client'):
+    def acquire(client: "Client"):
         """受信箱のメッセージを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
 
         Returns
         -------
         PrivateMessageInbox
             受信箱のメッセージ
         """
         return PrivateMessageInbox(
-            PrivateMessageCollection._acquire(client, 'dashboard/messages/DMInboxModule'))
+            PrivateMessageCollection._acquire(
+                client, "dashboard/messages/DMInboxModule"
+            )
+        )
 
 
 class PrivateMessageSentBox(PrivateMessageCollection):
     @staticmethod
-    def from_ids(
-            client: 'Client',
-            message_ids: list[int]
-    ) -> 'PrivateMessageSentBox':
+    def from_ids(client: "Client", message_ids: list[int]) -> "PrivateMessageSentBox":
         """メッセージIDのリストから受信箱のメッセージオブジェクトのリストを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
         message_ids: list[int]
             メッセージIDのリスト
 
         Returns
         -------
         PrivateMessageSentBox
             受信箱のメッセージオブジェクトのリスト
         """
-        return PrivateMessageSentBox(PrivateMessageCollection.from_ids(client, message_ids))
+        return PrivateMessageSentBox(
+            PrivateMessageCollection.from_ids(client, message_ids)
+        )
 
     @staticmethod
-    def acquire(client: 'Client') -> 'PrivateMessageSentBox':
+    def acquire(client: "Client") -> "PrivateMessageSentBox":
         """送信箱のメッセージを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
 
         Returns
         -------
         PrivateMessageSentBox
             受信箱のメッセージ
         """
-        return PrivateMessageSentBox(PrivateMessageCollection._acquire(client, 'dashboard/messages/DMSentModule'))
+        return PrivateMessageSentBox(
+            PrivateMessageCollection._acquire(client, "dashboard/messages/DMSentModule")
+        )
 
 
 @dataclass
 class PrivateMessage:
     """プライベートメッセージオブジェクト
 
     Attributes
@@ -224,30 +240,28 @@
     subject: str
         件名
     body: str
         本文
     created_at: str
         作成日時
     """
-    client: 'Client'
+
+    client: "Client"
     id: int
-    sender: 'AbstractUser'
-    recipient: 'AbstractUser'
+    sender: "AbstractUser"
+    recipient: "AbstractUser"
     subject: str
     body: str
     created_at: datetime
 
     def __str__(self):
-        return f'PrivateMessage(id={self.id}, sender={self.sender}, recipient={self.recipient}, subject={self.subject})'
+        return f"PrivateMessage(id={self.id}, sender={self.sender}, recipient={self.recipient}, subject={self.subject})"
 
     @staticmethod
-    def from_id(
-            client: 'Client',
-            message_id: int
-    ) -> 'PrivateMessage':
+    def from_id(client: "Client", message_id: int) -> "PrivateMessage":
         """メッセージIDからメッセージオブジェクトを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
         message_id: int
@@ -258,34 +272,33 @@
         PrivateMessage
             メッセージオブジェクト
         """
         return PrivateMessageCollection.from_ids(client, [message_id])[0]
 
     @staticmethod
     @login_required
-    def send(
-            client: 'Client',
-            recipient: 'User',
-            subject: str,
-            body: str
-    ) -> None:
+    def send(client: "Client", recipient: "User", subject: str, body: str) -> None:
         """メッセージを送信する
 
         Parameters
         ----------
         client: Client
             クライアント
         recipient: User
             受信者
         subject: str
             件名
         body: str
             本文
         """
-        client.amc_client.request([{
-            'source': body,
-            'subject': subject,
-            'to_user_id': recipient.id,
-            'action': 'DashboardMessageAction',
-            'event': 'send',
-            'moduleName': 'Empty'
-        }])
+        client.amc_client.request(
+            [
+                {
+                    "source": body,
+                    "subject": subject,
+                    "to_user_id": recipient.id,
+                    "action": "DashboardMessageAction",
+                    "event": "send",
+                    "moduleName": "Empty",
+                }
+            ]
+        )
```

### Comparing `wikidot-3.0.3/wikidot/module/site.py` & `wikidot-3.0.4/src/wikidot/module/site.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Optional
 
 import httpx
 
 from wikidot.common import exceptions
 from wikidot.common.decorators import login_required
-from wikidot.module.page import SearchPagesQuery, PageCollection
+from wikidot.module.page import PageCollection, SearchPagesQuery
 from wikidot.module.site_application import SiteApplication
 
 if TYPE_CHECKING:
     from wikidot.module.client import Client
-    from wikidot.module.user import User
     from wikidot.module.page import Page
+    from wikidot.module.user import User
 
 
 class SitePagesMethods:
-    def __init__(self, site: 'Site'):
+    def __init__(self, site: "Site"):
         self.site = site
 
-    def search(
-            self,
-            **kwargs
-    ) -> 'PageCollection':
+    def search(self, **kwargs) -> "PageCollection":
         """ページを検索する
 
         Parameters
         ----------
         site: Site
             サイト
         query: SearchPagesQuery
@@ -39,22 +36,18 @@
         """
 
         query = SearchPagesQuery(**kwargs)
         return PageCollection.search_pages(self.site, query)
 
 
 class SitePageMethods:
-    def __init__(self, site: 'Site'):
+    def __init__(self, site: "Site"):
         self.site = site
 
-    def get(
-            self,
-            fullname: str,
-            raise_when_not_found: bool = True
-    ) -> Optional['Page']:
+    def get(self, fullname: str, raise_when_not_found: bool = True) -> Optional["Page"]:
         """フルネームからページを取得する
 
         Parameters
         ----------
         fullname: str
             ページのフルネーム
         raise_when_not_found: bool
@@ -62,20 +55,19 @@
 
         Returns
         -------
         Page
             ページオブジェクト
         """
         res = PageCollection.search_pages(
-            self.site,
-            SearchPagesQuery(fullname=fullname)
+            self.site, SearchPagesQuery(fullname=fullname)
         )
         if len(res) == 0:
             if raise_when_not_found:
-                raise exceptions.NotFoundException(f'Page is not found: {fullname}')
+                raise exceptions.NotFoundException(f"Page is not found: {fullname}")
             return None
         return res[0]
 
 
 @dataclass
 class Site:
     """サイトオブジェクト
@@ -96,34 +88,32 @@
     Raises
     ------
     NotFoundException
         サイトが存在しない場合
     UnexpectedException
         予期しないエラーが発生した場合
     """
-    client: 'Client'
+
+    client: "Client"
 
     id: int
     title: str
     unix_name: str
     domain: str
     ssl_supported: bool
 
     def __post_init__(self):
         self.pages = SitePagesMethods(self)
         self.page = SitePageMethods(self)
 
     def __str__(self):
-        return f'Site(id={self.id}, title={self.title}, unix_name={self.unix_name})'
+        return f"Site(id={self.id}, title={self.title}, unix_name={self.unix_name})"
 
     @staticmethod
-    def from_unix_name(
-            client: 'Client',
-            unix_name: str
-    ) -> 'Site':
+    def from_unix_name(client: "Client", unix_name: str) -> "Site":
         """UNIX名からサイトオブジェクトを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
         unix_name: str
@@ -133,88 +123,107 @@
         -------
         Site
             サイトオブジェクト
         """
         # サイト情報を取得
         # リダイレクトには従う
         response = httpx.get(
-            f'http://{unix_name}.wikidot.com',
+            f"http://{unix_name}.wikidot.com",
             follow_redirects=True,
-            timeout=client.amc_client.config.request_timeout
+            timeout=client.amc_client.config.request_timeout,
         )
 
         # サイトが存在しない場合
         if response.status_code == httpx.codes.NOT_FOUND:
-            raise exceptions.NotFoundException(f'Site is not found: {unix_name}.wikidot.com')
+            raise exceptions.NotFoundException(
+                f"Site is not found: {unix_name}.wikidot.com"
+            )
 
         # サイトが存在する場合
         source = response.text
 
         # id : WIKIREQUEST.info.siteId = xxxx;
-        id_match = re.search(r'WIKIREQUEST\.info\.siteId = (\d+);', source)
+        id_match = re.search(r"WIKIREQUEST\.info\.siteId = (\d+);", source)
         if id_match is None:
-            raise exceptions.UnexpectedException(f'Cannot find site id: {unix_name}.wikidot.com')
+            raise exceptions.UnexpectedException(
+                f"Cannot find site id: {unix_name}.wikidot.com"
+            )
         site_id = int(id_match.group(1))
 
         # title : titleタグ
-        title_match = re.search(r'<title>(.*?)</title>', source)
+        title_match = re.search(r"<title>(.*?)</title>", source)
         if title_match is None:
-            raise exceptions.UnexpectedException(f'Cannot find site title: {unix_name}.wikidot.com')
+            raise exceptions.UnexpectedException(
+                f"Cannot find site title: {unix_name}.wikidot.com"
+            )
         title = title_match.group(1)
 
         # unix_name : WIKIREQUEST.info.siteUnixName = "xxxx";
-        unix_name_match = re.search(r'WIKIREQUEST\.info\.siteUnixName = "(.*?)";', source)
+        unix_name_match = re.search(
+            r'WIKIREQUEST\.info\.siteUnixName = "(.*?)";', source
+        )
         if unix_name_match is None:
-            raise exceptions.UnexpectedException(f'Cannot find site unix_name: {unix_name}.wikidot.com')
+            raise exceptions.UnexpectedException(
+                f"Cannot find site unix_name: {unix_name}.wikidot.com"
+            )
         unix_name = unix_name_match.group(1)
 
         # domain :WIKIREQUEST.info.domain = "xxxx";
         domain_match = re.search(r'WIKIREQUEST\.info\.domain = "(.*?)";', source)
         if domain_match is None:
-            raise exceptions.UnexpectedException(f'Cannot find site domain: {unix_name}.wikidot.com')
+            raise exceptions.UnexpectedException(
+                f"Cannot find site domain: {unix_name}.wikidot.com"
+            )
         domain = domain_match.group(1)
 
         # SSL対応チェック
-        ssl_supported = str(response.url).startswith('https')
+        ssl_supported = str(response.url).startswith("https")
 
         return Site(
             client=client,
             id=site_id,
             title=title,
             unix_name=unix_name,
             domain=domain,
-            ssl_supported=ssl_supported
+            ssl_supported=ssl_supported,
         )
 
     def amc_request(self, bodies: list[dict], return_exceptions: bool = False):
         """このサイトに対してAMCリクエストを実行する"""
-        return self.client.amc_client.request(bodies, return_exceptions, self.unix_name, self.ssl_supported)
+        return self.client.amc_client.request(
+            bodies, return_exceptions, self.unix_name, self.ssl_supported
+        )
 
     def get_applications(self):
         """サイトへの未処理の参加申請を取得する"""
         return SiteApplication.acquire_all(self)
 
     @login_required
-    def invite_user(self, user: 'User', text: str):
-        """ユーザーをサイトに招待する
-        """
+    def invite_user(self, user: "User", text: str):
+        """ユーザーをサイトに招待する"""
         try:
-            self.amc_request([{
-                'action': 'ManageSiteMembershipAction',
-                'event': 'inviteMember',
-                'user_id': user.id,
-                'text': text,
-                'moduleName': 'Empty'
-            }])
+            self.amc_request(
+                [
+                    {
+                        "action": "ManageSiteMembershipAction",
+                        "event": "inviteMember",
+                        "user_id": user.id,
+                        "text": text,
+                        "moduleName": "Empty",
+                    }
+                ]
+            )
         except exceptions.WikidotStatusCodeException as e:
-            if e.status_code == 'already_invited':
+            if e.status_code == "already_invited":
                 raise exceptions.TargetErrorException(
-                    f'User is already invited to {self.unix_name}: {user.name}') from e
-            elif e.status_code == 'already_member':
+                    f"User is already invited to {self.unix_name}: {user.name}"
+                ) from e
+            elif e.status_code == "already_member":
                 raise exceptions.TargetErrorException(
-                    f'User is already a member of {self.unix_name}: {user.name}') from e
+                    f"User is already a member of {self.unix_name}: {user.name}"
+                ) from e
             else:
                 raise e
 
     def get_url(self):
         """サイトのURLを取得する"""
         return f'http{"s" if self.ssl_supported else ""}://{self.domain}'
```

### Comparing `wikidot-3.0.3/wikidot/module/site_application.py` & `wikidot-3.0.4/src/wikidot/module/site_application.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,99 +4,109 @@
 from bs4 import BeautifulSoup
 
 from wikidot.common import exceptions
 from wikidot.common.decorators import login_required
 from wikidot.util.parser import user as user_parser
 
 if TYPE_CHECKING:
-    from wikidot.module.user import AbstractUser
     from wikidot.module.site import Site
+    from wikidot.module.user import AbstractUser
 
 
 @dataclass
 class SiteApplication:
-    site: 'Site'
-    user: 'AbstractUser'
+    site: "Site"
+    user: "AbstractUser"
     text: str
 
     def __str__(self):
-        return f'SiteApplication(user={self.user}, site={self.site}, text={self.text})'
+        return f"SiteApplication(user={self.user}, site={self.site}, text={self.text})"
 
     @staticmethod
     @login_required
-    def acquire_all(site: 'Site') -> list['SiteApplication']:
+    def acquire_all(site: "Site") -> list["SiteApplication"]:
         """サイトへの未処理の申請を取得する
 
         Parameters
         ----------
         site: Site
             サイト
 
         Returns
         -------
         list[SiteApplication]
             申請のリスト
         """
-        response = site.amc_request([{
-            'moduleName': 'managesite/ManageSiteMembersApplicationsModule'
-        }])[0]
-
-        body = response.json()['body']
-
-        if 'WIKIDOT.page.listeners.loginClick(event)' in body:
-            raise exceptions.ForbiddenException('You are not allowed to access this page')
+        response = site.amc_request(
+            [{"moduleName": "managesite/ManageSiteMembersApplicationsModule"}]
+        )[0]
+
+        body = response.json()["body"]
+
+        if "WIKIDOT.page.listeners.loginClick(event)" in body:
+            raise exceptions.ForbiddenException(
+                "You are not allowed to access this page"
+            )
 
-        html = BeautifulSoup(response.json()['body'], 'lxml')
+        html = BeautifulSoup(response.json()["body"], "lxml")
 
         applications = []
 
-        user_elements = html.select('h3 span.printuser')
-        text_wrapper_elements = html.select('table')
+        user_elements = html.select("h3 span.printuser")
+        text_wrapper_elements = html.select("table")
 
         if len(user_elements) != len(text_wrapper_elements):
-            raise exceptions.UnexpectedException('Length of user_elements and text_wrapper_elements are different')
+            raise exceptions.UnexpectedException(
+                "Length of user_elements and text_wrapper_elements are different"
+            )
 
         for i in range(len(user_elements)):
             user_element = user_elements[i]
             text_wrapper_element = text_wrapper_elements[i]
 
             user = user_parser(site.client, user_element)
-            text = text_wrapper_element.select('td')[1].text.strip()
+            text = text_wrapper_element.select("td")[1].text.strip()
 
             applications.append(SiteApplication(site, user, text))
 
         return applications
 
     @login_required
     def _process(self, action: str):
         """申請を処理する
 
         Parameters
         ----------
         action: str
             処理の種類
         """
-        if action not in ['accept', 'decline']:
-            raise ValueError(f'Invalid action: {action}')
+        if action not in ["accept", "decline"]:
+            raise ValueError(f"Invalid action: {action}")
 
         try:
-            self.site.amc_request([{
-                'action': 'ManageSiteMembershipAction',
-                'event': f'acceptApplication',
-                'user_id': self.user.id,
-                'text': f'your application has been {action}ed',
-                'type': action,
-                'moduleName': 'Empty'
-            }])
+            self.site.amc_request(
+                [
+                    {
+                        "action": "ManageSiteMembershipAction",
+                        "event": "acceptApplication",
+                        "user_id": self.user.id,
+                        "text": f"your application has been {action}ed",
+                        "type": action,
+                        "moduleName": "Empty",
+                    }
+                ]
+            )
         except exceptions.WikidotStatusCodeException as e:
-            if e.status_code == 'no_application':
-                raise exceptions.NotFoundException(f'Application not found: {self.user}') from e
+            if e.status_code == "no_application":
+                raise exceptions.NotFoundException(
+                    f"Application not found: {self.user}"
+                ) from e
             else:
                 raise e
 
     def accept(self):
         """申請を承認する"""
-        self._process('accept')
+        self._process("accept")
 
     def decline(self):
         """申請を拒否する"""
-        self._process('decline')
+        self._process("decline")
```

### Comparing `wikidot-3.0.3/wikidot/module/user.py` & `wikidot-3.0.4/src/wikidot/module/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,24 @@
 from wikidot.util.requestutil import RequestUtil
 from wikidot.util.stringutil import StringUtil
 
 if TYPE_CHECKING:
     from wikidot.module.client import Client
 
 
-class UserCollection(list['AbstractUser']):
+class UserCollection(list["AbstractUser"]):
     """ユーザーオブジェクトのリスト"""
 
-    def __iter__(self) -> Iterator['AbstractUser']:
+    def __iter__(self) -> Iterator["AbstractUser"]:
         return super().__iter__()
 
     @staticmethod
     def from_names(
-            client: 'Client',
-            names: list[str],
-            raise_when_not_found: bool = False
-    ) -> 'UserCollection':
+            client: "Client", names: list[str], raise_when_not_found: bool = False
+    ) -> "UserCollection":
         """ユーザー名のリストからユーザーオブジェクトのリストを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
         names: list[str]
@@ -39,50 +37,56 @@
         Returns
         -------
         UserCollection
             ユーザーオブジェクトのリスト
         """
         responses = RequestUtil.request(
             client,
-            'GET',
-            [f'https://www.wikidot.com/user:info/{StringUtil.to_unix(name)}' for name in names]
+            "GET",
+            [
+                f"https://www.wikidot.com/user:info/{StringUtil.to_unix(name)}"
+                for name in names
+            ],
         )
 
-        users = []
+        users: list[AbstractUser] = []
 
         for response in responses:
             if isinstance(response, Exception):
                 raise response
 
-            html = BeautifulSoup(response.text, 'lxml')
+            html = BeautifulSoup(response.text, "lxml")
 
             # 存在チェック
-            if html.select_one('div.error-block'):
+            if html.select_one("div.error-block"):
                 if raise_when_not_found:
-                    raise NotFoundException(f'User not found: {response.url}')
+                    raise NotFoundException(f"User not found: {response.url}")
                 else:
-                    users.append(None)
                     continue
 
             # id取得
-            user_id = int(html.select_one('a.btn.btn-default.btn-xs')['href'].split('/')[-1])
+            user_id = int(
+                html.select_one("a.btn.btn-default.btn-xs")["href"].split("/")[-1]
+            )
 
             # name取得
-            name = html.select_one('h1.profile-title').get_text(strip=True)
+            name = html.select_one("h1.profile-title").get_text(strip=True)
 
             # avatar_url取得
-            avatar_url = f'https://www.wikidot.com/avatar.php?userid={user_id}'
+            avatar_url = f"https://www.wikidot.com/avatar.php?userid={user_id}"
 
-            users.append(User(
-                client=client,
-                id=user_id,
-                name=name,
-                unix_name=StringUtil.to_unix(name),
-                avatar_url=avatar_url
-            ))
+            users.append(
+                User(
+                    client=client,
+                    id=user_id,
+                    name=name,
+                    unix_name=StringUtil.to_unix(name),
+                    avatar_url=avatar_url,
+                )
+            )
 
         return UserCollection(users)
 
 
 @dataclass
 class AbstractUser:
     """ユーザーオブジェクトの抽象クラス
@@ -98,23 +102,24 @@
     unix_name: str | None
         ユーザーのUNIX名
     avatar_url: str | None
         ユーザーアバターのURL
     ip: str | None
         ユーザーのIPアドレス
     """
-    client: 'Client'
+
+    client: "Client"
     id: int | None = None
     name: str | None = None
     unix_name: str | None = None
     avatar_url: str | None = None
     ip: str | None = None
 
     def __str__(self):
-        return f'{self.__class__.__name__}(id={self.id}, name={self.name}, unix_name={self.unix_name})'
+        return f"{self.__class__.__name__}(id={self.id}, name={self.name}, unix_name={self.unix_name})"
 
 
 @dataclass
 class User(AbstractUser):
     """一般のユーザーオブジェクト
 
     Attributes
@@ -128,27 +133,26 @@
     unix_name: str | None
         ユーザーのUNIX名
     avatar_url: str | None
         ユーザーアバターのURL
     ip: None
         ユーザーのIPアドレス（取得できないためNone）
     """
+
     # client: 'Client'
     # id: int | None
     # name: str | None
     # unix_name: str | None
     # avatar_url: str | None
     ip: None = None
 
     @staticmethod
     def from_name(
-            client: 'Client',
-            name: str,
-            raise_when_not_found: bool = False
-    ) -> 'User':
+            client: "Client", name: str, raise_when_not_found: bool = False
+    ) -> "User":
         """ユーザー名からユーザーオブジェクトを取得する
 
         Parameters
         ----------
         client: Client
             クライアント
         name: str
@@ -180,14 +184,15 @@
     unix_name: str
         ユーザーのUNIX名（削除されたため"account_deleted"）
     avatar_url: None
         ユーザーアバターのURL（削除されたためNone）
     ip: None
         ユーザーのIPアドレス（取得できないためNone）
     """
+
     # client: 'Client'
     # id: int | None
     name: str = "account deleted"
     unix_name: str = "account_deleted"
     avatar_url: None = None
     ip: None = None
 
@@ -207,14 +212,15 @@
     unix_name: str
         ユーザーのUNIX名（匿名ユーザーのため"anonymous"）
     avatar_url: None
         ユーザーアバターのURL（匿名ユーザーのためNone）
     ip: str
         ユーザーのIPアドレス
     """
+
     # client: 'Client'
     id: None = None
     name: str = "Anonymous"
     unix_name: str = "anonymous"
     avatar_url: None = None
     # ip: None = None
 
@@ -234,14 +240,15 @@
     unix_name: None
         ユーザーのUNIX名（ゲストユーザーのためNone）
     avatar_url: None
         ユーザーアバターのURL（ゲストユーザーのためNone）
     ip: None
         ユーザーのIPアドレス（取得できないためNone）
     """
+
     # client: 'Client'
     id: None = None
     # name: str | None
     unix_name: None = None
     avatar_url: None = None
     ip: None = None
 
@@ -261,13 +268,14 @@
     unix_name: str
         ユーザーのUNIX名（Wikidotシステムユーザーのため"wikidot"）
     avatar_url: None
         ユーザーアバターのURL（WikidotシステムユーザーのためNone）
     ip: None
         ユーザーのIPアドレス（取得できないためNone）
     """
+
     # client: 'Client'
     id: None = None
     name: str = "Wikidot"
     unix_name: str = "wikidot"
     avatar_url: None = None
     ip: None = None
```

### Comparing `wikidot-3.0.3/wikidot/util/parser/odate.py` & `wikidot-3.0.4/src/wikidot/util/parser/odate.py`

 * *Files identical despite different names*

### Comparing `wikidot-3.0.3/wikidot/util/parser/user.py` & `wikidot-3.0.4/src/wikidot/util/parser/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from wikidot.module import user
 
 if TYPE_CHECKING:
     from wikidot.module.client import Client
 
 
-def user_parse(client: 'Client', elem: bs4.Tag) -> user.AbstractUser:
-    """ printuser要素をパースし、ユーザーオブジェクトを返す
+def user_parse(client: "Client", elem: bs4.Tag) -> user.AbstractUser:
+    """printuser要素をパースし、ユーザーオブジェクトを返す
 
     Parameters
     ----------
     elem: bs4.Tag
         パース対象の要素（printuserクラスがついた要素）
     client: Client
         クライアント
@@ -22,25 +22,25 @@
     -------
     user.AbstractUser
         パースされて得られたユーザーオブジェクト
         User | DeletedUser | AnonymousUser | GuestUser | WikidotUser のいずれか
     """
 
     if "class" in elem.attrs and "deleted" in elem["class"]:
-        return user.DeletedUser(
-            client=client,
-            id=int(elem["data-id"])
-        )
+        return user.DeletedUser(client=client, id=int(elem["data-id"]))
 
     elif "class" in elem.attrs and "anonymous" in elem["class"]:
-        ip = elem.find("span", class_="ip").get_text().replace("(", "").replace(")", "").strip()
-        return user.AnonymousUser(
-            client=client,
-            ip=ip
+        ip = (
+            elem.find("span", class_="ip")
+            .get_text()
+            .replace("(", "")
+            .replace(")", "")
+            .strip()
         )
+        return user.AnonymousUser(client=client, ip=ip)
 
     # TODO: [[user ukwhatn]]構文をパースできなくなる（aが1つしかない）ので、一度無効化 -> GuestUserの例を探して実装を戻す
     # elif len(elem.find_all("a", recursive=False)) == 1:
     #     return user.GuestUser(
     #         name=elem.get_text().strip()
     #     )
 
@@ -48,17 +48,19 @@
         return user.WikidotUser(client=client)
 
     else:
         _user = elem.find_all("a")[-1]
         user_name = _user.get_text()
         user_unix = str(_user["href"]).replace("http://www.wikidot.com/user:info/", "")
         user_id = int(
-            str(_user["onclick"]).replace("WIKIDOT.page.listeners.userInfo(", "").replace("); return false;", "")
+            str(_user["onclick"])
+            .replace("WIKIDOT.page.listeners.userInfo(", "")
+            .replace("); return false;", "")
         )
 
         return user.User(
             client=client,
             id=user_id,
             name=user_name,
             unix_name=user_unix,
-            avatar_url=f"http://www.wikidot.com/avatar.php?userid={user_id}"
+            avatar_url=f"http://www.wikidot.com/avatar.php?userid={user_id}",
         )
```

### Comparing `wikidot-3.0.3/wikidot/util/quick_module.py` & `wikidot-3.0.4/src/wikidot/util/quick_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     title: str
     unix_name: str
 
 
 class QuickModule:
     @staticmethod
     def _request(
-            module_name: str,
-            site_id: int,
-            query: str,
+        module_name: str,
+        site_id: int,
+        query: str,
     ):
         """リクエストを送信する
 
         Parameters
         ----------
         module_name: str
             モジュール名
@@ -37,25 +37,22 @@
         if module_name not in [
             "MemberLookupQModule",
             "UserLookupQModule",
             "PageLookupQModule",
         ]:
             raise ValueError("Invalid module name")
 
-        url = f'https://www.wikidot.com/quickmodule.php?module={module_name}&s={site_id}&q={query}'
+        url = f"https://www.wikidot.com/quickmodule.php?module={module_name}&s={site_id}&q={query}"
         response = httpx.get(url, timeout=300)
         if response.status_code == httpx.codes.INTERNAL_SERVER_ERROR:
             raise ValueError("Site is not found")
         return response.json()
 
     @staticmethod
-    def member_lookup(
-            site_id: int,
-            query: str
-    ):
+    def member_lookup(site_id: int, query: str):
         """メンバーを検索する
 
         Parameters
         ----------
         site_id: int
             サイトID
         query: str
@@ -63,21 +60,18 @@
 
         Returns
         -------
         list[QMCUser]
             ユーザーのリスト
         """
         users = QuickModule._request("MemberLookupQModule", site_id, query)["users"]
-        return [QMCUser(id=user["user_id"], name=user["name"]) for user in users]
+        return [QMCUser(id=int(user["user_id"]), name=user["name"]) for user in users]
 
     @staticmethod
-    def user_lookup(
-            site_id: int,
-            query: str
-    ):
+    def user_lookup(site_id: int, query: str):
         """ユーザーを検索する
 
         Parameters
         ----------
         site_id: int
             サイトID
         query: str
@@ -85,21 +79,18 @@
 
         Returns
         -------
         list[QMCUser]
             ユーザーのリスト
         """
         users = QuickModule._request("UserLookupQModule", site_id, query)["users"]
-        return [QMCUser(id=user["user_id"], name=user["name"]) for user in users]
+        return [QMCUser(id=int(user["user_id"]), name=user["name"]) for user in users]
 
     @staticmethod
-    def page_lookup(
-            site_id: int,
-            query: str
-    ):
+    def page_lookup(site_id: int, query: str):
         """ページを検索する
 
         Parameters
         ----------
         site_id: int
             サイトID
         query: str
@@ -107,8 +98,10 @@
 
         Returns
         -------
         list[QMCPage]
             ページのリスト
         """
         pages = QuickModule._request("PageLookupQModule", site_id, query)["pages"]
-        return [QMCPage(title=page["title"], unix_name=page["unix_name"]) for page in pages]
+        return [
+            QMCPage(title=page["title"], unix_name=page["unix_name"]) for page in pages
+        ]
```

### Comparing `wikidot-3.0.3/wikidot/util/requestutil.py` & `wikidot-3.0.4/src/wikidot/util/requestutil.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 if TYPE_CHECKING:
     from wikidot.module.client import Client
 
 
 class RequestUtil:
     @staticmethod
     def request(
-            client: 'Client',
-            method: str,
-            urls: list[str],
-            return_exceptions: bool = False
+        client: "Client", method: str, urls: list[str], return_exceptions: bool = False
     ) -> list[httpx.Response | Exception]:
         """GETリクエストを送信する
 
         Parameters
         ----------
         client: Client
             クライアント
@@ -33,30 +30,30 @@
         -------
         list[httpx.Response | Exception]
             レスポンスのリスト
         """
         config = client.amc_client.config
         semaphore = asyncio.Semaphore(config.semaphore_limit)
 
-        async def _get(
-                url: str
-        ) -> httpx.Response:
+        async def _get(url: str) -> httpx.Response:
             async with semaphore:
                 async with httpx.AsyncClient() as _client:
                     return await _client.get(url)
 
-        async def _post(
-                url: str
-        ) -> httpx.Response:
+        async def _post(url: str) -> httpx.Response:
             async with semaphore:
                 async with httpx.AsyncClient() as _client:
                     return await _client.post(url)
 
         async def _execute():
-            if method == 'GET':
-                return await asyncio.gather(*[_get(url) for url in urls], return_exceptions=return_exceptions)
-            elif method == 'POST':
-                return await asyncio.gather(*[_post(url) for url in urls], return_exceptions=return_exceptions)
+            if method == "GET":
+                return await asyncio.gather(
+                    *[_get(url) for url in urls], return_exceptions=return_exceptions
+                )
+            elif method == "POST":
+                return await asyncio.gather(
+                    *[_post(url) for url in urls], return_exceptions=return_exceptions
+                )
             else:
-                raise ValueError('Invalid method')
+                raise ValueError("Invalid method")
 
         return asyncio.run(_execute())
```

### Comparing `wikidot-3.0.3/wikidot/util/stringutil.py` & `wikidot-3.0.4/src/wikidot/util/stringutil.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,24 +25,24 @@
         # 変換実施
         target_str = target_str.translate(table)
 
         # lowercaseへの変換
         target_str = target_str.lower()
 
         # ascii以外の文字を削除
-        target_str = re.sub(r'[^a-z0-9\-:_]', '-', target_str)
-        target_str = re.sub(r'^_', ':_', target_str)
-        target_str = re.sub(r'(?<!:)_', '-', target_str)
-        target_str = re.sub(r'^-*', '', target_str)
-        target_str = re.sub(r'-*$', '', target_str)
-        target_str = re.sub(r'-{2,}', '-', target_str)
-        target_str = re.sub(r':{2,}', ':', target_str)
-        target_str = target_str.replace(':-', ':')
-        target_str = target_str.replace('-:', ':')
-        target_str = target_str.replace('_-', '_')
-        target_str = target_str.replace('-_', '_')
+        target_str = re.sub(r"[^a-z0-9\-:_]", "-", target_str)
+        target_str = re.sub(r"^_", ":_", target_str)
+        target_str = re.sub(r"(?<!:)_", "-", target_str)
+        target_str = re.sub(r"^-*", "", target_str)
+        target_str = re.sub(r"-*$", "", target_str)
+        target_str = re.sub(r"-{2,}", "-", target_str)
+        target_str = re.sub(r":{2,}", ":", target_str)
+        target_str = target_str.replace(":-", ":")
+        target_str = target_str.replace("-:", ":")
+        target_str = target_str.replace("_-", "_")
+        target_str = target_str.replace("-_", "_")
 
         # 先頭と末尾の:を削除
-        target_str = re.sub(r'^:', '', target_str)
-        target_str = re.sub(r':$', '', target_str)
+        target_str = re.sub(r"^:", "", target_str)
+        target_str = re.sub(r":$", "", target_str)
 
         return target_str
```

### Comparing `wikidot-3.0.3/wikidot/util/table/char_table.py` & `wikidot-3.0.4/src/wikidot/util/table/char_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,9 +461,9 @@
     "Ԋ": "n",
     "ԋ": "n",
     "Ԏ": "t",
     "ԏ": "t",
     "Ԛ": "q",
     "ԛ": "q",
     "Ԝ": "w",
-    "ԝ": "w"
+    "ԝ": "w",
 }
```

### Comparing `wikidot-3.0.3/wikidot.egg-info/PKG-INFO` & `wikidot-3.0.4/src/wikidot.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: wikidot
-Version: 3.0.3
+Version: 3.0.4
 Summary: Wikidot Utility Library
 Author-email: ukwhatn <ukwhatn@gmail.com>
 Project-URL: Homepage, https://github.com/ukwhatn/wikidot.py
 Project-URL: Bug Tracker, https://github.com/ukwhatn/wikidot.py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx~=0.25.0
+Requires-Dist: httpx<0.28,>=0.25
 Requires-Dist: beautifulsoup4~=4.12.2
-Requires-Dist: lxml~=4.9.3
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
+Requires-Dist: lxml<5.3.0,>=4.9.3
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Requires-Dist: twine; extra == "build"
+Provides-Extra: lint
+Requires-Dist: flake8; extra == "lint"
+Requires-Dist: mypy; extra == "lint"
+Requires-Dist: isort; extra == "lint"
+Provides-Extra: format
+Requires-Dist: black; extra == "format"
+Requires-Dist: isort; extra == "format"
 
 # wikidot.py - A Python library for making requests to the Wikidot sites.
 
 ## Installation
 ```bash
 pip install wikidot
 ```
```

### Comparing `wikidot-3.0.3/wikidot.egg-info/SOURCES.txt` & `wikidot-3.0.4/src/wikidot.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
-wikidot/__init__.py
-wikidot.egg-info/PKG-INFO
-wikidot.egg-info/SOURCES.txt
-wikidot.egg-info/dependency_links.txt
-wikidot.egg-info/requires.txt
-wikidot.egg-info/top_level.txt
-wikidot/common/__init__.py
-wikidot/common/decorators.py
-wikidot/common/exceptions.py
-wikidot/common/logger.py
-wikidot/connector/__init__.py
-wikidot/connector/ajax.py
-wikidot/connector/api.py
-wikidot/module/__init__.py
-wikidot/module/auth.py
-wikidot/module/client.py
-wikidot/module/page.py
-wikidot/module/page_revision.py
-wikidot/module/page_source.py
-wikidot/module/page_votes.py
-wikidot/module/private_message.py
-wikidot/module/site.py
-wikidot/module/site_application.py
-wikidot/module/user.py
-wikidot/util/__init__.py
-wikidot/util/quick_module.py
-wikidot/util/requestutil.py
-wikidot/util/stringutil.py
-wikidot/util/parser/__init__.py
-wikidot/util/parser/odate.py
-wikidot/util/parser/user.py
-wikidot/util/table/__init__.py
-wikidot/util/table/char_table.py
+src/wikidot/__init__.py
+src/wikidot.egg-info/PKG-INFO
+src/wikidot.egg-info/SOURCES.txt
+src/wikidot.egg-info/dependency_links.txt
+src/wikidot.egg-info/requires.txt
+src/wikidot.egg-info/top_level.txt
+src/wikidot/common/__init__.py
+src/wikidot/common/decorators.py
+src/wikidot/common/exceptions.py
+src/wikidot/common/logger.py
+src/wikidot/connector/__init__.py
+src/wikidot/connector/ajax.py
+src/wikidot/connector/api.py
+src/wikidot/module/__init__.py
+src/wikidot/module/auth.py
+src/wikidot/module/client.py
+src/wikidot/module/page.py
+src/wikidot/module/page_revision.py
+src/wikidot/module/page_source.py
+src/wikidot/module/page_votes.py
+src/wikidot/module/private_message.py
+src/wikidot/module/site.py
+src/wikidot/module/site_application.py
+src/wikidot/module/user.py
+src/wikidot/util/__init__.py
+src/wikidot/util/quick_module.py
+src/wikidot/util/requestutil.py
+src/wikidot/util/stringutil.py
+src/wikidot/util/parser/__init__.py
+src/wikidot/util/parser/odate.py
+src/wikidot/util/parser/user.py
+src/wikidot/util/table/__init__.py
+src/wikidot/util/table/char_table.py
```

