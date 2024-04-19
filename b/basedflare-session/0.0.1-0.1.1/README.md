# Comparing `tmp/basedflare-session-0.0.1.tar.gz` & `tmp/basedflare_session-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basedflare-session-0.0.1.tar", last modified: Wed Apr 10 23:30:48 2024, max compression
+gzip compressed data, was "basedflare_session-0.1.1.tar", last modified: Fri Apr 19 18:35:00 2024, max compression
```

## Comparing `basedflare-session-0.0.1.tar` & `basedflare_session-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rmseq     (1000) rmseq     (1000)        0 2024-04-10 23:30:48.575788 basedflare-session-0.0.1/
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)    34523 2024-04-10 18:49:43.000000 basedflare-session-0.0.1/LICENSE
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)    41386 2024-04-10 23:30:48.575788 basedflare-session-0.0.1/PKG-INFO
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)      845 2024-04-10 22:23:06.000000 basedflare-session-0.0.1/README.md
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)      828 2024-04-10 23:30:37.000000 basedflare-session-0.0.1/pyproject.toml
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)       38 2024-04-10 23:30:48.575788 basedflare-session-0.0.1/setup.cfg
-drwxr-xr-x   0 rmseq     (1000) rmseq     (1000)        0 2024-04-10 23:30:48.572788 basedflare-session-0.0.1/src/
-drwxr-xr-x   0 rmseq     (1000) rmseq     (1000)        0 2024-04-10 23:30:48.573788 basedflare-session-0.0.1/src/basedflare_session/
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)       34 2024-04-10 21:50:33.000000 basedflare-session-0.0.1/src/basedflare_session/__init__.py
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)      233 2024-04-10 00:20:06.000000 basedflare-session-0.0.1/src/basedflare_session/exceptions.py
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)     2359 2024-04-10 18:42:51.000000 basedflare-session-0.0.1/src/basedflare_session/session.py
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)      576 2024-04-10 01:18:05.000000 basedflare-session-0.0.1/src/basedflare_session/utils.py
-drwxr-xr-x   0 rmseq     (1000) rmseq     (1000)        0 2024-04-10 23:30:48.574788 basedflare-session-0.0.1/src/basedflare_session.egg-info/
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)    41386 2024-04-10 23:30:48.000000 basedflare-session-0.0.1/src/basedflare_session.egg-info/PKG-INFO
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)      399 2024-04-10 23:30:48.000000 basedflare-session-0.0.1/src/basedflare_session.egg-info/SOURCES.txt
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)        1 2024-04-10 23:30:48.000000 basedflare-session-0.0.1/src/basedflare_session.egg-info/dependency_links.txt
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)       37 2024-04-10 23:30:48.000000 basedflare-session-0.0.1/src/basedflare_session.egg-info/requires.txt
--rw-r--r--   0 rmseq     (1000) rmseq     (1000)       19 2024-04-10 23:30:48.000000 basedflare-session-0.0.1/src/basedflare_session.egg-info/top_level.txt
+drwxr-xr-x   0 rmseq     (1000) rmseq     (1000)        0 2024-04-19 18:35:00.937494 basedflare_session-0.1.1/
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)    34523 2024-04-10 18:49:43.000000 basedflare_session-0.1.1/LICENSE
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)    41558 2024-04-19 18:35:00.936494 basedflare_session-0.1.1/PKG-INFO
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)      935 2024-04-19 18:19:25.000000 basedflare_session-0.1.1/README.md
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)      910 2024-04-19 18:32:40.000000 basedflare_session-0.1.1/pyproject.toml
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)       38 2024-04-19 18:35:00.937494 basedflare_session-0.1.1/setup.cfg
+drwxr-xr-x   0 rmseq     (1000) rmseq     (1000)        0 2024-04-19 18:35:00.933494 basedflare_session-0.1.1/src/
+drwxr-xr-x   0 rmseq     (1000) rmseq     (1000)        0 2024-04-19 18:35:00.935494 basedflare_session-0.1.1/src/basedflare_session/
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)      332 2024-04-12 20:46:48.000000 basedflare_session-0.1.1/src/basedflare_session/__init__.py
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)      233 2024-04-10 00:20:06.000000 basedflare_session-0.1.1/src/basedflare_session/exceptions.py
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)     3047 2024-04-12 20:47:38.000000 basedflare_session-0.1.1/src/basedflare_session/session.py
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)      902 2024-04-12 20:21:05.000000 basedflare_session-0.1.1/src/basedflare_session/utils.py
+drwxr-xr-x   0 rmseq     (1000) rmseq     (1000)        0 2024-04-19 18:35:00.936494 basedflare_session-0.1.1/src/basedflare_session.egg-info/
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)    41558 2024-04-19 18:35:00.000000 basedflare_session-0.1.1/src/basedflare_session.egg-info/PKG-INFO
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)      399 2024-04-19 18:35:00.000000 basedflare_session-0.1.1/src/basedflare_session.egg-info/SOURCES.txt
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)        1 2024-04-19 18:35:00.000000 basedflare_session-0.1.1/src/basedflare_session.egg-info/dependency_links.txt
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)       37 2024-04-19 18:35:00.000000 basedflare_session-0.1.1/src/basedflare_session.egg-info/requires.txt
+-rw-r--r--   0 rmseq     (1000) rmseq     (1000)       19 2024-04-19 18:35:00.000000 basedflare_session-0.1.1/src/basedflare_session.egg-info/top_level.txt
```

### Comparing `basedflare-session-0.0.1/LICENSE` & `basedflare_session-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `basedflare-session-0.0.1/PKG-INFO` & `basedflare_session-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: basedflare-session
-Version: 0.0.1
-Summary: Extends the requests-flavored session to solve BasedFlare challenges.
+Version: 0.1.1
+Summary: Provides a requests-flavored session to solve BasedFlare challenges automatically. It also includes utility functions to solve the challenges manually.
 Author-email: loynet <loynet@protonmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -676,21 +676,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: argon2-cffi>=23.1.0
 
 # basedflare-session
 
-A package that
-extends [Python's requests session](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) to solve
-some [BasedFlare](https://basedflare.com/) Proof of Work (PoW) challenges.
-
+A package that extends [Python's requests session](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) to solve some [BasedFlare](https://basedflare.com/) Proof of Work (PoW) challenges automatically.
+It also includes utility functions to solve the challenges manually.
 
 Please note that **this package is a work in progress** and may not function in all cases.
-Currently, it only supports the `argon2` PoW challenge. 
+Currently, it supports the `argon2` and `sha256` PoW challenges.
 Any other challenge, such as a CAPTCHA, will raise an exception.
 
 ## Usage
 
 Suppose `example.com` is a website that requires you to solve a challenge before you can access it. Below is a simple
 example of how to use the package:
```

