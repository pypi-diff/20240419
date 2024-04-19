# Comparing `tmp/openframe_criteria_set_protocol-1.4.3.tar.gz` & `tmp/openframe_criteria_set_protocol-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openframe_criteria_set_protocol-1.4.3.tar", last modified: Thu Apr 18 13:01:48 2024, max compression
+gzip compressed data, was "openframe_criteria_set_protocol-1.4.4.tar", last modified: Thu Apr 18 13:36:23 2024, max compression
```

## Comparing `openframe_criteria_set_protocol-1.4.3.tar` & `openframe_criteria_set_protocol-1.4.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:01:48.845367 openframe_criteria_set_protocol-1.4.3/
--rw-r--r--   0 andresangulo   (501) staff       (20)    19134 2023-10-19 16:06:44.000000 openframe_criteria_set_protocol-1.4.3/LICENSE
--rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-04-18 13:01:48.845180 openframe_criteria_set_protocol-1.4.3/PKG-INFO
--rw-r--r--   0 andresangulo   (501) staff       (20)     4797 2023-10-25 12:32:39.000000 openframe_criteria_set_protocol-1.4.3/README.md
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:01:48.841115 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/
--rw-r--r--   0 andresangulo   (501) staff       (20)       17 2024-01-06 19:43:41.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/__init__.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:01:48.843640 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/
--rw-r--r--   0 andresangulo   (501) staff       (20)       62 2024-01-09 10:55:39.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/__init__.py
--rw-r--r--   0 andresangulo   (501) staff       (20)      741 2024-01-05 22:18:50.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/errors.py
--rw-r--r--   0 andresangulo   (501) staff       (20)      585 2024-02-01 10:45:40.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/schemas.py
--rw-r--r--   0 andresangulo   (501) staff       (20)     3315 2024-02-01 10:44:34.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/services.py
--rw-r--r--   0 andresangulo   (501) staff       (20)     6370 2024-04-18 13:01:31.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/types.py
--rw-r--r--   0 andresangulo   (501) staff       (20)     1628 2024-03-08 19:22:46.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/utils.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:01:48.844945 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol.egg-info/
--rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-04-18 13:01:48.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol.egg-info/PKG-INFO
--rw-r--r--   0 andresangulo   (501) staff       (20)      665 2024-04-18 13:01:48.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 andresangulo   (501) staff       (20)        1 2024-04-18 13:01:48.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-04-18 13:01:48.000000 openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol.egg-info/top_level.txt
--rw-r--r--   0 andresangulo   (501) staff       (20)      671 2024-04-18 13:01:31.000000 openframe_criteria_set_protocol-1.4.3/pyproject.toml
--rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-04-18 13:01:48.845408 openframe_criteria_set_protocol-1.4.3/setup.cfg
--rw-r--r--   0 andresangulo   (501) staff       (20)      417 2024-04-18 13:01:31.000000 openframe_criteria_set_protocol-1.4.3/setup.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:01:48.843975 openframe_criteria_set_protocol-1.4.3/tests/
--rw-r--r--   0 andresangulo   (501) staff       (20)        0 2023-10-19 14:05:39.000000 openframe_criteria_set_protocol-1.4.3/tests/__init__.py
-drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:01:48.844582 openframe_criteria_set_protocol-1.4.3/tests/v1/
--rw-r--r--   0 andresangulo   (501) staff       (20)       41 2023-10-24 11:21:14.000000 openframe_criteria_set_protocol-1.4.3/tests/v1/__init__.py
--rw-r--r--   0 andresangulo   (501) staff       (20)      788 2023-10-24 11:36:52.000000 openframe_criteria_set_protocol-1.4.3/tests/v1/test_schemas.py
--rw-r--r--   0 andresangulo   (501) staff       (20)    11950 2024-01-27 14:13:37.000000 openframe_criteria_set_protocol-1.4.3/tests/v1/test_types.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:36:23.022085 openframe_criteria_set_protocol-1.4.4/
+-rw-r--r--   0 andresangulo   (501) staff       (20)    19134 2023-10-19 16:06:44.000000 openframe_criteria_set_protocol-1.4.4/LICENSE
+-rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-04-18 13:36:23.021907 openframe_criteria_set_protocol-1.4.4/PKG-INFO
+-rw-r--r--   0 andresangulo   (501) staff       (20)     4797 2023-10-25 12:32:39.000000 openframe_criteria_set_protocol-1.4.4/README.md
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:36:23.018300 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/
+-rw-r--r--   0 andresangulo   (501) staff       (20)       17 2024-01-06 19:43:41.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/__init__.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:36:23.020488 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/
+-rw-r--r--   0 andresangulo   (501) staff       (20)       62 2024-01-09 10:55:39.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/__init__.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)      741 2024-01-05 22:18:50.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/errors.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)      585 2024-02-01 10:45:40.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/schemas.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)     3315 2024-02-01 10:44:34.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/services.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)     6404 2024-04-18 13:34:54.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/types.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)     1628 2024-03-08 19:22:46.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/utils.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:36:23.021685 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol.egg-info/
+-rw-r--r--   0 andresangulo   (501) staff       (20)     5434 2024-04-18 13:36:23.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 andresangulo   (501) staff       (20)      665 2024-04-18 13:36:23.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 andresangulo   (501) staff       (20)        1 2024-04-18 13:36:23.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-04-18 13:36:23.000000 openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol.egg-info/top_level.txt
+-rw-r--r--   0 andresangulo   (501) staff       (20)      671 2024-04-18 13:36:17.000000 openframe_criteria_set_protocol-1.4.4/pyproject.toml
+-rw-r--r--   0 andresangulo   (501) staff       (20)       38 2024-04-18 13:36:23.022125 openframe_criteria_set_protocol-1.4.4/setup.cfg
+-rw-r--r--   0 andresangulo   (501) staff       (20)      417 2024-04-18 13:36:17.000000 openframe_criteria_set_protocol-1.4.4/setup.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:36:23.020726 openframe_criteria_set_protocol-1.4.4/tests/
+-rw-r--r--   0 andresangulo   (501) staff       (20)        0 2023-10-19 14:05:39.000000 openframe_criteria_set_protocol-1.4.4/tests/__init__.py
+drwxr-xr-x   0 andresangulo   (501) staff       (20)        0 2024-04-18 13:36:23.021324 openframe_criteria_set_protocol-1.4.4/tests/v1/
+-rw-r--r--   0 andresangulo   (501) staff       (20)       41 2023-10-24 11:21:14.000000 openframe_criteria_set_protocol-1.4.4/tests/v1/__init__.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)      788 2023-10-24 11:36:52.000000 openframe_criteria_set_protocol-1.4.4/tests/v1/test_schemas.py
+-rw-r--r--   0 andresangulo   (501) staff       (20)    11950 2024-01-27 14:13:37.000000 openframe_criteria_set_protocol-1.4.4/tests/v1/test_types.py
```

### Comparing `openframe_criteria_set_protocol-1.4.3/LICENSE` & `openframe_criteria_set_protocol-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.3/PKG-INFO` & `openframe_criteria_set_protocol-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openframe-criteria-set-protocol
-Version: 1.4.3
+Version: 1.4.4
 Summary: A protocol and tools for defining and working with criteria sets
 Author: Andrés Angulo <aa@openframe.org>
 Author-email: Andrés Angulo <aa@openframe.org>
 Project-URL: Homepage, https://github.com/openframe-org/criteria-set-protocol
 Project-URL: Bug Tracker, https://github.com/openframe-org/criteria-set-protocol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openframe_criteria_set_protocol-1.4.3/README.md` & `openframe_criteria_set_protocol-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/errors.py` & `openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/errors.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/schemas.py` & `openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/schemas.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/services.py` & `openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/services.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/types.py` & `openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,87 +159,87 @@
 
 
 @dataclass
 class CriteriaTree:
     version: str
     qualities: list[Quality] = field(init=False, default_factory=list)
     result: any = None
