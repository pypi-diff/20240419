# Comparing `tmp/django_cqrs-2.7.2.tar.gz` & `tmp/django_cqrs-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cqrs-2.7.2.tar", max compression
+gzip compressed data, was "django_cqrs-2.7.3.tar", max compression
```

## Comparing `django_cqrs-2.7.2.tar` & `django_cqrs-2.7.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11369 2023-07-04 08:09:02.272786 django_cqrs-2.7.2/LICENSE
--rw-r--r--   0        0        0     9131 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/README.md
--rw-r--r--   0        0        0      196 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/__init__.py
--rw-r--r--   0        0        0     7634 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/_validation.py
--rw-r--r--   0        0        0     1842 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/admin.py
--rw-r--r--   0        0        0      289 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/apps.py
--rw-r--r--   0        0        0      917 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/constants.py
--rw-r--r--   0        0        0       60 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/controller/__init__.py
--rw-r--r--   0        0        0     3379 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/controller/consumer.py
--rw-r--r--   0        0        0      284 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/controller/producer.py
--rw-r--r--   0        0        0      698 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/correlation.py
--rw-r--r--   0        0        0     4722 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/dataclasses.py
--rw-r--r--   0        0        0     2232 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/delay.py
--rw-r--r--   0        0        0     1895 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/logger.py
--rw-r--r--   0        0        0       60 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/__init__.py
--rw-r--r--   0        0        0       60 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/__init__.py
--rw-r--r--   0        0        0     4512 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_bulk_dump.py
--rw-r--r--   0        0        0     3612 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_bulk_load.py
--rw-r--r--   0        0        0     5805 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_consume.py
--rw-r--r--   0        0        0     5196 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_dead_letters.py
--rw-r--r--   0        0        0     1569 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_deleted_diff_master.py
--rw-r--r--   0        0        0     2433 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py
--rw-r--r--   0        0        0     1178 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py
--rw-r--r--   0        0        0     2538 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_diff_master.py
--rw-r--r--   0        0        0     1866 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_diff_replica.py
--rw-r--r--   0        0        0     2156 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_diff_sync.py
--rw-r--r--   0        0        0     4675 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_sync.py
--rw-r--r--   0        0        0      484 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/management/utils.py
--rw-r--r--   0        0        0    13276 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/managers.py
--rw-r--r--   0        0        0     5316 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/metas.py
--rw-r--r--   0        0        0    17146 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/mixins.py
--rw-r--r--   0        0        0     1390 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/registries.py
--rw-r--r--   0        0        0     5196 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/signals.py
--rw-r--r--   0        0        0     1807 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/tracker.py
--rw-r--r--   0        0        0      545 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/transport/__init__.py
--rw-r--r--   0        0        0     1003 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/transport/base.py
--rw-r--r--   0        0        0     6620 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/transport/kombu.py
--rw-r--r--   0        0        0     3292 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/transport/mixins.py
--rw-r--r--   0        0        0      316 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/transport/mock.py
--rw-r--r--   0        0        0    15631 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/transport/rabbit_mq.py
--rw-r--r--   0        0        0     2352 2023-07-04 08:09:02.276786 django_cqrs-2.7.2/dj_cqrs/utils.py
--rw-r--r--   0        0        0     3332 2023-07-04 08:11:29.746211 django_cqrs-2.7.2/pyproject.toml
--rw-r--r--   0        0        0    10408 1970-01-01 00:00:00.000000 django_cqrs-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11369 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/LICENSE
+-rw-r--r--   0        0        0     9131 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/README.md
+-rw-r--r--   0        0        0      196 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/__init__.py
+-rw-r--r--   0        0        0     7634 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/_validation.py
+-rw-r--r--   0        0        0     1842 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/admin.py
+-rw-r--r--   0        0        0      289 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/apps.py
+-rw-r--r--   0        0        0      917 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/constants.py
+-rw-r--r--   0        0        0       60 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/controller/__init__.py
+-rw-r--r--   0        0        0     3379 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/controller/consumer.py
+-rw-r--r--   0        0        0      284 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/controller/producer.py
+-rw-r--r--   0        0        0      698 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/correlation.py
+-rw-r--r--   0        0        0     4722 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/dataclasses.py
+-rw-r--r--   0        0        0     2232 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/delay.py
+-rw-r--r--   0        0        0     1895 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/logger.py
+-rw-r--r--   0        0        0       60 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/__init__.py
+-rw-r--r--   0        0        0       60 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/__init__.py
+-rw-r--r--   0        0        0     4512 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_bulk_dump.py
+-rw-r--r--   0        0        0     3612 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_bulk_load.py
+-rw-r--r--   0        0        0     5805 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_consume.py
+-rw-r--r--   0        0        0     5196 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_dead_letters.py
+-rw-r--r--   0        0        0     1569 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_deleted_diff_master.py
+-rw-r--r--   0        0        0     2433 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py
+-rw-r--r--   0        0        0     1178 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py
+-rw-r--r--   0        0        0     2538 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_diff_master.py
+-rw-r--r--   0        0        0     1866 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_diff_replica.py
+-rw-r--r--   0        0        0     2156 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_diff_sync.py
+-rw-r--r--   0        0        0     4675 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_sync.py
+-rw-r--r--   0        0        0      484 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/management/utils.py
+-rw-r--r--   0        0        0    13276 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/managers.py
+-rw-r--r--   0        0        0     5316 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/metas.py
+-rw-r--r--   0        0        0    17145 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/mixins.py
+-rw-r--r--   0        0        0     1390 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/registries.py
+-rw-r--r--   0        0        0     5196 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/signals.py
+-rw-r--r--   0        0        0     1807 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/tracker.py
+-rw-r--r--   0        0        0      545 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/transport/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/transport/base.py
+-rw-r--r--   0        0        0     6620 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/transport/kombu.py
+-rw-r--r--   0        0        0     3292 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/transport/mixins.py
+-rw-r--r--   0        0        0      316 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/transport/mock.py
+-rw-r--r--   0        0        0    15631 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/transport/rabbit_mq.py
+-rw-r--r--   0        0        0     2352 2024-04-19 08:57:28.722175 django_cqrs-2.7.3/dj_cqrs/utils.py
+-rw-r--r--   0        0        0     3337 2024-04-19 08:58:47.353425 django_cqrs-2.7.3/pyproject.toml
+-rw-r--r--   0        0        0    10464 1970-01-01 00:00:00.000000 django_cqrs-2.7.3/PKG-INFO
```

### Comparing `django_cqrs-2.7.2/LICENSE` & `django_cqrs-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/README.md` & `django_cqrs-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/_validation.py` & `django_cqrs-2.7.3/dj_cqrs/_validation.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/admin.py` & `django_cqrs-2.7.3/dj_cqrs/admin.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/constants.py` & `django_cqrs-2.7.3/dj_cqrs/constants.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/controller/consumer.py` & `django_cqrs-2.7.3/dj_cqrs/controller/consumer.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/correlation.py` & `django_cqrs-2.7.3/dj_cqrs/correlation.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/dataclasses.py` & `django_cqrs-2.7.3/dj_cqrs/dataclasses.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/delay.py` & `django_cqrs-2.7.3/dj_cqrs/delay.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/logger.py` & `django_cqrs-2.7.3/dj_cqrs/logger.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_bulk_dump.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_bulk_dump.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_bulk_load.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_bulk_load.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_consume.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_consume.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_dead_letters.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_dead_letters.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_deleted_diff_master.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_deleted_diff_master.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_diff_master.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_diff_master.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_diff_replica.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_diff_replica.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_diff_sync.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_diff_sync.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/management/commands/cqrs_sync.py` & `django_cqrs-2.7.3/dj_cqrs/management/commands/cqrs_sync.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/managers.py` & `django_cqrs-2.7.3/dj_cqrs/managers.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/metas.py` & `django_cqrs-2.7.3/dj_cqrs/metas.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/mixins.py` & `django_cqrs-2.7.3/dj_cqrs/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from dj_cqrs.signals import MasterSignals, post_bulk_create, post_update
 
 
 logger = logging.getLogger('django-cqrs')
 
 
 class RawMasterMixin(Model):
