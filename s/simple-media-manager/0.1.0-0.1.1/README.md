# Comparing `tmp/simple_media_manager-0.1.0.tar.gz` & `tmp/simple_media_manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_media_manager-0.1.0.tar", max compression
+gzip compressed data, was "simple_media_manager-0.1.1.tar", max compression
```

## Comparing `simple_media_manager-0.1.0.tar` & `simple_media_manager-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      767 2024-04-19 08:43:37.694901 simple_media_manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.196430 simple_media_manager-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-19 06:26:01.604320 simple_media_manager-0.1.0/simple_media_manager/__init__.py
--rw-r--r--   0        0        0       85 2024-04-19 08:48:06.059508 simple_media_manager-0.1.0/simple_media_manager/admin.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.197179 simple_media_manager-0.1.0/simple_media_manager/application/__init__.py
--rw-r--r--   0        0        0       26 2024-02-09 16:22:47.199185 simple_media_manager-0.1.0/simple_media_manager/application/dependency/__init__.py
--rw-r--r--   0        0        0      414 2024-04-19 06:27:23.141068 simple_media_manager-0.1.0/simple_media_manager/application/dependency/registry.py
--rw-r--r--   0        0        0      176 2024-04-19 06:26:01.602821 simple_media_manager-0.1.0/simple_media_manager/apps.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.203188 simple_media_manager-0.1.0/simple_media_manager/domain/__init__.py
--rw-r--r--   0        0        0      101 2024-02-09 16:22:47.203692 simple_media_manager-0.1.0/simple_media_manager/domain/command/__init__.py
--rw-r--r--   0        0        0      938 2024-04-19 06:27:23.128551 simple_media_manager-0.1.0/simple_media_manager/domain/command/image.py
--rw-r--r--   0        0        0       94 2024-02-09 16:22:47.204695 simple_media_manager-0.1.0/simple_media_manager/domain/repository/__init__.py
--rw-r--r--   0        0        0     1690 2024-02-09 16:22:47.204695 simple_media_manager-0.1.0/simple_media_manager/domain/repository/image.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.205194 simple_media_manager-0.1.0/simple_media_manager/infrastructure/__init__.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.205194 simple_media_manager-0.1.0/simple_media_manager/infrastructure/adapters/__init__.py
--rw-r--r--   0        0        0     1468 2024-04-19 06:27:23.126044 simple_media_manager-0.1.0/simple_media_manager/infrastructure/adapters/image.py
--rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 20:25:02.937865 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/class_responses/__init__.py
--rw-r--r--   0        0        0      738 2024-03-30 19:22:07.519967 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/class_responses/error_response.py
--rw-r--r--   0        0        0        0 2024-03-27 18:46:29.371811 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/data_responses/__init__.py
--rw-r--r--   0        0        0      132 2024-03-27 19:20:26.473062 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/data_responses/data_response.py
--rw-r--r--   0        0        0     7766 2024-04-19 08:44:17.849804 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/exception_handlers.py
--rw-r--r--   0        0        0     2094 2024-04-19 07:02:52.805267 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/pagination.py
--rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/serializers/__init__.py
--rw-r--r--   0        0        0      166 2024-03-01 10:40:40.967046 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/serializers/common_serializer.py
--rw-r--r--   0        0        0        0 2024-02-23 09:25:48.358460 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/serializers/custom_fields/__init__.py
--rw-r--r--   0        0        0     2047 2024-02-23 09:25:48.358960 simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/serializers/custom_fields/fields.py
--rw-r--r--   0        0        0      991 2024-04-19 06:56:02.120922 simple_media_manager-0.1.0/simple_media_manager/infrastructure/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.206692 simple_media_manager-0.1.0/simple_media_manager/infrastructure/migrations/__init__.py
--rw-r--r--   0        0        0       22 2024-02-09 16:22:47.205692 simple_media_manager-0.1.0/simple_media_manager/infrastructure/models/__init__.py
--rw-r--r--   0        0        0      375 2024-04-19 07:00:07.952897 simple_media_manager-0.1.0/simple_media_manager/infrastructure/models/file.py
--rw-r--r--   0        0        0      184 2024-04-19 08:36:46.181930 simple_media_manager-0.1.0/simple_media_manager/infrastructure/models/image.py
--rw-r--r--   0        0        0        0 2024-02-23 20:41:56.964740 simple_media_manager-0.1.0/simple_media_manager/presentation/__init__.py
--rw-r--r--   0        0        0        4 2024-02-09 16:22:47.197179 simple_media_manager-0.1.0/simple_media_manager/presentation/apis/__init__.py
--rw-r--r--   0        0        0     4337 2024-04-19 08:33:53.576207 simple_media_manager-0.1.0/simple_media_manager/presentation/apis/image.py
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.197678 simple_media_manager-0.1.0/simple_media_manager/presentation/apis/serializers/__init__.py
--rw-r--r--   0        0        0     1024 2024-04-19 07:15:40.566637 simple_media_manager-0.1.0/simple_media_manager/presentation/apis/serializers/image.py
--rw-r--r--   0        0        0      491 2024-04-19 06:27:23.110546 simple_media_manager-0.1.0/simple_media_manager/urls.py
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 simple_media_manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      766 2024-04-19 09:09:19.073463 simple_media_manager-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.196430 simple_media_manager-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 06:26:01.604320 simple_media_manager-0.1.1/simple_media_manager/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-19 08:48:06.059508 simple_media_manager-0.1.1/simple_media_manager/admin.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.197179 simple_media_manager-0.1.1/simple_media_manager/application/__init__.py
+-rw-r--r--   0        0        0       26 2024-02-09 16:22:47.199185 simple_media_manager-0.1.1/simple_media_manager/application/dependency/__init__.py
+-rw-r--r--   0        0        0      414 2024-04-19 06:27:23.141068 simple_media_manager-0.1.1/simple_media_manager/application/dependency/registry.py
+-rw-r--r--   0        0        0      176 2024-04-19 06:26:01.602821 simple_media_manager-0.1.1/simple_media_manager/apps.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.203188 simple_media_manager-0.1.1/simple_media_manager/domain/__init__.py
+-rw-r--r--   0        0        0      101 2024-02-09 16:22:47.203692 simple_media_manager-0.1.1/simple_media_manager/domain/command/__init__.py
+-rw-r--r--   0        0        0      938 2024-04-19 06:27:23.128551 simple_media_manager-0.1.1/simple_media_manager/domain/command/image.py
+-rw-r--r--   0        0        0       94 2024-02-09 16:22:47.204695 simple_media_manager-0.1.1/simple_media_manager/domain/repository/__init__.py
+-rw-r--r--   0        0        0     1690 2024-02-09 16:22:47.204695 simple_media_manager-0.1.1/simple_media_manager/domain/repository/image.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.205194 simple_media_manager-0.1.1/simple_media_manager/infrastructure/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.205194 simple_media_manager-0.1.1/simple_media_manager/infrastructure/adapters/__init__.py
+-rw-r--r--   0        0        0     1468 2024-04-19 06:27:23.126044 simple_media_manager-0.1.1/simple_media_manager/infrastructure/adapters/image.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 20:25:02.937865 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/class_responses/__init__.py
+-rw-r--r--   0        0        0      738 2024-03-30 19:22:07.519967 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/class_responses/error_response.py
+-rw-r--r--   0        0        0        0 2024-03-27 18:46:29.371811 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/data_responses/__init__.py
+-rw-r--r--   0        0        0      132 2024-03-27 19:20:26.473062 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/data_responses/data_response.py
+-rw-r--r--   0        0        0     7766 2024-04-19 08:44:17.849804 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/exception_handlers.py
+-rw-r--r--   0        0        0     2094 2024-04-19 07:02:52.805267 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/pagination.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/serializers/__init__.py
+-rw-r--r--   0        0        0      166 2024-03-01 10:40:40.967046 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/serializers/common_serializer.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:25:48.358460 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/serializers/custom_fields/__init__.py
+-rw-r--r--   0        0        0     2047 2024-02-23 09:25:48.358960 simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/serializers/custom_fields/fields.py
+-rw-r--r--   0        0        0      991 2024-04-19 06:56:02.120922 simple_media_manager-0.1.1/simple_media_manager/infrastructure/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.206692 simple_media_manager-0.1.1/simple_media_manager/infrastructure/migrations/__init__.py
+-rw-r--r--   0        0        0       22 2024-02-09 16:22:47.205692 simple_media_manager-0.1.1/simple_media_manager/infrastructure/models/__init__.py
+-rw-r--r--   0        0        0      375 2024-04-19 07:00:07.952897 simple_media_manager-0.1.1/simple_media_manager/infrastructure/models/file.py
+-rw-r--r--   0        0        0      184 2024-04-19 08:36:46.181930 simple_media_manager-0.1.1/simple_media_manager/infrastructure/models/image.py
+-rw-r--r--   0        0        0        0 2024-02-23 20:41:56.964740 simple_media_manager-0.1.1/simple_media_manager/presentation/__init__.py
+-rw-r--r--   0        0        0        4 2024-02-09 16:22:47.197179 simple_media_manager-0.1.1/simple_media_manager/presentation/apis/__init__.py
+-rw-r--r--   0        0        0     4337 2024-04-19 08:33:53.576207 simple_media_manager-0.1.1/simple_media_manager/presentation/apis/image.py
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.197678 simple_media_manager-0.1.1/simple_media_manager/presentation/apis/serializers/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-19 07:15:40.566637 simple_media_manager-0.1.1/simple_media_manager/presentation/apis/serializers/image.py
+-rw-r--r--   0        0        0      491 2024-04-19 06:27:23.110546 simple_media_manager-0.1.1/simple_media_manager/urls.py
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 simple_media_manager-0.1.1/PKG-INFO
```

### Comparing `simple_media_manager-0.1.0/pyproject.toml` & `simple_media_manager-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple-media-manager"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["aliseylaneh <aliseylaneh@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -19,14 +19,14 @@
 drf-jwt = "1.19.2"
 boto3 = "1.24.71"
 attrs = "22.1.0"
 djangorestframework-simplejwt = "5.2.2"
 drf-spectacular = "0.24.2"
 django-redis = "5.2.0"
 setuptools = "69.0.3"