-    certificates: Optional[list[str]] = None
+    certifications: Optional[list[str]] = None
 
 
 CriteriaTreeElement = typing.Union[Quality, Criterion, TaskGroup, Task, TaskItem]
 
 
 SchemaDefinition = dict[str, typing.Any]
 
 
 @dataclass
 class SchemaDefinitions:
     parameters: Optional[SchemaDefinition] = None
     result: Optional[SchemaDefinition] = None
 
 
-CertificateDefinitionType = typing.Literal['number', 'percentage']
+CertificationDefinitionType = typing.Literal['number', 'percentage']
 
 
 @dataclass
-class CertificateDefinition(ABC):
+class CertificationDefinition(ABC):
     code: str
     type: str
     name: str
     rules: Optional[ABC] = None
     rulesText: Optional[str] = None
     icon: Optional[str] = None
     url: Optional[str] = None
     description: Optional[str] = None
 
 
 @dataclass
-class NumberBasedCertificateDefinitionRules(ABC):
+class NumberBasedCertificationDefinitionRules(ABC):
     minimum: Optional[float] = None
     maximum: Optional[float] = None
     exclusiveMinimum: Optional[float] = None
     exclusiveMaximum: Optional[float] = None
 
 
-PercentageBasedCertificateDefinitionRules = NumberBasedCertificateDefinitionRules
+PercentageBasedCertificationDefinitionRules = NumberBasedCertificationDefinitionRules
 
 
 @dataclass
