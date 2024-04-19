# Comparing `tmp/qrdm-2.0.1.tar.gz` & `tmp/qrdm-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrdm-2.0.1.tar", last modified: Fri Mar 22 16:56:31 2024, max compression
+gzip compressed data, was "qrdm-2.0.2.tar", last modified: Fri Apr 19 14:40:51 2024, max compression
```

## Comparing `qrdm-2.0.1.tar` & `qrdm-2.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-03-22 16:56:31.137544 qrdm-2.0.1/
--rw-r--r--   0 er27743    (501) staff       (20)     1093 2024-02-01 15:51:39.000000 qrdm-2.0.1/LICENSE.txt
--rw-r--r--   0 er27743    (501) staff       (20)      165 2024-02-01 20:42:07.000000 qrdm-2.0.1/MANIFEST.in
--rw-r--r--   0 er27743    (501) staff       (20)     5231 2024-03-22 16:56:31.137320 qrdm-2.0.1/PKG-INFO
--rw-r--r--   0 er27743    (501) staff       (20)     3146 2024-03-20 18:50:58.000000 qrdm-2.0.1/README.md
--rw-r--r--   0 er27743    (501) staff       (20)     2377 2024-03-20 18:17:25.000000 qrdm-2.0.1/pyproject.toml
--rw-r--r--   0 er27743    (501) staff       (20)       38 2024-03-22 16:56:31.137587 qrdm-2.0.1/setup.cfg
--rw-r--r--   0 er27743    (501) staff       (20)      405 2024-03-19 18:31:04.000000 qrdm-2.0.1/setup.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-03-22 16:56:31.131026 qrdm-2.0.1/src/
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-03-22 16:56:31.132586 qrdm-2.0.1/src/qrdm/
--rw-r--r--   0 er27743    (501) staff       (20)      410 2024-03-22 16:55:20.000000 qrdm-2.0.1/src/qrdm/__init__.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-03-22 16:56:31.133916 qrdm-2.0.1/src/qrdm/backend/
--rw-r--r--   0 er27743    (501) staff       (20)      582 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/backend/__init__.py
--rw-r--r--   0 er27743    (501) staff       (20)     5110 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/backend/config.py
--rw-r--r--   0 er27743    (501) staff       (20)     2274 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/backend/main.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-03-22 16:56:31.134267 qrdm-2.0.1/src/qrdm/backend/routers/
--rw-r--r--   0 er27743    (501) staff       (20)       49 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/backend/routers/__init__.py
--rw-r--r--   0 er27743    (501) staff       (20)     5650 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/backend/routers/qr.py
--rw-r--r--   0 er27743    (501) staff       (20)      485 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/exceptions.py
--rw-r--r--   0 er27743    (501) staff       (20)     4430 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/models.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-03-22 16:56:31.135139 qrdm-2.0.1/src/qrdm/qr/
--rw-r--r--   0 er27743    (501) staff       (20)       45 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/qr/__init__.py
--rw-r--r--   0 er27743    (501) staff       (20)     1234 2024-02-01 20:42:07.000000 qrdm-2.0.1/src/qrdm/qr/_const.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-03-22 16:56:31.135644 qrdm-2.0.1/src/qrdm/qr/data/
--rw-r--r--   0 er27743    (501) staff       (20)       50 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/qr/data/__init__.py
--rw-r--r--   0 er27743    (501) staff       (20)      789 2024-02-01 20:42:07.000000 qrdm-2.0.1/src/qrdm/qr/data/qr_capacity.csv
--rw-r--r--   0 er27743    (501) staff       (20)    35444 2024-02-01 20:42:07.000000 qrdm-2.0.1/src/qrdm/qr/data/qrdm_logo_red.png
--rw-r--r--   0 er27743    (501) staff       (20)    12725 2024-03-22 16:41:47.000000 qrdm-2.0.1/src/qrdm/qr/decode.py
--rw-r--r--   0 er27743    (501) staff       (20)    11076 2024-03-20 12:57:07.000000 qrdm-2.0.1/src/qrdm/qr/encode.py
--rw-r--r--   0 er27743    (501) staff       (20)     9598 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/qr/pdf_writer.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-03-22 16:56:31.136257 qrdm-2.0.1/src/qrdm/qr/protobuf/
--rw-r--r--   0 er27743    (501) staff       (20)      823 2024-03-19 18:31:04.000000 qrdm-2.0.1/src/qrdm/qr/protobuf/__init__.py
--rw-r--r--   0 er27743    (501) staff       (20)      383 2024-02-05 20:55:14.000000 qrdm-2.0.1/src/qrdm/qr/protobuf/qrdm.proto
--rw-r--r--   0 er27743    (501) staff       (20)     2046 2024-02-05 20:56:25.000000 qrdm-2.0.1/src/qrdm/qr/protobuf/qrdm_pb2.py
--rw-r--r--   0 er27743    (501) staff       (20)     2310 2024-02-09 16:48:01.000000 qrdm-2.0.1/src/qrdm/qr/protobuf/qrdm_pb2.pyi
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-03-22 16:56:31.136440 qrdm-2.0.1/src/qrdm.egg-info/
--rw-r--r--   0 er27743    (501) staff       (20)     5231 2024-03-22 16:56:31.000000 qrdm-2.0.1/src/qrdm.egg-info/PKG-INFO
--rw-r--r--   0 er27743    (501) staff       (20)      773 2024-03-22 16:56:31.000000 qrdm-2.0.1/src/qrdm.egg-info/SOURCES.txt
--rw-r--r--   0 er27743    (501) staff       (20)        1 2024-03-22 16:56:31.000000 qrdm-2.0.1/src/qrdm.egg-info/dependency_links.txt
--rw-r--r--   0 er27743    (501) staff       (20)      439 2024-03-22 16:56:31.000000 qrdm-2.0.1/src/qrdm.egg-info/requires.txt
--rw-r--r--   0 er27743    (501) staff       (20)        5 2024-03-22 16:56:31.000000 qrdm-2.0.1/src/qrdm.egg-info/top_level.txt
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.840281 qrdm-2.0.2/
+-rw-r--r--   0 er27743    (501) staff       (20)     1093 2024-02-01 15:51:39.000000 qrdm-2.0.2/LICENSE.txt
+-rw-r--r--   0 er27743    (501) staff       (20)      165 2024-02-01 20:42:07.000000 qrdm-2.0.2/MANIFEST.in
+-rw-r--r--   0 er27743    (501) staff       (20)     5231 2024-04-19 14:40:51.840073 qrdm-2.0.2/PKG-INFO
+-rw-r--r--   0 er27743    (501) staff       (20)     3146 2024-03-20 18:50:58.000000 qrdm-2.0.2/README.md
+-rw-r--r--   0 er27743    (501) staff       (20)     2377 2024-03-20 18:17:25.000000 qrdm-2.0.2/pyproject.toml
+-rw-r--r--   0 er27743    (501) staff       (20)       38 2024-04-19 14:40:51.840318 qrdm-2.0.2/setup.cfg
+-rw-r--r--   0 er27743    (501) staff       (20)      405 2024-03-19 18:31:04.000000 qrdm-2.0.2/setup.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.831039 qrdm-2.0.2/src/
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.833181 qrdm-2.0.2/src/qrdm/
+-rw-r--r--   0 er27743    (501) staff       (20)      410 2024-04-18 18:52:12.000000 qrdm-2.0.2/src/qrdm/__init__.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.835103 qrdm-2.0.2/src/qrdm/backend/
+-rw-r--r--   0 er27743    (501) staff       (20)      582 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/backend/__init__.py
+-rw-r--r--   0 er27743    (501) staff       (20)     5110 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/backend/config.py
+-rw-r--r--   0 er27743    (501) staff       (20)     2274 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/backend/main.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.835811 qrdm-2.0.2/src/qrdm/backend/routers/
+-rw-r--r--   0 er27743    (501) staff       (20)       49 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/backend/routers/__init__.py
+-rw-r--r--   0 er27743    (501) staff       (20)     5650 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/backend/routers/qr.py
+-rw-r--r--   0 er27743    (501) staff       (20)      485 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/exceptions.py
+-rw-r--r--   0 er27743    (501) staff       (20)     4430 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/models.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.837021 qrdm-2.0.2/src/qrdm/qr/
+-rw-r--r--   0 er27743    (501) staff       (20)       45 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/qr/__init__.py
+-rw-r--r--   0 er27743    (501) staff       (20)     1234 2024-02-01 20:42:07.000000 qrdm-2.0.2/src/qrdm/qr/_const.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.837776 qrdm-2.0.2/src/qrdm/qr/data/
+-rw-r--r--   0 er27743    (501) staff       (20)       50 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/qr/data/__init__.py
+-rw-r--r--   0 er27743    (501) staff       (20)      789 2024-02-01 20:42:07.000000 qrdm-2.0.2/src/qrdm/qr/data/qr_capacity.csv
+-rw-r--r--   0 er27743    (501) staff       (20)    35444 2024-02-01 20:42:07.000000 qrdm-2.0.2/src/qrdm/qr/data/qrdm_logo_red.png
+-rw-r--r--   0 er27743    (501) staff       (20)    12725 2024-04-18 18:49:43.000000 qrdm-2.0.2/src/qrdm/qr/decode.py
+-rw-r--r--   0 er27743    (501) staff       (20)    11089 2024-04-18 18:49:43.000000 qrdm-2.0.2/src/qrdm/qr/encode.py
+-rw-r--r--   0 er27743    (501) staff       (20)     9598 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/qr/pdf_writer.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.838950 qrdm-2.0.2/src/qrdm/qr/protobuf/
+-rw-r--r--   0 er27743    (501) staff       (20)      823 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/qr/protobuf/__init__.py
+-rw-r--r--   0 er27743    (501) staff       (20)      383 2024-02-05 20:55:14.000000 qrdm-2.0.2/src/qrdm/qr/protobuf/qrdm.proto
+-rw-r--r--   0 er27743    (501) staff       (20)     2046 2024-02-05 20:56:25.000000 qrdm-2.0.2/src/qrdm/qr/protobuf/qrdm_pb2.py
+-rw-r--r--   0 er27743    (501) staff       (20)     2310 2024-02-09 16:48:01.000000 qrdm-2.0.2/src/qrdm/qr/protobuf/qrdm_pb2.pyi
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.839160 qrdm-2.0.2/src/qrdm.egg-info/
+-rw-r--r--   0 er27743    (501) staff       (20)     5231 2024-04-19 14:40:51.000000 qrdm-2.0.2/src/qrdm.egg-info/PKG-INFO
+-rw-r--r--   0 er27743    (501) staff       (20)      773 2024-04-19 14:40:51.000000 qrdm-2.0.2/src/qrdm.egg-info/SOURCES.txt
+-rw-r--r--   0 er27743    (501) staff       (20)        1 2024-04-19 14:40:51.000000 qrdm-2.0.2/src/qrdm.egg-info/dependency_links.txt
+-rw-r--r--   0 er27743    (501) staff       (20)      439 2024-04-19 14:40:51.000000 qrdm-2.0.2/src/qrdm.egg-info/requires.txt
+-rw-r--r--   0 er27743    (501) staff       (20)        5 2024-04-19 14:40:51.000000 qrdm-2.0.2/src/qrdm.egg-info/top_level.txt
```

### Comparing `qrdm-2.0.1/LICENSE.txt` & `qrdm-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/PKG-INFO` & `qrdm-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrdm
-Version: 2.0.1
+Version: 2.0.2
 Summary: QR Data Manager
 Author: MIT Lincoln Laboratory
 Author-email: "Cuyler D. O'Brien" <cuyler.obrien@ll.mit.edu>, "Eric A. Quintero" <Eric.Quintero@ll.mit.edu>, Tod Shannon <tod@ll.mit.edu>, "Michael J. Snyder" <michael.snyder@ll.mit.edu>
 License: MIT License
 Project-URL: Documentation, https://mit-ll.github.io/qrdm
 Project-URL: Repository, https://github.com/mit-ll/qrdm
 Keywords: QR,QR code
