# Comparing `tmp/fal_client-0.2.2.tar.gz` & `tmp/fal_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_client-0.2.2.tar", last modified: Sat Apr  6 16:39:21 2024, max compression
+gzip compressed data, was "fal_client-0.3.0.tar", last modified: Fri Apr 19 21:20:56 2024, max compression
```

## Comparing `fal_client-0.2.2.tar` & `fal_client-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-06 16:39:21.436859 fal_client-0.2.2/
--rw-r--r--   0 isidentical   (501) staff       (20)     2584 2024-04-06 16:39:21.436547 fal_client-0.2.2/PKG-INFO
--rw-r--r--   0 isidentical   (501) staff       (20)     2243 2024-04-06 16:25:46.000000 fal_client-0.2.2/README.md
--rw-r--r--   0 isidentical   (501) staff       (20)      634 2024-04-06 16:32:44.000000 fal_client-0.2.2/pyproject.toml
--rw-r--r--   0 isidentical   (501) staff       (20)       38 2024-04-06 16:39:21.436917 fal_client-0.2.2/setup.cfg
-drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-06 16:39:21.432328 fal_client-0.2.2/src/
-drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-06 16:39:21.434215 fal_client-0.2.2/src/fal_client/
--rw-r--r--   0 isidentical   (501) staff       (20)      899 2024-04-06 05:04:12.000000 fal_client-0.2.2/src/fal_client/__init__.py
--rw-r--r--   0 isidentical   (501) staff       (20)      565 2024-04-05 17:23:39.000000 fal_client-0.2.2/src/fal_client/auth.py
--rw-r--r--   0 isidentical   (501) staff       (20)    13864 2024-04-06 16:30:33.000000 fal_client-0.2.2/src/fal_client/client.py
--rw-r--r--   0 isidentical   (501) staff       (20)        0 2024-04-05 17:23:39.000000 fal_client-0.2.2/src/fal_client/py.typed
-drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-06 16:39:21.436226 fal_client-0.2.2/src/fal_client.egg-info/
--rw-r--r--   0 isidentical   (501) staff       (20)     2584 2024-04-06 16:39:21.000000 fal_client-0.2.2/src/fal_client.egg-info/PKG-INFO
--rw-r--r--   0 isidentical   (501) staff       (20)      365 2024-04-06 16:39:21.000000 fal_client-0.2.2/src/fal_client.egg-info/SOURCES.txt
--rw-r--r--   0 isidentical   (501) staff       (20)        1 2024-04-06 16:39:21.000000 fal_client-0.2.2/src/fal_client.egg-info/dependency_links.txt
--rw-r--r--   0 isidentical   (501) staff       (20)       39 2024-04-06 16:39:21.000000 fal_client-0.2.2/src/fal_client.egg-info/requires.txt
--rw-r--r--   0 isidentical   (501) staff       (20)       11 2024-04-06 16:39:21.000000 fal_client-0.2.2/src/fal_client.egg-info/top_level.txt
-drwxr-xr-x   0 isidentical   (501) staff       (20)        0 2024-04-06 16:39:21.435914 fal_client-0.2.2/tests/
--rw-r--r--   0 isidentical   (501) staff       (20)     2465 2024-04-05 20:26:54.000000 fal_client-0.2.2/tests/test_async_client.py
--rw-r--r--   0 isidentical   (501) staff       (20)     2219 2024-04-05 20:26:54.000000 fal_client-0.2.2/tests/test_sync_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:56.222720 fal_client-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-19 21:20:56.222720 fal_client-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 21:20:49.000000 fal_client-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-19 21:20:49.000000 fal_client-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:20:56.222720 fal_client-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:56.222720 fal_client-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:56.222720 fal_client-0.3.0/src/fal_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-19 21:20:49.000000 fal_client-0.3.0/src/fal_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-19 21:20:49.000000 fal_client-0.3.0/src/fal_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14789 2024-04-19 21:20:49.000000 fal_client-0.3.0/src/fal_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:49.000000 fal_client-0.3.0/src/fal_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:56.222720 fal_client-0.3.0/src/fal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-19 21:20:56.000000 fal_client-0.3.0/src/fal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 21:20:56.000000 fal_client-0.3.0/src/fal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:20:56.000000 fal_client-0.3.0/src/fal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 21:20:56.000000 fal_client-0.3.0/src/fal_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 21:20:56.000000 fal_client-0.3.0/src/fal_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:56.222720 fal_client-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-19 21:20:49.000000 fal_client-0.3.0/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-19 21:20:49.000000 fal_client-0.3.0/tests/test_sync_client.py
```

### Comparing `fal_client-0.2.2/PKG-INFO` & `fal_client-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal_client
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python client for fal.ai
 Author: fal <hello@fal.ai>
 Project-URL: homepage, https://fal.ai
 Project-URL: repository, https://github.com/fal-ai/fal
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx<1,>=0.21.0
@@ -62,14 +62,26 @@
 import fal_client
 
 audio_url = fal_client.upload_file("path/to/audio.wav")
 response = fal_client.run("fal-ai/whisper", arguments={"audio_url": audio_url})
 print(response["text"])
 ```
 
+## Encoding files as in-memory data URLs
+
+If you don't want to upload your file to our CDN service (for latency reasons, for example), you can encode it as a data URL and pass it directly to the client. Here's an example:
+
+```python
+import fal_client
+
+audio_data_url = fal_client.encode_file("path/to/audio.wav")
+response = fal_client.run("fal-ai/whisper", arguments={"audio_url": audio_data_url})
+print(response["text"])
+```
+
 ## Queuing requests
 
 When you want to send a request and keep receiving updates on its status, you can use the `submit` method. Here's an example:
 
 ```python
 import asyncio
 import fal_client
