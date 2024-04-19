# Comparing `tmp/igrafx_mining_sdk-2.30.0.tar.gz` & `tmp/igrafx_mining_sdk-2.31.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igrafx_mining_sdk-2.30.0.tar", last modified: Fri Mar 15 08:57:34 2024, max compression
+gzip compressed data, was "igrafx_mining_sdk-2.31.2.tar", last modified: Fri Apr 19 08:08:13 2024, max compression
```

## Comparing `igrafx_mining_sdk-2.30.0.tar` & `igrafx_mining_sdk-2.31.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:57:34.393666 igrafx_mining_sdk-2.30.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-03-15 08:57:34.393666 igrafx_mining_sdk-2.30.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:57:34.389666 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/column_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    21713 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/workgroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:57:34.389666 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-03-15 08:57:34.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-15 08:57:34.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 08:57:34.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-15 08:57:34.000000 igrafx_mining_sdk-2.30.0/igrafx_mining_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 08:57:34.393666 igrafx_mining_sdk-2.30.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-15 08:57:19.000000 igrafx_mining_sdk-2.30.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:57:34.389666 igrafx_mining_sdk-2.30.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:57:34.389666 igrafx_mining_sdk-2.30.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:57:34.393666 igrafx_mining_sdk-2.30.0/tests/data/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/data/graphs/graph.json
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/data/graphs/graph_with_invalid_edges.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 08:57:34.393666 igrafx_mining_sdk-2.30.0/tests/data/tables/
--rw-r--r--   0 runner    (1001) docker     (127)    27136 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/data/tables/p2pShortExcel.xls
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/data/tables/p2pShortExcel.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/data/tables/testdata.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/test_00_workgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/test_01_column_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/test_02_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/test_03_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/test_04_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-15 08:57:17.000000 igrafx_mining_sdk-2.30.0/tests/test_05_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17408 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23262 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/workgroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-19 08:08:13.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 08:08:13.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:08:13.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 08:08:13.000000 igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:08:13.505211 igrafx_mining_sdk-2.31.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 08:07:59.000000 igrafx_mining_sdk-2.31.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.497211 igrafx_mining_sdk-2.31.2/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/tests/data/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/data/graphs/graph.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/data/graphs/graph_with_invalid_edges.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:08:13.501211 igrafx_mining_sdk-2.31.2/tests/data/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)    27136 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/data/tables/p2pShortExcel.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/data/tables/p2pShortExcel.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/data/tables/testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_00_workgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_01_column_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35094 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_02_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_03_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_04_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 08:07:50.000000 igrafx_mining_sdk-2.31.2/tests/test_05_delete.py
```

### Comparing `igrafx_mining_sdk-2.30.0/LICENSE` & `igrafx_mining_sdk-2.31.2/LICENSE`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/README.md` & `igrafx_mining_sdk-2.31.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 The iGrafx P360 Live Mining SDK uses Python.
 
 A detailed tutorial can be found in the [howto.md](https://github.com/igrafx/mining-python-sdk/blob/dev/howto.md) file.
 
 
 ## Requirements
 
-This package requires python 3.6.8 or above. Get the latest version of [Python](https://www.python.org/).
+This package requires python 3.10 or above. Get the latest version of [Python](https://www.python.org/).
 
 The required packages should be installed via the ```pyproject.toml``` when running the  ```poetry install``` command. 
 
 ## Installing
 
 ### With pip:
 To install the current release of the iGrafx P360 Live Mining SDK with **pip**, simply navigate to the console and type the following command:
```

### Comparing `igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/__init__.py` & `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/api_connector.py` & `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/api_connector.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/column_mapping.py` & `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/column_mapping.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/datasource.py` & `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/datasource.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/graph.py` & `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/graph.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/project.py` & `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License, Copyright 2023 iGrafx
 # https://github.com/igrafx/mining-python-sdk/blob/dev/LICENSE
-
+import json
 import os
 import random
 from igrafx_mining_sdk.graph import Graph, GraphInstance
 from igrafx_mining_sdk.column_mapping import FileStructure, ColumnMapping
 from igrafx_mining_sdk.datasource import Datasource
 from igrafx_mining_sdk.api_connector import APIConnector
 from igrafx_mining_sdk.dtos.PredictionStatusDto import PredictionStatusDto
