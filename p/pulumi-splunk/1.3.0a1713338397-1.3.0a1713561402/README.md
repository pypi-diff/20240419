# Comparing `tmp/pulumi_splunk-1.3.0a1713338397.tar.gz` & `tmp/pulumi_splunk-1.3.0a1713561402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_splunk-1.3.0a1713338397.tar", last modified: Wed Apr 17 07:42:21 2024, max compression
+gzip compressed data, was "pulumi_splunk-1.3.0a1713561402.tar", last modified: Fri Apr 19 21:22:16 2024, max compression
```

## Comparing `pulumi_splunk-1.3.0a1713338397.tar` & `pulumi_splunk-1.3.0a1713561402.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:42:21.566026 pulumi_splunk-1.3.0a1713338397/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-17 07:42:21.566026 pulumi_splunk-1.3.0a1713338397/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:42:21.562026 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   148655 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/admin_saml_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    38756 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/apps_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    22001 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/authentication_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/authorization_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:42:21.566026 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/configs_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14457 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/data_ui_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/generic_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/global_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)   154940 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    42158 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    29999 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_tcp_cooked.py
--rw-r--r--   0 runner    (1001) docker     (127)    36720 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_tcp_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_tcp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    34349 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_udp.py
--rw-r--r--   0 runner    (1001) docker     (127)   127784 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44131 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/outputs_tcp_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    43577 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/outputs_tcp_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    32027 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/outputs_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    27963 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/outputs_tcp_syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   514567 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/saved_searches.py
--rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk/sh_indexes_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:42:21.566026 pulumi_splunk-1.3.0a1713338397/pulumi_splunk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-17 07:42:21.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-17 07:42:21.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:42:21.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 07:42:21.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 07:42:21.000000 pulumi_splunk-1.3.0a1713338397/pulumi_splunk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-17 07:42:15.000000 pulumi_splunk-1.3.0a1713338397/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:42:21.566026 pulumi_splunk-1.3.0a1713338397/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:16.216618 pulumi_splunk-1.3.0a1713561402/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-19 21:22:16.216618 pulumi_splunk-1.3.0a1713561402/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:16.212618 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148655 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/admin_saml_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38906 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/apps_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22055 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/authentication_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45992 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/authorization_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:16.216618 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/configs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/data_ui_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/generic_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/global_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   155006 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23938 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42272 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30131 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19073 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_cooked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36774 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34401 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127784 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44187 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43639 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32121 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28027 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   514639 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/saved_searches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/sh_indexes_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:16.216618 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-19 21:22:16.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-19 21:22:16.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:22:16.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 21:22:16.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 21:22:16.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:22:16.216618 pulumi_splunk-1.3.0a1713561402/setup.cfg
```

### Comparing `pulumi_splunk-1.3.0a1713338397/PKG-INFO` & `pulumi_splunk-1.3.0a1713561402/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1713338397
+Version: 1.3.0a1713561402
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi,splunk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_splunk-1.3.0a1713338397/README.md` & `pulumi_splunk-1.3.0a1713561402/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/__init__.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/_inputs.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/_utilities.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/admin_saml_groups.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/admin_saml_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,18 +107,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        saml_group = splunk.AdminSamlGroups("saml-group", roles=[
-            "admin",
-            "power",
-        ])
+        saml_group = splunk.AdminSamlGroups("saml-group",
+            name="mygroup",
+            roles=[
+                "admin",
+                "power",
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         SAML groups can be imported using the id, e.g.
 
@@ -145,18 +147,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        saml_group = splunk.AdminSamlGroups("saml-group", roles=[
-            "admin",
-            "power",
-        ])
+        saml_group = splunk.AdminSamlGroups("saml-group",
+            name="mygroup",
+            roles=[
+                "admin",
+                "power",
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         SAML groups can be imported using the id, e.g.
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/apps_local.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/apps_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -516,17 +516,18 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        amazon_connect_app = splunk.AppsLocal("amazonConnectApp",
-            explicit_appname="amazon_connect_app_for_splunk",
-            filename=True)
+        amazon_connect_app = splunk.AppsLocal("amazon_connect_app",
+            filename=True,
+            name="/usr/home/amazon_connect_app_for_splunk-0.0.1.tar.gz",
+            explicit_appname="amazon_connect_app_for_splunk")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['AppsLocalAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] auth: Splunkbase session token for operations like install and update that require login. Use auth or session when installing or updating an app through Splunkbase.
@@ -567,17 +568,18 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        amazon_connect_app = splunk.AppsLocal("amazonConnectApp",
-            explicit_appname="amazon_connect_app_for_splunk",
-            filename=True)
+        amazon_connect_app = splunk.AppsLocal("amazon_connect_app",
+            filename=True,
+            name="/usr/home/amazon_connect_app_for_splunk-0.0.1.tar.gz",
+            explicit_appname="amazon_connect_app_for_splunk")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AppsLocalArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/authentication_users.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/authentication_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,17 +339,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         user01 = splunk.AuthenticationUsers("user01",
+            name="user01",
             email="user01@example.com",
-            force_change_pass=False,
             password="password01",
+            force_change_pass=False,
             roles=["terraform-user01-role"])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_app: User default app. Overrides the default app inherited from the user roles.
@@ -377,17 +378,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         user01 = splunk.AuthenticationUsers("user01",
+            name="user01",
             email="user01@example.com",
-            force_change_pass=False,
             password="password01",
+            force_change_pass=False,
             roles=["terraform-user01-role"])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AuthenticationUsersArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/authorization_roles.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/authorization_roles.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,24 +471,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         role01 = splunk.AuthorizationRoles("role01",
-            capabilities=[
-                "accelerate_datamodel",
-                "change_authentication",
-                "restart_splunkd",
-            ],
+            name="terraform-user01-role",
             default_app="search",
             imported_roles=[
                 "power",
                 "user",
             ],
+            capabilities=[
+                "accelerate_datamodel",
+                "change_authentication",
+                "restart_splunkd",
+            ],
             search_indexes_alloweds=[
                 "_audit",
                 "_internal",
                 "main",
             ],
             search_indexes_defaults=[
                 "_audit",
@@ -529,24 +530,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         role01 = splunk.AuthorizationRoles("role01",
-            capabilities=[
-                "accelerate_datamodel",
-                "change_authentication",
-                "restart_splunkd",
-            ],
+            name="terraform-user01-role",
             default_app="search",
             imported_roles=[
                 "power",
                 "user",
             ],
+            capabilities=[
+                "accelerate_datamodel",
+                "change_authentication",
+                "restart_splunkd",
+            ],
             search_indexes_alloweds=[
                 "_audit",
                 "_internal",
                 "main",
             ],
             search_indexes_defaults=[
                 "_audit",
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/config/__init__.pyi` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/config/vars.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/configs_conf.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/configs_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,18 +134,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        new_conf_stanza = splunk.ConfigsConf("new-conf-stanza", variables={
-            "disabled": "false",
-            "custom_key": "value",
-        })
+        new_conf_stanza = splunk.ConfigsConf("new-conf-stanza",
+            name="custom-conf/custom",
+            variables={
+                "disabled": "false",
+                "custom_key": "value",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: A '/' separated string consisting of {conf_file_name}/{stanza_name} ex. props/custom_stanza
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] variables: A map of key value pairs for a stanza.
@@ -164,18 +166,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        new_conf_stanza = splunk.ConfigsConf("new-conf-stanza", variables={
-            "disabled": "false",
-            "custom_key": "value",
-        })
+        new_conf_stanza = splunk.ConfigsConf("new-conf-stanza",
+            name="custom-conf/custom",
+            variables={
+                "disabled": "false",
+                "custom_key": "value",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ConfigsConfArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/data_ui_views.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/data_ui_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,19 +137,20 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         dashboard = splunk.DataUiViews("dashboard",
+            name="Terraform_Sample_Dashboard",
+            eai_data="<dashboard version=\\"1.1\\"><label>Terraform</label><description>Terraform operations</description><row><panel><chart><search><query>index=_internal sourcetype=splunkd_access useragent=\\"splunk-simple-go-client\\" | timechart fixedrange=f values(status) by uri_path</query><earliest>-24h@h</earliest><latest>now</latest><sampleRatio>1</sampleRatio></search><option name=\\"charting.axisLabelsX.majorLabelStyle.overflowMode\\">ellipsisNone</option><option name=\\"charting.axisLabelsX.majorLabelStyle.rotation\\">0</option><option name=\\"charting.axisTitleX.visibility\\">collapsed</option><option name=\\"charting.axisTitleY.text\\">HTTP status codes</option><option name=\\"charting.axisTitleY.visibility\\">visible</option><option name=\\"charting.axisTitleY2.visibility\\">visible</option><option name=\\"charting.axisX.abbreviation\\">none</option><option name=\\"charting.axisX.scale\\">linear</option><option name=\\"charting.axisY.abbreviation\\">none</option><option name=\\"charting.axisY.scale\\">linear</option><option name=\\"charting.axisY2.abbreviation\\">none</option><option name=\\"charting.axisY2.enabled\\">0</option><option name=\\"charting.axisY2.scale\\">inherit</option><option name=\\"charting.chart\\">column</option><option name=\\"charting.chart.bubbleMaximumSize\\">50</option><option name=\\"charting.chart.bubbleMinimumSize\\">10</option><option name=\\"charting.chart.bubbleSizeBy\\">area</option><option name=\\"charting.chart.nullValueMode\\">connect</option><option name=\\"charting.chart.showDataLabels\\">none</option><option name=\\"charting.chart.sliceCollapsingThreshold\\">0.01</option><option name=\\"charting.chart.stackMode\\">default</option><option name=\\"charting.chart.style\\">shiny</option><option name=\\"charting.drilldown\\">none</option><option name=\\"charting.layout.splitSeries\\">0</option><option name=\\"charting.layout.splitSeries.allowIndependentYRanges\\">0</option><option name=\\"charting.legend.labelStyle.overflowMode\\">ellipsisMiddle</option><option name=\\"charting.legend.mode\\">standard</option><option name=\\"charting.legend.placement\\">right</option><option name=\\"charting.lineWidth\\">2</option><option name=\\"trellis.enabled\\">0</option><option name=\\"trellis.scales.shared\\">1</option><option name=\\"trellis.size\\">small</option><option name=\\"trellis.splitBy\\">_aggregation</option></chart></panel></row></dashboard>",
             acl=splunk.DataUiViewsAclArgs(
-                app="search",
                 owner="admin",
-            ),
-            eai_data="<dashboard version=\\"1.1\\"><label>Terraform</label><description>Terraform operations</description><row><panel><chart><search><query>index=_internal sourcetype=splunkd_access useragent=\\"splunk-simple-go-client\\" | timechart fixedrange=f values(status) by uri_path</query><earliest>-24h@h</earliest><latest>now</latest><sampleRatio>1</sampleRatio></search><option name=\\"charting.axisLabelsX.majorLabelStyle.overflowMode\\">ellipsisNone</option><option name=\\"charting.axisLabelsX.majorLabelStyle.rotation\\">0</option><option name=\\"charting.axisTitleX.visibility\\">collapsed</option><option name=\\"charting.axisTitleY.text\\">HTTP status codes</option><option name=\\"charting.axisTitleY.visibility\\">visible</option><option name=\\"charting.axisTitleY2.visibility\\">visible</option><option name=\\"charting.axisX.abbreviation\\">none</option><option name=\\"charting.axisX.scale\\">linear</option><option name=\\"charting.axisY.abbreviation\\">none</option><option name=\\"charting.axisY.scale\\">linear</option><option name=\\"charting.axisY2.abbreviation\\">none</option><option name=\\"charting.axisY2.enabled\\">0</option><option name=\\"charting.axisY2.scale\\">inherit</option><option name=\\"charting.chart\\">column</option><option name=\\"charting.chart.bubbleMaximumSize\\">50</option><option name=\\"charting.chart.bubbleMinimumSize\\">10</option><option name=\\"charting.chart.bubbleSizeBy\\">area</option><option name=\\"charting.chart.nullValueMode\\">connect</option><option name=\\"charting.chart.showDataLabels\\">none</option><option name=\\"charting.chart.sliceCollapsingThreshold\\">0.01</option><option name=\\"charting.chart.stackMode\\">default</option><option name=\\"charting.chart.style\\">shiny</option><option name=\\"charting.drilldown\\">none</option><option name=\\"charting.layout.splitSeries\\">0</option><option name=\\"charting.layout.splitSeries.allowIndependentYRanges\\">0</option><option name=\\"charting.legend.labelStyle.overflowMode\\">ellipsisMiddle</option><option name=\\"charting.legend.mode\\">standard</option><option name=\\"charting.legend.placement\\">right</option><option name=\\"charting.lineWidth\\">2</option><option name=\\"trellis.enabled\\">0</option><option name=\\"trellis.scales.shared\\">1</option><option name=\\"trellis.size\\">small</option><option name=\\"trellis.splitBy\\">_aggregation</option></chart></panel></row></dashboard>")
+                app="search",
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] eai_data: Dashboard XML definition.
         :param pulumi.Input[str] name: Dashboard name.
@@ -169,19 +170,20 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         dashboard = splunk.DataUiViews("dashboard",
+            name="Terraform_Sample_Dashboard",
+            eai_data="<dashboard version=\\"1.1\\"><label>Terraform</label><description>Terraform operations</description><row><panel><chart><search><query>index=_internal sourcetype=splunkd_access useragent=\\"splunk-simple-go-client\\" | timechart fixedrange=f values(status) by uri_path</query><earliest>-24h@h</earliest><latest>now</latest><sampleRatio>1</sampleRatio></search><option name=\\"charting.axisLabelsX.majorLabelStyle.overflowMode\\">ellipsisNone</option><option name=\\"charting.axisLabelsX.majorLabelStyle.rotation\\">0</option><option name=\\"charting.axisTitleX.visibility\\">collapsed</option><option name=\\"charting.axisTitleY.text\\">HTTP status codes</option><option name=\\"charting.axisTitleY.visibility\\">visible</option><option name=\\"charting.axisTitleY2.visibility\\">visible</option><option name=\\"charting.axisX.abbreviation\\">none</option><option name=\\"charting.axisX.scale\\">linear</option><option name=\\"charting.axisY.abbreviation\\">none</option><option name=\\"charting.axisY.scale\\">linear</option><option name=\\"charting.axisY2.abbreviation\\">none</option><option name=\\"charting.axisY2.enabled\\">0</option><option name=\\"charting.axisY2.scale\\">inherit</option><option name=\\"charting.chart\\">column</option><option name=\\"charting.chart.bubbleMaximumSize\\">50</option><option name=\\"charting.chart.bubbleMinimumSize\\">10</option><option name=\\"charting.chart.bubbleSizeBy\\">area</option><option name=\\"charting.chart.nullValueMode\\">connect</option><option name=\\"charting.chart.showDataLabels\\">none</option><option name=\\"charting.chart.sliceCollapsingThreshold\\">0.01</option><option name=\\"charting.chart.stackMode\\">default</option><option name=\\"charting.chart.style\\">shiny</option><option name=\\"charting.drilldown\\">none</option><option name=\\"charting.layout.splitSeries\\">0</option><option name=\\"charting.layout.splitSeries.allowIndependentYRanges\\">0</option><option name=\\"charting.legend.labelStyle.overflowMode\\">ellipsisMiddle</option><option name=\\"charting.legend.mode\\">standard</option><option name=\\"charting.legend.placement\\">right</option><option name=\\"charting.lineWidth\\">2</option><option name=\\"trellis.enabled\\">0</option><option name=\\"trellis.scales.shared\\">1</option><option name=\\"trellis.size\\">small</option><option name=\\"trellis.splitBy\\">_aggregation</option></chart></panel></row></dashboard>",
             acl=splunk.DataUiViewsAclArgs(
-                app="search",
                 owner="admin",
-            ),
-            eai_data="<dashboard version=\\"1.1\\"><label>Terraform</label><description>Terraform operations</description><row><panel><chart><search><query>index=_internal sourcetype=splunkd_access useragent=\\"splunk-simple-go-client\\" | timechart fixedrange=f values(status) by uri_path</query><earliest>-24h@h</earliest><latest>now</latest><sampleRatio>1</sampleRatio></search><option name=\\"charting.axisLabelsX.majorLabelStyle.overflowMode\\">ellipsisNone</option><option name=\\"charting.axisLabelsX.majorLabelStyle.rotation\\">0</option><option name=\\"charting.axisTitleX.visibility\\">collapsed</option><option name=\\"charting.axisTitleY.text\\">HTTP status codes</option><option name=\\"charting.axisTitleY.visibility\\">visible</option><option name=\\"charting.axisTitleY2.visibility\\">visible</option><option name=\\"charting.axisX.abbreviation\\">none</option><option name=\\"charting.axisX.scale\\">linear</option><option name=\\"charting.axisY.abbreviation\\">none</option><option name=\\"charting.axisY.scale\\">linear</option><option name=\\"charting.axisY2.abbreviation\\">none</option><option name=\\"charting.axisY2.enabled\\">0</option><option name=\\"charting.axisY2.scale\\">inherit</option><option name=\\"charting.chart\\">column</option><option name=\\"charting.chart.bubbleMaximumSize\\">50</option><option name=\\"charting.chart.bubbleMinimumSize\\">10</option><option name=\\"charting.chart.bubbleSizeBy\\">area</option><option name=\\"charting.chart.nullValueMode\\">connect</option><option name=\\"charting.chart.showDataLabels\\">none</option><option name=\\"charting.chart.sliceCollapsingThreshold\\">0.01</option><option name=\\"charting.chart.stackMode\\">default</option><option name=\\"charting.chart.style\\">shiny</option><option name=\\"charting.drilldown\\">none</option><option name=\\"charting.layout.splitSeries\\">0</option><option name=\\"charting.layout.splitSeries.allowIndependentYRanges\\">0</option><option name=\\"charting.legend.labelStyle.overflowMode\\">ellipsisMiddle</option><option name=\\"charting.legend.mode\\">standard</option><option name=\\"charting.legend.placement\\">right</option><option name=\\"charting.lineWidth\\">2</option><option name=\\"trellis.enabled\\">0</option><option name=\\"trellis.scales.shared\\">1</option><option name=\\"trellis.size\\">small</option><option name=\\"trellis.splitBy\\">_aggregation</option></chart></panel></row></dashboard>")
+                app="search",
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param DataUiViewsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/generic_acl.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/generic_acl.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,33 +116,33 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        my_app = splunk.GenericAcl("myApp",
+        my_app = splunk.GenericAcl("my_app",
+            path="apps/local/my_app",
             acl=splunk.GenericAclAclArgs(
                 app="system",
                 owner="nobody",
                 reads=["*"],
                 writes=[
                     "admin",
                     "power",
                 ],
-            ),
-            path="apps/local/my_app")
-        my_dashboard = splunk.GenericAcl("myDashboard",
+            ))
+        my_dashboard = splunk.GenericAcl("my_dashboard",
+            path="data/ui/views/my_dashboard",
             acl=splunk.GenericAclAclArgs(
                 app="my_app",
                 owner="joe_user",
                 reads=["team_joe"],
                 writes=["team_joe"],
-            ),
-            path="data/ui/views/my_dashboard")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Generic ACL resources can be imported by specifying their owner, app, and path with a colon-delimited string as the ID:
 
@@ -168,33 +168,33 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        my_app = splunk.GenericAcl("myApp",
+        my_app = splunk.GenericAcl("my_app",
+            path="apps/local/my_app",
             acl=splunk.GenericAclAclArgs(
                 app="system",
                 owner="nobody",
                 reads=["*"],
                 writes=[
                     "admin",
                     "power",
                 ],
-            ),
-            path="apps/local/my_app")
-        my_dashboard = splunk.GenericAcl("myDashboard",
+            ))
+        my_dashboard = splunk.GenericAcl("my_dashboard",
+            path="data/ui/views/my_dashboard",
             acl=splunk.GenericAclAclArgs(
                 app="my_app",
                 owner="joe_user",
                 reads=["team_joe"],
                 writes=["team_joe"],
-            ),
-            path="data/ui/views/my_dashboard")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Generic ACL resources can be imported by specifying their owner, app, and path with a colon-delimited string as the ID:
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/global_http_event_collector.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/global_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/indexes.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/indexes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1512,14 +1512,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         user01_index = splunk.Indexes("user01-index",
+            name="user01-index",
             max_hot_buckets=6,
             max_total_data_size_mb=1000000)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -1627,14 +1628,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         user01_index = splunk.Indexes("user01-index",
+            name="user01-index",
             max_hot_buckets=6,
             max_total_data_size_mb=1000000)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param IndexesArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_http_event_collector.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_http_event_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,30 +374,31 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         hec_token_01 = splunk.InputsHttpEventCollector("hec-token-01",
-            acl=splunk.InputsHttpEventCollectorAclArgs(
-                owner="user01",
-                reads=["admin"],
-                sharing="global",
-                writes=["admin"],
-            ),
-            disabled=False,
+            name="hec-token-01",
             index="main",
             indexes=[
                 "main",
                 "history",
                 "summary",
             ],
             source="new:source",
             sourcetype="new:sourcetype",
-            use_ack=0)
+            disabled=False,
+            use_ack=0,
+            acl=splunk.InputsHttpEventCollectorAclArgs(
+                owner="user01",
+                sharing="global",
+                reads=["admin"],
+                writes=["admin"],
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsHttpEventCollectorAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[bool] disabled: Input disabled indicator
@@ -425,30 +426,31 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         hec_token_01 = splunk.InputsHttpEventCollector("hec-token-01",
-            acl=splunk.InputsHttpEventCollectorAclArgs(
-                owner="user01",
-                reads=["admin"],
-                sharing="global",
-                writes=["admin"],
-            ),
-            disabled=False,
+            name="hec-token-01",
             index="main",
             indexes=[
                 "main",
                 "history",
                 "summary",
             ],
             source="new:source",
             sourcetype="new:sourcetype",
-            use_ack=0)
+            disabled=False,
+            use_ack=0,
+            acl=splunk.InputsHttpEventCollectorAclArgs(
+                owner="user01",
+                sharing="global",
+                reads=["admin"],
+                writes=["admin"],
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsHttpEventCollectorArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_monitor.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,14 +572,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         monitor = splunk.InputsMonitor("monitor",
+            name="opt/splunk/var/log/splunk/health.log",
             recursive=True,
             sourcetype="text")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -615,14 +616,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         monitor = splunk.InputsMonitor("monitor",
+            name="opt/splunk/var/log/splunk/health.log",
             recursive=True,
             sourcetype="text")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsMonitorArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_script.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,15 +380,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        script = splunk.InputsScript("script", interval=360)
+        script = splunk.InputsScript("script",
+            name="opt/splunk/bin/scripts/readme.txt",
+            interval=360)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsScriptAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[bool] disabled: Specifies whether the input script is disabled.
@@ -417,15 +419,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        script = splunk.InputsScript("script", interval=360)
+        script = splunk.InputsScript("script",
+            name="opt/splunk/bin/scripts/readme.txt",
+            interval=360)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsScriptArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_tcp_cooked.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_cooked.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,17 +261,18 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_cooked = splunk.InputsTcpCooked("tcpCooked",
-            connection_host="dns",
+        tcp_cooked = splunk.InputsTcpCooked("tcp_cooked",
+            name="50000",
             disabled=False,
+            connection_host="dns",
             restrict_to_host="splunk")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsTcpCookedAclArgs']] acl: The app/user context that is the namespace for the resource
@@ -300,17 +301,18 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_cooked = splunk.InputsTcpCooked("tcpCooked",
-            connection_host="dns",
+        tcp_cooked = splunk.InputsTcpCooked("tcp_cooked",
+            name="50000",
             disabled=False,
+            connection_host="dns",
             restrict_to_host="splunk")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsTcpCookedArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_tcp_raw.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,20 +454,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_raw = splunk.InputsTcpRaw("tcpRaw",
-            disabled=False,
+        tcp_raw = splunk.InputsTcpRaw("tcp_raw",
+            name="41000",
             index="main",
             queue="indexQueue",
             source="new",
-            sourcetype="new")
+            sourcetype="new",
+            disabled=False)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsTcpRawAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] connection_host: Valid values: (ip | dns | none)
@@ -507,20 +508,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_raw = splunk.InputsTcpRaw("tcpRaw",
-            disabled=False,
+        tcp_raw = splunk.InputsTcpRaw("tcp_raw",
+            name="41000",
             index="main",
             queue="indexQueue",
             source="new",
-            sourcetype="new")
+            sourcetype="new",
+            disabled=False)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsTcpRawArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_tcp_splunk_tcp_token.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_splunk_tcp_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_splunk_tcp_token = splunk.InputsTcpSplunkTcpToken("tcpSplunkTcpToken", token="D66C45B3-7C28-48A1-A13A-027914146501")
+        tcp_splunk_tcp_token = splunk.InputsTcpSplunkTcpToken("tcp_splunk_tcp_token",
+            name="new-splunk-tcp-token",
+            token="D66C45B3-7C28-48A1-A13A-027914146501")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsTcpSplunkTcpTokenAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] name: Required. Name for the token to create.
@@ -170,15 +172,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_splunk_tcp_token = splunk.InputsTcpSplunkTcpToken("tcpSplunkTcpToken", token="D66C45B3-7C28-48A1-A13A-027914146501")
+        tcp_splunk_tcp_token = splunk.InputsTcpSplunkTcpToken("tcp_splunk_tcp_token",
+            name="new-splunk-tcp-token",
+            token="D66C45B3-7C28-48A1-A13A-027914146501")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsTcpSplunkTcpTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_tcp_ssl.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_ssl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/inputs_udp.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_udp.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,18 +464,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         udp = splunk.InputsUdp("udp",
-            disabled=False,
+            name="41000",
             index="main",
             source="new",
-            sourcetype="new")
+            sourcetype="new",
+            disabled=False)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsUdpAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] connection_host: Valid values: (ip | dns | none)
@@ -511,18 +512,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         udp = splunk.InputsUdp("udp",
-            disabled=False,
+            name="41000",
             index="main",
             source="new",
-            sourcetype="new")
+            sourcetype="new",
+            disabled=False)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsUdpArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/outputs.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/outputs_tcp_default.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_default.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,21 +388,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_default = splunk.OutputsTcpDefault("tcpDefault",
-            default_group="test-indexers",
+        tcp_default = splunk.OutputsTcpDefault("tcp_default",
+            name="tcpout",
             disabled=False,
+            default_group="test-indexers",
             drop_events_on_queue_full=60,
             index_and_forward=True,
-            max_queue_size="100KB",
-            send_cooked_data=True)
+            send_cooked_data=True,
+            max_queue_size="100KB")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['OutputsTcpDefaultAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] default_group: Comma-separated list of one or more target group names, specified later in [tcpout:<target_group>] stanzas of outputs.conf.spec file.
@@ -440,21 +441,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_default = splunk.OutputsTcpDefault("tcpDefault",
-            default_group="test-indexers",
+        tcp_default = splunk.OutputsTcpDefault("tcp_default",
+            name="tcpout",
             disabled=False,
+            default_group="test-indexers",
             drop_events_on_queue_full=60,
             index_and_forward=True,
-            max_queue_size="100KB",
-            send_cooked_data=True)
+            send_cooked_data=True,
+            max_queue_size="100KB")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param OutputsTcpDefaultArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/outputs_tcp_group.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,19 +445,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_group = splunk.OutputsTcpGroup("tcpGroup",
+        tcp_group = splunk.OutputsTcpGroup("tcp_group",
+            name="tcp-group",
             disabled=False,
             drop_events_on_queue_full=60,
-            max_queue_size="100KB",
             send_cooked_data=True,
+            max_queue_size="100KB",
             servers=[
                 "1.1.1.1:1234",
                 "2.2.2.2:1234",
             ])
         ```
         <!--End PulumiCodeChooser -->
 
@@ -499,19 +500,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_group = splunk.OutputsTcpGroup("tcpGroup",
+        tcp_group = splunk.OutputsTcpGroup("tcp_group",
+            name="tcp-group",
             disabled=False,
             drop_events_on_queue_full=60,
-            max_queue_size="100KB",
             send_cooked_data=True,
+            max_queue_size="100KB",
             servers=[
                 "1.1.1.1:1234",
                 "2.2.2.2:1234",
             ])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/outputs_tcp_server.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,15 +418,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_server = splunk.OutputsTcpServer("tcpServer", ssl_alt_name_to_check="old-host")
+        tcp_server = splunk.OutputsTcpServer("tcp_server",
+            name="new-host:1234",
+            ssl_alt_name_to_check="old-host")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['OutputsTcpServerAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[bool] disabled: If true, disables the group.
@@ -457,15 +459,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_server = splunk.OutputsTcpServer("tcpServer", ssl_alt_name_to_check="old-host")
+        tcp_server = splunk.OutputsTcpServer("tcp_server",
+            name="new-host:1234",
+            ssl_alt_name_to_check="old-host")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param OutputsTcpServerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/outputs_tcp_syslog.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_syslog.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,17 +331,18 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_syslog = splunk.OutputsTcpSyslog("tcpSyslog",
-            priority=5,
-            server="new-host-1:1234")
+        tcp_syslog = splunk.OutputsTcpSyslog("tcp_syslog",
+            name="new-syslog",
+            server="new-host-1:1234",
+            priority=5)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['OutputsTcpSyslogAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[bool] disabled: If true, disables global syslog settings.
@@ -372,17 +373,18 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        tcp_syslog = splunk.OutputsTcpSyslog("tcpSyslog",
-            priority=5,
-            server="new-host-1:1234")
+        tcp_syslog = splunk.OutputsTcpSyslog("tcp_syslog",
+            name="new-syslog",
+            server="new-host-1:1234",
+            priority=5)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param OutputsTcpSyslogArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/provider.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/saved_searches.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/saved_searches.py`

 * *Files 0% similar despite different names*

```diff
@@ -5508,32 +5508,33 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        saved_search = splunk.SavedSearches("savedSearch",
-            acl=splunk.SavedSearchesAclArgs(
-                app="launcher",
-                owner="admin",
-                sharing="app",
-            ),
+        saved_search = splunk.SavedSearches("saved_search",
+            name="Test New Alert",
+            search="index=main",
+            actions="email",
             action_email_format="table",
-            action_email_max_results=10,
             action_email_max_time="5m",
+            action_email_max_results=10,
             action_email_send_results=False,
             action_email_subject="Splunk Alert: $name$",
             action_email_to="splunk@splunk.com",
             action_email_track_alert=True,
-            actions="email",
-            cron_schedule="*/5 * * * *",
             dispatch_earliest_time="rt-15m",
             dispatch_latest_time="rt-0m",
-            search="index=main")
+            cron_schedule="*/5 * * * *",
+            acl=splunk.SavedSearchesAclArgs(
+                owner="admin",
+                sharing="app",
+                app="launcher",
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['SavedSearchesAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] action_create_xsoar_incident: Enable XSOAR alerting (Should by 1 (Enabled) or 0 (Disabled))
@@ -5722,32 +5723,33 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
-        saved_search = splunk.SavedSearches("savedSearch",
-            acl=splunk.SavedSearchesAclArgs(
-                app="launcher",
-                owner="admin",
-                sharing="app",
-            ),
+        saved_search = splunk.SavedSearches("saved_search",
+            name="Test New Alert",
+            search="index=main",
+            actions="email",
             action_email_format="table",
-            action_email_max_results=10,
             action_email_max_time="5m",
+            action_email_max_results=10,
             action_email_send_results=False,
             action_email_subject="Splunk Alert: $name$",
             action_email_to="splunk@splunk.com",
             action_email_track_alert=True,
-            actions="email",
-            cron_schedule="*/5 * * * *",
             dispatch_earliest_time="rt-15m",
             dispatch_latest_time="rt-0m",
-            search="index=main")
+            cron_schedule="*/5 * * * *",
+            acl=splunk.SavedSearchesAclArgs(
+                owner="admin",
+                sharing="app",
+                app="launcher",
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SavedSearchesArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk/sh_indexes_manager.py` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/sh_indexes_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tf_index = splunk.ShIndexesManager("tf-index",
+            name="tf-test-index-0",
             datatype="event",
             frozen_time_period_in_secs="94608000",
             max_global_raw_data_size_mb="100")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
@@ -251,14 +252,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tf_index = splunk.ShIndexesManager("tf-index",
+            name="tf-test-index-0",
             datatype="event",
             frozen_time_period_in_secs="94608000",
             max_global_raw_data_size_mb="100")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk.egg-info/PKG-INFO` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1713338397
+Version: 1.3.0a1713561402
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi,splunk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_splunk-1.3.0a1713338397/pulumi_splunk.egg-info/SOURCES.txt` & `pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713338397/pyproject.toml` & `pulumi_splunk-1.3.0a1713561402/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_splunk"
   description = "A Pulumi package for creating and managing splunk cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0a1,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "splunk"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.3.0a1713338397"
+  version = "1.3.0a1713561402"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-splunk"
 
 [build-system]
```

