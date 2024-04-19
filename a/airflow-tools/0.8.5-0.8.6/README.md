# Comparing `tmp/airflow_tools-0.8.5.tar.gz` & `tmp/airflow_tools-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_tools-0.8.5.tar", max compression
+gzip compressed data, was "airflow_tools-0.8.6.tar", max compression
```

## Comparing `airflow_tools-0.8.5.tar` & `airflow_tools-0.8.6.tar`

### file list

```diff
@@ -1,38 +1,69 @@
--rw-r--r--   0        0        0    11358 2024-04-17 09:35:16.813856 airflow_tools-0.8.5/LICENSE.txt
--rw-r--r--   0        0        0     8788 2024-04-17 09:35:16.813856 airflow_tools-0.8.5/README.md
--rw-r--r--   0        0        0     1315 2024-04-17 09:35:16.813856 airflow_tools-0.8.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/__init__.py
--rw-r--r--   0        0        0       22 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/_version.py
--rw-r--r--   0        0        0     1794 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/compression_utils.py
--rw-r--r--   0        0        0     4426 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/data_lake_facade.py
--rw-r--r--   0        0        0      115 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/__init__.py
--rw-r--r--   0        0        0     2298 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/filesystem_factory.py
--rw-r--r--   0        0        0      561 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/filesystem_protocol.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/__init__.py
--rw-r--r--   0        0        0     2382 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
--rw-r--r--   0        0        0     1974 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
--rw-r--r--   0        0        0     2472 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
--rw-r--r--   0        0        0     1586 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/local_filesystem.py
--rw-r--r--   0        0        0     2185 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/s3_filesystem.py
--rw-r--r--   0        0        0     1396 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/sftp_filesystem.py
--rw-r--r--   0        0        0     3877 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/notifications/slack/webhook.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/azure/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/azure/hooks/__init__.py
--rw-r--r--   0        0        0     3396 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/azure/hooks/azure_databricks.py
--rw-r--r--   0        0        0     1619 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/azure/hooks/azure_file_share.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/data_lake/operators/__init__.py
--rw-r--r--   0        0        0     2355 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/data_lake/operators/data_lake.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/operators/__init__.py
--rw-r--r--   0        0        0     6241 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/operators/filesystem.py
--rw-r--r--   0        0        0    11455 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py
--rw-r--r--   0        0        0      821 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/tasks.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/http_to_data_lake/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
--rw-r--r--   0        0        0     9015 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
--rw-r--r--   0        0        0     1108 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/providers/package.py
--rw-r--r--   0        0        0        0 2024-04-17 09:35:16.817855 airflow_tools-0.8.5/src/airflow_tools/py.typed
--rw-r--r--   0        0        0    10023 1970-01-01 00:00:00.000000 airflow_tools-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-15 09:01:15.875283 airflow_tools-0.8.6/LICENSE.txt
+-rw-r--r--   0        0        0     8788 2024-04-11 13:00:04.903032 airflow_tools-0.8.6/README.md
+-rw-r--r--   0        0        0     1315 2024-04-19 09:25:44.526673 airflow_tools-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.879171 airflow_tools-0.8.6/src/airflow_tools/__init__.py
+-rw-r--r--   0        0        0      185 2024-04-02 07:57:30.222077 airflow_tools-0.8.6/src/airflow_tools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      206 2024-04-02 08:15:12.748926 airflow_tools-0.8.6/src/airflow_tools/__pycache__/_version.cpython-311.pyc
+-rw-r--r--   0        0        0     4951 2024-04-02 07:57:39.047196 airflow_tools-0.8.6/src/airflow_tools/__pycache__/compression_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     6677 2024-04-02 07:57:38.301672 airflow_tools-0.8.6/src/airflow_tools/__pycache__/data_lake_facade.cpython-311.pyc
+-rw-r--r--   0        0        0      513 2024-04-02 07:57:38.331836 airflow_tools-0.8.6/src/airflow_tools/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0       22 2024-04-19 09:25:44.527084 airflow_tools-0.8.6/src/airflow_tools/_version.py
+-rw-r--r--   0        0        0     1794 2024-03-15 09:01:15.879695 airflow_tools-0.8.6/src/airflow_tools/compression_utils.py
+-rw-r--r--   0        0        0     4426 2024-03-23 22:52:20.616265 airflow_tools-0.8.6/src/airflow_tools/data_lake_facade.py
+-rw-r--r--   0        0        0      115 2024-03-15 09:01:15.880246 airflow_tools-0.8.6/src/airflow_tools/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.880736 airflow_tools-0.8.6/src/airflow_tools/filesystems/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-02 07:57:30.223361 airflow_tools-0.8.6/src/airflow_tools/filesystems/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3372 2024-04-02 07:57:30.227492 airflow_tools-0.8.6/src/airflow_tools/filesystems/__pycache__/filesystem_factory.cpython-311.pyc
+-rw-r--r--   0        0        0     2013 2024-04-02 07:57:36.176523 airflow_tools-0.8.6/src/airflow_tools/filesystems/__pycache__/filesystem_protocol.cpython-311.pyc
+-rw-r--r--   0        0        0     2298 2024-03-15 14:21:53.853567 airflow_tools-0.8.6/src/airflow_tools/filesystems/filesystem_factory.py
+-rw-r--r--   0        0        0      561 2024-03-23 23:14:28.037837 airflow_tools-0.8.6/src/airflow_tools/filesystems/filesystem_protocol.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.882284 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/__init__.py
+-rw-r--r--   0        0        0      202 2024-04-02 07:57:36.177762 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6142 2024-04-11 13:18:39.090296 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/__pycache__/azure_databricks_volume_filesystem.cpython-311.pyc
+-rw-r--r--   0        0        0     5414 2024-04-02 07:57:36.211529 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/__pycache__/azure_file_share_filesystem.cpython-311.pyc
+-rw-r--r--   0        0        0     5017 2024-04-02 07:57:36.182403 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/__pycache__/blob_storage_filesystem.cpython-311.pyc
+-rw-r--r--   0        0        0     4725 2024-04-02 07:57:36.191389 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/__pycache__/local_filesystem.cpython-311.pyc
+-rw-r--r--   0        0        0     4998 2024-04-02 07:57:36.202224 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/__pycache__/s3_filesystem.cpython-311.pyc
+-rw-r--r--   0        0        0     3921 2024-04-02 07:57:36.207463 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/__pycache__/sftp_filesystem.cpython-311.pyc
+-rw-r--r--   0        0        0     2382 2024-04-11 13:00:04.951649 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py
+-rw-r--r--   0        0        0     1974 2024-03-24 00:50:06.290603 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py
+-rw-r--r--   0        0        0     2472 2024-03-25 16:17:00.235954 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py
+-rw-r--r--   0        0        0     1640 2024-04-19 09:02:14.344679 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/local_filesystem.py
+-rw-r--r--   0        0        0     2185 2024-03-24 00:50:06.294839 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/s3_filesystem.py
+-rw-r--r--   0        0        0     1396 2024-03-24 00:21:54.788482 airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/sftp_filesystem.py
+-rw-r--r--   0        0        0     4490 2024-04-02 07:57:39.108030 airflow_tools-0.8.6/src/airflow_tools/notifications/slack/__pycache__/webhook.cpython-311.pyc
+-rw-r--r--   0        0        0     3877 2024-03-15 09:01:15.884092 airflow_tools-0.8.6/src/airflow_tools/notifications/slack/webhook.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.884537 airflow_tools-0.8.6/src/airflow_tools/providers/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-02 07:57:36.499592 airflow_tools-0.8.6/src/airflow_tools/providers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1228 2024-04-02 08:15:12.747744 airflow_tools-0.8.6/src/airflow_tools/providers/__pycache__/package.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.884904 airflow_tools-0.8.6/src/airflow_tools/providers/azure/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-02 07:57:36.500910 airflow_tools-0.8.6/src/airflow_tools/providers/azure/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.885232 airflow_tools-0.8.6/src/airflow_tools/providers/azure/hooks/__init__.py
+-rw-r--r--   0        0        0      207 2024-04-02 07:57:36.502143 airflow_tools-0.8.6/src/airflow_tools/providers/azure/hooks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5510 2024-04-02 07:57:37.605666 airflow_tools-0.8.6/src/airflow_tools/providers/azure/hooks/__pycache__/azure_databricks.cpython-311.pyc
+-rw-r--r--   0        0        0     2922 2024-04-02 07:57:36.506366 airflow_tools-0.8.6/src/airflow_tools/providers/azure/hooks/__pycache__/azure_file_share.cpython-311.pyc
+-rw-r--r--   0        0        0     3396 2024-03-18 14:38:56.888663 airflow_tools-0.8.6/src/airflow_tools/providers/azure/hooks/azure_databricks.py
+-rw-r--r--   0        0        0     1619 2024-03-15 09:01:15.885704 airflow_tools-0.8.6/src/airflow_tools/providers/azure/hooks/azure_file_share.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.886187 airflow_tools-0.8.6/src/airflow_tools/providers/data_lake/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-02 07:57:38.291881 airflow_tools-0.8.6/src/airflow_tools/providers/data_lake/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.886773 airflow_tools-0.8.6/src/airflow_tools/providers/data_lake/operators/__init__.py
+-rw-r--r--   0        0        0      215 2024-04-02 07:57:38.292857 airflow_tools-0.8.6/src/airflow_tools/providers/data_lake/operators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4073 2024-04-02 07:57:38.297166 airflow_tools-0.8.6/src/airflow_tools/providers/data_lake/operators/__pycache__/data_lake.cpython-311.pyc
+-rw-r--r--   0        0        0     2355 2024-03-23 22:52:20.625836 airflow_tools-0.8.6/src/airflow_tools/providers/data_lake/operators/data_lake.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.887444 airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/__init__.py
+-rw-r--r--   0        0        0      206 2024-04-02 07:57:38.309748 airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.888053 airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/operators/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-02 07:57:38.310934 airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/operators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8763 2024-04-02 07:57:38.313770 airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/operators/__pycache__/filesystem.cpython-311.pyc
+-rw-r--r--   0        0        0     6241 2024-04-11 13:40:29.952773 airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/operators/filesystem.py
+-rw-r--r--   0        0        0    11455 2024-04-19 09:05:28.898832 airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py
+-rw-r--r--   0        0        0      821 2024-04-11 13:00:04.959496 airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/tasks.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.890235 airflow_tools-0.8.6/src/airflow_tools/providers/http_to_data_lake/__init__.py
+-rw-r--r--   0        0        0      213 2024-04-02 07:57:38.332619 airflow_tools-0.8.6/src/airflow_tools/providers/http_to_data_lake/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.891091 airflow_tools-0.8.6/src/airflow_tools/providers/http_to_data_lake/operators/__init__.py
+-rw-r--r--   0        0        0      223 2024-04-02 07:57:38.333536 airflow_tools-0.8.6/src/airflow_tools/providers/http_to_data_lake/operators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11985 2024-04-02 07:57:38.342633 airflow_tools-0.8.6/src/airflow_tools/providers/http_to_data_lake/operators/__pycache__/http_to_data_lake.cpython-311.pyc
+-rw-r--r--   0        0        0     9015 2024-04-11 13:00:04.964694 airflow_tools-0.8.6/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py
+-rw-r--r--   0        0        0     1108 2024-03-18 14:38:56.889184 airflow_tools-0.8.6/src/airflow_tools/providers/package.py
+-rw-r--r--   0        0        0        0 2024-03-15 09:01:15.891899 airflow_tools-0.8.6/src/airflow_tools/py.typed
+-rw-r--r--   0        0        0    10023 1970-01-01 00:00:00.000000 airflow_tools-0.8.6/PKG-INFO
```

### Comparing `airflow_tools-0.8.5/LICENSE.txt` & `airflow_tools-0.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/README.md` & `airflow_tools-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/pyproject.toml` & `airflow_tools-0.8.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airflow-tools"
-version = "0.8.5"
+version = "0.8.6"
 
 description = ""
 authors = ["Biel Llobera <biel_llobera@dkl.digital>"]
 readme = "README.md"
 include = ["src/airflow_tools"]
 
 [tool.poetry.dependencies]
