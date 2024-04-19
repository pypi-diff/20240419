# Comparing `tmp/jobbergate_api-5.0.0a2.tar.gz` & `tmp/jobbergate_api-5.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_api-5.0.0a2.tar", max compression
+gzip compressed data, was "jobbergate_api-5.1.0a0.tar", max compression
```

## Comparing `jobbergate_api-5.0.0a2.tar` & `jobbergate_api-5.1.0a0.tar`

### file list

```diff
@@ -1,42 +1,46 @@
--rw-r--r--   0        0        0     1082 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/LICENSE
--rw-r--r--   0        0        0      683 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/README.md
--rw-r--r--   0        0        0      169 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0      177 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/constants.py
--rw-r--r--   0        0        0     5251 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/dependencies.py
--rw-r--r--   0        0        0     3620 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/file_validation.py
--rw-r--r--   0        0        0     1955 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/garbage_collector.py
--rw-r--r--   0        0        0       43 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_script_templates/__init__.py
--rw-r--r--   0        0        0      100 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_script_templates/constants.py
--rw-r--r--   0        0        0     4098 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_script_templates/models.py
--rw-r--r--   0        0        0    15042 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_script_templates/routers.py
--rw-r--r--   0        0        0     7060 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_script_templates/schemas.py
--rw-r--r--   0        0        0     3749 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_script_templates/services.py
--rw-r--r--   0        0        0       40 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     2984 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    13361 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     4759 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0     6390 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/services.py
--rw-r--r--   0        0        0     1295 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/tools.py
--rw-r--r--   0        0        0       44 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0     6561 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     3575 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    14275 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0     8208 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0     1285 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/services.py
--rw-r--r--   0        0        0     5986 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/models.py
--rw-r--r--   0        0        0      558 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     2254 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/schemas.py
--rw-r--r--   0        0        0    23693 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/apps/services.py
--rw-r--r--   0        0        0     4589 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/config.py
--rw-r--r--   0        0        0     2467 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     1627 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/logging.py
--rw-r--r--   0        0        0     3496 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/main.py
--rw-r--r--   0        0        0     3436 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0     2781 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/rabbitmq_notification.py
--rw-r--r--   0        0        0     1082 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/safe_types.py
--rw-r--r--   0        0        0     4598 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/security.py
--rw-r--r--   0        0        0    10874 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/storage.py
--rw-r--r--   0        0        0     1146 2024-04-10 20:48:36.476936 jobbergate_api-5.0.0a2/jobbergate_api/version.py
--rw-r--r--   0        0        0     3982 2024-04-10 20:48:36.480936 jobbergate_api-5.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jobbergate_api-5.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-19 17:22:07.000610 jobbergate_api-5.1.0a0/LICENSE
+-rw-r--r--   0        0        0      683 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/README.md
+-rw-r--r--   0        0        0      169 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/__init__.py
+-rw-r--r--   0        0        0      944 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/models.py
+-rw-r--r--   0        0        0     2126 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/routers.py
+-rw-r--r--   0        0        0     1582 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/clusters/schemas.py
+-rw-r--r--   0        0        0      177 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/constants.py
+-rw-r--r--   0        0        0     5251 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/dependencies.py
+-rw-r--r--   0        0        0     3620 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/file_validation.py
+-rw-r--r--   0        0        0     1955 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/garbage_collector.py
+-rw-r--r--   0        0        0       43 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/__init__.py
+-rw-r--r--   0        0        0      100 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/constants.py
+-rw-r--r--   0        0        0     4098 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/models.py
+-rw-r--r--   0        0        0    15042 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/routers.py
+-rw-r--r--   0        0        0     7060 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/schemas.py
+-rw-r--r--   0        0        0     3749 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/services.py
+-rw-r--r--   0        0        0       40 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     2984 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    13361 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     4759 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0     6390 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/services.py
+-rw-r--r--   0        0        0     1295 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/tools.py
+-rw-r--r--   0        0        0       44 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0     6561 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     3575 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    14275 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0     8208 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0     1285 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/services.py
+-rw-r--r--   0        0        0     5986 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/models.py
+-rw-r--r--   0        0        0      558 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     2254 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/schemas.py
+-rw-r--r--   0        0        0    23693 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/apps/services.py
+-rw-r--r--   0        0        0     4589 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2467 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     1627 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/logging.py
+-rw-r--r--   0        0        0     3622 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3436 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0     2781 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/rabbitmq_notification.py
+-rw-r--r--   0        0        0     1082 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/safe_types.py
+-rw-r--r--   0        0        0     4598 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/security.py
+-rw-r--r--   0        0        0    10874 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/storage.py
+-rw-r--r--   0        0        0     1146 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/jobbergate_api/version.py
+-rw-r--r--   0        0        0     3982 2024-04-19 17:22:07.004610 jobbergate_api-5.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jobbergate_api-5.1.0a0/PKG-INFO
```

### Comparing `jobbergate_api-5.0.0a2/LICENSE` & `jobbergate_api-5.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/README.md` & `jobbergate_api-5.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/dependencies.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/dependencies.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/file_validation.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/garbage_collector.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_script_templates/models.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_script_templates/routers.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_script_templates/schemas.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_script_templates/services.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_script_templates/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/models.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/services.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_scripts/tools.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_scripts/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/models.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/job_submissions/services.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/job_submissions/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/models.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/permissions.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/permissions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/schemas.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/apps/services.py` & `jobbergate_api-5.1.0a0/jobbergate_api/apps/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/config.py` & `jobbergate_api-5.1.0a0/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/email_notification.py` & `jobbergate_api-5.1.0a0/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/logging.py` & `jobbergate_api-5.1.0a0/jobbergate_api/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/main.py` & `jobbergate_api-5.1.0a0/jobbergate_api/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from fastapi.exceptions import RequestValidationError
 from fastapi_pagination import add_pagination
 from loguru import logger
 from sentry_sdk.integrations.asgi import SentryAsgiMiddleware
 from starlette.middleware.cors import CORSMiddleware
 
 from jobbergate_api import __version__
