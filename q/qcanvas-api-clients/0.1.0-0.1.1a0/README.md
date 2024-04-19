# Comparing `tmp/qcanvas_api_clients-0.1.0.tar.gz` & `tmp/qcanvas_api_clients-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcanvas_api_clients-0.1.0.tar", max compression
+gzip compressed data, was "qcanvas_api_clients-0.1.1a0.tar", max compression
```

## Comparing `qcanvas_api_clients-0.1.0.tar` & `qcanvas_api_clients-0.1.1a0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      147 2024-04-19 08:16:32.823915 qcanvas_api_clients-0.1.0/README.md
--rw-r--r--   0        0        0      381 2024-04-19 09:20:16.563996 qcanvas_api_clients-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      255 2024-04-19 09:18:37.120994 qcanvas_api_clients-0.1.0/qcanvas_api_clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 05:01:07.784421 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__init__.py
--rw-r--r--   0        0        0      190 2024-04-19 04:07:35.842093 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1468 2024-04-19 05:49:53.468880 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/canvas_api_config.cpython-311.pyc
--rw-r--r--   0        0        0     3704 2024-04-19 05:49:53.496881 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/canvas_authenticator.cpython-311.pyc
--rw-r--r--   0        0        0     8434 2024-04-19 08:20:42.812628 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/canvas_client.cpython-311.pyc
--rw-r--r--   0        0        0     1751 2024-04-19 05:06:06.454980 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/canvas_file_downloader_stream_wrapper.cpython-311.pyc
--rw-r--r--   0        0        0     7794 2024-04-19 05:06:06.454980 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/legacy_canvas_types.cpython-311.pyc
--rw-r--r--   0        0        0      457 2024-04-19 09:17:43.907392 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/canvas_api_config.py
--rw-r--r--   0        0        0     1988 2024-04-19 05:40:53.034056 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/canvas_authenticator.py
--rw-r--r--   0        0        0     4734 2024-04-19 09:15:22.823158 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/canvas_client.py
--rw-r--r--   0        0        0      705 2024-04-19 04:50:25.347231 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/canvas_file_downloader_stream_wrapper.py
--rw-r--r--   0        0        0     3983 2024-04-18 05:02:17.926825 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/legacy_canvas_types.py
--rw-r--r--   0        0        0       99 2024-04-19 09:20:16.559996 qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/mock_canvas_client.py
--rw-r--r--   0        0        0        0 2024-04-19 05:07:33.773897 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/__init__.py
--rw-r--r--   0        0        0      191 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1117 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/__pycache__/panopto_api_config.cpython-311.pyc
--rw-r--r--   0        0        0     2295 2024-04-19 06:01:27.788908 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/__pycache__/panopto_authenticator.cpython-311.pyc
--rw-r--r--   0        0        0     4427 2024-04-19 08:21:09.309538 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/__pycache__/panopto_client.cpython-311.pyc
--rw-r--r--   0        0        0    59613 2024-04-19 08:17:05.305062 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/__pycache__/panopto_types.cpython-311.pyc
--rw-r--r--   0        0        0   150579 2024-04-19 07:58:51.585821 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/panoptoApi.yaml
--rw-r--r--   0        0        0      307 2024-04-19 05:12:01.198822 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/panopto_api_config.py
--rw-r--r--   0        0        0      958 2024-04-19 05:58:43.250658 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/panopto_authenticator.py
--rw-r--r--   0        0        0     2316 2024-04-19 09:16:51.517817 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/panopto_client.py
--rw-r--r--   0        0        0    33132 2024-04-19 08:16:34.915989 qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/panopto_types.py
--rw-r--r--   0        0        0        0 2024-04-19 03:16:57.450750 qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/__init__.py
--rw-r--r--   0        0        0      188 2024-04-19 04:07:36.070100 qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2618 2024-04-19 04:07:36.070100 qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/__pycache__/custom_httpx_async_transport.cpython-311.pyc
--rw-r--r--   0        0        0     4821 2024-04-19 07:17:01.422818 qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/__pycache__/generic_authenticator.cpython-311.pyc
--rw-r--r--   0        0        0     1203 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/__pycache__/request_exceptions.cpython-311.pyc
--rw-r--r--   0        0        0      545 2024-04-19 05:49:53.496881 qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/__pycache__/url_converter.cpython-311.pyc
--rw-r--r--   0        0        0     1227 2024-02-22 02:22:40.749609 qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/custom_httpx_async_transport.py
--rw-r--r--   0        0        0     2462 2024-04-19 07:14:54.759701 qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/generic_authenticator.py
--rw-r--r--   0        0        0      201 2024-04-18 06:15:03.569027 qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/request_exceptions.py
--rw-r--r--   0        0        0      151 2024-04-19 05:11:10.937145 qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/url_converter.py
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 qcanvas_api_clients-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      147 2024-04-19 08:16:32.823915 qcanvas_api_clients-0.1.1a0/README.md
+-rw-r--r--   0        0        0      383 2024-04-19 10:16:25.369754 qcanvas_api_clients-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      256 2024-04-19 10:17:43.392358 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 05:01:07.784421 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-19 04:07:35.842093 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1468 2024-04-19 05:49:53.468880 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_api_config.cpython-311.pyc
+-rw-r--r--   0        0        0     3704 2024-04-19 05:49:53.496881 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_authenticator.cpython-311.pyc
+-rw-r--r--   0        0        0     8434 2024-04-19 08:20:42.812628 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_client.cpython-311.pyc
+-rw-r--r--   0        0        0     1751 2024-04-19 05:06:06.454980 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_file_downloader_stream_wrapper.cpython-311.pyc
+-rw-r--r--   0        0        0     7794 2024-04-19 05:06:06.454980 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/legacy_canvas_types.cpython-311.pyc
+-rw-r--r--   0        0        0      457 2024-04-19 09:17:43.907392 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_api_config.py
+-rw-r--r--   0        0        0     1889 2024-04-19 09:49:16.184890 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_authenticator.py
+-rw-r--r--   0        0        0     4898 2024-04-19 10:17:43.356357 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_client.py
+-rw-r--r--   0        0        0      703 2024-04-19 10:17:43.360357 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_file_downloader_stream_wrapper.py
+-rw-r--r--   0        0        0     3983 2024-04-18 05:02:17.926825 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/legacy_canvas_types.py
+-rw-r--r--   0        0        0       99 2024-04-19 09:20:16.559996 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/mock_canvas_client.py
+-rw-r--r--   0        0        0        0 2024-04-19 05:07:33.773897 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1117 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_api_config.cpython-311.pyc
+-rw-r--r--   0        0        0     2295 2024-04-19 06:01:27.788908 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_authenticator.cpython-311.pyc
+-rw-r--r--   0        0        0     4427 2024-04-19 08:21:09.309538 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_client.cpython-311.pyc
+-rw-r--r--   0        0        0    59613 2024-04-19 08:17:05.305062 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_types.cpython-311.pyc
+-rw-r--r--   0        0        0   154580 2024-04-19 10:17:43.392358 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panoptoApi.yaml
+-rw-r--r--   0        0        0      307 2024-04-19 05:12:01.198822 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_api_config.py
+-rw-r--r--   0        0        0      966 2024-04-19 10:17:43.400359 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_authenticator.py
+-rw-r--r--   0        0        0     2304 2024-04-19 10:17:43.396358 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_client.py
+-rw-r--r--   0        0        0    33132 2024-04-19 08:16:34.915989 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_types.py
+-rw-r--r--   0        0        0        0 2024-04-19 03:16:57.450750 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-19 04:07:36.070100 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2618 2024-04-19 04:07:36.070100 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/custom_httpx_async_transport.cpython-311.pyc
+-rw-r--r--   0        0        0     4821 2024-04-19 07:17:01.422818 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/generic_authenticator.cpython-311.pyc
+-rw-r--r--   0        0        0     1203 2024-04-19 05:49:53.500881 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/request_exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0      545 2024-04-19 05:49:53.496881 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/url_converter.cpython-311.pyc
+-rw-r--r--   0        0        0     1227 2024-02-22 02:22:40.749609 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/custom_httpx_async_transport.py
+-rw-r--r--   0        0        0     2462 2024-04-19 07:14:54.759701 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/generic_authenticator.py
+-rw-r--r--   0        0        0      204 2024-04-19 10:17:43.400359 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/request_exceptions.py
+-rw-r--r--   0        0        0      151 2024-04-19 05:11:10.937145 qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/url_converter.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 qcanvas_api_clients-0.1.1a0/PKG-INFO
```

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/canvas_api_config.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_api_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/canvas_authenticator.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_authenticator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/canvas_client.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/canvas_file_downloader_stream_wrapper.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/canvas_file_downloader_stream_wrapper.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/__pycache__/legacy_canvas_types.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/__pycache__/legacy_canvas_types.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/canvas_authenticator.py` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_authenticator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import json
-from typing import Optional
 
 import httpx
-from asynctaskpool import AsyncTaskPool
-from httpx import Response, Cookies
+from httpx import Response
 
 from qcanvas_api_clients.canvas.canvas_api_config import CanvasApiConfig
 from qcanvas_api_clients.util.generic_authenticator import GenericAuthenticator
-from qcanvas_api_clients.util.request_exceptions import AuthenticationFailedError, UnauthenticatedError
+from qcanvas_api_clients.util.request_exceptions import AuthenticationFailedError
 
 
 class CanvasAuthenticator(GenericAuthenticator):
     def __init__(self, client: httpx.AsyncClient, canvas_api_config: CanvasApiConfig):
         super().__init__(client)
         self._canvas_api_config = canvas_api_config
```

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/canvas_client.py` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import asyncio
 import json
 from typing import Any, Optional
 
 import gql
-from gql.client import DocumentNode as GraphQLQuery
 import httpx
+from gql.client import DocumentNode as GraphQLQuery
 from httpx import Response, URL, Request
 from tenacity import retry, wait_exponential, wait_random, stop_after_attempt, retry_if_exception_type
 
 from qcanvas_api_clients.canvas.canvas_api_config import CanvasApiConfig
 from qcanvas_api_clients.canvas.canvas_authenticator import CanvasAuthenticator
 from qcanvas_api_clients.canvas.canvas_file_downloader_stream_wrapper import CanvasFileDownloaderStreamWrapper
 from qcanvas_api_clients.canvas.legacy_canvas_types import LegacyPage, LegacyFile
-from qcanvas_api_clients.util.request_exceptions import RatelimitedError
 from qcanvas_api_clients.util.custom_httpx_async_transport import CustomHTTPXAsyncTransport
+from qcanvas_api_clients.util.request_exceptions import RatelimitedError
 
 
 class CanvasClient:
     def __init__(self, api_config: CanvasApiConfig, max_concurrent_operations: int = 20, gql_timeout: int = 120):
         self._api_config = api_config
         self.client = httpx.AsyncClient()
         self._authentication_controller = CanvasAuthenticator(self.client, self._api_config)
@@ -89,22 +89,23 @@
         return response
 
     @retry(
         wait=wait_exponential(exp_base=1.2, max=10) + wait_random(0, 1),
         retry=retry_if_exception_type(RatelimitedError),
         stop=stop_after_attempt(8)
     )
-    async def _execute_request_and_handle_retry_if_ratelimited(self, request: Request, follow_redirects: Optional[bool] = None) -> Response:
+    async def _execute_request_and_handle_retry_if_ratelimited(self, request: Request,
+                                                               follow_redirects: Optional[bool] = None) -> Response:
         async with self._concurrent_request_limiter:
-            response = await self._authentication_controller.do_request_and_authenticate_if_necessary(request, follow_redirects=follow_redirects)
+            response = await self._authentication_controller.do_request_and_authenticate_if_necessary(request,
+                                                                                                      follow_redirects=follow_redirects)
 
         self._detect_ratelimit_and_raise(response)
 
         return response
 
-
     @staticmethod
     def _detect_ratelimit_and_raise(response: Response):
         # Who the FUCK decided to use 403 instead of 429?? With this stupid message??
         # And the newline at the end for some fucking reason is the cherry on top...
         if response.status_code == 403 and response.text == "403 Forbidden (Rate Limit Exceeded)\n":
             raise RatelimitedError()
