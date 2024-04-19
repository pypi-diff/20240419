# Comparing `tmp/dbt_loom-0.4.1.tar.gz` & `tmp/dbt_loom-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_loom-0.4.1.tar", max compression
+gzip compressed data, was "dbt_loom-0.5.0.tar", max compression
```

## Comparing `dbt_loom-0.4.1.tar` & `dbt_loom-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1211 2024-02-29 14:27:54.390778 dbt_loom-0.4.1/LICENSE
--rw-r--r--   0        0        0     6654 2024-02-29 14:27:54.390778 dbt_loom-0.4.1/README.md
--rw-r--r--   0        0        0     9376 2024-02-29 14:27:54.390778 dbt_loom-0.4.1/dbt_loom/__init__.py
--rw-r--r--   0        0        0     1883 2024-02-29 14:27:54.390778 dbt_loom-0.4.1/dbt_loom/clients/az_blob.py
--rw-r--r--   0        0        0     2442 2024-02-29 14:27:54.390778 dbt_loom-0.4.1/dbt_loom/clients/dbt_cloud.py
--rw-r--r--   0        0        0     1367 2024-02-29 14:27:54.390778 dbt_loom-0.4.1/dbt_loom/clients/gcs.py
--rw-r--r--   0        0        0     1401 2024-02-29 14:27:54.390778 dbt_loom-0.4.1/dbt_loom/clients/s3.py
--rw-r--r--   0        0        0     1036 2024-02-29 14:27:54.390778 dbt_loom-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7447 1970-01-01 00:00:00.000000 dbt_loom-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-19 16:35:41.742745 dbt_loom-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6654 2024-04-19 16:35:41.742745 dbt_loom-0.5.0/README.md
+-rw-r--r--   0        0        0     5328 2024-04-19 16:35:41.742745 dbt_loom-0.5.0/dbt_loom/__init__.py
+-rw-r--r--   0        0        0     2088 2024-04-19 16:35:41.742745 dbt_loom-0.5.0/dbt_loom/clients/az_blob.py
+-rw-r--r--   0        0        0     2675 2024-04-19 16:35:41.742745 dbt_loom-0.5.0/dbt_loom/clients/dbt_cloud.py
+-rw-r--r--   0        0        0     1603 2024-04-19 16:35:41.742745 dbt_loom-0.5.0/dbt_loom/clients/gcs.py
+-rw-r--r--   0        0        0     1641 2024-04-19 16:35:41.742745 dbt_loom-0.5.0/dbt_loom/clients/s3.py
+-rw-r--r--   0        0        0     1161 2024-04-19 16:35:41.742745 dbt_loom-0.5.0/dbt_loom/config.py
+-rw-r--r--   0        0        0     4578 2024-04-19 16:35:41.742745 dbt_loom-0.5.0/dbt_loom/manifests.py
+-rw-r--r--   0        0        0     1059 2024-04-19 16:35:41.742745 dbt_loom-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7505 1970-01-01 00:00:00.000000 dbt_loom-0.5.0/PKG-INFO
```

### Comparing `dbt_loom-0.4.1/LICENSE` & `dbt_loom-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.4.1/README.md` & `dbt_loom-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.4.1/dbt_loom/clients/az_blob.py` & `dbt_loom-0.5.0/dbt_loom/clients/az_blob.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 import json
 import os
 from typing import Dict
 
 from azure.identity import DefaultAzureCredential
 from azure.storage.blob import BlobServiceClient
