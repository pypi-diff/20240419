# Comparing `tmp/alphaz-next-0.4.1.tar.gz` & `tmp/alphaz-next-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.4.1.tar", last modified: Thu Apr 18 09:55:12 2024, max compression
+gzip compressed data, was "alphaz-next-0.4.2.tar", last modified: Thu Apr 18 22:13:19 2024, max compression
```

## Comparing `alphaz-next-0.4.1.tar` & `alphaz-next-0.4.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.920163 alphaz-next-0.4.1/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.920163 alphaz-next-0.4.1/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.920163 alphaz-next-0.4.1/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.920163 alphaz-next-0.4.1/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    11076 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/responses/ujson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/core/uvicorn_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.920163 alphaz-next-0.4.1/alphaz_next/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/alphaz_next/models/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/config/directories_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/models/config/openapi_config_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.920163 alphaz-next-0.4.1/alphaz_next/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/alphaz_next/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-18 09:55:09.000000 alphaz-next-0.4.1/alphaz_next/utils/logging_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:55:12.920163 alphaz-next-0.4.1/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-18 09:55:12.000000 alphaz-next-0.4.1/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 09:55:12.000000 alphaz-next-0.4.1/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:55:12.000000 alphaz-next-0.4.1/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 09:55:12.000000 alphaz-next-0.4.1/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 09:55:12.000000 alphaz-next-0.4.1/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:55:12.924163 alphaz-next-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 09:55:11.000000 alphaz-next-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.632899 alphaz-next-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-18 22:13:19.632899 alphaz-next-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/responses/ujson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/core/uvicorn_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/models/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/directories_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/models/config/openapi_config_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.628899 alphaz-next-0.4.2/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27232 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.632899 alphaz-next-0.4.2/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-18 22:13:17.000000 alphaz-next-0.4.2/alphaz_next/utils/logging_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:13:19.624899 alphaz-next-0.4.2/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 22:13:19.632899 alphaz-next-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-18 22:13:19.000000 alphaz-next-0.4.2/setup.py
```

### Comparing `alphaz-next-0.4.1/PKG-INFO` & `alphaz-next-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.4.1
+Version: 0.4.2
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.4.1.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.4.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.4.1/README.md` & `alphaz-next-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/auth/auth.py` & `alphaz-next-0.4.2/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/_base.py` & `alphaz-next-0.4.2/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/_middleware.py` & `alphaz-next-0.4.2/alphaz_next/core/_middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/application.py` & `alphaz-next-0.4.2/alphaz_next/core/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,15 +114,16 @@
     )
 
     return openapi_schema
 
 
 def create_app(
     config: _AlphaConfigSchema,
-    routers: _List[_APIRouter],
+    routes: _Optional[_BaseRoute] = None,
+    routers: _Optional[_List[_APIRouter]] = None,
     container: _Optional[_ContainerType] = None,
     lifespan: _Optional[_AsyncContextManager] = None,
     allow_origins: _Sequence[str] = (),
     allow_methods: _Sequence[str] = ("GET",),
     allow_headers: _Sequence[str] = (),
     allow_credentials: bool = False,
     allow_private_network: bool = False,
@@ -130,14 +131,15 @@
     uvicorn_formatter: _Optional[_logging.Formatter] = None,
 ) -> _FastAPI:
     """
     Create a FastAPI application with the specified configuration.
 
     Args:
         config (AlphaConfigSchema): The configuration for the application.
+        routes (Optional[BaseRoute]): The list of routes to include in the application. Defaults to None.
         routers (List[APIRouter]): The list of API routers to include in the application.
         container (Optional[containers.DeclarativeContainer]): The dependency injection container. Defaults to None.
         allow_origins (Sequence[str]): The list of allowed origins for CORS. Defaults to ().
         allow_methods (Sequence[str]): The list of allowed HTTP methods for CORS. Defaults to ("GET",).
         allow_headers (Sequence[str]): The list of allowed headers for CORS. Defaults to ().
         allow_credentials (bool): Whether to allow credentials for CORS. Defaults to False.
         allow_private_network (bool): Whether to allow private network for CORS. Defaults to False.
@@ -175,14 +177,15 @@
             _ExcludeRoutersFilter(
                 router_names=config.api_config.logging.excluded_routers
             )
         )
 
     # APP
     app = _FastAPI(
+        routes=routes,
         title=config.project_name.upper(),
         version=config.version,
         docs_url=None,
         redoc_url=None,
         lifespan=lifespan,
     )
     app.container = container
@@ -207,15 +210,15 @@
                 "SERVER_CERT": config.api_config.apm.ssl_ca_cert,
                 "VERIFY_SERVER_CERT": config.api_config.apm.ssl_verify,
             }
         )
 
         app.add_middleware(_ElasticAPM, client=apm)
 
-    for router in routers:
+    for router in routers or []:
         app.include_router(router)
 
     app.openapi_schema = _custom_openapi(config=config, routes=app.routes)
 
     swagger_favicon_url = _DEFAULT_FAVICON_URL
     redoc_favicon_url = _DEFAULT_FAVICON_URL
     if (openapi_config := config.api_config.openapi) is not None:
```

### Comparing `alphaz-next-0.4.1/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.4.2/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/exceptions.py` & `alphaz-next-0.4.2/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.4.2/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.4.2/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.4.2/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.4.2/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.4.2/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.4.2/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.4.2/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/responses/response.py` & `alphaz-next-0.4.2/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.4.2/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.4.2/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/libs/httpx.py` & `alphaz-next-0.4.2/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.4.2/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,29 @@
         algorithm_alias (str, optional): The alias for the algorithm. Defaults to "ALPHA_ALGORITHM".
 
     Returns:
         AlphaInternalConfigSettingsSchema: An instance of the AlphaInternalConfigSettingsSchema class.
     """
 
     class AlphaInternalConfigSettingsSchema(BaseSettings):
