# Comparing `tmp/pulumi_kong-4.6.0a1713332908.tar.gz` & `tmp/pulumi_kong-4.6.0a1713561070.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kong-4.6.0a1713332908.tar", last modified: Wed Apr 17 05:59:32 2024, max compression
+gzip compressed data, was "pulumi_kong-4.6.0a1713561070.tar", last modified: Fri Apr 19 21:14:23 2024, max compression
```

## Comparing `pulumi_kong-4.6.0a1713332908.tar` & `pulumi_kong-4.6.0a1713561070.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:32.442613 pulumi_kong-4.6.0a1713332908/
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-17 05:59:32.442613 pulumi_kong-4.6.0a1713332908/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:32.442613 pulumi_kong-4.6.0a1713332908/pulumi_kong/
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16572 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:32.442613 pulumi_kong-4.6.0a1713332908/pulumi_kong/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11411 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13249 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    18822 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer_jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer_key_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    22500 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25586 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54876 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/route.py
--rw-r--r--   0 runner    (1001) docker     (127)    36357 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/target.py
--rw-r--r--   0 runner    (1001) docker     (127)    73196 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong/upstream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:59:32.442613 pulumi_kong-4.6.0a1713332908/pulumi_kong.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-17 05:59:32.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-17 05:59:32.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:59:32.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 05:59:32.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 05:59:32.000000 pulumi_kong-4.6.0a1713332908/pulumi_kong.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-17 05:59:26.000000 pulumi_kong-4.6.0a1713332908/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:59:32.442613 pulumi_kong-4.6.0a1713332908/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:23.109725 pulumi_kong-4.6.0a1713561070/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-19 21:14:23.109725 pulumi_kong-4.6.0a1713561070/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:23.105724 pulumi_kong-4.6.0a1713561070/pulumi_kong/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16572 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:23.105724 pulumi_kong-4.6.0a1713561070/pulumi_kong/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11411 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_key_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22656 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25984 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54868 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36457 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13150 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73268 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/upstream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:23.109725 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-19 21:14:23.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-19 21:14:23.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:14:23.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:14:23.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 21:14:23.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:14:23.109725 pulumi_kong-4.6.0a1713561070/setup.cfg
```

### Comparing `pulumi_kong-4.6.0a1713332908/PKG-INFO` & `pulumi_kong-4.6.0a1713561070/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kong
-Version: 4.6.0a1713332908
+Version: 4.6.0a1713561070
 Summary: A Pulumi package for creating and managing Kong resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kong
 Keywords: pulumi,kong
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kong-4.6.0a1713332908/README.md` & `pulumi_kong-4.6.0a1713561070/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/__init__.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/_inputs.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/_utilities.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/certificate.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/config/__init__.pyi` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/config/vars.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,17 +141,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         consumer = kong.Consumer("consumer",
+            username="User1",
             custom_id="123",
-            tags=["mySuperTag"],
-            username="User1")
+            tags=["mySuperTag"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a consumer:
 
@@ -180,17 +180,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         consumer = kong.Consumer("consumer",
+            username="User1",
             custom_id="123",
-            tags=["mySuperTag"],
-            username="User1")
+            tags=["mySuperTag"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a consumer:
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer_acl.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_acl.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,23 +138,24 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        my_consumer = kong.Consumer("myConsumer",
-            custom_id="123",
-            username="User1")
-        acl_plugin = kong.Plugin("aclPlugin", config_json=\"\"\"	{
+        my_consumer = kong.Consumer("my_consumer",
+            username="User1",
+            custom_id="123")
+        acl_plugin = kong.Plugin("acl_plugin",
+            name="acl",
+            config_json=\"\"\"	{
         		"allow": ["group1", "group2"]
         	}
-
         \"\"\")
-        consumer_acl = kong.ConsumerAcl("consumerAcl",
+        consumer_acl = kong.ConsumerAcl("consumer_acl",
             consumer_id=my_consumer.id,
             group="group2",
             tags=[
                 "myTag",
                 "otherTag",
             ])
         ```
