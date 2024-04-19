# Comparing `tmp/blackduck-1.1.0.tar.gz` & `tmp/blackduck-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackduck-1.1.0.tar", last modified: Fri Feb 24 17:39:18 2023, max compression
+gzip compressed data, was "blackduck-1.1.3.tar", last modified: Fri Apr 19 21:46:42 2024, max compression
```

## Comparing `blackduck-1.1.0.tar` & `blackduck-1.1.3.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxr-xr-x   0 gsnyder    (501) staff       (20)        0 2023-02-24 17:39:18.951934 blackduck-1.1.0/
--rw-r--r--   0 gsnyder    (501) staff       (20)    11357 2019-03-14 18:13:41.000000 blackduck-1.1.0/LICENSE
--rw-r--r--   0 gsnyder    (501) staff       (20)     4968 2023-02-24 17:39:18.952073 blackduck-1.1.0/PKG-INFO
--rw-r--r--   0 gsnyder    (501) staff       (20)     4242 2023-02-24 13:59:12.000000 blackduck-1.1.0/README.md
-drwxr-xr-x   0 gsnyder    (501) staff       (20)        0 2023-02-24 17:39:18.903975 blackduck-1.1.0/blackduck/
--rw-r--r--   0 gsnyder    (501) staff       (20)     7692 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Authentication.py
--rw-r--r--   0 gsnyder    (501) staff       (20)    11169 2023-02-24 13:55:25.000000 blackduck-1.1.0/blackduck/Client.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     3147 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Components.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     7803 2022-09-09 20:01:39.000000 blackduck-1.1.0/blackduck/Core.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     4847 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/CustomFields.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     1040 2022-09-09 20:01:39.000000 blackduck-1.1.0/blackduck/Exceptions.py
--rwxr-xr-x   0 gsnyder    (501) staff       (20)     7049 2022-09-09 20:01:39.000000 blackduck-1.1.0/blackduck/HubRestApi.py
--rw-r--r--   0 gsnyder    (501) staff       (20)      593 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Jobs.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     1342 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Ldap.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     1744 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Licences.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     1490 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Policy.py
--rw-r--r--   0 gsnyder    (501) staff       (20)    27790 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Projects.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     3736 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Reporting.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     2427 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Roles.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     5342 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Scans.py
--rw-r--r--   0 gsnyder    (501) staff       (20)      528 2022-09-09 20:01:39.000000 blackduck-1.1.0/blackduck/Snippet.py
--rw-r--r--   0 gsnyder    (501) staff       (20)      605 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/System.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     2406 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/UserGroup.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     2496 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Users.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     4285 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Utils.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     2040 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Versions.py
--rw-r--r--   0 gsnyder    (501) staff       (20)     1695 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/Vulnerabilities.py
--rw-r--r--   0 gsnyder    (501) staff       (20)       64 2022-09-09 20:01:39.000000 blackduck-1.1.0/blackduck/__init__.py
--rw-r--r--   0 gsnyder    (501) staff       (20)       63 2023-02-24 13:55:42.000000 blackduck-1.1.0/blackduck/__version__.py
--rw-r--r--   0 gsnyder    (501) staff       (20)      313 2022-03-22 19:02:57.000000 blackduck-1.1.0/blackduck/constants.py
-drwxr-xr-x   0 gsnyder    (501) staff       (20)        0 2023-02-24 17:39:18.949660 blackduck-1.1.0/blackduck.egg-info/
--rw-r--r--   0 gsnyder    (501) staff       (20)     4968 2023-02-24 17:39:18.000000 blackduck-1.1.0/blackduck.egg-info/PKG-INFO
--rw-r--r--   0 gsnyder    (501) staff       (20)      781 2023-02-24 17:39:18.000000 blackduck-1.1.0/blackduck.egg-info/SOURCES.txt
--rw-r--r--   0 gsnyder    (501) staff       (20)        1 2023-02-24 17:39:18.000000 blackduck-1.1.0/blackduck.egg-info/dependency_links.txt
--rw-r--r--   0 gsnyder    (501) staff       (20)       25 2023-02-24 17:39:18.000000 blackduck-1.1.0/blackduck.egg-info/requires.txt
--rw-r--r--   0 gsnyder    (501) staff       (20)       10 2023-02-24 17:39:18.000000 blackduck-1.1.0/blackduck.egg-info/top_level.txt
--rw-r--r--   0 gsnyder    (501) staff       (20)       63 2023-02-24 17:39:18.953430 blackduck-1.1.0/setup.cfg
--rw-r--r--   0 gsnyder    (501) staff       (20)     4149 2022-03-22 19:02:57.000000 blackduck-1.1.0/setup.py
-drwxr-xr-x   0 gsnyder    (501) staff       (20)        0 2023-02-24 17:39:18.951006 blackduck-1.1.0/test/
--rw-r--r--   0 gsnyder    (501) staff       (20)    19966 2021-03-27 11:52:38.000000 blackduck-1.1.0/test/test_hub_rest_api_python.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 21:46:42.529744 blackduck-1.1.3/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-04-19 21:00:00.000000 blackduck-1.1.3/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     5003 2024-04-19 21:46:42.529744 blackduck-1.1.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4242 2024-04-19 21:00:00.000000 blackduck-1.1.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 21:46:42.525744 blackduck-1.1.3/blackduck/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7691 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Authentication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11169 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Client.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3147 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Components.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7803 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Core.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4847 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/CustomFields.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1040 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Exceptions.py
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     7049 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/HubRestApi.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      593 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Jobs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1342 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Ldap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1744 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Licences.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1490 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Policy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    27790 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Projects.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3736 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Reporting.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2427 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Roles.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5342 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Scans.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      528 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Snippet.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      605 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/System.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2406 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/UserGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2496 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Users.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4285 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Utils.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2040 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Versions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1727 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/Vulnerabilities.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       63 2024-04-19 21:24:33.000000 blackduck-1.1.3/blackduck/__version__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      313 2024-04-19 21:00:00.000000 blackduck-1.1.3/blackduck/constants.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-19 21:46:42.525744 blackduck-1.1.3/blackduck.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     5003 2024-04-19 21:46:42.000000 blackduck-1.1.3/blackduck.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      748 2024-04-19 21:46:42.000000 blackduck-1.1.3/blackduck.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 21:46:42.000000 blackduck-1.1.3/blackduck.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-04-19 21:46:42.000000 blackduck-1.1.3/blackduck.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-04-19 21:46:42.000000 blackduck-1.1.3/blackduck.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       63 2024-04-19 21:46:42.529744 blackduck-1.1.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4149 2024-04-19 21:45:04.000000 blackduck-1.1.3/setup.py
```

### Comparing `blackduck-1.1.0/LICENSE` & `blackduck-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/PKG-INFO` & `blackduck-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: blackduck
-Version: 1.1.0
+Version: 1.1.3
 Summary: Package for using the Synopsys Black Duck Hub REST API.
 Home-page: https://github.com/blackducksoftware/hub-rest-api-python
 Author: Glenn Snyder
 Author-email: gsnyder@synopsys.com
 License: Apache
 Keywords: api
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: python-dateutil
 
 
 # Overview
 
 The hub-rest-api-python provides Python bindings for Hub REST API.
 
 # Paging and Black Duck v2022.2