+from jobbergate_api.apps.clusters.routers import router as cluster_status_router
 from jobbergate_api.apps.job_script_templates.routers import router as job_script_templates_router
 from jobbergate_api.apps.job_scripts.routers import router as job_scripts_router
 from jobbergate_api.apps.job_submissions.routers import router as job_submissions_router
 from jobbergate_api.config import settings
 from jobbergate_api.logging import init_logging
 from jobbergate_api.storage import engine_factory, handle_fk_error
 
@@ -55,14 +56,15 @@
     subapp.add_middleware(SentryAsgiMiddleware)
 else:
     logger.info("Skipping Sentry")
 
 subapp.include_router(job_script_templates_router)
 subapp.include_router(job_scripts_router)
 subapp.include_router(job_submissions_router)
+subapp.include_router(cluster_status_router)
 subapp.exception_handler(asyncpg.exceptions.ForeignKeyViolationError)(handle_fk_error)
 
 add_pagination(subapp)
 
 
 @subapp.get(
     "/health",
```

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/meta_mapper.py` & `jobbergate_api-5.1.0a0/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/rabbitmq_notification.py` & `jobbergate_api-5.1.0a0/jobbergate_api/rabbitmq_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/safe_types.py` & `jobbergate_api-5.1.0a0/jobbergate_api/safe_types.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/security.py` & `jobbergate_api-5.1.0a0/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/storage.py` & `jobbergate_api-5.1.0a0/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/jobbergate_api/version.py` & `jobbergate_api-5.1.0a0/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.0.0a2/pyproject.toml` & `jobbergate_api-5.1.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "5.0.0a2"
+version = "5.1.0a0"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_api-5.0.0a2/PKG-INFO` & `jobbergate_api-5.1.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 5.0.0a2
+Version: 5.1.0a0
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