-djangorestframework = "^3.15.1"
 djangorestframework-camel-case = "^1.4.2"
+djangorestframework = "3.13.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `simple_media_manager-0.1.0/simple_media_manager/domain/command/image.py` & `simple_media_manager-0.1.1/simple_media_manager/domain/command/image.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.0/simple_media_manager/domain/repository/image.py` & `simple_media_manager-0.1.1/simple_media_manager/domain/repository/image.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.0/simple_media_manager/infrastructure/adapters/image.py` & `simple_media_manager-0.1.1/simple_media_manager/infrastructure/adapters/image.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/class_responses/error_response.py` & `simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/class_responses/error_response.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/exception_handlers.py` & `simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/pagination.py` & `simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/pagination.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.0/simple_media_manager/infrastructure/common/serializers/custom_fields/fields.py` & `simple_media_manager-0.1.1/simple_media_manager/infrastructure/common/serializers/custom_fields/fields.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.0/simple_media_manager/infrastructure/migrations/0001_initial.py` & `simple_media_manager-0.1.1/simple_media_manager/infrastructure/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.0/simple_media_manager/presentation/apis/image.py` & `simple_media_manager-0.1.1/simple_media_manager/presentation/apis/image.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.0/simple_media_manager/presentation/apis/serializers/image.py` & `simple_media_manager-0.1.1/simple_media_manager/presentation/apis/serializers/image.py`

 * *Files identical despite different names*

### Comparing `simple_media_manager-0.1.0/PKG-INFO` & `simple_media_manager-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-media-manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: aliseylaneh
 Author-email: aliseylaneh@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Dist: django (==4.0.7)
 Requires-Dist: django-cors-headers (==3.13.0)
 Requires-Dist: django-environ (==0.9.0)
 Requires-Dist: django-extensions (==3.2.1)
 Requires-Dist: django-filter (==22.1)
 Requires-Dist: django-redis (==5.2.0)
 Requires-Dist: django-storages (==1.13.1)
-Requires-Dist: djangorestframework (>=3.15.1,<4.0.0)
+Requires-Dist: djangorestframework (==3.13.1)
 Requires-Dist: djangorestframework-camel-case (>=1.4.2,<2.0.0)
 Requires-Dist: djangorestframework-simplejwt (==5.2.2)
 Requires-Dist: drf-jwt (==1.19.2)
 Requires-Dist: drf-spectacular (==0.24.2)
 Requires-Dist: psycopg2-binary (==2.9.9)
 Requires-Dist: setuptools (==69.0.3)
 Requires-Dist: whitenoise (==6.2.0)
```