-        token_url: str = Field(validation_alias=token_url_alias)
-        user_me_url: str = Field(validation_alias=user_me_url_alias)
-        api_key_me_url: str = Field(validation_alias=api_key_me_url_alias)
-        secret_key: str = Field(validation_alias=secret_key_alias)
-        algorithm: str = Field(validation_alias=algorithm_alias)
+        token_url: str = Field(
+            default="/auth",
+            validation_alias=token_url_alias,
+        )
+        user_me_url: str = Field(
+            default="user/me",
+            validation_alias=user_me_url_alias,
+        )
+        api_key_me_url: str = Field(
+            default="api-key/me",
+            validation_alias=api_key_me_url_alias,
+        )
+        secret_key: str = Field(
+            default="",
+            validation_alias=secret_key_alias,
+        )
+        algorithm: str = Field(
+            default="",
+            validation_alias=algorithm_alias,
+        )
 
     return AlphaInternalConfigSettingsSchema()
```

### Comparing `alphaz-next-0.4.1/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.4.2/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.4.2/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/models/config/api_config.py` & `alphaz-next-0.4.2/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.4.2/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.4.2/alphaz_next/models/config/config_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,18 +35,18 @@
         workers_alias (str, optional): The alias for the workers field in the JSON file. Defaults to "ALPHA_WORKERS".
 
     Returns:
         _T: The validated configuration data based on the provided model class.
     """
 
     class AlphaConfigSettingsSchema(_BaseSettings):
-        environment: str = _Field(validation_alias=environment_alias)
-        root: str = _Field(validation_alias=root_alias)
-        port: int = _Field(validation_alias=port_alias)
-        workers: int = _Field(validation_alias=workers_alias)
+        environment: str = _Field(default="local", validation_alias=environment_alias)
+        root: str = _Field(default=str(_Path.cwd()), validation_alias=root_alias)
+        port: int = _Field(default=8000, validation_alias=port_alias)
+        workers: int = _Field(default=1, validation_alias=workers_alias)
 
         @_computed_field
         @property
         def main_config(self) -> _T:
             data = _open_json_file(path=_Path(path))
 
             data_ext = {
```

### Comparing `alphaz-next-0.4.1/alphaz_next/models/config/database_config.py` & `alphaz-next-0.4.2/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.4.2/alphaz_next/models/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.4.2/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.4.2/alphaz_next/tests/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/utils/format.py` & `alphaz-next-0.4.2/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/utils/logger.py` & `alphaz-next-0.4.2/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.4.2/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.4.2/alphaz_next.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.4.1
+Version: 0.4.2
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.4.1.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.4.2.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `alphaz-next-0.4.1/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.4.2/alphaz_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.4.1/setup.py` & `alphaz-next-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.4.1"
+version = "0.4.2"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 
 EXTRAS_REQUIRE = {
     "dependency-injector": ["dependency-injector"],
```

