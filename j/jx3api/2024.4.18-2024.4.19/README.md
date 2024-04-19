# Comparing `tmp/jx3api-2024.4.18.tar.gz` & `tmp/jx3api-2024.4.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jx3api-2024.4.18.tar", last modified: Wed Apr 17 16:42:05 2024, max compression
+gzip compressed data, was "jx3api-2024.4.19.tar", last modified: Fri Apr 19 07:51:19 2024, max compression
```

## Comparing `jx3api-2024.4.18.tar` & `jx3api-2024.4.19.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:42:05.124254 jx3api-2024.4.18/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-17 16:42:05.124254 jx3api-2024.4.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-17 16:41:58.000000 jx3api-2024.4.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:42:05.124254 jx3api-2024.4.18/jx3api/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 16:41:58.000000 jx3api-2024.4.18/jx3api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-17 16:41:58.000000 jx3api-2024.4.18/jx3api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    75007 2024-04-17 16:41:58.000000 jx3api-2024.4.18/jx3api/jx3api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:42:05.124254 jx3api-2024.4.18/jx3api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-17 16:42:05.000000 jx3api-2024.4.18/jx3api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-17 16:42:05.000000 jx3api-2024.4.18/jx3api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:42:05.000000 jx3api-2024.4.18/jx3api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 16:42:05.000000 jx3api-2024.4.18/jx3api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 16:42:05.000000 jx3api-2024.4.18/jx3api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:42:05.124254 jx3api-2024.4.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-17 16:41:58.000000 jx3api-2024.4.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:19.534470 jx3api-2024.4.19/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-19 07:51:19.534470 jx3api-2024.4.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-19 07:51:16.000000 jx3api-2024.4.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:19.534470 jx3api-2024.4.19/jx3api/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 07:51:16.000000 jx3api-2024.4.19/jx3api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-19 07:51:16.000000 jx3api-2024.4.19/jx3api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75007 2024-04-19 07:51:16.000000 jx3api-2024.4.19/jx3api/jx3api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:51:19.534470 jx3api-2024.4.19/jx3api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-19 07:51:19.000000 jx3api-2024.4.19/jx3api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-19 07:51:19.000000 jx3api-2024.4.19/jx3api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:51:19.000000 jx3api-2024.4.19/jx3api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 07:51:19.000000 jx3api-2024.4.19/jx3api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 07:51:19.000000 jx3api-2024.4.19/jx3api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:51:19.534470 jx3api-2024.4.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 07:51:16.000000 jx3api-2024.4.19/setup.py
```

### Comparing `jx3api-2024.4.18/PKG-INFO` & `jx3api-2024.4.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx3api
-Version: 2024.4.18
+Version: 2024.4.19
 Summary: The Python SDK to the JX3API
 Home-page: https://www.jx3api.com
 Author: JX3API
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
```

### Comparing `jx3api-2024.4.18/README.md` & `jx3api-2024.4.19/README.md`

 * *Files identical despite different names*

### Comparing `jx3api-2024.4.18/jx3api/jx3api.py` & `jx3api-2024.4.19/jx3api/jx3api.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     def request(self: Self, *, endpoint: str, **kwargs) -> Any:
         logging.debug(f"requesting: {endpoint=}, {kwargs=}")
 
         kwargs["ticket"] = self.ticket
 
         req = Request(
-            urljoin(base="https://www.jx3api.com", url=endpoint),
+            urljoin(base="https://api.jx3api.com", url=endpoint),
             data=json.dumps(kwargs).encode(encoding="utf-8"),
             headers={"token": self.token} if self.token else {},
         )
 
         with closing(urlopen(req)) as resp:
             if (data := json.loads(resp.read()))["code"] != HTTPStatus.OK:
                 raise APIError(code=data["code"], msg=data["msg"])
@@ -1166,15 +1166,15 @@
     async def request(self: Self, *, endpoint: str, **kwargs) -> Any:
         logging.debug(f"requesting: {endpoint=}, {kwargs=}")
 
         kwargs["ticket"] = self.ticket
 
         async with aiohttp.request(
             "GET",
-            urljoin(base="https://www.jx3api.com", url=endpoint),
+            urljoin(base="https://api.jx3api.com", url=endpoint),
             data=json.dumps(kwargs).encode(encoding="utf-8"),
             headers={"token": self.token} if self.token else None,
         ) as resp:
             if (data := await resp.json(loads=json.loads))["code"] != HTTPStatus.OK:
                 raise APIError(code=data["code"], msg=data["msg"])
 
         return data["data"]
```

### Comparing `jx3api-2024.4.18/jx3api.egg-info/PKG-INFO` & `jx3api-2024.4.19/jx3api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jx3api
-Version: 2024.4.18
+Version: 2024.4.19
 Summary: The Python SDK to the JX3API
 Home-page: https://www.jx3api.com
 Author: JX3API
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
```

### Comparing `jx3api-2024.4.18/setup.py` & `jx3api-2024.4.19/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r+") as f:
     readme = f.read()
 
 setup(
     name="jx3api",
-    version="2024.04.18",
+    version="2024.04.19",
     description="The Python SDK to the JX3API",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="JX3API",
     url="https://www.jx3api.com",
     packages=find_packages(),
     classifiers=[
```