```

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/canvas_file_downloader_stream_wrapper.py` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/canvas_file_downloader_stream_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,7 @@
             follow_redirects=True
         )
 
         return self.stream
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.stream.aclose()
-
-
```

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/canvas/legacy_canvas_types.py` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/canvas/legacy_canvas_types.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/__pycache__/panopto_api_config.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_api_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/__pycache__/panopto_authenticator.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_authenticator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/__pycache__/panopto_client.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/__pycache__/panopto_types.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/__pycache__/panopto_types.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/panoptoApi.yaml` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panoptoApi.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 openapi: 3.0.1
 info:
   title: Panopto Public API
   description: The public API for Panopto. OpenID & OAuth information can be found
     at Panopto/oauth2/.well-known/openid-configuration
   version: "1"
 servers:
-- url: https://<PanoptoServerURL>(i.e. example.hosted.panopto.com)/Panopto
+  - url: https://<PanoptoServerURL>(i.e. example.hosted.panopto.com)/Panopto
 tags:
-- name: Auth
-  description: Authentication API
-- name: RemoteRecorderAPI
-  description: "Remote Recorder Device API. Warning: this endpoint is for Panopto's\
+  - name: Auth
+    description: Authentication API
+  - name: RemoteRecorderAPI
+    description: "Remote Recorder Device API. Warning: this endpoint is for Panopto's\
     \ hardware partners only and cannot be used without a partner API key."
-- name: Folders
-  description: Folder API
-- name: Groups
-  description: Group API
-- name: Playlists
-  description: Playlist API
-- name: RemoteRecorders
-  description: Remote Recorder Management API
-- name: ScheduledRecordings
-  description: Scheduled Recording API
-- name: SearchIndexSyncUpdates
-  description: Search Index Integration API
-- name: Sessions
-  description: Session API
-- name: Streams
-  description: Stream API
-- name: Tags
-  description: Tag API
-- name: Users
-  description: User API
+  - name: Folders
+    description: Folder API
+  - name: Groups
+    description: Group API
+  - name: Playlists
+    description: Playlist API
+  - name: RemoteRecorders
+    description: Remote Recorder Management API
+  - name: ScheduledRecordings
+    description: Scheduled Recording API
+  - name: SearchIndexSyncUpdates
+    description: Search Index Integration API
+  - name: Sessions
+    description: Session API
+  - name: Streams
+    description: Stream API
+  - name: Tags
+    description: Tag API
+  - name: Users
+    description: User API
 paths:
   /api/v1/auth/legacyLogin:
     get:
       tags:
-      - Auth
+        - Auth
       summary: Get a legacy authentication cookie
       description: Gets an authentication cookie from a valid Oauth2 token for use
         with legacy APIs.
       operationId: Auth_LegacyLogin
       responses:
         "200":
           description: The authentication cookie should be set
           content:
             application/json:
               schema:
                 type: string
         "401":
           description: "No valid authorization. The token may be invalid, or the user\
             \ was not authenticated or found."
-          content: {}
+          content: { }
   /api/v1/remoteRecorderAPI/remoteRecorder:
     put:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: Register a new remote recorder
       description: "Retrieves the remote recorder public ID and credentials to access\
         \ the RR API. \r\n                  Uses BasicAuth requiring a remote recorder\
         \ registration key from an admin"
       operationId: RemoteRecorderAPI_RegisterRemoteRecorder
       requestBody:
         content:
@@ -82,95 +82,95 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: registrationRequest
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/connect:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: Connect as the provided remote recorder
       description: "Remote recorder is identified via the GUID public id\r\n     \
         \           recorderVersion is a version identifier in the form of \"<vendor>.<product>.<major>.<minor>.<servicing>\"\
         \r\n                buildVersion is the vendor specific build string"
       operationId: RemoteRecorderAPI_Connect
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: recorderVersion
-        in: query
-        required: true
-        schema:
-          type: string
-          nullable: true
-      - name: recorderBuild
-        in: query
-        required: true
-        schema:
-          type: string
-          nullable: true
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: recorderVersion
+          in: query
+          required: true
+          schema:
+            type: string
+            nullable: true
+        - name: recorderBuild
+          in: query
+          required: true
+          schema:
+            type: string
+            nullable: true
       responses:
         "400":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/disconnect:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: "Disconnect as the provided remote recorder, identified via the GUID\
         \ public id"
       operationId: RemoteRecorderAPI_Disconnect
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "400":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/heartbeat:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: Heartbeat and preview as the provided remote recorder
       description: "Remote recorder is identified via the GUID public id\r\n     \
         \           Include options: defaults (provides default quality settings and\
         \ folder), extendedConfigurations (provides extended configurations)"
       operationId: RemoteRecorderAPI_Heartbeat
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: include
-        in: query
-        style: form
-        explode: true
-        schema:
-          type: array
-          nullable: true
-          items:
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
             type: string
+            format: guid
+            nullable: false
+        - name: include
+          in: query
+          style: form
+          explode: true
+          schema:
+            type: array
+            nullable: true
+            items:
+              type: string
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RemoteRecorderHeartbeatData'
         required: false
       responses:
@@ -186,36 +186,36 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: updateData
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/schedule:
     get:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: Retrieve a schedule for the next 7 days for the provided remote recorder.As
         a best practice a new scheduled should be fetched every day even if the schedule
         version in the heartbeat hasn't changed
       operationId: RemoteRecorderAPI_GetSchedule
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: include
-        in: query
-        style: form
-        explode: true
-        schema:
-          type: array
-          nullable: true
-          items:
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
             type: string
+            format: guid
+            nullable: false
+        - name: include
+          in: query
+          style: form
+          explode: true
+          schema:
+            type: array
+            nullable: true
+            items:
+              type: string
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/RemoteRecorderSchedule'
@@ -223,27 +223,27 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: "Update or add a set of scheduled recordings for the provided remote\
         \ recorder. To add a scheduled recording, the recording should have all relevant\
         \ fields filled in but an empty (all zeros) guid"
       operationId: RemoteRecorderAPI_UpdateSchedule
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               type: array
               items:
                 $ref: '#/components/schemas/RemoteRecorderScheduledRecording'
@@ -255,25 +255,25 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: recordingsToUpdate
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/error:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: Register an error with the provided remote recorder on the server
       operationId: RemoteRecorderAPI_Error
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RemoteRecorderError'
         required: false
       responses:
@@ -283,46 +283,46 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: remoteRecorderError
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/legacyLogin:
     get:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: Retrieve a legacy ASPXAUTH cookie
       operationId: RemoteRecorderAPI_LegacyLogin
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "401":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/remoteRecorderAPI/session/{sessionId}/pause:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: Pause the recording of the specified session on the server
       operationId: RemoteRecorderAPI_PauseRecording
       parameters:
-      - name: sessionId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: sessionId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RemoteRecorderPauseRecordingRequest'
         required: false
       responses:
@@ -332,25 +332,25 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: pauseRecordingRequest
   /api/v1/remoteRecorderAPI/session/{sessionId}/resume:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: Resume the recording of the specified session on the server
       operationId: RemoteRecorderAPI_ResumeRecording
       parameters:
-      - name: sessionId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: sessionId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RemoteRecorderResumeRecordingRequest'
         required: false
       responses:
@@ -360,28 +360,28 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: resumeRecordingRequest
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/urls:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: "Provides a list of URLs and URL types to present to administrators\
         \ to help them manage this remote recorder.Calling this replaces all previously\
         \ reported URLs. URLs are preserved until replaced, so this only needs to\
         \ be called when they have changed"
       operationId: RemoteRecorderAPI_ReportRemoteRecorderURLs
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/RemoteRecorderURLsUpdateRequest'
         required: false
       responses:
@@ -391,27 +391,27 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: urlUpdateRequest
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/liveMonitoring/webRtc/connect:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: "Establishes a new connection which enables the WebRTC-based media\
         \ preview feature.  After this, the client should commence WebRTC session\
         \ negotiation by sending us an SDP offer."
       operationId: RemoteRecorderAPI_WebRtcConnect
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/WebRtcConnectPostData'
         required: false
       responses:
@@ -439,26 +439,26 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: postData
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/liveMonitoring/webRtc/disconnect:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: Destroys the connection which enables the WebRTC-based media preview
         feature.
       operationId: RemoteRecorderAPI_WebRtcDisconnect
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/WebRtcDisconnectPostData'
         required: false
       responses:
@@ -480,15 +480,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: postData
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/liveMonitoring/webRtc/events:
     get:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: "After the client has sent us an SDP offer, they should poll this \
         \ endpoint periodically to receive messages."
       description: "After sending the SDP offer, the client should check here for\
         \ events periodically.  This is not a long-polling call,\r\nso it will return\
         \ quickly.\r\n\r\nPrior to receiving the SDP answer, the client should wait\
         \ `PingFastInterval` seconds between requests.  Five seconds\r\nafter receiving\
         \ the SDP answer, the client should wait `PingSlowInterval` seconds between\
@@ -514,21 +514,21 @@
         \ associated with this WebRTC session.  It does not need to call the REST\
         \ endpoint to explicitly\r\ndisconnect because the server is already aware\
         \ that WebRTC session is in a bad state, and the standard method for\r\ngraceful\
         \ cleanup is no longer possible.\r\n\r\n  The payload is human readable additional\
         \ information about the situation."
       operationId: RemoteRecorderAPI_WebRtcGetEvents
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/WebRtcEventsResponse'
@@ -543,36 +543,36 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/liveMonitoring/webRtc/iceCandidates:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: Sends a batch of ICE candidates from client to signaling server.
       description: "Sends a batch of ICE candidates from client (the RTP sender) to\
         \ signaling server.  ICE Candidates are used for the\r\ntransmission of RTP\
         \ and RTCP payloads.\r\n\r\nThis is a JSON array of ICE candidates, where\
         \ each ICE candidate is an object containing 2 fields.\r\n\r\n1.  `Index`:\
         \ This is a non-negative integer.  This is a zero-based index, corresponding\
         \ to a specific section within an\r\n    SDP offer, where each section begins\
         \ with an `m=`  line.\r\n2.  `Candidate`:  A single line of text representing\
         \ the ICE candidate, the format of which is consistent with the\r\n    standard\
         \ definition for ICE Candidates as defined by SDP standard.  For example:\r\
         \n    `candidate:8 1 TCP 1015022335 fe80::52d3:1968:14ec:8246 9 typ host tcptype\
         \ active`"
       operationId: RemoteRecorderAPI_WebRtcIceCandidates
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/WebRtcIceCandidates'
         required: false
       responses:
@@ -594,15 +594,15 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: postData
   /api/v1/remoteRecorderAPI/remoteRecorder/{remoteRecorderPublicId}/liveMonitoring/webRtc/sdpOffer:
     post:
       tags:
-      - RemoteRecorderAPI
+        - RemoteRecorderAPI
       summary: The client begins WebRTC session negotiation by submitting an SDP offer.
       description: "This is the next step after starting a new WebRTC connection.\
         \  The client submits an SDP offer to describe the session\r\nit hopes to\
         \ create.  After this is sent, the client should begin 2 other activities:\r\
         \n1.  The client should send ICE candidates as soon as they are known (using\
         \ another REST endpoint).\r\n2.  The client should begin polling for events\
         \ (using another REST endpoint). \r\n\r\n## SessionDescription\r\nThe SDP\
@@ -615,21 +615,21 @@
         \na=sendrecv\r\na=rtpmap:97 OPUS/48000/2\r\na=rtcp-fb:97 nack pli\r\na=fmtp:97\
         \ sprop-maxcapturerate=48000;sprop-stereo=0\r\na=ssrc:2876771208 msid:user3992408561@host-b8077b5\
         \ webrtctransceiver0\r\na=ssrc:2876771208 cname:user3992408561@host-b8077b5\r\
         \na=mid:audio0\r\na=fingerprint:sha-256 66:CD:30:01:9B:76:7E:4D:CA:F2:EF:BC:7C:61:BA:AC:AF:01:E8:72:37:92:9B:28:15:04:D8:D6:6B:0C:78:8B\r\
         \n```"
       operationId: RemoteRecorderAPI_WebRtcSdpOffer
       parameters:
-      - name: remoteRecorderPublicId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: remoteRecorderPublicId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/WebRtcSdpOfferPostData'
         required: false
       responses:
@@ -651,25 +651,25 @@
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: postData
   /api/v1/folders/{id}:
     get:
       tags:
-      - Folders
+        - Folders
       summary: Get a folder by Id
       operationId: Folders_GetFolderById
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Folder'
@@ -677,38 +677,38 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested folder was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
     put:
       tags:
-      - Folders
+        - Folders
       summary: Update a folder
       description: "Update the folders's name, description, or parent folder."
       operationId: Folders_UpdateFolderMetadata
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/FolderUpdate'
         required: false
       responses:
@@ -722,40 +722,40 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested folder was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: folderUpdate
     delete:
       tags:
-      - Folders
+        - Folders
       summary: Delete a folder
       description: Deletes a folder and all of its contents (including sessions and
         subfolders) according to the retention policy.
       operationId: Folders_DeleteFolder
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 type: string
@@ -764,77 +764,77 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested folder was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/folders/{id}/children:
     get:
       tags:
-      - Folders
+        - Folders
       summary: Get a list of child folders from the given parent
       description: "To fetch all elements, this endpoint can be called multiple times,\
         \ starting at pageNumber = 0 and incrementing the page number until no results\
         \ are returned."
       operationId: Folders_GetChildFolders
       parameters:
-      - name: id
-        in: path
-        description: "To get a list of all top level folders, use an empty GUID (00000000-0000-0000-0000-000000000000)"
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: sortField
-        in: query
-        description: '''Relevance'' is not valid for this function.'
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
-          - Relevance
+        - name: id
+          in: path
+          description: "To get a list of all top level folders, use an empty GUID (00000000-0000-0000-0000-000000000000)"
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: sortField
+          in: query
+          description: '''Relevance'' is not valid for this function.'
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/FolderSortFields'
           x-schema:
             $ref: '#/definitions/FolderSortFields'
-        x-schema:
-          $ref: '#/definitions/FolderSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfFolder'
@@ -842,71 +842,71 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/folders/{id}/sessions:
     get:
       tags:
-      - Folders
+        - Folders
       summary: Get a list of sessions in the given folder
       description: |-
         To fetch all elements, this endpoint can be called multiple times, starting at pageNumber = 0 and incrementing the page number until no results are returned.
 
         **Note:** This endpoint does not return all available properties for a session. The CreatedBy and Urls properties (except the ViewerUrl) are not returned when listing sessions in a folder. To get these properties, you can get the specific session by Id using the Sessions API.
       operationId: Folders_GetSessions
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
-          - CreatedDate
-          - Relevance
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+              - CreatedDate
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/SessionSortFields'
           x-schema:
             $ref: '#/definitions/SessionSortFields'
-        x-schema:
-          $ref: '#/definitions/SessionSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfSession'
@@ -914,77 +914,77 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/folders/{id}/sessions/search:
     get:
       tags:
-      - Folders
+        - Folders
       summary: Search for sessions within this folder
       description: |-
         To fetch all elements, this endpoint can be called multiple times, starting at pageNumber = 0 and incrementing the page number until no results are returned.
 
         **Note:** This endpoint does not return all available properties for a session. The CreatedBy and Urls properties (except the ViewerUrl) are not returned when listing sessions in a folder. To get these properties, you can get the specific session by Id using the Sessions API.
       operationId: Folders_SearchSessionsInFolder
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: searchQuery
-        in: query
-        required: true
-        schema:
-          type: string
-          nullable: true
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
-          - CreatedDate
-          - Relevance
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: searchQuery
+          in: query
+          required: true
+          schema:
+            type: string
+            nullable: true
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+              - CreatedDate
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/SessionSortFields'
           x-schema:
             $ref: '#/definitions/SessionSortFields'
-        x-schema:
-          $ref: '#/definitions/SessionSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfSession'
@@ -992,71 +992,71 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/folders/{id}/playlists:
     get:
       tags:
-      - Folders
+        - Folders
       summary: Get a list of playlists in the given folder
       description: |-
         To fetch all elements, this endpoint can be called multiple times, starting at pageNumber = 0 and incrementing the page number until no results are returned.
 
         **Note:** This endpoint does not return all available properties for a playlist. The Urls property (except the ViewerUrl) is not returned when listing playlists in a folder. To get these properties, you can get the specific playlist by Id using the Playlists API.
       operationId: Folders_GetPlaylists
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
-          - CreatedDate
-          - Relevance
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+              - CreatedDate
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/PlaylistSortFields'
           x-schema:
             $ref: '#/definitions/PlaylistSortFields'
-        x-schema:
-          $ref: '#/definitions/PlaylistSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfPlaylist'
@@ -1064,32 +1064,32 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/folders/{id}/settings/access:
     get:
       tags:
-      - Folders
+        - Folders
       summary: Get the access settings for the given folder
       operationId: Folders_GetAccessSettings
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/AccessSettings'
@@ -1097,39 +1097,39 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested folder was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
     put:
       tags:
-      - Folders
+        - Folders
       summary: Update the access settings for the given folder
       description: "If setting IsInherited to true, the access Level is ignored. Inheritance\
         \ can not be set on a top-level folder."
       operationId: Folders_UpdateAccessSettings
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/AccessSettings'
         required: false
       responses:
@@ -1143,50 +1143,50 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested folder was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: accessSettings
   /api/v1/folders/{id}/permissions:
     get:
       tags:
-      - Folders
+        - Folders
       summary: Get the user and group permissions for the given folder
       description: "To fetch all elements, this endpoint can be called multiple times,\
         \ starting at pageNumber = 0 and incrementing the page number until no results\
         \ are returned."
       operationId: Folders_GetPermissions
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfPermission'
@@ -1194,32 +1194,32 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
     post:
       tags:
-      - Folders
+        - Folders
       summary: Create a folder permission by assigning a role to a user or group
       description: This operation is only supported when access is not inherited.
       operationId: Folders_CreatePermission
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/PermissionCreate'
         required: false
       responses:
@@ -1233,79 +1233,79 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
       x-codegen-request-body-name: permissionCreate
     delete:
       tags:
-      - Folders
+        - Folders
       summary: Remove permission from the folder
       description: "This operation is only valid for non-inherited permissions. If\
         \ role type and role id are omitted, all non-inherited permissions for the\
         \ principal will be removed."
       operationId: Folders_DeletePermission
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: RoleId
-        in: query
-        description: Id of the role to remove from the user or group. Required when
-          RoleType is null or None.
-        schema:
-          type: string
-          format: guid
-          nullable: true
-      - name: RoleType
-        in: query
-        description: Type of the role to remove from the user or group. Required when
-          RoleId is null.
-        schema:
-          type: string
-          nullable: true
-          enum:
-          - None
-          - Viewer
-          - Creator
-          - Publisher
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: RoleId
+          in: query
+          description: Id of the role to remove from the user or group. Required when
+            RoleType is null or None.
+          schema:
+            type: string
+            format: guid
+            nullable: true
+        - name: RoleType
+          in: query
+          description: Type of the role to remove from the user or group. Required when
+            RoleId is null.
+          schema:
+            type: string
+            nullable: true
+            enum:
+              - None
+              - Viewer
+              - Creator
+              - Publisher
+            x-schema:
+              $ref: '#/definitions/BuiltInRoleType'
           x-schema:
             $ref: '#/definitions/BuiltInRoleType'
-        x-schema:
-          $ref: '#/definitions/BuiltInRoleType'
-      - name: PrincipalId
-        in: query
-        description: Id of the user or group from which the role is being removed.
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: PrincipalType
-        in: query
-        description: "Type of principal, either a user or group."
-        schema:
-          type: string
-          nullable: false
-          enum:
-          - User
-          - Group
+        - name: PrincipalId
+          in: query
+          description: Id of the user or group from which the role is being removed.
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: PrincipalType
+          in: query
+          description: "Type of principal, either a user or group."
+          schema:
+            type: string
+            nullable: false
+            enum:
+              - User
+              - Group
+            x-schema:
+              $ref: '#/definitions/PrincipalType'
           x-schema:
             $ref: '#/definitions/PrincipalType'
-        x-schema:
-          $ref: '#/definitions/PrincipalType'
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PermissionDelete'
@@ -1313,28 +1313,28 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested folder or share was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/folders:
     post:
       tags:
-      - Folders
+        - Folders
       summary: Create a new folder
       operationId: Folders_CreateFolder
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/FolderCreate'
@@ -1350,69 +1350,69 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
       x-codegen-request-body-name: folder
   /api/v1/folders/search:
     get:
       tags:
-      - Folders
+        - Folders
       summary: Search for folders based on a keyword
       description: "To fetch all elements, this endpoint can be called multiple times,\
         \ starting at pageNumber = 0 and incrementing the page number until no results\
         \ are returned."
       operationId: Folders_SearchForFolders
       parameters:
-      - name: searchQuery
-        in: query
-        required: true
-        schema:
-          type: string
-          nullable: true
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Relevance
-          enum:
-          - Name
-          - Relevance
+        - name: searchQuery
+          in: query
+          required: true
+          schema:
+            type: string
+            nullable: true
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Relevance
+            enum:
+              - Name
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/FolderSortFields'
           x-schema:
             $ref: '#/definitions/FolderSortFields'
-        x-schema:
-          $ref: '#/definitions/FolderSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfFolder'
@@ -1420,31 +1420,31 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/groups/search:
     get:
       tags:
-      - Groups
+        - Groups
       summary: Search for groups based on a keyword
       operationId: Groups_Search
       parameters:
-      - name: searchQuery
-        in: query
-        required: true
-        schema:
-          type: string
-          nullable: true
+        - name: searchQuery
+          in: query
+          required: true
+          schema:
+            type: string
+            nullable: true
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfGroup'
@@ -1452,32 +1452,32 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/playlists/{id}:
     get:
       tags:
-      - Playlists
+        - Playlists
       summary: Get a playlist by Id
       operationId: Playlists_GetPlaylistById
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Playlist'
@@ -1485,38 +1485,38 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested playlist was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
     put:
       tags:
-      - Playlists
+        - Playlists
       summary: Update a playlist
       description: "Update the playlist's name, description, or folder."
       operationId: Playlists_UpdatePlaylistMetadata
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/PlaylistUpdate'
         required: false
       responses:
@@ -1530,39 +1530,39 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested playlist was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: playlistUpdate
     delete:
       tags:
-      - Playlists
+        - Playlists
       summary: Delete a playlist
       description: Deletes a playlist based on the retention policies
       operationId: Playlists_DeletePlaylist
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 type: string
@@ -1571,78 +1571,78 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested playlist was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/playlists/{id}/sessions:
     get:
       tags:
-      - Playlists
+        - Playlists
       summary: Get a list of sessions in the given playlist
       description: |-
         To fetch all elements, this endpoint can be called multiple times, starting at pageNumber = 0 and incrementing the page number until no results are returned.
 
         **Note:** This endpoint does not return all available properties for a session. The CreatedBy and Urls properties (except the ViewerUrl and ThumbnailUrl) are not returned when searching for a session. To get these properties, you can get the specific session by Id.
       operationId: Playlists_GetSessionsForPlaylist
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Order
-          enum:
-          - Name
-          - CreatedDate
-          - Relevance
-          - Order
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Order
+            enum:
+              - Name
+              - CreatedDate
+              - Relevance
+              - Order
+            x-schema:
+              $ref: '#/definitions/PlaylistSessionSortFields'
           x-schema:
             $ref: '#/definitions/PlaylistSessionSortFields'
-        x-schema:
-          $ref: '#/definitions/PlaylistSessionSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfSession'
@@ -1650,34 +1650,34 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
     put:
       tags:
-      - Playlists
+        - Playlists
       summary: Add a session to a playlist
       description: "Adds the given session to a playlist. You can optionally specify\
         \ an index to insert the session at a specific position in the playlist. Otherwise,\
         \ it will be added to the end of the playlist."
       operationId: Playlists_AddSessionToPlaylist
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/PlaylistAddSession'
         required: false
       responses:
@@ -1691,23 +1691,23 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
       x-codegen-request-body-name: session
   /api/v1/playlists:
     post:
       tags:
-      - Playlists
+        - Playlists
       summary: Create a new playlist
       operationId: Playlists_CreatePlaylist
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/PlaylistCreate'
@@ -1723,71 +1723,71 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
       x-codegen-request-body-name: playlist
   /api/v1/playlists/search:
     get:
       tags:
-      - Playlists
+        - Playlists
       summary: Search for playlists based on a keyword
       description: |-
         To fetch all elements, this endpoint can be called multiple times, starting at pageNumber = 0 and incrementing the page number until no results are returned.
 
         **Note:** The Playlist Search API does not return all available properties for a playlist. The Urls property (except the ViewerUrl) is not returned when listing playlists in a folder. To get these properties, you can get the specific playlist by Id using the Playlists API.
       operationId: Playlists_SearchForPlaylists
       parameters:
-      - name: searchQuery
-        in: query
-        required: true
-        schema:
-          type: string
-          nullable: true
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
-          - CreatedDate
-          - Relevance
+        - name: searchQuery
+          in: query
+          required: true
+          schema:
+            type: string
+            nullable: true
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+              - CreatedDate
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/PlaylistSortFields'
           x-schema:
             $ref: '#/definitions/PlaylistSortFields'
-        x-schema:
-          $ref: '#/definitions/PlaylistSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfPlaylist'
@@ -1795,40 +1795,40 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/playlists/{id}/sessions/{sessionId}:
     delete:
       tags:
-      - Playlists
+        - Playlists
       summary: Remove a session from a playlist
       description: Removes the given session from a playlist.
       operationId: Playlists_RemoveSessionFromPlaylist
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: sessionId
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: sessionId
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Session'
@@ -1836,67 +1836,67 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/remoteRecorders/search:
     get:
       tags:
-      - RemoteRecorders
+        - RemoteRecorders
       summary: Search for remote recorders based on a keyword
       description: "To fetch all elements, this endpoint can be called multiple times,\
         \ starting at pageNumber = 0 and incrementing the page number until no results\
         \ are returned."
       operationId: RemoteRecorders_SearchForRemoteRecorders
       parameters:
