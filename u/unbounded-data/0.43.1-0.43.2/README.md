# Comparing `tmp/unbounded_data-0.43.1.tar.gz` & `tmp/unbounded_data-0.43.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbounded_data-0.43.1.tar", max compression
+gzip compressed data, was "unbounded_data-0.43.2.tar", max compression
```

## Comparing `unbounded_data-0.43.1.tar` & `unbounded_data-0.43.2.tar`

### file list

```diff
@@ -1,14 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-12-28 12:04:50.664044 unbounded_data-0.43.1/pyproject.toml
--rw-r--r--   0        0        0       30 2023-12-28 12:04:49.102932 unbounded_data-0.43.1/unbounded_data/__init__.py
--rw-r--r--   0        0        0       89 2023-12-28 12:04:49.102932 unbounded_data-0.43.1/unbounded_data/datasets/__init__.py
--rw-r--r--   0        0        0    29809 2023-12-28 12:04:49.102932 unbounded_data-0.43.1/unbounded_data/datasets/client.py
--rw-r--r--   0        0        0     1168 2023-12-28 12:04:49.102932 unbounded_data-0.43.1/unbounded_data/ethereum/__init__.py
--rw-r--r--   0        0        0    11539 2023-12-28 12:04:49.102932 unbounded_data-0.43.1/unbounded_data/ethereum/chainlink.py
--rw-r--r--   0        0        0     9481 2023-12-28 12:04:49.102932 unbounded_data-0.43.1/unbounded_data/ethereum/client.py
--rw-r--r--   0        0        0     7672 2023-12-28 12:04:49.102932 unbounded_data-0.43.1/unbounded_data/ethereum/summaries.py
--rw-r--r--   0        0        0    10513 2023-12-28 12:04:49.102932 unbounded_data-0.43.1/unbounded_data/ethereum/tokens.py
--rw-r--r--   0        0        0     8297 2023-12-28 12:04:49.103932 unbounded_data-0.43.1/unbounded_data/ethereum/transactions.py
--rw-r--r--   0        0        0    19292 2023-12-28 12:04:49.103932 unbounded_data-0.43.1/unbounded_data/ethereum/transfers.py
--rw-r--r--   0        0        0     3831 2023-12-28 12:04:49.103932 unbounded_data-0.43.1/unbounded_data/ethereum/utilities.py
--rw-r--r--   0        0        0    14948 2023-12-28 12:04:49.103932 unbounded_data-0.43.1/unbounded_data/high_level_api.py
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 unbounded_data-0.43.1/PKG-INFO
+-rw-r--r--   0        0        0     1047 2024-04-19 14:36:01.426631 unbounded_data-0.43.2/pyproject.toml
+-rw-r--r--   0        0        0       30 2024-04-19 14:35:59.806491 unbounded_data-0.43.2/unbounded_data/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-19 14:35:59.806491 unbounded_data-0.43.2/unbounded_data/datasets/__init__.py
+-rw-r--r--   0        0        0    28321 2024-04-19 14:35:59.807491 unbounded_data-0.43.2/unbounded_data/datasets/client.py
+-rw-r--r--   0        0        0    13209 2024-04-19 14:35:59.807491 unbounded_data-0.43.2/unbounded_data/high_level_api.py
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 unbounded_data-0.43.2/PKG-INFO
```

### Comparing `unbounded_data-0.43.1/pyproject.toml` & `unbounded_data-0.43.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "unbounded-data"
-version = "0.43.1"
+version = "0.43.2"
 authors = ["Unbounded Network"]
 description = "The Unbounded Network Data Python interface"
 
 [tool.poetry.dependencies]
   "python" = "^3.10"
   "pandas" =  "^1.4.3"
   "gql" = "^3.4.0"
   "python-benedict" = "^0.25.2"
-  "aiohttp" = "^3.8.3"
+  "requests" = "^2.31.0"
   "openpyxl" = {version="^3.0.10", optional=true}
   "pyarrow" = {version="^14.0.0", optional=true}
   
 [tool.poetry.dev-dependencies]
   "pytest" = "^7.1.2"
   "pytest-mock" = "^3.8.2"
-  "pytest-aiohttp" = "^1.0.4"
   "pytest-asyncio" = "^0.19.0"
   "python-semantic-release" = "^8.7.0"
   "pylint" = "^2.14.5"
   "openpyxl" = "^3.0.10"
   "pyarrow" = "^14.0.0"
