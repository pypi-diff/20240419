# Comparing `tmp/pulumi_rabbitmq-3.4.0a1713336691.tar.gz` & `tmp/pulumi_rabbitmq-3.4.0a1713561329.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rabbitmq-3.4.0a1713336691.tar", last modified: Wed Apr 17 06:59:28 2024, max compression
+gzip compressed data, was "pulumi_rabbitmq-3.4.0a1713561329.tar", last modified: Fri Apr 19 21:18:49 2024, max compression
```

## Comparing `pulumi_rabbitmq-3.4.0a1713336691.tar` & `pulumi_rabbitmq-3.4.0a1713561329.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:28.782082 pulumi_rabbitmq-3.4.0a1713336691/
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-17 06:59:28.782082 pulumi_rabbitmq-3.4.0a1713336691/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:28.778082 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41845 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20719 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:28.778082 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/federation_upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/get_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/get_v_host.py
--rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/operator_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    37993 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11613 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/shovel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/topic_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/v_host.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:59:28.782082 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-17 06:59:28.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-17 06:59:28.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:59:28.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 06:59:28.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 06:59:28.000000 pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-17 06:59:22.000000 pulumi_rabbitmq-3.4.0a1713336691/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:59:28.782082 pulumi_rabbitmq-3.4.0a1713336691/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41845 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20753 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11398 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15249 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/federation_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_v_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/operator_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37993 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/shovel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/topic_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/v_host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-19 21:18:49.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-19 21:18:49.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:18:49.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:18:49.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 21:18:49.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/setup.cfg
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1713561329/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rabbitmq
-Version: 3.4.0a1713336691
+Version: 3.4.0a1713561329
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi,rabbitmq
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/README.md` & `pulumi_rabbitmq-3.4.0a1713561329/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/__init__.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/_inputs.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/_utilities.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/binding.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,42 +275,44 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
+            user="guest",
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user="guest",
-            vhost=test_v_host.name)
-        test_exchange = rabbitmq.Exchange("testExchange",
+                read=".*",
+            ))
+        test_exchange = rabbitmq.Exchange("test",
+            name="test",
+            vhost=guest.vhost,
             settings=rabbitmq.ExchangeSettingsArgs(
-                auto_delete=True,
-                durable=False,
                 type="fanout",
-            ),
-            vhost=guest.vhost)
-        test_queue = rabbitmq.Queue("testQueue",
+                durable=False,
+                auto_delete=True,
+            ))
+        test_queue = rabbitmq.Queue("test",
+            name="test",
+            vhost=guest.vhost,
             settings=rabbitmq.QueueSettingsArgs(
-                auto_delete=False,
                 durable=True,
-            ),
-            vhost=guest.vhost)
-        test_binding = rabbitmq.Binding("testBinding",
+                auto_delete=False,
+            ))
+        test_binding = rabbitmq.Binding("test",
+            source=test_exchange.name,
+            vhost=test.name,
             destination=test_queue.name,
             destination_type="queue",
-            routing_key="#",
-            source=test_exchange.name,
-            vhost=test_v_host.name)
+            routing_key="#")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Bindings can be imported using the `id` which is composed of
           `vhost/source/destination/destination_type/properties_key`. E.g.