@@ -180,23 +181,24 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        my_consumer = kong.Consumer("myConsumer",
-            custom_id="123",
-            username="User1")
-        acl_plugin = kong.Plugin("aclPlugin", config_json=\"\"\"	{
+        my_consumer = kong.Consumer("my_consumer",
+            username="User1",
+            custom_id="123")
+        acl_plugin = kong.Plugin("acl_plugin",
+            name="acl",
+            config_json=\"\"\"	{
         		"allow": ["group1", "group2"]
         	}
-
         \"\"\")
-        consumer_acl = kong.ConsumerAcl("consumerAcl",
+        consumer_acl = kong.ConsumerAcl("consumer_acl",
             consumer_id=my_consumer.id,
             group="group2",
             tags=[
                 "myTag",
                 "otherTag",
             ])
         ```
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer_basic_auth.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_basic_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,26 +170,26 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        my_consumer = kong.Consumer("myConsumer",
-            custom_id="123",
-            username="User1")
-        basic_auth_plugin = kong.Plugin("basicAuthPlugin")
-        consumer_basic_auth = kong.ConsumerBasicAuth("consumerBasicAuth",
+        my_consumer = kong.Consumer("my_consumer",
+            username="User1",
+            custom_id="123")
+        basic_auth_plugin = kong.Plugin("basic_auth_plugin", name="basic-auth")
+        consumer_basic_auth = kong.ConsumerBasicAuth("consumer_basic_auth",
             consumer_id=my_consumer.id,
+            username="foo_updated",
             password="bar_updated",
             tags=[
                 "myTag",
                 "anotherTag",
-            ],
-            username="foo_updated")
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] consumer_id: the id of the consumer to be configured with basic auth
         :param pulumi.Input[str] password: password to be used for basic auth
@@ -210,26 +210,26 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        my_consumer = kong.Consumer("myConsumer",
-            custom_id="123",
-            username="User1")
-        basic_auth_plugin = kong.Plugin("basicAuthPlugin")
-        consumer_basic_auth = kong.ConsumerBasicAuth("consumerBasicAuth",
+        my_consumer = kong.Consumer("my_consumer",
+            username="User1",
+            custom_id="123")
+        basic_auth_plugin = kong.Plugin("basic_auth_plugin", name="basic-auth")
+        consumer_basic_auth = kong.ConsumerBasicAuth("consumer_basic_auth",
             consumer_id=my_consumer.id,
+            username="foo_updated",
             password="bar_updated",
             tags=[
                 "myTag",
                 "anotherTag",
-            ],
-            username="foo_updated")
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ConsumerBasicAuthArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer_jwt_auth.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_jwt_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,25 +237,26 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        my_consumer = kong.Consumer("myConsumer",
-            custom_id="123",
-            username="User1")
-        jwt_plugin = kong.Plugin("jwtPlugin", config_json=\"\"\"	{
+        my_consumer = kong.Consumer("my_consumer",
+            username="User1",
+            custom_id="123")
+        jwt_plugin = kong.Plugin("jwt_plugin",
+            name="jwt",
+            config_json=\"\"\"	{
         		"claims_to_verify": ["exp"]
         	}
-
         \"\"\")
-        consumer_jwt_config = kong.ConsumerJwtAuth("consumerJwtConfig",
-            algorithm="HS256",
+        consumer_jwt_config = kong.ConsumerJwtAuth("consumer_jwt_config",
             consumer_id=my_consumer.id,
+            algorithm="HS256",
             key="my_key",
             rsa_public_key="foo",
             secret="my_secret")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
@@ -281,25 +282,26 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        my_consumer = kong.Consumer("myConsumer",
-            custom_id="123",
-            username="User1")
-        jwt_plugin = kong.Plugin("jwtPlugin", config_json=\"\"\"	{
+        my_consumer = kong.Consumer("my_consumer",
+            username="User1",
+            custom_id="123")
+        jwt_plugin = kong.Plugin("jwt_plugin",
+            name="jwt",
+            config_json=\"\"\"	{
         		"claims_to_verify": ["exp"]
         	}
-
         \"\"\")
-        consumer_jwt_config = kong.ConsumerJwtAuth("consumerJwtConfig",
-            algorithm="HS256",
+        consumer_jwt_config = kong.ConsumerJwtAuth("consumer_jwt_config",
             consumer_id=my_consumer.id,
+            algorithm="HS256",
             key="my_key",
             rsa_public_key="foo",
             secret="my_secret")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer_key_auth.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_key_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,19 +139,19 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        my_consumer = kong.Consumer("myConsumer",
+        my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
-        key_auth_plugin = kong.Plugin("keyAuthPlugin")
-        consumer_key_auth = kong.ConsumerKeyAuth("consumerKeyAuth",
+        key_auth_plugin = kong.Plugin("key_auth_plugin", name="key-auth")
+        consumer_key_auth = kong.ConsumerKeyAuth("consumer_key_auth",
             consumer_id=my_consumer.id,
             key="secret",
             tags=[
                 "myTag",
                 "anotherTag",
             ])
         ```
@@ -177,19 +177,19 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        my_consumer = kong.Consumer("myConsumer",
+        my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
-        key_auth_plugin = kong.Plugin("keyAuthPlugin")
-        consumer_key_auth = kong.ConsumerKeyAuth("consumerKeyAuth",
+        key_auth_plugin = kong.Plugin("key_auth_plugin", name="key-auth")
+        consumer_key_auth = kong.ConsumerKeyAuth("consumer_key_auth",
             consumer_id=my_consumer.id,
             key="secret",
             tags=[
                 "myTag",
                 "anotherTag",
             ])
         ```
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/consumer_oauth2.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,30 +270,32 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        my_consumer = kong.Consumer("myConsumer",
-            custom_id="123",
-            username="User1")
-        oauth2_plugin = kong.Plugin("oauth2Plugin", config_json=\"\"\"	{
+        my_consumer = kong.Consumer("my_consumer",
+            username="User1",
+            custom_id="123")
+        oauth2_plugin = kong.Plugin("oauth2_plugin",
+            name="oauth2",
+            config_json=\"\"\"	{
         		"global_credentials": true,
         		"enable_password_grant": true,
         		"token_expiration": 180,
         		"refresh_token_ttl": 180,
         		"provision_key": "testprovisionkey"
         	}
-
         \"\"\")
-        consumer_oauth2 = kong.ConsumerOauth2("consumerOauth2",
+        consumer_oauth2 = kong.ConsumerOauth2("consumer_oauth2",
+            name="test_application",
+            consumer_id=my_consumer.id,
             client_id="client_id",
             client_secret="client_secret",
-            consumer_id=my_consumer.id,
             redirect_uris=[
                 "https://asdf.com/callback",
                 "https://test.cl/callback",
             ],
             tags=["myTag"])
         ```
         <!--End PulumiCodeChooser -->
@@ -322,30 +324,32 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        my_consumer = kong.Consumer("myConsumer",
-            custom_id="123",
-            username="User1")
-        oauth2_plugin = kong.Plugin("oauth2Plugin", config_json=\"\"\"	{
+        my_consumer = kong.Consumer("my_consumer",
+            username="User1",
+            custom_id="123")
+        oauth2_plugin = kong.Plugin("oauth2_plugin",
+            name="oauth2",
+            config_json=\"\"\"	{
         		"global_credentials": true,
         		"enable_password_grant": true,
         		"token_expiration": 180,
         		"refresh_token_ttl": 180,
         		"provision_key": "testprovisionkey"
         	}
-
         \"\"\")
-        consumer_oauth2 = kong.ConsumerOauth2("consumerOauth2",
+        consumer_oauth2 = kong.ConsumerOauth2("consumer_oauth2",
+            name="test_application",
+            consumer_id=my_consumer.id,
             client_id="client_id",
             client_secret="client_secret",
-            consumer_id=my_consumer.id,
             redirect_uris=[
                 "https://asdf.com/callback",
                 "https://test.cl/callback",
             ],
             tags=["myTag"])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/outputs.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/plugin.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,83 +306,86 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        rate_limit = kong.Plugin("rateLimit", config_json=\"\"\"	{
+        rate_limit = kong.Plugin("rate_limit",
+            name="rate-limiting",
+            config_json=\"\"\"	{
         		"second": 5,
         		"hour" : 1000
         	}
-
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
         To apply a plugin to a consumer use the `consumer_id` property, for example:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        plugin_consumer = kong.Consumer("pluginConsumer",
-            custom_id="567",
-            username="PluginUser")
-        rate_limit = kong.Plugin("rateLimit",
+        plugin_consumer = kong.Consumer("plugin_consumer",
+            username="PluginUser",
+            custom_id="567")
+        rate_limit = kong.Plugin("rate_limit",
+            name="rate-limiting",
+            consumer_id=plugin_consumer.id,
             config_json=\"\"\"	{
         		"second": 5,
         		"hour" : 1000
         	}
-
-        \"\"\",
-            consumer_id=plugin_consumer.id)
+        \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         To apply a plugin to a service use the `service_id` property, for example:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
-            host="test.org",
-            protocol="http")
-        rate_limit = kong.Plugin("rateLimit",
+            name="test",
+            protocol="http",
+            host="test.org")
+        rate_limit = kong.Plugin("rate_limit",
+            name="rate-limiting",
+            service_id=service.id,
             config_json=\"\"\"	{
         		"second": 10,
         		"hour" : 2000
         	}
-
-        \"\"\",
-            service_id=service.id)
+        \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         To apply a plugin to a route use the `route_id` property, for example:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
-            host="test.org",
-            protocol="http")
-        rate_limit = kong.Plugin("rateLimit",
+            name="test",
+            protocol="http",
+            host="test.org")
+        rate_limit = kong.Plugin("rate_limit",
+            name="rate-limiting",
+            enabled=True,
+            service_id=service.id,
             config_json=\"\"\"	{
         		"second": 11,
         		"hour" : 4000
         	}
-
-        \"\"\",
-            enabled=True,
-            service_id=service.id)
+        \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a plugin:
 
@@ -415,83 +418,86 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        rate_limit = kong.Plugin("rateLimit", config_json=\"\"\"	{
+        rate_limit = kong.Plugin("rate_limit",
+            name="rate-limiting",
+            config_json=\"\"\"	{
         		"second": 5,
         		"hour" : 1000
         	}
-
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
         To apply a plugin to a consumer use the `consumer_id` property, for example:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
-        plugin_consumer = kong.Consumer("pluginConsumer",
-            custom_id="567",
-            username="PluginUser")
-        rate_limit = kong.Plugin("rateLimit",
+        plugin_consumer = kong.Consumer("plugin_consumer",
+            username="PluginUser",
+            custom_id="567")
+        rate_limit = kong.Plugin("rate_limit",
+            name="rate-limiting",
+            consumer_id=plugin_consumer.id,
             config_json=\"\"\"	{
         		"second": 5,
         		"hour" : 1000
         	}
-
-        \"\"\",
-            consumer_id=plugin_consumer.id)
+        \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         To apply a plugin to a service use the `service_id` property, for example:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
-            host="test.org",
-            protocol="http")
-        rate_limit = kong.Plugin("rateLimit",
+            name="test",
+            protocol="http",
+            host="test.org")
+        rate_limit = kong.Plugin("rate_limit",
+            name="rate-limiting",
+            service_id=service.id,
             config_json=\"\"\"	{
         		"second": 10,
         		"hour" : 2000
         	}
-
-        \"\"\",
-            service_id=service.id)
+        \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         To apply a plugin to a route use the `route_id` property, for example:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
-            host="test.org",
-            protocol="http")
-        rate_limit = kong.Plugin("rateLimit",
+            name="test",
+            protocol="http",
+            host="test.org")
+        rate_limit = kong.Plugin("rate_limit",
+            name="rate-limiting",
+            enabled=True,
+            service_id=service.id,
             config_json=\"\"\"	{
         		"second": 11,
         		"hour" : 4000
         	}
-
-        \"\"\",
-            enabled=True,
-            service_id=service.id)
+        \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a plugin:
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/provider.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/route.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -638,28 +638,29 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         route = kong.Route("route",
+            name="MyRoute",
             protocols=[
                 "http",
                 "https",
             ],
             methods=[
                 "GET",
                 "POST",
             ],
             hosts=["example2.com"],
             paths=["/test"],
             strip_path=False,
             preserve_host=True,
             regex_priority=1,
-            service_id=kong_service["service"]["id"],
+            service_id=service["id"],
             headers=[kong.RouteHeaderArgs(
                 name="x-test-1",
                 values=[
                     "a",
                     "b",
                 ],
             )])