@@ -134,9 +135,7 @@
 
 `pip3 install blackduck`
 
 ## Documentation ##
 Documentation for hub-rest-api-python can be found on the base project:
 [Hub REST API Python Wiki](https://github.com/blackducksoftware/hub-rest-api-python/wiki)
 
-
-
```

### Comparing `blackduck-1.1.0/README.md` & `blackduck-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Authentication.py` & `blackduck-1.1.3/blackduck/Authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def authenticate(self):
         if not self.session.verify:
             requests.packages.urllib3.disable_warnings()
             # Announce this on every auth attempt, as a little incentive to properly configure certs
             logger.warning("ssl verification disabled, connection insecure. do NOT use verify=False in production!")
 
         response = self.session.post(
-            url="/api/tokens/authenticate",
+            url="api/tokens/authenticate",
             auth=NoAuth(),  # temporarily strip authentication to avoid infinite recursion
             headers={"Authorization": f"token {self.access_token}"}
         )
 
         if response.status_code == 200:
             try:
                 content = response.json()
```

### Comparing `blackduck-1.1.0/blackduck/Client.py` & `blackduck-1.1.3/blackduck/Client.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Components.py` & `blackduck-1.1.3/blackduck/Components.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Core.py` & `blackduck-1.1.3/blackduck/Core.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/CustomFields.py` & `blackduck-1.1.3/blackduck/CustomFields.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Exceptions.py` & `blackduck-1.1.3/blackduck/Exceptions.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/HubRestApi.py` & `blackduck-1.1.3/blackduck/HubRestApi.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Jobs.py` & `blackduck-1.1.3/blackduck/Jobs.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Ldap.py` & `blackduck-1.1.3/blackduck/Ldap.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Licences.py` & `blackduck-1.1.3/blackduck/Licences.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Policy.py` & `blackduck-1.1.3/blackduck/Policy.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Projects.py` & `blackduck-1.1.3/blackduck/Projects.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Reporting.py` & `blackduck-1.1.3/blackduck/Reporting.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Roles.py` & `blackduck-1.1.3/blackduck/Roles.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Scans.py` & `blackduck-1.1.3/blackduck/Scans.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Snippet.py` & `blackduck-1.1.3/blackduck/Snippet.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/System.py` & `blackduck-1.1.3/blackduck/System.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/UserGroup.py` & `blackduck-1.1.3/blackduck/UserGroup.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Users.py` & `blackduck-1.1.3/blackduck/Users.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Utils.py` & `blackduck-1.1.3/blackduck/Utils.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Versions.py` & `blackduck-1.1.3/blackduck/Versions.py`

 * *Files identical despite different names*

### Comparing `blackduck-1.1.0/blackduck/Vulnerabilities.py` & `blackduck-1.1.3/blackduck/Vulnerabilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # TODO: Refactor this, i.e. use get_link method?
 def get_vulnerable_bom_components(self, version_obj, limit=9999):
     url = "{}/vulnerable-bom-components".format(version_obj['_meta']['href'])
     custom_headers = {'Accept': 'application/vnd.blackducksoftware.bill-of-materials-6+json'}
     param_string = self._get_parameter_string({'limit': limit})
     url = "{}{}".format(url, param_string)
     response = self.execute_get(url, custom_headers=custom_headers)
+    response.raise_for_status()
     return response.json()
 
 # TODO: Remove or refactor this
 def get_component_remediation(self, bom_component):
     url = "{}/remediating".format(bom_component['componentVersion'])
     logger.debug("Url for getting remediation info is : {}".format(url))
     response = self.execute_get(url)
```

### Comparing `blackduck-1.1.0/blackduck.egg-info/PKG-INFO` & `blackduck-1.1.3/blackduck.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: blackduck
-Version: 1.1.0
+Version: 1.1.3
 Summary: Package for using the Synopsys Black Duck Hub REST API.
 Home-page: https://github.com/blackducksoftware/hub-rest-api-python
 Author: Glenn Snyder
 Author-email: gsnyder@synopsys.com
 License: Apache
 Keywords: api
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: python-dateutil
 
 
 # Overview
 
 The hub-rest-api-python provides Python bindings for Hub REST API.
 
 # Paging and Black Duck v2022.2
@@ -134,9 +135,7 @@
 
 `pip3 install blackduck`
 
 ## Documentation ##
 Documentation for hub-rest-api-python can be found on the base project:
 [Hub REST API Python Wiki](https://github.com/blackducksoftware/hub-rest-api-python/wiki)
 
-
-
```

### Comparing `blackduck-1.1.0/setup.py` & `blackduck-1.1.3/setup.py`

 * *Files identical despite different names*

