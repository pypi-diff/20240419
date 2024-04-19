# Comparing `tmp/knowledgeai_client-0.4.3.tar.gz` & `tmp/knowledgeai_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledgeai_client-0.4.3.tar", max compression
+gzip compressed data, was "knowledgeai_client-0.5.0.tar", max compression
```

## Comparing `knowledgeai_client-0.4.3.tar` & `knowledgeai_client-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1080 2024-02-11 14:39:56.544899 knowledgeai_client-0.4.3/LICENSE
--rw-r--r--   0        0        0     7385 2024-03-28 10:42:38.426177 knowledgeai_client-0.4.3/README.md
--rw-r--r--   0        0        0        0 2024-02-11 11:57:58.557100 knowledgeai_client-0.4.3/knowledgeai/__init__.py
--rw-r--r--   0        0        0      392 2024-03-28 09:35:58.450495 knowledgeai_client-0.4.3/knowledgeai/client/__init__.py
--rw-r--r--   0        0        0     5030 2024-02-11 11:55:35.829638 knowledgeai_client-0.4.3/knowledgeai/client/admin.py
--rw-r--r--   0        0        0    12897 2024-02-11 13:24:03.012391 knowledgeai_client-0.4.3/knowledgeai/client/client.py
--rw-r--r--   0        0        0     2039 2024-02-11 13:27:19.153360 knowledgeai_client-0.4.3/knowledgeai/client/schema.py
--rw-r--r--   0        0        0     4465 2024-03-28 09:42:26.199926 knowledgeai_client-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     8169 1970-01-01 00:00:00.000000 knowledgeai_client-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-02-12 12:45:05.581822 knowledgeai_client-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7385 2024-04-19 14:53:31.500483 knowledgeai_client-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-12 12:45:05.582349 knowledgeai_client-0.5.0/knowledgeai/__init__.py
+-rw-r--r--   0        0        0      392 2024-04-19 14:53:31.499925 knowledgeai_client-0.5.0/knowledgeai/client/__init__.py
+-rw-r--r--   0        0        0     5050 2024-04-19 14:49:37.775006 knowledgeai_client-0.5.0/knowledgeai/client/admin.py
+-rw-r--r--   0        0        0    12964 2024-04-19 15:20:04.932119 knowledgeai_client-0.5.0/knowledgeai/client/client.py
+-rw-r--r--   0        0        0     2044 2024-04-19 15:19:14.290191 knowledgeai_client-0.5.0/knowledgeai/client/schema.py
+-rw-r--r--   0        0        0     4465 2024-04-19 14:59:02.915726 knowledgeai_client-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8212 1970-01-01 00:00:00.000000 knowledgeai_client-0.5.0/PKG-INFO
```

### Comparing `knowledgeai_client-0.4.3/LICENSE` & `knowledgeai_client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `knowledgeai_client-0.4.3/README.md` & `knowledgeai_client-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # Avvia Intelligence - KnowledgeAI Python Client
 
-Version: 0.4.3, (c) 2024 Arvato Systems
+Version: 0.5.0, (c) 2024 Arvato Systems
 
 This library is designed to provide easy access to the KnowledgeAI backend service. It enables users to manage projects, upload documents, and perform various tasks programmatically. The client offers an intuitive interface for seamless integration into Python applications.
 
 ## Installation
 ```bash
 pip install knowledgeai-client
 ```
```

### Comparing `knowledgeai_client-0.4.3/knowledgeai/client/admin.py` & `knowledgeai_client-0.5.0/knowledgeai/client/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             >>> for user in users:
             ...     print(user.name)
         """
 
         url: str = self.url + "/admin/user/"
         headers: dict[str, str] = {
             "accept": "application/json",
-            "x-apikey": self.api_key,
+            "Authorization": self.api_key,
         }
         response: Response = requests.get(url, headers=headers, timeout=self.timeout)
         response.raise_for_status()
         return [User(**user) for user in response.json()]
 
     def create_user(self, user: User) -> User:
         """
@@ -80,15 +80,15 @@
             ... )
             >>> client.create_user(user)
         """
 
         url: str = self.url + "/admin/user"
         headers: dict[str, str] = {
             "accept": "application/json",
-            "x-apikey": self.api_key,
+            "Authorization": self.api_key,
             "Content-Type": "application/x-www-form-urlencoded",
         }
         data: dict[str, Any] = {
             "name": user.name,
             "company": user.company,
             "language": user.language.value,
             "plan": user.plan.value,
@@ -119,15 +119,15 @@
             >>> user = client.get_user("put key here")
             >>> print(user.name)
         """
 
         url: str = self.url + "/admin/user/" + api_key
         headers: dict[str, str] = {
             "accept": "application/json",
-            "x-apikey": self.api_key,
+            "Authorization": self.api_key,
         }
         response: Response = requests.get(url, headers=headers, timeout=self.timeout)
         response.raise_for_status()
         return User(**response.json())
 
     def update_user(self, user: User) -> User:
         """
@@ -147,15 +147,15 @@
             >>> user.company = "new company name"
             >>> client.update_user(user)
         """
 
         url: str = self.url + "/admin/user/" + user.api_key
         headers: dict[str, str] = {
             "accept": "application/json",
-            "x-apikey": self.api_key,
+            "Authorization": self.api_key,
             "Content-Type": "application/x-www-form-urlencoded",
         }
         data = {
             "api_key": user.api_key,
             "name": user.name,
             "company": user.company,
             "language": user.language.value,
```

### Comparing `knowledgeai_client-0.4.3/knowledgeai/client/client.py` & `knowledgeai_client-0.5.0/knowledgeai/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         data: Optional[Any] = None,
         params: Optional[Any] = None,
         headers: Optional[dict[str, str]] = None,
         form: bool = True,
     ) -> Response:
         headers_default: dict[str, str] = {
             "accept": "application/json",
-            "x-apikey": self.api_key,
+            "Authorization": self.api_key,
         }
 
         if form:
             headers_default["Content-Type"] = "application/x-www-form-urlencoded"
 
         with httpx.Client(
             limits=limits,
@@ -125,15 +125,15 @@
                 )
         """
         url: str = "/index/document"
         filesp = tqdm(files)
 
         headers: dict[str, str] = {
             "accept": "application/json",
-            "x-apikey": self.api_key,
+            "Authorization": self.api_key,
         }
 
         with httpx.Client(
             limits=limits, base_url=self.url, headers=headers, timeout=self.timeout
         ) as client:
             for file in filesp:
                 log.debug("Uploading file: %s", file)
@@ -394,15 +394,19 @@
 
         Example:
             >>> references = client.retrieve(1, "What is the capital of Germany?")
             >>> for reference in references:
             ...     print(reference.content)
         """
         url: str = "/index/retrieve"