-  "twine" = "^3.8.0"
+  "twine" = "^4.0.2"
 
 [tool.semantic_release]
   version_toml = [
       "pyproject.toml:tool.poetry.version"
   ]
   commit_message = "[skip ci] version bump"
   build_command = "poetry build"
```

### Comparing `unbounded_data-0.43.1/unbounded_data/datasets/client.py` & `unbounded_data-0.43.2/unbounded_data/datasets/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 import os
 import io
 import json
 import logging
 from dateutil import parser
-import aiohttp
-from aiohttp import ClientResponseError, ContentTypeError
+import requests
+from requests import Response
 import pandas as pd
 
+DEFAULT_TIMEOUT = 30
 DEFAULT_ENDPOINT = "https://unbounded.network/api/v1"
 
 file_access_audit_func = None
 
 
+class APIError(Exception):
+    "Error raised by Client in case of unexpected server response"
+
+    def __init__(self, status=-1, message=None):
+        super().__init__(': '.join([x for x in [status if status > 0 else None, message] if x]))
+        self.status = status
+        self.message = message
+
+
 class FileAccessAudit:
     "this class is used for internal file audit"
 
     def __init__(self, dataset_id, dataset_version, file_id, file_version, operation):
         self.dataset_id = dataset_id
         self.dataset_version = dataset_version
         self.file_id = file_id