### Comparing `basedflare-session-0.0.1/pyproject.toml` & `basedflare_session-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=69.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "basedflare-session"
-version = "0.0.1"
+version = "0.1.1"
 dependencies = [
     "requests>=2.31.0",
     "argon2-cffi>=23.1.0",
 ]
 requires-python = ">=3.8"
 authors = [
     { name = "loynet", email = "loynet@protonmail.com" },
 ]
-description = "Extends the requests-flavored session to solve BasedFlare challenges."
+description = "Provides a requests-flavored session to solve BasedFlare challenges automatically. It also includes utility functions to solve the challenges manually."
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["basedflare", "session"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
```

### Comparing `basedflare-session-0.0.1/src/basedflare_session.egg-info/PKG-INFO` & `basedflare_session-0.1.1/src/basedflare_session.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: basedflare-session
-Version: 0.0.1
-Summary: Extends the requests-flavored session to solve BasedFlare challenges.
+Version: 0.1.1
+Summary: Provides a requests-flavored session to solve BasedFlare challenges automatically. It also includes utility functions to solve the challenges manually.
 Author-email: loynet <loynet@protonmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -676,21 +676,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: argon2-cffi>=23.1.0
 
 # basedflare-session
 
-A package that
-extends [Python's requests session](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) to solve
-some [BasedFlare](https://basedflare.com/) Proof of Work (PoW) challenges.
-
+A package that extends [Python's requests session](https://docs.python-requests.org/en/latest/_modules/requests/sessions/) to solve some [BasedFlare](https://basedflare.com/) Proof of Work (PoW) challenges automatically.
+It also includes utility functions to solve the challenges manually.
 
 Please note that **this package is a work in progress** and may not function in all cases.
-Currently, it only supports the `argon2` PoW challenge. 
+Currently, it supports the `argon2` and `sha256` PoW challenges.
 Any other challenge, such as a CAPTCHA, will raise an exception.
 
 ## Usage
 
 Suppose `example.com` is a website that requires you to solve a challenge before you can access it. Below is a simple
 example of how to use the package:
```

