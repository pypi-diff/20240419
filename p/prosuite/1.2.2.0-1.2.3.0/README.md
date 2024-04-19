# Comparing `tmp/prosuite-1.2.2.0.tar.gz` & `tmp/prosuite-1.2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosuite-1.2.2.0.tar", last modified: Fri Feb  2 14:20:53 2024, max compression
+gzip compressed data, was "prosuite-1.2.3.0.tar", last modified: Thu Apr 18 09:39:36 2024, max compression
```

## Comparing `prosuite-1.2.2.0.tar` & `prosuite-1.2.3.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-02-02 14:20:53.496137 prosuite-1.2.2.0/
--rw-rw-rw-   0        0        0     1103 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/LICENSE
--rw-rw-rw-   0        0        0     1792 2024-02-02 14:20:53.496137 prosuite-1.2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1026 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-02 14:20:53.438287 prosuite-1.2.2.0/prosuite/
--rw-rw-rw-   0        0        0      717 2024-01-30 16:09:58.000000 prosuite-1.2.2.0/prosuite/__init__.py
--rw-rw-rw-   0        0        0     3829 2024-01-30 16:09:58.000000 prosuite-1.2.2.0/prosuite/data_model.py
-drwxrwxrwx   0        0        0        0 2024-02-02 14:20:53.473729 prosuite-1.2.2.0/prosuite/datatypes/
--rw-rw-rw-   0        0        0        0 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/datatypes/__init__.py
--rw-rw-rw-   0        0        0      160 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/datatypes/esri_geometry_type.py
--rw-rw-rw-   0        0        0      127 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/datatypes/expected_case.py
--rw-rw-rw-   0        0        0      117 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/datatypes/expected_string_difference.py
--rw-rw-rw-   0        0        0      208 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/datatypes/non_linear_segment_type.py
--rw-rw-rw-   0        0        0       98 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/datatypes/unique_strings_constraint.py
-drwxrwxrwx   0        0        0        0 2024-02-02 14:20:53.480550 prosuite-1.2.2.0/prosuite/factories/
--rw-rw-rw-   0        0        0        0 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/factories/__init__.py
--rw-rw-rw-   0        0        0     3790 2024-01-30 17:04:33.000000 prosuite-1.2.2.0/prosuite/factories/enums.py
--rw-rw-rw-   0        0        0      845 2024-01-30 16:09:58.000000 prosuite-1.2.2.0/prosuite/factories/issue_filters.py
--rw-rw-rw-   0        0        0   444637 2024-02-01 16:28:18.000000 prosuite-1.2.2.0/prosuite/factories/quality_conditions.py
--rw-rw-rw-   0        0        0      760 2024-01-30 16:09:58.000000 prosuite-1.2.2.0/prosuite/factories/transformers.py
-drwxrwxrwx   0        0        0        0 2024-02-02 14:20:53.493762 prosuite-1.2.2.0/prosuite/generated/
--rw-rw-rw-   0        0        0      454 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/generated/__init__.py
--rw-rw-rw-   0        0        0     3578 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/generated/quality_test_pb2.py
--rw-rw-rw-   0        0        0     4799 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/generated/quality_test_pb2.pyi
--rw-rw-rw-   0        0        0     2705 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/generated/quality_test_pb2_grpc.py
--rw-rw-rw-   0        0        0     5064 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/generated/quality_verification_service_pb2.py
--rw-rw-rw-   0        0        0     6087 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/generated/quality_verification_service_pb2.pyi
--rw-rw-rw-   0        0        0     6983 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/prosuite/generated/quality_verification_service_pb2_grpc.py
--rw-rw-rw-   0        0        0    12461 2024-01-30 16:08:53.000000 prosuite-1.2.2.0/prosuite/generated/shared_qa_pb2.py
--rw-rw-rw-   0        0        0    24963 2024-01-30 16:08:53.000000 prosuite-1.2.2.0/prosuite/generated/shared_qa_pb2.pyi
--rw-rw-rw-   0        0        0     5870 2024-01-30 16:08:53.000000 prosuite-1.2.2.0/prosuite/generated/shared_types_pb2.py
--rw-rw-rw-   0        0        0     9630 2024-01-30 16:08:53.000000 prosuite-1.2.2.0/prosuite/generated/shared_types_pb2.pyi
--rw-rw-rw-   0        0        0     1041 2024-02-02 12:08:15.000000 prosuite-1.2.2.0/prosuite/issue_demo.py
--rw-rw-rw-   0        0        0    11869 2024-01-30 16:09:58.000000 prosuite-1.2.2.0/prosuite/quality.py
--rw-rw-rw-   0        0        0     5254 2024-01-30 16:09:58.000000 prosuite-1.2.2.0/prosuite/utils.py
--rw-rw-rw-   0        0        0    21181 2024-02-01 15:26:05.000000 prosuite-1.2.2.0/prosuite/verification.py
-drwxrwxrwx   0        0        0        0 2024-02-02 14:20:53.495130 prosuite-1.2.2.0/prosuite.egg-info/
--rw-rw-rw-   0        0        0     1792 2024-02-02 14:20:53.000000 prosuite-1.2.2.0/prosuite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2024-02-02 14:20:53.000000 prosuite-1.2.2.0/prosuite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-02 14:20:53.000000 prosuite-1.2.2.0/prosuite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-02-02 14:20:53.000000 prosuite-1.2.2.0/prosuite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-02 14:20:53.000000 prosuite-1.2.2.0/prosuite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      925 2024-02-02 14:20:53.501808 prosuite-1.2.2.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2024-01-03 11:03:20.000000 prosuite-1.2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:39:36.712522 prosuite-1.2.3.0/
+-rw-rw-rw-   0        0        0     1103 2023-01-20 23:17:38.000000 prosuite-1.2.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1792 2024-04-18 09:39:36.712522 prosuite-1.2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2023-02-24 14:29:45.000000 prosuite-1.2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 09:39:36.675778 prosuite-1.2.3.0/prosuite/
+-rw-rw-rw-   0        0        0      717 2024-02-01 12:50:23.000000 prosuite-1.2.3.0/prosuite/__init__.py
+-rw-rw-rw-   0        0        0     3829 2024-02-01 12:50:23.000000 prosuite-1.2.3.0/prosuite/data_model.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:39:36.688012 prosuite-1.2.3.0/prosuite/datatypes/
+-rw-rw-rw-   0        0        0        0 2023-01-20 23:17:38.000000 prosuite-1.2.3.0/prosuite/datatypes/__init__.py
+-rw-rw-rw-   0        0        0      160 2023-01-20 23:17:38.000000 prosuite-1.2.3.0/prosuite/datatypes/esri_geometry_type.py
+-rw-rw-rw-   0        0        0      127 2023-01-20 23:17:38.000000 prosuite-1.2.3.0/prosuite/datatypes/expected_case.py
+-rw-rw-rw-   0        0        0      117 2023-01-20 23:17:38.000000 prosuite-1.2.3.0/prosuite/datatypes/expected_string_difference.py
+-rw-rw-rw-   0        0        0      208 2023-01-20 23:17:38.000000 prosuite-1.2.3.0/prosuite/datatypes/non_linear_segment_type.py
+-rw-rw-rw-   0        0        0       98 2023-01-20 23:17:38.000000 prosuite-1.2.3.0/prosuite/datatypes/unique_strings_constraint.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:39:36.693763 prosuite-1.2.3.0/prosuite/factories/
+-rw-rw-rw-   0        0        0        0 2023-01-20 23:17:38.000000 prosuite-1.2.3.0/prosuite/factories/__init__.py
+-rw-rw-rw-   0        0        0     3790 2024-04-18 09:39:15.000000 prosuite-1.2.3.0/prosuite/factories/enums.py
+-rw-rw-rw-   0        0        0      845 2024-02-01 12:50:23.000000 prosuite-1.2.3.0/prosuite/factories/issue_filters.py
+-rw-rw-rw-   0        0        0   444624 2024-04-18 09:39:15.000000 prosuite-1.2.3.0/prosuite/factories/quality_conditions.py
+-rw-rw-rw-   0        0        0      760 2024-02-01 12:50:23.000000 prosuite-1.2.3.0/prosuite/factories/transformers.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:39:36.710154 prosuite-1.2.3.0/prosuite/generated/
+-rw-rw-rw-   0        0        0      454 2023-01-20 23:17:38.000000 prosuite-1.2.3.0/prosuite/generated/__init__.py
+-rw-rw-rw-   0        0        0     3540 2024-01-29 17:01:16.000000 prosuite-1.2.3.0/prosuite/generated/quality_test_pb2.py
+-rw-rw-rw-   0        0        0     4722 2024-01-29 17:01:16.000000 prosuite-1.2.3.0/prosuite/generated/quality_test_pb2.pyi
+-rw-rw-rw-   0        0        0     2628 2024-01-29 17:01:16.000000 prosuite-1.2.3.0/prosuite/generated/quality_test_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5025 2024-01-29 17:01:15.000000 prosuite-1.2.3.0/prosuite/generated/quality_verification_service_pb2.py
+-rw-rw-rw-   0        0        0     6001 2024-01-29 17:01:15.000000 prosuite-1.2.3.0/prosuite/generated/quality_verification_service_pb2.pyi
+-rw-rw-rw-   0        0        0     6837 2024-01-29 17:01:15.000000 prosuite-1.2.3.0/prosuite/generated/quality_verification_service_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12461 2024-01-30 10:33:35.000000 prosuite-1.2.3.0/prosuite/generated/shared_qa_pb2.py
+-rw-rw-rw-   0        0        0    24963 2024-01-30 10:33:35.000000 prosuite-1.2.3.0/prosuite/generated/shared_qa_pb2.pyi
+-rw-rw-rw-   0        0        0     5870 2024-01-30 10:33:35.000000 prosuite-1.2.3.0/prosuite/generated/shared_types_pb2.py
+-rw-rw-rw-   0        0        0     9630 2024-01-30 10:33:35.000000 prosuite-1.2.3.0/prosuite/generated/shared_types_pb2.pyi
+-rw-rw-rw-   0        0        0    11869 2024-02-01 12:50:23.000000 prosuite-1.2.3.0/prosuite/quality.py
+-rw-rw-rw-   0        0        0     5254 2024-02-01 12:50:23.000000 prosuite-1.2.3.0/prosuite/utils.py
+-rw-rw-rw-   0        0        0    21701 2024-03-15 21:43:06.000000 prosuite-1.2.3.0/prosuite/verification.py
+drwxrwxrwx   0        0        0        0 2024-04-18 09:39:36.711516 prosuite-1.2.3.0/prosuite.egg-info/
+-rw-rw-rw-   0        0        0     1792 2024-04-18 09:39:36.000000 prosuite-1.2.3.0/prosuite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1216 2024-04-18 09:39:36.000000 prosuite-1.2.3.0/prosuite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 09:39:36.000000 prosuite-1.2.3.0/prosuite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-18 09:39:36.000000 prosuite-1.2.3.0/prosuite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 09:39:36.000000 prosuite-1.2.3.0/prosuite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       84 2023-02-24 14:29:45.000000 prosuite-1.2.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      925 2024-04-18 09:39:36.713524 prosuite-1.2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-02-24 14:29:45.000000 prosuite-1.2.3.0/setup.py
```

### Comparing `prosuite-1.2.2.0/LICENSE` & `prosuite-1.2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/PKG-INFO` & `prosuite-1.2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosuite
-Version: 1.2.2.0
+Version: 1.2.3.0
 Summary: An API to configure quality assurance tests for geodata and execute quality verifications on a ProSuite Server
 Home-page: https://dirageosystems.ch/prosuite/doc/api
 Author: Dira GeoSystems
 Author-email: programmers@dirageosystems.ch
 License: MIT
 Keywords: prosuite,gis,arcgis,geodata,spatial-data,quality,quality-assurance,qa,test
 Classifier: Operating System :: OS Independent