```

### Comparing `fal_client-0.2.2/README.md` & `fal_client-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,26 @@
 import fal_client
 
 audio_url = fal_client.upload_file("path/to/audio.wav")
 response = fal_client.run("fal-ai/whisper", arguments={"audio_url": audio_url})
 print(response["text"])
 ```
 
+## Encoding files as in-memory data URLs
+
+If you don't want to upload your file to our CDN service (for latency reasons, for example), you can encode it as a data URL and pass it directly to the client. Here's an example:
+
+```python
+import fal_client
+
+audio_data_url = fal_client.encode_file("path/to/audio.wav")
+response = fal_client.run("fal-ai/whisper", arguments={"audio_url": audio_data_url})
+print(response["text"])
+```
+
 ## Queuing requests
 
 When you want to send a request and keep receiving updates on its status, you can use the `submit` method. Here's an example:
 
 ```python
 import asyncio
 import fal_client
```

### Comparing `fal_client-0.2.2/src/fal_client/__init__.py` & `fal_client-0.3.0/src/fal_client/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,17 @@
     SyncClient,
     Status,
     Queued,
     InProgress,
     Completed,
     SyncRequestHandle,
     AsyncRequestHandle,
+    encode,
+    encode_file,
+    encode_image,
 )
 
 __all__ = [
     "SyncClient",
     "AsyncClient",
     "Status",
     "Queued",
@@ -20,14 +23,17 @@
     "AsyncRequestHandle",
     "run",
     "submit",
     "stream",
     "run_async",
     "submit_async",
     "stream_async",
+    "encode",
+    "encode_file",
+    "encode_image",
 ]
 
 sync_client = SyncClient()
 run = sync_client.run
 submit = sync_client.submit
 stream = sync_client.stream
 upload = sync_client.upload
```

### Comparing `fal_client-0.2.2/src/fal_client/auth.py` & `fal_client-0.3.0/src/fal_client/auth.py`

 * *Files identical despite different names*

### Comparing `fal_client-0.2.2/src/fal_client/client.py` & `fal_client-0.3.0/src/fal_client/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import io
 import os
 import mimetypes
 import asyncio
 import time
