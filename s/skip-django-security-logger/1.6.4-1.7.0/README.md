# Comparing `tmp/skip-django-security-logger-1.6.4.tar.gz` & `tmp/skip_django_security_logger-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-security-logger-1.6.4.tar", last modified: Wed Nov 29 15:28:35 2023, max compression
+gzip compressed data, was "skip_django_security_logger-1.7.0.tar", last modified: Fri Apr 19 10:25:00 2024, max compression
```

## Comparing `skip-django-security-logger-1.6.4.tar` & `skip_django_security_logger-1.7.0.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.696582 skip-django-security-logger-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-11-29 15:28:35.696582 skip-django-security-logger-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.676582 skip-django-security-logger-1.6.4/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.676582 skip-django-security-logger-1.6.4/example/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.676582 skip-django-security-logger-1.6.4/example/apps/test_security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.676582 skip-django-security-logger-1.6.4/example/apps/test_security/management/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.676582 skip-django-security-logger-1.6.4/example/apps/test_security/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/management/commands/create_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/management/commands/create_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/management/commands/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/management/commands/test_command_with_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/management/commands/test_error_command.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.680582 skip-django-security-logger-1.6.4/example/apps/test_security/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    53788 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tests/celery_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    16934 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tests/command_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tests/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    31077 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tests/input_request_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    20624 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tests/output_request_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tests/partitioned_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tests/throttling_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/apps/test_security/views.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      330 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.680582 skip-django-security-logger-1.6.4/example/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/settings/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/test_elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/example/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.684582 skip-django-security-logger-1.6.4/security/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.684582 skip-django-security-logger-1.6.4/security/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.684582 skip-django-security-logger-1.6.4/security/backends/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/common/is_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/common/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.684582 skip-django-security-logger-1.6.4/security/backends/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.684582 skip-django-security-logger-1.6.4/security/backends/elasticsearch/is_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/is_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/is_core/cores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/is_core/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.688582 skip-django-security-logger-1.6.4/security/backends/elasticsearch/logstash/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/logstash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/logstash/handler_tcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/logstash/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.688582 skip-django-security-logger-1.6.4/security/backends/elasticsearch/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.688582 skip-django-security-logger-1.6.4/security/backends/elasticsearch/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/management/commands/init_elasticsearch_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     8812 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    18775 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/elasticsearch/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.688582 skip-django-security-logger-1.6.4/security/backends/logging/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/logging/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    16999 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/logging/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/purge_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.688582 skip-django-security-logger-1.6.4/security/backends/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/db_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.688582 skip-django-security-logger-1.6.4/security/backends/sql/is_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/is_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/is_core/cores.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/is_core/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.688582 skip-django-security-logger-1.6.4/security/backends/sql/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    15347 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/migrations/0002_auto_20211119_1940.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/migrations/0003_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/migrations/0004_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12138 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12831 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/sql/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.688582 skip-django-security-logger-1.6.4/security/backends/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/testing/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/testing/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/testing/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/backends/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.688582 skip-django-security-logger-1.6.4/security/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/contrib/debug_toolbar_log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/contrib/debug_toolbar_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/contrib/debug_toolbar_log/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/contrib/pyston/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/contrib/pyston/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/contrib/pyston/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.672582 skip-django-security-logger-1.6.4/security/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.672582 skip-django-security-logger-1.6.4/security/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/log_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/logging/celery/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/logging/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/logging/celery/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/logging/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/logging/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/logging/commands/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/logging/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/logging/requests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/logging/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/logging/requests/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/logging/requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/management/
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/management/commands/purge_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/management/commands/set_celery_task_log_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/storages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/suds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/templates/429.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.692582 skip-django-security-logger-1.6.4/security/throttling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/throttling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/throttling/default_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/throttling/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/throttling/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/throttling/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/security/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-29 15:28:35.696582 skip-django-security-logger-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2023-11-29 15:28:23.000000 skip-django-security-logger-1.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 15:28:35.696582 skip-django-security-logger-1.6.4/skip_django_security_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-11-29 15:28:35.000000 skip-django-security-logger-1.6.4/skip_django_security_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2023-11-29 15:28:35.000000 skip-django-security-logger-1.6.4/skip_django_security_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 15:28:35.000000 skip-django-security-logger-1.6.4/skip_django_security_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 15:28:35.000000 skip-django-security-logger-1.6.4/skip_django_security_logger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-11-29 15:28:35.000000 skip-django-security-logger-1.6.4/skip_django_security_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-29 15:28:35.000000 skip-django-security-logger-1.6.4/skip_django_security_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.815289 skip_django_security_logger-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-19 10:25:00.815289 skip_django_security_logger-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.791289 skip_django_security_logger-1.7.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.791289 skip_django_security_logger-1.7.0/example/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.791289 skip_django_security_logger-1.7.0/example/apps/test_security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.791289 skip_django_security_logger-1.7.0/example/apps/test_security/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.795289 skip_django_security_logger-1.7.0/example/apps/test_security/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/management/commands/create_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/management/commands/create_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/management/commands/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/management/commands/test_command_with_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/management/commands/test_error_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.795289 skip_django_security_logger-1.7.0/example/apps/test_security/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53788 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tests/celery_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16934 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tests/command_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tests/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31075 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tests/input_request_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tests/output_request_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tests/partitioned_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tests/throttling_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/apps/test_security/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      330 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.795289 skip_django_security_logger-1.7.0/example/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/settings/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/test_elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/example/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.799289 skip_django_security_logger-1.7.0/security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.799289 skip_django_security_logger-1.7.0/security/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.799289 skip_django_security_logger-1.7.0/security/backends/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18938 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/common/is_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/common/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.803289 skip_django_security_logger-1.7.0/security/backends/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.803289 skip_django_security_logger-1.7.0/security/backends/elasticsearch/is_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/is_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/is_core/cores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/is_core/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.803289 skip_django_security_logger-1.7.0/security/backends/elasticsearch/logstash/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/logstash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/logstash/handler_tcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/logstash/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.803289 skip_django_security_logger-1.7.0/security/backends/elasticsearch/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.803289 skip_django_security_logger-1.7.0/security/backends/elasticsearch/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/management/commands/init_elasticsearch_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18775 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/elasticsearch/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.803289 skip_django_security_logger-1.7.0/security/backends/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/logging/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16999 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/logging/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/purge_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.807289 skip_django_security_logger-1.7.0/security/backends/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/db_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.807289 skip_django_security_logger-1.7.0/security/backends/sql/is_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/is_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/is_core/cores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/is_core/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.807289 skip_django_security_logger-1.7.0/security/backends/sql/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    15347 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/migrations/0002_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/migrations/0003_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/migrations/0004_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/sql/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.807289 skip_django_security_logger-1.7.0/security/backends/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/testing/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/testing/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/testing/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/backends/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.807289 skip_django_security_logger-1.7.0/security/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.807289 skip_django_security_logger-1.7.0/security/contrib/debug_toolbar_log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/contrib/debug_toolbar_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/contrib/debug_toolbar_log/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.807289 skip_django_security_logger-1.7.0/security/contrib/pyston/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/contrib/pyston/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/contrib/pyston/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.791289 skip_django_security_logger-1.7.0/security/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.791289 skip_django_security_logger-1.7.0/security/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.807289 skip_django_security_logger-1.7.0/security/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/log_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.807289 skip_django_security_logger-1.7.0/security/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.811289 skip_django_security_logger-1.7.0/security/logging/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/logging/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/logging/celery/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.811289 skip_django_security_logger-1.7.0/security/logging/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/logging/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/logging/commands/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/logging/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.811289 skip_django_security_logger-1.7.0/security/logging/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/logging/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/logging/requests/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/logging/requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.811289 skip_django_security_logger-1.7.0/security/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.811289 skip_django_security_logger-1.7.0/security/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/management/commands/purge_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/management/commands/set_celery_task_log_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/suds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.811289 skip_django_security_logger-1.7.0/security/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/templates/429.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.811289 skip_django_security_logger-1.7.0/security/throttling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/throttling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/throttling/default_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/throttling/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/throttling/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/throttling/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/security/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:25:00.815289 skip_django_security_logger-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-19 10:24:57.000000 skip_django_security_logger-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:25:00.815289 skip_django_security_logger-1.7.0/skip_django_security_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-19 10:25:00.000000 skip_django_security_logger-1.7.0/skip_django_security_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-19 10:25:00.000000 skip_django_security_logger-1.7.0/skip_django_security_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:25:00.000000 skip_django_security_logger-1.7.0/skip_django_security_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:25:00.000000 skip_django_security_logger-1.7.0/skip_django_security_logger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-19 10:25:00.000000 skip_django_security_logger-1.7.0/skip_django_security_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 10:25:00.000000 skip_django_security_logger-1.7.0/skip_django_security_logger.egg-info/top_level.txt
```

### Comparing `skip-django-security-logger-1.6.4/LICENSE` & `skip_django_security_logger-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/PKG-INFO` & `skip_django_security_logger-1.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-security-logger
-Version: 1.6.4
+Version: 1.7.0
 Summary: Django security library.
 Home-page: https://github.com/skip-pay/django-security
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,throttling
 Classifier: Development Status :: 3 - Alpha