```

### Comparing `qrdm-2.0.1/README.md` & `qrdm-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/pyproject.toml` & `qrdm-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/backend/__init__.py` & `qrdm-2.0.2/src/qrdm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/backend/config.py` & `qrdm-2.0.2/src/qrdm/backend/config.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/backend/main.py` & `qrdm-2.0.2/src/qrdm/backend/main.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/backend/routers/qr.py` & `qrdm-2.0.2/src/qrdm/backend/routers/qr.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/models.py` & `qrdm-2.0.2/src/qrdm/models.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/qr/_const.py` & `qrdm-2.0.2/src/qrdm/qr/_const.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/qr/data/qr_capacity.csv` & `qrdm-2.0.2/src/qrdm/qr/data/qr_capacity.csv`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/qr/data/qrdm_logo_red.png` & `qrdm-2.0.2/src/qrdm/qr/data/qrdm_logo_red.png`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/qr/decode.py` & `qrdm-2.0.2/src/qrdm/qr/decode.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,18 +189,18 @@
         fixed_symbols = [
             decoding_codec.decode(x, erase_pos=dropped_code_inds, only_erasures=True)[0]
             for x in received_symbols
         ]
         sorted_payloads = [bytes(x) for x in zip(*fixed_symbols)]
         logger.debug("Post-EC payloads: %r", [p.hex(" ", 4) for p in sorted_payloads])
 