+import base64
 from dataclasses import dataclass, field
 from functools import cached_property
 from typing import Any, AsyncIterator, Iterator, TYPE_CHECKING
 
 import httpx
 from httpx_sse import aconnect_sse, connect_sse
 from fal_client.auth import FAL_RUN_HOST, fetch_credentials
@@ -411,7 +412,32 @@
 
     def upload_image(self, image: Image.Image, format: str = "jpeg") -> str:
         """Upload a pillow image object to the CDN and return the access URL."""
 
         with io.BytesIO() as buffer:
             image.save(buffer, format=format)
             return self.upload(buffer.getvalue(), f"image/{format}")
+
+
+def encode(data: str | bytes, content_type: str) -> str:
+    """Encode the given data blob to a data URL with the specified content type."""
+    if isinstance(data, str):
+        data = data.encode("utf-8")
+
+    return f"data:{content_type};base64,{base64.b64encode(data).decode()}"
+
+
+def encode_file(path: os.PathLike) -> str:
+    """Encode a file from the local filesystem to a data URL with the inferred content type."""
+    mime_type, _ = mimetypes.guess_type(path)
+    if mime_type is None:
+        mime_type = "application/octet-stream"
+
+    with open(path, "rb") as file:
+        return encode(file.read(), mime_type)
+
+
+def encode_image(image: Image.Image, format: str = "jpeg") -> str:
+    """Encode a pillow image object to a data URL with the specified format."""
+    with io.BytesIO() as buffer:
+        image.save(buffer, format=format)
+        return encode(buffer.getvalue(), f"image/{format}")
```

### Comparing `fal_client-0.2.2/src/fal_client.egg-info/PKG-INFO` & `fal_client-0.3.0/src/fal_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal_client
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python client for fal.ai
 Author: fal <hello@fal.ai>
 Project-URL: homepage, https://fal.ai
 Project-URL: repository, https://github.com/fal-ai/fal
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx<1,>=0.21.0
@@ -62,14 +62,26 @@
 import fal_client
 
 audio_url = fal_client.upload_file("path/to/audio.wav")
 response = fal_client.run("fal-ai/whisper", arguments={"audio_url": audio_url})
 print(response["text"])
 ```
 
+## Encoding files as in-memory data URLs
+
+If you don't want to upload your file to our CDN service (for latency reasons, for example), you can encode it as a data URL and pass it directly to the client. Here's an example:
+
+```python
+import fal_client
+
+audio_data_url = fal_client.encode_file("path/to/audio.wav")
+response = fal_client.run("fal-ai/whisper", arguments={"audio_url": audio_data_url})
+print(response["text"])
+```
+
 ## Queuing requests
 
 When you want to send a request and keep receiving updates on its status, you can use the `submit` method. Here's an example:
 
 ```python
 import asyncio
 import fal_client
```

### Comparing `fal_client-0.2.2/tests/test_async_client.py` & `fal_client-0.3.0/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `fal_client-0.2.2/tests/test_sync_client.py` & `fal_client-0.3.0/tests/test_sync_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -81,7 +81,21 @@
     response = httpx.get(url)
     response.raise_for_status()
 
     response_image = Image.open(io.BytesIO(response.content))
     assert response_image.size == (100, 100)
     assert response_image.mode == "RGB"
     assert response_image.getpixel((0, 0)) == (0, 0, 0)
+
+
+def test_fal_client_encode(client: fal_client.SyncClient, tmp_path):
+    image = Image.new("RGB", (1024, 1024))
+
+    url = fal_client.encode_image(image)
+    response = client.run(
+        "fal-ai/fast-sdxl/image-to-image",
+        arguments={"image_url": url, "prompt": "a cat"},
+    )
+
+    assert len(response["images"]) == 1
+    assert response["images"][0]["width"] == 1024
+    assert response["images"][0]["height"] == 1024
```

