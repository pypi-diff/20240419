# Comparing `tmp/simple_media_manager-0.1.2.tar.gz` & `tmp/simple_media_manager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_media_manager-0.1.2.tar", max compression
+gzip compressed data, was "simple_media_manager-0.1.3.tar", max compression
```

## Comparing `simple_media_manager-0.1.2.tar` & `simple_media_manager-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0      788 2024-04-19 10:24:53.290591 simple_media_manager-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.196430 simple_media_manager-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-19 06:26:01.604320 simple_media_manager-0.1.2/simple_media_manager/__init__.py
--rw-r--r--   0        0        0       85 2024-04-19 08:48:06.059508 simple_media_manager-0.1.2/simple_media_manager/admin.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.197179 simple_media_manager-0.1.2/simple_media_manager/application/__init__.py
--rw-r--r--   0        0        0       26 2024-02-09 16:22:47.199185 simple_media_manager-0.1.2/simple_media_manager/application/dependency/__init__.py
--rw-r--r--   0        0        0      414 2024-04-19 06:27:23.141068 simple_media_manager-0.1.2/simple_media_manager/application/dependency/registry.py
--rw-r--r--   0        0        0      176 2024-04-19 06:26:01.602821 simple_media_manager-0.1.2/simple_media_manager/apps.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.203188 simple_media_manager-0.1.2/simple_media_manager/domain/__init__.py
--rw-r--r--   0        0        0      101 2024-02-09 16:22:47.203692 simple_media_manager-0.1.2/simple_media_manager/domain/command/__init__.py
--rw-r--r--   0        0        0      938 2024-04-19 06:27:23.128551 simple_media_manager-0.1.2/simple_media_manager/domain/command/image.py
--rw-r--r--   0        0        0       94 2024-02-09 16:22:47.204695 simple_media_manager-0.1.2/simple_media_manager/domain/repository/__init__.py
--rw-r--r--   0        0        0     1690 2024-02-09 16:22:47.204695 simple_media_manager-0.1.2/simple_media_manager/domain/repository/image.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.205194 simple_media_manager-0.1.2/simple_media_manager/infrastructure/__init__.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.205194 simple_media_manager-0.1.2/simple_media_manager/infrastructure/adapters/__init__.py
--rw-r--r--   0        0        0     1468 2024-04-19 06:27:23.126044 simple_media_manager-0.1.2/simple_media_manager/infrastructure/adapters/image.py
--rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 20:25:02.937865 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/class_responses/__init__.py
--rw-r--r--   0        0        0      738 2024-03-30 19:22:07.519967 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/class_responses/error_response.py
--rw-r--r--   0        0        0        0 2024-03-27 18:46:29.371811 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/data_responses/__init__.py
--rw-r--r--   0        0        0      132 2024-03-27 19:20:26.473062 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/data_responses/data_response.py
--rw-r--r--   0        0        0     7766 2024-04-19 08:44:17.849804 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/exception_handlers.py
--rw-r--r--   0        0        0     2094 2024-04-19 07:02:52.805267 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/pagination.py
--rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/serializers/__init__.py
--rw-r--r--   0        0        0      166 2024-03-01 10:40:40.967046 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/serializers/common_serializer.py
--rw-r--r--   0        0        0        0 2024-02-23 09:25:48.358460 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/serializers/custom_fields/__init__.py
--rw-r--r--   0        0        0     2047 2024-02-23 09:25:48.358960 simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/serializers/custom_fields/fields.py
--rw-r--r--   0        0        0      984 2024-04-19 10:27:16.885651 simple_media_manager-0.1.2/simple_media_manager/infrastructure/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.206692 simple_media_manager-0.1.2/simple_media_manager/infrastructure/migrations/__init__.py
--rw-r--r--   0        0        0       22 2024-02-09 16:22:47.205692 simple_media_manager-0.1.2/simple_media_manager/infrastructure/models/__init__.py
--rw-r--r--   0        0        0      389 2024-04-19 10:20:52.059597 simple_media_manager-0.1.2/simple_media_manager/infrastructure/models/file.py
--rw-r--r--   0        0        0      177 2024-04-19 10:22:27.263915 simple_media_manager-0.1.2/simple_media_manager/infrastructure/models/image.py
--rw-r--r--   0        0        0        0 2024-02-23 20:41:56.964740 simple_media_manager-0.1.2/simple_media_manager/presentation/__init__.py
--rw-r--r--   0        0        0        4 2024-02-09 16:22:47.197179 simple_media_manager-0.1.2/simple_media_manager/presentation/apis/__init__.py
--rw-r--r--   0        0        0     4337 2024-04-19 08:33:53.576207 simple_media_manager-0.1.2/simple_media_manager/presentation/apis/image.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.197678 simple_media_manager-0.1.2/simple_media_manager/presentation/apis/serializers/__init__.py
--rw-r--r--   0        0        0     1024 2024-04-19 07:15:40.566637 simple_media_manager-0.1.2/simple_media_manager/presentation/apis/serializers/image.py
--rw-r--r--   0        0        0      491 2024-04-19 06:27:23.110546 simple_media_manager-0.1.2/simple_media_manager/urls.py
--rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 simple_media_manager-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      788 2024-04-19 12:13:22.083701 simple_media_manager-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.196430 simple_media_manager-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 06:26:01.604320 simple_media_manager-0.1.3/simple_media_manager/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-19 08:48:06.059508 simple_media_manager-0.1.3/simple_media_manager/admin.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.197179 simple_media_manager-0.1.3/simple_media_manager/application/__init__.py
+-rw-r--r--   0        0        0       26 2024-02-09 16:22:47.199185 simple_media_manager-0.1.3/simple_media_manager/application/dependency/__init__.py
+-rw-r--r--   0        0        0      414 2024-04-19 06:27:23.141068 simple_media_manager-0.1.3/simple_media_manager/application/dependency/registry.py
+-rw-r--r--   0        0        0      176 2024-04-19 06:26:01.602821 simple_media_manager-0.1.3/simple_media_manager/apps.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.203188 simple_media_manager-0.1.3/simple_media_manager/domain/__init__.py
+-rw-r--r--   0        0        0      101 2024-02-09 16:22:47.203692 simple_media_manager-0.1.3/simple_media_manager/domain/command/__init__.py
+-rw-r--r--   0        0        0      938 2024-04-19 06:27:23.128551 simple_media_manager-0.1.3/simple_media_manager/domain/command/image.py
+-rw-r--r--   0        0        0       94 2024-02-09 16:22:47.204695 simple_media_manager-0.1.3/simple_media_manager/domain/repository/__init__.py
+-rw-r--r--   0        0        0     1690 2024-02-09 16:22:47.204695 simple_media_manager-0.1.3/simple_media_manager/domain/repository/image.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.205194 simple_media_manager-0.1.3/simple_media_manager/infrastructure/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.205194 simple_media_manager-0.1.3/simple_media_manager/infrastructure/adapters/__init__.py
+-rw-r--r--   0        0        0     1468 2024-04-19 06:27:23.126044 simple_media_manager-0.1.3/simple_media_manager/infrastructure/adapters/image.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 20:25:02.937865 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/class_responses/__init__.py
+-rw-r--r--   0        0        0      738 2024-03-30 19:22:07.519967 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/class_responses/error_response.py
+-rw-r--r--   0        0        0        0 2024-03-27 18:46:29.371811 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/data_responses/__init__.py
+-rw-r--r--   0        0        0      132 2024-03-27 19:20:26.473062 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/data_responses/data_response.py
+-rw-r--r--   0        0        0     7766 2024-04-19 08:44:17.849804 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/exception_handlers.py
+-rw-r--r--   0        0        0     2094 2024-04-19 07:02:52.805267 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/pagination.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/serializers/__init__.py
+-rw-r--r--   0        0        0      166 2024-03-01 10:40:40.967046 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/serializers/common_serializer.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:25:48.358460 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/serializers/custom_fields/__init__.py
+-rw-r--r--   0        0        0     2047 2024-02-23 09:25:48.358960 simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/serializers/custom_fields/fields.py
+-rw-r--r--   0        0        0      984 2024-04-19 10:27:16.885651 simple_media_manager-0.1.3/simple_media_manager/infrastructure/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.206692 simple_media_manager-0.1.3/simple_media_manager/infrastructure/migrations/__init__.py
+-rw-r--r--   0        0        0       22 2024-02-09 16:22:47.205692 simple_media_manager-0.1.3/simple_media_manager/infrastructure/models/__init__.py
+-rw-r--r--   0        0        0      389 2024-04-19 10:20:52.059597 simple_media_manager-0.1.3/simple_media_manager/infrastructure/models/file.py
+-rw-r--r--   0        0        0      177 2024-04-19 10:22:27.263915 simple_media_manager-0.1.3/simple_media_manager/infrastructure/models/image.py
+-rw-r--r--   0        0        0        0 2024-02-23 20:41:56.964740 simple_media_manager-0.1.3/simple_media_manager/presentation/__init__.py
+-rw-r--r--   0        0        0        4 2024-02-09 16:22:47.197179 simple_media_manager-0.1.3/simple_media_manager/presentation/apis/__init__.py
+-rw-r--r--   0        0        0     4337 2024-04-19 08:33:53.576207 simple_media_manager-0.1.3/simple_media_manager/presentation/apis/image.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.197678 simple_media_manager-0.1.3/simple_media_manager/presentation/apis/serializers/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-19 07:15:40.566637 simple_media_manager-0.1.3/simple_media_manager/presentation/apis/serializers/image.py
+-rw-r--r--   0        0        0      323 2024-04-19 12:12:02.156105 simple_media_manager-0.1.3/simple_media_manager/settings.py
+-rw-r--r--   0        0        0      491 2024-04-19 06:27:23.110546 simple_media_manager-0.1.3/simple_media_manager/urls.py
+-rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 simple_media_manager-0.1.3/PKG-INFO
```

### Comparing `simple_media_manager-0.1.2/pyproject.toml` & `simple_media_manager-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple-media-manager"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["aliseylaneh <aliseylaneh@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `simple_media_manager-0.1.2/simple_media_manager/domain/command/image.py` & `simple_media_manager-0.1.3/simple_media_manager/domain/command/image.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.2/simple_media_manager/domain/repository/image.py` & `simple_media_manager-0.1.3/simple_media_manager/domain/repository/image.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.2/simple_media_manager/infrastructure/adapters/image.py` & `simple_media_manager-0.1.3/simple_media_manager/infrastructure/adapters/image.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/class_responses/error_response.py` & `simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/class_responses/error_response.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/exception_handlers.py` & `simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/pagination.py` & `simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/pagination.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.2/simple_media_manager/infrastructure/common/serializers/custom_fields/fields.py` & `simple_media_manager-0.1.3/simple_media_manager/infrastructure/common/serializers/custom_fields/fields.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.2/simple_media_manager/infrastructure/migrations/0001_initial.py` & `simple_media_manager-0.1.3/simple_media_manager/infrastructure/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.2/simple_media_manager/presentation/apis/image.py` & `simple_media_manager-0.1.3/simple_media_manager/presentation/apis/image.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.2/simple_media_manager/presentation/apis/serializers/image.py` & `simple_media_manager-0.1.3/simple_media_manager/presentation/apis/serializers/image.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.2/PKG-INFO` & `simple_media_manager-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-media-manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: aliseylaneh
 Author-email: aliseylaneh@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