-    total_payload_bytes = b"".join(sorted_payloads).strip(b"\0")
+    total_payload_bytes = b"".join(sorted_payloads)
     logger.debug("Concatenated total payload: %s", total_payload_bytes.hex(" ", 4))
 
-    h = hashlib.shake_256(total_payload_bytes)
+    h = hashlib.shake_256(total_payload_bytes.strip(b"\0"))
     hash_bytes_check = h.digest(8)
     document_hash_check = int.from_bytes(hash_bytes_check, "big")
     logger.debug("Recovered document hash: %s", hash_bytes_check.hex(" ", 4))
     if document_hash_check != first_content.meta.document_hash:
         logger.error(
             "Recovered document does not match verification hash: "
             f"{document_hash_check} vs. {first_content.meta.document_hash}"
```

### Comparing `qrdm-2.0.1/src/qrdm/qr/encode.py` & `qrdm-2.0.2/src/qrdm/qr/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     error_tolerance: ECSettingValues = ECSettingValues.M,
 ) -> list[bytes]:
     """Construct b85-encoded payloads from a document for QR code construction."""
     logger.debug("Generating QR code payloads")
     total_payload_bytes = document_content.model_dump_compressed_bytes()
     logger.debug("Compressed document: %s", total_payload_bytes.hex(" ", 4))
 