```

### Comparing `prosuite-1.2.2.0/README.md` & `prosuite-1.2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/__init__.py` & `prosuite-1.2.3.0/prosuite/__init__.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/data_model.py` & `prosuite-1.2.3.0/prosuite/data_model.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/factories/enums.py` & `prosuite-1.2.3.0/prosuite/factories/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿__author__ = "The ProSuite Authors"
 __copyright__ = "Copyright 2021-2024, The ProSuite Authors"
 __license__ = "MIT"
-__version__ = "1.2.1.4"
+__version__ = "1.2.3.0"
 __maintainer__ = "Dira GeoSystems"
 __email__ = "programmers@dirageosystems.ch"
-__date__  = "30/01/2024"
+__date__  = "18.04.2024"
 __status__ = "Production"
 
 
 from datetime import datetime
 from typing import List
```

### Comparing `prosuite-1.2.2.0/prosuite/factories/issue_filters.py` & `prosuite-1.2.3.0/prosuite/factories/issue_filters.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/factories/quality_conditions.py` & `prosuite-1.2.3.0/prosuite/factories/quality_conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿__author__ = "The ProSuite Authors"
 __copyright__ = "Copyright 2021-2024, The ProSuite Authors"
 __license__ = "MIT"
-__version__ = "1.2.1.4"
+__version__ = "1.2.3.0"
 __maintainer__ = "Dira GeoSystems"
 __email__ = "programmers@dirageosystems.ch"
-__date__  = "30/01/2024"
+__date__  = "18.04.2024"
 __status__ = "Production"
 
 
 from datetime import datetime
 from typing import List
 from prosuite.quality import Parameter, Condition
 from prosuite.data_model import BaseDataset
@@ -6901,28 +6901,28 @@
         A variable expression is formatted "<variablename>:<count expression>" (Example: "v1:Objektart=r"). The value of the variable is equal the count of the features at a point that fulfill the <count expression> (for the corresponding feature Class).
         For polyline featureclasses, an additional attribute "_StartsIn" is available in the count expression. The attribute value is true, if the FromPoint of the polyline lies at the point, and false, if the ToPoint lies at the point. Remark: If the FromPoint and ToPoint of a polyline are coincident, the polyline corresponds to two features in that point, one with _StartsIn=true and one with _StartsIn=false.  
         
         A count expression checks if the variables fulfill a condition (Example: "v1 =1 AND v2=1", where v1, v2 are declared variables). If the count expression is false, the corresponding rule is considered invalid and the next rules are checked for validity. A count expression can \/should use all variables declared in any expression of the corresponding rule. If a variable is not use in the count expression, the variable can be ommitted.
         
         Example:
         featureClasses: A, B