-      - name: searchQuery
-        in: query
-        required: true
-        schema:
-          type: string
-          nullable: true
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
+        - name: searchQuery
+          in: query
+          required: true
+          schema:
+            type: string
+            nullable: true
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+            x-schema:
+              $ref: '#/definitions/RemoteRecorderSortFields'
           x-schema:
             $ref: '#/definitions/RemoteRecorderSortFields'
-        x-schema:
-          $ref: '#/definitions/RemoteRecorderSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfRemoteRecorder'
@@ -1904,32 +1904,32 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/scheduledRecordings/{id}:
     get:
       tags:
-      - ScheduledRecordings
+        - ScheduledRecordings
       summary: Get the scheduled recording information for a session
       operationId: ScheduledRecordings_GetScheduledRecordingById
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ScheduledRecording'
@@ -1937,43 +1937,43 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested scheduled entry was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
     put:
       tags:
-      - ScheduledRecordings
+        - ScheduledRecordings
       summary: Update the start or end time of a scheduled recording.
       operationId: ScheduledRecordings_UpdateScheduledRecording
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: resolveConflicts
-        in: query
-        schema:
-          type: boolean
-          nullable: false
-          default: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: resolveConflicts
+          in: query
+          schema:
+            type: boolean
+            nullable: false
+            default: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/ScheduledRecordingUpdate'
         required: false
       responses:
@@ -1987,38 +1987,38 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested scheduled entry was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: scheduledRecording
     delete:
       tags:
-      - ScheduledRecordings
+        - ScheduledRecordings
       summary: Cancel a scheduled recording
       operationId: ScheduledRecordings_CancelScheduledRecording
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 type: string
@@ -2027,37 +2027,37 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested scheduled entry was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/scheduledRecordings:
     post:
       tags:
-      - ScheduledRecordings
+        - ScheduledRecordings
       summary: Create a new scheduled recording
       operationId: ScheduledRecordings_CreateScheduledRecording
       parameters:
-      - name: resolveConflicts
-        in: query
-        required: true
-        schema:
-          type: boolean
-          nullable: false
+        - name: resolveConflicts
+          in: query
+          required: true
+          schema:
+            type: boolean
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/ScheduledRecordingCreate'
         required: false
       responses:
@@ -2071,88 +2071,88 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested scheduled entry was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: scheduledRecording
   /api/v1/searchIndexSync/updates:
     get:
       tags:
-      - SearchIndexSyncUpdates
+        - SearchIndexSyncUpdates
       summary: Get IDs for videos and playlists updated after a specified UTC date
         time
       operationId: SearchIndexSyncUpdates_GetUpdates
       parameters:
-      - name: fromDate
-        in: query
-        required: true
-        schema:
-          type: string
-          format: date-time
-          nullable: false
-      - name: nextToken
-        in: query
-        schema:
-          type: string
-          nullable: true
+        - name: fromDate
+          in: query
+          required: true
+          schema:
+            type: string
+            format: date-time
+            nullable: false
+        - name: nextToken
+          in: query
+          schema:
+            type: string
+            nullable: true
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SearchIndexSyncUpdateResponse'
   /api/v1/searchIndexSync/content:
     get:
       tags:
-      - SearchIndexSyncUpdates
+        - SearchIndexSyncUpdates
       summary: Get the content for Search Index Integration for a video or playlist
         by ID
       operationId: SearchIndexSyncUpdates_GetContent
       parameters:
-      - name: id
-        in: query
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: query
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/SearchIndexSyncContentResponse'
   /api/v1/sessions/{id}:
     get:
       tags:
-      - Sessions
+        - Sessions
       summary: Get a session by Id
       operationId: Sessions_GetSessionById
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Session'
@@ -2160,38 +2160,38 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
     put:
       tags:
-      - Sessions
+        - Sessions
       summary: Update a session
       description: "Update the session's name, description, or parent folder."
       operationId: Sessions_UpdateSessionMetadata
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/SessionUpdate'
         required: false
       responses:
@@ -2205,39 +2205,39 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: sessionUpdate
     delete:
       tags:
-      - Sessions
+        - Sessions
       summary: Delete a session
       description: Deletes a session based on the retention policies
       operationId: Sessions_DeleteSession
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 type: string
@@ -2246,83 +2246,83 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/sessions/search:
     get:
       tags:
-      - Sessions
+        - Sessions
       summary: Search for sessions based on a keyword
       description: |-
         To fetch all elements, this endpoint can be called multiple times, starting at pageNumber = 0 and incrementing the page number until no results are returned.
 
         **Note:** The Session Search API does not return all available properties for a session. The CreatedBy and Urls properties (except the ViewerUrl and ThumbnailUrl) are not returned when searching for a session. To get these properties, you can get the specific session by Id.
       operationId: Sessions_SearchForSessions
       parameters:
-      - name: searchQuery
-        in: query
-        required: true
-        schema:
-          type: string
-          nullable: true
-      - name: includeFields
-        in: query
-        description: Comma delimited list of optional fields to include in search
-          results.  Currently this is limited to 'Context'
-        schema:
-          type: string
-          nullable: true
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
-          - CreatedDate
-          - Relevance
+        - name: searchQuery
+          in: query
+          required: true
+          schema:
+            type: string
+            nullable: true
+        - name: includeFields
+          in: query
+          description: Comma delimited list of optional fields to include in search
+            results.  Currently this is limited to 'Context'
+          schema:
+            type: string
+            nullable: true
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+              - CreatedDate
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/SessionSortFields'
           x-schema:
             $ref: '#/definitions/SessionSortFields'
-        x-schema:
-          $ref: '#/definitions/SessionSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfSession'
@@ -2330,64 +2330,64 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/sessions/inProgress/webcast:
     get:
       tags:
-      - Sessions
+        - Sessions
       summary: Get a list of webcasts (live sessions) that are currently in progress.
       description: |-
         To fetch all elements, this endpoint can be called multiple times, starting at pageNumber = 0 and incrementing the page number until no results are returned.
 
         **Note:** This endpoint does not return all available properties for a session. The CreatedBy and Urls properties (except the ViewerUrl and ThumbnailUrl) are not returned when searching for a session. To get these properties, you can get the specific session by Id.
       operationId: Sessions_GetInProgressWebcasts
       parameters:
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
-          - CreatedDate
-          - Relevance
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+              - CreatedDate
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/SessionSortFields'
           x-schema:
             $ref: '#/definitions/SessionSortFields'
-        x-schema:
-          $ref: '#/definitions/SessionSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfSession'
@@ -2395,64 +2395,64 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/sessions/inProgress/recording:
     get:
       tags:
-      - Sessions
+        - Sessions
       summary: Get a list of recordings that are currently in progress.
       description: |-
         To fetch all elements, this endpoint can be called multiple times, starting at pageNumber = 0 and incrementing the page number until no results are returned.
 
         **Note:** This endpoint does not return all available properties for a session. The CreatedBy and Urls properties (except the ViewerUrl and ThumbnailUrl) are not returned when searching for a session. To get these properties, you can get the specific session by Id.
       operationId: Sessions_GetInProgressRecordings
       parameters:
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
-          - CreatedDate
-          - Relevance
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+              - CreatedDate
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/SessionSortFields'
           x-schema:
             $ref: '#/definitions/SessionSortFields'
-        x-schema:
-          $ref: '#/definitions/SessionSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfSession'
@@ -2460,42 +2460,42 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/sessions/{id}/viewers:
     get:
       tags:
-      - Sessions
+        - Sessions
       summary: Get a list of users who have viewed this session
       description: "Gets a list of all users who have viewed this session, and how\
         \ much of the session they have viewed"
       operationId: Sessions_GetSessionViewingStats
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfSessionViewerStats'
@@ -2503,67 +2503,67 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/sessions/{id}/tags:
     get:
       tags:
-      - Sessions
+        - Sessions
       summary: Get a list of tags associated with the given session
       operationId: Sessions_GetTagsForSession
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: CreateDate
-          enum:
-          - CreateDate
-          - UsageCount
-          - Content
-          - Creator
-          - MostRecentUseDate
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: CreateDate
+            enum:
+              - CreateDate
+              - UsageCount
+              - Content
+              - Creator
+              - MostRecentUseDate
+            x-schema:
+              $ref: '#/definitions/TagSortFields'
           x-schema:
             $ref: '#/definitions/TagSortFields'
-        x-schema:
-          $ref: '#/definitions/TagSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfTag'
@@ -2571,39 +2571,39 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
     put:
       tags:
-      - Sessions
+        - Sessions
       summary: Update the tags associated with the given session
       description: Replaces the tags currently associated with the session with the
         provided tags.
       operationId: Sessions_UpdateTagsForSession
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/SessionTagUpdate'
         required: false
       responses:
@@ -2617,257 +2617,257 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: tags
   /api/v1/sessions/{id}/captions:
     post:
       tags:
-      - Sessions
+        - Sessions
       summary: Upload a caption file (in SRT or VTT format) to this session
       description: "Content should be sent as 'multipart/form-data', with the caption\
         \ file attached as part of the multi-part data. This endpoint is used to upload\
         \ captions for an entire session, based off of the edited times. Please verify\
         \ that the timestamps in your caption file are correlated to the session times,\
         \ and not an individual stream."
       operationId: Sessions_UploadCaptionsToSession
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               type: object
               properties:
                 language:
                   enum:
-                  - English_USA
-                  - English_GBR
-                  - Spanish_MEX
-                  - Spanish_ESP
-                  - German
-                  - French
-                  - Dutch
-                  - Thai
-                  - Chinese_Simplified
-                  - Chinese_Traditional
-                  - Korean
-                  - Japanese
-                  - Russian
-                  - Portuguese
-                  - Polish
-                  - English_AUS
-                  - Danish
-                  - Finnish
-                  - Hungarian
-                  - Norwegian
-                  - Swedish
-                  - Italian
-                  - Welsh
-                  - Catalan
-                  - Galician
-                  - Basque
+                    - English_USA
+                    - English_GBR
+                    - Spanish_MEX
+                    - Spanish_ESP
+                    - German
+                    - French
+                    - Dutch
+                    - Thai
+                    - Chinese_Simplified
+                    - Chinese_Traditional
+                    - Korean
+                    - Japanese
+                    - Russian
+                    - Portuguese
+                    - Polish
+                    - English_AUS
+                    - Danish
+                    - Finnish
+                    - Hungarian
+                    - Norwegian
+                    - Swedish
+                    - Italian
+                    - Welsh
+                    - Catalan
+                    - Galician
+                    - Basque
       responses:
         "200":
           description: ""
-          content: {}
+          content: { }
         "400":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
     delete:
       tags:
-      - Sessions
+        - Sessions
       summary: Deletes all captions for this session
       description: This operation is not reversible. Please be very careful before
         deleting captions. They cannot be recovered once deleted.
       operationId: Sessions_DeleteSessionCaptions
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
-          content: {}
+          content: { }
         "400":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/sessions/{id}/captions/languages/{language}:
     delete:
       tags:
-      - Sessions
+        - Sessions
       summary: Deletes all captions for this session in the specified language.
       description: "This operation is not reversible. Please be very careful before\
         \ deleting captions. They cannot be recovered once deleted. To delete \"Default\"\
         \ captions, set \"null\" for the language parameter in the URL."
       operationId: Sessions_DeleteSessionCaptionsForLanguage
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: language
-        in: path
-        required: true
-        schema:
-          type: string
-          nullable: false
-          enum:
-          - English_USA
-          - English_GBR
-          - Spanish_MEX
-          - Spanish_ESP
-          - German
-          - French
-          - Dutch
-          - Thai
-          - Chinese_Simplified
-          - Chinese_Traditional
-          - Korean
-          - Japanese
-          - Russian
-          - Portuguese
-          - Polish
-          - English_AUS
-          - Danish
-          - Finnish
-          - Hungarian
-          - Norwegian
-          - Swedish
-          - Italian
-          - Welsh
-          - Catalan
-          - Galician
-          - Basque
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: language
+          in: path
+          required: true
+          schema:
+            type: string
+            nullable: false
+            enum:
+              - English_USA
+              - English_GBR
+              - Spanish_MEX
+              - Spanish_ESP
+              - German
+              - French
+              - Dutch
+              - Thai
+              - Chinese_Simplified
+              - Chinese_Traditional
+              - Korean
+              - Japanese
+              - Russian
+              - Portuguese
+              - Polish
+              - English_AUS
+              - Danish
+              - Finnish
+              - Hungarian
+              - Norwegian
+              - Swedish
+              - Italian
+              - Welsh
+              - Catalan
+              - Galician
+              - Basque
+            x-schema:
+              $ref: '#/definitions/ContentLanguage2'
           x-schema:
             $ref: '#/definitions/ContentLanguage2'
