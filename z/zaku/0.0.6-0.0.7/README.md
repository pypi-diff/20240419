# Comparing `tmp/zaku-0.0.6-py3-none-any.whl.zip` & `tmp/zaku-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12307 bytes, number of entries: 12
+Zip file size: 12453 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       59 b- defN 24-Apr-15 02:31 zaku/__init__.py
 -rw-r--r--  2.0 unx     3780 b- defN 24-Apr-17 22:37 zaku/base.py
--rw-r--r--  2.0 unx     5045 b- defN 24-Apr-17 23:08 zaku/client.py
--rw-r--r--  2.0 unx     8316 b- defN 24-Apr-18 03:58 zaku/interfaces.py
+-rw-r--r--  2.0 unx     5423 b- defN 24-Apr-19 04:25 zaku/client.py
+-rw-r--r--  2.0 unx     8591 b- defN 24-Apr-19 05:16 zaku/interfaces.py
 -rw-r--r--  2.0 unx     1678 b- defN 24-Apr-14 19:38 zaku/job_queue.py
--rw-r--r--  2.0 unx     5983 b- defN 24-Apr-18 03:43 zaku/server.py
--rw-r--r--  2.0 unx     1064 b- defN 24-Apr-18 04:03 zaku-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     4220 b- defN 24-Apr-18 04:03 zaku-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 04:03 zaku-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-18 04:03 zaku-0.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-Apr-18 04:03 zaku-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      893 b- defN 24-Apr-18 04:03 zaku-0.0.6.dist-info/RECORD
-12 files, 31184 bytes uncompressed, 10829 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx     5982 b- defN 24-Apr-18 05:38 zaku/server.py
+-rw-r--r--  2.0 unx     1064 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4220 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      893 b- defN 24-Apr-19 05:25 zaku-0.0.7.dist-info/RECORD
+12 files, 31836 bytes uncompressed, 10975 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: zaku/job_queue.py
 Comment: 
 
 Filename: zaku/server.py
 Comment: 
 
-Filename: zaku-0.0.6.dist-info/LICENSE
+Filename: zaku-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: zaku-0.0.6.dist-info/METADATA
+Filename: zaku-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: zaku-0.0.6.dist-info/WHEEL
+Filename: zaku-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: zaku-0.0.6.dist-info/entry_points.txt
+Filename: zaku-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: zaku-0.0.6.dist-info/top_level.txt
+Filename: zaku-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: zaku-0.0.6.dist-info/RECORD
+Filename: zaku-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zaku/client.py

```diff
@@ -1,14 +1,14 @@
 from contextlib import contextmanager
+from typing import Dict
 from uuid import uuid4
 
 import msgpack
 import requests
 from params_proto import PrefixProto, Proto, Flag
-from typing import Dict
 
 from zaku.interfaces import Payload
 
 
 class TaskQ(PrefixProto, cli=False):
     """TaskQ Client
     ----------------
@@ -175,7 +175,17 @@
         try:
             yield job
         except Exception as e:
             self.mark_reset(job_id)
             raise e
 
         self.mark_done(job_id)
+
+    def clear_queue(self):
+        """Remove all jobs in a queue. Useful when stale jobs degrades performance."""
+        res = requests.delete(
+            self.uri + "/tasks",
+            json={"queue": self.name, "job_id": "*"},
+        )
+        if res.status_code == 200:
+            return True
+        raise Exception(f"Failed to reset job on {self.uri}.", res.content)
```

## zaku/interfaces.py

```diff
@@ -1,11 +1,11 @@
 from io import BytesIO
 from time import time
 from types import SimpleNamespace
-from typing import Literal, Any, Tuple, Coroutine, Dict, Union, TYPE_CHECKING
+from typing import Literal, Any, Coroutine, Dict, Union, TYPE_CHECKING, Tuple
 
 import msgpack
 import numpy as np
 
 if TYPE_CHECKING:
     import redis
     import torch
@@ -206,15 +206,15 @@
         p = r.pipeline()
         p.json().set(entry_key, ".", vars(job))
         if payload:
             p.set(entry_key + ".payload", payload)
         return p.execute()
 
     @staticmethod
-    async def take(r: "redis.asyncio.Redis", queue, *, prefix) -> Tuple[str, Any]:
+    async def take(r: "redis.asyncio.Redis", queue, *, prefix) -> Tuple[Any, Any]:
         from redis.commands.search.query import Query
         from redis.commands.search.result import Result
 
         index_name = f"{prefix}:{queue}"
 
         # note: search ranks results via FTIDF. Use aggregation to sort by created_ts
         q = Query("@status: { created }").paging(0, 1)
@@ -234,19 +234,30 @@
             .execute()
         )
 
         job_id = job.id[len(index_name) + 1 :]
         return job_id, payload
 
     @staticmethod
-    def remove(r: "redis.asyncio.Redis", job_id, queue, *, prefix) -> Coroutine:
+    async def remove(r: "redis.asyncio.Redis", job_id, queue, *, prefix) -> Coroutine:
+        print("deleting!!!!!!!!!!!!!!!!")
         entry_name = f"{prefix}:{queue}:{job_id}"
 
         p = r.pipeline()
-        response = p.json().delete(entry_name).delete(entry_name + ".payload").execute()
+
+        if job_id == "*":
+            count = 0
+            async for key in r.scan_iter(entry_name):
+                p = p.delete(key)
+                count += 1
+
+            await p.execute()
+            return count
+
+        response = await p.json().delete(entry_name).delete(entry_name + ".payload").execute()
         return response
 
     @staticmethod
     def reset(r: "redis.asyncio.Redis", job_id, queue, *, prefix):
         entry_name = f"{prefix}:{queue}:{job_id}"
 
         p = r.pipeline()
```