-        rules = {
-            { "ObjektArt IN (x,y)", "ObjektArt IN (u,v)" }, 
-                \/\/ Meaning: all involved features belong either to A with ObjektArt in (x,y) or to B with ObjektArt in (u,v)
+        rules:
+        {
+          { "ObjektArt IN (x,y)", "ObjektArt IN (u,v)" }, 
+              \/\/ Meaning: all involved features belong either to A with ObjektArt in (x,y) or to B with ObjektArt in (u,v)
         
-            { "ObjektArt = z", null },
-                \/\/ Meaning: No B-Feature must touch any A-Feature with ObjektArt = z
+          { "ObjektArt = z", null },
+             \/\/ Meaning: No B-Feature must touch any A-Feature with ObjektArt = z
         
-            { null, "ObjektArt = t" },
-                \/\/ Meaning: no A-Feature must touch any B-Feature with ObjektArt = t
+          { null, "ObjektArt = t" },
+             \/\/ Meaning: no A-Feature must touch any B-Feature with ObjektArt = t
         
-            { "true;v1:ObjektArt=r;v2:Objektart=s;", "ObjektArt in (u,v);v1 =1 AND v2=1" }
-                \/\/ Meaning: all feature of A and the features of B in (u,v) can be involved. Additionally, the count of A.ObjektArt =r must be 1 and the count of A.ObjektArt=s must be 1
+          { "true;v1:ObjektArt=r;v2:Objektart=s;", "ObjektArt in (u,v);v1 =1 AND v2=1" }
+             \/\/ Meaning: all feature of A and the features of B in (u,v) can be involved. Additionally, the count of A.ObjektArt =r must be 1 and the count of A.ObjektArt=s must be 1
         }
-
         """
         
         result = Condition("QaLineConnection")
         if type(feature_classes) == list:
             for element in feature_classes:
                 result.parameters.append(Parameter("featureClasses", element))
         else:
```

### Comparing `prosuite-1.2.2.0/prosuite/factories/transformers.py` & `prosuite-1.2.3.0/prosuite/factories/transformers.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/generated/quality_test_pb2.py` & `prosuite-1.2.3.0/prosuite/generated/quality_test_pb2.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: quality_test.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-import shared_types_pb2 as shared__types__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12quality_test.proto\x12*ProSuite.Microservices.Definitions.QA.Test\x1a\x12shared_types.proto\"\xa5\x02\n\x12\x45xecuteTestRequest\x12K\n\nworkspaces\x18\x01 \x03(\x0b\x32\x37.ProSuite.Microservices.Definitions.Shared.WorkspaceMsg\x12S\n\x0finvolved_tables\x18\x02 \x03(\x0b\x32:.ProSuite.Microservices.Definitions.QA.Test.TestDatasetMsg\x12\x46\n\tperimeter\x18\x03 \x01(\x0b\x32\x33.ProSuite.Microservices.Definitions.Shared.ShapeMsg\x12\x11\n\ttest_name\x18\x04 \x01(\t\x12\x12\n\nparameters\x18\x05 \x03(\t\"\xcf\x01\n\x13\x45xecuteTestResponse\x12\x1b\n\x13service_call_status\x18\x01 \x01(\x05\x12M\n\x08progress\x18\x02 \x01(\x0b\x32;.ProSuite.Microservices.Definitions.QA.Test.TestProgressMsg\x12L\n\x06issues\x18\x03 \x03(\x0b\x32<.ProSuite.Microservices.Definitions.QA.Test.DetectedIssueMsg\"\x80\x01\n\x0eTestDatasetMsg\x12S\n\x10\x63lass_definition\x18\x01 \x01(\x0b\x32\x39.ProSuite.Microservices.Definitions.Shared.ObjectClassMsg\x12\x19\n\x11\x66ilter_expression\x18\x02 \x01(\t\"_\n\x0fTestProgressMsg\x12\x1c\n\x14progress_total_steps\x18\x01 \x01(\x05\x12\x1d\n\x15progress_current_step\x18\x02 \x01(\x05\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xdb\x02\n\x10\x44\x65tectedIssueMsg\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12K\n\x0eissue_geometry\x18\x02 \x01(\x0b\x32\x33.ProSuite.Microservices.Definitions.Shared.ShapeMsg\x12\x15\n\rissue_code_id\x18\x03 \x01(\t\x12\x1e\n\x16issue_code_description\x18\x04 \x01(\t\x12X\n\x10involved_objects\x18\x05 \x03(\x0b\x32>.ProSuite.Microservices.Definitions.QA.Test.InvolvedObjectsMsg\x12\x16\n\x0estop_condition\x18\x06 \x01(\x08\x12\x1a\n\x12\x61\x66\x66\x65\x63ted_component\x18\x07 \x01(\t\x12 \n\x18\x63reation_date_time_ticks\x18\x08 \x01(\x03\"t\n\x12InvolvedObjectsMsg\x12J\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x39.ProSuite.Microservices.Definitions.Shared.ObjectClassMsg\x12\x12\n\nobject_ids\x18\x02 \x03(\x03\x32\xa2\x01\n\x0fQualityTestGrpc\x12\x8e\x01\n\x07\x45xecute\x12>.ProSuite.Microservices.Definitions.QA.Test.ExecuteTestRequest\x1a?.ProSuite.Microservices.Definitions.QA.Test.ExecuteTestResponse\"\x00\x30\x01\x62\x06proto3')
-
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'quality_test_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  _EXECUTETESTREQUEST._serialized_start=87
-  _EXECUTETESTREQUEST._serialized_end=380
-  _EXECUTETESTRESPONSE._serialized_start=383
-  _EXECUTETESTRESPONSE._serialized_end=590
-  _TESTDATASETMSG._serialized_start=593
-  _TESTDATASETMSG._serialized_end=721
-  _TESTPROGRESSMSG._serialized_start=723
-  _TESTPROGRESSMSG._serialized_end=818
-  _DETECTEDISSUEMSG._serialized_start=821
-  _DETECTEDISSUEMSG._serialized_end=1168
-  _INVOLVEDOBJECTSMSG._serialized_start=1170
-  _INVOLVEDOBJECTSMSG._serialized_end=1286
-  _QUALITYTESTGRPC._serialized_start=1289
-  _QUALITYTESTGRPC._serialized_end=1451
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: quality_test.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+import shared_types_pb2 as shared__types__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12quality_test.proto\x12*ProSuite.Microservices.Definitions.QA.Test\x1a\x12shared_types.proto\"\xa5\x02\n\x12\x45xecuteTestRequest\x12K\n\nworkspaces\x18\x01 \x03(\x0b\x32\x37.ProSuite.Microservices.Definitions.Shared.WorkspaceMsg\x12S\n\x0finvolved_tables\x18\x02 \x03(\x0b\x32:.ProSuite.Microservices.Definitions.QA.Test.TestDatasetMsg\x12\x46\n\tperimeter\x18\x03 \x01(\x0b\x32\x33.ProSuite.Microservices.Definitions.Shared.ShapeMsg\x12\x11\n\ttest_name\x18\x04 \x01(\t\x12\x12\n\nparameters\x18\x05 \x03(\t\"\xcf\x01\n\x13\x45xecuteTestResponse\x12\x1b\n\x13service_call_status\x18\x01 \x01(\x05\x12M\n\x08progress\x18\x02 \x01(\x0b\x32;.ProSuite.Microservices.Definitions.QA.Test.TestProgressMsg\x12L\n\x06issues\x18\x03 \x03(\x0b\x32<.ProSuite.Microservices.Definitions.QA.Test.DetectedIssueMsg\"\x80\x01\n\x0eTestDatasetMsg\x12S\n\x10\x63lass_definition\x18\x01 \x01(\x0b\x32\x39.ProSuite.Microservices.Definitions.Shared.ObjectClassMsg\x12\x19\n\x11\x66ilter_expression\x18\x02 \x01(\t\"_\n\x0fTestProgressMsg\x12\x1c\n\x14progress_total_steps\x18\x01 \x01(\x05\x12\x1d\n\x15progress_current_step\x18\x02 \x01(\x05\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xdb\x02\n\x10\x44\x65tectedIssueMsg\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12K\n\x0eissue_geometry\x18\x02 \x01(\x0b\x32\x33.ProSuite.Microservices.Definitions.Shared.ShapeMsg\x12\x15\n\rissue_code_id\x18\x03 \x01(\t\x12\x1e\n\x16issue_code_description\x18\x04 \x01(\t\x12X\n\x10involved_objects\x18\x05 \x03(\x0b\x32>.ProSuite.Microservices.Definitions.QA.Test.InvolvedObjectsMsg\x12\x16\n\x0estop_condition\x18\x06 \x01(\x08\x12\x1a\n\x12\x61\x66\x66\x65\x63ted_component\x18\x07 \x01(\t\x12 \n\x18\x63reation_date_time_ticks\x18\x08 \x01(\x03\"t\n\x12InvolvedObjectsMsg\x12J\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x39.ProSuite.Microservices.Definitions.Shared.ObjectClassMsg\x12\x12\n\nobject_ids\x18\x02 \x03(\x03\x32\xa2\x01\n\x0fQualityTestGrpc\x12\x8e\x01\n\x07\x45xecute\x12>.ProSuite.Microservices.Definitions.QA.Test.ExecuteTestRequest\x1a?.ProSuite.Microservices.Definitions.QA.Test.ExecuteTestResponse\"\x00\x30\x01\x62\x06proto3')
+
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'quality_test_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _EXECUTETESTREQUEST._serialized_start=87
+  _EXECUTETESTREQUEST._serialized_end=380
+  _EXECUTETESTRESPONSE._serialized_start=383
+  _EXECUTETESTRESPONSE._serialized_end=590
+  _TESTDATASETMSG._serialized_start=593
+  _TESTDATASETMSG._serialized_end=721
+  _TESTPROGRESSMSG._serialized_start=723
+  _TESTPROGRESSMSG._serialized_end=818
+  _DETECTEDISSUEMSG._serialized_start=821
+  _DETECTEDISSUEMSG._serialized_end=1168
+  _INVOLVEDOBJECTSMSG._serialized_start=1170
+  _INVOLVEDOBJECTSMSG._serialized_end=1286
+  _QUALITYTESTGRPC._serialized_start=1289
+  _QUALITYTESTGRPC._serialized_end=1451
+# @@protoc_insertion_point(module_scope)
```

### Comparing `prosuite-1.2.2.0/prosuite/generated/quality_test_pb2.pyi` & `prosuite-1.2.3.0/prosuite/generated/quality_test_pb2.pyi`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import shared_types_pb2 as _shared_types_pb2
-from google.protobuf.internal import containers as _containers
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
-
-DESCRIPTOR: _descriptor.FileDescriptor
-
-class DetectedIssueMsg(_message.Message):
-    __slots__ = ["affected_component", "creation_date_time_ticks", "description", "involved_objects", "issue_code_description", "issue_code_id", "issue_geometry", "stop_condition"]
-    AFFECTED_COMPONENT_FIELD_NUMBER: _ClassVar[int]
-    CREATION_DATE_TIME_TICKS_FIELD_NUMBER: _ClassVar[int]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    INVOLVED_OBJECTS_FIELD_NUMBER: _ClassVar[int]
-    ISSUE_CODE_DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
-    ISSUE_CODE_ID_FIELD_NUMBER: _ClassVar[int]
-    ISSUE_GEOMETRY_FIELD_NUMBER: _ClassVar[int]
-    STOP_CONDITION_FIELD_NUMBER: _ClassVar[int]
-    affected_component: str
-    creation_date_time_ticks: int
-    description: str
-    involved_objects: _containers.RepeatedCompositeFieldContainer[InvolvedObjectsMsg]
-    issue_code_description: str
-    issue_code_id: str
-    issue_geometry: _shared_types_pb2.ShapeMsg
-    stop_condition: bool
-    def __init__(self, description: _Optional[str] = ..., issue_geometry: _Optional[_Union[_shared_types_pb2.ShapeMsg, _Mapping]] = ..., issue_code_id: _Optional[str] = ..., issue_code_description: _Optional[str] = ..., involved_objects: _Optional[_Iterable[_Union[InvolvedObjectsMsg, _Mapping]]] = ..., stop_condition: bool = ..., affected_component: _Optional[str] = ..., creation_date_time_ticks: _Optional[int] = ...) -> None: ...
-
-class ExecuteTestRequest(_message.Message):
-    __slots__ = ["involved_tables", "parameters", "perimeter", "test_name", "workspaces"]
-    INVOLVED_TABLES_FIELD_NUMBER: _ClassVar[int]
-    PARAMETERS_FIELD_NUMBER: _ClassVar[int]
-    PERIMETER_FIELD_NUMBER: _ClassVar[int]
-    TEST_NAME_FIELD_NUMBER: _ClassVar[int]
-    WORKSPACES_FIELD_NUMBER: _ClassVar[int]
-    involved_tables: _containers.RepeatedCompositeFieldContainer[TestDatasetMsg]
-    parameters: _containers.RepeatedScalarFieldContainer[str]
-    perimeter: _shared_types_pb2.ShapeMsg
-    test_name: str
-    workspaces: _containers.RepeatedCompositeFieldContainer[_shared_types_pb2.WorkspaceMsg]
-    def __init__(self, workspaces: _Optional[_Iterable[_Union[_shared_types_pb2.WorkspaceMsg, _Mapping]]] = ..., involved_tables: _Optional[_Iterable[_Union[TestDatasetMsg, _Mapping]]] = ..., perimeter: _Optional[_Union[_shared_types_pb2.ShapeMsg, _Mapping]] = ..., test_name: _Optional[str] = ..., parameters: _Optional[_Iterable[str]] = ...) -> None: ...
-
-class ExecuteTestResponse(_message.Message):
-    __slots__ = ["issues", "progress", "service_call_status"]
-    ISSUES_FIELD_NUMBER: _ClassVar[int]
-    PROGRESS_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_CALL_STATUS_FIELD_NUMBER: _ClassVar[int]
-    issues: _containers.RepeatedCompositeFieldContainer[DetectedIssueMsg]
-    progress: TestProgressMsg
-    service_call_status: int
-    def __init__(self, service_call_status: _Optional[int] = ..., progress: _Optional[_Union[TestProgressMsg, _Mapping]] = ..., issues: _Optional[_Iterable[_Union[DetectedIssueMsg, _Mapping]]] = ...) -> None: ...
-
-class InvolvedObjectsMsg(_message.Message):
-    __slots__ = ["dataset", "object_ids"]
-    DATASET_FIELD_NUMBER: _ClassVar[int]
-    OBJECT_IDS_FIELD_NUMBER: _ClassVar[int]
-    dataset: _shared_types_pb2.ObjectClassMsg
-    object_ids: _containers.RepeatedScalarFieldContainer[int]
-    def __init__(self, dataset: _Optional[_Union[_shared_types_pb2.ObjectClassMsg, _Mapping]] = ..., object_ids: _Optional[_Iterable[int]] = ...) -> None: ...
-
-class TestDatasetMsg(_message.Message):
-    __slots__ = ["class_definition", "filter_expression"]
-    CLASS_DEFINITION_FIELD_NUMBER: _ClassVar[int]
-    FILTER_EXPRESSION_FIELD_NUMBER: _ClassVar[int]
-    class_definition: _shared_types_pb2.ObjectClassMsg
-    filter_expression: str
-    def __init__(self, class_definition: _Optional[_Union[_shared_types_pb2.ObjectClassMsg, _Mapping]] = ..., filter_expression: _Optional[str] = ...) -> None: ...
-
-class TestProgressMsg(_message.Message):
-    __slots__ = ["message", "progress_current_step", "progress_total_steps"]
-    MESSAGE_FIELD_NUMBER: _ClassVar[int]
-    PROGRESS_CURRENT_STEP_FIELD_NUMBER: _ClassVar[int]
-    PROGRESS_TOTAL_STEPS_FIELD_NUMBER: _ClassVar[int]
-    message: str
-    progress_current_step: int
-    progress_total_steps: int
-    def __init__(self, progress_total_steps: _Optional[int] = ..., progress_current_step: _Optional[int] = ..., message: _Optional[str] = ...) -> None: ...
+import shared_types_pb2 as _shared_types_pb2
+from google.protobuf.internal import containers as _containers
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+
+DESCRIPTOR: _descriptor.FileDescriptor
+
+class DetectedIssueMsg(_message.Message):
+    __slots__ = ["affected_component", "creation_date_time_ticks", "description", "involved_objects", "issue_code_description", "issue_code_id", "issue_geometry", "stop_condition"]
+    AFFECTED_COMPONENT_FIELD_NUMBER: _ClassVar[int]
+    CREATION_DATE_TIME_TICKS_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    INVOLVED_OBJECTS_FIELD_NUMBER: _ClassVar[int]
+    ISSUE_CODE_DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+    ISSUE_CODE_ID_FIELD_NUMBER: _ClassVar[int]
+    ISSUE_GEOMETRY_FIELD_NUMBER: _ClassVar[int]
+    STOP_CONDITION_FIELD_NUMBER: _ClassVar[int]
+    affected_component: str
+    creation_date_time_ticks: int
+    description: str
+    involved_objects: _containers.RepeatedCompositeFieldContainer[InvolvedObjectsMsg]
+    issue_code_description: str
+    issue_code_id: str
+    issue_geometry: _shared_types_pb2.ShapeMsg
+    stop_condition: bool
+    def __init__(self, description: _Optional[str] = ..., issue_geometry: _Optional[_Union[_shared_types_pb2.ShapeMsg, _Mapping]] = ..., issue_code_id: _Optional[str] = ..., issue_code_description: _Optional[str] = ..., involved_objects: _Optional[_Iterable[_Union[InvolvedObjectsMsg, _Mapping]]] = ..., stop_condition: bool = ..., affected_component: _Optional[str] = ..., creation_date_time_ticks: _Optional[int] = ...) -> None: ...
+
+class ExecuteTestRequest(_message.Message):
+    __slots__ = ["involved_tables", "parameters", "perimeter", "test_name", "workspaces"]
+    INVOLVED_TABLES_FIELD_NUMBER: _ClassVar[int]
+    PARAMETERS_FIELD_NUMBER: _ClassVar[int]
+    PERIMETER_FIELD_NUMBER: _ClassVar[int]
+    TEST_NAME_FIELD_NUMBER: _ClassVar[int]
+    WORKSPACES_FIELD_NUMBER: _ClassVar[int]
+    involved_tables: _containers.RepeatedCompositeFieldContainer[TestDatasetMsg]
+    parameters: _containers.RepeatedScalarFieldContainer[str]
+    perimeter: _shared_types_pb2.ShapeMsg
+    test_name: str
+    workspaces: _containers.RepeatedCompositeFieldContainer[_shared_types_pb2.WorkspaceMsg]
+    def __init__(self, workspaces: _Optional[_Iterable[_Union[_shared_types_pb2.WorkspaceMsg, _Mapping]]] = ..., involved_tables: _Optional[_Iterable[_Union[TestDatasetMsg, _Mapping]]] = ..., perimeter: _Optional[_Union[_shared_types_pb2.ShapeMsg, _Mapping]] = ..., test_name: _Optional[str] = ..., parameters: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class ExecuteTestResponse(_message.Message):
+    __slots__ = ["issues", "progress", "service_call_status"]
+    ISSUES_FIELD_NUMBER: _ClassVar[int]
+    PROGRESS_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_CALL_STATUS_FIELD_NUMBER: _ClassVar[int]
+    issues: _containers.RepeatedCompositeFieldContainer[DetectedIssueMsg]
+    progress: TestProgressMsg
+    service_call_status: int
+    def __init__(self, service_call_status: _Optional[int] = ..., progress: _Optional[_Union[TestProgressMsg, _Mapping]] = ..., issues: _Optional[_Iterable[_Union[DetectedIssueMsg, _Mapping]]] = ...) -> None: ...
+
+class InvolvedObjectsMsg(_message.Message):
+    __slots__ = ["dataset", "object_ids"]
+    DATASET_FIELD_NUMBER: _ClassVar[int]
+    OBJECT_IDS_FIELD_NUMBER: _ClassVar[int]
+    dataset: _shared_types_pb2.ObjectClassMsg
+    object_ids: _containers.RepeatedScalarFieldContainer[int]
+    def __init__(self, dataset: _Optional[_Union[_shared_types_pb2.ObjectClassMsg, _Mapping]] = ..., object_ids: _Optional[_Iterable[int]] = ...) -> None: ...
+
+class TestDatasetMsg(_message.Message):
+    __slots__ = ["class_definition", "filter_expression"]
+    CLASS_DEFINITION_FIELD_NUMBER: _ClassVar[int]
+    FILTER_EXPRESSION_FIELD_NUMBER: _ClassVar[int]
+    class_definition: _shared_types_pb2.ObjectClassMsg
+    filter_expression: str
+    def __init__(self, class_definition: _Optional[_Union[_shared_types_pb2.ObjectClassMsg, _Mapping]] = ..., filter_expression: _Optional[str] = ...) -> None: ...
+
+class TestProgressMsg(_message.Message):
+    __slots__ = ["message", "progress_current_step", "progress_total_steps"]
+    MESSAGE_FIELD_NUMBER: _ClassVar[int]
+    PROGRESS_CURRENT_STEP_FIELD_NUMBER: _ClassVar[int]
+    PROGRESS_TOTAL_STEPS_FIELD_NUMBER: _ClassVar[int]
+    message: str
+    progress_current_step: int
+    progress_total_steps: int
+    def __init__(self, progress_total_steps: _Optional[int] = ..., progress_current_step: _Optional[int] = ..., message: _Optional[str] = ...) -> None: ...
```

### Comparing `prosuite-1.2.2.0/prosuite/generated/quality_verification_service_pb2.py` & `prosuite-1.2.3.0/prosuite/generated/quality_verification_service_pb2.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: quality_verification_service.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-import shared_types_pb2 as shared__types__pb2
-import shared_qa_pb2 as shared__qa__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"quality_verification_service.proto\x12%ProSuite.Microservices.Definitions.QA\x1a\x12shared_types.proto\x1a\x0fshared_qa.proto\"\xa3\x03\n\x13VerificationRequest\x12K\n\x0cwork_context\x18\x01 \x01(\x0b\x32\x35.ProSuite.Microservices.Definitions.QA.WorkContextMsg\x12U\n\rspecification\x18\x02 \x01(\x0b\x32>.ProSuite.Microservices.Definitions.QA.QualitySpecificationMsg\x12T\n\nparameters\x18\x03 \x01(\x0b\x32@.ProSuite.Microservices.Definitions.QA.VerificationParametersMsg\x12I\n\x08\x66\x65\x61tures\x18\x05 \x03(\x0b\x32\x37.ProSuite.Microservices.Definitions.Shared.GdbObjectMsg\x12\x11\n\tuser_name\x18\x06 \x01(\t\x12\x1f\n\x17max_parallel_processing\x18\x07 \x01(\x05\x12\x13\n\x0b\x65nvironment\x18\x08 \x01(\t\"\xe6\x01\n\x17\x44\x61taVerificationRequest\x12K\n\x07request\x18\x01 \x01(\x0b\x32:.ProSuite.Microservices.Definitions.QA.VerificationRequest\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..ProSuite.Microservices.Definitions.QA.GdbData\x12@\n\x06schema\x18\x03 \x01(\x0b\x32\x30.ProSuite.Microservices.Definitions.QA.SchemaMsg\"\x81\x03\n\x1dStandaloneVerificationRequest\x12^\n\x11xml_specification\x18\x01 \x01(\x0b\x32\x41.ProSuite.Microservices.Definitions.QA.XmlQualitySpecificationMsgH\x00\x12l\n\x1c\x63ondition_list_specification\x18\x04 \x01(\x0b\x32\x44.ProSuite.Microservices.Definitions.QA.ConditionListSpecificationMsgH\x00\x12T\n\nparameters\x18\x02 \x01(\x0b\x32@.ProSuite.Microservices.Definitions.QA.VerificationParametersMsg\x12\x18\n\x10output_directory\x18\x03 \x01(\t\x12\x11\n\tuser_name\x18\x06 \x01(\tB\x0f\n\rspecification\"\xca\x03\n\x14VerificationResponse\x12\x1b\n\x13service_call_status\x18\x01 \x01(\x05\x12P\n\x08progress\x18\x02 \x01(\x0b\x32>.ProSuite.Microservices.Definitions.QA.VerificationProgressMsg\x12?\n\x06issues\x18\x03 \x03(\x0b\x32/.ProSuite.Microservices.Definitions.QA.IssueMsg\x12[\n\x14quality_verification\x18\x04 \x01(\x0b\x32=.ProSuite.Microservices.Definitions.QA.QualityVerificationMsg\x12O\n\x12verified_perimeter\x18\x05 \x01(\x0b\x32\x33.ProSuite.Microservices.Definitions.Shared.ShapeMsg\x12T\n\x13obsolete_exceptions\x18\x06 \x03(\x0b\x32\x37.ProSuite.Microservices.Definitions.Shared.GdbObjRefMsg\"\x81\x02\n\x18\x44\x61taVerificationResponse\x12M\n\x08response\x18\x01 \x01(\x0b\x32;.ProSuite.Microservices.Definitions.QA.VerificationResponse\x12H\n\x0c\x64\x61ta_request\x18\x02 \x01(\x0b\x32\x32.ProSuite.Microservices.Definitions.QA.DataRequest\x12L\n\x0eschema_request\x18\x03 \x01(\x0b\x32\x34.ProSuite.Microservices.Definitions.QA.SchemaRequest\"\xbe\x01\n\x1eStandaloneVerificationResponse\x12\x1b\n\x13service_call_status\x18\x01 \x01(\x05\x12>\n\x07message\x18\x02 \x01(\x0b\x32-.ProSuite.Microservices.Definitions.QA.LogMsg\x12?\n\x06issues\x18\x03 \x03(\x0b\x32/.ProSuite.Microservices.Definitions.QA.IssueMsg2\xee\x03\n\x17QualityVerificationGrpc\x12\x8c\x01\n\rVerifyQuality\x12:.ProSuite.Microservices.Definitions.QA.VerificationRequest\x1a;.ProSuite.Microservices.Definitions.QA.VerificationResponse\"\x00\x30\x01\x12\x9a\x01\n\x11VerifyDataQuality\x12>.ProSuite.Microservices.Definitions.QA.DataVerificationRequest\x1a?.ProSuite.Microservices.Definitions.QA.DataVerificationResponse\"\x00(\x01\x30\x01\x12\xa6\x01\n\x13VerifyStandaloneXml\x12\x44.ProSuite.Microservices.Definitions.QA.StandaloneVerificationRequest\x1a\x45.ProSuite.Microservices.Definitions.QA.StandaloneVerificationResponse\"\x00\x30\x01\x62\x06proto3')
-
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'quality_verification_service_pb2', globals())
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  _VERIFICATIONREQUEST._serialized_start=115
-  _VERIFICATIONREQUEST._serialized_end=534
-  _DATAVERIFICATIONREQUEST._serialized_start=537
-  _DATAVERIFICATIONREQUEST._serialized_end=767
-  _STANDALONEVERIFICATIONREQUEST._serialized_start=770
-  _STANDALONEVERIFICATIONREQUEST._serialized_end=1155
-  _VERIFICATIONRESPONSE._serialized_start=1158
-  _VERIFICATIONRESPONSE._serialized_end=1616
-  _DATAVERIFICATIONRESPONSE._serialized_start=1619
-  _DATAVERIFICATIONRESPONSE._serialized_end=1876
-  _STANDALONEVERIFICATIONRESPONSE._serialized_start=1879
-  _STANDALONEVERIFICATIONRESPONSE._serialized_end=2069
-  _QUALITYVERIFICATIONGRPC._serialized_start=2072
-  _QUALITYVERIFICATIONGRPC._serialized_end=2566
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: quality_verification_service.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import builder as _builder
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+import shared_types_pb2 as shared__types__pb2
+import shared_qa_pb2 as shared__qa__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"quality_verification_service.proto\x12%ProSuite.Microservices.Definitions.QA\x1a\x12shared_types.proto\x1a\x0fshared_qa.proto\"\xa3\x03\n\x13VerificationRequest\x12K\n\x0cwork_context\x18\x01 \x01(\x0b\x32\x35.ProSuite.Microservices.Definitions.QA.WorkContextMsg\x12U\n\rspecification\x18\x02 \x01(\x0b\x32>.ProSuite.Microservices.Definitions.QA.QualitySpecificationMsg\x12T\n\nparameters\x18\x03 \x01(\x0b\x32@.ProSuite.Microservices.Definitions.QA.VerificationParametersMsg\x12I\n\x08\x66\x65\x61tures\x18\x05 \x03(\x0b\x32\x37.ProSuite.Microservices.Definitions.Shared.GdbObjectMsg\x12\x11\n\tuser_name\x18\x06 \x01(\t\x12\x1f\n\x17max_parallel_processing\x18\x07 \x01(\x05\x12\x13\n\x0b\x65nvironment\x18\x08 \x01(\t\"\xe6\x01\n\x17\x44\x61taVerificationRequest\x12K\n\x07request\x18\x01 \x01(\x0b\x32:.ProSuite.Microservices.Definitions.QA.VerificationRequest\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..ProSuite.Microservices.Definitions.QA.GdbData\x12@\n\x06schema\x18\x03 \x01(\x0b\x32\x30.ProSuite.Microservices.Definitions.QA.SchemaMsg\"\x81\x03\n\x1dStandaloneVerificationRequest\x12^\n\x11xml_specification\x18\x01 \x01(\x0b\x32\x41.ProSuite.Microservices.Definitions.QA.XmlQualitySpecificationMsgH\x00\x12l\n\x1c\x63ondition_list_specification\x18\x04 \x01(\x0b\x32\x44.ProSuite.Microservices.Definitions.QA.ConditionListSpecificationMsgH\x00\x12T\n\nparameters\x18\x02 \x01(\x0b\x32@.ProSuite.Microservices.Definitions.QA.VerificationParametersMsg\x12\x18\n\x10output_directory\x18\x03 \x01(\t\x12\x11\n\tuser_name\x18\x06 \x01(\tB\x0f\n\rspecification\"\xca\x03\n\x14VerificationResponse\x12\x1b\n\x13service_call_status\x18\x01 \x01(\x05\x12P\n\x08progress\x18\x02 \x01(\x0b\x32>.ProSuite.Microservices.Definitions.QA.VerificationProgressMsg\x12?\n\x06issues\x18\x03 \x03(\x0b\x32/.ProSuite.Microservices.Definitions.QA.IssueMsg\x12[\n\x14quality_verification\x18\x04 \x01(\x0b\x32=.ProSuite.Microservices.Definitions.QA.QualityVerificationMsg\x12O\n\x12verified_perimeter\x18\x05 \x01(\x0b\x32\x33.ProSuite.Microservices.Definitions.Shared.ShapeMsg\x12T\n\x13obsolete_exceptions\x18\x06 \x03(\x0b\x32\x37.ProSuite.Microservices.Definitions.Shared.GdbObjRefMsg\"\x81\x02\n\x18\x44\x61taVerificationResponse\x12M\n\x08response\x18\x01 \x01(\x0b\x32;.ProSuite.Microservices.Definitions.QA.VerificationResponse\x12H\n\x0c\x64\x61ta_request\x18\x02 \x01(\x0b\x32\x32.ProSuite.Microservices.Definitions.QA.DataRequest\x12L\n\x0eschema_request\x18\x03 \x01(\x0b\x32\x34.ProSuite.Microservices.Definitions.QA.SchemaRequest\"\xbe\x01\n\x1eStandaloneVerificationResponse\x12\x1b\n\x13service_call_status\x18\x01 \x01(\x05\x12>\n\x07message\x18\x02 \x01(\x0b\x32-.ProSuite.Microservices.Definitions.QA.LogMsg\x12?\n\x06issues\x18\x03 \x03(\x0b\x32/.ProSuite.Microservices.Definitions.QA.IssueMsg2\xee\x03\n\x17QualityVerificationGrpc\x12\x8c\x01\n\rVerifyQuality\x12:.ProSuite.Microservices.Definitions.QA.VerificationRequest\x1a;.ProSuite.Microservices.Definitions.QA.VerificationResponse\"\x00\x30\x01\x12\x9a\x01\n\x11VerifyDataQuality\x12>.ProSuite.Microservices.Definitions.QA.DataVerificationRequest\x1a?.ProSuite.Microservices.Definitions.QA.DataVerificationResponse\"\x00(\x01\x30\x01\x12\xa6\x01\n\x13VerifyStandaloneXml\x12\x44.ProSuite.Microservices.Definitions.QA.StandaloneVerificationRequest\x1a\x45.ProSuite.Microservices.Definitions.QA.StandaloneVerificationResponse\"\x00\x30\x01\x62\x06proto3')
+
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'quality_verification_service_pb2', globals())
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _VERIFICATIONREQUEST._serialized_start=115
+  _VERIFICATIONREQUEST._serialized_end=534
+  _DATAVERIFICATIONREQUEST._serialized_start=537
+  _DATAVERIFICATIONREQUEST._serialized_end=767
+  _STANDALONEVERIFICATIONREQUEST._serialized_start=770
+  _STANDALONEVERIFICATIONREQUEST._serialized_end=1155
+  _VERIFICATIONRESPONSE._serialized_start=1158
+  _VERIFICATIONRESPONSE._serialized_end=1616
+  _DATAVERIFICATIONRESPONSE._serialized_start=1619
+  _DATAVERIFICATIONRESPONSE._serialized_end=1876
+  _STANDALONEVERIFICATIONRESPONSE._serialized_start=1879
+  _STANDALONEVERIFICATIONRESPONSE._serialized_end=2069
+  _QUALITYVERIFICATIONGRPC._serialized_start=2072
+  _QUALITYVERIFICATIONGRPC._serialized_end=2566
+# @@protoc_insertion_point(module_scope)
```

### Comparing `prosuite-1.2.2.0/prosuite/generated/quality_verification_service_pb2.pyi` & `prosuite-1.2.3.0/prosuite/generated/quality_verification_service_pb2.pyi`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import shared_types_pb2 as _shared_types_pb2
-import shared_qa_pb2 as _shared_qa_pb2
-from google.protobuf.internal import containers as _containers
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
-
-DESCRIPTOR: _descriptor.FileDescriptor
-
-class DataVerificationRequest(_message.Message):
-    __slots__ = ["data", "request", "schema"]
-    DATA_FIELD_NUMBER: _ClassVar[int]
-    REQUEST_FIELD_NUMBER: _ClassVar[int]
-    SCHEMA_FIELD_NUMBER: _ClassVar[int]
-    data: _shared_qa_pb2.GdbData
-    request: VerificationRequest
-    schema: _shared_qa_pb2.SchemaMsg
-    def __init__(self, request: _Optional[_Union[VerificationRequest, _Mapping]] = ..., data: _Optional[_Union[_shared_qa_pb2.GdbData, _Mapping]] = ..., schema: _Optional[_Union[_shared_qa_pb2.SchemaMsg, _Mapping]] = ...) -> None: ...
-
-class DataVerificationResponse(_message.Message):
-    __slots__ = ["data_request", "response", "schema_request"]
-    DATA_REQUEST_FIELD_NUMBER: _ClassVar[int]
-    RESPONSE_FIELD_NUMBER: _ClassVar[int]
-    SCHEMA_REQUEST_FIELD_NUMBER: _ClassVar[int]
-    data_request: _shared_qa_pb2.DataRequest
-    response: VerificationResponse
-    schema_request: _shared_qa_pb2.SchemaRequest
-    def __init__(self, response: _Optional[_Union[VerificationResponse, _Mapping]] = ..., data_request: _Optional[_Union[_shared_qa_pb2.DataRequest, _Mapping]] = ..., schema_request: _Optional[_Union[_shared_qa_pb2.SchemaRequest, _Mapping]] = ...) -> None: ...
-
-class StandaloneVerificationRequest(_message.Message):
-    __slots__ = ["condition_list_specification", "output_directory", "parameters", "user_name", "xml_specification"]
-    CONDITION_LIST_SPECIFICATION_FIELD_NUMBER: _ClassVar[int]
-    OUTPUT_DIRECTORY_FIELD_NUMBER: _ClassVar[int]
-    PARAMETERS_FIELD_NUMBER: _ClassVar[int]
-    USER_NAME_FIELD_NUMBER: _ClassVar[int]
-    XML_SPECIFICATION_FIELD_NUMBER: _ClassVar[int]
-    condition_list_specification: _shared_qa_pb2.ConditionListSpecificationMsg
-    output_directory: str
-    parameters: _shared_qa_pb2.VerificationParametersMsg
-    user_name: str
-    xml_specification: _shared_qa_pb2.XmlQualitySpecificationMsg
-    def __init__(self, xml_specification: _Optional[_Union[_shared_qa_pb2.XmlQualitySpecificationMsg, _Mapping]] = ..., condition_list_specification: _Optional[_Union[_shared_qa_pb2.ConditionListSpecificationMsg, _Mapping]] = ..., parameters: _Optional[_Union[_shared_qa_pb2.VerificationParametersMsg, _Mapping]] = ..., output_directory: _Optional[str] = ..., user_name: _Optional[str] = ...) -> None: ...
-
-class StandaloneVerificationResponse(_message.Message):
-    __slots__ = ["issues", "message", "service_call_status"]
-    ISSUES_FIELD_NUMBER: _ClassVar[int]
-    MESSAGE_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_CALL_STATUS_FIELD_NUMBER: _ClassVar[int]
-    issues: _containers.RepeatedCompositeFieldContainer[_shared_qa_pb2.IssueMsg]
-    message: _shared_qa_pb2.LogMsg
-    service_call_status: int
-    def __init__(self, service_call_status: _Optional[int] = ..., message: _Optional[_Union[_shared_qa_pb2.LogMsg, _Mapping]] = ..., issues: _Optional[_Iterable[_Union[_shared_qa_pb2.IssueMsg, _Mapping]]] = ...) -> None: ...
-
-class VerificationRequest(_message.Message):
-    __slots__ = ["environment", "features", "max_parallel_processing", "parameters", "specification", "user_name", "work_context"]
-    ENVIRONMENT_FIELD_NUMBER: _ClassVar[int]
-    FEATURES_FIELD_NUMBER: _ClassVar[int]
-    MAX_PARALLEL_PROCESSING_FIELD_NUMBER: _ClassVar[int]
-    PARAMETERS_FIELD_NUMBER: _ClassVar[int]
-    SPECIFICATION_FIELD_NUMBER: _ClassVar[int]
-    USER_NAME_FIELD_NUMBER: _ClassVar[int]
-    WORK_CONTEXT_FIELD_NUMBER: _ClassVar[int]
-    environment: str
-    features: _containers.RepeatedCompositeFieldContainer[_shared_types_pb2.GdbObjectMsg]
-    max_parallel_processing: int
-    parameters: _shared_qa_pb2.VerificationParametersMsg
-    specification: _shared_qa_pb2.QualitySpecificationMsg
-    user_name: str
-    work_context: _shared_qa_pb2.WorkContextMsg
-    def __init__(self, work_context: _Optional[_Union[_shared_qa_pb2.WorkContextMsg, _Mapping]] = ..., specification: _Optional[_Union[_shared_qa_pb2.QualitySpecificationMsg, _Mapping]] = ..., parameters: _Optional[_Union[_shared_qa_pb2.VerificationParametersMsg, _Mapping]] = ..., features: _Optional[_Iterable[_Union[_shared_types_pb2.GdbObjectMsg, _Mapping]]] = ..., user_name: _Optional[str] = ..., max_parallel_processing: _Optional[int] = ..., environment: _Optional[str] = ...) -> None: ...
-
-class VerificationResponse(_message.Message):
-    __slots__ = ["issues", "obsolete_exceptions", "progress", "quality_verification", "service_call_status", "verified_perimeter"]
-    ISSUES_FIELD_NUMBER: _ClassVar[int]
-    OBSOLETE_EXCEPTIONS_FIELD_NUMBER: _ClassVar[int]
-    PROGRESS_FIELD_NUMBER: _ClassVar[int]
-    QUALITY_VERIFICATION_FIELD_NUMBER: _ClassVar[int]
-    SERVICE_CALL_STATUS_FIELD_NUMBER: _ClassVar[int]
-    VERIFIED_PERIMETER_FIELD_NUMBER: _ClassVar[int]
-    issues: _containers.RepeatedCompositeFieldContainer[_shared_qa_pb2.IssueMsg]
-    obsolete_exceptions: _containers.RepeatedCompositeFieldContainer[_shared_types_pb2.GdbObjRefMsg]
-    progress: _shared_qa_pb2.VerificationProgressMsg
-    quality_verification: _shared_qa_pb2.QualityVerificationMsg
-    service_call_status: int
-    verified_perimeter: _shared_types_pb2.ShapeMsg
-    def __init__(self, service_call_status: _Optional[int] = ..., progress: _Optional[_Union[_shared_qa_pb2.VerificationProgressMsg, _Mapping]] = ..., issues: _Optional[_Iterable[_Union[_shared_qa_pb2.IssueMsg, _Mapping]]] = ..., quality_verification: _Optional[_Union[_shared_qa_pb2.QualityVerificationMsg, _Mapping]] = ..., verified_perimeter: _Optional[_Union[_shared_types_pb2.ShapeMsg, _Mapping]] = ..., obsolete_exceptions: _Optional[_Iterable[_Union[_shared_types_pb2.GdbObjRefMsg, _Mapping]]] = ...) -> None: ...
+import shared_types_pb2 as _shared_types_pb2
+import shared_qa_pb2 as _shared_qa_pb2
+from google.protobuf.internal import containers as _containers
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import message as _message
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
+
+DESCRIPTOR: _descriptor.FileDescriptor
+
+class DataVerificationRequest(_message.Message):
+    __slots__ = ["data", "request", "schema"]
+    DATA_FIELD_NUMBER: _ClassVar[int]
+    REQUEST_FIELD_NUMBER: _ClassVar[int]
+    SCHEMA_FIELD_NUMBER: _ClassVar[int]
+    data: _shared_qa_pb2.GdbData
+    request: VerificationRequest
+    schema: _shared_qa_pb2.SchemaMsg
+    def __init__(self, request: _Optional[_Union[VerificationRequest, _Mapping]] = ..., data: _Optional[_Union[_shared_qa_pb2.GdbData, _Mapping]] = ..., schema: _Optional[_Union[_shared_qa_pb2.SchemaMsg, _Mapping]] = ...) -> None: ...
+
+class DataVerificationResponse(_message.Message):
+    __slots__ = ["data_request", "response", "schema_request"]
+    DATA_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    RESPONSE_FIELD_NUMBER: _ClassVar[int]
+    SCHEMA_REQUEST_FIELD_NUMBER: _ClassVar[int]
+    data_request: _shared_qa_pb2.DataRequest
+    response: VerificationResponse
+    schema_request: _shared_qa_pb2.SchemaRequest
+    def __init__(self, response: _Optional[_Union[VerificationResponse, _Mapping]] = ..., data_request: _Optional[_Union[_shared_qa_pb2.DataRequest, _Mapping]] = ..., schema_request: _Optional[_Union[_shared_qa_pb2.SchemaRequest, _Mapping]] = ...) -> None: ...
+
+class StandaloneVerificationRequest(_message.Message):
+    __slots__ = ["condition_list_specification", "output_directory", "parameters", "user_name", "xml_specification"]
+    CONDITION_LIST_SPECIFICATION_FIELD_NUMBER: _ClassVar[int]
+    OUTPUT_DIRECTORY_FIELD_NUMBER: _ClassVar[int]
+    PARAMETERS_FIELD_NUMBER: _ClassVar[int]
+    USER_NAME_FIELD_NUMBER: _ClassVar[int]
+    XML_SPECIFICATION_FIELD_NUMBER: _ClassVar[int]
+    condition_list_specification: _shared_qa_pb2.ConditionListSpecificationMsg
+    output_directory: str
+    parameters: _shared_qa_pb2.VerificationParametersMsg
+    user_name: str
+    xml_specification: _shared_qa_pb2.XmlQualitySpecificationMsg
+    def __init__(self, xml_specification: _Optional[_Union[_shared_qa_pb2.XmlQualitySpecificationMsg, _Mapping]] = ..., condition_list_specification: _Optional[_Union[_shared_qa_pb2.ConditionListSpecificationMsg, _Mapping]] = ..., parameters: _Optional[_Union[_shared_qa_pb2.VerificationParametersMsg, _Mapping]] = ..., output_directory: _Optional[str] = ..., user_name: _Optional[str] = ...) -> None: ...
+
+class StandaloneVerificationResponse(_message.Message):
+    __slots__ = ["issues", "message", "service_call_status"]
+    ISSUES_FIELD_NUMBER: _ClassVar[int]
+    MESSAGE_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_CALL_STATUS_FIELD_NUMBER: _ClassVar[int]
+    issues: _containers.RepeatedCompositeFieldContainer[_shared_qa_pb2.IssueMsg]
+    message: _shared_qa_pb2.LogMsg
+    service_call_status: int
+    def __init__(self, service_call_status: _Optional[int] = ..., message: _Optional[_Union[_shared_qa_pb2.LogMsg, _Mapping]] = ..., issues: _Optional[_Iterable[_Union[_shared_qa_pb2.IssueMsg, _Mapping]]] = ...) -> None: ...
+
+class VerificationRequest(_message.Message):
+    __slots__ = ["environment", "features", "max_parallel_processing", "parameters", "specification", "user_name", "work_context"]
+    ENVIRONMENT_FIELD_NUMBER: _ClassVar[int]
+    FEATURES_FIELD_NUMBER: _ClassVar[int]
+    MAX_PARALLEL_PROCESSING_FIELD_NUMBER: _ClassVar[int]
+    PARAMETERS_FIELD_NUMBER: _ClassVar[int]
+    SPECIFICATION_FIELD_NUMBER: _ClassVar[int]
+    USER_NAME_FIELD_NUMBER: _ClassVar[int]
+    WORK_CONTEXT_FIELD_NUMBER: _ClassVar[int]
+    environment: str
+    features: _containers.RepeatedCompositeFieldContainer[_shared_types_pb2.GdbObjectMsg]
+    max_parallel_processing: int
+    parameters: _shared_qa_pb2.VerificationParametersMsg
+    specification: _shared_qa_pb2.QualitySpecificationMsg
+    user_name: str
+    work_context: _shared_qa_pb2.WorkContextMsg
+    def __init__(self, work_context: _Optional[_Union[_shared_qa_pb2.WorkContextMsg, _Mapping]] = ..., specification: _Optional[_Union[_shared_qa_pb2.QualitySpecificationMsg, _Mapping]] = ..., parameters: _Optional[_Union[_shared_qa_pb2.VerificationParametersMsg, _Mapping]] = ..., features: _Optional[_Iterable[_Union[_shared_types_pb2.GdbObjectMsg, _Mapping]]] = ..., user_name: _Optional[str] = ..., max_parallel_processing: _Optional[int] = ..., environment: _Optional[str] = ...) -> None: ...
+
+class VerificationResponse(_message.Message):
+    __slots__ = ["issues", "obsolete_exceptions", "progress", "quality_verification", "service_call_status", "verified_perimeter"]
+    ISSUES_FIELD_NUMBER: _ClassVar[int]
+    OBSOLETE_EXCEPTIONS_FIELD_NUMBER: _ClassVar[int]
+    PROGRESS_FIELD_NUMBER: _ClassVar[int]
+    QUALITY_VERIFICATION_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_CALL_STATUS_FIELD_NUMBER: _ClassVar[int]
+    VERIFIED_PERIMETER_FIELD_NUMBER: _ClassVar[int]
+    issues: _containers.RepeatedCompositeFieldContainer[_shared_qa_pb2.IssueMsg]
+    obsolete_exceptions: _containers.RepeatedCompositeFieldContainer[_shared_types_pb2.GdbObjRefMsg]
+    progress: _shared_qa_pb2.VerificationProgressMsg
+    quality_verification: _shared_qa_pb2.QualityVerificationMsg
+    service_call_status: int
+    verified_perimeter: _shared_types_pb2.ShapeMsg
+    def __init__(self, service_call_status: _Optional[int] = ..., progress: _Optional[_Union[_shared_qa_pb2.VerificationProgressMsg, _Mapping]] = ..., issues: _Optional[_Iterable[_Union[_shared_qa_pb2.IssueMsg, _Mapping]]] = ..., quality_verification: _Optional[_Union[_shared_qa_pb2.QualityVerificationMsg, _Mapping]] = ..., verified_perimeter: _Optional[_Union[_shared_types_pb2.ShapeMsg, _Mapping]] = ..., obsolete_exceptions: _Optional[_Iterable[_Union[_shared_types_pb2.GdbObjRefMsg, _Mapping]]] = ...) -> None: ...
```

### Comparing `prosuite-1.2.2.0/prosuite/generated/quality_verification_service_pb2_grpc.py` & `prosuite-1.2.3.0/prosuite/generated/quality_verification_service_pb2_grpc.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
-import grpc
-
-import quality_verification_service_pb2 as quality__verification__service__pb2
-
-
-class QualityVerificationGrpcStub(object):
-    """*
-    The quality verification service definition.
-    """
-
-    def __init__(self, channel):
-        """Constructor.
-
-        Args:
-            channel: A grpc.Channel.
-        """
-        self.VerifyQuality = channel.unary_stream(
-                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyQuality',
-                request_serializer=quality__verification__service__pb2.VerificationRequest.SerializeToString,
-                response_deserializer=quality__verification__service__pb2.VerificationResponse.FromString,
-                )
-        self.VerifyDataQuality = channel.stream_stream(
-                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyDataQuality',
-                request_serializer=quality__verification__service__pb2.DataVerificationRequest.SerializeToString,
-                response_deserializer=quality__verification__service__pb2.DataVerificationResponse.FromString,
-                )
-        self.VerifyStandaloneXml = channel.unary_stream(
-                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyStandaloneXml',
-                request_serializer=quality__verification__service__pb2.StandaloneVerificationRequest.SerializeToString,
-                response_deserializer=quality__verification__service__pb2.StandaloneVerificationResponse.FromString,
-                )
-
-
-class QualityVerificationGrpcServicer(object):
-    """*
-    The quality verification service definition.
-    """
-
-    def VerifyQuality(self, request, context):
-        """*
-        Verifies the quality definied in the data dictionary.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def VerifyDataQuality(self, request_iterator, context):
-        """*
-        Experimental - Verifies the data quality definied in the data dictionary. The data is provided by the client.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def VerifyStandaloneXml(self, request, context):
-        """*
-        Verifies the quality using an XML definition instead of accessing the data dictionary.
-        This is a simplified interface with a basic response and no parallelism. Consider using
-        VerifyQuality instead.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-
-def add_QualityVerificationGrpcServicer_to_server(servicer, server):
-    rpc_method_handlers = {
-            'VerifyQuality': grpc.unary_stream_rpc_method_handler(
-                    servicer.VerifyQuality,
-                    request_deserializer=quality__verification__service__pb2.VerificationRequest.FromString,
-                    response_serializer=quality__verification__service__pb2.VerificationResponse.SerializeToString,
-            ),
-            'VerifyDataQuality': grpc.stream_stream_rpc_method_handler(
-                    servicer.VerifyDataQuality,
-                    request_deserializer=quality__verification__service__pb2.DataVerificationRequest.FromString,
-                    response_serializer=quality__verification__service__pb2.DataVerificationResponse.SerializeToString,
-            ),
-            'VerifyStandaloneXml': grpc.unary_stream_rpc_method_handler(
-                    servicer.VerifyStandaloneXml,
-                    request_deserializer=quality__verification__service__pb2.StandaloneVerificationRequest.FromString,
-                    response_serializer=quality__verification__service__pb2.StandaloneVerificationResponse.SerializeToString,
-            ),
-    }
-    generic_handler = grpc.method_handlers_generic_handler(
-            'ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc', rpc_method_handlers)
-    server.add_generic_rpc_handlers((generic_handler,))
-
-
- # This class is part of an EXPERIMENTAL API.
-class QualityVerificationGrpc(object):
-    """*
-    The quality verification service definition.
-    """
-
-    @staticmethod
-    def VerifyQuality(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyQuality',
-            quality__verification__service__pb2.VerificationRequest.SerializeToString,
-            quality__verification__service__pb2.VerificationResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def VerifyDataQuality(request_iterator,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.stream_stream(request_iterator, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyDataQuality',
-            quality__verification__service__pb2.DataVerificationRequest.SerializeToString,
-            quality__verification__service__pb2.DataVerificationResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def VerifyStandaloneXml(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyStandaloneXml',
-            quality__verification__service__pb2.StandaloneVerificationRequest.SerializeToString,
-            quality__verification__service__pb2.StandaloneVerificationResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+# Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
+"""Client and server classes corresponding to protobuf-defined services."""
+import grpc
+
+import quality_verification_service_pb2 as quality__verification__service__pb2
+
+
+class QualityVerificationGrpcStub(object):
+    """*
+    The quality verification service definition.
+    """
+
+    def __init__(self, channel):
+        """Constructor.
+
+        Args:
+            channel: A grpc.Channel.
+        """
+        self.VerifyQuality = channel.unary_stream(
+                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyQuality',
+                request_serializer=quality__verification__service__pb2.VerificationRequest.SerializeToString,
+                response_deserializer=quality__verification__service__pb2.VerificationResponse.FromString,
+                )
+        self.VerifyDataQuality = channel.stream_stream(
+                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyDataQuality',
+                request_serializer=quality__verification__service__pb2.DataVerificationRequest.SerializeToString,
+                response_deserializer=quality__verification__service__pb2.DataVerificationResponse.FromString,
+                )
+        self.VerifyStandaloneXml = channel.unary_stream(
+                '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyStandaloneXml',
+                request_serializer=quality__verification__service__pb2.StandaloneVerificationRequest.SerializeToString,
+                response_deserializer=quality__verification__service__pb2.StandaloneVerificationResponse.FromString,
+                )
+
+
+class QualityVerificationGrpcServicer(object):
+    """*
+    The quality verification service definition.
+    """
+
+    def VerifyQuality(self, request, context):
+        """*
+        Verifies the quality definied in the data dictionary.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def VerifyDataQuality(self, request_iterator, context):
+        """*
+        Experimental - Verifies the data quality definied in the data dictionary. The data is provided by the client.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def VerifyStandaloneXml(self, request, context):
+        """*
+        Verifies the quality using an XML definition instead of accessing the data dictionary.
+        This is a simplified interface with a basic response and no parallelism. Consider using
+        VerifyQuality instead.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+
+def add_QualityVerificationGrpcServicer_to_server(servicer, server):
+    rpc_method_handlers = {
+            'VerifyQuality': grpc.unary_stream_rpc_method_handler(
+                    servicer.VerifyQuality,
+                    request_deserializer=quality__verification__service__pb2.VerificationRequest.FromString,
+                    response_serializer=quality__verification__service__pb2.VerificationResponse.SerializeToString,
+            ),
+            'VerifyDataQuality': grpc.stream_stream_rpc_method_handler(
+                    servicer.VerifyDataQuality,
+                    request_deserializer=quality__verification__service__pb2.DataVerificationRequest.FromString,
+                    response_serializer=quality__verification__service__pb2.DataVerificationResponse.SerializeToString,
+            ),
+            'VerifyStandaloneXml': grpc.unary_stream_rpc_method_handler(
+                    servicer.VerifyStandaloneXml,
+                    request_deserializer=quality__verification__service__pb2.StandaloneVerificationRequest.FromString,
+                    response_serializer=quality__verification__service__pb2.StandaloneVerificationResponse.SerializeToString,
+            ),
+    }
+    generic_handler = grpc.method_handlers_generic_handler(
+            'ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc', rpc_method_handlers)
+    server.add_generic_rpc_handlers((generic_handler,))
+
+
+ # This class is part of an EXPERIMENTAL API.
+class QualityVerificationGrpc(object):
+    """*
+    The quality verification service definition.
+    """
+
+    @staticmethod
+    def VerifyQuality(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyQuality',
+            quality__verification__service__pb2.VerificationRequest.SerializeToString,
+            quality__verification__service__pb2.VerificationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def VerifyDataQuality(request_iterator,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.stream_stream(request_iterator, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyDataQuality',
+            quality__verification__service__pb2.DataVerificationRequest.SerializeToString,
+            quality__verification__service__pb2.DataVerificationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def VerifyStandaloneXml(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/ProSuite.Microservices.Definitions.QA.QualityVerificationGrpc/VerifyStandaloneXml',
+            quality__verification__service__pb2.StandaloneVerificationRequest.SerializeToString,
+            quality__verification__service__pb2.StandaloneVerificationResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `prosuite-1.2.2.0/prosuite/generated/shared_qa_pb2.py` & `prosuite-1.2.3.0/prosuite/generated/shared_qa_pb2.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/generated/shared_qa_pb2.pyi` & `prosuite-1.2.3.0/prosuite/generated/shared_qa_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/generated/shared_types_pb2.py` & `prosuite-1.2.3.0/prosuite/generated/shared_types_pb2.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/generated/shared_types_pb2.pyi` & `prosuite-1.2.3.0/prosuite/generated/shared_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/quality.py` & `prosuite-1.2.3.0/prosuite/quality.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/utils.py` & `prosuite-1.2.3.0/prosuite/utils.py`

 * *Files identical despite different names*

### Comparing `prosuite-1.2.2.0/prosuite/verification.py` & `prosuite-1.2.3.0/prosuite/verification.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,23 +42,28 @@
 
 class VerificationParameters():
     """
     Contains all parameters that can be passed to a verification. 
 
     :param tile_size: size (in meter) for testing quality conditions
     :type tile_size: int
-    :param username: the executing user
+    :param username: the executing user which will be used in issue features.
     :type username: str
+    :param desired_parallel_processing: the desired number of parallel worker processes to be used 
+    if the server allows parallel processing.
+    :type desired_parallel_processing: int
     """
 
     def __init__(self, tile_size: int = 5000, user_name: str = None) -> None:
         #:
         self.tile_size: int = tile_size
         #:
         self.user_name: str = user_name
+        #:
+        self.desired_parallel_processing = 0
 
 class InvolvedTable:
     """
     Represents a table involved in a verification issue.
 
     :param table_name: The name of the table.
     :type table_name: str
@@ -176,17 +181,20 @@
         self.specification:  Union[Specification,
                                    XmlSpecification] = specification
         self.perimeter: Union[EnvelopePerimeter,
                               EsriShapePerimeter, WkbPerimeter] = perimeter
         self.output_dir: str = output_dir
         self.tile_size: int = 5000
         self.user_name: str = None
+        self.desired_parallel_processing = 0
+        
         if (verification_params):
             self.tile_size = verification_params.tile_size
             self.user_name = verification_params.user_name
+            self.desired_parallel_processing = verification_params.desired_parallel_processing
 
 
 MAX_MESSAGE_LENGTH_MB = 1024
 
 class Service:
     from prosuite.quality import Condition
     from typing import Iterable
@@ -314,14 +322,16 @@
                 "No specification is defined. Please assign verification.specification.")
 
     def _compile_request(self, parameters: AdvancedParameters):
         req = service_util.VerificationRequest()
 
         self._configure_verification_parameter_msg(req.parameters, parameters)
         self._configure_specification_msg(req.specification, parameters.specification)
+
+        req.max_parallel_processing = parameters.desired_parallel_processing
         
         return req
     
     def _create_secure_channel(self, options) -> grpc.Channel:
         channel = grpc.secure_channel(
             f'{self.host_name}:{self.port_nr}', self.ssl_channel_credentials, options)
         try:
```

### Comparing `prosuite-1.2.2.0/prosuite.egg-info/PKG-INFO` & `prosuite-1.2.3.0/prosuite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosuite
-Version: 1.2.2.0
+Version: 1.2.3.0
 Summary: An API to configure quality assurance tests for geodata and execute quality verifications on a ProSuite Server
 Home-page: https://dirageosystems.ch/prosuite/doc/api
 Author: Dira GeoSystems
 Author-email: programmers@dirageosystems.ch
 License: MIT
 Keywords: prosuite,gis,arcgis,geodata,spatial-data,quality,quality-assurance,qa,test
 Classifier: Operating System :: OS Independent
```

### Comparing `prosuite-1.2.2.0/prosuite.egg-info/SOURCES.txt` & `prosuite-1.2.3.0/prosuite.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 prosuite/__init__.py
 prosuite/data_model.py
-prosuite/issue_demo.py
 prosuite/quality.py
 prosuite/utils.py
 prosuite/verification.py
 prosuite.egg-info/PKG-INFO
 prosuite.egg-info/SOURCES.txt
 prosuite.egg-info/dependency_links.txt
 prosuite.egg-info/requires.txt
```

### Comparing `prosuite-1.2.2.0/setup.cfg` & `prosuite-1.2.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 00000160: 726b 646f 776e 0d0a 6b65 7977 6f72 6473  rkdown..keywords
 00000170: 203d 2070 726f 7375 6974 652c 2067 6973   = prosuite, gis
 00000180: 2c20 6172 6367 6973 2c20 6765 6f64 6174  , arcgis, geodat
 00000190: 612c 2073 7061 7469 616c 2d64 6174 612c  a, spatial-data,
 000001a0: 2071 7561 6c69 7479 2c20 7175 616c 6974   quality, qualit
 000001b0: 792d 6173 7375 7261 6e63 652c 2071 612c  y-assurance, qa,
 000001c0: 2074 6573 740d 0a76 6572 7369 6f6e 203d   test..version =
-000001d0: 2031 2e32 2e32 2e30 0d0a 6c69 6365 6e73   1.2.2.0..licens
+000001d0: 2031 2e32 2e33 2e30 0d0a 6c69 6365 6e73   1.2.3.0..licens
 000001e0: 6520 3d20 4d49 540d 0a6c 6963 656e 7365  e = MIT..license
 000001f0: 5f66 696c 6573 203d 204c 4943 454e 5345  _files = LICENSE
 00000200: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
 00000210: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
 00000220: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
 00000230: 6e64 656e 740d 0a09 5072 6f67 7261 6d6d  ndent...Programm
 00000240: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language ::
```