@@ -16,21 +16,21 @@
 Classifier: Natural Language :: Czech
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: django<4.0,>=3.1
+Requires-Dist: django>=4.2
 Requires-Dist: django-ipware>=3.0.2
 Requires-Dist: ansi2html>=1.6.0
-Requires-Dist: skip-django-chamber>=0.6.16.3
+Requires-Dist: skip-django-chamber>=0.7.2
 Requires-Dist: skip-django-choice-enumfields>=1.1.3.2
-Requires-Dist: skip-django-generic-m2m-field>=0.0.9.3
-Requires-Dist: skip-django-celery-extensions>=0.0.37.1
+Requires-Dist: skip-django-generic-m2m-field>=0.1.0
+Requires-Dist: skip-django-celery-extensions>=0.1.0
 Requires-Dist: isodate>=0.6.1
 
 Prolog
 ======
 
 Django-security-logger is library for logging input and output request. Library can be used with django-reversion to log which data was changed in a request.
 The library provides throttling security mechanism.
```

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/management/__init__.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/management/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/tasks.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/tasks.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/tests/base.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/tests/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/tests/celery_log.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/tests/celery_log.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/tests/command_log.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/tests/command_log.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/tests/commands.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/tests/commands.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/tests/input_request_log.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/tests/input_request_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import responses
 
 from django import get_version
 from django.test import override_settings
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from germanium.decorators import data_consumer
 from germanium.test_cases.client import ClientTestCase
 from germanium.tools import (
     assert_equal, assert_false, assert_http_not_found, assert_http_ok, assert_http_redirect,
     assert_http_too_many_requests, assert_in, assert_is_none, assert_is_not_none, assert_not_in,
     assert_raises, assert_true, assert_equal_model_fields, assert_length_equal, all_eq_obj, not_none_eq_obj
@@ -182,15 +182,15 @@
             assert_equal(len(logged_data.input_request[0].request_body), 4162)
             assert_false(logged_data.input_request[0].request_body.endswith(TRUNCATION_CHAR))
 
     @override_settings(SECURITY_LOG_RESPONSE_BODY_LENGTH=None, SECURITY_HIDE_SENSITIVE_DATA=False)
     def test_response_body_truncation_should_be_turned_off(self):
         with capture_security_logs() as logged_data:
             response = self.post('/admin/login/', data={'username': 2000 * 'a', 'password': 2000 * 'b'})
-            assert_equal(logged_data.input_request[0].response_body, force_text(response.content))
+            assert_equal(logged_data.input_request[0].response_body, force_str(response.content))
             assert_false(logged_data.input_request[0].response_body.endswith(TRUNCATION_CHAR))
 
     @override_settings(SECURITY_LOG_RESPONSE_BODY_CONTENT_TYPES=())
     def test_not_allowed_content_type_body_should_not_be_logged(self):
         with capture_security_logs() as logged_data:
             assert_http_ok(self.get('/home/'))
             assert_is_none(logged_data.input_request[0].response_body)
```

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/tests/output_request_log.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/tests/output_request_log.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/tests/partitioned_log.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/tests/partitioned_log.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/tests/utils.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/apps/test_security/views.py` & `skip_django_security_logger-1.7.0/example/apps/test_security/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/settings/base.py` & `skip_django_security_logger-1.7.0/example/settings/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,18 +110,18 @@
     'django.contrib.messages',
     'django.contrib.staticfiles',
     'django.contrib.humanize',
 
     # apps
     'django_celery_extensions',
     'security',
