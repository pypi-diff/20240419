# Comparing `tmp/qcanvas_api_clients-0.1.1a0.tar.gz` & `tmp/qcanvas_api_clients-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcanvas_api_clients-0.1.1a0.tar", max compression
+gzip compressed data, was "qcanvas_api_clients-0.1.1a1.tar", max compression
```

## Comparing `qcanvas_api_clients-0.1.1a0.tar` & `qcanvas_api_clients-0.1.1a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      147 2024-04-19 08:16:32.823915 qcanvas_api_clients-0.1.1a0/README.md
--rw-r--r--   0        0        0      383 2024-04-19 10:16:25.369754 qcanvas_api_clients-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0      256 2024-04-19 10:17:43.392358 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 05:01:07.784421 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__init__.py
--rw-r--r--   0        0        0      190 2024-04-19 04:07:35.842093 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1468 2024-04-19 05:49:53.468880 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_api_config.cpython-311.pyc
--rw-r--r--   0        0        0     3704 2024-04-19 05:49:53.496881 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_authenticator.cpython-311.pyc
--rw-r--r--   0        0        0     8434 2024-04-19 08:20:42.812628 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_client.cpython-311.pyc
--rw-r--r--   0        0        0     1751 2024-04-19 05:06:06.454980 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_file_downloader_stream_wrapper.cpython-311.pyc
--rw-r--r--   0        0        0     7794 2024-04-19 05:06:06.454980 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/legacy_canvas_types.cpython-311.pyc
--rw-r--r--   0        0        0      457 2024-04-19 09:17:43.907392 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_api_config.py
--rw-r--r--   0        0        0     1889 2024-04-19 09:49:16.184890 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_authenticator.py
--rw-r--r--   0        0        0     4898 2024-04-19 10:17:43.356357 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_client.py
--rw-r--r--   0        0        0      703 2024-04-19 10:17:43.360357 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_file_downloader_stream_wrapper.py
--rw-r--r--   0        0        0     3983 2024-04-18 05:02:17.926825 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/legacy_canvas_types.py
--rw-r--r--   0        0        0       99 2024-04-19 09:20:16.559996 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/mock_canvas_client.py
--rw-r--r--   0        0        0        0 2024-04-19 05:07:33.773897 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__init__.py
--rw-r--r--   0        0        0      191 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1117 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_api_config.cpython-311.pyc
--rw-r--r--   0        0        0     2295 2024-04-19 06:01:27.788908 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_authenticator.cpython-311.pyc
--rw-r--r--   0        0        0     4427 2024-04-19 08:21:09.309538 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_client.cpython-311.pyc
--rw-r--r--   0        0        0    59613 2024-04-19 08:17:05.305062 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_types.cpython-311.pyc
--rw-r--r--   0        0        0   154580 2024-04-19 10:17:43.392358 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panoptoApi.yaml
--rw-r--r--   0        0        0      307 2024-04-19 05:12:01.198822 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_api_config.py
--rw-r--r--   0        0        0      966 2024-04-19 10:17:43.400359 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_authenticator.py
--rw-r--r--   0        0        0     2304 2024-04-19 10:17:43.396358 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_client.py
--rw-r--r--   0        0        0    33132 2024-04-19 08:16:34.915989 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_types.py
--rw-r--r--   0        0        0        0 2024-04-19 03:16:57.450750 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__init__.py
--rw-r--r--   0        0        0      188 2024-04-19 04:07:36.070100 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2618 2024-04-19 04:07:36.070100 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/custom_httpx_async_transport.cpython-311.pyc
--rw-r--r--   0        0        0     4821 2024-04-19 07:17:01.422818 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/generic_authenticator.cpython-311.pyc
--rw-r--r--   0        0        0     1203 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/request_exceptions.cpython-311.pyc
--rw-r--r--   0        0        0      545 2024-04-19 05:49:53.496881 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/url_converter.cpython-311.pyc
--rw-r--r--   0        0        0     1227 2024-02-22 02:22:40.749609 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/custom_httpx_async_transport.py
--rw-r--r--   0        0        0     2462 2024-04-19 07:14:54.759701 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/generic_authenticator.py
--rw-r--r--   0        0        0      204 2024-04-19 10:17:43.400359 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/request_exceptions.py
--rw-r--r--   0        0        0      151 2024-04-19 05:11:10.937145 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/url_converter.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 qcanvas_api_clients-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0      147 2024-04-19 08:16:32.823915 qcanvas_api_clients-0.1.1a1/README.md
+-rw-r--r--   0        0        0      383 2024-04-19 11:42:51.536409 qcanvas_api_clients-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0      256 2024-04-19 10:17:43.392358 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 05:01:07.784421 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-19 04:07:35.842093 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1468 2024-04-19 05:49:53.468880 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/canvas_api_config.cpython-311.pyc
+-rw-r--r--   0        0        0     3704 2024-04-19 05:49:53.496881 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/canvas_authenticator.cpython-311.pyc
+-rw-r--r--   0        0        0     8434 2024-04-19 08:20:42.812628 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/canvas_client.cpython-311.pyc
+-rw-r--r--   0        0        0     1751 2024-04-19 05:06:06.454980 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/canvas_file_downloader_stream_wrapper.cpython-311.pyc
+-rw-r--r--   0        0        0     7794 2024-04-19 05:06:06.454980 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/legacy_canvas_types.cpython-311.pyc
+-rw-r--r--   0        0        0      457 2024-04-19 09:17:43.907392 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/canvas_api_config.py
+-rw-r--r--   0        0        0     1889 2024-04-19 09:49:16.184890 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/canvas_authenticator.py
+-rw-r--r--   0        0        0     4963 2024-04-19 11:42:16.095622 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/canvas_client.py
+-rw-r--r--   0        0        0      703 2024-04-19 10:17:43.360357 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/canvas_file_downloader_stream_wrapper.py
+-rw-r--r--   0        0        0     3983 2024-04-18 05:02:17.926825 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/legacy_canvas_types.py
+-rw-r--r--   0        0        0       99 2024-04-19 09:20:16.559996 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/mock_canvas_client.py
+-rw-r--r--   0        0        0        0 2024-04-19 05:07:33.773897 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1117 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/__pycache__/panopto_api_config.cpython-311.pyc
+-rw-r--r--   0        0        0     2295 2024-04-19 06:01:27.788908 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/__pycache__/panopto_authenticator.cpython-311.pyc
+-rw-r--r--   0        0        0     4427 2024-04-19 08:21:09.309538 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/__pycache__/panopto_client.cpython-311.pyc
+-rw-r--r--   0        0        0    59613 2024-04-19 08:17:05.305062 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/__pycache__/panopto_types.cpython-311.pyc
+-rw-r--r--   0        0        0   154580 2024-04-19 10:17:43.392358 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/panoptoApi.yaml
+-rw-r--r--   0        0        0      307 2024-04-19 05:12:01.198822 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/panopto_api_config.py
+-rw-r--r--   0        0        0      966 2024-04-19 10:17:43.400359 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/panopto_authenticator.py
+-rw-r--r--   0        0        0     2304 2024-04-19 10:17:43.396358 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/panopto_client.py
+-rw-r--r--   0        0        0    33132 2024-04-19 08:16:34.915989 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/panopto_types.py
+-rw-r--r--   0        0        0        0 2024-04-19 03:16:57.450750 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-19 04:07:36.070100 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2618 2024-04-19 04:07:36.070100 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/__pycache__/custom_httpx_async_transport.cpython-311.pyc
+-rw-r--r--   0        0        0     4821 2024-04-19 07:17:01.422818 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/__pycache__/generic_authenticator.cpython-311.pyc
+-rw-r--r--   0        0        0     1203 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/__pycache__/request_exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0      545 2024-04-19 05:49:53.496881 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/__pycache__/url_converter.cpython-311.pyc
+-rw-r--r--   0        0        0     1227 2024-02-22 02:22:40.749609 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/custom_httpx_async_transport.py
+-rw-r--r--   0        0        0     2462 2024-04-19 07:14:54.759701 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/generic_authenticator.py
+-rw-r--r--   0        0        0      204 2024-04-19 10:17:43.400359 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/request_exceptions.py
+-rw-r--r--   0        0        0      151 2024-04-19 05:11:10.937145 qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/url_converter.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 qcanvas_api_clients-0.1.1a1/PKG-INFO
```

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_api_config.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/canvas_api_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_authenticator.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/canvas_authenticator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_client.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/canvas_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_file_downloader_stream_wrapper.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/canvas_file_downloader_stream_wrapper.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/legacy_canvas_types.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/__pycache__/legacy_canvas_types.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_authenticator.py` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/canvas_authenticator.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_client.py` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/canvas_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from qcanvas_api_clients.canvas.canvas_file_downloader_stream_wrapper import CanvasFileDownloaderStreamWrapper
 from qcanvas_api_clients.canvas.legacy_canvas_types import LegacyPage, LegacyFile
 from qcanvas_api_clients.util.custom_httpx_async_transport import CustomHTTPXAsyncTransport
 from qcanvas_api_clients.util.request_exceptions import RatelimitedError
 
 
 class CanvasClient:
-    def __init__(self, api_config: CanvasApiConfig, max_concurrent_operations: int = 20, gql_timeout: int = 120):
+    def __init__(self, api_config: CanvasApiConfig, max_concurrent_operations: int = 20, gql_timeout: float = 120, httpx_timeout: float = 120):
         self._api_config = api_config
-        self.client = httpx.AsyncClient()
+        self.client = httpx.AsyncClient(timeout=httpx_timeout)
         self._authentication_controller = CanvasAuthenticator(self.client, self._api_config)
         self._concurrent_request_limiter = asyncio.Semaphore(max_concurrent_operations)
         self._gql_timeout = gql_timeout
 
     async def run_graphql_query(self, query: GraphQLQuery, query_variables: dict[str, Any] = None) -> dict[str, Any]:
         if query_variables is None:
             query_variables = {}
@@ -41,15 +41,15 @@
             client=self.client,
             url=self._api_config.get_endpoint("api/graphql"),
             headers=self._api_config.get_authorization_header()
         )
 
         return gql.Client(
             transport=transport,
-            execute_timeout=120
+            execute_timeout=self._gql_timeout
         )
 
     def open_stream_to_download_file(self, file_url: str | URL) -> CanvasFileDownloaderStreamWrapper:
         return CanvasFileDownloaderStreamWrapper(
             request=self.client.build_request(
                 method="GET",
                 url=file_url
```

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_file_downloader_stream_wrapper.py` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/canvas_file_downloader_stream_wrapper.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/legacy_canvas_types.py` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/canvas/legacy_canvas_types.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_api_config.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/__pycache__/panopto_api_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_authenticator.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/__pycache__/panopto_authenticator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_client.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/__pycache__/panopto_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_types.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/__pycache__/panopto_types.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panoptoApi.yaml` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/panoptoApi.yaml`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_authenticator.py` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/panopto_authenticator.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_client.py` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/panopto_client.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_types.py` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/panopto/panopto_types.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/custom_httpx_async_transport.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/__pycache__/custom_httpx_async_transport.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/generic_authenticator.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/__pycache__/generic_authenticator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/request_exceptions.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/__pycache__/request_exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/url_converter.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/__pycache__/url_converter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/custom_httpx_async_transport.py` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/custom_httpx_async_transport.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/generic_authenticator.py` & `qcanvas_api_clients-0.1.1a1/qcanvas_api_clients/util/generic_authenticator.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.1a0/PKG-INFO` & `qcanvas_api_clients-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcanvas-api-clients
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: 
 Author: QCanvas
 Author-email: qcanvas@noreply.codeberg.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

