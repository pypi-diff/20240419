# Comparing `tmp/hasura_ndc-0.7.tar.gz` & `tmp/hasura_ndc-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hasura_ndc-0.7.tar", last modified: Mon Dec 18 05:27:00 2023, max compression
+gzip compressed data, was "hasura_ndc-0.8.tar", last modified: Fri Apr 19 20:35:02 2024, max compression
```

## Comparing `hasura_ndc-0.7.tar` & `hasura_ndc-0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tristen    (502) staff       (20)        0 2023-12-18 05:27:00.426295 hasura_ndc-0.7/
--rw-r--r--   0 tristen    (502) staff       (20)      683 2023-12-18 05:27:00.426189 hasura_ndc-0.7/PKG-INFO
--rw-r--r--   0 tristen    (502) staff       (20)      309 2023-12-17 06:14:09.000000 hasura_ndc-0.7/README.md
-drwxr-xr-x   0 tristen    (502) staff       (20)        0 2023-12-18 05:27:00.425402 hasura_ndc-0.7/hasura_ndc/
--rw-r--r--   0 tristen    (502) staff       (20)       62 2023-12-17 06:03:42.000000 hasura_ndc-0.7/hasura_ndc/__init__.py
--rw-r--r--   0 tristen    (502) staff       (20)     2096 2023-12-17 19:43:20.000000 hasura_ndc-0.7/hasura_ndc/configuration_server.py
--rw-r--r--   0 tristen    (502) staff       (20)     2545 2023-12-17 18:37:10.000000 hasura_ndc-0.7/hasura_ndc/connector.py
--rw-r--r--   0 tristen    (502) staff       (20)     1884 2023-12-17 05:44:55.000000 hasura_ndc-0.7/hasura_ndc/main.py
--rw-r--r--   0 tristen    (502) staff       (20)     6984 2023-12-18 05:17:41.000000 hasura_ndc-0.7/hasura_ndc/models.py
--rw-r--r--   0 tristen    (502) staff       (20)     3452 2023-12-17 21:50:00.000000 hasura_ndc-0.7/hasura_ndc/server.py
-drwxr-xr-x   0 tristen    (502) staff       (20)        0 2023-12-18 05:27:00.426053 hasura_ndc-0.7/hasura_ndc.egg-info/
--rw-r--r--   0 tristen    (502) staff       (20)      683 2023-12-18 05:27:00.000000 hasura_ndc-0.7/hasura_ndc.egg-info/PKG-INFO
--rw-r--r--   0 tristen    (502) staff       (20)      330 2023-12-18 05:27:00.000000 hasura_ndc-0.7/hasura_ndc.egg-info/SOURCES.txt
--rw-r--r--   0 tristen    (502) staff       (20)        1 2023-12-18 05:27:00.000000 hasura_ndc-0.7/hasura_ndc.egg-info/dependency_links.txt
--rw-r--r--   0 tristen    (502) staff       (20)      206 2023-12-18 05:27:00.000000 hasura_ndc-0.7/hasura_ndc.egg-info/requires.txt
--rw-r--r--   0 tristen    (502) staff       (20)       11 2023-12-18 05:27:00.000000 hasura_ndc-0.7/hasura_ndc.egg-info/top_level.txt
--rw-r--r--   0 tristen    (502) staff       (20)       38 2023-12-18 05:27:00.426330 hasura_ndc-0.7/setup.cfg
--rw-r--r--   0 tristen    (502) staff       (20)      844 2023-12-18 05:26:12.000000 hasura_ndc-0.7/setup.py
+drwxr-xr-x   0 tristen    (502) staff       (20)        0 2024-04-19 20:35:02.073182 hasura_ndc-0.8/
+-rw-r--r--   0 tristen    (502) staff       (20)      683 2024-04-19 20:35:02.073053 hasura_ndc-0.8/PKG-INFO
+-rw-r--r--   0 tristen    (502) staff       (20)      309 2023-12-17 06:14:09.000000 hasura_ndc-0.8/README.md
+drwxr-xr-x   0 tristen    (502) staff       (20)        0 2024-04-19 20:35:02.072088 hasura_ndc-0.8/hasura_ndc/
+-rw-r--r--   0 tristen    (502) staff       (20)       30 2024-04-19 15:18:26.000000 hasura_ndc-0.8/hasura_ndc/__init__.py
+-rw-r--r--   0 tristen    (502) staff       (20)     2247 2024-04-19 18:35:54.000000 hasura_ndc-0.8/hasura_ndc/connector.py
+-rw-r--r--   0 tristen    (502) staff       (20)     3978 2024-04-19 20:17:06.000000 hasura_ndc-0.8/hasura_ndc/instrumentation.py
+-rw-r--r--   0 tristen    (502) staff       (20)     1722 2024-04-19 20:33:51.000000 hasura_ndc-0.8/hasura_ndc/main.py
+-rw-r--r--   0 tristen    (502) staff       (20)    22361 2024-04-19 18:28:10.000000 hasura_ndc-0.8/hasura_ndc/models.py
+-rw-r--r--   0 tristen    (502) staff       (20)     3692 2024-04-19 20:34:21.000000 hasura_ndc-0.8/hasura_ndc/server.py
+drwxr-xr-x   0 tristen    (502) staff       (20)        0 2024-04-19 20:35:02.072877 hasura_ndc-0.8/hasura_ndc.egg-info/
+-rw-r--r--   0 tristen    (502) staff       (20)      683 2024-04-19 20:35:02.000000 hasura_ndc-0.8/hasura_ndc.egg-info/PKG-INFO
+-rw-r--r--   0 tristen    (502) staff       (20)      325 2024-04-19 20:35:02.000000 hasura_ndc-0.8/hasura_ndc.egg-info/SOURCES.txt
+-rw-r--r--   0 tristen    (502) staff       (20)        1 2024-04-19 20:35:02.000000 hasura_ndc-0.8/hasura_ndc.egg-info/dependency_links.txt
+-rw-r--r--   0 tristen    (502) staff       (20)      936 2024-04-19 20:35:02.000000 hasura_ndc-0.8/hasura_ndc.egg-info/requires.txt
+-rw-r--r--   0 tristen    (502) staff       (20)       11 2024-04-19 20:35:02.000000 hasura_ndc-0.8/hasura_ndc.egg-info/top_level.txt
+-rw-r--r--   0 tristen    (502) staff       (20)       38 2024-04-19 20:35:02.073225 hasura_ndc-0.8/setup.cfg
+-rw-r--r--   0 tristen    (502) staff       (20)      844 2024-04-19 20:27:55.000000 hasura_ndc-0.8/setup.py
```

### Comparing `hasura_ndc-0.7/PKG-INFO` & `hasura_ndc-0.8/hasura_ndc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hasura_ndc
-Version: 0.7
+Name: hasura-ndc
+Version: 0.8
 Summary: A Hasura Data Connector SDK
 Author: Tristen Harr
 Author-email: tristen.harr@hasura.io
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hasura_ndc-0.7/hasura_ndc/connector.py` & `hasura_ndc-0.8/hasura_ndc/connector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,67 @@
-from typing import Generic, TypeVar, Any, Dict
+from typing import Generic, TypeVar, Any
 from typing import Optional
 from abc import ABC, abstractmethod