-    'security.backends.sql',
-    'security.backends.logging',
-    'security.backends.elasticsearch',
-    'security.backends.testing',
+    'security.backends.sql.app.SecuritySQLBackend',
+    'security.backends.logging.app.SecurityLoggingBackend',
+    'security.backends.elasticsearch.app.SecurityElasticsearchBackend',
+    'security.backends.testing.app.SecurityTestingBackend',
     'reversion',
     'apps.test_security',
 )
 
 # A sample logging configuration. The only tangible logging
 # performed by this configuration is to send an email to
 # the site admins on every HTTP 500 error when DEBUG=False.
```

### Comparing `skip-django-security-logger-1.6.4/example/settings/settings.py` & `skip_django_security_logger-1.7.0/example/settings/settings.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/test_elastic.py` & `skip_django_security_logger-1.7.0/example/test_elastic.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/example/urls.py` & `skip_django_security_logger-1.7.0/example/urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.contrib import admin
 
 from apps.test_security.views import (
     extra_throttling_view, hide_request_body_view, log_exempt_view, proxy_view, throttling_exempt_view, home_view,
     error_view
 )
 
-from django.conf.urls import url
+from django.urls import re_path as url
 
 
 urlpatterns = [
     url('admin/', admin.site.urls),
     url('proxy/', proxy_view),
     url('hide-request-body/', hide_request_body_view),
     url('log-exempt/', log_exempt_view),
```

### Comparing `skip-django-security-logger-1.6.4/example/wsgi.py` & `skip_django_security_logger-1.7.0/example/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/app.py` & `skip_django_security_logger-1.7.0/security/backends/app.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/common/is_core.py` & `skip_django_security_logger-1.7.0/security/backends/common/is_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 from ansi2html import Ansi2HTMLConverter
 
 from django.contrib.contenttypes.models import ContentType
 from django.template.defaultfilters import truncatechars
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.utils.html import mark_safe
 
 from chamber.shortcuts import get_object_or_none
 
 from pyston.utils.decorators import filter_by, order_by
 
 from is_core.generic_views.detail_views import DjangoReadonlyDetailView
```

### Comparing `skip-django-security-logger-1.6.4/security/backends/common/mixins.py` & `skip_django_security_logger-1.7.0/security/backends/common/mixins.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/elasticsearch/connection.py` & `skip_django_security_logger-1.7.0/security/backends/elasticsearch/connection.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/elasticsearch/is_core/cores.py` & `skip_django_security_logger-1.7.0/security/backends/elasticsearch/is_core/cores.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from pyston.utils.decorators import filter_class, order_by
 
 from is_core.utils.decorators import short_description
 from is_core.contrib.elasticsearch.cores import ElasticsearchUiRestCore
 from is_core.contrib.elasticsearch.views import ElasticsearchInlineTableView
```

### Comparing `skip-django-security-logger-1.6.4/security/backends/elasticsearch/is_core/filters.py` & `skip_django_security_logger-1.7.0/security/backends/elasticsearch/is_core/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib.auth import get_user_model
 from django.db import router
 from django.db.models import TextField
 from django.db.models.functions import Cast
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 from django.contrib.contenttypes.models import ContentType
 
 from elasticsearch_dsl import Q
 
 from pyston.contrib.elasticsearch.filters import ElasticsearchFilter
 from pyston.filters.utils import OperatorSlug
 from pyston.filters.exceptions import FilterValueError
@@ -26,15 +26,15 @@
         queryset = user_model.objects.filter(
             **{'{}__contains'.format(user_model.USERNAME_FIELD): value}
         ).annotate(
             str_id=Cast('id', output_field=TextField())
         )
 
         if queryset[:settings.ELASTICSEARCH_MAX_NUMBER_OF_TERMS].count() > settings.ELASTICSEARCH_MAX_NUMBER_OF_TERMS:
-            raise FilterValueError(ugettext('Too many users found for specified username.'))
+            raise FilterValueError(gettext('Too many users found for specified username.'))
 
         return list(queryset.values_list('str_id', flat=True))
 
     def get_filter_term(self, value, operator_slug, request):
         return Q('terms', **{'user_id': value})
 
 
@@ -50,15 +50,15 @@
         ]
 
     def clean_value(self, value, operator_slug, request):
         try:
             return self._enum[value]
         except KeyError:
             raise FilterValueError(
-                ugettext('Invalid value. Please use one of the following values: {}.').format(
+                gettext('Invalid value. Please use one of the following values: {}.').format(
                     ', '.join([a.name for a in self._enum])
                 )
             )
 
     def get_filter_term(self, value, operator_slug, request):
         return Q('term', **{self.get_full_filter_key(): value.name})
 
@@ -84,12 +84,12 @@
                 content_type = ContentType.objects.get(pk=content_type_id)
                 model_db = router.db_for_write(content_type.model_class())
 
                 cleaned_values.append(
                     get_key_from_content_type_object_id_and_model_db(model_db, content_type_id, object_id)
                 )
             except (ValueError, ContentType.DoesNotExist):
-                raise FilterValueError(ugettext('Invalid value.'))
+                raise FilterValueError(gettext('Invalid value.'))
         return cleaned_values
 
     def get_filter_term(self, value, operator_slug, request):
         return Q('terms', related_objects=value)
```

### Comparing `skip-django-security-logger-1.6.4/security/backends/elasticsearch/logstash/handler_tcp.py` & `skip_django_security_logger-1.7.0/security/backends/elasticsearch/logstash/handler_tcp.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/elasticsearch/management/commands/init_elasticsearch_log.py` & `skip_django_security_logger-1.7.0/security/backends/elasticsearch/management/commands/init_elasticsearch_log.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/elasticsearch/models.py` & `skip_django_security_logger-1.7.0/security/backends/elasticsearch/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/elasticsearch/reader.py` & `skip_django_security_logger-1.7.0/security/backends/elasticsearch/reader.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/elasticsearch/tests.py` & `skip_django_security_logger-1.7.0/security/backends/elasticsearch/tests.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/elasticsearch/writer.py` & `skip_django_security_logger-1.7.0/security/backends/elasticsearch/writer.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/logging/writer.py` & `skip_django_security_logger-1.7.0/security/backends/logging/writer.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/purge_logs.py` & `skip_django_security_logger-1.7.0/security/backends/purge_logs.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/reader.py` & `skip_django_security_logger-1.7.0/security/backends/reader.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/signals.py` & `skip_django_security_logger-1.7.0/security/backends/signals.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/app.py` & `skip_django_security_logger-1.7.0/security/backends/sql/app.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/db_router.py` & `skip_django_security_logger-1.7.0/security/backends/sql/db_router.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/is_core/cores.py` & `skip_django_security_logger-1.7.0/security/backends/sql/is_core/cores.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.core.exceptions import ObjectDoesNotExist
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from pyston.utils.decorators import filter_class, order_by
 
 from is_core.utils.decorators import short_description
 
 from is_core.main import DjangoUiRestCore
 from is_core.generic_views.inlines.inline_table_views import DjangoInlineTableView
```

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/is_core/filters.py` & `skip_django_security_logger-1.7.0/security/backends/sql/is_core/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 import operator
 
 from django.contrib.auth import get_user_model
 from django.db.models import TextField, Q
 from django.db.models.functions import Cast
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 from django.contrib.contenttypes.models import ContentType
 
 from pyston.filters.django_filters import SimpleMethodFilter
 from pyston.filters.utils import OperatorSlug
 from pyston.filters.exceptions import FilterValueError
 
 
@@ -37,15 +37,15 @@
     def clean_value(self, value, operator_slug, request):
         cleaned_values = []
         for v in value:
             try:
                 content_type_id, object_id = v.split('|')
                 cleaned_values.append((int(content_type_id), object_id))
             except (ValueError, ContentType.DoesNotExist):
-                raise FilterValueError(ugettext('Invalid value.'))
+                raise FilterValueError(gettext('Invalid value.'))
         return cleaned_values
 
     def get_filter_term(self, value, operator_slug, request):
         return functools.reduce(operator.or_, (
             Q(
                 related_objects__object_id=object_id,
                 related_objects__object_ct_id=object_ct_id
```

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/migrations/0001_initial.py` & `skip_django_security_logger-1.7.0/security/backends/sql/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/migrations/0002_auto_20211119_1940.py` & `skip_django_security_logger-1.7.0/security/backends/sql/migrations/0002_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/migrations/0003_migration.py` & `skip_django_security_logger-1.7.0/security/backends/sql/migrations/0003_migration.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('security_backends_sql', '0002_auto_20211119_1940'),
+        ('security_backends_sql', '0002_migration'),
     ]
 
     operations = [
         migrations.AddField(
             model_name='celerytaskinvocationlog',
             name='parent_log',
             field=models.CharField(blank=True, db_index=True, max_length=250, null=True),
```

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/migrations/0004_migration.py` & `skip_django_security_logger-1.7.0/security/backends/sql/migrations/0004_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/models.py` & `skip_django_security_logger-1.7.0/security/backends/sql/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.serializers.json import DjangoJSONEncoder
 from django.contrib.auth import get_user_model
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.functional import cached_property
 from django.utils.timezone import localtime
 
 from generic_m2m_field.models import MultipleDBGenericManyToManyField
 
 from chamber.models import SmartQuerySet
 
@@ -158,15 +158,15 @@
         null=False,
         blank=False,
         default=RequestLogState.INCOMPLETE
     )
 
     def __str__(self):
         return ' '.join(
-            (force_text(v) for v in (
+            (force_str(v) for v in (
                 self.slug, self.response_code, localtime(self.start.replace(microsecond=0))
             ) if v)
         )
 
     class Meta:
         abstract = True
```

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/reader.py` & `skip_django_security_logger-1.7.0/security/backends/sql/reader.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/sql/writer.py` & `skip_django_security_logger-1.7.0/security/backends/sql/writer.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/testing/reader.py` & `skip_django_security_logger-1.7.0/security/backends/testing/reader.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/testing/writer.py` & `skip_django_security_logger-1.7.0/security/backends/testing/writer.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/backends/writer.py` & `skip_django_security_logger-1.7.0/security/backends/writer.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/command.py` & `skip_django_security_logger-1.7.0/security/command.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/config.py` & `skip_django_security_logger-1.7.0/security/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/contrib/debug_toolbar_log/middleware.py` & `skip_django_security_logger-1.7.0/security/contrib/debug_toolbar_log/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/contrib/pyston/resources.py` & `skip_django_security_logger-1.7.0/security/contrib/pyston/resources.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/decorators.py` & `skip_django_security_logger-1.7.0/security/decorators.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/enums.py` & `skip_django_security_logger-1.7.0/security/enums.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/locale/cs/LC_MESSAGES/django.mo` & `skip_django_security_logger-1.7.0/security/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/locale/cs/LC_MESSAGES/django.po` & `skip_django_security_logger-1.7.0/security/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/logging/celery/logger.py` & `skip_django_security_logger-1.7.0/security/logging/celery/logger.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/logging/commands/logger.py` & `skip_django_security_logger-1.7.0/security/logging/commands/logger.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/logging/common.py` & `skip_django_security_logger-1.7.0/security/logging/common.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/logging/requests/logger.py` & `skip_django_security_logger-1.7.0/security/logging/requests/logger.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/logging/requests/utils.py` & `skip_django_security_logger-1.7.0/security/logging/requests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 
 from urllib.parse import parse_qs, urlparse
 
 from json import JSONDecodeError
 
 from django.template.defaultfilters import truncatechars
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from security.config import settings
 from security.utils import remove_nul_from_string
 
 
 def is_base_collection(v):
     return isinstance(v, (list, tuple, set))
@@ -84,15 +84,15 @@
     elif isinstance(data, str):
         return truncatechars(data, settings.LOG_JSON_STRING_LENGTH)
     else:
         return data
 
 
 def truncate_body(content, max_length):
-    content = force_text(content, errors='replace')
+    content = force_str(content, errors='replace')
     if len(content) > max_length:
         try:
             json_content = json.loads(content)
             return (
                 json.dumps(truncate_json_data(json_content))
                 if isinstance(json_content, (dict, list)) and settings.LOG_JSON_STRING_LENGTH is not None
                 else content[:max_length + 1]
@@ -102,15 +102,15 @@
     else:
         return content
 
 
 def clean_body(body, max_length):
     if body is None:
         return body
-    body = force_text(body, errors='replace')
+    body = force_str(body, errors='replace')
     cleaned_body = truncatechars(
         truncate_body(body, max_length), max_length + len(settings.SENSITIVE_DATA_REPLACEMENT)
     ) if max_length is not None else str(body)
     cleaned_body = hide_sensitive_data_body(remove_nul_from_string(cleaned_body)) if cleaned_body else cleaned_body
     cleaned_body = truncatechars(cleaned_body, max_length) if max_length else cleaned_body
     return cleaned_body
```

### Comparing `skip-django-security-logger-1.6.4/security/management/__init__.py` & `skip_django_security_logger-1.7.0/security/management/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/management/commands/purge_logs.py` & `skip_django_security_logger-1.7.0/security/management/commands/purge_logs.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/middleware.py` & `skip_django_security_logger-1.7.0/security/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/requests.py` & `skip_django_security_logger-1.7.0/security/requests.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/suds.py` & `skip_django_security_logger-1.7.0/security/suds.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/task.py` & `skip_django_security_logger-1.7.0/security/task.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/security/throttling/validators.py` & `skip_django_security_logger-1.7.0/security/throttling/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import timedelta
 
 from django.utils import timezone
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.urls import resolve, Resolver404
 
 from ipware.ip import get_client_ip
 
 from security.config import settings
 from security.backends.reader import get_count_input_requests
 from security.enums import InputRequestSlug
```

### Comparing `skip-django-security-logger-1.6.4/security/utils.py` & `skip_django_security_logger-1.7.0/security/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.6.4/setup.py` & `skip_django_security_logger-1.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,18 +33,18 @@
         'Natural Language :: Czech',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Internet :: WWW/HTTP :: Site Management',
     ],
     install_requires=[
-        'django>=3.1,<4.0',
+        'django>=4.2',
         'django-ipware>=3.0.2',
         'ansi2html>=1.6.0',
-        'skip-django-chamber>=0.6.16.3',
+        'skip-django-chamber>=0.7.2',
         'skip-django-choice-enumfields>=1.1.3.2',
-        'skip-django-generic-m2m-field>=0.0.9.3',
-        'skip-django-celery-extensions>=0.0.37.1',
+        'skip-django-generic-m2m-field>=0.1.0',
+        'skip-django-celery-extensions>=0.1.0',
         'isodate>=0.6.1',
     ],
     zip_safe=False
 )
```

### Comparing `skip-django-security-logger-1.6.4/skip_django_security_logger.egg-info/PKG-INFO` & `skip_django_security_logger-1.7.0/skip_django_security_logger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-security-logger
-Version: 1.6.4
+Version: 1.7.0
 Summary: Django security library.
 Home-page: https://github.com/skip-pay/django-security
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,throttling
 Classifier: Development Status :: 3 - Alpha
@@ -16,21 +16,21 @@
 Classifier: Natural Language :: Czech
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: django<4.0,>=3.1
+Requires-Dist: django>=4.2
 Requires-Dist: django-ipware>=3.0.2
 Requires-Dist: ansi2html>=1.6.0
-Requires-Dist: skip-django-chamber>=0.6.16.3
+Requires-Dist: skip-django-chamber>=0.7.2
 Requires-Dist: skip-django-choice-enumfields>=1.1.3.2
-Requires-Dist: skip-django-generic-m2m-field>=0.0.9.3
-Requires-Dist: skip-django-celery-extensions>=0.0.37.1
+Requires-Dist: skip-django-generic-m2m-field>=0.1.0
+Requires-Dist: skip-django-celery-extensions>=0.1.0
 Requires-Dist: isodate>=0.6.1
 
 Prolog
 ======
 
 Django-security-logger is library for logging input and output request. Library can be used with django-reversion to log which data was changed in a request.
 The library provides throttling security mechanism.
```

### Comparing `skip-django-security-logger-1.6.4/skip_django_security_logger.egg-info/SOURCES.txt` & `skip_django_security_logger-1.7.0/skip_django_security_logger.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 security/backends/sql/models.py
 security/backends/sql/reader.py
 security/backends/sql/writer.py
 security/backends/sql/is_core/__init__.py
 security/backends/sql/is_core/cores.py
 security/backends/sql/is_core/filters.py
 security/backends/sql/migrations/0001_initial.py
-security/backends/sql/migrations/0002_auto_20211119_1940.py
+security/backends/sql/migrations/0002_migration.py
 security/backends/sql/migrations/0003_migration.py
 security/backends/sql/migrations/0004_migration.py
 security/backends/sql/migrations/__init__.py
 security/backends/testing/__init__.py
 security/backends/testing/app.py
 security/backends/testing/reader.py
 security/backends/testing/writer.py
```

