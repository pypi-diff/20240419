# Comparing `tmp/NetSuite-Connector-0.2.2.tar.gz` & `tmp/netsuite_connector-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NetSuite-Connector-0.2.2.tar", last modified: Tue May  9 22:45:01 2023, max compression
+gzip compressed data, was "netsuite_connector-0.3.0.tar", last modified: Fri Apr 19 00:41:41 2024, max compression
```

## Comparing `NetSuite-Connector-0.2.2.tar` & `netsuite_connector-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 22:45:00.965000 NetSuite-Connector-0.2.2/
--rw-rw-rw-   0        0        0     1090 2023-03-22 19:27:04.000000 NetSuite-Connector-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     4284 2023-05-09 22:45:00.911000 NetSuite-Connector-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2467 2023-03-22 21:11:08.000000 NetSuite-Connector-0.2.2/README.md
--rw-rw-rw-   0        0        0      735 2023-05-09 22:42:04.000000 NetSuite-Connector-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 22:45:00.953000 NetSuite-Connector-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 22:44:58.483000 NetSuite-Connector-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 22:44:59.736000 NetSuite-Connector-0.2.2/src/NetSuite_Connector/
--rw-rw-rw-   0        0        0     4004 2023-03-22 21:05:45.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector/NetSuite.py
--rw-rw-rw-   0        0        0     4154 2023-03-22 20:27:37.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector/ODBC.py
--rw-rw-rw-   0        0        0        0 2022-10-25 21:58:40.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 22:45:00.562000 NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/
--rw-rw-rw-   0        0        0     4284 2023-05-09 22:44:57.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-05-09 22:44:58.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 22:44:57.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-09 22:44:57.000000 NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 22:45:00.771000 NetSuite-Connector-0.2.2/tests/
--rw-rw-rw-   0        0        0      345 2022-10-25 22:40:03.000000 NetSuite-Connector-0.2.2/tests/test_odbc.py
+drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-19 00:41:41.539584 netsuite_connector-0.3.0/
+-rw-r--r--   0 marcos     (501) staff       (20)     1069 2024-04-18 21:33:03.000000 netsuite_connector-0.3.0/LICENSE
+-rw-r--r--   0 marcos     (501) staff       (20)     4440 2024-04-19 00:41:41.539176 netsuite_connector-0.3.0/PKG-INFO
+-rw-r--r--   0 marcos     (501) staff       (20)     2661 2024-04-18 23:56:48.000000 netsuite_connector-0.3.0/README.md
+-rw-r--r--   0 marcos     (501) staff       (20)      713 2024-04-18 23:05:56.000000 netsuite_connector-0.3.0/pyproject.toml
+-rw-r--r--   0 marcos     (501) staff       (20)       38 2024-04-19 00:41:41.539648 netsuite_connector-0.3.0/setup.cfg
+drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-19 00:41:41.531896 netsuite_connector-0.3.0/src/
+drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-19 00:41:41.533578 netsuite_connector-0.3.0/src/NetSuite_Connector/
+-rw-r--r--   0 marcos     (501) staff       (20)     5585 2024-04-18 23:53:43.000000 netsuite_connector-0.3.0/src/NetSuite_Connector/NetSuite.py
+-rw-r--r--   0 marcos     (501) staff       (20)     1612 2024-04-19 00:01:26.000000 netsuite_connector-0.3.0/src/NetSuite_Connector/ODBC.py
+-rw-------   0 marcos     (501) staff       (20)        0 2022-10-25 21:58:40.000000 netsuite_connector-0.3.0/src/NetSuite_Connector/__init__.py
+drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-19 00:41:41.538701 netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/
+-rw-r--r--   0 marcos     (501) staff       (20)     4440 2024-04-19 00:41:41.000000 netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/PKG-INFO
+-rw-r--r--   0 marcos     (501) staff       (20)      359 2024-04-19 00:41:41.000000 netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/SOURCES.txt
+-rw-r--r--   0 marcos     (501) staff       (20)        1 2024-04-19 00:41:41.000000 netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/dependency_links.txt
+-rw-r--r--   0 marcos     (501) staff       (20)       19 2024-04-19 00:41:41.000000 netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/top_level.txt
+drwxr-xr-x   0 marcos     (501) staff       (20)        0 2024-04-19 00:41:41.538259 netsuite_connector-0.3.0/tests/
+-rw-r--r--   0 marcos     (501) staff       (20)    12133 2024-04-18 23:59:11.000000 netsuite_connector-0.3.0/tests/test_netsuite.py
+-rw-r--r--   0 marcos     (501) staff       (20)     7682 2024-04-18 21:33:57.000000 netsuite_connector-0.3.0/tests/test_odbc.py
```

### Comparing `NetSuite-Connector-0.2.2/LICENSE` & `netsuite_connector-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Marcos Lopez
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Marcos Lopez
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `NetSuite-Connector-0.2.2/PKG-INFO` & `netsuite_connector-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,117 +1,108 @@
-Metadata-Version: 2.1
-Name: NetSuite-Connector
-Version: 0.2.2
-Summary: NetSuite Connector
-Author-email: Marcos Lopez <merick16@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Marcos Lopez
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/IngMarcosLopez/NetSuite-Connector
-Project-URL: Bug Tracker, https://github.com/IngMarcosLopez/NetSuite-Connector/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# NetSuite-Connector
-
-## Installation
-
-Only Restlet support:
-
-    $ pip install NetSuite-Connector
-## Get Started
-The following examples shows how to use this module.
-
-### RESTlet GET
-```python
-from NetSuite_Connector.NetSuite import NetSuite
-nt = NetSuite(
-    account_id=123456,
-    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
-    token_keys=dict(token_id="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
-)
-
-x = nt.get(
-    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
-    headers={"Content-Type": "application/json"},
-    params={}
-)
-print(x)
-# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, response='{"foo":"bar"}', code=200)
-```
-### RESTlet PUT - POST - DELETE
-```python
-from NetSuite_Connector.NetSuite import NetSuite
-nt = NetSuite(
-    account_id=123456,
-    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
-    token_keys=dict(token_id="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
-)
-body={"foo":"bar"}
-x = nt.post(
-    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
-    headers={"Content-Type": "application/json"},
-    params={},
-    body=body
-)
-print(x)
-# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
-```
-# ODBC Queries
-
-Connector only supports ODBC Driver queries, JDBC is not supported
-## Get Started
-
-Before you begin install [ODBC Driver](https://system.netsuite.com/app/help/helpcenter.nl?fid=book_N748613.html).
-
-Note that Support for NetSuite2.com is supported, which means that Only roles that hat not activated 2FA are supported. Also note that role must have permission to SuiteAnalitics.
-
-### ODBC Query
-
-```python
-from NetSuite_Connector.ODBC import ODBC
-
-nt = ODBC(
-    account_id="*****",
-    user_email="*****",
-    role_id="*****",
-    dsn="*****",
-    password="*****"
-)
-q = nt.query("SELECT * FROM OA_tables")
-print(q.status)
-# 200
-print(q.response)
-#[{"foo":"bar"}]
-print(q.data_received)
-# SELECT * FROM OA_tables
-print(q.columns)
-# ["foo"]
-```
-
-
-## TODO
-
-- Add TBA for ODBC connector support
+Metadata-Version: 2.1
+Name: NetSuite-Connector
+Version: 0.3.0
+Summary: NetSuite Connector
+Author-email: Marcos Lopez <merick16@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Marcos Lopez
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/IngMarcosLopez/NetSuite-Connector
+Project-URL: Bug Tracker, https://github.com/IngMarcosLopez/NetSuite-Connector/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# NetSuite-Connector
+
+## Supports
+
+- [SuiteTalk REST Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_1559132836.html)
+- [Restlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799403.html#Related-Support-Articles)
+
+## Installation
+
+    $ pip install NetSuite-Connector
+
+## Get Started
+
+The following examples shows how to use this module.
+
+### RESTlet GET
+
+```python
+from NetSuite_Connector.NetSuite import NetSuite
+nt = NetSuite(
+    account_id=123456,
+    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
+    token_keys=dict(token_key="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
+)
+
+x = nt.get(
+    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
+    headers={"Content-Type": "application/json"},
+    params={"foo":"bar"}
+)
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, response='{"foo":"bar"}', code=200)
+```
+
+### RESTlet PUT - POST - DELETE
+
+```python
+from NetSuite_Connector.NetSuite import NetSuite
+nt = NetSuite(
+    account_id=123456,
+    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
+    token_keys=dict(token_key="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
+)
+body={"foo":"bar"}
+x = nt.post(
+    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
+    headers={"Content-Type": "application/json"},
+    params={},
+    body=body
+)
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
+```
+
+# SuiteQL Queries
+
+To execute SuiteQL queries through REST web services, send a POST request to the `suiteql` resource, and specify the query in the request body after the query parameter `q`. The following example shows a SuiteQL query executed through REST web services.
+
+### SuiteQL Query
+
+```python
+from NetSuite_Connector.ODBC import ODBC
+
+nt = ODBC(
+    account_id=123456,
+    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
+    token_keys=dict(token_key="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
+)
+q = nt.query("SELECT top 10 * FROM transaction")
+print(q)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
+```
```

### Comparing `NetSuite-Connector-0.2.2/README.md` & `netsuite_connector-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,72 @@
-# NetSuite-Connector
-
-## Installation
-
-Only Restlet support:
-
-    $ pip install NetSuite-Connector
-## Get Started
-The following examples shows how to use this module.
-
-### RESTlet GET
-```python
-from NetSuite_Connector.NetSuite import NetSuite
-nt = NetSuite(
-    account_id=123456,
-    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
-    token_keys=dict(token_id="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
-)
-
-x = nt.get(
-    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
-    headers={"Content-Type": "application/json"},
-    params={}
-)
-print(x)
-# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, response='{"foo":"bar"}', code=200)
-```
-### RESTlet PUT - POST - DELETE
-```python
-from NetSuite_Connector.NetSuite import NetSuite
-nt = NetSuite(
-    account_id=123456,
-    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
-    token_keys=dict(token_id="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
-)
-body={"foo":"bar"}
-x = nt.post(
-    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
-    headers={"Content-Type": "application/json"},
-    params={},
-    body=body
-)
-print(x)
-# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
-```
-# ODBC Queries
-
-Connector only supports ODBC Driver queries, JDBC is not supported
-## Get Started
-
-Before you begin install [ODBC Driver](https://system.netsuite.com/app/help/helpcenter.nl?fid=book_N748613.html).
-
-Note that Support for NetSuite2.com is supported, which means that Only roles that hat not activated 2FA are supported. Also note that role must have permission to SuiteAnalitics.
-
-### ODBC Query
-
-```python
-from NetSuite_Connector.ODBC import ODBC
-
-nt = ODBC(
-    account_id="*****",
-    user_email="*****",
-    role_id="*****",
-    dsn="*****",
-    password="*****"
-)
-q = nt.query("SELECT * FROM OA_tables")
-print(q.status)
-# 200
-print(q.response)
-#[{"foo":"bar"}]
-print(q.data_received)
-# SELECT * FROM OA_tables
-print(q.columns)
-# ["foo"]
-```
-
-
-## TODO
-
-- Add TBA for ODBC connector support
+# NetSuite-Connector
+
+## Supports
+
+- [SuiteTalk REST Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_1559132836.html)
+- [Restlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799403.html#Related-Support-Articles)
+
+## Installation
+
+    $ pip install NetSuite-Connector
+
+## Get Started
+
+The following examples shows how to use this module.
+
+### RESTlet GET
+
+```python
+from NetSuite_Connector.NetSuite import NetSuite
+nt = NetSuite(
+    account_id=123456,
+    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
+    token_keys=dict(token_key="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
+)
+
+x = nt.get(
+    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
+    headers={"Content-Type": "application/json"},
+    params={"foo":"bar"}
+)
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, response='{"foo":"bar"}', code=200)
+```
+
+### RESTlet PUT - POST - DELETE
+
+```python
+from NetSuite_Connector.NetSuite import NetSuite
+nt = NetSuite(
+    account_id=123456,
+    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
+    token_keys=dict(token_key="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
+)
+body={"foo":"bar"}
+x = nt.post(
+    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
+    headers={"Content-Type": "application/json"},
+    params={},
+    body=body
+)
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
+```
+
+# SuiteQL Queries
+
+To execute SuiteQL queries through REST web services, send a POST request to the `suiteql` resource, and specify the query in the request body after the query parameter `q`. The following example shows a SuiteQL query executed through REST web services.
+
+### SuiteQL Query
+
+```python
+from NetSuite_Connector.ODBC import ODBC
+
+nt = ODBC(
+    account_id=123456,
+    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
+    token_keys=dict(token_key="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
+)
+q = nt.query("SELECT top 10 * FROM transaction")
+print(q)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
+```
```

### Comparing `NetSuite-Connector-0.2.2/src/NetSuite_Connector.egg-info/PKG-INFO` & `netsuite_connector-0.3.0/src/NetSuite_Connector.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,117 +1,108 @@
-Metadata-Version: 2.1
-Name: NetSuite-Connector
-Version: 0.2.2
-Summary: NetSuite Connector
-Author-email: Marcos Lopez <merick16@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Marcos Lopez
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/IngMarcosLopez/NetSuite-Connector
-Project-URL: Bug Tracker, https://github.com/IngMarcosLopez/NetSuite-Connector/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# NetSuite-Connector
-
-## Installation
-
-Only Restlet support:
-
-    $ pip install NetSuite-Connector
-## Get Started
-The following examples shows how to use this module.
-
-### RESTlet GET
-```python
-from NetSuite_Connector.NetSuite import NetSuite
-nt = NetSuite(
-    account_id=123456,
-    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
-    token_keys=dict(token_id="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
-)
-
-x = nt.get(
-    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
-    headers={"Content-Type": "application/json"},
-    params={}
-)
-print(x)
-# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, response='{"foo":"bar"}', code=200)
-```
-### RESTlet PUT - POST - DELETE
-```python
-from NetSuite_Connector.NetSuite import NetSuite
-nt = NetSuite(
-    account_id=123456,
-    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
-    token_keys=dict(token_id="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
-)
-body={"foo":"bar"}
-x = nt.post(
-    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
-    headers={"Content-Type": "application/json"},
-    params={},
-    body=body
-)
-print(x)
-# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
-```
-# ODBC Queries
-
-Connector only supports ODBC Driver queries, JDBC is not supported
-## Get Started
-
-Before you begin install [ODBC Driver](https://system.netsuite.com/app/help/helpcenter.nl?fid=book_N748613.html).
-
-Note that Support for NetSuite2.com is supported, which means that Only roles that hat not activated 2FA are supported. Also note that role must have permission to SuiteAnalitics.
-
-### ODBC Query
-
-```python
-from NetSuite_Connector.ODBC import ODBC
-
-nt = ODBC(
-    account_id="*****",
-    user_email="*****",
-    role_id="*****",
-    dsn="*****",
-    password="*****"
-)
-q = nt.query("SELECT * FROM OA_tables")
-print(q.status)
-# 200
-print(q.response)
-#[{"foo":"bar"}]
-print(q.data_received)
-# SELECT * FROM OA_tables
-print(q.columns)
-# ["foo"]
-```
-
-
-## TODO
-
-- Add TBA for ODBC connector support
+Metadata-Version: 2.1
+Name: NetSuite-Connector
+Version: 0.3.0
+Summary: NetSuite Connector
+Author-email: Marcos Lopez <merick16@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Marcos Lopez
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/IngMarcosLopez/NetSuite-Connector
+Project-URL: Bug Tracker, https://github.com/IngMarcosLopez/NetSuite-Connector/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# NetSuite-Connector
+
+## Supports
+
+- [SuiteTalk REST Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_1559132836.html)
+- [Restlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799403.html#Related-Support-Articles)
+
+## Installation
+
+    $ pip install NetSuite-Connector
+
+## Get Started
+
+The following examples shows how to use this module.
+
+### RESTlet GET
+
+```python
+from NetSuite_Connector.NetSuite import NetSuite
+nt = NetSuite(
+    account_id=123456,
+    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
+    token_keys=dict(token_key="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
+)
+
+x = nt.get(
+    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
+    headers={"Content-Type": "application/json"},
+    params={"foo":"bar"}
+)
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, response='{"foo":"bar"}', code=200)
+```
+
+### RESTlet PUT - POST - DELETE
+
+```python
+from NetSuite_Connector.NetSuite import NetSuite
+nt = NetSuite(
+    account_id=123456,
+    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
+    token_keys=dict(token_key="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
+)
+body={"foo":"bar"}
+x = nt.post(
+    url="https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx",
+    headers={"Content-Type": "application/json"},
+    params={},
+    body=body
+)
+print(x)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
+```
+
+# SuiteQL Queries
+
+To execute SuiteQL queries through REST web services, send a POST request to the `suiteql` resource, and specify the query in the request body after the query parameter `q`. The following example shows a SuiteQL query executed through REST web services.
+
+### SuiteQL Query
+
+```python
+from NetSuite_Connector.ODBC import ODBC
+
+nt = ODBC(
+    account_id=123456,
+    consumer_keys=dict(consumer_key="2345678", consumer_secret="3456yhg"),
+    token_keys=dict(token_key="wfdbfdsdfg", token_secret="efguhfjoidejhfije"),
+)
+q = nt.query("SELECT top 10 * FROM transaction")
+print(q)
+# NetsuiteObject(url='https://xxxx.restlets.api.netsuite.com/app/site/hosting/restlet.nl?script=xxxx&deploy=xxxx', request_headers={'Content-Type': 'application/json'}, request_data={"foo":"bar"}, response='{"foo":"bar"}', code=200)
+```
```

