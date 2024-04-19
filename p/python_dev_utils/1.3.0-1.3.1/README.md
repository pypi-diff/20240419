# Comparing `tmp/python_dev_utils-1.3.0.tar.gz` & `tmp/python_dev_utils-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-1.3.0.tar", last modified: Wed Apr 17 07:02:09 2024, max compression
+gzip compressed data, was "python_dev_utils-1.3.1.tar", last modified: Fri Apr 19 13:44:52 2024, max compression
```

## Comparing `python_dev_utils-1.3.0.tar` & `python_dev_utils-1.3.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.3.0/LICENCE
--rw-r--r--   0        0        0     4373 2024-04-15 09:42:56.043729 python_dev_utils-1.3.0/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.3.0/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.3.0/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/core/abstract.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.3.0/dev_utils/core/exc.py
--rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.3.0/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/core/logging.py
--rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.3.0/dev_utils/core/results.py
--rw-r--r--   0        0        0      215 2024-04-16 09:16:58.960481 python_dev_utils-1.3.0/dev_utils/core/utils/__init__.py
--rw-r--r--   0        0        0      293 2024-04-16 09:15:43.772084 python_dev_utils-1.3.0/dev_utils/core/utils/datetime.py
--rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.3.0/dev_utils/core/utils/inspect.py
--rw-r--r--   0        0        0      209 2024-04-16 09:13:36.355106 python_dev_utils-1.3.0/dev_utils/core/utils/text.py
--rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.3.0/dev_utils/fastapi/__init__.py
--rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.3.0/dev_utils/fastapi/middlewares/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
--rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py
--rw-r--r--   0        0        0    12481 2024-04-12 12:10:40.465060 python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/exc.py
--rw-r--r--   0        0        0     4341 2024-04-12 12:19:20.576031 python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py
--rw-r--r--   0        0        0      691 2024-04-12 09:58:17.224272 python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/utils.py
--rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.3.0/dev_utils/py.typed
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.3.0/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/audit.py
--rw-r--r--   0        0        0     1141 2024-04-10 08:55:37.140201 python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/base.py
--rw-r--r--   0        0        0     1302 2024-04-10 10:08:21.445027 python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/general.py
--rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/ids.py
--rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/containers.py
--rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/profilers.py
--rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.3.0/dev_utils/sqlalchemy/types/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-16 07:24:43.054226 python_dev_utils-1.3.0/dev_utils/sqlalchemy/types/datetime.py
--rw-r--r--   0        0        0     2349 2024-04-16 10:07:40.662627 python_dev_utils-1.3.0/dev_utils/sqlalchemy/types/pydantic.py
--rw-r--r--   0        0        0    12370 2024-04-16 09:14:15.986788 python_dev_utils-1.3.0/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0     3113 2024-04-17 07:02:09.040941 python_dev_utils-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.3.0/tests/core/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/core/test_abstract.py
--rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.3.0/tests/core/test_guards.py
--rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/core/test_results.py
--rw-r--r--   0        0        0     1278 2024-04-16 09:18:12.890888 python_dev_utils-1.3.0/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.3.0/tests/fastapi/__init__.py
--rw-r--r--   0        0        0     1407 2024-04-12 12:14:52.442153 python_dev_utils-1.3.0/tests/fastapi/conftest.py
--rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/fastapi/test_middlewares.py
--rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions.py
--rw-r--r--   0        0        0     2072 2024-04-12 12:18:33.383580 python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions_handlers.py
--rw-r--r--   0        0        0      803 2024-04-12 12:23:22.923870 python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.3.0/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.3.0/tests/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.3.0/tests/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_audit.py
--rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_base.py
--rw-r--r--   0        0        0     1122 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_general.py
--rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_ids.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.3.0/tests/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.3.0/tests/sqlalchemy/profiling/test_profilers.py
--rw-r--r--   0        0        0     1423 2024-04-17 07:01:59.517966 python_dev_utils-1.3.0/tests/sqlalchemy/test_types.py
--rw-r--r--   0        0        0     7086 2024-04-16 09:18:34.220718 python_dev_utils-1.3.0/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.3.0/tests/types.py
--rw-r--r--   0        0        0     7726 2024-04-16 09:37:08.400872 python_dev_utils-1.3.0/tests/utils.py
--rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 python_dev_utils-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.3.1/LICENCE
+-rw-r--r--   0        0        0     4373 2024-04-15 09:42:56.043729 python_dev_utils-1.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.3.1/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.3.1/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.3.1/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.3.1/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/core/logging.py
+-rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.3.1/dev_utils/core/results.py
+-rw-r--r--   0        0        0      215 2024-04-16 09:16:58.960481 python_dev_utils-1.3.1/dev_utils/core/utils/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-16 09:15:43.772084 python_dev_utils-1.3.1/dev_utils/core/utils/datetime.py
+-rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.3.1/dev_utils/core/utils/inspect.py
+-rw-r--r--   0        0        0      209 2024-04-16 09:13:36.355106 python_dev_utils-1.3.1/dev_utils/core/utils/text.py
+-rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.3.1/dev_utils/fastapi/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.3.1/dev_utils/fastapi/middlewares/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
+-rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/__init__.py
+-rw-r--r--   0        0        0    12481 2024-04-12 12:10:40.465060 python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/exc.py
+-rw-r--r--   0        0        0     4341 2024-04-12 12:19:20.576031 python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/handlers.py
+-rw-r--r--   0        0        0      691 2024-04-12 09:58:17.224272 python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.3.1/dev_utils/py.typed
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.3.1/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/audit.py
+-rw-r--r--   0        0        0     1141 2024-04-10 08:55:37.140201 python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/base.py
+-rw-r--r--   0        0        0     1302 2024-04-10 10:08:21.445027 python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/general.py
+-rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/ids.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/containers.py
+-rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/profilers.py
+-rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.3.1/dev_utils/sqlalchemy/types/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-16 07:24:43.054226 python_dev_utils-1.3.1/dev_utils/sqlalchemy/types/datetime.py
+-rw-r--r--   0        0        0     2349 2024-04-16 10:07:40.662627 python_dev_utils-1.3.1/dev_utils/sqlalchemy/types/pydantic.py
+-rw-r--r--   0        0        0    12968 2024-04-19 13:44:02.168069 python_dev_utils-1.3.1/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0     3113 2024-04-19 13:44:52.349383 python_dev_utils-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.3.1/tests/core/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.3.1/tests/core/test_guards.py
+-rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/core/test_results.py
+-rw-r--r--   0        0        0     1278 2024-04-16 09:18:12.890888 python_dev_utils-1.3.1/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.3.1/tests/fastapi/__init__.py
+-rw-r--r--   0        0        0     1407 2024-04-12 12:14:52.442153 python_dev_utils-1.3.1/tests/fastapi/conftest.py
+-rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/fastapi/test_middlewares.py
+-rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions.py
+-rw-r--r--   0        0        0     2072 2024-04-12 12:18:33.383580 python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions_handlers.py
+-rw-r--r--   0        0        0      803 2024-04-12 12:23:22.923870 python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions_utils.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.3.1/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.3.1/tests/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.3.1/tests/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_audit.py
+-rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_base.py
+-rw-r--r--   0        0        0     1122 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_general.py
+-rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_ids.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.3.1/tests/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/sqlalchemy/profiling/test_profilers.py
+-rw-r--r--   0        0        0     2103 2024-04-17 07:02:19.144904 python_dev_utils-1.3.1/tests/sqlalchemy/test_types.py
+-rw-r--r--   0        0        0     7086 2024-04-16 09:18:34.220718 python_dev_utils-1.3.1/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.3.1/tests/types.py
+-rw-r--r--   0        0        0     7726 2024-04-16 09:37:08.400872 python_dev_utils-1.3.1/tests/utils.py
+-rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 python_dev_utils-1.3.1/PKG-INFO
```

### Comparing `python_dev_utils-1.3.0/LICENCE` & `python_dev_utils-1.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/README.md` & `python_dev_utils-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/core/abstract.py` & `python_dev_utils-1.3.1/dev_utils/core/abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/core/exc.py` & `python_dev_utils-1.3.1/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/core/guards.py` & `python_dev_utils-1.3.1/dev_utils/core/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/core/logging.py` & `python_dev_utils-1.3.1/dev_utils/core/logging.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/core/results.py` & `python_dev_utils-1.3.1/dev_utils/core/results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/core/utils/inspect.py` & `python_dev_utils-1.3.1/dev_utils/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/fastapi/__init__.py` & `python_dev_utils-1.3.1/dev_utils/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py` & `python_dev_utils-1.3.1/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py` & `python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/exc.py` & `python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py` & `python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/fastapi/verbose_http_exceptions/utils.py` & `python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/filters/types.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/audit.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/base.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/general.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/mixins/ids.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/ids.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/containers.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/containers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/profilers.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/profiling/utils.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/types/datetime.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/types/datetime.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/types/pydantic.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/types/pydantic.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-1.3.1/dev_utils/sqlalchemy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utils module of sqlalchemy dev package.
 
 Contains functions, which inspect models, apply joins, apply options and wrap some sqlalchemy
 functionality.
 """
 
 import types
-from typing import TYPE_CHECKING, Any, TypeGuard, TypeVar
+from typing import TYPE_CHECKING, Any, Literal, TypeGuard, TypeVar, overload
 
 from sqlalchemy import Delete, Insert, Select, Table, Update, inspect
 from sqlalchemy.ext.hybrid import HybridExtensionType
 from sqlalchemy.orm import DeclarativeBase, joinedload
 
 from dev_utils.core.exc import (
     NoDeclarativeModelError,
@@ -17,15 +17,15 @@
     NoModelRelationshipError,
 )
 from dev_utils.core.logging import logger
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Sequence
 
-    from sqlalchemy.orm import Mapper, QueryableAttribute
+    from sqlalchemy.orm import InstrumentedAttribute, Mapper, QueryableAttribute
     from sqlalchemy.orm.base import InspectionAttr
     from sqlalchemy.orm.clsregistry import _ClsRegistryType  # type: ignore
     from sqlalchemy.orm.strategy_options import _AbstractLoad  # type: ignore
 
     T = TypeVar("T", bound=Select[Any])
 
 Statement = (
@@ -57,33 +57,58 @@
         return False
     else:
         if not hasattr(mapper, "is_mapper"):
             return False
         return mapper.is_mapper
 
 
+@overload
 def get_sqlalchemy_attribute(
     model: type["DeclarativeBase"],
     field_name: str,
+    *,
+    only_columns: Literal[True],
+) -> "InstrumentedAttribute[Any]": ...
+
+
+@overload
+def get_sqlalchemy_attribute(
+    model: type["DeclarativeBase"],
+    field_name: str,
+    *,
+    only_columns: Literal[False] = False,
+) -> "QueryableAttribute[Any]": ...
+
+
+def get_sqlalchemy_attribute(
+    model: type["DeclarativeBase"],
+    field_name: str,
+    *,
+    only_columns: bool = False,
 ) -> "QueryableAttribute[Any]":
     """Get sqlalchemy field (column) or relationship object from given model.
 
     Args
     ----
     model : type[DeclarativeBase]
         SQLAlchemy declarative model.
     field_name : str
         name of field to find in model.
