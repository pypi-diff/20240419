# Comparing `tmp/aporacle-0.0.137.tar.gz` & `tmp/aporacle-0.0.138.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporacle-0.0.137.tar", max compression
+gzip compressed data, was "aporacle-0.0.138.tar", max compression
```

## Comparing `aporacle-0.0.137.tar` & `aporacle-0.0.138.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.137/README.md
--rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.137/aporacle/__init__.py
--rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.137/aporacle/broadcast/__init__.py
--rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.137/aporacle/conf/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.137/aporacle/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.137/aporacle/core/utils/__init__.py
--rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.137/aporacle/core/utils/async_call_scheduler.py
--rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.137/aporacle/data/__init__.py
--rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.137/aporacle/data/asset/__init__.py
--rw-r--r--   0        0        0     1459 2024-03-25 05:26:42.304279 aporacle-0.0.137/aporacle/data/combination.py
--rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.137/aporacle/data/db/__init__.py
--rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.137/aporacle/data/db/crud.py
--rw-r--r--   0        0        0    10174 2024-03-22 09:49:57.935682 aporacle-0.0.137/aporacle/data/gcp/__init__.py
--rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.137/aporacle/data/symbols/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.137/aporacle/execution/__init__.py
--rw-r--r--   0        0        0     5666 2024-03-27 10:53:43.099151 aporacle-0.0.137/aporacle/execution/executables.py
--rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.137/aporacle/network/__init__.py
--rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.137/aporacle/network/network_base.py
--rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.137/aporacle/shared_setup.py
--rw-r--r--   0        0        0      399 2024-04-19 05:34:07.279268 aporacle-0.0.137/pyproject.toml
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.137/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.138/README.md
+-rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.138/aporacle/__init__.py
+-rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.138/aporacle/broadcast/__init__.py
+-rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.138/aporacle/conf/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.138/aporacle/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.138/aporacle/core/utils/__init__.py
+-rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.138/aporacle/core/utils/async_call_scheduler.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.138/aporacle/data/__init__.py
+-rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.138/aporacle/data/asset/__init__.py
+-rw-r--r--   0        0        0     1531 2024-04-19 06:26:40.914071 aporacle-0.0.138/aporacle/data/combination.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.138/aporacle/data/db/__init__.py
+-rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.138/aporacle/data/db/crud.py
+-rw-r--r--   0        0        0      806 2024-04-19 06:26:40.786070 aporacle-0.0.138/aporacle/data/feed_results.py
+-rw-r--r--   0        0        0    10186 2024-04-19 06:26:40.918071 aporacle-0.0.138/aporacle/data/gcp/__init__.py
+-rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.138/aporacle/data/symbols/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.138/aporacle/execution/__init__.py
+-rw-r--r--   0        0        0     5666 2024-03-27 10:53:43.099151 aporacle-0.0.138/aporacle/execution/executables.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.138/aporacle/network/__init__.py
+-rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.138/aporacle/network/network_base.py
+-rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.138/aporacle/shared_setup.py
+-rw-r--r--   0        0        0      399 2024-04-19 06:26:52.306176 aporacle-0.0.138/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.138/PKG-INFO
```

### Comparing `aporacle-0.0.137/aporacle/broadcast/__init__.py` & `aporacle-0.0.138/aporacle/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.137/aporacle/conf/__init__.py` & `aporacle-0.0.138/aporacle/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.137/aporacle/core/utils/async_call_scheduler.py` & `aporacle-0.0.138/aporacle/core/utils/async_call_scheduler.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.137/aporacle/data/asset/__init__.py` & `aporacle-0.0.138/aporacle/data/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.137/aporacle/data/db/crud.py` & `aporacle-0.0.138/aporacle/data/db/crud.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.137/aporacle/data/gcp/__init__.py` & `aporacle-0.0.138/aporacle/data/gcp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             blob = bucket.blob(source_file_path.split('/')[-1])  # Use filename by default
         blob.upload_from_filename(source_file_path)
         print(f"File uploaded to {bucket_name}/{blob.name}")
     except Exception as err:
         print(f"Error uploading file: {err}")
 
 
-# 4. Download file from bucket by symbol name.
+# 4. Download file from bucket by file_name name.
 def download_file_from_bucket(bucket_name: str, object_name: str, local_path: str):
     """Downloads a file from GCP storage and returns the local path.
 
       Args:
           bucket_name: The name of the bucket containing the file.
           object_name: The name of the file to download.
           local_path: The local path to save the downloaded file.
@@ -104,15 +104,15 @@
         blob.download_to_filename(local_path)
         return local_path
     except Exception as err:
         print(f"Error downloading file: {err}")
         return None
 
 
-# 5. Delete file from bucket by symbol name.
+# 5. Delete file from bucket by file_name name.
 def delete_file_from_bucket(bucket_name: str, object_name: str):
     """Deletes a file (blob) from a bucket in Google Cloud Storage.
 
       Args:
           bucket_name: The name of the bucket containing the file.
           object_name: The name of the file (blob) to delete.
 
@@ -164,16 +164,16 @@
     storage_client = storage.Client()
     bucket = storage_client.bucket(bucket_name)
     blob = bucket.blob(destination_blob_name)
     blob.upload_from_string(csv_buffer.getvalue())
 
 
 # 8. Download CSV from GCP and return as DataFrame
-def download_csv_from_gcp_return_df(bucket_name: str, symbol: str):
-    file_path = f"{symbol}.csv".lower()
+def download_csv_from_gcp_return_df(bucket_name: str, file_name: str):
+    file_path = f"{file_name}.csv".lower()
 
     # Download the CSV file from GCP bucket
     storage_client = storage.Client()
     bucket = storage_client.bucket(bucket_name)
     blob = bucket.blob(file_path)
 
     # Download data as a byte stream
```

### Comparing `aporacle-0.0.137/aporacle/data/symbols/__init__.py` & `aporacle-0.0.138/aporacle/data/symbols/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.137/aporacle/execution/executables.py` & `aporacle-0.0.138/aporacle/execution/executables.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.137/aporacle/network/network_base.py` & `aporacle-0.0.138/aporacle/network/network_base.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.137/aporacle/shared_setup.py` & `aporacle-0.0.138/aporacle/shared_setup.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.137/PKG-INFO` & `aporacle-0.0.138/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aporacle
-Version: 0.0.137
+Version: 0.0.138
 Summary: 
 Author: Makhosonke Morafo
 Author-email: makhosonke@komokun.org
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