@@ -341,42 +343,44 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
+            user="guest",
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user="guest",
-            vhost=test_v_host.name)
-        test_exchange = rabbitmq.Exchange("testExchange",
+                read=".*",
+            ))
+        test_exchange = rabbitmq.Exchange("test",
+            name="test",
+            vhost=guest.vhost,
             settings=rabbitmq.ExchangeSettingsArgs(
-                auto_delete=True,
-                durable=False,
                 type="fanout",
-            ),
-            vhost=guest.vhost)
-        test_queue = rabbitmq.Queue("testQueue",
+                durable=False,
+                auto_delete=True,
+            ))
+        test_queue = rabbitmq.Queue("test",
+            name="test",
+            vhost=guest.vhost,
             settings=rabbitmq.QueueSettingsArgs(
-                auto_delete=False,
                 durable=True,
-            ),
-            vhost=guest.vhost)
-        test_binding = rabbitmq.Binding("testBinding",
+                auto_delete=False,
+            ))
+        test_binding = rabbitmq.Binding("test",
+            source=test_exchange.name,
+            vhost=test.name,
             destination=test_queue.name,
             destination_type="queue",
-            routing_key="#",
-            source=test_exchange.name,
-            vhost=test_v_host.name)
+            routing_key="#")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Bindings can be imported using the `id` which is composed of
           `vhost/source/destination/destination_type/properties_key`. E.g.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/config/__init__.pyi` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/config/vars.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/exchange.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,30 +143,31 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
+            user="guest",
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user="guest",
-            vhost=test_v_host.name)
-        test_exchange = rabbitmq.Exchange("testExchange",
+                read=".*",
+            ))
+        test_exchange = rabbitmq.Exchange("test",
+            name="test",
+            vhost=guest.vhost,
             settings=rabbitmq.ExchangeSettingsArgs(
-                auto_delete=True,
-                durable=False,
                 type="fanout",
-            ),
-            vhost=guest.vhost)
+                durable=False,
+                auto_delete=True,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Exchanges can be imported using the `id` which is composed of  `name@vhost`.
 
@@ -195,30 +196,31 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
+            user="guest",
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user="guest",
-            vhost=test_v_host.name)
-        test_exchange = rabbitmq.Exchange("testExchange",
+                read=".*",
+            ))
+        test_exchange = rabbitmq.Exchange("test",
+            name="test",
+            vhost=guest.vhost,
             settings=rabbitmq.ExchangeSettingsArgs(
-                auto_delete=True,
-                durable=False,
                 type="fanout",
-            ),
-            vhost=guest.vhost)
+                durable=False,
+                auto_delete=True,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Exchanges can be imported using the `id` which is composed of  `name@vhost`.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/federation_upstream.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/federation_upstream.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,45 +154,48 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test = rabbitmq.VHost("test")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
             vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
                 write=".*",
                 read=".*",
             ))
         # downstream exchange
-        foo_exchange = rabbitmq.Exchange("fooExchange",
+        foo = rabbitmq.Exchange("foo",
+            name="foo",
             vhost=guest.vhost,
             settings=rabbitmq.ExchangeSettingsArgs(
                 type="topic",
                 durable=True,
             ))
         # upstream broker
-        foo_federation_upstream = rabbitmq.FederationUpstream("fooFederationUpstream",
+        foo_federation_upstream = rabbitmq.FederationUpstream("foo",
+            name="foo",
             vhost=guest.vhost,
             definition=rabbitmq.FederationUpstreamDefinitionArgs(
                 uri="amqp://guest:guest@upstream-server-name:5672/%2f",
                 prefetch_count=1000,
                 reconnect_delay=5,
                 ack_mode="on-confirm",
                 trust_user_id=False,
                 max_hops=1,
             ))
-        foo_policy = rabbitmq.Policy("fooPolicy",
+        foo_policy = rabbitmq.Policy("foo",
+            name="foo",
             vhost=guest.vhost,
             policy=rabbitmq.PolicyPolicyArgs(
-                pattern=foo_exchange.name.apply(lambda name: f"(^{name}$)"),
+                pattern=foo.name.apply(lambda name: f"(^{name}$)"),
                 priority=1,
                 apply_to="exchanges",
                 definition={
                     "federation-upstream": foo_federation_upstream.name,
                 },
             ))
         ```
@@ -224,45 +227,48 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test = rabbitmq.VHost("test")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
             vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
                 write=".*",
                 read=".*",
             ))
         # downstream exchange
