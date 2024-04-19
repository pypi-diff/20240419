# Comparing `tmp/django_microservice_common-0.1.6.tar.gz` & `tmp/django_microservice_common-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_microservice_common-0.1.6.tar", max compression
+gzip compressed data, was "django_microservice_common-0.1.7.tar", max compression
```

## Comparing `django_microservice_common-0.1.6.tar` & `django_microservice_common-0.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0        0 2024-01-04 16:31:34.906617 django_microservice_common-0.1.6/django_microservice_common/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 django_microservice_common-0.1.6/django_microservice_common/api/__init__.py
--rw-r--r--   0        0        0      651 2024-04-19 09:21:26.744752 django_microservice_common-0.1.6/django_microservice_common/api/api_view.py
--rw-r--r--   0        0        0        0 2024-03-27 20:25:02.937865 django_microservice_common-0.1.6/django_microservice_common/api/class_responses/__init__.py
--rw-r--r--   0        0        0      738 2024-03-30 19:22:07.519967 django_microservice_common-0.1.6/django_microservice_common/api/class_responses/error_response.py
--rw-r--r--   0        0        0        0 2024-03-27 18:46:29.371811 django_microservice_common-0.1.6/django_microservice_common/api/data_responses/__init__.py
--rw-r--r--   0        0        0      132 2024-03-27 19:20:26.473062 django_microservice_common-0.1.6/django_microservice_common/api/data_responses/data_response.py
--rw-r--r--   0        0        0     7658 2024-04-19 09:21:26.745252 django_microservice_common-0.1.6/django_microservice_common/api/exception_handlers.py
--rw-r--r--   0        0        0     1105 2024-01-04 16:31:34.904606 django_microservice_common-0.1.6/django_microservice_common/api/mixins.py
--rw-r--r--   0        0        0     2090 2024-01-04 16:31:34.904606 django_microservice_common-0.1.6/django_microservice_common/api/pagination.py
--rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 django_microservice_common-0.1.6/django_microservice_common/api/serializers/__init__.py
--rw-r--r--   0        0        0      166 2024-03-01 10:40:40.967046 django_microservice_common-0.1.6/django_microservice_common/api/serializers/common_serializer.py
--rw-r--r--   0        0        0        0 2024-02-23 09:25:48.358460 django_microservice_common-0.1.6/django_microservice_common/api/serializers/custom_fields/__init__.py
--rw-r--r--   0        0        0     2047 2024-02-23 09:25:48.358960 django_microservice_common-0.1.6/django_microservice_common/api/serializers/custom_fields/fields.py
--rw-r--r--   0        0        0      419 2024-01-04 16:31:34.905115 django_microservice_common-0.1.6/django_microservice_common/api/utils.py
--rw-r--r--   0        0        0      261 2024-04-19 09:20:42.606665 django_microservice_common-0.1.6/django_microservice_common/apps.py
--rw-r--r--   0        0        0        0 2024-03-07 09:20:24.096957 django_microservice_common-0.1.6/django_microservice_common/authorization/__init__.py
--rw-r--r--   0        0        0      716 2024-03-07 09:29:14.886407 django_microservice_common-0.1.6/django_microservice_common/authorization/enums.py
--rw-r--r--   0        0        0      285 2024-03-07 09:56:04.815774 django_microservice_common-0.1.6/django_microservice_common/authorization/exceptions.py
--rw-r--r--   0        0        0      347 2024-03-14 07:39:10.868897 django_microservice_common-0.1.6/django_microservice_common/authorization/grants.py
--rw-r--r--   0        0        0      172 2024-03-14 07:39:12.953128 django_microservice_common-0.1.6/django_microservice_common/authorization/grants_func.py
--rw-r--r--   0        0        0     1088 2024-03-14 07:39:12.602386 django_microservice_common-0.1.6/django_microservice_common/authorization/mapper.py
--rw-r--r--   0        0        0      192 2024-03-16 18:53:20.757793 django_microservice_common-0.1.6/django_microservice_common/authorization/roles.py
--rw-r--r--   0        0        0      210 2024-03-17 20:37:22.815545 django_microservice_common-0.1.6/django_microservice_common/authorization/validators.py
--rw-r--r--   0        0        0       55 2023-11-16 11:00:48.634630 django_microservice_common-0.1.6/django_microservice_common/dependency_manager/__init__.py
--rw-r--r--   0        0        0     1404 2024-04-19 09:21:26.745752 django_microservice_common-0.1.6/django_microservice_common/dependency_manager/container.py
--rw-r--r--   0        0        0      122 2024-02-23 19:26:04.983081 django_microservice_common-0.1.6/django_microservice_common/dependency_manager/registry.py
--rw-r--r--   0        0        0        0 2024-02-23 20:02:43.782079 django_microservice_common-0.1.6/django_microservice_common/exceptions/__init__.py
--rw-r--r--   0        0        0      185 2024-02-20 16:25:25.324908 django_microservice_common-0.1.6/django_microservice_common/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-23 19:33:24.530743 django_microservice_common-0.1.6/django_microservice_common/migrations/__init__.py
--rw-r--r--   0        0        0       27 2024-02-23 19:28:50.313726 django_microservice_common-0.1.6/django_microservice_common/models/__init__.py
--rw-r--r--   0        0        0      425 2024-03-01 10:43:08.540480 django_microservice_common-0.1.6/django_microservice_common/models/base_model.py
--rw-r--r--   0        0        0        0 2024-02-23 19:23:38.738916 django_microservice_common-0.1.6/django_microservice_common/services/__init__.py
--rw-r--r--   0        0        0     1505 2024-02-23 19:24:05.923066 django_microservice_common-0.1.6/django_microservice_common/services/services.py
--rw-r--r--   0        0        0        0 2024-02-23 19:23:27.086623 django_microservice_common-0.1.6/django_microservice_common/types/__init__.py
--rw-r--r--   0        0        0      261 2024-01-04 16:31:34.908619 django_microservice_common-0.1.6/django_microservice_common/types/types.py
--rw-r--r--   0        0        0        0 2024-02-23 19:25:09.081927 django_microservice_common-0.1.6/django_microservice_common/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 19:25:15.469691 django_microservice_common-0.1.6/django_microservice_common/utils/django/__init__.py
--rw-r--r--   0        0        0     1366 2024-02-23 19:32:24.949313 django_microservice_common-0.1.6/django_microservice_common/utils/django/utils.py
--rw-r--r--   0        0        0        0 2024-02-23 19:32:14.673528 django_microservice_common-0.1.6/django_microservice_common/utils/drf/__init__.py
--rw-r--r--   0        0        0      418 2024-02-23 19:32:37.981929 django_microservice_common-0.1.6/django_microservice_common/utils/drf/utils.py
--rw-r--r--   0        0        0      215 2023-11-16 11:00:48.645630 django_microservice_common-0.1.6/django_microservice_common/utils/singletone.py
--rw-r--r--   0        0        0      834 2024-04-19 09:17:46.065992 django_microservice_common-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-09 16:22:47.196430 django_microservice_common-0.1.6/README.md
--rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 django_microservice_common-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-04 16:31:34.906617 django_microservice_common-0.1.7/django_microservice_common/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 django_microservice_common-0.1.7/django_microservice_common/api/__init__.py
+-rw-r--r--   0        0        0      651 2024-04-19 09:21:26.744752 django_microservice_common-0.1.7/django_microservice_common/api/api_view.py
+-rw-r--r--   0        0        0        0 2024-03-27 20:25:02.937865 django_microservice_common-0.1.7/django_microservice_common/api/class_responses/__init__.py
+-rw-r--r--   0        0        0      738 2024-03-30 19:22:07.519967 django_microservice_common-0.1.7/django_microservice_common/api/class_responses/error_response.py
+-rw-r--r--   0        0        0        0 2024-03-27 18:46:29.371811 django_microservice_common-0.1.7/django_microservice_common/api/data_responses/__init__.py
+-rw-r--r--   0        0        0      132 2024-03-27 19:20:26.473062 django_microservice_common-0.1.7/django_microservice_common/api/data_responses/data_response.py
+-rw-r--r--   0        0        0     7658 2024-04-19 09:21:26.745252 django_microservice_common-0.1.7/django_microservice_common/api/exception_handlers.py
+-rw-r--r--   0        0        0     1105 2024-01-04 16:31:34.904606 django_microservice_common-0.1.7/django_microservice_common/api/mixins.py
+-rw-r--r--   0        0        0     2090 2024-01-04 16:31:34.904606 django_microservice_common-0.1.7/django_microservice_common/api/pagination.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:25:48.357959 django_microservice_common-0.1.7/django_microservice_common/api/serializers/__init__.py
+-rw-r--r--   0        0        0      166 2024-03-01 10:40:40.967046 django_microservice_common-0.1.7/django_microservice_common/api/serializers/common_serializer.py
+-rw-r--r--   0        0        0        0 2024-02-23 09:25:48.358460 django_microservice_common-0.1.7/django_microservice_common/api/serializers/custom_fields/__init__.py
+-rw-r--r--   0        0        0     2047 2024-02-23 09:25:48.358960 django_microservice_common-0.1.7/django_microservice_common/api/serializers/custom_fields/fields.py
+-rw-r--r--   0        0        0      419 2024-01-04 16:31:34.905115 django_microservice_common-0.1.7/django_microservice_common/api/utils.py
+-rw-r--r--   0        0        0      261 2024-04-19 09:20:42.606665 django_microservice_common-0.1.7/django_microservice_common/apps.py
+-rw-r--r--   0        0        0        0 2024-03-07 09:20:24.096957 django_microservice_common-0.1.7/django_microservice_common/authorization/__init__.py
+-rw-r--r--   0        0        0      716 2024-03-07 09:29:14.886407 django_microservice_common-0.1.7/django_microservice_common/authorization/enums.py
+-rw-r--r--   0        0        0      285 2024-03-07 09:56:04.815774 django_microservice_common-0.1.7/django_microservice_common/authorization/exceptions.py
+-rw-r--r--   0        0        0      347 2024-03-14 07:39:10.868897 django_microservice_common-0.1.7/django_microservice_common/authorization/grants.py
+-rw-r--r--   0        0        0      172 2024-03-14 07:39:12.953128 django_microservice_common-0.1.7/django_microservice_common/authorization/grants_func.py
+-rw-r--r--   0        0        0     1088 2024-03-14 07:39:12.602386 django_microservice_common-0.1.7/django_microservice_common/authorization/mapper.py
+-rw-r--r--   0        0        0      192 2024-03-16 18:53:20.757793 django_microservice_common-0.1.7/django_microservice_common/authorization/roles.py
+-rw-r--r--   0        0        0      210 2024-03-17 20:37:22.815545 django_microservice_common-0.1.7/django_microservice_common/authorization/validators.py
+-rw-r--r--   0        0        0       55 2023-11-16 11:00:48.634630 django_microservice_common-0.1.7/django_microservice_common/dependency_manager/__init__.py
+-rw-r--r--   0        0        0     1404 2024-04-19 09:21:26.745752 django_microservice_common-0.1.7/django_microservice_common/dependency_manager/container.py
+-rw-r--r--   0        0        0      122 2024-02-23 19:26:04.983081 django_microservice_common-0.1.7/django_microservice_common/dependency_manager/registry.py
+-rw-r--r--   0        0        0        0 2024-02-23 20:02:43.782079 django_microservice_common-0.1.7/django_microservice_common/exceptions/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-20 16:25:25.324908 django_microservice_common-0.1.7/django_microservice_common/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-23 19:33:24.530743 django_microservice_common-0.1.7/django_microservice_common/migrations/__init__.py
+-rw-r--r--   0        0        0       27 2024-02-23 19:28:50.313726 django_microservice_common-0.1.7/django_microservice_common/models/__init__.py
+-rw-r--r--   0        0        0      425 2024-03-01 10:43:08.540480 django_microservice_common-0.1.7/django_microservice_common/models/base_model.py
+-rw-r--r--   0        0        0        0 2024-02-23 19:23:38.738916 django_microservice_common-0.1.7/django_microservice_common/services/__init__.py
+-rw-r--r--   0        0        0     1505 2024-02-23 19:24:05.923066 django_microservice_common-0.1.7/django_microservice_common/services/services.py
+-rw-r--r--   0        0        0        0 2024-02-23 19:23:27.086623 django_microservice_common-0.1.7/django_microservice_common/types/__init__.py
+-rw-r--r--   0        0        0      261 2024-01-04 16:31:34.908619 django_microservice_common-0.1.7/django_microservice_common/types/types.py
+-rw-r--r--   0        0        0        0 2024-02-23 19:25:09.081927 django_microservice_common-0.1.7/django_microservice_common/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 19:25:15.469691 django_microservice_common-0.1.7/django_microservice_common/utils/django/__init__.py
+-rw-r--r--   0        0        0     1366 2024-02-23 19:32:24.949313 django_microservice_common-0.1.7/django_microservice_common/utils/django/utils.py
+-rw-r--r--   0        0        0        0 2024-02-23 19:32:14.673528 django_microservice_common-0.1.7/django_microservice_common/utils/drf/__init__.py
+-rw-r--r--   0        0        0      418 2024-02-23 19:32:37.981929 django_microservice_common-0.1.7/django_microservice_common/utils/drf/utils.py
+-rw-r--r--   0        0        0      215 2023-11-16 11:00:48.645630 django_microservice_common-0.1.7/django_microservice_common/utils/singletone.py
+-rw-r--r--   0        0        0      834 2024-04-19 10:11:16.753322 django_microservice_common-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-09 16:22:47.196430 django_microservice_common-0.1.7/README.md
+-rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 django_microservice_common-0.1.7/PKG-INFO
```

### Comparing `django_microservice_common-0.1.6/django_microservice_common/api/api_view.py` & `django_microservice_common-0.1.7/django_microservice_common/api/api_view.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/django_microservice_common/api/class_responses/error_response.py` & `django_microservice_common-0.1.7/django_microservice_common/api/class_responses/error_response.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/django_microservice_common/api/exception_handlers.py` & `django_microservice_common-0.1.7/django_microservice_common/api/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/django_microservice_common/api/mixins.py` & `django_microservice_common-0.1.7/django_microservice_common/api/mixins.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/django_microservice_common/api/pagination.py` & `django_microservice_common-0.1.7/django_microservice_common/api/pagination.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/django_microservice_common/api/serializers/custom_fields/fields.py` & `django_microservice_common-0.1.7/django_microservice_common/api/serializers/custom_fields/fields.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/django_microservice_common/authorization/enums.py` & `django_microservice_common-0.1.7/django_microservice_common/authorization/enums.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/django_microservice_common/authorization/mapper.py` & `django_microservice_common-0.1.7/django_microservice_common/authorization/mapper.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/django_microservice_common/dependency_manager/container.py` & `django_microservice_common-0.1.7/django_microservice_common/dependency_manager/container.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/django_microservice_common/services/services.py` & `django_microservice_common-0.1.7/django_microservice_common/services/services.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/django_microservice_common/utils/django/utils.py` & `django_microservice_common-0.1.7/django_microservice_common/utils/django/utils.py`

 * *Files identical despite different names*

### Comparing `django_microservice_common-0.1.6/pyproject.toml` & `django_microservice_common-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "django-microservice-common"
-version = "0.1.6"
+version = "0.1.7"
 description = "A common library for Django microservices"
 authors = ["aliseylaneh <aliseylaneh@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 django = "4.0.7"
 django-environ = "0.9.0"
-psycopg2-binary = "2.9.5"
+psycopg2-binary = "2.9.9"
 djangorestframework = "3.13.1"
 whitenoise = "6.2.0"
 django-filter = "22.1"
 django-extensions = "3.2.1"
 django-cors-headers = "3.13.0"
 django-storages = "1.13.1"
 drf-jwt = "1.19.2"
```

### Comparing `django_microservice_common-0.1.6/PKG-INFO` & `django_microservice_common-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-microservice-common
-Version: 0.1.6
+Version: 0.1.7
 Summary: A common library for Django microservices
 Author: aliseylaneh
 Author-email: aliseylaneh@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -19,13 +19,13 @@
 Requires-Dist: django-redis (==5.2.0)
 Requires-Dist: django-storages (==1.13.1)
 Requires-Dist: djangorestframework (==3.13.1)
 Requires-Dist: djangorestframework-camel-case (==1.4.2)
 Requires-Dist: djangorestframework-simplejwt (==5.2.2)
 Requires-Dist: drf-jwt (==1.19.2)
 Requires-Dist: drf-spectacular (==0.24.2)
-Requires-Dist: psycopg2-binary (==2.9.5)
+Requires-Dist: psycopg2-binary (==2.9.9)
 Requires-Dist: setuptools (==69.0.3)
 Requires-Dist: whitenoise (==6.2.0)
 Description-Content-Type: text/markdown
```

