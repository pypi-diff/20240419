# Comparing `tmp/iam_actions-1.2.20240417.tar.gz` & `tmp/iam_actions-1.2.20240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240417.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240418.tar", max compression
```

## Comparing `iam_actions-1.2.20240417.tar` & `iam_actions-1.2.20240418.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/README.md
--rw-r--r--   0        0        0      228 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/__init__.py
--rw-r--r--   0        0        0  4801338 2024-04-17 02:19:16.413418 iam_actions-1.2.20240417/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-17 02:17:22.805236 iam_actions-1.2.20240417/iam_actions/generate/services.py
--rw-r--r--   0        0        0   623955 2024-04-17 02:19:16.413418 iam_actions-1.2.20240417/iam_actions/policies.json
--rw-r--r--   0        0        0   208021 2024-04-17 02:19:16.413418 iam_actions-1.2.20240417/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   605333 2024-04-17 02:19:16.413418 iam_actions-1.2.20240417/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-17 02:19:17.053403 iam_actions-1.2.20240417/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240417/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240417/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-18 02:17:01.606270 iam_actions-1.2.20240418/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-18 02:17:01.606270 iam_actions-1.2.20240418/README.md
+-rw-r--r--   0        0        0      228 2024-04-18 02:17:01.610271 iam_actions-1.2.20240418/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4802214 2024-04-18 02:18:38.558787 iam_actions-1.2.20240418/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-18 02:17:01.610271 iam_actions-1.2.20240418/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-18 02:17:01.610271 iam_actions-1.2.20240418/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-18 02:17:01.610271 iam_actions-1.2.20240418/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-18 02:17:01.610271 iam_actions-1.2.20240418/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-18 02:17:01.610271 iam_actions-1.2.20240418/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-18 02:17:01.610271 iam_actions-1.2.20240418/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-18 02:17:01.610271 iam_actions-1.2.20240418/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-18 02:17:01.610271 iam_actions-1.2.20240418/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   624005 2024-04-18 02:18:38.558787 iam_actions-1.2.20240418/iam_actions/policies.json
+-rw-r--r--   0        0        0   208291 2024-04-18 02:18:38.558787 iam_actions-1.2.20240418/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   605381 2024-04-18 02:18:38.558787 iam_actions-1.2.20240418/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-18 02:18:39.242790 iam_actions-1.2.20240418/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240418/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240418/PKG-INFO
```

### Comparing `iam_actions-1.2.20240417/LICENSE` & `iam_actions-1.2.20240418/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240417/README.md` & `iam_actions-1.2.20240418/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240417/iam_actions/actions.json` & `iam_actions-1.2.20240418/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998079274613801%*

 * *Differences: {"'emr-containers'": "{'DescribeSecurityConfiguration': {'access_level': 'Read', 'description': "*

 * *                     "'Grants permission to describe a security configuration', 'resources': "*

 * *                     "['securityConfiguration']}, 'CreateSecurityConfiguration': {'access_level': "*

 * *                     "'Write', 'condition_keys': ['aws:RequestTag/${TagKey}', 'aws:TagKeys'], "*

 * *                     "'description': 'Grants permission to create a security configuration'}, "*

 * *                     "'List […]*

```diff
@@ -66386,18 +66386,21 @@
             "description": "Grants permission to create a managed endpoint",
             "orphan": false,
             "resources": [
                 "virtualCluster"
             ]
         },
         "CreateSecurityConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateSecurityConfiguration",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a security configuration",
             "orphan": false,
             "resources": []
         },
         "CreateVirtualCluster": {
             "access_level": "Write",
             "action": "CreateVirtualCluster",
             "condition_keys": [
@@ -66465,20 +66468,22 @@
             "description": "Grants permission to describe a managed endpoint",
             "orphan": false,
             "resources": [
                 "managedEndpoint"
             ]
         },
         "DescribeSecurityConfiguration": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeSecurityConfiguration",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a security configuration",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "securityConfiguration"
+            ]
         },
         "DescribeVirtualCluster": {
             "access_level": "Read",
             "action": "DescribeVirtualCluster",
             "condition_keys": [],
             "description": "Grants permission to describe a virtual cluster",
             "orphan": false,
@@ -66521,18 +66526,18 @@
             "description": "Grants permission to list managed endpoints associated with a virtual cluster",
             "orphan": false,
             "resources": [
                 "virtualCluster"
             ]
         },
         "ListSecurityConfigurations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListSecurityConfigurations",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list security configurations",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "List",
             "action": "ListTagsForResource",
             "condition_keys": [],
@@ -84316,14 +84321,24 @@
             "condition_keys": [],
             "description": "Grants permission to get information about a health event for a specified monitor",
             "orphan": false,
             "resources": [
                 "HealthEvent"
             ]
         },
+        "GetInternetEvent": {
+            "access_level": "Read",
+            "action": "GetInternetEvent",
+            "condition_keys": [],
+            "description": "Grants permission to get information about a specified internet event",
+            "orphan": false,
+            "resources": [
+                "InternetEvent"
+            ]
+        },
         "GetMonitor": {
             "access_level": "Read",
             "action": "GetMonitor",
             "condition_keys": [],
             "description": "Grants permission to get information about a monitor",
             "orphan": false,
             "resources": [
@@ -84364,14 +84379,22 @@
             "condition_keys": [],
             "description": "Grants permission to list all health events for a monitor",
             "orphan": false,
             "resources": [
                 "Monitor"
             ]
         },
+        "ListInternetEvents": {
+            "access_level": "List",
+            "action": "ListInternetEvents",
+            "condition_keys": [],
+            "description": "Grants permission to list all internet events",
+            "orphan": false,
+            "resources": []
+        },
         "ListMonitors": {
             "access_level": "List",
             "action": "ListMonitors",
             "condition_keys": [],
             "description": "Grants permission to list all monitors in an account and their statuses",
             "orphan": false,
             "resources": []
@@ -118479,20 +118502,22 @@
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
         "CancelCapacityTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CancelCapacityTask",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to cancel a Capacity Task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "outpost"
+            ]
         },
         "CancelOrder": {
             "access_level": "Write",
             "action": "CancelOrder",
             "condition_keys": [],
             "description": "Grants permission to cancel an order",
             "orphan": false,
@@ -118557,20 +118582,22 @@
             "description": "Grants permission to delete a site",
             "orphan": false,
             "resources": [
                 "site"
             ]
         },
         "GetCapacityTask": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetCapacityTask",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get information about the specified Capacity Task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "outpost"
+            ]
         },
         "GetCatalogItem": {
             "access_level": "Read",
             "action": "GetCatalogItem",
             "condition_keys": [],
             "description": "Grants permission to get a catalog item",
             "orphan": false,
@@ -118609,20 +118636,22 @@
             "description": "Grants permission to get the instance types for the specified Outpost",
             "orphan": false,
             "resources": [
                 "outpost"
             ]
         },
         "GetOutpostSupportedInstanceTypes": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetOutpostSupportedInstanceTypes",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to get the supported instance types for the specified Outpost",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "outpost"
+            ]
         },
         "GetPrivateConnectivityConfig": {
             "access_level": "Read",
             "action": "GetPrivateConnectivityConfig",
             "condition_keys": [],
             "description": "Grants permission to get a private connectivity configuration",
             "orphan": false,
@@ -118653,18 +118682,18 @@
             "action": "ListAssets",
             "condition_keys": [],
             "description": "Grants permission to list the assets for your Outpost",
             "orphan": false,
             "resources": []
         },
         "ListCapacityTasks": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListCapacityTasks",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list the Capacity Tasks for your AWS account",
             "orphan": false,
             "resources": []
         },
         "ListCatalogItems": {
             "access_level": "List",
             "action": "ListCatalogItems",
             "condition_keys": [],
@@ -118701,20 +118730,22 @@
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags for a resource",
             "orphan": false,
             "resources": []
         },
         "StartCapacityTask": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartCapacityTask",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a Capacity Task",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "outpost"
+            ]
         },
         "StartConnection": {
             "access_level": "Write",
             "action": "StartConnection",
             "condition_keys": [],
             "description": "Grants permission to start a connection for your Outpost server",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20240417/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240418/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240417/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240418/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240417/iam_actions/generate/generate.py` & `iam_actions-1.2.20240418/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240417/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240418/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240417/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240418/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240417/iam_actions/generate/services.py` & `iam_actions-1.2.20240418/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240417/iam_actions/policies.json` & `iam_actions-1.2.20240418/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999987985390234%*

 * *Differences: {"'serviceMap'": "{'Amazon CloudWatch Internet Monitor': {'Actions': {insert: [(3, "*

 * *                 "'GetInternetEvent'), (9, 'ListInternetEvents')]}}}"}*

```diff
@@ -12297,19 +12297,21 @@
         "Amazon CloudWatch Internet Monitor": {
             "ARNFormat": "arn:aws:internetmonitor:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:internetmonitor:.+:.+:.+",
             "Actions": [
                 "CreateMonitor",
                 "DeleteMonitor",
                 "GetHealthEvent",
+                "GetInternetEvent",
                 "GetMonitor",
                 "GetQueryResults",
                 "GetQueryStatus",
                 "Link",
                 "ListHealthEvents",
+                "ListInternetEvents",
                 "ListMonitors",
                 "ListTagsForResource",
                 "StartQuery",
                 "StopQuery",
                 "TagResource",
                 "UntagResource",
                 "UpdateMonitor"
```

### Comparing `iam_actions-1.2.20240417/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240418/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993162393162394%*

 * *Differences: {"'emr-containers'": "{'securityConfiguration': OrderedDict([('arn_pattern', "*

 * *                     "'arn:*:emr-containers:*:*:/securityconfigurations/*'), ('condition_keys', "*

 * *                     "'aws:ResourceTag/${TagKey}')])}",*

 * * "'internetmonitor'": "{'InternetEvent': OrderedDict([('arn_pattern', "*

 * *                      "'arn:*:internetmonitor::*:internet-event/*'), ('condition_keys', None)])}"}*

```diff
@@ -2645,14 +2645,18 @@
             "arn_pattern": "arn:*:emr-containers:*:*:/jobtemplates/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "managedEndpoint": {
             "arn_pattern": "arn:*:emr-containers:*:*:/virtualclusters/*/endpoints/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "securityConfiguration": {
+            "arn_pattern": "arn:*:emr-containers:*:*:/securityconfigurations/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "virtualCluster": {
             "arn_pattern": "arn:*:emr-containers:*:*:/virtualclusters/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "emr-serverless": {
         "application": {
@@ -3456,14 +3460,18 @@
         }
     },
     "internetmonitor": {
         "HealthEvent": {
             "arn_pattern": "arn:*:internetmonitor:*:*:monitor/*/health-event/*",
             "condition_keys": null
         },
+        "InternetEvent": {
+            "arn_pattern": "arn:*:internetmonitor::*:internet-event/*",
+            "condition_keys": null
+        },
         "Monitor": {
             "arn_pattern": "arn:*:internetmonitor:*:*:monitor/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "invoicing": {},
     "iot": {
```

### Comparing `iam_actions-1.2.20240417/iam_actions/services.json` & `iam_actions-1.2.20240418/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999874308697838%*

 * *Differences: {"'internetmonitor'": "{'Actions': {insert: [(3, 'GetInternetEvent'), (9, 'ListInternetEvents')]}}"}*

```diff
@@ -11614,19 +11614,21 @@
         "ARNRegexes": [
             "^arn:aws:internetmonitor:.+:.+:.+"
         ],
         "Actions": [
             "CreateMonitor",
             "DeleteMonitor",
             "GetHealthEvent",
+            "GetInternetEvent",
             "GetMonitor",
             "GetQueryResults",
             "GetQueryStatus",
             "Link",
             "ListHealthEvents",
+            "ListInternetEvents",
             "ListMonitors",
             "ListTagsForResource",
             "StartQuery",
             "StopQuery",
             "TagResource",
             "UntagResource",
             "UpdateMonitor"
```

### Comparing `iam_actions-1.2.20240417/pyproject.toml` & `iam_actions-1.2.20240418/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240417"
+version = "1.2.20240418"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240417/setup.py` & `iam_actions-1.2.20240418/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240417',
+    'version': '1.2.20240418',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240417/PKG-INFO` & `iam_actions-1.2.20240418/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240417
+Version: 1.2.20240418
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