@@ -32,27 +42,14 @@
         }
 
 
 class Client:
     """
     This client class is used to send http requests
     to query datasets from unbounded network.
-
-    Note: In order to send requests to the endpoint
-    a Client session must be created using create_session()
-    method.
-
-    Note: Close the session when done sending requests to
-    the endpoint. Otherwise an 'Unclosed Session` warning
-    will be issued.
-
-    Note: If the Client session was accidentally closed
-    too early, it can always be re-opened using create_session()
-    method. Then all objects that stored an instance of a Client
-    will be able to send requests to the endpoint.
     """
 
     def __init__(
         self,
         api_key: str = None,
         timeout: float = 30,
         endpoint_url: str = DEFAULT_ENDPOINT,
@@ -65,33 +62,16 @@
 
         if endpoint_url == DEFAULT_ENDPOINT and os.getenv("UNBOUNDED_DATA_ENDPOINT"):
             endpoint_url = os.getenv("UNBOUNDED_DATA_ENDPOINT")
 
         self.endpoint_url = endpoint_url
         self.api_key = api_key
         self.timeout = timeout
-        self.session = None
-
-    def create_session(self):
-        """
-        creates an aiohttp client session
-        """
-        self.session = aiohttp.ClientSession(
-            timeout=aiohttp.ClientTimeout(self.timeout),
-            raise_for_status=False,
-        )
-
-    async def close_session(self):
-        """
-        closes aiohttp client session if it is open
-        """
-        if self.session:
-            await self.session.close()
 
-    async def list_datasets(
+    def list_datasets(
         self,
         search_string: str = "",
         visibility: str = "private",
         with_files: str = "true",
     ):
         """
         description:    the function is used to query all datasets
@@ -112,26 +92,26 @@
         datasets_url = self.endpoint_url + "/datasets"
         parameters_dict = {
             "search": search_string,
             "visibility": visibility,
             "with_files": with_files,
         }
 
-        client_response = await self.do_request(
+        client_response = self.do_request(
             "GET", datasets_url, params=parameters_dict
         )
-        response_json = await self.response_to_json(client_response)
+        response_json = self.response_to_json(client_response)
         ds_list = pd.json_normalize(response_json["data"], sep="_").to_dict("records")
         ds_entries = []
         for dataset in ds_list:
             ds_entries.append(Dataset(dataset, self))
 
         return ds_entries
 
-    async def get_dataset(self, *, uuid: str = None, name: str = None):
+    def get_dataset(self, *, uuid: str = None, name: str = None):
         """
         description:    the function is used to query datasets
                         by id, name
 
         arguments:      uuid - dataset id
                         name - dataset name
                         dataset_version (optional) - if provided, used to fetch a specific dataset version
@@ -140,24 +120,24 @@
         """
 
         if uuid and name:
             raise ValueError("Only one query parameter can be provided at a time")
 
         if uuid:
             dataset_url = self.endpoint_url + "/datasets/" + uuid
-            client_response = await self.do_request("GET", dataset_url)
-            response_json = await self.response_to_json(client_response)
+            client_response = self.do_request("GET", dataset_url)
+            response_json = self.response_to_json(client_response)
             dataset = pd.json_normalize(response_json["data"], sep="_")
             return Dataset(dataset.iloc[0].to_dict(), self)
         if name:
-            datasets = await self.list_datasets(
+            datasets = self.list_datasets(
                 search_string=name, visibility="private"
             )
             if len(datasets) == 0:
-                datasets = await self.list_datasets(
+                datasets = self.list_datasets(
                     search_string=name, visibility="public"
                 )
                 if len(datasets) == 0:
                     return None
 
             matched_datasets = []
             min_timestamp = None
@@ -180,15 +160,15 @@
             if len(matched_datasets) == 0:
                 return None
 
             return matched_datasets[min_index]
 
         raise ValueError("None of the query parameters provided")
 
-    async def create_dataset(self, name: str, description: str, public: bool = False):
+    def create_dataset(self, name: str, description: str, public: bool = False):
         """
         description:    the function is used to create a new dataset
                         with given name, description and visibility
 
         arguments:      name - new dataset name
                         description - new dataset description
                         public - new dataset visibility
@@ -199,59 +179,57 @@
             raise ValueError("dataset must have name")
 
         creation_url = self.endpoint_url + "/datasets"
         request_body = json.dumps(
             {"name": name, "description": description, "public": public}
         )
 
-        client_response = await self.do_request(
+        client_response = self.do_request(
             "POST",
             creation_url,
             headers={"content-type": "application/json"},
             data=request_body,
         )
-        response_json = await self.response_to_json(client_response)
+        response_json = self.response_to_json(client_response)
         dataset = pd.json_normalize(response_json["data"], sep="_")
         return Dataset(dataset.iloc[0].to_dict(), self)
 
-    async def delete_dataset(self, uuid: str):
+    def delete_dataset(self, uuid: str):
         """
         description:    the function is used to delete
                         a dataset with given uuid
 
         arguments:      uuid - the id of the dataset to be deleted
         """
         if uuid is None:
             raise ValueError("invalid dataset uuid")
         delete_url = self.endpoint_url + "/datasets/" + uuid
-        return await self.do_request("DELETE", delete_url)
+        return self.do_request("DELETE", delete_url)
 
-    async def response_to_json(self, response: aiohttp.ClientResponse):
+    def response_to_json(self, response: Response):
         """
         converts aiohttp client response into json
         """
-        return await response.json()
+        return response.json()
 
-    async def response_to_text(self, response: aiohttp.ClientResponse):
+    def response_to_text(self, response: Response):
         """
         converts aiohttp client response into text
         """
-        return await response.text()
+        return response.text
 
-    async def response_to_bytes_buffer(self, response: aiohttp.ClientResponse):
+    def response_to_bytes_buffer(self, response: Response):
         """
         converts aiohttp client response into bytes buffer
         """
-        buffer = io.BytesIO()
-        async for chunk in response.content.iter_chunked(1024):
-            buffer.write(chunk)
+        buffer = io.BytesIO(response.content)
         buffer.seek(0)
         return buffer
 
-    async def do_request(
+    def do_request(
         self,
         method: str,
         url: str,
         *,
         params: dict = None,
         headers: dict = None,
         data: str = None,
@@ -263,63 +241,58 @@
 
         arguments:      method - http request method
                         url - unbounded network endpoint url
                         parameters - request parameters
 
         returns:        aiohttp client response
         """
-        if not self.session or self.session.closed:
-            self.create_session()
-
         if not params:
             params = {}
 
         if not headers:
             headers = {}
 
         if method not in ("GET", "POST", "PUT", "PATCH", "DELETE"):
             raise ValueError(f"Unknown http request method: {method}")
 
         if self.api_key:
             headers["X-API-Key"] = self.api_key
 
         response = None
         if method == "GET":
-            response = await self.session.get(url, params=params, headers=headers)
+            response = requests.get(url, params=params, headers=headers, timeout=DEFAULT_TIMEOUT)
         if method == "POST":
-            response = await self.session.post(
-                url, data=data, params=params, headers=headers
+            response = requests.post(
+                url, data=data, params=params, headers=headers, timeout=DEFAULT_TIMEOUT
             )
         if method == "PUT":
-            response = await self.session.put(
-                url, data=data, params=params, headers=headers
+            response = requests.put(
+                url, data=data, params=params, headers=headers, timeout=DEFAULT_TIMEOUT
             )
         if method == "PATCH":
-            response = await self.session.patch(
-                url, data=data, params=params, headers=headers
+            response = requests.patch(
+                url, data=data, params=params, headers=headers, timeout=DEFAULT_TIMEOUT
             )
         if method == "DELETE":
-            response = await self.session.delete(url, params=params, headers=headers)
+            response = requests.delete(url, params=params, headers=headers, timeout=DEFAULT_TIMEOUT)
 
-        if response.status not in (200, 204):
+        if response.status_code not in (200, 204):
             try:
-                error = (await response.json())["error"]
-            except (KeyError, ContentTypeError):
-                error = await response.text()
-            raise ClientResponseError(
-                response.request_info,
-                response.history,
-                status=response.status,
+                error = response.json()["error"]
+            except KeyError:
+                error = response.text
+            raise APIError(
+                status=response.status_code,
                 message=error,
             )
 
         return response
 
     def __repr__(self):
-        return f"Client(endpoint_url: {self.endpoint_url}, session_closed: {self.session.closed})"
+        return f"Client(endpoint_url: {self.endpoint_url})"
 
 
 class Dataset:
     """
     This class is used to represent a dataset from Unbounded Network.
     Note: it contains all of the versions and files. To work with a
     specific version of the dataset, use latest() or version() functions
@@ -339,75 +312,75 @@
         }
         self.public = dataset_desc["public"]
         self.thumbnail = (
             dataset_desc["thumbnail"] if "thumbnail" in dataset_desc else None
         )
         self.created_at = dataset_desc["created_at"]
         self.updated_at = dataset_desc["updated_at"]
-        self.owner_id = dataset_desc["owner_id"]
-        self.owner_username = dataset_desc["owner_username"]
+        self.owner_id = dataset_desc.get("owner_id")
+        self.owner_username = dataset_desc.get("owner_username")
         self.client = client
 
-    async def get_thumbnail(self):
+    def get_thumbnail(self):
         """
         description:    the function is used to retrieve
                         a thumbnail image of the dataset
 
         returns:        thumbnail image bytes
         """
         thumbnail_url = (
             self.client.endpoint_url + "/datasets/" + self.uuid + "/thumbnail"
         )
-        resp = await self.client.do_request("GET", thumbnail_url)
-        buffer = await self.client.response_to_bytes_buffer(resp)
+        resp = self.client.do_request("GET", thumbnail_url)
+        buffer = self.client.response_to_bytes_buffer(resp)
         return buffer.read()
 
-    async def upload_thumbnail(self, image: bytes, image_name: str, content_type: str):
+    def upload_thumbnail(self, image: bytes, image_name: str, content_type: str):
         """
         description:    the function is used to upload a thumbnail
                         image to the dataset
 
         arguments:      image - image bytes
                         file_name - name of the image file
                         content_type - type of image
         """
         if not isinstance(image, bytes):
-            return NotImplemented
+            raise NotImplementedError('image must be bytes()')
 
         thumbnail_url = (
             self.client.endpoint_url + "/datasets/" + self.uuid + "/thumbnail/upload"
         )
-        resp = await self.client.do_request("POST", thumbnail_url)
-        upload_info = await self.client.response_to_json(resp)
+        resp = self.client.do_request("POST", thumbnail_url)
+        upload_info = self.client.response_to_json(resp)
 
-        resp = await self.client.do_request(
+        resp = self.client.do_request(
             "PUT",
             upload_info["url"],
             headers={"content-type": content_type},
             data=image,
         )
 
         upload_complete_url = (
             self.client.endpoint_url
             + "/datasets/"
             + self.uuid
             + "/thumbnail/upload-complete"
         )
         image_info_json = json.dumps({"id": upload_info["id"], "filename": image_name})
 
-        await self.client.do_request(
+        self.client.do_request(
             "POST",
             upload_complete_url,
             headers={"content-type": "application/json"},
             data=image_info_json,
         )
-        dataset = await self.client.get_dataset(uuid=self.uuid)
+        dataset = self.client.get_dataset(uuid=self.uuid)
         self.__update_dataset(dataset)
 
-    async def update_dataset_info(self, name: str = None, description: str = None):
+    def update_dataset_info(self, name: str = None, description: str = None):
         """
         description:    the function is used to update
                         dataset name or description or both.
                         Note: at least one must be defined
 
 
         arguments:      name - new dataset name
@@ -424,47 +397,47 @@
 
         if name is not None:
             data["name"] = name
 
         if description is not None:
             data["description"] = description
 
-        await self.client.do_request(
+        self.client.do_request(
             "PATCH",
             update_url,
             headers={"content-type": "application/json"},
             data=json.dumps(data),
         )
-        dataset = await self.client.get_dataset(uuid=self.uuid)
+        dataset = self.client.get_dataset(uuid=self.uuid)
         self.__update_dataset(dataset)
 
-    async def change_visibility(self, *, public: bool):
+    def change_visibility(self, *, public: bool):
         """
         description:    the function is used to change the
                         visibility of the dataset
 
 
         arguments:      public - boolean that indicates if
                         dataset should be public or not. If
                         dataset visibility is the same as the
                         argument passed, nothing is done.
         """
         if self.public == public:
             return
 
         update_url = self.client.endpoint_url + "/datasets/" + self.uuid
-        await self.client.do_request(
+        self.client.do_request(
             "PATCH",
             update_url,
             headers={"content-type": "application/json"},
             data=json.dumps({"public": public}),
         )
         self.public = public
 
-    async def delete_file(self, file_name: str):
+    def delete_file(self, file_name: str):
         """
         description:    the function is used to delete
                         a new file from the dataset
 
         arguments:      file_name - name of the file to
                         be deleted
         """
@@ -475,101 +448,101 @@
                     delete_url = (
                         self.client.endpoint_url
                         + "/datasets/"
                         + self.uuid
                         + "/files/"
                         + file_uuid
                     )
-                    await self.client.do_request("DELETE", delete_url)
-                    dataset = await self.client.get_dataset(uuid=self.uuid)
+                    self.client.do_request("DELETE", delete_url)
+                    dataset = self.client.get_dataset(uuid=self.uuid)
                     self.__update_dataset(dataset)
                     return
         raise RuntimeError("Dataset does not have any files")
 
-    async def create_raw_file(
+    def create_raw_file(
         self, data_buffer: io.BytesIO, file_name: str, content_type: str
     ):
         """
         description:    the function is used to create
                         a new file in the dataset
 
         arguments:      data_buffer - buffer containing the data
                         file_name - name of the new file
                         content_type - type of the new file
         """
 
         create_file_url = (
             self.client.endpoint_url + "/datasets/" + self.uuid + "/files/upload"
         )
-        resp = await self.client.do_request("POST", create_file_url)
-        upload_info = await self.client.response_to_json(resp)
+        resp = self.client.do_request("POST", create_file_url)
+        upload_info = self.client.response_to_json(resp)
 
-        resp = await self.client.do_request(
+        resp = self.client.do_request(
             "PUT",
             upload_info["url"],
             headers={"content-type": content_type},
             data=data_buffer.read(),
         )
 
         upload_complete_url = (
             self.client.endpoint_url
             + "/datasets/"
             + self.uuid
             + "/files/upload-complete"
         )
         file_info_json = json.dumps({"id": upload_info["id"], "filename": file_name})
-        response = await self.client.do_request(
+        response = self.client.do_request(
             "POST",
             upload_complete_url,
             headers={"content-type": "application/json"},
             data=file_info_json,
         )
-        dataset = await self.client.get_dataset(uuid=self.uuid)
+        dataset = self.client.get_dataset(uuid=self.uuid)
         self.__update_dataset(dataset)
 
-        response_json = await self.client.response_to_json(response)
+        response_json = self.client.response_to_json(response)
         if file_access_audit_func is not None:
-            await file_access_audit_func(  # pylint: disable=not-callable
+            file_access_audit_func(  # pylint: disable=not-callable
                 FileAccessAudit(
                     self.uuid,
                     self.latest_version_number,
                     response_json["data"]["uuid"],
                     response_json["data"]["version"]["sequence_number"],
                     "write",
                 ).to_dict()
             )
 
-    async def create_csv_file(self, file_name: str, data_frame: pd.DataFrame):
+    def create_csv_file(self, file_name: str, data_frame: pd.DataFrame):
         """
         description:    the function is used to create
                         a new csv file in the dataset
 
         arguments:      file_name - name of the new csv file (must include extension)
                         data_frame - dataframe containing the csv data
         """
         buffer = io.BytesIO()
         data_frame.to_csv(buffer, index=False)
         buffer.seek(0)
 
-        await self.create_raw_file(buffer, file_name, "text/csv")
+        self.create_raw_file(buffer, file_name, "text/csv")
 
-    async def create_json_file(self, file_name: str, data_frame: pd.DataFrame):
+    def create_json_file(self, file_name: str, data_frame: pd.DataFrame):
         """
         description:    the function is used to create
                         a new json file in the dataset
 
         arguments:      file_name - name of the new json file (must include extension)
                         data_frame - dataframe containing the json data
         """
         buffer = io.BytesIO()
         data_frame.to_json(buffer)
         buffer.seek(0)
-        await self.create_raw_file(buffer, file_name, "application/json")
+        self.create_raw_file(buffer, file_name, "application/json")
 
-    async def create_spreadsheet_file(self, file_name: str, data_frame: pd.DataFrame):
+    def create_spreadsheet_file(self, file_name: str, data_frame: pd.DataFrame):
         """
         description:    the function is used to create
                         a new spreadsheet file in the dataset
 
         arguments:      file_name - name of the new spreadsheet file (must include extension)
                         data_frame - dataframe containing the spreadsheet data
         """
@@ -588,48 +561,48 @@
 
         buffer = io.BytesIO()
         with pd.ExcelWriter(  # pylint: disable=abstract-class-instantiated
             buffer
         ) as writer:
             data_frame.to_excel(writer, index=False)
         buffer.seek(0)
-        await self.create_raw_file(buffer, file_name, content_type)
+        self.create_raw_file(buffer, file_name, content_type)
 
-    async def create_parquet_file(self, file_name: str, data_frame: pd.DataFrame):
+    def create_parquet_file(self, file_name: str, data_frame: pd.DataFrame):
         """
         description:    the function is used to create
                         a new parquet file in the dataset
 
         arguments:      file_name - name of the new parquet file (must include extension)
                         data_frame - dataframe containing the parquet data
         """
         buffer = io.BytesIO()
         data_frame.to_parquet(buffer)
         buffer.seek(0)
-        await self.create_raw_file(buffer, file_name, "application/vnd.apache.parquet")
+        self.create_raw_file(buffer, file_name, "application/vnd.apache.parquet")
 
-    async def latest(self):
+    def latest(self):
         """
         Returns the latest version of the dataset in the form
         of a DatasetVersion instance
         """
-        dataset = await self.client.get_dataset(uuid=self.uuid)
+        dataset = self.client.get_dataset(uuid=self.uuid)
         return DatasetVersion(self, dataset.version)
 
-    async def get_version(self, dataset_version: int):
+    def get_version(self, dataset_version: int):
         """
         This function is going to return a requested
         version of the dataset
         """
 
         dataset_url = self.client.endpoint_url + "/datasets/" + self.uuid
-        client_response = await self.client.do_request(
+        client_response = self.client.do_request(
             "GET", dataset_url, params={"dataset_version": dataset_version}
         )
-        response_json = await self.client.response_to_json(client_response)
+        response_json = self.client.response_to_json(client_response)
         dataset_df = pd.json_normalize(response_json["data"], sep="_")
         dataset = Dataset(dataset_df.iloc[0].to_dict(), self)
         if dataset:
             return DatasetVersion(self, dataset.version)
         return None
 
     def __eq__(self, other):
@@ -657,15 +630,14 @@
             owner_username: {self.owner_username}
             thumbnail: {self.thumbnail}
             created_at: {self.created_at}
             updated_at: {self.updated_at}
             latest_version_number: {self.version["sequence_number"]}
             client: {{
                 endpoint_url: {self.client.endpoint_url}
-                session_closed: {self.client.session.closed}
             }}
         )"""
 
     def __str__(self):
         return f"Dataset(uuid: {self.uuid}, created_at: {self.created_at}, updated_time: {self.updated_at})"
 
     def __update_dataset(self, dataset):
@@ -725,15 +697,14 @@
             owner_username: {self.dataset.owner_username}
             thumbnail: {self.dataset.thumbnail}
             created_at: {self.created_at}
             updated_at: {self.dataset.updated_at}
             latest_version_number: {self.dataset.version["sequence_number"]}
             client: {{
                 endpoint_url: {self.dataset.client.endpoint_url}
-                session_closed: {self.dataset.client.session.closed}
             }})
             sequence_number: {self.sequence_number}
             name: {self.name}
             description: {self.description}
             create_at: {self.created_at}
             files: {self.files}
         )"""
@@ -759,74 +730,73 @@
         self.filename = file_desc["version"]["filename"]
         self.size = file_desc["version"]["size"]
         self.version = file_desc["version"]["sequence_number"]
         self.version_created_at = file_desc["version"]["created_at"]
         self.file_type = os.path.splitext(self.filename)[1]
         self.client = client
 
-    async def as_df(self):
+    def as_df(self):
         """
         converts the file contents into a dataframe
         """
 
         if self.file_type == ".csv":
-            return pd.read_csv(await self.raw(), sep=",")
+            return pd.read_csv(self.raw(), sep=",")
         if self.file_type == ".json":
-            return pd.read_json(await self.raw())
+            return pd.read_json(self.raw())
         if self.file_type in (".xls", ".xlsx", ".ods"):
             try:
-                buffer = await self.raw()
+                buffer = self.raw()
                 dataframe = pd.read_excel(buffer)
                 return dataframe
             except ModuleNotFoundError as error:
                 raise ModuleNotFoundError(
                     f"Missing optional dependency. {error.msg}"
                 ) from error
 
         if self.file_type == ".parquet":
-            return pd.read_parquet(await self.raw())
+            return pd.read_parquet(self.raw())
 
         raise ValueError("Unsupported file type")
 
-    async def raw(self):
+    def raw(self):
         """
         converts the file contents into a bytes buffer
         """
         file_url = (
             self.client.endpoint_url
             + "/datasets/"
             + self.dataset_uuid
             + "/files/"
             + self.uuid
         )
         parameters = {"dataset_version": self.dataset_version}
-        resp = await self.client.do_request("GET", file_url, params=parameters)
+        resp = self.client.do_request("GET", file_url, params=parameters)
 
         if file_access_audit_func is not None:
-            await file_access_audit_func(  # pylint: disable=not-callable
+            file_access_audit_func(  # pylint: disable=not-callable
                 FileAccessAudit(
                     self.dataset_uuid,
                     self.dataset_version,
                     self.uuid,
                     self.version,
                     "read",
                 ).to_dict()
             )
-        return await self.client.response_to_bytes_buffer(resp)
+        return self.client.response_to_bytes_buffer(resp)
 
     def __repr__(self):
         return f"""DatasetFile(
             dataset_uuid: {self.dataset_uuid}
             dataset_version: {self.dataset_version}
             file_uuid: {self.uuid}
             filename: {self.filename}
             version: {self.version}
             size: {self.size}
             created_at: {self.created_at}
             client: {{
                 endpoint_url: {self.client.endpoint_url}
-                session_closed: {self.client.session.closed}
             }}
         )"""
 
     def __str__(self):
         return f"DatasetFile(file_uuid: {self.uuid}, filename: {self.filename}, version: {self.version}, size: {self.size})"
```

### Comparing `unbounded_data-0.43.1/unbounded_data/high_level_api.py` & `unbounded_data-0.43.2/unbounded_data/high_level_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Union, Optional
-import os
 import asyncio
 import re
 import csv
 import json
-import threading
 from io import StringIO, BytesIO
 
 import pandas as pd
 
 from .datasets import Client, Dataset
 
 
@@ -41,54 +39,14 @@
         return to_return
 
     future = asyncio.Future()
     future.set_result(to_return)
     return future
 
 
-def _synchronize_async_helper(to_await: asyncio.Future, sync: bool = True) -> Union[asyncio.Future, any]:
-    """
-    description:    runs asynchronous queries synchronously.
-
-    arguments:      to_await - input future.
-                    sync - whether to run the request synchronously or asynchronously. await is required if sync is false.
-
-    returns:        to_await (if not sync) or return value of to_await (if sync).
-    """
-
-    if not sync:
-        return to_await
-
-    async_response = []
-    async_exception = []
-
-    async def run_and_capture_result():
-        try:
-            response = await to_await
-            async_response.append(response)
-        except Exception as exc:
-            async_exception.append(exc)
-
-    def thread_func():
-        if os.name == 'nt':
-            asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-        loop = asyncio.new_event_loop()
-        coroutine = run_and_capture_result()
-        loop.run_until_complete(coroutine)
-
-    thread = threading.Thread(target=thread_func)
-    thread.start()
-    thread.join()
-
-    if async_exception:
-        raise async_exception[0]
-
-    return async_response[0]
-
-
 def _guess_mime_type(check_bytes: bytes) -> str:
     """
     description:    guesses MIME type. raises with a nice error if magic is not installed.
 
     arguments:      check_bytes - byte array to autodetect.
 
     returns:        MIME type.
@@ -132,26 +90,23 @@
                     file_name - file name to read.
                     sync - whether to run the request synchronously or asynchronously. await is required if sync is false.
                     client - custom Client structure, if any.
 
     returns:        file content.
     """
 
-    async def read_file_func():
+    def read_file_func():
         real_client = _refresh_client(client=client)
-        try:
-            dataset = await _get_dataset_from_arg(dataset_name_or_id, client=real_client)
-            dataset_version = await dataset.latest()
-            buf = await dataset_version.get_file(file_name).raw()
-            buf.seek(0)
-            return buf.read()
-        finally:
-            await real_client.close_session()
+        dataset = _get_dataset_from_arg(dataset_name_or_id, client=real_client)
+        dataset_version = dataset.latest()
+        buf = dataset_version.get_file(file_name).raw()
+        buf.seek(0)
+        return buf.read()
 
-    return _synchronize_async_helper(read_file_func(), sync=sync)
+    return _desynchronize_async_helper(read_file_func(), sync=sync)
 
 
 def write_file(dataset_name_or_id: Union[Dataset, str],
                file_name: str,
                content: Union[str, bytes],
                mime_type: Optional[str] = None,
                sync: bool = True,
@@ -175,23 +130,20 @@
     if not isinstance(content, bytes):
         content = content.encode('utf-8')
 
     buf = BytesIO()
     buf.write(content)
     buf.seek(0)
 
-    async def write_file_func():
+    def write_file_func():
         real_client = _refresh_client(client=client)
-        try:
-            dataset = await _get_dataset_from_arg(dataset_name_or_id, client=real_client)
-            await dataset.create_raw_file(buf, file_name, mime_type)
-        finally:
-            await real_client.close_session()
+        dataset = _get_dataset_from_arg(dataset_name_or_id, client=real_client)
+        dataset.create_raw_file(buf, file_name, mime_type)
 
-    return _synchronize_async_helper(write_file_func(), sync=sync)
+    return _desynchronize_async_helper(write_file_func(), sync=sync)
 
 
 def read_json(dataset_name_or_id: Union[Dataset, str],
               file_name: str,
               sync: bool = True,
               client: Optional[Client] = None) -> Union[Union[dict, list, str, bool, int, float, None],
                                                         asyncio.Future[dict, list, str, bool, int, float, None]]:
@@ -243,26 +195,23 @@
                     sync - whether to run the request synchronously or asynchronously. await is required if sync is false.
                     client - custom Client structure, if any.
                     sep - column separator, defaults to comma (,).
 
     returns:        DataFrame.
     """
 
-    async def read_file_func():
+    def read_file_func():
         real_client = _refresh_client(client=client)
-        try:
-            dataset = await _get_dataset_from_arg(dataset_name_or_id, client=real_client)
-            dataset_version = await dataset.latest()
-            buf = await dataset_version.get_file(file_name).raw()
-            buf.seek(0)
-            return buf.read()
-        finally:
-            await real_client.close_session()
+        dataset = _get_dataset_from_arg(dataset_name_or_id, client=real_client)
+        dataset_version = dataset.latest()
+        buf = dataset_version.get_file(file_name).raw()
+        buf.seek(0)
+        return buf.read()
 
-    as_bytes = _synchronize_async_helper(read_file_func(), sync=True)
+    as_bytes = read_file_func()
     buf = StringIO()
     buf.write(as_bytes.decode('utf-8', errors='surrogateescape'))
     buf.seek(0)
     return _desynchronize_async_helper(pd.read_csv(buf, engine='python', sep=sep), sync=sync)
 
 
 def read_tsv(dataset_name_or_id: Union[Dataset, str],
@@ -348,26 +297,23 @@
                     file_name - file name to read.
                     sync - whether to run the request synchronously or asynchronously. await is required if sync is false.
                     client - custom Client structure, if any.
 
     returns:        DataFrame.
     """
 
-    async def read_file_func():
+    def read_file_func():
         real_client = _refresh_client(client=client)
-        try:
-            dataset = await _get_dataset_from_arg(dataset_name_or_id, client=real_client)
-            dataset_version = await dataset.latest()
-            buf = await dataset_version.get_file(file_name).raw()
-            buf.seek(0)
-            return buf
-        finally:
-            await real_client.close_session()
+        dataset = _get_dataset_from_arg(dataset_name_or_id, client=real_client)
+        dataset_version = dataset.latest()
+        buf = dataset_version.get_file(file_name).raw()
+        buf.seek(0)
+        return buf
 
-    return _desynchronize_async_helper(pd.read_parquet(_synchronize_async_helper(read_file_func(), sync=True)), sync=sync)
+    return _desynchronize_async_helper(pd.read_parquet(read_file_func()), sync=sync)
 
 
 def write_parquet(dataset_name_or_id: Union[Dataset, str],
                   file_name: str,
                   content: Union[list[list], pd.DataFrame],
                   sync: bool = True,
                   client: Optional[Client] = None) -> Optional[asyncio.Future]:
```

### Comparing `unbounded_data-0.43.1/PKG-INFO` & `unbounded_data-0.43.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: unbounded-data
-Version: 0.43.1
+Version: 0.43.2
 Summary: The Unbounded Network Data Python interface
 Author: Unbounded Network
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pyarrow (>=14.0.0,<15.0.0)
 Requires-Dist: python-benedict (>=0.25.2,<0.26.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
```

