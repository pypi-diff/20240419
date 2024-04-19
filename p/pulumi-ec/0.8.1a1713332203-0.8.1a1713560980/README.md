# Comparing `tmp/pulumi_ec-0.8.1a1713332203.tar.gz` & `tmp/pulumi_ec-0.8.1a1713560980.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ec-0.8.1a1713332203.tar", last modified: Wed Apr 17 05:44:43 2024, max compression
+gzip compressed data, was "pulumi_ec-0.8.1a1713560980.tar", last modified: Fri Apr 19 21:12:28 2024, max compression
```

## Comparing `pulumi_ec-0.8.1a1713332203.tar` & `pulumi_ec-0.8.1a1713560980.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:44:43.760062 pulumi_ec-0.8.1a1713332203/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-17 05:44:43.760062 pulumi_ec-0.8.1a1713332203/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:44:43.756062 pulumi_ec-0.8.1a1713332203/pulumi_ec/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   224309 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:44:43.760062 pulumi_ec-0.8.1a1713332203/pulumi_ec/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    58094 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    18785 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/deployment_elasticsearch_keystore.py
--rw-r--r--   0 runner    (1001) docker     (127)    23082 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/deployment_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    23937 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/deployment_traffic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/deployment_traffic_filter_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/get_aws_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/get_azure_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/get_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/get_deployment_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/get_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/get_gcp_private_service_connect_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/get_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/get_traffic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)   298706 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12554 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec/snapshot_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:44:43.760062 pulumi_ec-0.8.1a1713332203/pulumi_ec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-17 05:44:43.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 05:44:43.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:44:43.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 05:44:43.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 05:44:43.000000 pulumi_ec-0.8.1a1713332203/pulumi_ec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-17 05:44:36.000000 pulumi_ec-0.8.1a1713332203/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:44:43.760062 pulumi_ec-0.8.1a1713332203/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:12:28.270733 pulumi_ec-0.8.1a1713560980/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-19 21:12:28.270733 pulumi_ec-0.8.1a1713560980/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:12:28.266733 pulumi_ec-0.8.1a1713560980/pulumi_ec/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   224309 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:12:28.270733 pulumi_ec-0.8.1a1713560980/pulumi_ec/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58094 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18881 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/deployment_elasticsearch_keystore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23082 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/deployment_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24455 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/deployment_traffic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/deployment_traffic_filter_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/get_aws_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/get_azure_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/get_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/get_deployment_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15822 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/get_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/get_gcp_private_service_connect_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/get_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/get_traffic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)   298706 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12886 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec/snapshot_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:12:28.270733 pulumi_ec-0.8.1a1713560980/pulumi_ec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-19 21:12:28.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-19 21:12:28.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:12:28.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:12:28.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 21:12:28.000000 pulumi_ec-0.8.1a1713560980/pulumi_ec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-19 21:12:21.000000 pulumi_ec-0.8.1a1713560980/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:12:28.270733 pulumi_ec-0.8.1a1713560980/setup.cfg
```

### Comparing `pulumi_ec-0.8.1a1713332203/PKG-INFO` & `pulumi_ec-0.8.1a1713560980/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ec
-Version: 0.8.1a1713332203
+Version: 0.8.1a1713560980
 Summary: A Pulumi package for creating and managing ElasticCloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ec
 Keywords: pulumi,ec,elasticsearch,es,elastic,elasticcloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ec-0.8.1a1713332203/README.md` & `pulumi_ec-0.8.1a1713560980/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/__init__.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/_inputs.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/_utilities.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/config/__init__.pyi` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/config/vars.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/deployment.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/deployment_elasticsearch_keystore.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/deployment_elasticsearch_keystore.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,60 +167,62 @@
 
         ### Basic
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ec as ec
+        import pulumi_std as std
 
         latest = ec.get_stack(version_regex="latest",
             region="us-east-1")
         # Create an Elastic Cloud deployment
-        example_keystore = ec.Deployment("exampleKeystore",
+        example_keystore = ec.Deployment("example_keystore",
             region="us-east-1",
             version=latest.version,
             deployment_template_id="aws-io-optimized-v2",
             elasticsearch=ec.DeploymentElasticsearchArgs(
                 hot=ec.DeploymentElasticsearchHotArgs(
                     autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
                 ),
             ))
         # Create the keystore secret entry
-        gcs_credential = ec.DeploymentElasticsearchKeystore("gcsCredential",
+        gcs_credential = ec.DeploymentElasticsearchKeystore("gcs_credential",
             deployment_id=example_keystore.id,
             setting_name="gcs.client.default.credentials_file",
-            value=(lambda path: open(path).read())("service-account-key.json"),
+            value=std.file(input="service-account-key.json").result,
             as_file=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Adding credentials to use GCS as a snapshot repository
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ec as ec
+        import pulumi_std as std
 
         latest = ec.get_stack(version_regex="latest",
             region="us-east-1")
         # Create an Elastic Cloud deployment
-        example_keystore = ec.Deployment("exampleKeystore",
+        example_keystore = ec.Deployment("example_keystore",
             region="us-east-1",
             version=latest.version,
             deployment_template_id="aws-io-optimized-v2",
             elasticsearch=ec.DeploymentElasticsearchArgs(
                 hot=ec.DeploymentElasticsearchHotArgs(
                     autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
                 ),
             ))
         # Create the keystore secret entry
-        gcs_credential = ec.DeploymentElasticsearchKeystore("gcsCredential",
+        gcs_credential = ec.DeploymentElasticsearchKeystore("gcs_credential",
             deployment_id=example_keystore.id,
             setting_name="gcs.client.default.credentials_file",
-            value=(lambda path: open(path).read())("service-account-key.json"),
+            value=std.file(input="service-account-key.json").result,
             as_file=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource cannot be imported
@@ -243,60 +245,62 @@
 
         ### Basic
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ec as ec
+        import pulumi_std as std
 
         latest = ec.get_stack(version_regex="latest",
             region="us-east-1")
         # Create an Elastic Cloud deployment
-        example_keystore = ec.Deployment("exampleKeystore",
+        example_keystore = ec.Deployment("example_keystore",
             region="us-east-1",
             version=latest.version,
             deployment_template_id="aws-io-optimized-v2",
             elasticsearch=ec.DeploymentElasticsearchArgs(
                 hot=ec.DeploymentElasticsearchHotArgs(
                     autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
                 ),
             ))
         # Create the keystore secret entry
-        gcs_credential = ec.DeploymentElasticsearchKeystore("gcsCredential",
+        gcs_credential = ec.DeploymentElasticsearchKeystore("gcs_credential",
             deployment_id=example_keystore.id,
             setting_name="gcs.client.default.credentials_file",
-            value=(lambda path: open(path).read())("service-account-key.json"),
+            value=std.file(input="service-account-key.json").result,
             as_file=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Adding credentials to use GCS as a snapshot repository
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ec as ec
+        import pulumi_std as std
 
         latest = ec.get_stack(version_regex="latest",
             region="us-east-1")
         # Create an Elastic Cloud deployment
-        example_keystore = ec.Deployment("exampleKeystore",
+        example_keystore = ec.Deployment("example_keystore",
             region="us-east-1",
             version=latest.version,
             deployment_template_id="aws-io-optimized-v2",
             elasticsearch=ec.DeploymentElasticsearchArgs(
                 hot=ec.DeploymentElasticsearchHotArgs(
                     autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
                 ),
             ))
         # Create the keystore secret entry
-        gcs_credential = ec.DeploymentElasticsearchKeystore("gcsCredential",
+        gcs_credential = ec.DeploymentElasticsearchKeystore("gcs_credential",
             deployment_id=example_keystore.id,
             setting_name="gcs.client.default.credentials_file",
-            value=(lambda path: open(path).read())("service-account-key.json"),
+            value=std.file(input="service-account-key.json").result,
             as_file=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         This resource cannot be imported
```

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/deployment_extension.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/deployment_extension.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/deployment_traffic_filter.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/deployment_traffic_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,21 +240,23 @@
         ```python
         import pulumi
         import pulumi_ec as ec
 
         latest = ec.get_stack(version_regex="latest",
             region="us-east-1")
         example = ec.DeploymentTrafficFilter("example",
+            name="my traffic filter name",
             region="us-east-1",
             type="ip",
             rules=[ec.DeploymentTrafficFilterRuleArgs(
                 source="0.0.0.0/0",
             )])
         # Create an Elastic Cloud deployment
-        example_minimal = ec.Deployment("exampleMinimal",
+        example_minimal = ec.Deployment("example_minimal",
+            name="my_example_deployment",
             region="us-east-1",
             version=latest.version,
             deployment_template_id="aws-io-optimized-v2",
             traffic_filters=[example.id],
             elasticsearch=ec.DeploymentElasticsearchArgs(
                 hot=ec.DeploymentElasticsearchHotArgs(
                     autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
@@ -271,22 +273,24 @@
         import pulumi
         import pulumi_ec as ec
 
         region = azure_australiaeast
         latest = ec.get_stack(version_regex="latest",
             region=region)
         azure = ec.DeploymentTrafficFilter("azure",
+            name="my traffic filter name",
             region=region,
             type="azure_private_endpoint",
             rules=[ec.DeploymentTrafficFilterRuleArgs(
                 azure_endpoint_name="my-azure-pl",
                 azure_endpoint_guid="78c64959-fd88-41cc-81ac-1cfcdb1ac32e",
             )])
         # Create an Elastic Cloud deployment
-        example_minimal = ec.Deployment("exampleMinimal",
+        example_minimal = ec.Deployment("example_minimal",
+            name="my_example_deployment",
             region=region,
             version=latest.version,
             deployment_template_id="azure-io-optimized-v3",
             traffic_filters=[azure.id],
             elasticsearch=ec.DeploymentElasticsearchArgs(
                 hot=ec.DeploymentElasticsearchHotArgs(
                     autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
@@ -302,22 +306,24 @@
         ```python
         import pulumi
         import pulumi_ec as ec
 
         region = asia_east1
         latest = ec.get_stack(version_regex="latest",
             region=region)