-        x-schema:
-          $ref: '#/definitions/ContentLanguage2'
-      - name: language
-        in: query
-        schema:
-          enum:
-          - English_USA
-          - English_GBR
-          - Spanish_MEX
-          - Spanish_ESP
-          - German
-          - French
-          - Dutch
-          - Thai
-          - Chinese_Simplified
-          - Chinese_Traditional
-          - Korean
-          - Japanese
-          - Russian
-          - Portuguese
-          - Polish
-          - English_AUS
-          - Danish
-          - Finnish
-          - Hungarian
-          - Norwegian
-          - Swedish
-          - Italian
-          - Welsh
-          - Catalan
-          - Galician
-          - Basque
+        - name: language
+          in: query
+          schema:
+            enum:
+              - English_USA
+              - English_GBR
+              - Spanish_MEX
+              - Spanish_ESP
+              - German
+              - French
+              - Dutch
+              - Thai
+              - Chinese_Simplified
+              - Chinese_Traditional
+              - Korean
+              - Japanese
+              - Russian
+              - Portuguese
+              - Polish
+              - English_AUS
+              - Danish
+              - Finnish
+              - Hungarian
+              - Norwegian
+              - Swedish
+              - Italian
+              - Welsh
+              - Catalan
+              - Galician
+              - Basque
       responses:
         "200":
           description: ""
-          content: {}
+          content: { }
         "400":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/sessions/{id}/settings/access:
     get:
       tags:
-      - Sessions
+        - Sessions
       summary: Get the access settings for the given session
       operationId: Sessions_GetAccessSettings
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/AccessSettings'
@@ -2875,40 +2875,40 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
     put:
       tags:
-      - Sessions
+        - Sessions
       summary: Update the access settings for the given session
       description: "IsInherited is readonly and indicates whether or not access is\
         \ being inherited from a parent folder. If AccessLevel is set to a more restrictive\
         \ value than that inherited, the inherited value will take precedence."
       operationId: Sessions_UpdateAccessSettings
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/AccessSettings'
         required: false
       responses:
@@ -2922,50 +2922,50 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: accessSettings
   /api/v1/sessions/{id}/permissions:
     get:
       tags:
-      - Sessions
+        - Sessions
       summary: Get the user and group permissions for the given session
       description: "To fetch all elements, this endpoint can be called multiple times,\
         \ starting at pageNumber = 0 and incrementing the page number until no results\
         \ are returned."
       operationId: Sessions_GetPermissions
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfPermission'
@@ -2973,31 +2973,31 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
     post:
       tags:
-      - Sessions
+        - Sessions
       summary: Create a session permission by assigning a role to a user or group
       operationId: Sessions_CreatePermission
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/PermissionCreate'
         required: false
       responses:
@@ -3011,79 +3011,79 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
       x-codegen-request-body-name: permissionCreate
     delete:
       tags:
-      - Sessions
+        - Sessions
       summary: Remove permission from the session
       description: "This operation is only valid for non-inherited permissions. If\
         \ role type and role id are omitted, all non-inherited permissions for the\
         \ principal will be removed."
       operationId: Sessions_DeletePermission
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: RoleId
-        in: query
-        description: Id of the role to remove from the user or group. Required when
-          RoleType is null or None.
-        schema:
-          type: string
-          format: guid
-          nullable: true
-      - name: RoleType
-        in: query
-        description: Type of the role to remove from the user or group. Required when
-          RoleId is null.
-        schema:
-          type: string
-          nullable: true
-          enum:
-          - None
-          - Viewer
-          - Creator
-          - Publisher
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: RoleId
+          in: query
+          description: Id of the role to remove from the user or group. Required when
+            RoleType is null or None.
+          schema:
+            type: string
+            format: guid
+            nullable: true
+        - name: RoleType
+          in: query
+          description: Type of the role to remove from the user or group. Required when
+            RoleId is null.
+          schema:
+            type: string
+            nullable: true
+            enum:
+              - None
+              - Viewer
+              - Creator
+              - Publisher
+            x-schema:
+              $ref: '#/definitions/BuiltInRoleType'
           x-schema:
             $ref: '#/definitions/BuiltInRoleType'
-        x-schema:
-          $ref: '#/definitions/BuiltInRoleType'
-      - name: PrincipalId
-        in: query
-        description: Id of the user or group from which the role is being removed.
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: PrincipalType
-        in: query
-        description: "Type of principal, either a user or group."
-        schema:
-          type: string
-          nullable: false
-          enum:
-          - User
-          - Group
+        - name: PrincipalId
+          in: query
+          description: Id of the user or group from which the role is being removed.
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: PrincipalType
+          in: query
+          description: "Type of principal, either a user or group."
+          schema:
+            type: string
+            nullable: false
+            enum:
+              - User
+              - Group
+            x-schema:
+              $ref: '#/definitions/PrincipalType'
           x-schema:
             $ref: '#/definitions/PrincipalType'
-        x-schema:
-          $ref: '#/definitions/PrincipalType'
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/PermissionDelete'
@@ -3091,145 +3091,145 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested session or permission was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/streams/{id}/captions:
     post:
       tags:
-      - Streams
+        - Streams
       summary: Upload a caption file (in SRT or VTT format) to this stream
       description: "Content should be sent as 'multipart/form-data', with the caption\
         \ file attached as part of the multi-part data. This endpoint is used to upload\
         \ captions for a single stream, and timestamps should be based on the un-edited\
         \ stream. Please verify that the timestamps in your caption file are correlated\
         \ to the unedited time for this stream."
       operationId: Streams_UploadCaptionsToStream
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               type: object
               properties:
                 language:
                   enum:
-                  - English_USA
-                  - English_GBR
-                  - Spanish_MEX
-                  - Spanish_ESP
-                  - German
-                  - French
-                  - Dutch
-                  - Thai
-                  - Chinese_Simplified
-                  - Chinese_Traditional
-                  - Korean
-                  - Japanese
-                  - Russian
-                  - Portuguese
-                  - Polish
-                  - English_AUS
-                  - Danish
-                  - Finnish
-                  - Hungarian
-                  - Norwegian
-                  - Swedish
-                  - Italian
-                  - Welsh
-                  - Catalan
-                  - Galician
-                  - Basque
+                    - English_USA
+                    - English_GBR
+                    - Spanish_MEX
+                    - Spanish_ESP
+                    - German
+                    - French
+                    - Dutch
+                    - Thai
+                    - Chinese_Simplified
+                    - Chinese_Traditional
+                    - Korean
+                    - Japanese
+                    - Russian
+                    - Portuguese
+                    - Polish
+                    - English_AUS
+                    - Danish
+                    - Finnish
+                    - Hungarian
+                    - Norwegian
+                    - Swedish
+                    - Italian
+                    - Welsh
+                    - Catalan
+                    - Galician
+                    - Basque
       responses:
         "200":
           description: ""
-          content: {}
+          content: { }
         "400":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested stream was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/tags:
     get:
       tags:
-      - Tags
+        - Tags
       summary: Get a paged list of tags.
       description: "To fetch all elements, this endpoint can be called multiple times,\
         \ starting at pageNumber = 0 and incrementing the page number until no results\
         \ are returned."
       operationId: Tags_GetTags
       parameters:
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: CreateDate
-          enum:
-          - CreateDate
-          - UsageCount
-          - Content
-          - Creator
-          - MostRecentUseDate
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: CreateDate
+            enum:
+              - CreateDate
+              - UsageCount
+              - Content
+              - Creator
+              - MostRecentUseDate
+            x-schema:
+              $ref: '#/definitions/TagSortFields'
           x-schema:
             $ref: '#/definitions/TagSortFields'
-        x-schema:
-          $ref: '#/definitions/TagSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
+        - name: pageNumber
+          in: query
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfTag'
@@ -3237,21 +3237,21 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action.
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function.
-          content: {}
+          content: { }
     post:
       tags:
-      - Tags
+        - Tags
       summary: Create a new tag.
       description: Create a new tag with the provided content.
       operationId: Tags_CreateTag
       requestBody:
         content:
           application/json:
             schema:
@@ -3268,33 +3268,33 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action.
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function.
-          content: {}
+          content: { }
       x-codegen-request-body-name: tag
   /api/v1/tags/{id}:
     get:
       tags:
-      - Tags
+        - Tags
       summary: Get a tag by ID.
       operationId: Tags_GetTagById
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/Tag'
@@ -3302,38 +3302,38 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action.
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function.
-          content: {}
+          content: { }
         "404":
           description: The requested tag was not found.
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
     put:
       tags:
-      - Tags
+        - Tags
       summary: Update a tag.
       description: Update the tag's content.
       operationId: Tags_UpdateTag
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/TagUpdate'
         required: false
       responses:
@@ -3347,39 +3347,39 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action.
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function.
-          content: {}
+          content: { }
         "404":
           description: The requested tag was not found.
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: tagUpdate
     delete:
       tags:
-      - Tags
+        - Tags
       summary: Delete a tag.
       description: Delete the tag with the given ID.
       operationId: Tags_DeleteTag
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 type: string
@@ -3388,34 +3388,34 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
   /api/v1/tags/{id}/merge:
     post:
       tags:
-      - Tags
+        - Tags
       summary: "Merge one or more tags into the tag represented by {id}."
       description: "This will delete the merged tags and update videos to reference\
         \ the tag represented by {id}."
       operationId: Tags_MergeTags
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
       requestBody:
         content:
           application/json:
             schema:
               $ref: '#/components/schemas/TagMerge'
         required: false
       responses:
@@ -3429,73 +3429,73 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested tag was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
       x-codegen-request-body-name: tagMerge
   /api/v1/users/me/sessions/viewed:
     get:
       tags:
-      - Users
+        - Users
       summary: Get a list of partially viewed sessions for the current user
       operationId: Users_GetMyViewedSessions
       parameters:
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
-          - CreatedDate
-          - Relevance
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+              - CreatedDate
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/SessionSortFields'
           x-schema:
             $ref: '#/definitions/SessionSortFields'
-        x-schema:
-          $ref: '#/definitions/SessionSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
-      - name: includeCompleted
-        in: query
-        schema:
-          type: boolean
-          nullable: false
-          default: false
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
+        - name: includeCompleted
+          in: query
+          schema:
+            type: boolean
+            nullable: false
+            default: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfSession'
@@ -3503,80 +3503,80 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested user was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/users/{id}/sessions/viewed:
     get:
       tags:
-      - Users
+        - Users
       summary: Get a list of partially viewed sessions for the specified user
       description: This endpoint can only be called by an admin
       operationId: Users_GetUsersViewedSessions
       parameters:
-      - name: id
-        in: path
-        required: true
-        schema:
-          type: string
-          format: guid
-          nullable: false
-      - name: sortField
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Name
-          enum:
-          - Name
-          - CreatedDate
-          - Relevance
+        - name: id
+          in: path
+          required: true
+          schema:
+            type: string
+            format: guid
+            nullable: false
+        - name: sortField
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Name
+            enum:
+              - Name
+              - CreatedDate
+              - Relevance
+            x-schema:
+              $ref: '#/definitions/SessionSortFields'
           x-schema:
             $ref: '#/definitions/SessionSortFields'
-        x-schema:
-          $ref: '#/definitions/SessionSortFields'
-      - name: sortOrder
-        in: query
-        schema:
-          type: string
-          nullable: false
-          default: Asc
-          enum:
-          - Asc
-          - Desc
+        - name: sortOrder
+          in: query
+          schema:
+            type: string
+            nullable: false
+            default: Asc
+            enum:
+              - Asc
+              - Desc
+            x-schema:
+              $ref: '#/definitions/SortOrder'
           x-schema:
             $ref: '#/definitions/SortOrder'
-        x-schema:
-          $ref: '#/definitions/SortOrder'
-      - name: pageNumber
-        in: query
-        description: Page numbering starts at 0
-        schema:
-          type: integer
-          format: int32
-          nullable: false
-          default: 0
-      - name: includeCompleted
-        in: query
-        schema:
-          type: boolean
-          nullable: false
-          default: false
+        - name: pageNumber
+          in: query
+          description: Page numbering starts at 0
+          schema:
+            type: integer
+            format: int32
+            nullable: false
+            default: 0
+        - name: includeCompleted
+          in: query
+          schema:
+            type: boolean
+            nullable: false
+            default: false
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfSession'
@@ -3584,37 +3584,37 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
         "404":
           description: The requested user was not found
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
   /api/v1/users/search:
     get:
       tags:
-      - Users
+        - Users
       summary: Search for users based on a keyword
       operationId: Users_Search
       parameters:
-      - name: searchQuery
-        in: query
-        required: true
-        schema:
-          type: string
-          nullable: true
+        - name: searchQuery
+          in: query
+          required: true
+          schema:
+            type: string
+            nullable: true
       responses:
         "200":
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/ListResponseOfUser'
@@ -3622,37 +3622,37 @@
           description: ""
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/APIError'
         "401":
           description: The user is not authorized to perform the requested action
-          content: {}
+          content: { }
         "403":
           description: User does not have permission to access this function
-          content: {}
+          content: { }
 components:
   schemas:
     HttpRequestMessage:
       type: object
     ExternalProviderType:
       type: string
       description: ""
       enum:
-      - Zoom
-      - Hive
-      - Kollective
-      - Webex
-      - TeamsTenant
+        - Zoom
+        - Hive
+        - Kollective
+        - Webex
+        - TeamsTenant
       x-enumNames:
-      - Zoom
-      - Hive
-      - Kollective
-      - Webex
-      - TeamsTenant
+        - Zoom
+        - Hive
+        - Kollective
+        - Webex
+        - TeamsTenant
     FindImportEligibilityAndProvisionMeetingFolderForUserDto:
       type: object
     CreateSessionForSessionGroupIdAndUserIdDto:
       type: object
     ProvisionExternalContextForSessionByExternalProviderWithPublicIdDto:
       type: object
     CreateMeetingImportStreamDto:
@@ -3667,36 +3667,36 @@
       type: object
     CreateCustomThumbnailFromUploadDto:
       type: object
     BatchAddCommentThreadsToSessionDto:
       type: object
     RemoteRecorderRegistrationResponse:
       allOf:
-      - $ref: '#/components/schemas/APIError'
-      - required:
-        - ClientKey
-        - RemoteRecorderPublicId
-        type: object
-        properties:
-          RemoteRecorderPublicId:
-            type: string
-            format: guid
-          ClientKey:
-            type: string
-            format: guid
-          ClientSecret:
-            type: string
+        - $ref: '#/components/schemas/APIError'
+        - required:
+            - ClientKey
+            - RemoteRecorderPublicId
+          type: object
+          properties:
+            RemoteRecorderPublicId:
+              type: string
+              format: guid
+            ClientKey:
+              type: string
+              format: guid
+            ClientSecret:
+              type: string
     APIError:
       type: object
       properties:
         Error:
           $ref: '#/components/schemas/APIErrorInternal'
     APIErrorInternal:
       required:
-      - Success
+        - Success
       type: object
       properties:
         ErrorCode:
           type: string
           description: Internal error code
         Message:
           type: string
@@ -3729,54 +3729,54 @@
             type: string
         Description:
           type: string
           description: Description of this remote recorder - the name presented to
             users
     RemoteRecorderHeartbeatResponse:
       allOf:
-      - $ref: '#/components/schemas/APIError'
-      - required:
-        - PingInterval
-        - ScheduleVersion
-        - SettingsVersion
-        type: object
-        properties:
-          ScheduleVersion:
-            type: string
-            format: guid
-          SettingsVersion:
-            type: string
-            format: guid
-          PingInterval:
-            type: integer
-            format: int32
-          Configuration:
-            $ref: '#/components/schemas/RemoteRecorderConfiguration'
-          RecordingSessionIsPaused:
-            type: boolean
-            description: Indicates whether the current recording (as per CurrentRecordingSessionId)
-              is in a paused state. This parameter will not be emitted if no CurrentRecordingSessionId
-              is provided.
-          LiveMonitoring:
-            $ref: '#/components/schemas/LiveMonitoringHeartbeatResponseData'
-          DefaultFolder:
-            type: string
-            format: guid
-          DefaultPrimaryQualitySettings:
-            $ref: '#/components/schemas/QualitySettings'
-          DefaultSecondaryQualitySettings:
-            $ref: '#/components/schemas/QualitySettings'
-          ExtendedConfiguration:
-            $ref: '#/components/schemas/RemoteRecorderExtendedConfiguration'
+        - $ref: '#/components/schemas/APIError'
+        - required:
+            - PingInterval
+            - ScheduleVersion
+            - SettingsVersion
+          type: object
+          properties:
+            ScheduleVersion:
+              type: string
+              format: guid
+            SettingsVersion:
+              type: string
+              format: guid
+            PingInterval:
+              type: integer
+              format: int32
+            Configuration:
+              $ref: '#/components/schemas/RemoteRecorderConfiguration'
+            RecordingSessionIsPaused:
+              type: boolean
+              description: Indicates whether the current recording (as per CurrentRecordingSessionId)
+                is in a paused state. This parameter will not be emitted if no CurrentRecordingSessionId
+                is provided.
+            LiveMonitoring:
+              $ref: '#/components/schemas/LiveMonitoringHeartbeatResponseData'
+            DefaultFolder:
+              type: string
+              format: guid
+            DefaultPrimaryQualitySettings:
+              $ref: '#/components/schemas/QualitySettings'
+            DefaultSecondaryQualitySettings:
+              $ref: '#/components/schemas/QualitySettings'
+            ExtendedConfiguration:
+              $ref: '#/components/schemas/RemoteRecorderExtendedConfiguration'
     RemoteRecorderConfiguration:
       required:
-      - CaptureScreen
-      - CaptureSlides
-      - CaptureSystemAudio
-      - HighlightMouseCursor
+        - CaptureScreen
+        - CaptureSlides
+        - CaptureSystemAudio
+        - HighlightMouseCursor
       type: object
       properties:
         PrimaryVideoDevice:
           type: string
         PrimaryAudioDevice:
           type: string
         DevicesToIgnore:
@@ -3793,37 +3793,37 @@
           type: boolean
         CaptureSystemAudio:
           type: boolean
         HighlightMouseCursor:
           type: boolean
     LiveMonitoringHeartbeatResponseData:
       required:
-      - Mode
+        - Mode
       type: object
       properties:
         Mode:
           $ref: '#/components/schemas/LiveMonitoringMode'
         Id:
           type: string
     LiveMonitoringMode:
       type: string
       description: ""
       enum:
-      - Disabled
-      - WebRtcPrimaryAudio
+        - Disabled
+        - WebRtcPrimaryAudio
       x-enumNames:
-      - Disabled
-      - WebRtcPrimaryAudio
+        - Disabled
+        - WebRtcPrimaryAudio
     QualitySettings:
       required:
-      - AudioBitrate
-      - Framerate
-      - MultipleBitrateCount
-      - PixelCount
-      - VideoBitrate
+        - AudioBitrate
+        - Framerate
+        - MultipleBitrateCount
+        - PixelCount
+        - VideoBitrate
       type: object
       properties:
         AudioBitrate:
           type: integer
           format: int32
         Framerate:
           type: integer
@@ -3835,15 +3835,15 @@
           type: integer
           format: int32
         VideoBitrate:
           type: integer
           format: int32
     RemoteRecorderExtendedConfiguration:
       required:
-      - AudioHistogramModeType
+        - AudioHistogramModeType
       type: object
       properties:
         SecondsToUseNextRecordingTemplate:
           type: number
           description: The number of seconds prior to the start of the next scheduled
             recording to apply the recording's template configurations.
           format: double
@@ -3858,26 +3858,26 @@
           format: double
         AudioHistogramModeType:
           $ref: '#/components/schemas/RemoteRecorderAudioHistogramType'
     RemoteRecorderAudioHistogramType:
       type: string
       description: ""
       enum:
-      - Automatic
-      - AlwaysStereoHistograms
-      - AlwaysMonoHistograms
+        - Automatic
+        - AlwaysStereoHistograms
+        - AlwaysMonoHistograms
       x-enumNames:
-      - Automatic
-      - AlwaysStereoHistograms
-      - AlwaysMonoHistograms
+        - Automatic
+        - AlwaysStereoHistograms
+        - AlwaysMonoHistograms
     RemoteRecorderHeartbeatData:
       required:
-      - DiskSpaceFreeMegabytes
-      - LiveMonitoringBlocked
-      - State
+        - DiskSpaceFreeMegabytes
+        - LiveMonitoringBlocked
+        - State
       type: object
       properties:
         State:
           $ref: '#/components/schemas/RemoteRecorderState'
         DiskSpaceFreeMegabytes:
           type: integer
           format: int32
@@ -3894,64 +3894,64 @@
           type: boolean
           description: "If supported, whether or not live audio monitoring is currently\
             \ blocked."
     RemoteRecorderState:
       type: string
       description: ""
       enum:
-      - Stopped
-      - Previewing
-      - Recording
-      - Paused
-      - Faulted
-      - Disconnected
-      - RecorderRunning
+        - Stopped
+        - Previewing
+        - Recording
+        - Paused
+        - Faulted
+        - Disconnected
+        - RecorderRunning
       x-enumNames:
-      - Stopped
-      - Previewing
-      - Recording
-      - Paused
-      - Faulted
-      - Disconnected
-      - RecorderRunning
+        - Stopped
+        - Previewing
+        - Recording
+        - Paused
+        - Faulted
+        - Disconnected
+        - RecorderRunning
     DeviceDescriptionWithPreview:
       type: object
       properties:
         Device:
           $ref: '#/components/schemas/Device'
         Preview:
           $ref: '#/components/schemas/RemoteRecorderDevicePreview'
     Device:
       required:
-      - Type
+        - Type
       type: object
       properties:
         DeviceId:
           type: string
         Name:
           type: string
         Type:
           $ref: '#/components/schemas/DeviceType'
     DeviceType:
       type: string
       description: ""
       enum:
-      - Unknown
-      - Audio
-      - Video
-      - AudioVideo
+        - Unknown
+        - Audio
+        - Video
+        - AudioVideo
       x-enumNames:
-      - Unknown
-      - Audio
-      - Video
-      - AudioVideo
+        - Unknown
+        - Audio
+        - Video
+        - AudioVideo
     RemoteRecorderDevicePreview:
       required:
-      - AudioFormat
-      - VideoFormat
+        - AudioFormat
+        - VideoFormat
       type: object
       properties:
         AudioFormat:
           $ref: '#/components/schemas/DeviceThumbnailFormat'
         AudioPreviewData:
           type: string
         VideoFormat:
@@ -3961,50 +3961,50 @@
         StreamID:
           type: string
           format: guid
     DeviceThumbnailFormat:
       type: string
       description: ""
       enum:
-      - None
-      - AudioHist
-      - VideoJpeg
-      - AudioHist2Channel
+        - None
+        - AudioHist
+        - VideoJpeg
+        - AudioHist2Channel
       x-enumNames:
-      - None
-      - AudioHist
-      - VideoJpeg
-      - AudioHist2Channel
+        - None
+        - AudioHist
+        - VideoJpeg
+        - AudioHist2Channel
     RemoteRecorderSchedule:
       allOf:
-      - $ref: '#/components/schemas/APIError'
-      - required:
-        - ScheduleId
-        - ServerTime
-        type: object
-        properties:
-          ScheduleId:
-            type: string
-            format: guid
-          ServerTime:
-            type: number
-            format: double
-          Recordings:
-            type: array
-            items:
-              $ref: '#/components/schemas/RemoteRecorderScheduledRecording'
+        - $ref: '#/components/schemas/APIError'
+        - required:
+            - ScheduleId
+            - ServerTime
+          type: object
+          properties:
+            ScheduleId:
+              type: string
+              format: guid
+            ServerTime:
+              type: number
+              format: double
+            Recordings:
+              type: array
+              items:
+                $ref: '#/components/schemas/RemoteRecorderScheduledRecording'
     RemoteRecorderScheduledRecording:
       required:
-      - EndTime
-      - FolderId
-      - IsBroadcast
-      - SessionId
-      - StartTime
-      - SuppressPrimaryDevices
-      - SuppressSecondaryDevices
+        - EndTime
+        - FolderId
+        - IsBroadcast
+        - SessionId
+        - StartTime
+        - SuppressPrimaryDevices
+        - SuppressSecondaryDevices
       type: object
       properties:
         Id:
           type: string
           format: guid
         SessionId:
           type: string
@@ -4035,17 +4035,17 @@
           $ref: '#/components/schemas/QualitySettings'
         SecondaryQualitySettings:
           $ref: '#/components/schemas/QualitySettings'
         Configuration:
           $ref: '#/components/schemas/RemoteRecorderConfiguration'
     RemoteRecorderError:
       required:
-      - ErrorCode
-      - ErrorType
-      - Severity
+        - ErrorCode
+        - ErrorType
+        - Severity
       type: object
       properties:
         Severity:
           $ref: '#/components/schemas/RemoteRecorderErrorSeverity'
         ErrorType:
           $ref: '#/components/schemas/RemoteRecorderErrorType'
         ErrorCode:
@@ -4059,50 +4059,50 @@
           type: string
           description: "If this error is associated with a session, which session"
           format: guid
     RemoteRecorderErrorSeverity:
       type: string
       description: ""
       enum:
-      - Invalid
-      - Critical
-      - Error
-      - Warning
+        - Invalid
+        - Critical
+        - Error
+        - Warning
       x-enumNames:
-      - Invalid
-      - Critical
-      - Error
-      - Warning
+        - Invalid
+        - Critical
+        - Error
+        - Warning
     RemoteRecorderErrorType:
       type: string
       description: ""
       enum:
-      - Invalid
-      - General
-      - Device
-      - Network
-      - Storage
+        - Invalid
+        - General
+        - Device
+        - Network
+        - Storage
       x-enumNames:
-      - Invalid
-      - General
-      - Device
-      - Network
-      - Storage
+        - Invalid
+        - General
+        - Device
+        - Network
+        - Storage
     RemoteRecorderPauseRecordingRequest:
       required:
-      - PauseRecordingTime
+        - PauseRecordingTime
       type: object
       properties:
         PauseRecordingTime:
           type: number
           description: Pause recording time in UTC file time seconds
           format: double
     RemoteRecorderResumeRecordingRequest:
       required:
-      - ResumeRecordingTime
+        - ResumeRecordingTime
       type: object
       properties:
         ResumeRecordingTime:
           type: number
           description: Resume recording time in UTC file time seconds
           format: double
     RemoteRecorderURLsUpdateRequest:
@@ -4110,125 +4110,125 @@
       properties:
         URLs:
           type: array
           items:
             $ref: '#/components/schemas/RemoteRecorderURL'
     RemoteRecorderURL:
       required:
-      - URLType
+        - URLType
       type: object
       properties:
         URLType:
           $ref: '#/components/schemas/RemoteRecorderURLType'
         URL:
           type: string
           description: Must be a well formed URL
     RemoteRecorderURLType:
       type: string
       description: ""
       enum:
-      - Management
-      - PrimaryPreview
-      - SecondaryPreview
-      - Support
-      - SecondaryPreview2
-      - SecondaryPreview3
-      - SecondaryPreview4
+        - Management
+        - PrimaryPreview
+        - SecondaryPreview
+        - Support
+        - SecondaryPreview2
+        - SecondaryPreview3
+        - SecondaryPreview4
       x-enumNames:
-      - Management
-      - PrimaryPreview
-      - SecondaryPreview
-      - Support
-      - SecondaryPreview2
-      - SecondaryPreview3
-      - SecondaryPreview4
+        - Management
+        - PrimaryPreview
+        - SecondaryPreview
+        - Support
+        - SecondaryPreview2
+        - SecondaryPreview3
+        - SecondaryPreview4
     WebRtcConnectPostData:
       required:
-      - OperationType
+        - OperationType
       type: object
       properties:
         OperationType:
           $ref: '#/components/schemas/WebRtcConnectOperationType'
     WebRtcConnectOperationType:
       type: string
       description: ""
       enum:
-      - Unknown
-      - Initialize
+        - Unknown
+        - Initialize
       x-enumNames:
-      - Unknown
-      - Initialize
+        - Unknown
+        - Initialize
     WebRtcDisconnectPostData:
       required:
-      - OperationType
+        - OperationType
       type: object
       properties:
         OperationType:
           $ref: '#/components/schemas/WebRtcDisconnectOperationType'
     WebRtcDisconnectOperationType:
       type: string
       description: ""
       enum:
-      - Unknown
-      - Destroy
+        - Unknown
+        - Destroy
       x-enumNames:
-      - Unknown
-      - Destroy
+        - Unknown
+        - Destroy
     WebRtcEventsResponse:
       allOf:
-      - $ref: '#/components/schemas/APIError'
-      - required:
-        - PingFastInterval
-        - PingSlowInterval
-        type: object
-        properties:
-          Events:
-            type: array
-            items:
-              $ref: '#/components/schemas/WebRtcEvent'
-          PingFastInterval:
-            type: integer
-            format: int32
-          PingSlowInterval:
-            type: integer
-            format: int32
+        - $ref: '#/components/schemas/APIError'
+        - required:
+            - PingFastInterval
+            - PingSlowInterval
+          type: object
+          properties:
+            Events:
+              type: array
+              items:
+                $ref: '#/components/schemas/WebRtcEvent'
+            PingFastInterval:
+              type: integer
+              format: int32
+            PingSlowInterval:
+              type: integer
+              format: int32
     WebRtcEvent:
       required:
-      - EventType
+        - EventType
       type: object
       properties:
         EventType:
           $ref: '#/components/schemas/WebRtcEventType'
         Payload:
           type: string
     WebRtcEventType:
       type: string
       description: ""
       enum:
-      - Unknown
-      - IceCandidate
-      - SdpAnswer
-      - TemporaryFailure
-      - PermanentFailure
+        - Unknown
+        - IceCandidate
+        - SdpAnswer
+        - TemporaryFailure
+        - PermanentFailure
       x-enumNames:
-      - Unknown
-      - IceCandidate
-      - SdpAnswer
-      - TemporaryFailure
-      - PermanentFailure
+        - Unknown
+        - IceCandidate
+        - SdpAnswer
+        - TemporaryFailure
+        - PermanentFailure
     WebRtcIceCandidates:
       type: object
       properties:
         Candidates:
           type: array
           items:
             $ref: '#/components/schemas/WebRtcIceCandidate'
     WebRtcIceCandidate:
       required:
-      - Index
+        - Index
       type: object
       properties:
         Candidate:
           type: string
         Index:
           type: integer
     WebRtcSdpOfferPostData:
@@ -4281,39 +4281,39 @@
           description: The list of results from the API call
           items:
             $ref: '#/components/schemas/Folder'
     FolderSortFields:
       type: string
       description: ""
       enum:
-      - Name
-      - Relevance
+        - Name
+        - Relevance
       x-enumNames:
-      - Name
-      - Relevance
+        - Name
+        - Relevance
     SortOrder:
       type: string
       description: ""
       enum:
-      - Asc
-      - Desc
+        - Asc
+        - Desc
       x-enumNames:
-      - Asc
-      - Desc
+        - Asc
+        - Desc
     ListResponseOfSession:
       type: object
       properties:
         Results:
           type: array
           description: The list of results from the API call
           items:
             $ref: '#/components/schemas/Session'
     Session:
       required:
-      - Folder
+        - Folder
       type: object
       properties:
         Id:
           type: string
           format: guid
         Name:
           type: string
@@ -4345,15 +4345,15 @@
         PercentCompleted:
           type: integer
           description: The percentage from 0-100 of the session watched by the requested
             user
           format: int32
     User:
       required:
-      - Id
+        - Id
       type: object
       properties:
         Id:
           type: string
           description: The id of the user.
           format: guid
         Username:
@@ -4394,40 +4394,40 @@
           format: double
         ThumbnailUrl:
           type: string
     SessionSortFields:
       type: string
       description: ""
       enum:
-      - Name
-      - CreatedDate
-      - Relevance
+        - Name
+        - CreatedDate
+        - Relevance
       x-enumNames:
-      - Name
-      - CreatedDate
-      - Relevance
+        - Name
+        - CreatedDate
+        - Relevance
     ListResponseOfPlaylist:
       type: object
       properties:
         Results:
           type: array
           description: The list of results from the API call
           items:
             $ref: '#/components/schemas/Playlist'
     Playlist:
       allOf:
-      - $ref: '#/components/schemas/ModelBaseOfGuid'
-      - type: object
-        properties:
-          Description:
-            type: string
-          Folder:
-            $ref: '#/components/schemas/BasicFolder'
-          Urls:
-            $ref: '#/components/schemas/PlaylistUrls'
+        - $ref: '#/components/schemas/ModelBaseOfGuid'
+        - type: object
+          properties:
+            Description:
+              type: string
+            Folder:
+              $ref: '#/components/schemas/BasicFolder'
+            Urls:
+              $ref: '#/components/schemas/PlaylistUrls'
     PlaylistUrls:
       type: object
       properties:
         ViewerUrl:
           type: string
           description: The URL to view this playlist in Panopto
         EmbedUrl:
@@ -4444,101 +4444,101 @@
           format: guid
         Name:
           type: string
     PlaylistSortFields:
       type: string
       description: ""
       enum:
-      - Name
-      - CreatedDate
-      - Relevance
+        - Name
+        - CreatedDate
+        - Relevance
       x-enumNames:
-      - Name
-      - CreatedDate
-      - Relevance
+        - Name
+        - CreatedDate
+        - Relevance
     AccessSettings:
       required:
-      - IsInherited
-      - Level
+        - IsInherited
+        - Level
       type: object
       properties:
         IsInherited:
           type: boolean
           description: Indicates whether or not the access settings are inherited.
         Level:
           $ref: '#/components/schemas/AccessLevel'
     AccessLevel:
       type: string
       description: ""
       enum:
-      - Restricted
-      - OrganizationUnlisted
-      - Organization
-      - PublicUnlisted
-      - Public
+        - Restricted
+        - OrganizationUnlisted
+        - Organization
+        - PublicUnlisted
+        - Public
       x-enumNames:
-      - Restricted
-      - OrganizationUnlisted
-      - Organization
-      - PublicUnlisted
-      - Public
+        - Restricted
+        - OrganizationUnlisted
+        - Organization
+        - PublicUnlisted
+        - Public
     ListResponseOfPermission:
       type: object
       properties:
         Results:
           type: array
           description: The list of results from the API call
           items:
             $ref: '#/components/schemas/Permission'
     Permission:
       required:
-      - IsInherited
+        - IsInherited
       type: object
       properties:
         IsInherited:
           type: boolean
           description: Indicates whether or not the permission is inherited.
         Principal:
           $ref: '#/components/schemas/Principal'
         Role:
           $ref: '#/components/schemas/Role'
     Principal:
       required:
-      - Type
+        - Type
       type: object
       properties:
         Id:
           type: string
           description: The unique id that represents this principal.
           format: guid
         Type:
           $ref: '#/components/schemas/PrincipalType'
     PrincipalType:
       type: string
       description: ""
       enum:
-      - User
-      - Group
+        - User
+        - Group
       x-enumNames:
-      - User
-      - Group
+        - User
+        - Group
     Role:
       type: object
       properties:
         Id:
           type: string
           description: The unique id that identifies the role.
           format: guid
         Name:
           type: string
           description: The name of this role.
     PermissionCreate:
       required:
-      - PrincipalId
-      - PrincipalType
+        - PrincipalId
+        - PrincipalType
       type: object
       properties:
         RoleId:
           type: string
           description: Id of the role to assign to the user or group. Required when
             RoleType is null or None.
           format: guid
@@ -4550,27 +4550,27 @@
           format: guid
         PrincipalType:
           $ref: '#/components/schemas/PrincipalType'
     BuiltInRoleType:
       type: string
       description: ""
       enum:
-      - None
-      - Viewer
-      - Creator
-      - Publisher
+        - None
+        - Viewer
+        - Creator
+        - Publisher
       x-enumNames:
-      - None
-      - Viewer
-      - Creator
-      - Publisher
+        - None
+        - Viewer
+        - Creator
+        - Publisher
     PermissionDelete:
       required:
-      - PrincipalId
-      - PrincipalType
+        - PrincipalId
+        - PrincipalType
       type: object
       properties:
         RoleId:
           type: string
           description: Id of the role to remove from the user or group. Required when
             RoleType is null or None.
           format: guid
@@ -4618,16 +4618,16 @@
         Results:
           type: array
           description: The list of results from the API call
           items:
             $ref: '#/components/schemas/Group'
     Group:
       allOf:
-      - $ref: '#/components/schemas/ModelBaseOfGuid'
-      - type: object
+        - $ref: '#/components/schemas/ModelBaseOfGuid'
+        - type: object
     PlaylistUpdate:
       type: object
       properties:
         Name:
           type: string
           description: The new name for the playlist.
         Description:
@@ -4637,26 +4637,26 @@
           type: string
           description: The id of the folder to move this playlist to.
           format: guid
     PlaylistSessionSortFields:
       type: string
       description: ""
       enum:
-      - Name
-      - CreatedDate
-      - Relevance
-      - Order
+        - Name
+        - CreatedDate
+        - Relevance
+        - Order
       x-enumNames:
-      - Name
-      - CreatedDate
-      - Relevance
-      - Order
+        - Name
+        - CreatedDate
+        - Relevance
+        - Order
     PlaylistCreate:
       required:
-      - FolderId
+        - FolderId
       type: object
       properties:
         Name:
           type: string
           description: The name of the playlist.
         Description:
           type: string
@@ -4670,15 +4670,15 @@
           description: A list of session IDs to add to this playlist. They will be
             added in order.
           items:
             type: string
             format: guid
     PlaylistAddSession:
       required:
-      - SessionId
+        - SessionId
       type: object
       properties:
         SessionId:
           type: string
           description: The id of the session to add to this playlist.
           format: guid
         Index:
