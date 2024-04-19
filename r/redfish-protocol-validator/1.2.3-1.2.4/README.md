# Comparing `tmp/redfish_protocol_validator-1.2.3.tar.gz` & `tmp/redfish_protocol_validator-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_protocol_validator-1.2.3.tar", last modified: Sat Feb  3 02:03:32 2024, max compression
+gzip compressed data, was "redfish_protocol_validator-1.2.4.tar", last modified: Fri Apr 19 19:59:59 2024, max compression
```

## Comparing `redfish_protocol_validator-1.2.3.tar` & `redfish_protocol_validator-1.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 02:03:32.918936 redfish_protocol_validator-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-02-03 02:03:32.918936 redfish_protocol_validator-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 02:03:32.914935 redfish_protocol_validator-1.2.3/redfish_protocol_validator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/console_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/protocol_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    24902 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/redfish_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    20487 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    52407 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/security_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    45918 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/service_details.py
--rw-r--r--   0 runner    (1001) docker     (127)    64194 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/service_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28730 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/service_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/system_under_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 02:03:32.914935 redfish_protocol_validator-1.2.3/redfish_protocol_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-02-03 02:03:32.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-03 02:03:32.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 02:03:32.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-03 02:03:32.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-03 02:03:32.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-03 02:03:32.000000 redfish_protocol_validator-1.2.3/redfish_protocol_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 02:03:32.918936 redfish_protocol_validator-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-02-03 02:03:23.000000 redfish_protocol_validator-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:59:59.068926 redfish_protocol_validator-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-19 19:59:59.068926 redfish_protocol_validator-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:59:59.068926 redfish_protocol_validator-1.2.4/redfish_protocol_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/console_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/protocol_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24902 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/redfish_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20487 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52407 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/security_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45918 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64194 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18110 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/system_under_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:59:59.068926 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 19:59:59.000000 redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:59:59.068926 redfish_protocol_validator-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-19 19:59:48.000000 redfish_protocol_validator-1.2.4/setup.py
```

### Comparing `redfish_protocol_validator-1.2.3/LICENSE.md` & `redfish_protocol_validator-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/PKG-INFO` & `redfish_protocol_validator-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_protocol_validator
-Version: 1.2.3
+Version: 1.2.4
 Summary: Redfish Protocol Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_protocol_validator-1.2.3/README.md` & `redfish_protocol_validator-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/accounts.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/console_scripts.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/console_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from redfish_protocol_validator import service_requests
 from redfish_protocol_validator import service_responses
 from redfish_protocol_validator import sessions
 from redfish_protocol_validator import utils
 from redfish_protocol_validator.constants import Result
 from redfish_protocol_validator.system_under_test import SystemUnderTest
 
-tool_version = '1.2.3'
+tool_version = '1.2.4'
 
 
 def perform_tests(sut: SystemUnderTest):
     """Perform the protocol validation tests on the resources."""
     protocol_details.test_protocol_details(sut)
     service_requests.test_service_requests(sut)
     service_responses.test_service_responses(sut)
```

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/constants.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/constants.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/protocol_details.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/protocol_details.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/redfish_logo.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/redfish_logo.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/report.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/report.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/resources.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/resources.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/security_details.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/security_details.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/service_details.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_details.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/service_requests.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_requests.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/service_responses.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/service_responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,17 +290,41 @@
     uri = '/redfish/v1/'
     method = 'GET'
     header = 'OData-Version'
     response = sut.get_response(method, uri)
     test_header_value(sut, header, '4.0', uri, method, response,
                       Assertion.RESP_HEADERS_ODATA_VERSION)
 
+def test_www_authenticate_requirement(sut: SystemUnderTest):
+    """Check for HTTPBasicAuth Property"""
+    response = sut.get_response('GET', sut.account_service_uri)
+
+    if (response is not None and response.ok):
+        data = response.json()
+        key = 'HTTPBasicAuth'
+        if key in data:
+            if data[key] != "Enabled":
+                #  could be either Disabled or Unadvertised
+                return False
+            else:
+                return True
+    # Any Failure will be considered as HTTPBasicAuth not present
+    return True
+
 
 def test_www_authenticate_header(sut: SystemUnderTest):
     """Perform tests for Assertion.RESP_HEADERS_WWW_AUTHENTICATE."""
+
+    if(False == test_www_authenticate_requirement(sut)):
+        msg = ('The WWW-Authenticate header is not tested because value of HTTPBasicAuth '
+                   'is either Disabled or Unadvertised ')
+        sut.log(Result.NOT_TESTED, '', '', '',
+                Assertion.RESP_HEADERS_WWW_AUTHENTICATE, msg)
+        return
+
     # a selection of URis to test
     uris = [sut.sessions_uri, sut.mgr_net_proto_uri, sut.systems_uri,
             sut.accounts_uri, sut.account_service_uri,
             sut.privilege_registry_uri]
     # eliminate URIs the service doesn't support
     uris = [u for u in uris if u is not None]
     found_unauthorized = False
```

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/sessions.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/sessions.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/system_under_test.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/system_under_test.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator/utils.py` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator/utils.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator.egg-info/PKG-INFO` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_protocol_validator
-Version: 1.2.3
+Version: 1.2.4
 Summary: Redfish Protocol Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_protocol_validator-1.2.3/redfish_protocol_validator.egg-info/SOURCES.txt` & `redfish_protocol_validator-1.2.4/redfish_protocol_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.2.3/setup.py` & `redfish_protocol_validator-1.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_protocol_validator",
-    version="1.2.3",
+    version="1.2.4",
     description="Redfish Protocol Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