@@ -687,15 +688,15 @@
                 ),
             ],
             destinations=[kong.RouteDestinationArgs(
                 ip="172.10.1.1",
                 port=81,
             )],
             snis=["foo.com"],
-            service_id=kong_service["service"]["id"])
+            service_id=service["id"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a route:
 
@@ -741,28 +742,29 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         route = kong.Route("route",
+            name="MyRoute",
             protocols=[
                 "http",
                 "https",
             ],
             methods=[
                 "GET",
                 "POST",
             ],
             hosts=["example2.com"],
             paths=["/test"],
             strip_path=False,
             preserve_host=True,
             regex_priority=1,
-            service_id=kong_service["service"]["id"],
+            service_id=service["id"],
             headers=[kong.RouteHeaderArgs(
                 name="x-test-1",
                 values=[
                     "a",
                     "b",
                 ],
             )])
@@ -790,15 +792,15 @@
                 ),
             ],
             destinations=[kong.RouteDestinationArgs(
                 ip="172.10.1.1",
                 port=81,
             )],
             snis=["foo.com"],
-            service_id=kong_service["service"]["id"])
+            service_id=service["id"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a route:
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/service.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,22 +503,23 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
-            connect_timeout=1000,
+            name="test",
+            protocol="http",
             host="test.org",
-            path="/mypath",
             port=8080,
-            protocol="http",
-            read_timeout=3000,
+            path="/mypath",
             retries=5,
-            write_timeout=2000)
+            connect_timeout=1000,
+            write_timeout=2000,
+            read_timeout=3000)
         ```
         <!--End PulumiCodeChooser -->
 
         To use a client certificate and ca certificates combine with certificate resource (note protocol must be `https`):
 
         <!--Start PulumiCodeChooser -->
         ```python