```

### Comparing `airflow_tools-0.8.5/src/airflow_tools/compression_utils.py` & `airflow_tools-0.8.6/src/airflow_tools/compression_utils.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/data_lake_facade.py` & `airflow_tools-0.8.6/src/airflow_tools/data_lake_facade.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/filesystems/filesystem_factory.py` & `airflow_tools-0.8.6/src/airflow_tools/filesystems/filesystem_factory.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/filesystems/filesystem_protocol.py` & `airflow_tools-0.8.6/src/airflow_tools/filesystems/filesystem_protocol.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py` & `airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/azure_databricks_volume_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py` & `airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/azure_file_share_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py` & `airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/blob_storage_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/local_filesystem.py` & `airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/local_filesystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
     def delete_prefix(self, prefix: str):
         path_to_delete = Path(self.hook.get_path()) / prefix
         shutil.rmtree(str(path_to_delete))
 
     def check_file(self, path: str) -> bool:
         path_to_check = Path(self.hook.get_path()) / path
-        return path_to_check.is_file()
+        return path_to_check.exists() and path_to_check.is_file()
 
     def check_prefix(self, prefix: str) -> bool:
         path_to_check = Path(self.hook.get_path()) / prefix
-        return path_to_check.exists()
+        return path_to_check.exists() and path_to_check.is_dir()
 
     def list_files(self, prefix: str) -> list[str]:
         path_to_list = Path(self.hook.get_path()) / prefix
         return [str(file) for file in path_to_list.glob("*") if file.is_file()]
