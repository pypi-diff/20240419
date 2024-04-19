# Comparing `tmp/zvolv_sdk-0.0.2.tar.gz` & `tmp/zvolv_sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zvolv_sdk-0.0.2.tar", last modified: Mon Feb 27 06:18:54 2023, max compression
+gzip compressed data, was "zvolv_sdk-0.0.4.tar", last modified: Fri Apr 19 05:22:39 2024, max compression
```

## Comparing `zvolv_sdk-0.0.2.tar` & `zvolv_sdk-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,30 @@
-drwxr-xr-x   0 akshay-mac   (501) staff       (20)        0 2023-02-27 06:18:54.325573 zvolv_sdk-0.0.2/
--rw-r--r--   0 akshay-mac   (501) staff       (20)     1065 2023-02-15 12:21:54.000000 zvolv_sdk-0.0.2/LICENSE
--rw-r--r--   0 akshay-mac   (501) staff       (20)     5265 2023-02-27 06:18:54.325636 zvolv_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 akshay-mac   (501) staff       (20)     4228 2023-02-27 05:49:18.000000 zvolv_sdk-0.0.2/README.md
--rw-r--r--   0 akshay-mac   (501) staff       (20)       79 2023-02-27 06:18:54.325843 zvolv_sdk-0.0.2/setup.cfg
--rw-r--r--   0 akshay-mac   (501) staff       (20)     1564 2023-02-27 05:18:44.000000 zvolv_sdk-0.0.2/setup.py
-drwxr-xr-x   0 akshay-mac   (501) staff       (20)        0 2023-02-27 06:18:54.324545 zvolv_sdk-0.0.2/tests/
--rw-r--r--   0 akshay-mac   (501) staff       (20)        0 2023-02-25 13:29:39.000000 zvolv_sdk-0.0.2/tests/__init__.py
--rw-r--r--   0 akshay-mac   (501) staff       (20)      194 2023-02-25 13:48:28.000000 zvolv_sdk-0.0.2/tests/test_divide_by_three.py
-drwxr-xr-x   0 akshay-mac   (501) staff       (20)        0 2023-02-27 06:18:54.324964 zvolv_sdk-0.0.2/zvolv_sdk/
--rw-r--r--   0 akshay-mac   (501) staff       (20)        0 2023-02-27 05:18:28.000000 zvolv_sdk-0.0.2/zvolv_sdk/__init__.py
--rw-r--r--   0 akshay-mac   (501) staff       (20)       41 2023-02-25 13:46:47.000000 zvolv_sdk-0.0.2/zvolv_sdk/divide_by_three.py
--rw-r--r--   0 akshay-mac   (501) staff       (20)       91 2023-02-27 06:17:42.000000 zvolv_sdk-0.0.2/zvolv_sdk/version.py
-drwxr-xr-x   0 akshay-mac   (501) staff       (20)        0 2023-02-27 06:18:54.325462 zvolv_sdk-0.0.2/zvolv_sdk.egg-info/
--rw-r--r--   0 akshay-mac   (501) staff       (20)     5265 2023-02-27 06:18:54.000000 zvolv_sdk-0.0.2/zvolv_sdk.egg-info/PKG-INFO
--rw-r--r--   0 akshay-mac   (501) staff       (20)      288 2023-02-27 06:18:54.000000 zvolv_sdk-0.0.2/zvolv_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 akshay-mac   (501) staff       (20)        1 2023-02-27 06:18:54.000000 zvolv_sdk-0.0.2/zvolv_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 akshay-mac   (501) staff       (20)       16 2023-02-27 06:18:54.000000 zvolv_sdk-0.0.2/zvolv_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.222741 zvolv_sdk-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.222741 zvolv_sdk-0.0.4/src/devide/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/src/devide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/src/devide/divide_by_three.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/src/zvolv_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/src/zvolv_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/src/zvolv_client/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/tests/test_divide_by_three.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/zvolv_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/common_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/server_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/user_defined_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 05:22:28.000000 zvolv_sdk-0.0.4/zvolv_sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:22:39.226741 zvolv_sdk-0.0.4/zvolv_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 05:22:39.000000 zvolv_sdk-0.0.4/zvolv_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-19 05:22:39.000000 zvolv_sdk-0.0.4/zvolv_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:22:39.000000 zvolv_sdk-0.0.4/zvolv_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 05:22:39.000000 zvolv_sdk-0.0.4/zvolv_sdk.egg-info/top_level.txt
```

### Comparing `zvolv_sdk-0.0.2/LICENSE` & `zvolv_sdk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.2/PKG-INFO` & `zvolv_sdk-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zvolv_sdk
-Version: 0.0.2
+Version: 0.0.4
 Summary: The Zvolv API Platform SDK for Python
 Home-page: https://github.com/zvolvapi/python-zvolv-sdk
 Download-URL: https://github.com/zvolvapi/python-zvolv-sdk/archive/v_01.tar.gz
 Author: Akshay Jadhav
 Author-email: support@zvolv.com
 License: MIT
 Keywords: zvolv,zvolv-api,web-api,sdk,rest-api-client