-    h = hashlib.shake_256(total_payload_bytes)
+    h = hashlib.shake_256(total_payload_bytes.strip(b"\0"))
     hash_bytes = h.digest(8)
     logger.debug("Document hash: %s", hash_bytes.hex(" ", 4))
     document_hash = int.from_bytes(hash_bytes, "big")
 
     max_qr_bytes = qr_const.QR_CAPACITIES[qr_const.QR_SIZE][error_tolerance.name]
     single_qr_payload_size = max_qr_bytes - PROTOBUF_RESERVED_LEN
     # Reduce payload size to account for b85 inflation
```

### Comparing `qrdm-2.0.1/src/qrdm/qr/pdf_writer.py` & `qrdm-2.0.2/src/qrdm/qr/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/qr/protobuf/__init__.py` & `qrdm-2.0.2/src/qrdm/qr/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/qr/protobuf/qrdm_pb2.py` & `qrdm-2.0.2/src/qrdm/qr/protobuf/qrdm_pb2.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm/qr/protobuf/qrdm_pb2.pyi` & `qrdm-2.0.2/src/qrdm/qr/protobuf/qrdm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.1/src/qrdm.egg-info/PKG-INFO` & `qrdm-2.0.2/src/qrdm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrdm
-Version: 2.0.1
+Version: 2.0.2
 Summary: QR Data Manager
 Author: MIT Lincoln Laboratory
 Author-email: "Cuyler D. O'Brien" <cuyler.obrien@ll.mit.edu>, "Eric A. Quintero" <Eric.Quintero@ll.mit.edu>, Tod Shannon <tod@ll.mit.edu>, "Michael J. Snyder" <michael.snyder@ll.mit.edu>
 License: MIT License
 Project-URL: Documentation, https://mit-ll.github.io/qrdm
 Project-URL: Repository, https://github.com/mit-ll/qrdm
 Keywords: QR,QR code
```

### Comparing `qrdm-2.0.1/src/qrdm.egg-info/SOURCES.txt` & `qrdm-2.0.2/src/qrdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