-        gcp_psc = ec.DeploymentTrafficFilter("gcpPsc",
+        gcp_psc = ec.DeploymentTrafficFilter("gcp_psc",
+            name="my traffic filter name",
             region=region,
             type="gcp_private_service_connect_endpoint",
             rules=[ec.DeploymentTrafficFilterRuleArgs(
                 source="18446744072646845332",
             )])
         # Create an Elastic Cloud deployment
-        example_minimal = ec.Deployment("exampleMinimal",
+        example_minimal = ec.Deployment("example_minimal",
+            name="my_example_deployment",
             region=region,
             version=latest.version,
             deployment_template_id="gcp-storage-optimized",
             traffic_filters=[gcp_psc.id],
             elasticsearch=ec.DeploymentElasticsearchArgs(
                 hot=ec.DeploymentElasticsearchHotArgs(
                     autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
@@ -359,21 +365,23 @@
         ```python
         import pulumi
         import pulumi_ec as ec
 
         latest = ec.get_stack(version_regex="latest",
             region="us-east-1")
         example = ec.DeploymentTrafficFilter("example",
+            name="my traffic filter name",
             region="us-east-1",
             type="ip",
             rules=[ec.DeploymentTrafficFilterRuleArgs(
                 source="0.0.0.0/0",
             )])
         # Create an Elastic Cloud deployment
-        example_minimal = ec.Deployment("exampleMinimal",
+        example_minimal = ec.Deployment("example_minimal",
+            name="my_example_deployment",
             region="us-east-1",
             version=latest.version,
             deployment_template_id="aws-io-optimized-v2",
             traffic_filters=[example.id],
             elasticsearch=ec.DeploymentElasticsearchArgs(
                 hot=ec.DeploymentElasticsearchHotArgs(
                     autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
@@ -390,22 +398,24 @@
         import pulumi
         import pulumi_ec as ec
 
         region = azure_australiaeast
         latest = ec.get_stack(version_regex="latest",
             region=region)
         azure = ec.DeploymentTrafficFilter("azure",
+            name="my traffic filter name",
             region=region,
             type="azure_private_endpoint",
             rules=[ec.DeploymentTrafficFilterRuleArgs(
                 azure_endpoint_name="my-azure-pl",
                 azure_endpoint_guid="78c64959-fd88-41cc-81ac-1cfcdb1ac32e",
             )])
         # Create an Elastic Cloud deployment
-        example_minimal = ec.Deployment("exampleMinimal",
+        example_minimal = ec.Deployment("example_minimal",
+            name="my_example_deployment",
             region=region,
             version=latest.version,
             deployment_template_id="azure-io-optimized-v3",
             traffic_filters=[azure.id],
             elasticsearch=ec.DeploymentElasticsearchArgs(
                 hot=ec.DeploymentElasticsearchHotArgs(
                     autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
@@ -421,22 +431,24 @@
         ```python
         import pulumi
         import pulumi_ec as ec
 
         region = asia_east1
         latest = ec.get_stack(version_regex="latest",
             region=region)
-        gcp_psc = ec.DeploymentTrafficFilter("gcpPsc",
+        gcp_psc = ec.DeploymentTrafficFilter("gcp_psc",
+            name="my traffic filter name",
             region=region,
             type="gcp_private_service_connect_endpoint",
             rules=[ec.DeploymentTrafficFilterRuleArgs(
                 source="18446744072646845332",
             )])
         # Create an Elastic Cloud deployment
-        example_minimal = ec.Deployment("exampleMinimal",
+        example_minimal = ec.Deployment("example_minimal",
+            name="my_example_deployment",
             region=region,
             version=latest.version,
             deployment_template_id="gcp-storage-optimized",
             traffic_filters=[gcp_psc.id],
             elasticsearch=ec.DeploymentElasticsearchArgs(
                 hot=ec.DeploymentElasticsearchHotArgs(
                     autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
```

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/deployment_traffic_filter_association.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/deployment_traffic_filter_association.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,24 +101,25 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ec as ec
 
-        example_deployment = ec.get_deployment(id="320b7b540dfc967a7a649c18e2fce4ed")
-        example_deployment_traffic_filter = ec.DeploymentTrafficFilter("exampleDeploymentTrafficFilter",
+        example = ec.get_deployment(id="320b7b540dfc967a7a649c18e2fce4ed")
+        example_deployment_traffic_filter = ec.DeploymentTrafficFilter("example",
+            name="my traffic filter name",
             region="us-east-1",
             type="ip",
             rules=[ec.DeploymentTrafficFilterRuleArgs(
                 source="0.0.0.0/0",
             )])
-        example_deployment_traffic_filter_association = ec.DeploymentTrafficFilterAssociation("exampleDeploymentTrafficFilterAssociation",
+        example_deployment_traffic_filter_association = ec.DeploymentTrafficFilterAssociation("example",
             traffic_filter_id=example_deployment_traffic_filter.id,
-            deployment_id=ec_deployment["example"]["id"])
+            deployment_id=example_ec_deployment["id"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Import is not supported on this resource
 
@@ -137,24 +138,25 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ec as ec
 
-        example_deployment = ec.get_deployment(id="320b7b540dfc967a7a649c18e2fce4ed")
-        example_deployment_traffic_filter = ec.DeploymentTrafficFilter("exampleDeploymentTrafficFilter",
+        example = ec.get_deployment(id="320b7b540dfc967a7a649c18e2fce4ed")
+        example_deployment_traffic_filter = ec.DeploymentTrafficFilter("example",
+            name="my traffic filter name",
             region="us-east-1",
             type="ip",
             rules=[ec.DeploymentTrafficFilterRuleArgs(
                 source="0.0.0.0/0",
             )])
-        example_deployment_traffic_filter_association = ec.DeploymentTrafficFilterAssociation("exampleDeploymentTrafficFilterAssociation",
+        example_deployment_traffic_filter_association = ec.DeploymentTrafficFilterAssociation("example",
             traffic_filter_id=example_deployment_traffic_filter.id,
-            deployment_id=ec_deployment["example"]["id"])
+            deployment_id=example_ec_deployment["id"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Import is not supported on this resource
```

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/get_aws_privatelink_endpoint.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/get_aws_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/get_azure_privatelink_endpoint.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/get_azure_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/get_deployment.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/get_deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/get_deployment_templates.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/get_deployment_templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,18 +105,19 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ec as ec
 
     example = ec.get_deployment_templates(region="us-east-1")
-    my_deployment = ec.Deployment("myDeployment",
+    my_deployment = ec.Deployment("my_deployment",
+        name="My Deployment",
         version="8.12.2",
-        region=data["ec_deployment_templates"]["all_templates"]["region"],
-        deployment_template_id=data["ec_deployment_templates"]["all_templates"]["templates"][0]["id"],
+        region=all_templates["region"],
+        deployment_template_id=all_templates["templates"][0]["id"],
         elasticsearch=ec.DeploymentElasticsearchArgs(
             hot=ec.DeploymentElasticsearchHotArgs(
                 autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
             ),
         ),
         kibana=ec.DeploymentKibanaArgs())
     ```
@@ -157,18 +158,19 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ec as ec
 
     example = ec.get_deployment_templates(region="us-east-1")
-    my_deployment = ec.Deployment("myDeployment",
+    my_deployment = ec.Deployment("my_deployment",
+        name="My Deployment",
         version="8.12.2",
-        region=data["ec_deployment_templates"]["all_templates"]["region"],
-        deployment_template_id=data["ec_deployment_templates"]["all_templates"]["templates"][0]["id"],
+        region=all_templates["region"],
+        deployment_template_id=all_templates["templates"][0]["id"],
         elasticsearch=ec.DeploymentElasticsearchArgs(
             hot=ec.DeploymentElasticsearchHotArgs(
                 autoscaling=ec.DeploymentElasticsearchHotAutoscalingArgs(),
             ),
         ),
         kibana=ec.DeploymentKibanaArgs())
     ```
```

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/get_deployments.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/get_deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,32 +220,32 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ec as ec
 
-    example = ec.get_deployments(deployment_template_id="azure-compute-optimized",
+    example = ec.get_deployments(name_prefix="test",
+        deployment_template_id="azure-compute-optimized",
+        size=200,
+        tags={
+            "foo": "bar",
+        },
         elasticsearches=[ec.GetDeploymentsElasticsearchArgs(
             healthy="true",
         )],
-        enterprise_searches=[ec.GetDeploymentsEnterpriseSearchArgs(
-            healthy="true",
+        kibanas=[ec.GetDeploymentsKibanaArgs(
+            status="started",
         )],
         integrations_servers=[ec.GetDeploymentsIntegrationsServerArgs(
             version="8.0.0",
         )],
-        kibanas=[ec.GetDeploymentsKibanaArgs(
-            status="started",
-        )],
-        name_prefix="test",
-        size=200,
-        tags={
-            "foo": "bar",
-        })
+        enterprise_searches=[ec.GetDeploymentsEnterpriseSearchArgs(
+            healthy="true",
+        )])
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetDeploymentsApmArgs']] apms: Filter by APM resource kind status or configuration.
     :param str deployment_template_id: Filter the result set by the ID of the deployment template the deployment is based off.
     :param Sequence[pulumi.InputType['GetDeploymentsElasticsearchArgs']] elasticsearches: Filter by Elasticsearch resource kind status or configuration.
@@ -309,32 +309,32 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ec as ec
 
-    example = ec.get_deployments(deployment_template_id="azure-compute-optimized",
+    example = ec.get_deployments(name_prefix="test",
+        deployment_template_id="azure-compute-optimized",
+        size=200,
+        tags={
+            "foo": "bar",
+        },
         elasticsearches=[ec.GetDeploymentsElasticsearchArgs(
             healthy="true",
         )],
-        enterprise_searches=[ec.GetDeploymentsEnterpriseSearchArgs(
-            healthy="true",
+        kibanas=[ec.GetDeploymentsKibanaArgs(
+            status="started",
         )],
         integrations_servers=[ec.GetDeploymentsIntegrationsServerArgs(
             version="8.0.0",
         )],
-        kibanas=[ec.GetDeploymentsKibanaArgs(
-            status="started",
-        )],
-        name_prefix="test",
-        size=200,
-        tags={
-            "foo": "bar",
-        })
+        enterprise_searches=[ec.GetDeploymentsEnterpriseSearchArgs(
+            healthy="true",
+        )])
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetDeploymentsApmArgs']] apms: Filter by APM resource kind status or configuration.
     :param str deployment_template_id: Filter the result set by the ID of the deployment template the deployment is based off.
     :param Sequence[pulumi.InputType['GetDeploymentsElasticsearchArgs']] elasticsearches: Filter by Elasticsearch resource kind status or configuration.
```

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/get_gcp_private_service_connect_endpoint.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/get_gcp_private_service_connect_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/get_stack.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/get_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,19 +201,19 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ec as ec
 
-    latest = ec.get_stack(lock=True,
+    latest = ec.get_stack(version_regex="latest",
         region="us-east-1",
-        version_regex="latest")
-    latest_patch = ec.get_stack(region="us-east-1",
-        version_regex="7.9.?")
+        lock=True)
+    latest_patch = ec.get_stack(version_regex="7.9.?",
+        region="us-east-1")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param bool lock: Lock the `latest` `version_regex` obtained, so that the new stack release doesn't cascade the changes down to the deployments. It can be changed at any time.
     :param str region: Region where the stack pack is. For Elastic Cloud Enterprise (ECE) installations, use `ece-region`.
     :param str version_regex: Regex to filter the available stacks. Can be any valid regex expression, when multiple stacks are matched through a regex, the latest version is returned. `latest` is also accepted to obtain the latest available stack version.
@@ -254,19 +254,19 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ec as ec
 
-    latest = ec.get_stack(lock=True,
+    latest = ec.get_stack(version_regex="latest",
         region="us-east-1",
-        version_regex="latest")
-    latest_patch = ec.get_stack(region="us-east-1",
-        version_regex="7.9.?")
+        lock=True)
+    latest_patch = ec.get_stack(version_regex="7.9.?",
+        region="us-east-1")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param bool lock: Lock the `latest` `version_regex` obtained, so that the new stack release doesn't cascade the changes down to the deployments. It can be changed at any time.
     :param str region: Region where the stack pack is. For Elastic Cloud Enterprise (ECE) installations, use `ece-region`.
     :param str version_regex: Regex to filter the available stacks. Can be any valid regex expression, when multiple stacks are matched through a regex, the latest version is returned. `latest` is also accepted to obtain the latest available stack version.
```

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/get_traffic_filter.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/get_traffic_filter.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/outputs.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/provider.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec/snapshot_repository.py` & `pulumi_ec-0.8.1a1713560980/pulumi_ec/snapshot_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,41 +145,45 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_ec as ec
 
-        this = ec.SnapshotRepository("this", generic=ec.SnapshotRepositoryGenericArgs(
-            type="azure",
-            settings=json.dumps({
-                "container": "my_container",
-                "client": "my_alternate_client",
-                "compress": False,
-            }),
-        ))
+        this = ec.SnapshotRepository("this",
+            name="my-snapshot-repository",
+            generic=ec.SnapshotRepositoryGenericArgs(
+                type="azure",
+                settings=json.dumps({
+                    "container": "my_container",
+                    "client": "my_alternate_client",
+                    "compress": False,
+                }),
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### GCS
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_ec as ec
 
-        this = ec.SnapshotRepository("this", generic=ec.SnapshotRepositoryGenericArgs(
-            type="gcs",
-            settings=json.dumps({
-                "bucket": "my_bucket",
-                "client": "my_alternate_client",
-                "compress": False,
-            }),
-        ))
+        this = ec.SnapshotRepository("this",
+            name="my-snapshot-repository",
+            generic=ec.SnapshotRepositoryGenericArgs(
+                type="gcs",
+                settings=json.dumps({
+                    "bucket": "my_bucket",
+                    "client": "my_alternate_client",
+                    "compress": False,
+                }),
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         You can import snapshot repositories using the `name`, for example:
 
@@ -210,41 +214,45 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_ec as ec
 
-        this = ec.SnapshotRepository("this", generic=ec.SnapshotRepositoryGenericArgs(
-            type="azure",
-            settings=json.dumps({
-                "container": "my_container",
-                "client": "my_alternate_client",
-                "compress": False,
-            }),
-        ))
+        this = ec.SnapshotRepository("this",
+            name="my-snapshot-repository",
+            generic=ec.SnapshotRepositoryGenericArgs(
+                type="azure",
+                settings=json.dumps({
+                    "container": "my_container",
+                    "client": "my_alternate_client",
+                    "compress": False,
+                }),
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### GCS
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_ec as ec
 
-        this = ec.SnapshotRepository("this", generic=ec.SnapshotRepositoryGenericArgs(
-            type="gcs",
-            settings=json.dumps({
-                "bucket": "my_bucket",
-                "client": "my_alternate_client",
-                "compress": False,
-            }),
-        ))
+        this = ec.SnapshotRepository("this",
+            name="my-snapshot-repository",
+            generic=ec.SnapshotRepositoryGenericArgs(
+                type="gcs",
+                settings=json.dumps({
+                    "bucket": "my_bucket",
+                    "client": "my_alternate_client",
+                    "compress": False,
+                }),
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         You can import snapshot repositories using the `name`, for example:
```

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec.egg-info/PKG-INFO` & `pulumi_ec-0.8.1a1713560980/pulumi_ec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ec
-Version: 0.8.1a1713332203
+Version: 0.8.1a1713560980
 Summary: A Pulumi package for creating and managing ElasticCloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ec
 Keywords: pulumi,ec,elasticsearch,es,elastic,elasticcloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ec-0.8.1a1713332203/pulumi_ec.egg-info/SOURCES.txt` & `pulumi_ec-0.8.1a1713560980/pulumi_ec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

