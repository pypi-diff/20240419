# Comparing `tmp/pulumi_ns1-3.3.0a1713333847.tar.gz` & `tmp/pulumi_ns1-3.3.0a1713561640.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ns1-3.3.0a1713333847.tar", last modified: Wed Apr 17 06:17:31 2024, max compression
+gzip compressed data, was "pulumi_ns1-3.3.0a1713561640.tar", last modified: Fri Apr 19 21:27:13 2024, max compression
```

## Comparing `pulumi_ns1-3.3.0a1713333847.tar` & `pulumi_ns1-3.3.0a1713561640.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:17:31.794255 pulumi_ns1-3.3.0a1713333847/
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-17 06:17:31.794255 pulumi_ns1-3.3.0a1713333847/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:17:31.794255 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38901 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/account_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    87352 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:17:31.794255 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/data_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)    11178 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/dnsview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/get_dns_sec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/get_monitoring_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/get_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/get_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    45856 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/monitoring_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/notify_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    46058 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17050 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/pulsar_job.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    36697 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    19239 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    81738 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/tsigkey.py
--rw-r--r--   0 runner    (1001) docker     (127)    89294 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    42852 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:17:31.794255 pulumi_ns1-3.3.0a1713333847/pulumi_ns1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-17 06:17:31.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-17 06:17:31.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:17:31.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 06:17:31.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 06:17:31.000000 pulumi_ns1-3.3.0a1713333847/pulumi_ns1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-17 06:17:25.000000 pulumi_ns1-3.3.0a1713333847/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:17:31.794255 pulumi_ns1-3.3.0a1713333847/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38901 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/account_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87418 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/dnsview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_monitoring_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45912 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/monitoring_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/notify_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46058 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17050 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/pulsar_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    44687 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19239 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81870 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/tsigkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89390 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42852 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-19 21:27:13.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 21:27:13.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:27:13.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:27:13.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 21:27:13.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/setup.cfg
```

### Comparing `pulumi_ns1-3.3.0a1713333847/PKG-INFO` & `pulumi_ns1-3.3.0a1713561640/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ns1
-Version: 3.3.0a1713333847
+Version: 3.3.0a1713561640
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi,ns1
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ns1-3.3.0a1713333847/README.md` & `pulumi_ns1-3.3.0a1713561640/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/__init__.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/_inputs.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/_utilities.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/account_whitelist.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/account_whitelist.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,18 +106,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        example = ns1.AccountWhitelist("example", values=[
-            "1.1.1.1",
-            "2.2.2.2",
-        ])
+        example = ns1.AccountWhitelist("example",
+            name="Example Whitelist",
+            values=[
+                "1.1.1.1",
+                "2.2.2.2",
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         > You current source IP must be present in one of the whitelists to prevent locking yourself out.
 
         ## NS1 Documentation
 
@@ -148,18 +150,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        example = ns1.AccountWhitelist("example", values=[
-            "1.1.1.1",
-            "2.2.2.2",
-        ])
+        example = ns1.AccountWhitelist("example",
+            name="Example Whitelist",
+            values=[
+                "1.1.1.1",
+                "2.2.2.2",
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         > You current source IP must be present in one of the whitelists to prevent locking yourself out.
 
         ## NS1 Documentation
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/api_key.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1145,17 +1145,18 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        example_team = ns1.Team("exampleTeam")
-        example_api_key = ns1.APIKey("exampleAPIKey",
-            teams=[example_team.id],
+        example = ns1.Team("example", name="Example team")
+        example_api_key = ns1.APIKey("example",
+            name="Example key",
+            teams=[example.id],
             ip_whitelists=[
                 "1.1.1.1",
                 "2.2.2.2",
             ],
             dns_view_zones=False,
             account_manage_users=False)
         ```
@@ -1242,17 +1243,18 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        example_team = ns1.Team("exampleTeam")
-        example_api_key = ns1.APIKey("exampleAPIKey",
-            teams=[example_team.id],
+        example = ns1.Team("example", name="Example team")
+        example_api_key = ns1.APIKey("example",
+            name="Example key",
+            teams=[example.id],
             ip_whitelists=[
                 "1.1.1.1",
                 "2.2.2.2",
             ],
             dns_view_zones=False,
             account_manage_users=False)
         ```
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/application.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,36 +211,14 @@
                  default_config: Optional[pulumi.Input[pulumi.InputType['ApplicationDefaultConfigArgs']]] = None,
                  jobs_per_transaction: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a NS1 Pulsar application resource. This can be used to create, modify, and delete applications.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_ns1 as ns1
-
-        # Create a new pulsar application with default config
-        ns1_app = ns1.Application("ns1App", default_config=ns1.ApplicationDefaultConfigArgs(
-            http=True,
-            https=False,
-            job_timeout_millis=100,
-            request_timeout_millis=100,
-            static_values=True,
-        ))
-        ```
-        <!--End PulumiCodeChooser -->
-
-        ## NS1 Documentation
-
-        [Application Api Docs](https://ns1.com/api#get-list-pulsar-applications)
-
         ## Import
 
         ```sh
         $ pulumi import ns1:index/application:Application `ns1_application`
         ```
 
         So for the example above:
@@ -265,36 +243,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ApplicationArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a NS1 Pulsar application resource. This can be used to create, modify, and delete applications.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_ns1 as ns1
-
-        # Create a new pulsar application with default config
-        ns1_app = ns1.Application("ns1App", default_config=ns1.ApplicationDefaultConfigArgs(
-            http=True,
-            https=False,
-            job_timeout_millis=100,
-            request_timeout_millis=100,
-            static_values=True,
-        ))
-        ```
-        <!--End PulumiCodeChooser -->
-
-        ## NS1 Documentation
-
-        [Application Api Docs](https://ns1.com/api#get-list-pulsar-applications)
-
         ## Import
 
         ```sh
         $ pulumi import ns1:index/application:Application `ns1_application`
         ```
 
         So for the example above:
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/config/__init__.pyi` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/config/vars.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/data_feed.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/data_feed.py`

 * *Files 8% similar despite different names*

```diff
@@ -141,30 +141,37 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        example = ns1.DataSource("example", sourcetype="nsone_v1")
-        example_monitoring = ns1.DataSource("exampleMonitoring", sourcetype="nsone_monitoring")
-        uswest_feed = ns1.DataFeed("uswestFeed",
+        example = ns1.DataSource("example",
+            name="example",
+            sourcetype="nsone_v1")
+        example_monitoring = ns1.DataSource("example_monitoring",
+            name="example_monitoring",
+            sourcetype="nsone_monitoring")
+        uswest_feed = ns1.DataFeed("uswest_feed",
+            name="uswest_feed",
             source_id=example.id,
             config={
                 "label": "uswest",
             })
-        useast_feed = ns1.DataFeed("useastFeed",
+        useast_feed = ns1.DataFeed("useast_feed",
+            name="useast_feed",
             source_id=example.id,
             config={
                 "label": "useast",
             })
-        useast_monitor_feed = ns1.DataFeed("useastMonitorFeed",
+        useast_monitor_feed = ns1.DataFeed("useast_monitor_feed",
+            name="useast_monitor_feed",
             source_id=example_monitoring.id,
             config={
-                "jobid": ns1_monitoringjob["example_job"]["id"],
+                "jobid": example_job["id"],
             })
         ```
         <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Datafeed Api Doc](https://ns1.com/api#data-feeds)
@@ -194,30 +201,37 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        example = ns1.DataSource("example", sourcetype="nsone_v1")
-        example_monitoring = ns1.DataSource("exampleMonitoring", sourcetype="nsone_monitoring")
-        uswest_feed = ns1.DataFeed("uswestFeed",
+        example = ns1.DataSource("example",
+            name="example",
+            sourcetype="nsone_v1")
+        example_monitoring = ns1.DataSource("example_monitoring",
+            name="example_monitoring",
+            sourcetype="nsone_monitoring")
+        uswest_feed = ns1.DataFeed("uswest_feed",
+            name="uswest_feed",
             source_id=example.id,
             config={
                 "label": "uswest",
             })
-        useast_feed = ns1.DataFeed("useastFeed",
+        useast_feed = ns1.DataFeed("useast_feed",
+            name="useast_feed",
             source_id=example.id,
             config={
                 "label": "useast",
             })
-        useast_monitor_feed = ns1.DataFeed("useastMonitorFeed",
+        useast_monitor_feed = ns1.DataFeed("useast_monitor_feed",
+            name="useast_monitor_feed",
             source_id=example_monitoring.id,
             config={
-                "jobid": ns1_monitoringjob["example_job"]["id"],
+                "jobid": example_job["id"],
             })
         ```
         <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Datafeed Api Doc](https://ns1.com/api#data-feeds)
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/data_source.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        example = ns1.DataSource("example", sourcetype="nsone_v1")
+        example = ns1.DataSource("example",
+            name="example",
+            sourcetype="nsone_v1")
         ```
         <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Datasource Api Doc](https://ns1.com/api#data-sources)
 
@@ -178,15 +180,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        example = ns1.DataSource("example", sourcetype="nsone_v1")
+        example = ns1.DataSource("example",
+            name="example",
+            sourcetype="nsone_v1")
         ```
         <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Datasource Api Doc](https://ns1.com/api#data-sources)
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/dataset.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/dataset.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/dnsview.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/dnsview.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/get_dns_sec.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_dns_sec.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,18 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get DNSSEC details about a NS1 Zone.
-    example_zone = ns1.Zone("exampleZone",
-        dnssec=True,
-        zone="terraform.example.io")
-    example_dns_sec = ns1.get_dns_sec_output(zone=example_zone.zone)
+    example_zone = ns1.Zone("example",
+        zone="terraform.example.io",
+        dnssec=True)
+    example = ns1.get_dns_sec_output(zone=example_zone.zone)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str zone: The name of the zone to get DNSSEC details for.
     """
     __args__ = dict()
@@ -124,18 +124,18 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get DNSSEC details about a NS1 Zone.
-    example_zone = ns1.Zone("exampleZone",
-        dnssec=True,
-        zone="terraform.example.io")
-    example_dns_sec = ns1.get_dns_sec_output(zone=example_zone.zone)
+    example_zone = ns1.Zone("example",
+        zone="terraform.example.io",
+        dnssec=True)
+    example = ns1.get_dns_sec_output(zone=example_zone.zone)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str zone: The name of the zone to get DNSSEC details for.
     """
     ...
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/get_monitoring_regions.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_monitoring_regions.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
+    # Get details of all available monitoring regions.
     example = ns1.get_monitoring_regions()
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetMonitoringRegionsRegionArgs']] regions: A set of the available monitoring regions. Regions is
            documented below.
@@ -98,14 +99,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
+    # Get details of all available monitoring regions.
     example = ns1.get_monitoring_regions()
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetMonitoringRegionsRegionArgs']] regions: A set of the available monitoring regions. Regions is
            documented below.
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/get_networks.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_networks.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
+    # Get details about NS1 Networks.
     example = ns1.get_networks()
     ```
     <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ns1:index/getNetworks:getNetworks', __args__, opts=opts, typ=GetNetworksResult).value
@@ -94,12 +95,13 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
+    # Get details about NS1 Networks.
     example = ns1.get_networks()
     ```
     <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/get_record.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,17 +195,18 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
-    example = ns1.get_record(domain="terraform.example.io",
-        type="A",
-        zone="example.io")
+    # Get details about a NS1 Record.
+    example = ns1.get_record(zone="example.io",
+        domain="terraform.example.io",
+        type="A")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str domain: The records' domain.
     :param str type: The records' RR type.
     :param str zone: The zone the record belongs to.
@@ -247,17 +248,18 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
-    example = ns1.get_record(domain="terraform.example.io",
-        type="A",
-        zone="example.io")
+    # Get details about a NS1 Record.
+    example = ns1.get_record(zone="example.io",
+        domain="terraform.example.io",
+        type="A")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str domain: The records' domain.
     :param str type: The records' RR type.
     :param str zone: The zone the record belongs to.
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/get_zone.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_zone.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
+    # Get details about a NS1 Zone.
     example = ns1.get_zone(zone="terraform.example.io")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] additional_primaries: List of additional IPv4 addresses for the primary
            zone.
@@ -309,14 +310,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
+    # Get details about a NS1 Zone.
     example = ns1.get_zone(zone="terraform.example.io")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] additional_primaries: List of additional IPv4 addresses for the primary
            zone.
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/monitoring_job.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/monitoring_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,36 +565,37 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        uswest_monitor = ns1.MonitoringJob("uswestMonitor",
+        uswest_monitor = ns1.MonitoringJob("uswest_monitor",
+            name="uswest",
             active=True,
-            config={
-                "host": "example-elb-uswest.aws.amazon.com",
-                "port": 443,
-                "send": "HEAD / HTTP/1.0\\\\r\\\\n\\\\r\\\\n",
-                "ssl": 1,
-            },
-            frequency=60,
-            job_type="tcp",
-            mute=True,
-            policy="quorum",
-            rapid_recheck=True,
             regions=[
                 "lga",
                 "sjc",
                 "sin",
             ],
+            job_type="tcp",
+            frequency=60,
+            rapid_recheck=True,
+            policy="quorum",
+            mute=True,
+            config={
+                "ssl": 1,
+                "send": "HEAD / HTTP/1.0\\\\r\\\\n\\\\r\\\\n",
+                "port": 443,
+                "host": "example-elb-uswest.aws.amazon.com",
+            },
             rules=[ns1.MonitoringJobRuleArgs(
+                value="200 OK",
                 comparison="contains",
                 key="output",
-                value="200 OK",
             )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [MonitoringJob Api Doc](https://ns1.com/api#monitoring-jobs)
@@ -637,36 +638,37 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        uswest_monitor = ns1.MonitoringJob("uswestMonitor",
+        uswest_monitor = ns1.MonitoringJob("uswest_monitor",
+            name="uswest",
             active=True,
-            config={
-                "host": "example-elb-uswest.aws.amazon.com",
-                "port": 443,
-                "send": "HEAD / HTTP/1.0\\\\r\\\\n\\\\r\\\\n",
-                "ssl": 1,
-            },
-            frequency=60,
-            job_type="tcp",
-            mute=True,
-            policy="quorum",
-            rapid_recheck=True,
             regions=[
                 "lga",
                 "sjc",
                 "sin",
             ],
+            job_type="tcp",
+            frequency=60,
+            rapid_recheck=True,
+            policy="quorum",
+            mute=True,
+            config={
+                "ssl": 1,
+                "send": "HEAD / HTTP/1.0\\\\r\\\\n\\\\r\\\\n",
+                "port": 443,
+                "host": "example-elb-uswest.aws.amazon.com",
+            },
             rules=[ns1.MonitoringJobRuleArgs(
+                value="200 OK",
                 comparison="contains",
                 key="output",
-                value="200 OK",
             )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [MonitoringJob Api Doc](https://ns1.com/api#monitoring-jobs)
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/notify_list.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/notify_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,28 +107,30 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        nl = ns1.NotifyList("nl", notifications=[
-            ns1.NotifyListNotificationArgs(
-                config={
-                    "url": "http://www.mywebhook.com",
-                },
-                type="webhook",
-            ),
-            ns1.NotifyListNotificationArgs(
-                config={
-                    "email": "test@test.com",
-                },
-                type="email",
-            ),
-        ])
+        nl = ns1.NotifyList("nl",
+            name="my notify list",
+            notifications=[
+                ns1.NotifyListNotificationArgs(
+                    type="webhook",
+                    config={
+                        "url": "http://www.mywebhook.com",
+                    },
+                ),
+                ns1.NotifyListNotificationArgs(
+                    type="email",
+                    config={
+                        "email": "test@test.com",
+                    },
+                ),
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [NotifyList Api Doc](https://ns1.com/api#notification-lists)
 
@@ -155,28 +157,30 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        nl = ns1.NotifyList("nl", notifications=[
-            ns1.NotifyListNotificationArgs(
-                config={
-                    "url": "http://www.mywebhook.com",
-                },
-                type="webhook",
-            ),
-            ns1.NotifyListNotificationArgs(
-                config={
-                    "email": "test@test.com",
-                },
-                type="email",
-            ),
-        ])
+        nl = ns1.NotifyList("nl",
+            name="my notify list",
+            notifications=[
+                ns1.NotifyListNotificationArgs(
+                    type="webhook",
+                    config={
+                        "url": "http://www.mywebhook.com",
+                    },
+                ),
+                ns1.NotifyListNotificationArgs(
+                    type="email",
+                    config={
+                        "email": "test@test.com",
+                    },
+                ),
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [NotifyList Api Doc](https://ns1.com/api#notification-lists)
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/outputs.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/provider.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/pulsar_job.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/pulsar_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/record.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/record.py`

 * *Files 10% similar despite different names*

```diff
@@ -509,14 +509,130 @@
                  type: Optional[pulumi.Input[str]] = None,
                  use_client_subnet: Optional[pulumi.Input[bool]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a NS1 Record resource. This can be used to create, modify, and delete records.
 
+        ## Example Usage
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import json
+        import pulumi_external as external
+        import pulumi_ns1 as ns1
+        import pulumi_std as std
+
+        example = ns1.Zone("example", zone="terraform.example.io")
+        ns1 = ns1.DataSource("ns1",
+            name="ns1_source",
+            sourcetype="nsone_v1")
+        foo = ns1.DataFeed("foo",
+            name="foo_feed",
+            source_id=ns1.id,
+            config={
+                "label": "foo",
+            })
+        bar = ns1.DataFeed("bar",
+            name="bar_feed",
+            source_id=ns1.id,
+            config={
+                "label": "bar",
+            })
+        www = ns1.Record("www",
+            zone=tld["zone"],
+            domain=f"www.{tld['zone']}",
+            type="CNAME",
+            ttl=60,
+            meta={
+                "up": True,
+            },
+            regions=[
+                ns1.RecordRegionArgs(
+                    name="east",
+                    meta={
+                        "georegion": "US-EAST",
+                    },
+                ),
+                ns1.RecordRegionArgs(
+                    name="usa",
+                    meta={
+                        "country": "US",
+                    },
+                ),
+            ],
+            answers=[
+                ns1.RecordAnswerArgs(
+                    answer=f"sub1.{tld['zone']}",
+                    region="east",
+                    meta={
+                        "up": foo.id.apply(lambda id: f"{{\\"feed\\":\\"{id}\\"}}"),
+                    },
+                ),
+                ns1.RecordAnswerArgs(
+                    answer=f"sub2.{tld['zone']}",
+                    meta={
+                        "up": bar.id.apply(lambda id: f"{{\\"feed\\":\\"{id}\\"}}"),
+                        "connections": 3,
+                    },
+                ),
+                ns1.RecordAnswerArgs(
+                    answer=f"sub3.{tld['zone']}",
+                    meta={
+                        "pulsar": json.dumps([{
+                            "job_id": "abcdef",
+                            "bias": "*0.55",
+                            "a5m_cutoff": 0.9,
+                        }]),
+                        "subdivisions": json.dumps({
+                            "BR": [
+                                "SP",
+                                "SC",
+                            ],
+                            "DZ": [
+                                "01",
+                                "02",
+                                "03",
+                            ],
+                        }),
+                    },
+                ),
+            ],
+            filters=[ns1.RecordFilterArgs(
+                filter="select_first_n",
+                config={
+                    "N": 1,
+                },
+            )])
+        # Some other non-NS1 provider that returns a zone with a trailing dot and a domain with a leading dot.
+        baz = external.index.Source("baz",
+            zone=terraform.example.io.,
+            domain=.www.terraform.example.io)
+        # Basic record showing how to clean a zone or domain field that comes from
+        # another non-NS1 resource. DNS names often end in '.' characters to signify
+        # the root of the DNS tree, but the NS1 provider does not support this.
+        #
+        # In other cases, a domain or zone may be passed in with a preceding dot ('.')
+        # character which would likewise lead the system to fail.
+        external = ns1.Record("external",
+            zone=std.replace(text=zone,
+                search="/(^\\\\.)|(\\\\.$)/",
+                replace="").result,
+            domain=std.replace(text=domain,
+                search="/(^\\\\.)|(\\\\.$)/",
+                replace="").result,
+            type="CNAME")
+        ```
+        <!--End PulumiCodeChooser -->
+
+        ## NS1 Documentation
+
+        [Record Api Doc](https://ns1.com/api#records)
+
         ## Import
 
         ```sh
         $ pulumi import ns1:index/record:Record <name> <zone>/<domain>/<type>`
         ```
 
         So for the example above:
@@ -553,14 +669,130 @@
     def __init__(__self__,
                  resource_name: str,
                  args: RecordArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a NS1 Record resource. This can be used to create, modify, and delete records.
 
+        ## Example Usage
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import json
+        import pulumi_external as external
+        import pulumi_ns1 as ns1
+        import pulumi_std as std
+
+        example = ns1.Zone("example", zone="terraform.example.io")
+        ns1 = ns1.DataSource("ns1",
+            name="ns1_source",
+            sourcetype="nsone_v1")
+        foo = ns1.DataFeed("foo",
+            name="foo_feed",
+            source_id=ns1.id,
+            config={
+                "label": "foo",
+            })
+        bar = ns1.DataFeed("bar",
+            name="bar_feed",
+            source_id=ns1.id,
+            config={
+                "label": "bar",
+            })
+        www = ns1.Record("www",
+            zone=tld["zone"],
+            domain=f"www.{tld['zone']}",
+            type="CNAME",
+            ttl=60,
+            meta={
+                "up": True,
+            },
+            regions=[
+                ns1.RecordRegionArgs(
+                    name="east",
+                    meta={
+                        "georegion": "US-EAST",
+                    },
+                ),
+                ns1.RecordRegionArgs(
+                    name="usa",
+                    meta={
+                        "country": "US",
+                    },
+                ),
+            ],
+            answers=[
+                ns1.RecordAnswerArgs(
+                    answer=f"sub1.{tld['zone']}",
+                    region="east",
+                    meta={
+                        "up": foo.id.apply(lambda id: f"{{\\"feed\\":\\"{id}\\"}}"),
+                    },
+                ),
+                ns1.RecordAnswerArgs(
+                    answer=f"sub2.{tld['zone']}",
+                    meta={
+                        "up": bar.id.apply(lambda id: f"{{\\"feed\\":\\"{id}\\"}}"),
+                        "connections": 3,
+                    },
+                ),
+                ns1.RecordAnswerArgs(
+                    answer=f"sub3.{tld['zone']}",
+                    meta={
+                        "pulsar": json.dumps([{
+                            "job_id": "abcdef",
+                            "bias": "*0.55",
+                            "a5m_cutoff": 0.9,
+                        }]),
+                        "subdivisions": json.dumps({
+                            "BR": [
+                                "SP",
+                                "SC",
+                            ],
+                            "DZ": [
+                                "01",
+                                "02",
+                                "03",
+                            ],
+                        }),
+                    },
+                ),
+            ],
+            filters=[ns1.RecordFilterArgs(
+                filter="select_first_n",
+                config={
+                    "N": 1,
+                },
+            )])
+        # Some other non-NS1 provider that returns a zone with a trailing dot and a domain with a leading dot.
+        baz = external.index.Source("baz",
+            zone=terraform.example.io.,
+            domain=.www.terraform.example.io)
+        # Basic record showing how to clean a zone or domain field that comes from
+        # another non-NS1 resource. DNS names often end in '.' characters to signify
+        # the root of the DNS tree, but the NS1 provider does not support this.
+        #
+        # In other cases, a domain or zone may be passed in with a preceding dot ('.')
+        # character which would likewise lead the system to fail.
+        external = ns1.Record("external",
+            zone=std.replace(text=zone,
+                search="/(^\\\\.)|(\\\\.$)/",
+                replace="").result,
+            domain=std.replace(text=domain,
+                search="/(^\\\\.)|(\\\\.$)/",
+                replace="").result,
+            type="CNAME")
+        ```
+        <!--End PulumiCodeChooser -->
+
+        ## NS1 Documentation
+
+        [Record Api Doc](https://ns1.com/api#records)
+
         ## Import
 
         ```sh
         $ pulumi import ns1:index/record:Record <name> <zone>/<domain>/<type>`
         ```
 
         So for the example above:
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/subnet.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/team.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/team.py`

 * *Files 1% similar despite different names*

```diff
@@ -1066,16 +1066,15 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         # Create a new NS1 Team
         example = ns1.Team("example",
-            account_manage_users=False,
-            dns_view_zones=False,
+            name="Example team",
             ip_whitelists=[
                 ns1.TeamIpWhitelistArgs(
                     name="whitelist-1",
                     values=[
                         "1.1.1.1",
                         "2.2.2.2",
                     ],
@@ -1083,28 +1082,31 @@
                 ns1.TeamIpWhitelistArgs(
                     name="whitelist-2",
                     values=[
                         "3.3.3.3",
                         "4.4.4.4",
                     ],
                 ),
-            ])
+            ],
+            dns_view_zones=False,
+            account_manage_users=False)
         # Another team
         example2 = ns1.Team("example2",
-            data_manage_datasources=True,
+            name="another team",
+            dns_view_zones=True,
+            dns_zones_allow_by_default=True,
+            dns_zones_allows=["mytest.zone"],
+            dns_zones_denies=["myother.zone"],
             dns_records_allows=[ns1.TeamDnsRecordsAllowArgs(
                 domain="terraform.example.io",
                 include_subdomains=False,
-                type="A",
                 zone="example.io",
+                type="A",
             )],
-            dns_view_zones=True,
-            dns_zones_allows=["mytest.zone"],
-            dns_zones_allow_by_default=True,
-            dns_zones_denies=["myother.zone"])
+            data_manage_datasources=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Team Api Docs](https://ns1.com/api#team)
 
@@ -1167,16 +1169,15 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         # Create a new NS1 Team
         example = ns1.Team("example",
-            account_manage_users=False,
-            dns_view_zones=False,
+            name="Example team",
             ip_whitelists=[
                 ns1.TeamIpWhitelistArgs(
                     name="whitelist-1",
                     values=[
                         "1.1.1.1",
                         "2.2.2.2",
                     ],
@@ -1184,28 +1185,31 @@
                 ns1.TeamIpWhitelistArgs(
                     name="whitelist-2",
                     values=[
                         "3.3.3.3",
                         "4.4.4.4",
                     ],
                 ),
-            ])
+            ],
+            dns_view_zones=False,
+            account_manage_users=False)
         # Another team
         example2 = ns1.Team("example2",
-            data_manage_datasources=True,
+            name="another team",
+            dns_view_zones=True,
+            dns_zones_allow_by_default=True,
+            dns_zones_allows=["mytest.zone"],
+            dns_zones_denies=["myother.zone"],
             dns_records_allows=[ns1.TeamDnsRecordsAllowArgs(
                 domain="terraform.example.io",
                 include_subdomains=False,
-                type="A",
                 zone="example.io",
+                type="A",
             )],
-            dns_view_zones=True,
-            dns_zones_allows=["mytest.zone"],
-            dns_zones_allow_by_default=True,
-            dns_zones_denies=["myother.zone"])
+            data_manage_datasources=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Team Api Docs](https://ns1.com/api#team)
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/tsigkey.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/tsigkey.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.Tsigkey("example",
+            name="ExampleTsigKey",
             algorithm="hmac-sha256",
             secret="Ok1qR5IW1ajVka5cHPEJQIXfLyx5V3PSkFBROAzOn21JumDq6nIpoj6H8rfj5Uo+Ok55ZWQ0Wgrf302fDscHLA==")
         ```
         <!--End PulumiCodeChooser -->
         ## NS1 Documentation
 
         [TSIG Keys Api Doc](https://ns1.com/api/#tsig)
@@ -174,14 +175,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.Tsigkey("example",
+            name="ExampleTsigKey",
             algorithm="hmac-sha256",
             secret="Ok1qR5IW1ajVka5cHPEJQIXfLyx5V3PSkFBROAzOn21JumDq6nIpoj6H8rfj5Uo+Ok55ZWQ0Wgrf302fDscHLA==")
         ```
         <!--End PulumiCodeChooser -->
         ## NS1 Documentation
 
         [TSIG Keys Api Doc](https://ns1.com/api/#tsig)
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/user.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1200,25 +1200,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        example_team = ns1.Team("exampleTeam",
+        example = ns1.Team("example",
+            name="Example team",
             ip_whitelists=[
                 "1.1.1.1",
                 "2.2.2.2",
             ],
             dns_view_zones=False,
             account_manage_users=False)
-        example_user = ns1.User("exampleUser",
+        example_user = ns1.User("example",
+            name="Example User",
             username="example_user",
             email="user@example.com",
-            teams=[example_team.id],
+            teams=[example.id],
             notify={
                 "billing": False,
             })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Permissions
@@ -1299,25 +1301,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
-        example_team = ns1.Team("exampleTeam",
+        example = ns1.Team("example",
+            name="Example team",
             ip_whitelists=[
                 "1.1.1.1",
                 "2.2.2.2",
             ],
             dns_view_zones=False,
             account_manage_users=False)
-        example_user = ns1.User("exampleUser",
+        example_user = ns1.User("example",
+            name="Example User",
             username="example_user",
             email="user@example.com",
-            teams=[example_team.id],
+            teams=[example.id],
             notify={
                 "billing": False,
             })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Permissions
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1/zone.py` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1.egg-info/PKG-INFO` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ns1
-Version: 3.3.0a1713333847
+Version: 3.3.0a1713561640
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi,ns1
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ns1-3.3.0a1713333847/pulumi_ns1.egg-info/SOURCES.txt` & `pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713333847/pyproject.toml` & `pulumi_ns1-3.3.0a1713561640/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_ns1"
   description = "A Pulumi package for creating and managing ns1 cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "ns1"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.3.0a1713333847"
+  version = "3.3.0a1713561640"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-ns1"
 
 [build-system]
```