```

### Comparing `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/s3_filesystem.py` & `airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/s3_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/filesystems/impl/sftp_filesystem.py` & `airflow_tools-0.8.6/src/airflow_tools/filesystems/impl/sftp_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/notifications/slack/webhook.py` & `airflow_tools-0.8.6/src/airflow_tools/notifications/slack/webhook.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/providers/azure/hooks/azure_databricks.py` & `airflow_tools-0.8.6/src/airflow_tools/providers/azure/hooks/azure_databricks.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/providers/azure/hooks/azure_file_share.py` & `airflow_tools-0.8.6/src/airflow_tools/providers/azure/hooks/azure_file_share.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/providers/data_lake/operators/data_lake.py` & `airflow_tools-0.8.6/src/airflow_tools/providers/data_lake/operators/data_lake.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/operators/filesystem.py` & `airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/operators/filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py` & `airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/operators/http_to_filesystem.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/providers/filesystem/tasks.py` & `airflow_tools-0.8.6/src/airflow_tools/providers/filesystem/tasks.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py` & `airflow_tools-0.8.6/src/airflow_tools/providers/http_to_data_lake/operators/http_to_data_lake.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/src/airflow_tools/providers/package.py` & `airflow_tools-0.8.6/src/airflow_tools/providers/package.py`

 * *Files identical despite different names*

### Comparing `airflow_tools-0.8.5/PKG-INFO` & `airflow_tools-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-tools
-Version: 0.8.5
+Version: 0.8.6
 Summary: 
 Author: Biel Llobera
 Author-email: biel_llobera@dkl.digital
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airflow-tools Version: 0.8.5 Summary: Author: Biel
+Metadata-Version: 2.1 Name: airflow-tools Version: 0.8.6 Summary: Author: Biel
 Llobera Author-email: biel_llobera@dkl.digital Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: apache-
 airflow (==2.8.*) Requires-Dist: apache-airflow-providers-amazon
 (>=8.8.0,<9.0.0) Requires-Dist: apache-airflow-providers-microsoft-azure
 (>=8.0.0,<9.0.0) Requires-Dist: apache-airflow-providers-sftp (>=4.8.1,<5.0.0)
```