+    only_columns: bool
+        get attribute only from columns.
 
     Returns
     -------
     QueryableAttribute[Any]
         any attribute from model, that can be used in queries.
     """
-    valid_attributes = get_all_valid_queryable_attributes(model)
+    if only_columns:
+        valid_attributes = get_valid_field_names(model)
+    else:
+        valid_attributes = get_all_valid_queryable_attributes(model)
     if field_name not in valid_attributes:
         valid_field = ", ".join(valid_attributes)
         msg = (
             f'No sqlalchemy attribute "{field_name}" was found in model "{model}". '
             f"Valid attributes for {model}: {valid_field}"
         )
         raise NoModelAttributeError(msg)
```

### Comparing `python_dev_utils-1.3.0/pyproject.toml` & `python_dev_utils-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     "asyncpg>=0.29.0",
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "1.3.0"
+version = "1.3.1"
 description = "My project utils package, that I use in my projects."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
```

### Comparing `python_dev_utils-1.3.0/tests/conftest.py` & `python_dev_utils-1.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/core/test_abstract.py` & `python_dev_utils-1.3.1/tests/core/test_abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/core/test_guards.py` & `python_dev_utils-1.3.1/tests/core/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/core/test_results.py` & `python_dev_utils-1.3.1/tests/core/test_results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/core/test_utils.py` & `python_dev_utils-1.3.1/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/fastapi/conftest.py` & `python_dev_utils-1.3.1/tests/fastapi/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions.py` & `python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions_handlers.py` & `python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions_handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/fastapi/test_verbose_http_exceptions_utils.py` & `python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_guards.py` & `python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_audit.py` & `python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_base.py` & `python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/sqlalchemy/mixins/test_general.py` & `python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/sqlalchemy/profiling/test_profilers.py` & `python_dev_utils-1.3.1/tests/sqlalchemy/profiling/test_profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/sqlalchemy/test_types.py` & `python_dev_utils-1.3.1/tests/sqlalchemy/test_types.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import zoneinfo
 from typing import TYPE_CHECKING, Any
 
 import pytest
 from mimesis import Datetime
 
-from tests.utils import TableWithUTCDT, create_db_item_sync
+from tests.utils import PydanticTestSchema, TableWithUTCDT, create_db_item_sync
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
     from tests.types import SyncFactoryFunctionProtocol
 
 
@@ -24,14 +24,15 @@
         session: "Session",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
     ) -> TableWithUTCDT:
         params: dict[str, Any] = dict(
             dt_field=dt_faker.datetime(),
+            pydantic_field=PydanticTestSchema(a=2, b=3, c=4),
         )
         params.update(kwargs)
         return create_db_item_sync(session, TableWithUTCDT, params, commit=commit)
 
     return _create
 
 
@@ -50,7 +51,24 @@
 ) -> None:
     item = table_create(db_sync_session, dt_field=dt, commit=True)
     if tzinfo_presents:
         assert item.dt_field.tzinfo is not None
         assert item.dt_field.tzinfo == UTC
     else:
         assert item.dt_field.tzinfo is None
+
+
+@pytest.mark.parametrize(
+    ("field", "expected_value"),
+    [
+        (PydanticTestSchema(a=255, b=255, c=255), PydanticTestSchema(a=255, b=255, c=255)),
+        ({"a": 255, "b": 255, "c": 255}, PydanticTestSchema(a=255, b=255, c=255)),  # noqa: DTZ005
+    ],
+)
+def test_pydantic_field(
+    field: Any,  # noqa: ANN401
+    expected_value: Any,  # noqa: ANN401
+    db_sync_session: "Session",
+    table_create: "SyncFactoryFunctionProtocol[TableWithUTCDT]",
+) -> None:
+    item = table_create(db_sync_session, pydantic_field=field, commit=True)
+    assert item.pydantic_field == expected_value
```

### Comparing `python_dev_utils-1.3.0/tests/sqlalchemy/test_utils.py` & `python_dev_utils-1.3.1/tests/sqlalchemy/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/types.py` & `python_dev_utils-1.3.1/tests/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/tests/utils.py` & `python_dev_utils-1.3.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.0/PKG-INFO` & `python_dev_utils-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_dev_utils
-Version: 1.3.0
+Version: 1.3.1
 Summary: My project utils package, that I use in my projects.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: fastapi-exceptions
 Provides-Extra: profiling
 Provides-Extra: sqlalchemy-filters
```