@@ -542,14 +543,15 @@
         \"\"\",
             private_key=\"\"\"    -----BEGIN PRIVATE KEY-----
             .....
             -----END PRIVATE KEY-----
         \"\"\",
             snis=["ca.com"])
         service = kong.Service("service",
+            name="test",
             protocol="https",
             host="test.org",
             tls_verify=True,
             tls_verify_depth=2,
             client_certificate_id=certificate.id,
             ca_certificate_ids=[ca.id])
         ```
@@ -595,22 +597,23 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
-            connect_timeout=1000,
+            name="test",
+            protocol="http",
             host="test.org",
-            path="/mypath",
             port=8080,
-            protocol="http",
-            read_timeout=3000,
+            path="/mypath",
             retries=5,
-            write_timeout=2000)
+            connect_timeout=1000,
+            write_timeout=2000,
+            read_timeout=3000)
         ```
         <!--End PulumiCodeChooser -->
 
         To use a client certificate and ca certificates combine with certificate resource (note protocol must be `https`):
 
         <!--Start PulumiCodeChooser -->
         ```python
@@ -634,14 +637,15 @@
         \"\"\",
             private_key=\"\"\"    -----BEGIN PRIVATE KEY-----
             .....
             -----END PRIVATE KEY-----
         \"\"\",
             snis=["ca.com"])
         service = kong.Service("service",
+            name="test",
             protocol="https",
             host="test.org",
             tls_verify=True,
             tls_verify_depth=2,
             client_certificate_id=certificate.id,
             ca_certificate_ids=[ca.id])
         ```
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/target.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/target.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,16 +168,16 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         target = kong.Target("target",
             target="sample_target:80",
-            upstream_id=kong_upstream["upstream"]["id"],
-            weight=10)
+            weight=10,
+            upstream_id=upstream["id"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a target use a combination of the upstream id and the target id as follows:
 
@@ -204,16 +204,16 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         target = kong.Target("target",
             target="sample_target:80",
-            upstream_id=kong_upstream["upstream"]["id"],
-            weight=10)
+            weight=10,
+            upstream_id=upstream["id"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a target use a combination of the upstream id and the target id as follows:
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong/upstream.py` & `pulumi_kong-4.6.0a1713561070/pulumi_kong/upstream.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,14 +522,15 @@
         \"\"\",
             private_key=\"\"\"    -----BEGIN PRIVATE KEY-----
             .....
             -----END PRIVATE KEY-----
         \"\"\",
             snis=["foo.com"])
         upstream = kong.Upstream("upstream",
+            name="sample_upstream",
             slots=10,
             hash_on="header",
             hash_fallback="cookie",
             hash_on_header="HeaderName",
             hash_fallback_header="FallbackHeaderName",
             hash_on_cookie="CookieName",
             hash_on_cookie_path="/path",
@@ -655,14 +656,15 @@
         \"\"\",
             private_key=\"\"\"    -----BEGIN PRIVATE KEY-----
             .....
             -----END PRIVATE KEY-----
         \"\"\",
             snis=["foo.com"])
         upstream = kong.Upstream("upstream",
+            name="sample_upstream",
             slots=10,
             hash_on="header",
             hash_fallback="cookie",
             hash_on_header="HeaderName",
             hash_fallback_header="FallbackHeaderName",
             hash_on_cookie="CookieName",
             hash_on_cookie_path="/path",
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong.egg-info/PKG-INFO` & `pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kong
-Version: 4.6.0a1713332908
+Version: 4.6.0a1713561070
 Summary: A Pulumi package for creating and managing Kong resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kong
 Keywords: pulumi,kong
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kong-4.6.0a1713332908/pulumi_kong.egg-info/SOURCES.txt` & `pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713332908/pyproject.toml` & `pulumi_kong-4.6.0a1713561070/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kong"
   description = "A Pulumi package for creating and managing Kong resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "kong"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "4.6.0a1713332908"
+  version = "4.6.0a1713561070"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-kong"
 
 [build-system]
```