-        data = {"project_id": project_id, "query": query, "type": retrieval_type.value}
+        data = {
+            "project_id": project_id,
+            "query": query,
+            "retriever_type": retrieval_type.value,
+        }
 
         response = self._api_call(HttpMethod.POST, url, data=data)
         content = json.loads(response.content)
 
         references: List[RetrievedDocument] = []
         for reference in content["documents"]:
             references.append(RetrievedDocument(**reference))
```

### Comparing `knowledgeai_client-0.4.3/knowledgeai/client/schema.py` & `knowledgeai_client-0.5.0/knowledgeai/client/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import StrEnum
-from typing import List
+from typing import Any, List
 
 import iso639
 from pydantic import BaseModel, Field
 
 
 class HttpMethod(StrEnum):
     GET = "GET"
@@ -87,8 +87,8 @@
     default = "default"
     multiquery = "multiquery"
     compression = "compression"
 
 
 class RetrievedDocument(BaseModel):
     content: str
-    metadata: dict[str, str]
+    metadata: dict[str, Any]
```

### Comparing `knowledgeai_client-0.4.3/pyproject.toml` & `knowledgeai_client-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,40 +9,40 @@
     "avvia intelligence",
     "knowledgeai",
 ]
 license = "MIT"
 name = "knowledgeai-client"
 packages = [{ include = "knowledgeai", from = "." }]
 readme = "README.md"
-version = "0.4.3"
+version = "0.5.0"
 
 [tool.poetry.dependencies]
 python = ">=3.11"
 
-httpx         = "0.26.0"
-pydantic      = "2.6.1"
+httpx         = "0.27.0"
+pydantic      = "2.7.0"
+pydantic-settings = "2.2.1"
 python-iso639 = "2024.2.7"
 python-magic  = "0.4.27"
-tqdm          = "4.66.1"
+tqdm          = "4.66.2"
 
 
 [tool.poetry.group.dev.dependencies]
 detect-secrets    = "1.4.0"
-mypy              = "1.8.0"
-pre-commit        = "3.6.0"
-pydantic-settings = "2.1.0"
-ruff              = "0.2.1"
-types-requests    = "2.31.0.20240125"
-types-tqdm        = "4.66.0.20240106"
+mypy              = "1.9.0"
+pre-commit        = "3.7.0"
+ruff              = "0.4.1"
+types-requests    = "2.31.0.20240406"
+types-tqdm        = "4.66.0.20240417"
 
 
 [tool.poetry.group.test.dependencies]
 codecov       = "2.1.13"
-coverage      = "7.4.1"
-pytest        = "8.0.0"
+coverage      = "7.4.4"
+pytest        = "8.1.1"
 pytest-dotenv = "0.5.2"
 
 [tool.pytest.ini_options]
 cache_dir = ".cache/pytest"
 testpaths = ["tests"]
```

### Comparing `knowledgeai_client-0.4.3/PKG-INFO` & `knowledgeai_client-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: knowledgeai-client
-Version: 0.4.3
+Version: 0.5.0
 Summary: A python client for the Avvia Intelligence - Knowledge AI Rest API
 Home-page: https://github.com/arvato-systems-aila-solutions/KnowledgeAI-Python-Client
 License: MIT
 Keywords: AI,Knowledge Retrieval,arvato systems,avvia intelligence,knowledgeai
 Author: Arvato Systems
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: httpx (==0.26.0)
-Requires-Dist: pydantic (==2.6.1)
+Requires-Dist: httpx (==0.27.0)
+Requires-Dist: pydantic (==2.7.0)
+Requires-Dist: pydantic-settings (==2.2.1)
 Requires-Dist: python-iso639 (==2024.2.7)
 Requires-Dist: python-magic (==0.4.27)
-Requires-Dist: tqdm (==4.66.1)
+Requires-Dist: tqdm (==4.66.2)
 Description-Content-Type: text/markdown
 
 
 # Avvia Intelligence - KnowledgeAI Python Client
 
-Version: 0.4.3, (c) 2024 Arvato Systems
+Version: 0.5.0, (c) 2024 Arvato Systems
 
 This library is designed to provide easy access to the KnowledgeAI backend service. It enables users to manage projects, upload documents, and perform various tasks programmatically. The client offers an intuitive interface for seamless integration into Python applications.
 
 ## Installation
 ```bash
 pip install knowledgeai-client
 ```
```