@@ -13,14 +13,15 @@
 from igrafx_mining_sdk.dtos.PredictionPossibilityDto import PredictionPossibilityDto
 from igrafx_mining_sdk.dtos.PredictionErrorStatusDto import PredictionErrorStatusDto
 from igrafx_mining_sdk.dtos.WorkflowStatusDto import WorkflowStatusDto
 import uuid
 from enum import Enum
 from datetime import datetime
 from typing import List, Optional, Dict, Union
+from collections import OrderedDict
 
 
 class Project:
     """A iGrafx P360 Live Mining project"""
     def __init__(self, pid: str, api_connector: APIConnector):
         """Create a iGrafx P360 Live Mining project from a project ID and the Workgroup it was created from
 
@@ -203,14 +204,48 @@
 
     def get_mapping_infos(self):
         """Returns the mapping infos of the project such as the column names"""
 
         response_mapping_infos = self.api_connector.get_request(f"/project/{self.id}/mappingInfos").json()
         return response_mapping_infos
 
+    def get_column_mapping(self):
+
+        if self.column_mapping_exists:
+            response_column_mapping = self.api_connector.get_request(f"/project/{self.id}/column-mapping").json()
+
+            column_mapping = {}
+            for k, v in response_column_mapping.items():
+                if isinstance(v, dict):
+                    v['name'] = k
+                    if k == 'caseId':
+                        v['columnType'] = "CASE_ID"
+                    elif k == 'activity':
+                        v['columnType'] = "TASK_NAME"
+                    elif k in ["dateColumn", "otherDateColumn"]:
+                        v['columnType'] = "TIME"
+                    else:
+                        raise ValueError("Default columns should be of type 'caseId', 'activity', 'dateColumn' or 'otherDateColumn'")
+                    column_mapping['col' + str(v['columnIndex'])] = v
+                elif isinstance(v, list):
+                    for i, subdict in enumerate(v):
+                        if k == 'dimensions':
+                            subdict['columnType'] = "DIMENSION"
+                        elif k == 'metrics':
+                            subdict['columnType'] = "METRIC"
+                        else:
+                            raise ValueError("Nested lists should be of type 'dimensions' or 'metrics'")
+                        column_mapping['col' + str(subdict['columnIndex'])] = subdict
+
+            # Sort the column mapping by columnIndex value and cast to json
+            column_mapping = OrderedDict(sorted(column_mapping.items(), key=lambda x: x[1]["columnIndex"]))
+            return json.dumps(column_mapping)
+        else:
+            raise ValueError("Column mapping does not exist for this project.")
+
     def reset(self):
         """Makes an API call to manually reset a project"""
 
         response_reset = self.api_connector.post_request(f"/project/{self.id}/reset")
         return response_reset.status_code == 204
 
     def add_file(self, path):
@@ -369,23 +404,22 @@
         elif response.status_code == 424:
             print(f"Tried to delete predictions but service failed on project {self.id}. Response: {response}")
             return PredictionErrorStatusDto.PREDICTION_SERVICE_FAILURE
         else:
             print(f"Failed to delete predictions on project {self.id}. Response: {response}")
             return PredictionErrorStatusDto.UNKNOWN_ERROR
 
-    def _parse_workflow_status(self, item: Dict[str, str]) -> Union[WorkflowStatusDto, PredictionErrorStatusDto]:
+    def _parse_workflow_status(self, item: Dict[str, str]) ->  Union[WorkflowStatusDto, PredictionErrorStatusDto]:
         """Parses the prediction status object to a business class WorkflowStatusDto"""
 
         prediction_id = self._cast_string_to_uuid_or_none(item.get('workflowId'))
         project_id = self._cast_string_to_uuid_or_none(item.get('projectId'))
         status = self._get_enum_value_or_none(item.get('status'), PredictionStatusDto)
         start_time = item.get('startTime')
-        completed_tasks = [self._get_enum_value_or_none(task, PredictionTaskTypeDto)
-                           for task in item.get('completedTasks', [])]
+        completed_tasks = [self._get_enum_value_or_none(task, PredictionTaskTypeDto) for task in item.get('completedTasks', [])]
         end_time = item.get('endTime', None)
 
         if None in (prediction_id, project_id, status, completed_tasks):
             return PredictionErrorStatusDto.INVALID_RESPONSE
         else:
             try:
                 date_format = "%Y-%m-%dT%H:%M:%S.%fZ"
@@ -395,33 +429,28 @@
                     start_datetime = None
 
                 if end_time is not None:
                     end_datetime = datetime.strptime(end_time, date_format)
                 else:
                     end_datetime = None
 
-                return WorkflowStatusDto(prediction_id,
-                                         project_id,
-                                         status,
-                                         start_datetime,
-                                         end_datetime,
-                                         completed_tasks)
+                return WorkflowStatusDto(prediction_id, project_id, status, start_datetime, end_datetime, completed_tasks)
             except ValueError:
                 return PredictionErrorStatusDto.INVALID_RESPONSE
 
     def _get_enum_value_or_none(self, value_str: str, enum_type: Enum) -> Optional[Enum]:
-        """Parses the value_str string to the given enum_type or None if it does not match"""
+        """Parses the value_str string to the given enum_type or None if does not match"""
 
         try:
             return enum_type(value_str)
         except ValueError:
             return None
 
     def _cast_string_to_uuid_or_none(self, string_value: str) -> Optional[uuid.UUID]:
-        """Parses the string_value string to a UUID class or None if it does not match to a UUID"""
+        """Parses the string_value string to a UUID class or None if does not match to a UUID"""
 
         try:
             if string_value is None:
                 return None
             else:
                 return uuid.UUID(string_value)
         except ValueError:
```

### Comparing `igrafx_mining_sdk-2.30.0/igrafx_mining_sdk/workgroup.py` & `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk/workgroup.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/igrafx_mining_sdk.egg-info/SOURCES.txt` & `igrafx_mining_sdk-2.31.2/igrafx_mining_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/pyproject.toml` & `igrafx_mining_sdk-2.31.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [tool.poetry]
 name = "igrafx_mining_sdk"
-version = "2.29.0"
+version = "2.31.1"
 description = "The iGrafx P360 Live Mining SDK is an open source application that can be used to manage your mining projects."
 authors = ["iGrafx <contact@igrafx.com>"]
 license = "MIT"
 readme = "README.md"
-#packages = [{ include = "igrafx_mining_sdk" , from = "igrafx_mining_sdk" }]
 homepage = "https://www.grafx.com/"
 repository = "https://github.com/igrafx/mining-python-sdk"
 keywords = ["process mining"]
 
 [tool.poetry.dependencies]
-python = "^3.7.1,<3.11"
-requests = "2.29.0"
-pydruid = "0.6.5"
-pandas = "^1.3.5"
-SQLAlchemy = "2.0.12"
-networkx = "2.6.3"
-numpy = "^1.21.6"
+python = "^3.10.0,<3.12.1"
+requests = "2.31.0"
+pydruid = "0.6.6"
+pandas = "^2.0.0,<=2.2.1"
+SQLAlchemy = "2.0.29"
+networkx = "^3.0.0,<3.3.0"
+numpy = "^1.25.0"
 toml = "0.10.2"
-python-dotenv = "0.19.2"
+python-dotenv = "1.0.1"
+urllib3 = "2.2.1"
+pip = "24.0.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.3.1"
-pytest-dependency = "0.5.1"
+pytest = "8.1.1"
+pytest-dependency = "0.6.0"
+pytest-mock = "3.14.0"
 
 
 [tool.pytest.ini_options]
 pythonpath = "igrafx_mining_sdk"
 testpaths = ["tests"]
 
 [build-system]
```

### Comparing `igrafx_mining_sdk-2.30.0/setup.py` & `igrafx_mining_sdk-2.31.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 }
 
 # Extract requirements
 requirements = list(pyproject_data['tool']['poetry']['dependencies'].values())
 
 setup(
     name="igrafx_mining_sdk",
-    version='2.30.0',
+    version='2.31.2',
     description=package_infos['__doc__'],
     long_description=open("README.md", 'r').read(),
     long_description_content_type='text/markdown',
     url="https://www.igrafx.com",
     author=package_infos['__author__'],
     author_email=package_infos['__email__'],
     packages=find_packages(),
-    licence="Apache License 2.0"
+    licence="MIT"
 )
```

### Comparing `igrafx_mining_sdk-2.30.0/tests/data/graphs/graph.json` & `igrafx_mining_sdk-2.31.2/tests/data/graphs/graph.json`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/tests/data/graphs/graph_with_invalid_edges.json` & `igrafx_mining_sdk-2.31.2/tests/data/graphs/graph_with_invalid_edges.json`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/tests/data/tables/p2pShortExcel.xls` & `igrafx_mining_sdk-2.31.2/tests/data/tables/p2pShortExcel.xls`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/tests/data/tables/p2pShortExcel.xlsx` & `igrafx_mining_sdk-2.31.2/tests/data/tables/p2pShortExcel.xlsx`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/tests/test_00_workgroup.py` & `igrafx_mining_sdk-2.31.2/tests/test_00_workgroup.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/tests/test_01_column_mapping.py` & `igrafx_mining_sdk-2.31.2/tests/test_01_column_mapping.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/tests/test_02_project.py` & `igrafx_mining_sdk-2.31.2/tests/test_02_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,14 +126,20 @@
         ]
         column_mapping = ColumnMapping(column_list)
         base_dir = Path(__file__).resolve().parent
         file_path = base_dir / 'data' / 'tables' / 'testdata.csv'
         assert pytest.project.add_column_mapping(filestructure, column_mapping)
         assert pytest.project.add_file(str(file_path))
 
+    def test_get_column_mapping_not_exist(self):
+        """Test that if there is no column mapping, a ValueError is raised"""
+        pytest.project.reset()
+        with pytest.raises(ValueError):
+            pytest.project.get_column_mapping()
+
     @pytest.mark.dependency(name='add_csv_file', depends=['reset', 'add_column_mapping'], scope='session')
     def test_add_csv_file_from_json_column_mapping(self):
         """Test that a csv file can be added to a project. Using a json column mapping that contains grouped tasks"""
         pytest.project.reset()
         filestructure = FileStructure(
             file_type=FileType.csv,
         )
@@ -149,25 +155,46 @@
         }'''
         column_mapping = ColumnMapping.from_json(column_dict)
         base_dir = Path(__file__).resolve().parent
         file_path = base_dir / 'data' / 'tables' / 'testdata.csv'
         assert pytest.project.add_column_mapping(filestructure, column_mapping)
         assert pytest.project.add_file(str(file_path))
 
+    @pytest.mark.dependency(name='add_csv_file', depends=['reset', 'add_column_mapping'], scope='session')
+    def test_get_column_mapping_add_csv_groupedtasks(self):
+        """Test that the the column mapping that was recuperated can be used to add a csv file containing grouped_tasks"""
+        column_mapping_dict = pytest.project.get_column_mapping()
+        pytest.project.reset()
+        filestructure = FileStructure(
+            file_type=FileType.csv,
+        )
+        column_mapping = ColumnMapping.from_json(column_mapping_dict)
+        base_dir = Path(__file__).resolve().parent
+        file_path = base_dir / 'data' / 'tables' / 'testdata.csv'
+        assert pytest.project.add_column_mapping(filestructure, column_mapping)
+        assert pytest.project.add_file(str(file_path))
+        assert pytest.project.get_column_mapping()
+
     @pytest.mark.dependency(name='project_contains_data', depends=['add_csv_file'])
     def test_project_contains_data(self):
+        """Test that the project contains data"""
         count = 0
         while pytest.project.nodes_datasource.__class__ != Datasource:
             time.sleep(3)
             count += 1
             if count > 100:
                 assert False, 'Timeout reached'
         assert True
 
     @pytest.mark.dependency(depends=['project_contains_data'])
+    def test_get_column_mapping(self):
+        """Test that the correct column mapping can be returned"""
+        assert pytest.project.get_column_mapping()
+
+    @pytest.mark.dependency(depends=['project_contains_data'])
     def test_datasources_types(self):
         """Test the types of the datasources"""
         assert pytest.project.nodes_datasource.__class__ == Datasource
         assert pytest.project.edges_datasource.__class__ == Datasource
         assert pytest.project.cases_datasource.__class__ == Datasource
 
     @pytest.mark.dependency(depends=['project_contains_data'])
```

### Comparing `igrafx_mining_sdk-2.30.0/tests/test_03_datasource.py` & `igrafx_mining_sdk-2.31.2/tests/test_03_datasource.py`

 * *Files identical despite different names*

### Comparing `igrafx_mining_sdk-2.30.0/tests/test_04_graph.py` & `igrafx_mining_sdk-2.31.2/tests/test_04_graph.py`

 * *Files identical despite different names*

