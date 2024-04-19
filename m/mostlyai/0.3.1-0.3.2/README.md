# Comparing `tmp/mostlyai-0.3.1.tar.gz` & `tmp/mostlyai-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mostlyai-0.3.1.tar", max compression
+gzip compressed data, was "mostlyai-0.3.2.tar", max compression
```

## Comparing `mostlyai-0.3.1.tar` & `mostlyai-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-12-22 12:47:38.462094 mostlyai-0.3.1/LICENSE
--rw-r--r--   0        0        0     2303 2024-04-02 17:48:15.885881 mostlyai-0.3.1/README.md
--rw-r--r--   0        0        0       26 2024-03-13 18:10:22.492378 mostlyai-0.3.1/mostlyai/__init__.py
--rw-r--r--   0        0        0    13016 2024-04-04 19:13:15.035679 mostlyai-0.3.1/mostlyai/api.py
--rw-r--r--   0        0        0     9150 2024-04-04 19:13:15.037096 mostlyai-0.3.1/mostlyai/base.py
--rw-r--r--   0        0        0     2667 2024-03-13 19:00:02.355471 mostlyai-0.3.1/mostlyai/connectors.py
--rw-r--r--   0        0        0      574 2024-03-13 19:00:02.358865 mostlyai-0.3.1/mostlyai/exceptions.py
--rw-r--r--   0        0        0     3986 2024-03-13 19:00:02.362753 mostlyai-0.3.1/mostlyai/generators.py
--rw-r--r--   0        0        0    38859 2024-03-22 06:46:58.727500 mostlyai-0.3.1/mostlyai/model.py
--rw-r--r--   0        0        0     1742 2024-03-22 06:46:58.729767 mostlyai-0.3.1/mostlyai/shares.py
--rw-r--r--   0        0        0     7008 2024-03-13 19:00:02.364822 mostlyai-0.3.1/mostlyai/synthetic_datasets.py
--rw-r--r--   0        0        0     5217 2024-03-13 18:10:22.527374 mostlyai-0.3.1/mostlyai/utils.py
--rw-r--r--   0        0        0     1264 2024-04-04 19:22:11.858836 mostlyai-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 mostlyai-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-22 12:47:38.462094 mostlyai-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2303 2024-04-02 17:48:15.885881 mostlyai-0.3.2/README.md
+-rw-r--r--   0        0        0       26 2024-03-20 14:08:04.920127 mostlyai-0.3.2/mostlyai/__init__.py
+-rw-r--r--   0        0        0    13512 2024-04-19 17:00:58.547459 mostlyai-0.3.2/mostlyai/api.py
+-rw-r--r--   0        0        0     9150 2024-04-19 16:58:34.132208 mostlyai-0.3.2/mostlyai/base.py
+-rw-r--r--   0        0        0     2667 2024-04-19 17:47:47.986738 mostlyai-0.3.2/mostlyai/connectors.py
+-rw-r--r--   0        0        0      574 2024-04-19 16:58:25.136734 mostlyai-0.3.2/mostlyai/exceptions.py
+-rw-r--r--   0        0        0     3986 2024-04-19 17:47:38.895142 mostlyai-0.3.2/mostlyai/generators.py
+-rw-r--r--   0        0        0    38859 2024-04-19 16:58:34.132998 mostlyai-0.3.2/mostlyai/model.py
+-rw-r--r--   0        0        0     1694 2024-04-19 17:52:24.624339 mostlyai-0.3.2/mostlyai/shares.py
+-rw-r--r--   0        0        0     7008 2024-04-19 17:47:29.352485 mostlyai-0.3.2/mostlyai/synthetic_datasets.py
+-rw-r--r--   0        0        0     5217 2024-04-19 16:58:25.140847 mostlyai-0.3.2/mostlyai/utils.py
+-rw-r--r--   0        0        0     1264 2024-04-19 17:54:32.905630 mostlyai-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 mostlyai-0.3.2/PKG-INFO
```

### Comparing `mostlyai-0.3.1/LICENSE` & `mostlyai-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.1/README.md` & `mostlyai-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.1/mostlyai/api.py` & `mostlyai-0.3.2/mostlyai/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from mostlyai.generators import _MostlyGeneratorsClient
 from mostlyai.model import (
     Connector,
     CurrentUser,
     Generator,
     PermissionLevel,
     ProgressStatus,
-    SyntheticDataset,
 )
 from mostlyai.shares import _MostlySharesClient
 from mostlyai.synthetic_datasets import _MostlySyntheticDatasetsClient
 from mostlyai.utils import (
     ShareableResource,
     _get_subject_table_names,
     _read_table_from_path,
@@ -90,14 +89,26 @@
             - config
                 - host: string
                 - httpPath: string
                 - catalog: string
             - secrets
                 - accessToken: keyFile
             - location: schema.table
+        - HIVE
+            - config
+                - host: string
+                - port: integer, default: 10000
+                - username: string, optional
+                - kerberos_enabled: boolean, default: false
+                - kerberos_principal: string, optional
+                - kerberos_krb5_conf: string, optional
+            - secrets
+                - password: string, optional
+                - kerberos_keytab: base64-encoded string, optional
+            - location: database.table
         - MARIADB
             - config
                 - host: string
                 - port: integer, default: 3306
                 - username: string
             - secrets
                 - password: string
@@ -248,20 +259,20 @@
         if "tables" not in config:
             g = self.generators.get(config["generatorId"])
             subject_tables = _get_subject_table_names(g.config())
             config["tables"] = [
                 {
                     "name": table,
                     "configuration": {
-                        "sampleSize": size.get(table)
-                        if isinstance(size, dict)
-                        else size,
-                        "sampleSeedData": seed.get(table)
-                        if isinstance(seed, dict)
-                        else seed,
+                        "sampleSize": (
+                            size.get(table) if isinstance(size, dict) else size
+                        ),
+                        "sampleSeedData": (
+                            seed.get(table) if isinstance(seed, dict) else seed
+                        ),
                     },
                 }
                 for table in subject_tables
             ]
 
         if name is not None:
             config |= {"name": name}
@@ -327,11 +338,10 @@
         rich.print(
             f"Revoked access of resource [bold cyan]{resource.id}[/] for [bold]{user_email}[/]"
         )
 
     def me(self) -> CurrentUser:
         """
         Retrieve current user info.
-
         :return: info about the current user.
         """
         return self.request(verb=GET, path=["users", "me"], response_type=CurrentUser)
```

### Comparing `mostlyai-0.3.1/mostlyai/base.py` & `mostlyai-0.3.2/mostlyai/base.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.1/mostlyai/connectors.py` & `mostlyai-0.3.2/mostlyai/connectors.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.1/mostlyai/exceptions.py` & `mostlyai-0.3.2/mostlyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.1/mostlyai/generators.py` & `mostlyai-0.3.2/mostlyai/generators.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.1/mostlyai/model.py` & `mostlyai-0.3.2/mostlyai/model.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.1/mostlyai/shares.py` & `mostlyai-0.3.2/mostlyai/shares.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from typing import Union
-from uuid import UUID
-
 from mostlyai.base import DELETE, GET, POST, _MostlyBaseClient
 from mostlyai.model import (
     Connector,
     Generator,
     PermissionLevel,
     Share,
     SyntheticDataset,
```

### Comparing `mostlyai-0.3.1/mostlyai/synthetic_datasets.py` & `mostlyai-0.3.2/mostlyai/synthetic_datasets.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.1/mostlyai/utils.py` & `mostlyai-0.3.2/mostlyai/utils.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.1/pyproject.toml` & `mostlyai-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mostlyai"
-version = "0.3.1"
+version = "0.3.2"
 description = "The official Python client for the MOSTLY AI platform."
 homepage = "https://app.mostly.ai/"
 authors = ["MOSTLY AI <office@mostly.ai>"]
 license = "Proprietary"
 readme = "README.md"
 packages = [
     { include = "mostlyai" }
```

### Comparing `mostlyai-0.3.1/PKG-INFO` & `mostlyai-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mostlyai
-Version: 0.3.1
+Version: 0.3.2
 Summary: The official Python client for the MOSTLY AI platform.
 Home-page: https://app.mostly.ai/
 License: Proprietary
 Author: MOSTLY AI
 Author-email: office@mostly.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