@@ -4693,15 +4693,15 @@
         Results:
           type: array
           description: The list of results from the API call
           items:
             $ref: '#/components/schemas/RemoteRecorder'
     RemoteRecorder:
       required:
-      - State
+        - State
       type: object
       properties:
         Id:
           type: string
           format: guid
         Name:
           type: string
@@ -4709,17 +4709,17 @@
           $ref: '#/components/schemas/RemoteRecorderState'
         DefaultRecordingFolder:
           $ref: '#/components/schemas/BasicFolder'
     RemoteRecorderSortFields:
       type: string
       description: ""
       enum:
-      - Name
+        - Name
       x-enumNames:
-      - Name
+        - Name
     ScheduledRecording:
       type: object
       properties:
         Id:
           type: string
           format: guid
         Name:
@@ -4735,17 +4735,17 @@
           format: date-time
         EndTime:
           type: string
           description: The end time for the recording
           format: date-time
     RecorderScheduleEntry:
       required:
-      - RecorderId
-      - SuppressPrimaryCapture
-      - SuppressSecondaryCapture
+        - RecorderId
+        - SuppressPrimaryCapture
+        - SuppressSecondaryCapture
       type: object
       properties:
         Id:
           type: string
           format: guid
         Name:
           type: string
@@ -4769,18 +4769,18 @@
         EndTime:
           type: string
           description: The new end time. Times should be UTC. Must be later than the
             current time
           format: date-time
     ScheduledRecordingCreate:
       required:
-      - EndTime
-      - FolderId
-      - IsBroadcast
-      - StartTime
+        - EndTime
+        - FolderId
+        - IsBroadcast
+        - StartTime
       type: object
       properties:
         Name:
           type: string
           description: The name of the scheduled recording.
         Description:
           type: string
@@ -4804,17 +4804,17 @@
             $ref: '#/components/schemas/ScheduledRecordingRemoteRecorder'
         IsBroadcast:
           type: boolean
           description: Set to true if this recording should be broadcast live when
             it starts.
     ScheduledRecordingRemoteRecorder:
       required:
-      - RemoteRecorderId
-      - SuppressPrimary
-      - SuppressSecondary
+        - RemoteRecorderId
+        - SuppressPrimary
+        - SuppressSecondary
       type: object
       properties:
         RemoteRecorderId:
           type: string
           description: The id of the remote recorder to use for this recording. Only
             one can be specified at this time.
           format: guid
@@ -4825,30 +4825,30 @@
             stream.
         SuppressSecondary:
           type: boolean
           description: True if the secondary stream should be suppressed from this
             recorder.
     SearchIndexSyncUpdateResponse:
       allOf:
-      - $ref: '#/components/schemas/ModelBase'
-      - type: object
+        - $ref: '#/components/schemas/ModelBase'
+        - type: object
     ModelBase:
       type: object
       properties:
         Id:
           type: string
           description: The unique identifier for this item.
           format: guid
         Name:
           type: string
           description: The name of this item.
     SearchIndexSyncContentResponse:
       allOf:
-      - $ref: '#/components/schemas/ModelBase'
-      - type: object
+        - $ref: '#/components/schemas/ModelBase'
+        - type: object
     SessionUpdate:
       type: object
       properties:
         Name:
           type: string
           description: The new name for the session.
         Description:
@@ -4864,15 +4864,15 @@
         Results:
           type: array
           description: The list of results from the API call
           items:
             $ref: '#/components/schemas/SessionViewerStats'
     SessionViewerStats:
       required:
-      - LastViewedDateTime
+        - LastViewedDateTime
       type: object
       properties:
         User:
           $ref: '#/components/schemas/User'
         PercentCompleted:
           type: number
           format: double
@@ -4890,16 +4890,16 @@
         Results:
           type: array
           description: The list of results from the API call
           items:
             $ref: '#/components/schemas/Tag'
     Tag:
       required:
-      - CreateDate
-      - UsageCount
+        - CreateDate
+        - UsageCount
       type: object
       properties:
         Id:
           type: string
           format: guid
         Content:
           type: string
@@ -4914,25 +4914,25 @@
           format: date-time
         CreatedBy:
           $ref: '#/components/schemas/User'
     TagSortFields:
       type: string
       description: ""
       enum:
-      - CreateDate
-      - UsageCount
-      - Content
-      - Creator
-      - MostRecentUseDate
+        - CreateDate
+        - UsageCount
+        - Content
+        - Creator
+        - MostRecentUseDate
       x-enumNames:
-      - CreateDate
-      - UsageCount
-      - Content
-      - Creator
-      - MostRecentUseDate
+        - CreateDate
+        - UsageCount
+        - Content
+        - Creator
+        - MostRecentUseDate
     SessionTagUpdate:
       type: object
       properties:
         Tags:
           type: array
           description: The tags for the session.
           items:
@@ -4943,139 +4943,139 @@
       description: "Language of a content (i.e. session, potentially stream or per-language\
         \ captions).\nThis can be set per site initially, and will be expaneded to\
         \ per folder and/or per session.\nThis is used by search, ASR, OCR, and potentially\
         \ human transcription features.\nEnumDescription attribute is used by site\
         \ config UI, and may be used by other UI.\n            \nContentLanguage.ts\
         \ should stay in sync with this enum"
       enum:
-      - English_USA
-      - English_GBR
-      - Spanish_MEX
-      - Spanish_ESP
-      - German
-      - French
-      - Dutch
-      - Thai
-      - Chinese_Simplified
-      - Chinese_Traditional
-      - Korean
-      - Japanese
-      - Russian
-      - Portuguese
-      - Polish
-      - English_AUS
-      - Danish
-      - Finnish
-      - Hungarian
-      - Norwegian
-      - Swedish
-      - Italian
-      - Welsh
-      - Catalan
-      - Galician
-      - Basque
+        - English_USA
+        - English_GBR
+        - Spanish_MEX
+        - Spanish_ESP
+        - German
+        - French
+        - Dutch
+        - Thai
+        - Chinese_Simplified
+        - Chinese_Traditional
+        - Korean
+        - Japanese
+        - Russian
+        - Portuguese
+        - Polish
+        - English_AUS
+        - Danish
+        - Finnish
+        - Hungarian
+        - Norwegian
+        - Swedish
+        - Italian
+        - Welsh
+        - Catalan
+        - Galician
+        - Basque
       x-enumNames:
-      - English_USA
-      - English_GBR
-      - Spanish_MEX
-      - Spanish_ESP
-      - German
-      - French
-      - Dutch
-      - Thai
-      - Chinese_Simplified
-      - Chinese_Traditional
-      - Korean
-      - Japanese
-      - Russian
-      - Portuguese
-      - Polish
-      - English_AUS
-      - Danish
-      - Finnish
-      - Hungarian
-      - Norwegian
-      - Swedish
-      - Italian
-      - Welsh
-      - Catalan
-      - Galician
-      - Basque
+        - English_USA
+        - English_GBR
+        - Spanish_MEX
+        - Spanish_ESP
+        - German
+        - French
+        - Dutch
+        - Thai
+        - Chinese_Simplified
+        - Chinese_Traditional
+        - Korean
+        - Japanese
+        - Russian
+        - Portuguese
+        - Polish
+        - English_AUS
+        - Danish
+        - Finnish
+        - Hungarian
+        - Norwegian
+        - Swedish
+        - Italian
+        - Welsh
+        - Catalan
+        - Galician
+        - Basque
     ContentLanguage2:
       type: string
       description: "Language of a content (i.e. session, potentially stream or per-language\
         \ captions).\nThis can be set per site initially, and will be expaneded to\
         \ per folder and/or per session.\nThis is used by search, ASR, OCR, and potentially\
         \ human transcription features.\nEnumDescription attribute is used by site\
         \ config UI, and may be used by other UI.\n            \nContentLanguage.ts\
         \ should stay in sync with this enum"
       enum:
-      - English_USA
-      - English_GBR
-      - Spanish_MEX
-      - Spanish_ESP
-      - German
-      - French
-      - Dutch
-      - Thai
-      - Chinese_Simplified
-      - Chinese_Traditional
-      - Korean
-      - Japanese
-      - Russian
-      - Portuguese
-      - Polish
-      - English_AUS
-      - Danish
-      - Finnish
-      - Hungarian
-      - Norwegian
-      - Swedish
-      - Italian
-      - Welsh
-      - Catalan
-      - Galician
-      - Basque
+        - English_USA
+        - English_GBR
+        - Spanish_MEX
+        - Spanish_ESP
+        - German
+        - French
+        - Dutch
+        - Thai
+        - Chinese_Simplified
+        - Chinese_Traditional
+        - Korean
+        - Japanese
+        - Russian
+        - Portuguese
+        - Polish
+        - English_AUS
+        - Danish
+        - Finnish
+        - Hungarian
+        - Norwegian
+        - Swedish
+        - Italian
+        - Welsh
+        - Catalan
+        - Galician
+        - Basque
       x-enumNames:
-      - English_USA
-      - English_GBR
-      - Spanish_MEX
-      - Spanish_ESP
-      - German
-      - French
-      - Dutch
-      - Thai
-      - Chinese_Simplified
-      - Chinese_Traditional
-      - Korean
-      - Japanese
-      - Russian
-      - Portuguese
-      - Polish
-      - English_AUS
-      - Danish
-      - Finnish
-      - Hungarian
-      - Norwegian
-      - Swedish
-      - Italian
-      - Welsh
-      - Catalan
-      - Galician
-      - Basque
+        - English_USA
+        - English_GBR
+        - Spanish_MEX
+        - Spanish_ESP
+        - German
+        - French
+        - Dutch
+        - Thai
+        - Chinese_Simplified
+        - Chinese_Traditional
+        - Korean
+        - Japanese
+        - Russian
+        - Portuguese
+        - Polish
+        - English_AUS
+        - Danish
+        - Finnish
+        - Hungarian
+        - Norwegian
+        - Swedish
+        - Italian
+        - Welsh
+        - Catalan
+        - Galician
+        - Basque
     TagCreate:
       type: object
       properties:
         Content:
           type: string
           description: The content of the tag.
     TagUpdate:
       allOf:
-      - $ref: '#/components/schemas/TagCreate'
-      - type: object
+        - $ref: '#/components/schemas/TagCreate'
+        - type: object
     TagMerge:
       type: object
       properties:
         TagIdsToMerge:
           type: array
           description: The IDs of the tags that should be merged and then deleted.
           items:
```

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/panopto_authenticator.py` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_authenticator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,9 @@
         self._canvas_client = canvas_client
 
     def _detect_if_authentication_is_needed(self, response: Response) -> bool:
         auth_cookie = ".ASPXAUTH"
         return auth_cookie not in response.cookies.keys() or response.cookies.get(auth_cookie) == ""
 
     async def _authenticate(self):
-        await self._canvas_client.authenticate_to_panopto(self._panopto_api_config.get_endpoint("/Panopto/Pages/Auth/Login.aspx?instance=Canvas&AllowBounce=true"))
-
-
-
-
-
+        await self._canvas_client.authenticate_to_panopto(
+            self._panopto_api_config.get_endpoint("/Panopto/Pages/Auth/Login.aspx?instance=Canvas&AllowBounce=true"))
```

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/panopto_client.py` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import asyncio
-import json
 from typing import Optional
 
 from httpx import Response, URL, Request
+from tenacity import retry, wait_exponential, wait_random, stop_after_attempt, retry_if_exception_type
 
 from qcanvas_api_clients.canvas.canvas_client import CanvasClient
 from qcanvas_api_clients.panopto.panopto_api_config import PanoptoApiConfig
 from qcanvas_api_clients.panopto.panopto_authenticator import PanoptoAuthenticator
-from tenacity import retry, wait_exponential, wait_random, stop_after_attempt, retry_if_exception_type
-
 from qcanvas_api_clients.util.request_exceptions import RatelimitedError
 
+
 # todo unfinished
 
 class PanoptoClient:
     def __init__(self, panopto_api_config: PanoptoApiConfig, canvas_client: CanvasClient,
                  max_concurrent_operations: int = 20):
         self._api_config = panopto_api_config
         self._canvas_client = canvas_client
```

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/panopto/panopto_types.py` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/panopto/panopto_types.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/__pycache__/custom_httpx_async_transport.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/custom_httpx_async_transport.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/__pycache__/generic_authenticator.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/generic_authenticator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/__pycache__/request_exceptions.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/request_exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/__pycache__/url_converter.cpython-311.pyc` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/__pycache__/url_converter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/custom_httpx_async_transport.py` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/custom_httpx_async_transport.py`

 * *Files identical despite different names*

### Comparing `qcanvas_api_clients-0.1.0/qcanvas_api_clients/util/generic_authenticator.py` & `qcanvas_api_clients-0.1.1a0/qcanvas_api_clients/util/generic_authenticator.py`

 * *Files identical despite different names*

