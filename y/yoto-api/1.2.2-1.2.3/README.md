# Comparing `tmp/yoto_api-1.2.2.tar.gz` & `tmp/yoto_api-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.2.2.tar", last modified: Tue Apr 16 03:39:51 2024, max compression
+gzip compressed data, was "yoto_api-1.2.3.tar", last modified: Fri Apr 19 19:12:07 2024, max compression
```

## Comparing `yoto_api-1.2.2.tar` & `yoto_api-1.2.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:39:51.017190 yoto_api-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 03:39:27.000000 yoto_api-1.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-16 03:39:27.000000 yoto_api-1.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 03:39:27.000000 yoto_api-1.2.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 03:39:27.000000 yoto_api-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 03:39:27.000000 yoto_api-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-16 03:39:51.017190 yoto_api-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-16 03:39:27.000000 yoto_api-1.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:39:27.000000 yoto_api-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:39:51.017190 yoto_api-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-16 03:39:44.000000 yoto_api-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:39:51.013190 yoto_api-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:39:27.000000 yoto_api-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 03:39:27.000000 yoto_api-1.2.2/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:39:51.013190 yoto_api-1.2.2/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-16 03:39:27.000000 yoto_api-1.2.2/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-16 03:39:27.000000 yoto_api-1.2.2/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    19786 2024-04-16 03:39:27.000000 yoto_api-1.2.2/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-16 03:39:27.000000 yoto_api-1.2.2/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 03:39:27.000000 yoto_api-1.2.2/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 03:39:27.000000 yoto_api-1.2.2/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 03:39:27.000000 yoto_api-1.2.2/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:39:51.017190 yoto_api-1.2.2/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-16 03:39:51.000000 yoto_api-1.2.2/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-16 03:39:51.000000 yoto_api-1.2.2/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:39:51.000000 yoto_api-1.2.2/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:39:50.000000 yoto_api-1.2.2/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 03:39:51.000000 yoto_api-1.2.2/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:07.463125 yoto_api-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 19:11:43.000000 yoto_api-1.2.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-19 19:11:43.000000 yoto_api-1.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 19:11:43.000000 yoto_api-1.2.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 19:11:43.000000 yoto_api-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 19:11:43.000000 yoto_api-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 19:12:07.463125 yoto_api-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-19 19:11:43.000000 yoto_api-1.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 19:11:43.000000 yoto_api-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:12:07.463125 yoto_api-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 19:12:01.000000 yoto_api-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:07.459125 yoto_api-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:11:43.000000 yoto_api-1.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 19:11:43.000000 yoto_api-1.2.3/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:07.459125 yoto_api-1.2.3/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 19:11:43.000000 yoto_api-1.2.3/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:12:07.463125 yoto_api-1.2.3/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 19:12:07.000000 yoto_api-1.2.3/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.2.2/CONTRIBUTING.rst` & `yoto_api-1.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.2/LICENSE` & `yoto_api-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.2/PKG-INFO` & `yoto_api-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: pytz
+Requires-Dist: requests
 
 Introduction
 ============
 
 Early days of this API. Plan is to use this for home assistant. Basics are only item build for auth so far.
 
 To run this code for test I am doing::
```

### Comparing `yoto_api-1.2.2/README.rst` & `yoto_api-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.2/setup.py` & `yoto_api-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.2.2",
+    version="1.2.3",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.2.2/yoto_api/Card.py` & `yoto_api-1.2.3/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.2/yoto_api/YotoAPI.py` & `yoto_api-1.2.3/yoto_api/YotoAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,29 +46,26 @@
             scope=response["scope"],
             valid_until=valid_until,
         )
 
     # pass='audience=https%3A//api.yotoplay.com&client_id=FILL_THIS_IN&grant_type=password&password=FILL_THIS_IN&scope=openid%20email%20profile%20offline_access&username=FILL_THIS_IN%40gmail.com'
     # curl -d "$pass" https://api.yotoplay.com/auth/token | jq '.access_token'
 
-    def update_devices(self, token) -> dict[YotoPlayer]:
-        response = self._get_devices(token)
-        result = {}
-        for device in response["devices"]:
-            player: YotoPlayer = YotoPlayer(
-                id=device["deviceId"],
-                name=device["name"],
-                deviceType=device["deviceType"],
-                online=device["online"],
-                last_updated_at=datetime.datetime.now(pytz.utc)
-            )
-            result[player.id] = player
+    def update_devices(self, token, devices) -> dict[YotoPlayer]:
+        response = self._get_devices(token)      
+        if devices is None:
+            devices = {}
+        else: 
+            for player in response["devices"]:
+                devices[player.id].id = player["deviceId"]
+                devices[player.id].name = player["name"]
+                devices[player.id].deviceType = player["deviceType"]
+                devices[player.id].last_update_at = datetime.datetime.now(pytz.utc)
+                devices[player.id].online = player["online"],
 
-        return result
-        # TODO: parse the data and return a list of yoto devices.
 
     def update_library(self, token) -> list[Card]:
         cards = self._get_cards(token)
         return cards
         # TODO: parse the data and return a list of cards.
 
     def refresh_token(self, token: Token) -> Token:
```

### Comparing `yoto_api-1.2.2/yoto_api/YotoManager.py` & `yoto_api-1.2.3/yoto_api/YotoManager.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def initialize(self) -> None:
         self.token: Token = self.api.login(self.username, self.password)
         self.update_player_status()
         self.update_cards()
 
     def update_player_status(self) -> None:
         # Updates the data with current player data.
-        self.players = self.api.update_devices(self.token)
+        self.players = self.api.update_devices(self.token, self.players)
 
     def update_cards(self) -> None:
         # Updates library and all card data.  Typically only required on startup.
         # TODO: Should update the self.library object with a current dict of players. Should it do details for all cards too or separate?
         self.library = self.api.update_library(self.token)
 
     def check_and_refresh_token(self) -> bool:
```

### Comparing `yoto_api-1.2.2/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.2.3/yoto_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: pytz
+Requires-Dist: requests
 
 Introduction
 ============
 
 Early days of this API. Plan is to use this for home assistant. Basics are only item build for auth so far.
 
 To run this code for test I am doing::
```