## zaku/server.py

```diff
@@ -95,22 +95,21 @@
     )
 
     free_port: bool = Flag("kill process squatting target port if True.")
     static_root: str = "."
     verbose = Flag("show the list of configurations during launch if True.")
 
     def __post_init__(self):
-        Server.__post_init__(self)
-
         if self.verbose:
             print("========= Arguments =========")
             for k, v in vars(self).items():
                 print(f" {k} = {v},")
             print("-----------------------------")
 
+        Server.__post_init__(self)
         self.redis = redis.asyncio.Redis(**vars(Redis))
 
     async def create_queue(self, request: web.Request):
         data = await request.json()
         # print("==>", data)
         try:
             await Job.create_queue(self.redis, **data, prefix=self.prefix)
```

## Comparing `zaku-0.0.6.dist-info/LICENSE` & `zaku-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zaku-0.0.6.dist-info/METADATA` & `zaku-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaku
-Version: 0.0.6
+Version: 0.0.7
 Summary: Zaku Task Queue is for distributed ML-workloads.
 Home-page: https://github.com/geyang/zaku
 Author: Ge Yang<ge.ike.yang@gmail.com>
 Author-email: ge.ike.yang@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

## Comparing `zaku-0.0.6.dist-info/RECORD` & `zaku-0.0.7.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 zaku/__init__.py,sha256=dVBFG2RyfsJ9Yf3OgSN49X6Tpk7RgfdFHyFYgs1vvjs,59
 zaku/base.py,sha256=7jgQ1Rcz6eDLNjkryDXLC9QrDWcct9fdixwHPjXd59g,3780
-zaku/client.py,sha256=u0GhknUONMzwGjY7mcS3A8HCrDZAxWx-vCdn0cheOo8,5045
-zaku/interfaces.py,sha256=SQ-AzIJQ2SUyTw_famGbRa_BzSyey1oUraJyW_5zwVI,8316
+zaku/client.py,sha256=0peyk9FQgTy5ksHbjlCMlsnYFWGlpqd0tQadButsbA8,5423
+zaku/interfaces.py,sha256=CW8WP9Vno6hGto5Zfgt_cGCbXd-q94BPUMyb3nc5KWQ,8591
 zaku/job_queue.py,sha256=rClaiGYU6ZDSi-ehPtKbZfJcYxZaOr3DHMPfRq9jl4o,1678
-zaku/server.py,sha256=2WWzOpKVKE-KvBR5Tst9YNaaD2QrmYJqCfKmINSYbFA,5983
-zaku-0.0.6.dist-info/LICENSE,sha256=ViVJUWot4p3kmGwzBBRu6vqoBFQuLFKyGIR3jzh4X_A,1064
-zaku-0.0.6.dist-info/METADATA,sha256=YewKLELr9qYLgkGQ2eiiDgmZCnn-lCOR-RTvAVxj0b4,4220
-zaku-0.0.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-zaku-0.0.6.dist-info/entry_points.txt,sha256=OQmjyBNrqRKNAK7zutZ83SXuKvH6EURf28dG8-nPtdE,49
-zaku-0.0.6.dist-info/top_level.txt,sha256=NOH9JyYZg-VCpceLmApF5Rx3njTGe8RjuRaQsTc5k4o,5
-zaku-0.0.6.dist-info/RECORD,,
+zaku/server.py,sha256=G91fCTGtwaaQiuRlpFPV7_aJq_gc0lTWTLFeCDNTeS4,5982
+zaku-0.0.7.dist-info/LICENSE,sha256=ViVJUWot4p3kmGwzBBRu6vqoBFQuLFKyGIR3jzh4X_A,1064
+zaku-0.0.7.dist-info/METADATA,sha256=uUOqb-jTq1KDA6YGFdFjKgCjhLPwrgT55vwv49qXLC4,4220
+zaku-0.0.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+zaku-0.0.7.dist-info/entry_points.txt,sha256=OQmjyBNrqRKNAK7zutZ83SXuKvH6EURf28dG8-nPtdE,49
+zaku-0.0.7.dist-info/top_level.txt,sha256=NOH9JyYZg-VCpceLmApF5Rx3njTGe8RjuRaQsTc5k4o,5
+zaku-0.0.7.dist-info/RECORD,,
```

