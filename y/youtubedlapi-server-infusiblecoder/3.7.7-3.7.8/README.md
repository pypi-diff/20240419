# Comparing `tmp/youtubedlapi_server_infusiblecoder-3.7.7.tar.gz` & `tmp/youtubedlapi_server_infusiblecoder-3.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubedlapi_server_infusiblecoder-3.7.7.tar", last modified: Fri Mar 15 11:28:31 2024, max compression
+gzip compressed data, was "youtubedlapi_server_infusiblecoder-3.7.8.tar", last modified: Fri Apr 19 15:56:08 2024, max compression
```

## Comparing `youtubedlapi_server_infusiblecoder-3.7.7.tar` & `youtubedlapi_server_infusiblecoder-3.7.8.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 11:28:31.678295 youtubedlapi_server_infusiblecoder-3.7.7/
--rw-rw-rw-   0        0        0       87 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/AUTHORS.md
--rw-rw-rw-   0        0        0     1233 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/LICENSE.md
--rw-rw-rw-   0        0        0      102 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2991 2024-03-15 11:28:31.678295 youtubedlapi_server_infusiblecoder-3.7.7/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-02-22 10:40:18.000000 youtubedlapi_server_infusiblecoder-3.7.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-15 11:28:31.611268 youtubedlapi_server_infusiblecoder-3.7.7/docs/
--rw-rw-rw-   0        0        0     5829 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/Makefile
--rw-rw-rw-   0        0        0      232 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/about.rst
--rw-rw-rw-   0        0        0     4326 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/api.rst
--rw-rw-rw-   0        0        0       31 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/changelog.rst
--rw-rw-rw-   0        0        0     1680 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/conf.py
--rw-rw-rw-   0        0        0     1650 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/example_info.rst.inc
--rw-rw-rw-   0        0        0     1756 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/example_info_flatten.rst.inc
--rw-rw-rw-   0        0        0      556 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/index.rst
--rw-rw-rw-   0        0        0     1514 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/install.rst
--rwxrwxrwx   0        0        0     5342 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/make.bat
--rw-rw-rw-   0        0        0      688 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/docs/server-manual.rst
--rw-rw-rw-   0        0        0      140 2024-03-15 11:28:31.680808 youtubedlapi_server_infusiblecoder-3.7.7/setup.cfg
--rw-rw-rw-   0        0        0     1490 2024-03-15 11:28:20.000000 youtubedlapi_server_infusiblecoder-3.7.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-15 11:28:31.612266 youtubedlapi_server_infusiblecoder-3.7.7/test/
--rw-rw-rw-   0        0        0     3534 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/test/test_api.py
-drwxrwxrwx   0        0        0        0 2024-03-15 11:28:31.640981 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder/
--rw-rw-rw-   0        0        0       59 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder/__init__.py
--rw-rw-rw-   0        0        0       92 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder/__main__.py
--rw-rw-rw-   0        0        0     8553 2024-03-15 11:24:10.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder/app.py
--rw-rw-rw-   0        0        0     1282 2024-03-15 10:48:31.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder/server.py
--rw-rw-rw-   0        0        0       23 2024-03-15 11:28:04.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder/version.py
-drwxrwxrwx   0        0        0        0 2024-03-15 11:28:31.674783 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder.egg-info/
--rw-rw-rw-   0        0        0     2991 2024-03-15 11:28:31.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      859 2024-03-15 11:28:31.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 11:28:31.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-03-15 11:28:31.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      104 2024-03-15 11:28:31.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2024-03-15 11:28:31.000000 youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 15:56:08.820193 youtubedlapi_server_infusiblecoder-3.7.8/
+-rw-rw-rw-   0        0        0       87 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/AUTHORS.md
+-rw-rw-rw-   0        0        0     1233 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/LICENSE.md
+-rw-rw-rw-   0        0        0      102 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3873 2024-04-19 15:56:08.819375 youtubedlapi_server_infusiblecoder-3.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2885 2024-03-15 11:31:21.000000 youtubedlapi_server_infusiblecoder-3.7.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 15:56:08.764267 youtubedlapi_server_infusiblecoder-3.7.8/docs/
+-rw-rw-rw-   0        0        0     5829 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/Makefile
+-rw-rw-rw-   0        0        0      232 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/about.rst
+-rw-rw-rw-   0        0        0     4326 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/api.rst
+-rw-rw-rw-   0        0        0       31 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1680 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/conf.py
+-rw-rw-rw-   0        0        0     1650 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/example_info.rst.inc
+-rw-rw-rw-   0        0        0     1756 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/example_info_flatten.rst.inc
+-rw-rw-rw-   0        0        0      556 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/index.rst
+-rw-rw-rw-   0        0        0     1514 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/install.rst
+-rwxrwxrwx   0        0        0     5342 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/make.bat
+-rw-rw-rw-   0        0        0      688 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/docs/server-manual.rst
+-rw-rw-rw-   0        0        0      140 2024-04-19 15:56:08.820193 youtubedlapi_server_infusiblecoder-3.7.8/setup.cfg
+-rw-rw-rw-   0        0        0     1490 2024-04-19 15:48:52.000000 youtubedlapi_server_infusiblecoder-3.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:56:08.767221 youtubedlapi_server_infusiblecoder-3.7.8/test/
+-rw-rw-rw-   0        0        0     3534 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/test/test_api.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:56:08.791627 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/
+-rw-rw-rw-   0        0        0       59 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/__init__.py
+-rw-rw-rw-   0        0        0       92 2022-11-27 09:28:23.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/__main__.py
+-rw-rw-rw-   0        0        0     4568 2024-04-19 15:49:13.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/app.py
+-rw-rw-rw-   0        0        0     8037 2024-04-19 09:21:33.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/celery_app_test.py
+-rw-rw-rw-   0        0        0      284 2024-04-19 09:06:03.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/celery_config.py
+-rw-rw-rw-   0        0        0     4567 2024-04-19 15:47:43.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/fastapi_test.py
+-rw-rw-rw-   0        0        0     8553 2024-04-19 14:54:28.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/orignal_app.py
+-rw-rw-rw-   0        0        0     1282 2024-03-15 10:48:31.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/server.py
+-rw-rw-rw-   0        0        0       23 2024-04-19 15:48:46.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/version.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:56:08.817860 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder.egg-info/
+-rw-rw-rw-   0        0        0     3873 2024-04-19 15:56:08.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2024-04-19 15:56:08.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 15:56:08.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-19 15:56:08.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      104 2024-04-19 15:56:08.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2024-04-19 15:56:08.000000 youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder.egg-info/top_level.txt
```

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/LICENSE.md` & `youtubedlapi_server_infusiblecoder-3.7.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/PKG-INFO` & `youtubedlapi_server_infusiblecoder-3.7.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtubedlapi_server_infusiblecoder
-Version: 3.7.7
+Version: 3.7.8
 Summary: An API server based on yt-dlp
 Home-page: https://github.com/syedusama5556/youtubedlapi-server-infusiblecoder
 Author: Syed Usama Ahmad
 Author-email: syedusama5556@gmail.com
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Development Status :: 3 - Alpha
@@ -43,15 +43,45 @@
 
 About
 -----
 
 ``youtubedlapi-server-infusiblecoder`` is released to the public domain, read the [License](https://raw.githubusercontent.com/syedusama5556/youtubedlapi-server-infusiblecoder/master/LICENSE.md) for more info.
 
 
-Example
+NEW Example Usage
+-----
+``uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 127.0.0.1 --port 9191 --workers 1 --log-level info``
+
+or
+
+``uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 0.0.0.0 --port 9191 --workers 1 --log-level info``
+
+or for running in bacground 
+
+``nohup uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 0.0.0.0 --port 9191 --workers 1 --log-level info &``
+
+Run in BG with A Repeted Job To Restart Server When Its Down
+------------------------------------------------------------
+
+create a script named 'bgapi.sh' add below code in the file 
+
+```#!/bin/bash
+while true
+do
+uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 0.0.0.0 --port 9191 --workers 1 --log-level info
+sleep 2500
+done
+```
+save it then run this command to run it in the BG
+
+``nohup ./bgapi.sh &``
+
+
+
+Old Example Usage
 -----
 
 ``youtubedlapi-server-infusiblecoder -p 8000 --host 127.0.0.1 --number-processes 1``
 
 or
 
 ``youtubedlapi-server-infusiblecoder -p 9191 --host 0.0.0.0 --number-processes 1``
```

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/README.md` & `youtubedlapi_server_infusiblecoder-3.7.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,45 @@
 
 About
 -----
 
 ``youtubedlapi-server-infusiblecoder`` is released to the public domain, read the [License](https://raw.githubusercontent.com/syedusama5556/youtubedlapi-server-infusiblecoder/master/LICENSE.md) for more info.
 
 
-Example
+NEW Example Usage
+-----
+``uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 127.0.0.1 --port 9191 --workers 1 --log-level info``
+
+or
+
+``uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 0.0.0.0 --port 9191 --workers 1 --log-level info``
+
+or for running in bacground 
+
+``nohup uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 0.0.0.0 --port 9191 --workers 1 --log-level info &``
+
+Run in BG with A Repeted Job To Restart Server When Its Down
+------------------------------------------------------------
+
+create a script named 'bgapi.sh' add below code in the file 
+
+```#!/bin/bash
+while true
+do
+uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 0.0.0.0 --port 9191 --workers 1 --log-level info
+sleep 2500
+done
+```
+save it then run this command to run it in the BG
+
+``nohup ./bgapi.sh &``
+
+
+
+Old Example Usage
 -----
 
 ``youtubedlapi-server-infusiblecoder -p 8000 --host 127.0.0.1 --number-processes 1``
 
 or
 
 ``youtubedlapi-server-infusiblecoder -p 9191 --host 0.0.0.0 --number-processes 1``
```

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/docs/Makefile` & `youtubedlapi_server_infusiblecoder-3.7.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/docs/api.rst` & `youtubedlapi_server_infusiblecoder-3.7.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/docs/conf.py` & `youtubedlapi_server_infusiblecoder-3.7.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/docs/example_info.rst.inc` & `youtubedlapi_server_infusiblecoder-3.7.8/docs/example_info.rst.inc`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/docs/example_info_flatten.rst.inc` & `youtubedlapi_server_infusiblecoder-3.7.8/docs/example_info_flatten.rst.inc`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/docs/index.rst` & `youtubedlapi_server_infusiblecoder-3.7.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/docs/install.rst` & `youtubedlapi_server_infusiblecoder-3.7.8/docs/install.rst`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/docs/make.bat` & `youtubedlapi_server_infusiblecoder-3.7.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/docs/server-manual.rst` & `youtubedlapi_server_infusiblecoder-3.7.8/docs/server-manual.rst`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/setup.py` & `youtubedlapi_server_infusiblecoder-3.7.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description_txt = (this_directory / "README.md").read_text()
 
 setup(
     name="youtubedlapi_server_infusiblecoder",
-    version="3.7.7",
+    version="3.7.8",
     description="An API server based on yt-dlp",
     long_description=long_description_txt,
     long_description_content_type="text/markdown",
     author="Syed Usama Ahmad",
     author_email="syedusama5556@gmail.com",
     url="https://github.com/syedusama5556/youtubedlapi-server-infusiblecoder",
     packages=["youtubedlapi_server_infusiblecoder"],
```

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/test/test_api.py` & `youtubedlapi_server_infusiblecoder-3.7.8/test/test_api.py`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder/app.py` & `youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/orignal_app.py`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder/server.py` & `youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder/server.py`

 * *Files identical despite different names*

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder.egg-info/PKG-INFO` & `youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtubedlapi_server_infusiblecoder
-Version: 3.7.7
+Version: 3.7.8
 Summary: An API server based on yt-dlp
 Home-page: https://github.com/syedusama5556/youtubedlapi-server-infusiblecoder
 Author: Syed Usama Ahmad
 Author-email: syedusama5556@gmail.com
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Development Status :: 3 - Alpha
@@ -43,15 +43,45 @@
 
 About
 -----
 
 ``youtubedlapi-server-infusiblecoder`` is released to the public domain, read the [License](https://raw.githubusercontent.com/syedusama5556/youtubedlapi-server-infusiblecoder/master/LICENSE.md) for more info.
 
 
-Example
+NEW Example Usage
+-----
+``uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 127.0.0.1 --port 9191 --workers 1 --log-level info``
+
+or
+
+``uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 0.0.0.0 --port 9191 --workers 1 --log-level info``
+
+or for running in bacground 
+
+``nohup uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 0.0.0.0 --port 9191 --workers 1 --log-level info &``
+
+Run in BG with A Repeted Job To Restart Server When Its Down
+------------------------------------------------------------
+
+create a script named 'bgapi.sh' add below code in the file 
+
+```#!/bin/bash
+while true
+do
+uvicorn youtubedlapi_server_infusiblecoder.app:app_asgi --host 0.0.0.0 --port 9191 --workers 1 --log-level info
+sleep 2500
+done
+```
+save it then run this command to run it in the BG
+
+``nohup ./bgapi.sh &``
+
+
+
+Old Example Usage
 -----
 
 ``youtubedlapi-server-infusiblecoder -p 8000 --host 127.0.0.1 --number-processes 1``
 
 or
 
 ``youtubedlapi-server-infusiblecoder -p 9191 --host 0.0.0.0 --number-processes 1``
```

### Comparing `youtubedlapi_server_infusiblecoder-3.7.7/youtubedlapi_server_infusiblecoder.egg-info/SOURCES.txt` & `youtubedlapi_server_infusiblecoder-3.7.8/youtubedlapi_server_infusiblecoder.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 docs/install.rst
 docs/make.bat
 docs/server-manual.rst
 test/test_api.py
 youtubedlapi_server_infusiblecoder/__init__.py
 youtubedlapi_server_infusiblecoder/__main__.py
 youtubedlapi_server_infusiblecoder/app.py
+youtubedlapi_server_infusiblecoder/celery_app_test.py
+youtubedlapi_server_infusiblecoder/celery_config.py
+youtubedlapi_server_infusiblecoder/fastapi_test.py
+youtubedlapi_server_infusiblecoder/orignal_app.py
 youtubedlapi_server_infusiblecoder/server.py
 youtubedlapi_server_infusiblecoder/version.py
 youtubedlapi_server_infusiblecoder.egg-info/PKG-INFO
 youtubedlapi_server_infusiblecoder.egg-info/SOURCES.txt
 youtubedlapi_server_infusiblecoder.egg-info/dependency_links.txt
 youtubedlapi_server_infusiblecoder.egg-info/entry_points.txt
 youtubedlapi_server_infusiblecoder.egg-info/requires.txt
```