-class NumberBasedCertificateDefinition(CertificateDefinition):
-    type: CertificateDefinitionType = field(init=False, default='number')
-    rules: NumberBasedCertificateDefinitionRules
+class NumberBasedCertificationDefinition(CertificationDefinition):
+    type: CertificationDefinitionType = field(init=False, default='number')
+    rules: NumberBasedCertificationDefinitionRules
 
 
 @dataclass
-class PercentageBasedCertificateDefinition(CertificateDefinition):
-    type: CertificateDefinitionType = field(init=False, default='percentage')
-    rules: PercentageBasedCertificateDefinitionRules
+class PercentageBasedCertificationDefinition(CertificationDefinition):
+    type: CertificationDefinitionType = field(init=False, default='percentage')
+    rules: PercentageBasedCertificationDefinitionRules
 
 
 @dataclass
 class Metadata:
     id: str
     version: str
     date: datetime.datetime
     name: str
     description: str
     documentation: str
     locales: Optional[list[str]] = None
     defaultLocale: Optional[str] = None
     schemas: Optional[SchemaDefinitions] = None
-    certificateDefinitions: Optional[list[CertificateDefinition]] = None
+    certificationDefinitions: Optional[list[CertificationDefinition]] = None
 
 
 @dataclass
 class DataMap:
     version: str
     elements: dict[str, any]
     result: any = None
-    certificates: Optional[list[str]] = None
+    certifications: Optional[list[str]] = None
 
 
 MetadataResponse = Metadata
 DataMapResponse = DataMap
 
 
 @dataclass
```

### Comparing `openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol/v1/utils.py` & `openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol/v1/utils.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol.egg-info/PKG-INFO` & `openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openframe-criteria-set-protocol
-Version: 1.4.3
+Version: 1.4.4
 Summary: A protocol and tools for defining and working with criteria sets
 Author: Andrés Angulo <aa@openframe.org>
 Author-email: Andrés Angulo <aa@openframe.org>
 Project-URL: Homepage, https://github.com/openframe-org/criteria-set-protocol
 Project-URL: Bug Tracker, https://github.com/openframe-org/criteria-set-protocol/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openframe_criteria_set_protocol-1.4.3/openframe_criteria_set_protocol.egg-info/SOURCES.txt` & `openframe_criteria_set_protocol-1.4.4/openframe_criteria_set_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.3/pyproject.toml` & `openframe_criteria_set_protocol-1.4.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openframe-criteria-set-protocol"
-version = "1.4.3"
+version = "1.4.4"
 authors = [
     { name="Andrés Angulo", email="aa@openframe.org" },
 ]
 description = "A protocol and tools for defining and working with criteria sets"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `openframe_criteria_set_protocol-1.4.3/tests/v1/test_schemas.py` & `openframe_criteria_set_protocol-1.4.4/tests/v1/test_schemas.py`

 * *Files identical despite different names*

### Comparing `openframe_criteria_set_protocol-1.4.3/tests/v1/test_types.py` & `openframe_criteria_set_protocol-1.4.4/tests/v1/test_types.py`

 * *Files identical despite different names*