-        foo_exchange = rabbitmq.Exchange("fooExchange",
+        foo = rabbitmq.Exchange("foo",
+            name="foo",
             vhost=guest.vhost,
             settings=rabbitmq.ExchangeSettingsArgs(
                 type="topic",
                 durable=True,
             ))
         # upstream broker
-        foo_federation_upstream = rabbitmq.FederationUpstream("fooFederationUpstream",
+        foo_federation_upstream = rabbitmq.FederationUpstream("foo",
+            name="foo",
             vhost=guest.vhost,
             definition=rabbitmq.FederationUpstreamDefinitionArgs(
                 uri="amqp://guest:guest@upstream-server-name:5672/%2f",
                 prefetch_count=1000,
                 reconnect_delay=5,
                 ack_mode="on-confirm",
                 trust_user_id=False,
                 max_hops=1,
             ))
-        foo_policy = rabbitmq.Policy("fooPolicy",
+        foo_policy = rabbitmq.Policy("foo",
+            name="foo",
             vhost=guest.vhost,
             policy=rabbitmq.PolicyPolicyArgs(
-                pattern=foo_exchange.name.apply(lambda name: f"(^{name}$)"),
+                pattern=foo.name.apply(lambda name: f"(^{name}$)"),
                 priority=1,
                 apply_to="exchanges",
                 definition={
                     "federation-upstream": foo_federation_upstream.name,
                 },
             ))
         ```
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/get_exchange.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/get_user.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/get_v_host.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_v_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/operator_policy.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/operator_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,34 +142,35 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
+            user="guest",
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user="guest",
-            vhost=test_v_host.name)
-        test_operator_policy = rabbitmq.OperatorPolicy("testOperatorPolicy",
+                read=".*",
+            ))
+        test_operator_policy = rabbitmq.OperatorPolicy("test",
+            name="test",
+            vhost=guest.vhost,
             policy=rabbitmq.OperatorPolicyPolicyArgs(
+                pattern=".*",
+                priority=0,
                 apply_to="queues",
                 definition={
-                    "expires": 1800000,
                     "message-ttl": 3600000,
+                    "expires": 1800000,
                 },
-                pattern=".*",
-                priority=0,
-            ),
-            vhost=guest.vhost)
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Operator policies can be imported using the `id` which is composed of `name@vhost`.
 
@@ -198,34 +199,35 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
+            user="guest",
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user="guest",
-            vhost=test_v_host.name)
-        test_operator_policy = rabbitmq.OperatorPolicy("testOperatorPolicy",
+                read=".*",
+            ))
+        test_operator_policy = rabbitmq.OperatorPolicy("test",
+            name="test",
+            vhost=guest.vhost,
             policy=rabbitmq.OperatorPolicyPolicyArgs(
+                pattern=".*",
+                priority=0,
                 apply_to="queues",
                 definition={
-                    "expires": 1800000,
                     "message-ttl": 3600000,
+                    "expires": 1800000,
                 },
-                pattern=".*",
-                priority=0,
-            ),
-            vhost=guest.vhost)
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Operator policies can be imported using the `id` which is composed of `name@vhost`.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/outputs.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/permissions.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/permissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,26 +143,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
-        test_user = rabbitmq.User("testUser",
+        test = rabbitmq.VHost("test", name="test")
+        test_user = rabbitmq.User("test",
+            name="mctest",
             password="foobar",
             tags=["administrator"])
-        test_permissions = rabbitmq.Permissions("testPermissions",
+        test_permissions = rabbitmq.Permissions("test",
+            user=test_user.name,
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user=test_user.name,
-            vhost=test_v_host.name)
+                read=".*",
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Permissions can be imported using the `id` which is composed of  `user@vhost`.
 
@@ -192,26 +193,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
-        test_user = rabbitmq.User("testUser",
+        test = rabbitmq.VHost("test", name="test")
+        test_user = rabbitmq.User("test",
+            name="mctest",
             password="foobar",
             tags=["administrator"])
-        test_permissions = rabbitmq.Permissions("testPermissions",
+        test_permissions = rabbitmq.Permissions("test",
+            user=test_user.name,
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user=test_user.name,
-            vhost=test_v_host.name)
+                read=".*",
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Permissions can be imported using the `id` which is composed of  `user@vhost`.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/policy.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,33 +143,34 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
+            user="guest",
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user="guest",
-            vhost=test_v_host.name)
-        test_policy = rabbitmq.Policy("testPolicy",
+                read=".*",
+            ))
+        test_policy = rabbitmq.Policy("test",
+            name="test",
+            vhost=guest.vhost,
             policy=rabbitmq.PolicyPolicyArgs(
+                pattern=".*",
+                priority=0,
                 apply_to="all",
                 definition={
                     "ha-mode": "all",
                 },
-                pattern=".*",
-                priority=0,
-            ),
-            vhost=guest.vhost)
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Policies can be imported using the `id` which is composed of `name@vhost`.
 
@@ -199,33 +200,34 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
+            user="guest",
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user="guest",
-            vhost=test_v_host.name)
-        test_policy = rabbitmq.Policy("testPolicy",
+                read=".*",
+            ))
+        test_policy = rabbitmq.Policy("test",
+            name="test",
+            vhost=guest.vhost,
             policy=rabbitmq.PolicyPolicyArgs(
+                pattern=".*",
+                priority=0,
                 apply_to="all",
                 definition={
                     "ha-mode": "all",
                 },
-                pattern=".*",
-                priority=0,
-            ),
-            vhost=guest.vhost)
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Policies can be imported using the `id` which is composed of `name@vhost`.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/provider.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/queue.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,24 +145,25 @@
         ### Basic Example
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
-            vhost=test_v_host.name,
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
                 write=".*",
                 read=".*",
             ))
-        test_queue = rabbitmq.Queue("testQueue",
+        test_queue = rabbitmq.Queue("test",
+            name="test",
             vhost=guest.vhost,
             settings=rabbitmq.QueueSettingsArgs(
                 durable=False,
                 auto_delete=True,
                 arguments={
                     "x-queue-type": "quorum",
                 },
@@ -179,32 +180,32 @@
 
         config = pulumi.Config()
         arguments = config.get("arguments")
         if arguments is None:
             arguments = \"\"\"{
           "x-message-ttl": 5000
         }
-
         \"\"\"
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
+            user="guest",
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user="guest",
-            vhost=test_v_host.name)
-        test_queue = rabbitmq.Queue("testQueue",
+                read=".*",
+            ))
+        test_queue = rabbitmq.Queue("test",
+            name="test",
+            vhost=guest.vhost,
             settings=rabbitmq.QueueSettingsArgs(
-                arguments_json=arguments,
-                auto_delete=True,
                 durable=False,
-            ),
-            vhost=guest.vhost)
+                auto_delete=True,
+                arguments_json=arguments,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Queues can be imported using the `id` which is composed of `name@vhost`. E.g.
 
@@ -233,24 +234,25 @@
         ### Basic Example
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
-            vhost=test_v_host.name,
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
                 write=".*",
                 read=".*",
             ))
-        test_queue = rabbitmq.Queue("testQueue",
+        test_queue = rabbitmq.Queue("test",
+            name="test",
             vhost=guest.vhost,
             settings=rabbitmq.QueueSettingsArgs(
                 durable=False,
                 auto_delete=True,
                 arguments={
                     "x-queue-type": "quorum",
                 },
@@ -267,32 +269,32 @@
 
         config = pulumi.Config()
         arguments = config.get("arguments")
         if arguments is None:
             arguments = \"\"\"{
           "x-message-ttl": 5000
         }
-
         \"\"\"
-        test_v_host = rabbitmq.VHost("testVHost")
+        test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
+            user="guest",
+            vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
-                read=".*",
                 write=".*",
-            ),
-            user="guest",
-            vhost=test_v_host.name)
-        test_queue = rabbitmq.Queue("testQueue",
+                read=".*",
+            ))
+        test_queue = rabbitmq.Queue("test",
+            name="test",
+            vhost=guest.vhost,
             settings=rabbitmq.QueueSettingsArgs(
-                arguments_json=arguments,
-                auto_delete=True,
                 durable=False,
-            ),
-            vhost=guest.vhost)
+                auto_delete=True,
+                arguments_json=arguments,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Queues can be imported using the `id` which is composed of `name@vhost`. E.g.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/shovel.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/shovel.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,37 +142,40 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
-        test_exchange = rabbitmq.Exchange("testExchange",
+        test = rabbitmq.VHost("test", name="test")
+        test_exchange = rabbitmq.Exchange("test",
+            name="test_exchange",
+            vhost=test.name,
             settings=rabbitmq.ExchangeSettingsArgs(
-                auto_delete=True,
-                durable=False,
                 type="fanout",
-            ),
-            vhost=test_v_host.name)
-        test_queue = rabbitmq.Queue("testQueue",
-            settings=rabbitmq.QueueSettingsArgs(
+                durable=False,
                 auto_delete=True,
+            ))
+        test_queue = rabbitmq.Queue("test",
+            name="test_queue",
+            vhost=test.name,
+            settings=rabbitmq.QueueSettingsArgs(
                 durable=False,
-            ),
-            vhost=test_v_host.name)
+                auto_delete=True,
+            ))
         shovel_test = rabbitmq.Shovel("shovelTest",
+            name="shovelTest",
+            vhost=test.name,
             info=rabbitmq.ShovelInfoArgs(
-                destination_queue=test_queue.name,
-                destination_uri="amqp:///test",
+                source_uri="amqp:///test",
                 source_exchange=test_exchange.name,
                 source_exchange_key="test",
-                source_uri="amqp:///test",
-            ),
-            vhost=test_v_host.name)
+                destination_uri="amqp:///test",
+                destination_queue=test_queue.name,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Shovels can be imported using the `name` and `vhost`
 
@@ -201,37 +204,40 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
-        test_exchange = rabbitmq.Exchange("testExchange",
+        test = rabbitmq.VHost("test", name="test")
+        test_exchange = rabbitmq.Exchange("test",
+            name="test_exchange",
+            vhost=test.name,
             settings=rabbitmq.ExchangeSettingsArgs(
-                auto_delete=True,
-                durable=False,
                 type="fanout",
-            ),
-            vhost=test_v_host.name)
-        test_queue = rabbitmq.Queue("testQueue",
-            settings=rabbitmq.QueueSettingsArgs(
+                durable=False,
                 auto_delete=True,
+            ))
+        test_queue = rabbitmq.Queue("test",
+            name="test_queue",
+            vhost=test.name,
+            settings=rabbitmq.QueueSettingsArgs(
                 durable=False,
-            ),
-            vhost=test_v_host.name)
+                auto_delete=True,
+            ))
         shovel_test = rabbitmq.Shovel("shovelTest",
+            name="shovelTest",
+            vhost=test.name,
             info=rabbitmq.ShovelInfoArgs(
-                destination_queue=test_queue.name,
-                destination_uri="amqp:///test",
+                source_uri="amqp:///test",
                 source_exchange=test_exchange.name,
                 source_exchange_key="test",
-                source_uri="amqp:///test",
-            ),
-            vhost=test_v_host.name)
+                destination_uri="amqp:///test",
+                destination_queue=test_queue.name,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Shovels can be imported using the `name` and `vhost`
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/topic_permissions.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/topic_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,26 +143,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
-        test_user = rabbitmq.User("testUser",
+        test = rabbitmq.VHost("test", name="test")
+        test_user = rabbitmq.User("test",
+            name="mctest",
             password="foobar",
             tags=["administrator"])
-        test_topic_permissions = rabbitmq.TopicPermissions("testTopicPermissions",
+        test_topic_permissions = rabbitmq.TopicPermissions("test",
+            user=test_user.name,
+            vhost=test.name,
             permissions=[rabbitmq.TopicPermissionsPermissionArgs(
                 exchange="amq.topic",
-                read=".*",
                 write=".*",
-            )],
-            user=test_user.name,
-            vhost=test_v_host.name)
+                read=".*",
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Permissions can be imported using the `id` which is composed of  `user@vhost`.
 
@@ -192,26 +193,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        test_v_host = rabbitmq.VHost("testVHost")
-        test_user = rabbitmq.User("testUser",
+        test = rabbitmq.VHost("test", name="test")
+        test_user = rabbitmq.User("test",
+            name="mctest",
             password="foobar",
             tags=["administrator"])
-        test_topic_permissions = rabbitmq.TopicPermissions("testTopicPermissions",
+        test_topic_permissions = rabbitmq.TopicPermissions("test",
+            user=test_user.name,
+            vhost=test.name,
             permissions=[rabbitmq.TopicPermissionsPermissionArgs(
                 exchange="amq.topic",
-                read=".*",
                 write=".*",
-            )],
-            user=test_user.name,
-            vhost=test_v_host.name)
+                read=".*",
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Permissions can be imported using the `id` which is composed of  `user@vhost`.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/user.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.User("test",
+            name="mctest",
             password="foobar",
             tags=[
                 "administrator",
                 "management",
             ])
         ```
         <!--End PulumiCodeChooser -->
@@ -193,14 +194,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.User("test",
+            name="mctest",
             password="foobar",
             tags=[
                 "administrator",
                 "management",
             ])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq/v_host.py` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/v_host.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        my_vhost = rabbitmq.VHost("myVhost")
+        my_vhost = rabbitmq.VHost("my_vhost", name="my_vhost")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Vhosts can be imported using the `name`, e.g.
 
@@ -104,15 +104,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
-        my_vhost = rabbitmq.VHost("myVhost")
+        my_vhost = rabbitmq.VHost("my_vhost", name="my_vhost")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Vhosts can be imported using the `name`, e.g.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq.egg-info/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rabbitmq
-Version: 3.4.0a1713336691
+Version: 3.4.0a1713561329
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi,rabbitmq
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pulumi_rabbitmq.egg-info/SOURCES.txt` & `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713336691/pyproject.toml` & `pulumi_rabbitmq-3.4.0a1713561329/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rabbitmq"
   description = "A Pulumi package for creating and managing RabbitMQ resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rabbitmq"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.4.0a1713336691"
+  version = "3.4.0a1713561329"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rabbitmq"
 
 [build-system]
```