+from pydantic import BaseModel
+
+
+class AzureReferenceConfig(BaseModel):
+    """Configuration for an reference stored in Azure Storage"""
+
+    container_name: str
+    object_name: str
+    account_name: str
 
 
 class AzureClient:
     """A client for loading manifest files from Azure storage."""
 
     def __init__(
         self, container_name: str, object_name: str, account_name: str
```

### Comparing `dbt_loom-0.4.1/dbt_loom/clients/dbt_cloud.py` & `dbt_loom-0.5.0/dbt_loom/clients/dbt_cloud.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import os
 from typing import Any, Dict, Optional
 
+from pydantic import BaseModel
 import requests
 from dbt.events.functions import fire_event
 from dbt.events.types import Note
 
 
+class DbtCloudReferenceConfig(BaseModel):
+    """Configuration for a dbt Cloud reference."""
+
+    account_id: int
+    job_id: int
+    api_endpoint: Optional[str] = None
+    step: Optional[int] = None
+
+
 class DbtCloud:
     """API Client for dbt Cloud. Fetches latest manifest for a given dbt job."""
 
     def __init__(
         self,
         account_id: int,
         token: Optional[str] = None,
```

### Comparing `dbt_loom-0.4.1/dbt_loom/clients/gcs.py` & `dbt_loom-0.5.0/dbt_loom/clients/gcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import json
 from pathlib import Path
 from typing import Dict, Optional
 
 from google.cloud import storage
+from pydantic import BaseModel
+
+
+class GCSReferenceConfig(BaseModel):
+    """Configuration for a GCS reference"""
+
+    project_id: str
+    bucket_name: str
+    object_name: str
+    credentials: Optional[Path] = None
 
 
 class GCSClient:
     """Client for GCS. Fetches manifest for a given bucket."""
 
     def __init__(
         self,
@@ -29,15 +39,16 @@
             if self.credentials
             else storage.Client(project=self.project_id)
         )
         bucket = client.get_bucket(self.bucket_name)
         blob = bucket.get_blob(self.object_name)
         if not blob:
             raise Exception(
-                f"The object `{self.object_name}` does not exist in bucket `{self.bucket_name}`."
+                f"The object `{self.object_name}` does not exist in bucket "
+                f"`{self.bucket_name}`."
             )
 
         manifest_json = blob.download_as_text()
 
         try:
             return json.loads(manifest_json)
         except Exception:
```

### Comparing `dbt_loom-0.4.1/dbt_loom/clients/s3.py` & `dbt_loom-0.5.0/dbt_loom/clients/s3.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 import json
-from typing import Dict
+from pathlib import Path
+from typing import Dict, Optional
 
 import boto3
+from pydantic import BaseModel
+
+
+class S3ReferenceConfig(BaseModel):
+    """Configuration for an reference stored in S3"""
+
+    bucket_name: str
+    object_name: str
+    credentials: Optional[Path] = None
 
 
 class S3Client:
     """A client for loading manifest files from S3-compatible object stores."""
 
     def __init__(self, bucket_name: str, object_name: str) -> None:
         self.bucket_name = bucket_name
```

### Comparing `dbt_loom-0.4.1/pyproject.toml` & `dbt_loom-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "dbt-loom"
-version = "0.4.1"
+version = "0.5.0"
 description = "A dbt-core plugin to import public nodes in multi-project deployments."
 authors = ["Nicholas Yager <yager@nicholasyager.com>"]
 readme = "README.md"
 packages = [{ include = "dbt_loom" }]
 
 [tool.commitizen]
-version = "0.4.1"
+version = "0.5.0"
 version_files = ["pyproject.toml:^version"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 dbt-core = ">=1.6.0,<1.8.0"
 requests = "^2.31.0"
 google-cloud-storage = "^2.13.0"
 boto3 = "^1.28.84"
 azure-storage-blob = "^12.19.0"
 azure-identity = "^1.15.0"
 types-pyyaml = "^6.0.12.12"
+types-networkx = "^3.2.1.20240313"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.278"
+ruff = "^0.3.0"
 pytest = "^7.4.0"
 isort = "^5.12.0"
-black = "^23.7.0"
-dbt-duckdb = "^1.6.0"
+dbt-duckdb = ">=1.6.0,<1.8.0"
 duckdb = ">=0.8.0"
 pre-commit = "^3.6.0"
 mypy = "^1.8.0"
 
 [tool.ruff]
 line-length = 88
```

### Comparing `dbt_loom-0.4.1/PKG-INFO` & `dbt_loom-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-loom
-Version: 0.4.1
+Version: 0.5.0
 Summary: A dbt-core plugin to import public nodes in multi-project deployments.
 Author: Nicholas Yager
 Author-email: yager@nicholasyager.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.19.0,<13.0.0)
 Requires-Dist: boto3 (>=1.28.84,<2.0.0)
 Requires-Dist: dbt-core (>=1.6.0,<1.8.0)
 Requires-Dist: google-cloud-storage (>=2.13.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: types-networkx (>=3.2.1.20240313,<4.0.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.12,<7.0.0.0)
 Description-Content-Type: text/markdown
 
 # dbt-loom
 
 [![pypi version shield](https://img.shields.io/pypi/v/dbt-loom)](https://img.shields.io/pypi/v/dbt-loom)
```