-from hasura_ndc.models import (
+from models import (
     CapabilitiesResponse,
     SchemaResponse,
     QueryRequest,
     QueryResponse,
     ExplainResponse,
     MutationRequest,
     MutationResponse
 )
 from pydantic import BaseModel
 
-# Define type variables for RawConfiguration, Configuration, and State
-RawConfigurationType = TypeVar('RawConfigurationType', bound=BaseModel)
 ConfigurationType = TypeVar('ConfigurationType', bound=BaseModel)
 StateType = TypeVar('StateType', bound=BaseModel)
 
 
-class Connector(ABC, Generic[RawConfigurationType, ConfigurationType, StateType]):
+class Connector(ABC, Generic[ConfigurationType, StateType]):
 
-    def __init__(self, raw_configuration_type, configuration_type, state_type):
-        self.raw_configuration_type = raw_configuration_type
+    def __init__(self, configuration_type, state_type):
         self.configuration_type = configuration_type
         self.state_type = state_type
 
     @abstractmethod
-    def get_raw_configuration_schema(self) -> Dict[str, Any]:
-        pass
-
-    @abstractmethod
-    def make_empty_configuration(self) -> RawConfigurationType:
-        pass
-
-    @abstractmethod
-    async def update_configuration(self, raw_configuration: RawConfigurationType) -> RawConfigurationType:
-        pass
-
-    @abstractmethod
-    async def validate_raw_configuration(self, raw_configuration: RawConfigurationType) -> ConfigurationType:
+    async def parse_configuration(self, configuration_dir: str) -> ConfigurationType:
         pass
 
     @abstractmethod
     async def try_init_state(self, configuration: ConfigurationType, metrics: Any) -> StateType:
         pass
 
     @abstractmethod
-    async def fetch_metrics(self, configuration: ConfigurationType, state: StateType) -> Optional[None]:
+    async def fetch_metrics(self, configuration: ConfigurationType, state: StateType) -> Optional[Any]:
         pass
 
     @abstractmethod
-    async def health_check(self, configuration: ConfigurationType, state: StateType) -> Optional[None]:
+    async def health_check(self, configuration: ConfigurationType, state: StateType) -> Optional[Any]:
         pass
 
     @abstractmethod
     def get_capabilities(self, configuration: ConfigurationType) -> CapabilitiesResponse:
         pass
 
     @abstractmethod
     async def get_schema(self, configuration: ConfigurationType) -> SchemaResponse:
         pass
 
     @abstractmethod
-    async def explain(self, configuration: ConfigurationType, state: StateType,
-                      request: QueryRequest) -> ExplainResponse:
+    async def query_explain(self,
+                            configuration: ConfigurationType,
+                            state: StateType,
+                            request: QueryRequest) -> ExplainResponse:
+        pass
+
+    @abstractmethod
+    async def mutation_explain(self,
+                               configuration: ConfigurationType,
+                               state: StateType,
+                               request: MutationRequest) -> ExplainResponse:
         pass
 
     @abstractmethod
     async def mutation(self, configuration: ConfigurationType, state: StateType,
                        request: MutationRequest) -> MutationResponse:
         pass
```

### Comparing `hasura_ndc-0.7/hasura_ndc/server.py` & `hasura_ndc-0.8/hasura_ndc/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from fastapi import FastAPI, status, Request, Response, Depends
 from fastapi.security import APIKeyHeader
 from fastapi.exceptions import HTTPException
 from pydantic import BaseModel
 from typing import Any
 import uvicorn
-import json
-from hasura_ndc.connector import Connector, RawConfigurationType, ConfigurationType, StateType
-from hasura_ndc.models import (CapabilitiesResponse, SchemaResponse, QueryResponse, ExplainResponse, MutationResponse,
-                               QueryRequest, MutationRequest)
+from hasura_ndc.connector import Connector, ConfigurationType, StateType
+from models import (CapabilitiesResponse, SchemaResponse, QueryResponse, ExplainResponse, MutationResponse,
+                    QueryRequest, MutationRequest)
+from opentelemetry import trace
+import hasura_ndc.instrumentation as instrumentation
+
+tracer = trace.get_tracer("ndc-sdk-python.server")
 
 
 class ServerOptions(BaseModel):
     configuration: str
     port: int
     service_token_secret: str
-    oltp_endpoint: str
-    service_name: str
     log_level: str
     pretty_print_logs: str
 
 
-async def start_server(connector: Connector[RawConfigurationType, ConfigurationType, StateType],
+async def start_server(connector: Connector[ConfigurationType, StateType],
                        options: ServerOptions):
     api_key_header = APIKeyHeader(name="Authorization", auto_error=False)
-    with open(options.configuration, "r") as f:
-        raw_configuration = connector.raw_configuration_type(**json.load(f))
-    configuration = await connector.validate_raw_configuration(raw_configuration)
+    configuration = await connector.parse_configuration(configuration_dir=options.configuration)
     metrics = {}
     state = await connector.try_init_state(configuration, metrics)
 
     async def get_api_key(header: str = Depends(api_key_header)):
         match_value = f"{options.service_token_secret}" if options.service_token_secret else None
         if header == match_value:
             return header
@@ -55,28 +54,36 @@
 
     @app.get("/metrics")
     async def fetch_metrics() -> Any:
         return await connector.fetch_metrics(configuration, state)
 
     @app.get("/schema")
     async def get_schema() -> SchemaResponse:
-        return await connector.get_schema(configuration)
+        return instrumentation.with_active_span(
+            tracer,
+            "getSchema",
+            lambda span: connector.get_schema(configuration)
+        )
 
     @app.post("/query")
     async def execute_query(request: Request) -> QueryResponse:
         return await connector.query(configuration, state, QueryRequest(**await request.json()))
 
-    @app.post("/explain")
-    async def explain_query(request: Request) -> ExplainResponse:
-        return await connector.explain(configuration, state, QueryRequest(**await request.json()))
+    @app.post("/query/explain")
+    async def query_explain(request: Request) -> ExplainResponse:
+        return await connector.query_explain(configuration, state, QueryRequest(**await request.json()))
 
     @app.post("/mutation")
     async def execute_mutation(request: Request) -> MutationResponse:
         return await connector.mutation(configuration, state, MutationRequest(**await request.json()))
 
+    @app.post("/mutation/explain")
+    async def mutation_explain(request: Request) -> ExplainResponse:
+        return await connector.mutation_explain(configuration, state, MutationRequest(**await request.json()))
+
     @app.exception_handler(Exception)
     async def http_exception_handler(_: Request, e: Exception):
         return Response(
             status_code=status.HTTP_400_BAD_REQUEST,
             content={
                 "message": str(e),
                 "details": {}
```

### Comparing `hasura_ndc-0.7/hasura_ndc.egg-info/PKG-INFO` & `hasura_ndc-0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hasura-ndc
-Version: 0.7
+Name: hasura_ndc
+Version: 0.8
 Summary: A Hasura Data Connector SDK
 Author: Tristen Harr
 Author-email: tristen.harr@hasura.io
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hasura_ndc-0.7/setup.py` & `hasura_ndc-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='hasura_ndc',
-    version='0.07',
+    version='0.08',
     packages=find_packages(),
     install_requires=[
         # This line reads the requirements from your `requirements.txt`
         line.strip() for line in open('requirements.txt', 'r').readlines()
     ],
     author='Tristen Harr',
     author_email='tristen.harr@hasura.io',
```