-
     """Base class for MasterMixin. **Users shouldn't use this
     class directly.**"""
 
     CQRS_ID = None
     """Unique CQRS identifier for all microservices."""
 
     CQRS_PRODUCE = True
```

### Comparing `django_cqrs-2.7.2/dj_cqrs/registries.py` & `django_cqrs-2.7.3/dj_cqrs/registries.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/signals.py` & `django_cqrs-2.7.3/dj_cqrs/signals.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/tracker.py` & `django_cqrs-2.7.3/dj_cqrs/tracker.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/transport/__init__.py` & `django_cqrs-2.7.3/dj_cqrs/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/transport/base.py` & `django_cqrs-2.7.3/dj_cqrs/transport/base.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/transport/kombu.py` & `django_cqrs-2.7.3/dj_cqrs/transport/kombu.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/transport/mixins.py` & `django_cqrs-2.7.3/dj_cqrs/transport/mixins.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/transport/rabbit_mq.py` & `django_cqrs-2.7.3/dj_cqrs/transport/rabbit_mq.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/dj_cqrs/utils.py` & `django_cqrs-2.7.3/dj_cqrs/utils.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.2/pyproject.toml` & `django_cqrs-2.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cqrs"
-version = "2.7.2"
+version = "2.7.3"
 description = "Django CQRS data synchronisation"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "dj_cqrs" }
 ]
 readme = "./README.md"
@@ -36,15 +36,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 django = ">=3.2"
 pika = ">=1.0.0"
 kombu = ">=4.6.*"
 ujson = ">=5.4.0"
-django-model-utils = ">=4.0.0"
+django-model-utils = ">=4.0.0,<4.5"
 python-dateutil = ">=2.4"
 watchfiles = "^0.18.1"
 
 [tool.poetry.group.test.dependencies]
 black = ">=23.3"
 pytest = ">=7.2.0,<8"
 pytest-cov = ">=2.10.1,<5"
```

### Comparing `django_cqrs-2.7.2/PKG-INFO` & `django_cqrs-2.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cqrs
-Version: 2.7.2
+Version: 2.7.3
 Summary: Django CQRS data synchronisation
 Home-page: https://django-cqrs.readthedocs.org
 License: Apache-2.0
 Keywords: django,cqrs,sql,mixin,amqp
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,18 +16,19 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
 Classifier: Topic :: Database
 Requires-Dist: django (>=3.2)
-Requires-Dist: django-model-utils (>=4.0.0)
+Requires-Dist: django-model-utils (>=4.0.0,<4.5)
 Requires-Dist: kombu (>=4.6)
 Requires-Dist: pika (>=1.0.0)
 Requires-Dist: python-dateutil (>=2.4)
 Requires-Dist: ujson (>=5.4.0)
 Requires-Dist: watchfiles (>=0.18.1,<0.19.0)
 Project-URL: Repository, https://github.com/cloudblue/django-cqrs
 Description-Content-Type: text/markdown
```