@@ -20,37 +20,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Auth0 SDK for Python](https://cdn.auth0.com/website/sdks/banners/auth0-python-banner.png)
-
-![Release](https://img.shields.io/pypi/v/auth0-python)
-![Downloads](https://img.shields.io/pypi/dw/auth0-python)
-[![License](https://img.shields.io/:license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
+# ZvolvClient SDK
 
 <div>
 📚 <a href="#documentation">Documentation</a> - 🚀 <a href="#getting-started">Getting started</a> - 💻 <a href="#api-reference">API reference</a> - 💬 <a href="#feedback">Feedback</a>
 </div>
 
 
 Learn how to automate with Zvolv using Python.
 ## Documentation
-- [Docs site](https://www.zvolv.com/docs) - explore our docs site and learn more about Zvolv.
+- [Docs site](https://python-zvolv-sdk.readthedocs.io/) - explore our docs site and learn more about Zvolv.
+- [User Guide](https://github.com/zvolvapi/python-zvolv-sdk/blob/main/UserGuide.md) - explore our user guide docs and learn more about sdk.
 
 ## Getting started
 ### Installation
-You can install the auth0 Python SDK using the following command.
+You can install the Zvolv Python SDK using the following command.
 ```
-pip install zvolv_sdk
+pip install zvolv-sdk
 ```
 
-> Requires Python 3.7 or higher.
+> Requires Python 3.0 or higher.
 
 ### Usage
 The Zvolv Hyper automation platform offers several APIs to build apps. Each Zvolv API delivers part of the capabilities from the platform, so that you can pick just those that fit for your needs. This SDK offers a corresponding package for each of Zvolv’s APIs.
 
 #### Sending an email from Zvolv
 
 One of the most simple use-cases is sending an email from Zvolv. In our examples, we specify the channel name, however it is recommended to use the `channel_id` where possible. Also, if your app's bot user is not in a channel yet, invite the bot user before running the code snippet (or add `chat:write.public` to Bot Token Scopes for posting in any public channels).
@@ -70,33 +67,26 @@
     assert e.response["ok"] is False
     assert e.response["error"]  # str like 'invalid_auth', 'channel_not_found'
     print(f"Got an error: {e.response['error']}")
 ```
 
 Here we also ensure that the response back from Zvolv is a successful one and that the message is the one we sent by using the `assert` statement.
 
-### Authentication Endpoints
+### API References
 
 - Database ( `authentication.Database` )
 - Delegated ( `authentication.Delegated` )
 - Enterprise ( `authentication.Enterprise` )
 - API Authorization - Get Token ( `authentication.GetToken`)
 - Passwordless ( `authentication.Passwordless` )
 - RevokeToken ( `authentication.RevokeToken` )
 - Social ( `authentication.Social` )
 - Users ( `authentication.Users` )
 
 
-### Management Endpoints
-
-- Actions() (`Zvolv().action`)
-- AttackProtection() (`Zvolv().attack_protection`)
-- Blacklists() ( `Zvolv().blacklists` )
-- Branding() ( `Zvolv().branding` )
-
 
 ### Feedback
 
 ---
 
 If you get stuck, we’re here to help. The following are the best ways to get assistance working through your issue:
```

### Comparing `zvolv_sdk-0.0.2/README.md` & `zvolv_sdk-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-![Auth0 SDK for Python](https://cdn.auth0.com/website/sdks/banners/auth0-python-banner.png)
-
-![Release](https://img.shields.io/pypi/v/auth0-python)
-![Downloads](https://img.shields.io/pypi/dw/auth0-python)
-[![License](https://img.shields.io/:license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
+# ZvolvClient SDK
 
 <div>
 📚 <a href="#documentation">Documentation</a> - 🚀 <a href="#getting-started">Getting started</a> - 💻 <a href="#api-reference">API reference</a> - 💬 <a href="#feedback">Feedback</a>
 </div>
 
 
 Learn how to automate with Zvolv using Python.
 ## Documentation
-- [Docs site](https://www.zvolv.com/docs) - explore our docs site and learn more about Zvolv.
+- [Docs site](https://python-zvolv-sdk.readthedocs.io/) - explore our docs site and learn more about Zvolv.
+- [User Guide](https://github.com/zvolvapi/python-zvolv-sdk/blob/main/UserGuide.md) - explore our user guide docs and learn more about sdk.
 
 ## Getting started
 ### Installation
-You can install the auth0 Python SDK using the following command.
+You can install the Zvolv Python SDK using the following command.
 ```
-pip install zvolv_sdk
+pip install zvolv-sdk
 ```
 
-> Requires Python 3.7 or higher.
+> Requires Python 3.0 or higher.
 
 ### Usage
 The Zvolv Hyper automation platform offers several APIs to build apps. Each Zvolv API delivers part of the capabilities from the platform, so that you can pick just those that fit for your needs. This SDK offers a corresponding package for each of Zvolv’s APIs.
 
 #### Sending an email from Zvolv
 
 One of the most simple use-cases is sending an email from Zvolv. In our examples, we specify the channel name, however it is recommended to use the `channel_id` where possible. Also, if your app's bot user is not in a channel yet, invite the bot user before running the code snippet (or add `chat:write.public` to Bot Token Scopes for posting in any public channels).
@@ -44,33 +41,26 @@
     assert e.response["ok"] is False
     assert e.response["error"]  # str like 'invalid_auth', 'channel_not_found'
     print(f"Got an error: {e.response['error']}")
 ```
 
 Here we also ensure that the response back from Zvolv is a successful one and that the message is the one we sent by using the `assert` statement.
 
-### Authentication Endpoints
+### API References
 
 - Database ( `authentication.Database` )
 - Delegated ( `authentication.Delegated` )
 - Enterprise ( `authentication.Enterprise` )
 - API Authorization - Get Token ( `authentication.GetToken`)
 - Passwordless ( `authentication.Passwordless` )
 - RevokeToken ( `authentication.RevokeToken` )
 - Social ( `authentication.Social` )
 - Users ( `authentication.Users` )
 
 
-### Management Endpoints
-
-- Actions() (`Zvolv().action`)
-- AttackProtection() (`Zvolv().attack_protection`)
-- Blacklists() ( `Zvolv().blacklists` )
-- Branding() ( `Zvolv().branding` )
-
 
 ### Feedback
 
 ---
 
 If you get stuck, we’re here to help. The following are the best ways to get assistance working through your issue:
```

### Comparing `zvolv_sdk-0.0.2/setup.py` & `zvolv_sdk-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `zvolv_sdk-0.0.2/zvolv_sdk.egg-info/PKG-INFO` & `zvolv_sdk-0.0.4/zvolv_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zvolv-sdk
-Version: 0.0.2
+Name: zvolv_sdk
+Version: 0.0.4
 Summary: The Zvolv API Platform SDK for Python
 Home-page: https://github.com/zvolvapi/python-zvolv-sdk
 Download-URL: https://github.com/zvolvapi/python-zvolv-sdk/archive/v_01.tar.gz
 Author: Akshay Jadhav
 Author-email: support@zvolv.com
 License: MIT
 Keywords: zvolv,zvolv-api,web-api,sdk,rest-api-client
@@ -20,37 +20,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Auth0 SDK for Python](https://cdn.auth0.com/website/sdks/banners/auth0-python-banner.png)
-
-![Release](https://img.shields.io/pypi/v/auth0-python)
-![Downloads](https://img.shields.io/pypi/dw/auth0-python)
-[![License](https://img.shields.io/:license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
+# ZvolvClient SDK
 
 <div>
 📚 <a href="#documentation">Documentation</a> - 🚀 <a href="#getting-started">Getting started</a> - 💻 <a href="#api-reference">API reference</a> - 💬 <a href="#feedback">Feedback</a>
 </div>
 
 
 Learn how to automate with Zvolv using Python.
 ## Documentation
-- [Docs site](https://www.zvolv.com/docs) - explore our docs site and learn more about Zvolv.
+- [Docs site](https://python-zvolv-sdk.readthedocs.io/) - explore our docs site and learn more about Zvolv.
+- [User Guide](https://github.com/zvolvapi/python-zvolv-sdk/blob/main/UserGuide.md) - explore our user guide docs and learn more about sdk.
 
 ## Getting started
 ### Installation
-You can install the auth0 Python SDK using the following command.
+You can install the Zvolv Python SDK using the following command.
 ```
-pip install zvolv_sdk
+pip install zvolv-sdk
 ```
 
-> Requires Python 3.7 or higher.
+> Requires Python 3.0 or higher.
 
 ### Usage
 The Zvolv Hyper automation platform offers several APIs to build apps. Each Zvolv API delivers part of the capabilities from the platform, so that you can pick just those that fit for your needs. This SDK offers a corresponding package for each of Zvolv’s APIs.
 
 #### Sending an email from Zvolv
 
 One of the most simple use-cases is sending an email from Zvolv. In our examples, we specify the channel name, however it is recommended to use the `channel_id` where possible. Also, if your app's bot user is not in a channel yet, invite the bot user before running the code snippet (or add `chat:write.public` to Bot Token Scopes for posting in any public channels).
@@ -70,33 +67,26 @@
     assert e.response["ok"] is False
     assert e.response["error"]  # str like 'invalid_auth', 'channel_not_found'
     print(f"Got an error: {e.response['error']}")
 ```
 
 Here we also ensure that the response back from Zvolv is a successful one and that the message is the one we sent by using the `assert` statement.
 
-### Authentication Endpoints
+### API References
 
 - Database ( `authentication.Database` )
 - Delegated ( `authentication.Delegated` )
 - Enterprise ( `authentication.Enterprise` )
 - API Authorization - Get Token ( `authentication.GetToken`)
 - Passwordless ( `authentication.Passwordless` )
 - RevokeToken ( `authentication.RevokeToken` )
 - Social ( `authentication.Social` )
 - Users ( `authentication.Users` )
 
 
-### Management Endpoints
-
-- Actions() (`Zvolv().action`)
-- AttackProtection() (`Zvolv().attack_protection`)
-- Blacklists() ( `Zvolv().blacklists` )
-- Branding() ( `Zvolv().branding` )
-
 
 ### Feedback
 
 ---
 
 If you get stuck, we’re here to help. The following are the best ways to get assistance working through your issue:
```

