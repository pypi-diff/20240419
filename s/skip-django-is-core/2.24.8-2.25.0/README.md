# Comparing `tmp/skip-django-is-core-2.24.8.tar.gz` & `tmp/skip_django_is_core-2.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-is-core-2.24.8.tar", last modified: Wed Mar 20 10:56:20 2024, max compression
+gzip compressed data, was "skip_django_is_core-2.25.0.tar", last modified: Fri Apr 19 10:34:33 2024, max compression
```

## Comparing `skip-django-is-core-2.24.8.tar` & `skip_django_is_core-2.25.0.tar`

### file list

```diff
@@ -1,263 +1,263 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.753801 skip-django-is-core-2.24.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-20 10:56:20.749801 skip-django-is-core-2.24.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/README
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.713801 skip-django-is-core-2.24.8/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.713801 skip-django-is-core-2.24.8/example/dj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.713801 skip-django-is-core-2.24.8/example/dj/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.713801 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.717801 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/cores/
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/cores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/cores/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/cores/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.717801 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/dynamo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/dynamo/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/dynamo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.717801 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/elasticsearch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/elasticsearch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.717801 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.717801 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.721801 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/dynamo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/field_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/http_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/rest_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/ui_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/ui_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.721801 skip-django-is-core-2.24.8/example/dj/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/dj/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.721801 skip-django-is-core-2.24.8/is_core/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.721801 skip-django-is-core-2.24.8/is_core/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/auth/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.721801 skip-django-is-core-2.24.8/is_core/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.725801 skip-django-is-core-2.24.8/is_core/contrib/background_export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/cores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.725801 skip-django-is-core-2.24.8/is_core/contrib/background_export/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.725801 skip-django-is-core-2.24.8/is_core/contrib/background_export/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/management/commands/deleteexpiredexports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.725801 skip-django-is-core-2.24.8/is_core/contrib/background_export/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/migrations/0002_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.709802 skip-django-is-core-2.24.8/is_core/contrib/background_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.725801 skip-django-is-core-2.24.8/is_core/contrib/background_export/templates/is_core/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/templates/is_core/background_serialization.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.725801 skip-django-is-core-2.24.8/is_core/contrib/background_export/templates/is_core/generic_views/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/templates/is_core/generic_views/table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/background_export/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.725801 skip-django-is-core-2.24.8/is_core/contrib/dynamo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/dynamo/cores.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/dynamo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/dynamo/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/dynamo/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.725801 skip-django-is-core-2.24.8/is_core/contrib/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/elasticsearch/cores.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/elasticsearch/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/elasticsearch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/elasticsearch/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/contrib/elasticsearch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.725801 skip-django-is-core-2.24.8/is_core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/exceptions/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.729801 skip-django-is-core-2.24.8/is_core/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/fieldset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/formsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    13940 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15024 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.729801 skip-django-is-core-2.24.8/is_core/generic_views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/add_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/detail_views.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25720 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/form_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.729801 skip-django-is-core-2.24.8/is_core/generic_views/inlines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/inlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/inlines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/inlines/generic_inline_form_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/inlines/inline_form_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/inlines/inline_objects_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/inlines/inline_table_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/inlines/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/objects_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/generic_views/table_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.709802 skip-django-is-core-2.24.8/is_core/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.709802 skip-django-is-core-2.24.8/is_core/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.729801 skip-django-is-core-2.24.8/is_core/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)    25101 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.733801 skip-django-is-core-2.24.8/is_core/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/models/humanize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.733801 skip-django-is-core-2.24.8/is_core/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/rest/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/rest/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/rest/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/rest/paginators.py
--rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/rest/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.713801 skip-django-is-core-2.24.8/is_core/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.713801 skip-django-is-core-2.24.8/is_core/static/is_core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.733801 skip-django-is-core-2.24.8/is_core/static/is_core/css/
--rw-r--r--   0 runner    (1001) docker     (127)   277370 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/css/app.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.741801 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   136822 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   747545 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)   136516 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    92136 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    78460 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   144714 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34052 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   204814 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   917575 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   204528 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   104280 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    80300 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-solid-900.woff2
--rwxr-xr-x   0 runner    (1001) docker     (127)    32357 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/icon-works-webfont.eot
--rwxr-xr-x   0 runner    (1001) docker     (127)    95652 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/icon-works-webfont.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)    56512 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/icon-works-webfont.ttf
--rwxr-xr-x   0 runner    (1001) docker     (127)    35804 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/fonts/icon-works-webfont.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.741801 skip-django-is-core-2.24.8/is_core/static/is_core/images/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/images/arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/images/cal.png
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/images/select-arrow.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.741801 skip-django-is-core-2.24.8/is_core/static/is_core/js/
--rw-r--r--   0 runner    (1001) docker     (127)  1054526 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/static/is_core/js/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.713801 skip-django-is-core-2.24.8/is_core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.741801 skip-django-is-core-2.24.8/is_core/templates/is_core/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/500.html
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/error.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.745801 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/default_field.html
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/default_fieldset.html
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/default_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/inline_table.html
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/login_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/model_add_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/model_default_form.html
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/model_detail_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/responsive_inline_formset.html
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/responsive_inline_objects.html
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/stacked_inline_formset.html
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/tabular_inline_formset.html
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/forms/tabular_inline_objects.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.745801 skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/add_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/base_table.html
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/default_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/detail_form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/objects.html
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/readonly_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/readonly_fieldset.html
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/rest_documentation.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/table.html
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/home.html
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/logged_out.html
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.745801 skip-django-is-core-2.24.8/is_core/templates/is_core/menu/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/menu/bread_crumbs.html
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/menu/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/menu/sub_menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/menu/tabs_menu.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.745801 skip-django-is-core-2.24.8/is_core/templates/is_core/views/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templates/is_core/views/bulk-change-view.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.745801 skip-django-is-core-2.24.8/is_core/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templatetags/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templatetags/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templatetags/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/templatetags/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.749801 skip-django-is-core-2.24.8/is_core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/tests/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/tests/data_generator_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.749801 skip-django-is-core-2.24.8/is_core/tests/factory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/tests/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/tests/factory/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/tests/rest_generic_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/tests/ui_generic_test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.749801 skip-django-is-core-2.24.8/is_core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/utils/field_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.749801 skip-django-is-core-2.24.8/is_core/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/views/csrf.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/is_core/views/throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 10:56:20.753801 skip-django-is-core-2.24.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-20 10:56:17.000000 skip-django-is-core-2.24.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:56:20.749801 skip-django-is-core-2.24.8/skip_django_is_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-20 10:56:20.000000 skip-django-is-core-2.24.8/skip_django_is_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-03-20 10:56:20.000000 skip-django-is-core-2.24.8/skip_django_is_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:56:20.000000 skip-django-is-core-2.24.8/skip_django_is_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:56:20.000000 skip-django-is-core-2.24.8/skip_django_is_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-20 10:56:20.000000 skip-django-is-core-2.24.8/skip_django_is_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 10:56:20.000000 skip-django-is-core-2.24.8/skip_django_is_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.188297 skip_django_is_core-2.25.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-19 10:34:33.188297 skip_django_is_core-2.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/README
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/dynamo/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/dynamo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/elasticsearch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/elasticsearch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.144297 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.148296 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/dynamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/field_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/http_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/rest_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/ui_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/ui_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.148296 skip_django_is_core-2.25.0/example/dj/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/dj/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/auth/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/background_export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/cores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/background_export/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/background_export/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/management/commands/deleteexpiredexports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/0002_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.136296 skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.152296 skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/is_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/is_core/background_serialization.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.156297 skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/is_core/generic_views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/is_core/generic_views/table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/background_export/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.156297 skip_django_is_core-2.25.0/is_core/contrib/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/dynamo/cores.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/dynamo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/dynamo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/dynamo/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.156297 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/cores.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.156297 skip_django_is_core-2.25.0/is_core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/exceptions/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.160297 skip_django_is_core-2.25.0/is_core/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/fieldset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/formsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13940 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.160297 skip_django_is_core-2.25.0/is_core/generic_views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/add_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/detail_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25711 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/form_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.164296 skip_django_is_core-2.25.0/is_core/generic_views/inlines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/generic_inline_form_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_form_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_objects_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_table_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/inlines/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/objects_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/generic_views/table_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.140297 skip_django_is_core-2.25.0/is_core/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.140297 skip_django_is_core-2.25.0/is_core/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.164296 skip_django_is_core-2.25.0/is_core/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.164296 skip_django_is_core-2.25.0/is_core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/models/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.164296 skip_django_is_core-2.25.0/is_core/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/rest/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.140297 skip_django_is_core-2.25.0/is_core/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.140297 skip_django_is_core-2.25.0/is_core/static/is_core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.164296 skip_django_is_core-2.25.0/is_core/static/is_core/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   277370 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/css/app.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.172297 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   136822 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   747545 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   136516 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    92136 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    78460 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144714 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34052 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   204814 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   917575 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   204528 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   104280 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    80300 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32357 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.eot
+-rwxr-xr-x   0 runner    (1001) docker     (127)    95652 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56512 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35804 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.172297 skip_django_is_core-2.25.0/is_core/static/is_core/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/images/arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/images/cal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/images/select-arrow.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.172297 skip_django_is_core-2.25.0/is_core/static/is_core/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  1054526 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/static/is_core/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.140297 skip_django_is_core-2.25.0/is_core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.176297 skip_django_is_core-2.25.0/is_core/templates/is_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/error.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.180297 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/inline_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/login_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/model_add_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/model_default_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/model_detail_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/responsive_inline_formset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/responsive_inline_objects.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/stacked_inline_formset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/tabular_inline_formset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/forms/tabular_inline_objects.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.180297 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/add_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/base_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/default_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/detail_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/objects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/readonly_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/readonly_fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/rest_documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/logged_out.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.180297 skip_django_is_core-2.25.0/is_core/templates/is_core/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/menu/bread_crumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/menu/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/menu/sub_menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/menu/tabs_menu.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.180297 skip_django_is_core-2.25.0/is_core/templates/is_core/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templates/is_core/views/bulk-change-view.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.180297 skip_django_is_core-2.25.0/is_core/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templatetags/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templatetags/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templatetags/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/templatetags/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.184297 skip_django_is_core-2.25.0/is_core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/data_generator_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.184297 skip_django_is_core-2.25.0/is_core/tests/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/factory/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/rest_generic_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/tests/ui_generic_test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.184297 skip_django_is_core-2.25.0/is_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/utils/field_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.184297 skip_django_is_core-2.25.0/is_core/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/views/csrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/is_core/views/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:34:33.188297 skip_django_is_core-2.25.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-19 10:34:26.000000 skip_django_is_core-2.25.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:34:33.184297 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-19 10:34:33.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-19 10:34:33.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:34:33.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:34:32.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 10:34:33.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 10:34:33.000000 skip_django_is_core-2.25.0/skip_django_is_core.egg-info/top_level.txt
```

### Comparing `skip-django-is-core-2.24.8/LICENSE` & `skip_django_is_core-2.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/PKG-INFO` & `skip_django_is_core-2.25.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-is-core
-Version: 2.24.8
+Version: 2.25.0
 Summary: Information systems core.
 Home-page: https://github.com/skip-pay/django-is-core
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,admin,information systems,REST
 Classifier: Development Status :: 3 - Alpha
@@ -12,19 +12,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django<4.0,>=2.2
+Requires-Dist: django>=4.2
 Requires-Dist: import_string>=0.1.0
-Requires-Dist: skip-django-block-snippets>=2.0.2.1
-Requires-Dist: skip-django-chamber>=0.6.17.1
-Requires-Dist: skip-django-pyston>=2.16.5.1
+Requires-Dist: skip-django-block-snippets>=2.1.0
+Requires-Dist: skip-django-chamber>=0.7.2
+Requires-Dist: skip-django-pyston>=2.17.0
 Requires-Dist: python-dateutil>=2.8.1
 Requires-Dist: pytz
 Requires-Dist: Unidecode
 
 Prolog
 ======
```

### Comparing `skip-django-is-core-2.24.8/README.md` & `skip_django_is_core-2.25.0/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/cores/__init__.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/cores/resources.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/cores/resources.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/dynamo/core.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/dynamo/core.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/elasticsearch/models.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/elasticsearch/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/forms/__init__.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/forms/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pyston.forms import RestModelForm
 
 from django import forms
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class UserForm(RestModelForm):
 
     password = forms.CharField(label=_('Password'), widget=forms.PasswordInput)
 
     def __init__(self, instance=None, *args, **kwargs):
```

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/migrations/0001_initial.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/models.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/dynamo.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/dynamo.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/elasticsearch.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/factories.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/factories.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/field_permissions.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/field_permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/http_exceptions.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/permissions.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/rest.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/rest.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/rest_permissions.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/rest_permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/test_case.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/ui_ordering.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/ui_ordering.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/ui_permissions.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/ui_permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/apps/issue_tracker/tests/utils.py` & `skip_django_is_core-2.25.0/example/dj/apps/issue_tracker/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/settings/base.py` & `skip_django_is_core-2.25.0/example/dj/settings/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Django settings.
 import os
 
 try:
-    from django.utils.translation import ugettext_lazy as _
+    from django.utils.translation import gettext_lazy as _
 except ImportError:
     def _(val): return val
 
 PROJECT_DIR = os.path.abspath(
     os.path.join(os.path.dirname(__file__), '..', '..')
 )
```

### Comparing `skip-django-is-core-2.24.8/example/dj/settings/settings.py` & `skip_django_is_core-2.25.0/example/dj/settings/settings.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/example/dj/wsgi.py` & `skip_django_is_core-2.25.0/example/dj/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/actions.py` & `skip_django_is_core-2.25.0/is_core/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from pyston.utils import JsonObj
 
 
 class Action(JsonObj):
 
     def __init__(self, name, verbose_name, type, class_name=None):
```

### Comparing `skip-django-is-core-2.24.8/is_core/auth/permissions.py` & `skip_django_is_core-2.25.0/is_core/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/auth/views.py` & `skip_django_is_core-2.25.0/is_core/auth/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/config.py` & `skip_django_is_core-2.25.0/is_core/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/background_export/cores.py` & `skip_django_is_core-2.25.0/is_core/contrib/background_export/cores.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/background_export/management/commands/deleteexpiredexports.py` & `skip_django_is_core-2.25.0/is_core/contrib/background_export/management/commands/deleteexpiredexports.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/background_export/migrations/0001_initial.py` & `skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/background_export/migrations/0002_migration.py` & `skip_django_is_core-2.25.0/is_core/contrib/background_export/migrations/0002_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/background_export/models.py` & `skip_django_is_core-2.25.0/is_core/contrib/background_export/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.shortcuts import resolve_url
 from django.utils import timezone
 from django.utils.html import format_html
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from is_core.config import settings as is_core_settings
 from is_core.utils.decorators import short_description
 
 from chamber.models import SmartModel
 from chamber.models.fields import FileField
```

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/background_export/resource.py` & `skip_django_is_core-2.25.0/is_core/contrib/background_export/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from django.contrib.contenttypes.models import ContentType
 from django.shortcuts import render
 from django.utils import translation
-from django.utils.encoding import force_text
-from django.utils.translation import ugettext
+from django.utils.encoding import force_str
+from django.utils.translation import gettext
 
 from is_core.rest.resource import CoreResource, DjangoCoreResource
 
 from django_celery_extensions.task import obj_to_string
 
 from .models import ExportedFile
 from .tasks import background_serialization
 
 
 class ErrorResponseData(dict):
 
     def __init__(self, msg, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self['messages'] = {'error': force_text(msg)}
+        self['messages'] = {'error': force_str(msg)}
 
 
 def apply_background_export(user, queryset, rest_context, fieldset, serialization_format, filename):
     exported_file = ExportedFile.objects.create(
         created_by=user,
         content_type=ContentType.objects.get_for_model(queryset.model)
     )
@@ -39,28 +39,28 @@
     )
 
 
 class CeleryResourceMixin:
 
     def _get_error_response_data(self, message):
         return {
-            'messages': {'error': force_text(message)}
+            'messages': {'error': force_str(message)}
         }
 
     def _get_no_background_permissions_response_data(self, http_headers):
         return ErrorResponseData(
-            ugettext('User doesn\'t have permissions to export')
+            gettext('User doesn\'t have permissions to export')
         ), http_headers, 403, False
 
     def _serialize_data_in_background(self, result):
         apply_background_export(
             self.request.user,
             result,
             self.request._rest_context,
-            force_text(self._get_requested_fieldset(result)),
+            force_str(self._get_requested_fieldset(result)),
             self._get_serialization_format(),
             self._get_filename(),
         )
 
     def _get_filename(self):
         parts = super()._get_filename().rsplit(sep='.', maxsplit=1)
         return (
@@ -90,15 +90,15 @@
     def _get_headers_queryset_context_mapping(self):
         context_mapping = super()._get_headers_queryset_context_mapping()
         context_mapping['background_serialization'] = ('BACKGROUND_SERIALIZATION', '_background_serialization')
         return context_mapping
 
     def _get_name(self):
         obj = self._get_obj_or_none(pk=self.kwargs.get('pk'))
-        return force_text(obj).replace(' ', '-') if obj else super()._get_name()
+        return force_str(obj).replace(' ', '-') if obj else super()._get_name()
 
 
 class CeleryDjangoCoreResource(CeleryResourceMixin, DjangoCoreResource):
     pass
 
 
 class CeleryCoreResource(CeleryResourceMixin, CoreResource):
```

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/background_export/tasks.py` & `skip_django_is_core-2.25.0/is_core/contrib/background_export/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,23 +91,24 @@
         queryset.query = query
 
         # Prepare request.
         if settings.BACKGROUND_EXPORT_TASK_UPDATE_REQUEST_FUNCTION:
             request = import_string(settings.BACKGROUND_EXPORT_TASK_UPDATE_REQUEST_FUNCTION)(request)
 
         # Perform user-defined verification before saving exported file into the database.
+        bg_excs = tuple(import_string(exc) for exc in settings.BACKGROUND_EXPORT_TASK_CALLBACK_HANDLED_EXCEPTIONS)
         if settings.BACKGROUND_EXPORT_TASK_CALLBACK:
             try:
                 import_string(settings.BACKGROUND_EXPORT_TASK_CALLBACK)(
                     request=request,
                     queryset=queryset,
                     filename=filename,
                     exported_file=exported_file,
                 )
-            except tuple(import_string(exc) for exc in settings.BACKGROUND_EXPORT_TASK_CALLBACK_HANDLED_EXCEPTIONS) as exc:
+            except bg_excs as exc:
                 export_failure.send(sender=self.__class__, exception=exc)
                 return
 
         exported_file.file.save(filename, ContentFile(''))
 
         FileBackgroundExportGenerator(query.model).generate(
             exported_file, request, queryset, RFS.create_from_string(requested_fieldset), serialization_format
```

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/background_export/templates/is_core/generic_views/table.html` & `skip_django_is_core-2.25.0/is_core/contrib/background_export/templates/is_core/generic_views/table.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/background_export/views.py` & `skip_django_is_core-2.25.0/is_core/contrib/background_export/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.conf import settings
-from django.conf.urls import url
+from django.urls import re_path as url
 from django.contrib.auth.decorators import login_required
 from django.views.generic.base import RedirectView
 
 from chamber.shortcuts import get_object_or_404
 
 from is_core.exceptions import HttpForbiddenResponseException
 from is_core.site import get_model_core
```

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/dynamo/cores.py` & `skip_django_is_core-2.25.0/is_core/contrib/dynamo/cores.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/dynamo/views.py` & `skip_django_is_core-2.25.0/is_core/contrib/dynamo/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/elasticsearch/cores.py` & `skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/cores.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/elasticsearch/filters.py` & `skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/contrib/elasticsearch/views.py` & `skip_django_is_core-2.25.0/is_core/contrib/elasticsearch/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/exceptions/response.py` & `skip_django_is_core-2.25.0/is_core/exceptions/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import mimeparse
 
 from django.http.response import HttpResponse, HttpResponseRedirect
 from django.template.loader import render_to_string
-from django.utils.encoding import force_text
-from django.utils.translation import ugettext_lazy as _
+from django.utils.encoding import force_str
+from django.utils.translation import gettext_lazy as _
 
 import import_string
 
 from pyston.utils import set_rest_context_to_request
 from pyston.converters import (
     get_converter, get_supported_mime_types, get_converter_name_from_request, get_default_converters
 )
@@ -43,18 +43,18 @@
         status=response_code
     )
 
 
 def rest_response_exception_factory(request, response_code, title, message, response_class=HttpResponse,
                                     rest_error_response_class=None):
     message = (
-        ', '.join([force_text(val) for val in message])
+        ', '.join([force_str(val) for val in message])
         if isinstance(message, (list, tuple))
-        else force_text(message)
-    ) if message else force_text(title)
+        else force_str(message)
+    ) if message else force_str(title)
     set_rest_context_to_request(request, BaseResource.DEFAULT_REST_CONTEXT_MAPPING)
     converter_name = get_converter_name_from_request(request)
     converter = get_converter(converter_name)
     response = response_class(status=response_code, content_type=converter.content_type)
 
     rest_error_response_class = rest_error_response_class or import_string(pyston_settings.ERROR_RESPONSE_CLASS)
```

### Comparing `skip-django-is-core-2.24.8/is_core/forms/boundfield.py` & `skip_django_is_core-2.25.0/is_core/forms/boundfield.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/forms/fields.py` & `skip_django_is_core-2.25.0/is_core/forms/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django import forms
 from django.core.exceptions import ValidationError
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from is_core.forms.widgets import ReadonlyWidget, EmptyWidget, DivButtonWidget
 
 
 class ReadonlyField(forms.Field):
 
     widget = ReadonlyWidget
@@ -20,15 +20,15 @@
     def _has_changed(self, initial, data):
         return self.has_changed(initial, data)
 
     def has_changed(self, initial, data):
         return False
 
     def validate(self, value):
-        raise ValidationError(ugettext('Readonly field can not be validated'))
+        raise ValidationError(gettext('Readonly field can not be validated'))
 
 
 class EmptyReadonlyField(ReadonlyField):
 
     widget = EmptyWidget
     readonly_widget = EmptyWidget
```

### Comparing `skip-django-is-core-2.24.8/is_core/forms/fieldset.py` & `skip_django_is_core-2.25.0/is_core/forms/fieldset.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/forms/forms.py` & `skip_django_is_core-2.25.0/is_core/forms/forms.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/forms/formsets.py` & `skip_django_is_core-2.25.0/is_core/forms/formsets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.forms.formsets import DEFAULT_MIN_NUM, DEFAULT_MAX_NUM, BaseFormSet as OriginBaseFormSet
+from django.forms.renderers import get_default_renderer
 
 
 class BaseFormSetMixin:
     """
     Mixin that add method all_forms which return existing forms and empty form in one list
     """
 
@@ -55,10 +56,11 @@
         'can_order': can_order,
         'can_delete': can_delete,
         'can_delete_extra': can_delete_extra,
         'min_num': min_num,
         'max_num': max_num,
         'absolute_max': absolute_max,
         'validate_min': validate_min,
-        'validate_max': validate_max
+        'validate_max': validate_max,
+        'renderer': get_default_renderer(),
     }
     return type(form.__name__ + 'FormSet', (formset,), attrs)
```

### Comparing `skip-django-is-core-2.24.8/is_core/forms/generic.py` & `skip_django_is_core-2.25.0/is_core/forms/generic.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/forms/models.py` & `skip_django_is_core-2.25.0/is_core/forms/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/forms/patch.py` & `skip_django_is_core-2.25.0/is_core/forms/patch.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/forms/utils.py` & `skip_django_is_core-2.25.0/is_core/forms/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/forms/widgets.py` & `skip_django_is_core-2.25.0/is_core/forms/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from django import forms
 from django.core.validators import EMPTY_VALUES
 from django.db.models.base import Model
 from django.db.models.fields.files import FieldFile
 from django.forms.utils import flatatt
 from django.forms.widgets import MultiWidget, TextInput, Widget
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.functional import cached_property
 from django.utils.html import conditional_escape, format_html, format_html_join
 from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from is_core.config import settings
 from is_core.utils import EMPTY_VALUE, display_json
 
 from .utils import ReadonlyValue, add_class_name
 
 
@@ -200,15 +200,15 @@
         if hasattr(widget, 'choices'):
             return widget.choices.get_choice_from_value(value)
 
     def _render_readonly(self, name, value, attrs=None, renderer=None, request=None, form=None, initial_value=None):
         if request and self._get_widget():
             choice = self._choice(value)
             if choice:
-                rendered_value = self._render_object(request, choice.obj, force_text(choice[1]))
+                rendered_value = self._render_object(request, choice.obj, force_str(choice[1]))
             elif value in EMPTY_VALUES:
                 rendered_value = EMPTY_VALUE
 
             return format_html('<p>{}</p>', rendered_value)
         else:
             return super()._render_readonly(name, value, attrs, renderer, request, form, initial_value)
 
@@ -217,15 +217,15 @@
 
     def _render_readonly(self, name, value, attrs=None, renderer=None, request=None, form=None, initial_value=None):
         if request and isinstance(value, (list, tuple)) and self._get_widget():
             rendered_values = []
             for value_item in value:
                 choice = self._choice(value_item)
                 if choice:
-                    value_item = force_text(choice[1])
+                    value_item = force_str(choice[1])
                     if choice.obj:
                         rendered_values.append(self._render_object(request, choice.obj, value_item))
                     else:
                         rendered_values.append(value_item)
             return format_html(
                 '<p>{}</p>',
                 format_html_join(', ', '{}', ((v,) for v in rendered_values)) if rendered_values else EMPTY_VALUE
@@ -288,15 +288,15 @@
         super().__init__(attrs)
         self.separator = separator
 
     def render(self, name, value, attrs=None, renderer=None):
         if isinstance(value, str):
             value = [value]
         return super().render(
-            name, '{} '.format(self.separator).join(map(force_text, value)) if value else value, attrs, renderer
+            name, '{} '.format(self.separator).join(map(force_str, value)) if value else value, attrs, renderer
         )
 
     def value_from_datadict(self, data, files, name):
         value = super().value_from_datadict(data, files, name)
         return [v.strip() for v in value.split(self.separator)] if isinstance(value, str) else value
```

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/add_views.py` & `skip_django_is_core-2.25.0/is_core/generic_views/add_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from is_core.auth.permissions import PermissionsSet, CoreCreateAllowed, CoreAllowed, DEFAULT_PERMISSION
 
 from .form_views import DjangoCoreFormView
 
 
 class DjangoAddFormView(DjangoCoreFormView):
```

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/base.py` & `skip_django_is_core-2.25.0/is_core/generic_views/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from urllib.parse import urlunparse, urlparse
 
 from django.contrib.auth import REDIRECT_FIELD_NAME
 from django.http import QueryDict
 from django.http.response import Http404
 from django.views.generic.base import TemplateView
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.urls import reverse
 
 from block_snippets.views import JSONSnippetTemplateResponseMixin
 
 from is_core.auth.permissions import PermissionsSet, CoreReadAllowed, CoreAllowed, DEFAULT_PERMISSION
 from is_core.menu import LinkMenuItem
 from is_core.exceptions import (
```

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/detail_views.py` & `skip_django_is_core-2.25.0/is_core/generic_views/detail_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.http.response import Http404
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.utils.functional import cached_property
 from django.views.generic.base import TemplateView
 from django.template import RequestContext
 
 from chamber.shortcuts import get_object_or_none
 
 from is_core.auth.views import FieldPermissionViewMixin
```

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/form_views.py` & `skip_django_is_core-2.25.0/is_core/generic_views/form_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from copy import deepcopy
 
 from django.core.exceptions import ImproperlyConfigured, ValidationError
 from django.http.response import HttpResponseRedirect, Http404
-from django.utils.encoding import force_text
-from django.utils.translation import ugettext_lazy as _
+from django.utils.encoding import force_str
+from django.utils.translation import gettext_lazy as _
 from django.views.generic.edit import FormView
 from django.contrib.messages.api import get_messages, add_message
 from django.contrib.messages import constants
 
 from chamber.utils.forms import formset_has_file_field
 from chamber.utils import transaction
 
@@ -75,15 +75,15 @@
     def get_form_action(self):
         return self.request.get_full_path()
 
     def get_readonly_fields(self):
         return () if self.readonly_fields is None else self.readonly_fields
 
     def get_message_kwargs(self, obj):
-        return {'obj': force_text(obj)}
+        return {'obj': force_str(obj)}
 
     def get_message(self, msg_type_or_level, obj=None):
         msg_kwargs = {}
         if obj:
             msg_kwargs = self.get_message_kwargs(obj)
 
         msg_type = (isinstance(msg_type_or_level, int) and constants.DEFAULT_TAGS.get(msg_type_or_level) or
@@ -120,24 +120,24 @@
         try:
             if self.atomic_save_form:
                 obj = self._atomic_save_form(form, **kwargs)
             else:
                 obj = self.save_form(form, **kwargs)
             return self.success_render_to_response(obj, msg, msg_level)
         except ValidationError as ex:
-            return self.form_invalid(form, msg=force_text(ex.message), **kwargs)
+            return self.form_invalid(form, msg=force_str(ex.message), **kwargs)
 
     def form_invalid(self, form, msg=None, msg_level=None, **kwargs):
         msg_level = msg_level or constants.ERROR
         msg = msg or self.get_message(msg_level)
         add_message(self.request, msg_level, msg)
         return self.render_to_response(self.get_context_data(form=form, msg=msg, msg_level=msg_level, **kwargs))
 
     def get_popup_obj(self, obj):
-        return {'_obj_name': force_text(obj)}
+        return {'_obj_name': force_str(obj)}
 
     @property
     def is_ajax_form(self):
         """Return if form will be rendered for ajax"""
         return self.has_snippet()
 
     @property
@@ -265,15 +265,15 @@
             return HttpResponseRedirect(self.get_success_url(obj))
 
     def render_to_response(self, context, **response_kwargs):
         if self.has_snippet():
             extra_content = response_kwargs['extra_content'] = response_kwargs.get('extra_content', {})
             extra_content_messages = {}
             for message in get_messages(self.request):
-                extra_content_messages[message.tags] = force_text(message)
+                extra_content_messages[message.tags] = force_str(message)
             if extra_content_messages:
                 extra_content['messages'] = extra_content_messages
         return super().render_to_response(context, **response_kwargs)
 
 
 class DjangoBaseFormView(FieldPermissionViewMixin, BaseFormView):
 
@@ -297,15 +297,15 @@
         form_field = super().form_field(form, field_name, form_field)
         placeholder = self.model._ui_meta.placeholders.get(field_name, None)
         if placeholder:
             form_field.widget.placeholder = placeholder
         return form_field
 
     def get_message_kwargs(self, obj):
-        return {'obj': force_text(obj), 'name': force_text(obj._meta.verbose_name)}
+        return {'obj': force_str(obj), 'name': force_str(obj._meta.verbose_name)}
 
     def get_exclude(self):
         return self.exclude
 
     def generate_readonly_fields(self):
         return list(self.get_readonly_fields()) + list(self._get_readonly_fields_from_permissions())
 
@@ -508,15 +508,15 @@
             'show_save_button': show_buttons and self.has_save_button()
         })
         return context_data
 
     def get_popup_obj(self, obj):
         app_label = self.model._meta.app_label
         model_name = self.model._meta.object_name
-        return {'_obj_name': force_text(obj), 'pk': obj.pk, '_model': '%s.%s' % (app_label, model_name)}
+        return {'_obj_name': force_str(obj), 'pk': obj.pk, '_model': '%s.%s' % (app_label, model_name)}
 
 
 class DjangoCoreFormView(ListParentMixin, DjangoBaseFormView):
 
     show_save_and_continue = True
 
     save_button_title = _('Save and navigate to the list')
```

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/inlines/base.py` & `skip_django_is_core-2.25.0/is_core/generic_views/inlines/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/inlines/generic_inline_form_views.py` & `skip_django_is_core-2.25.0/is_core/generic_views/inlines/generic_inline_form_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/inlines/inline_form_views.py` & `skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_form_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.forms.formsets import DELETION_FIELD_NAME
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.utils.functional import cached_property
 
 from chamber.utils.forms import formset_has_file_field
 
 from is_core.forms.models import BaseInlineFormSet, smartinlineformset_factory, SmartModelForm
 from is_core.generic_views.inlines.base import RelatedInlineView
 from is_core.forms.fields import SmartReadonlyField, EmptyReadonlyField
```

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/inlines/inline_objects_views.py` & `skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_objects_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/inlines/inline_table_views.py` & `skip_django_is_core-2.25.0/is_core/generic_views/inlines/inline_table_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/inlines/permissions.py` & `skip_django_is_core-2.25.0/is_core/generic_views/inlines/permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/mixins.py` & `skip_django_is_core-2.25.0/is_core/generic_views/mixins.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/objects_views.py` & `skip_django_is_core-2.25.0/is_core/generic_views/objects_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/generic_views/table_views.py` & `skip_django_is_core-2.25.0/is_core/generic_views/table_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/loading.py` & `skip_django_is_core-2.25.0/is_core/loading.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import OrderedDict
 
 from importlib import import_module
 
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.apps import apps
 
 
 class App:
 
     def __init__(self):
         self.cores = []
@@ -29,15 +29,15 @@
     def _init_apps(self):
         import_module('is_core.main')
 
         for app in apps.get_app_configs():
             try:
                 import_module('{}.cores'.format(app.name))
             except ImportError as ex:
-                if force_text(ex) != 'No module named \'{}.cores\''.format(app.name):
+                if force_str(ex) != 'No module named \'{}.cores\''.format(app.name):
                     raise ex
 
     def get_cores(self):
         self._init_apps()
 
         for app in self.apps.values():
             for core in app.cores:
```

### Comparing `skip-django-is-core-2.24.8/is_core/locale/cs/LC_MESSAGES/django.mo` & `skip_django_is_core-2.25.0/is_core/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/locale/cs/LC_MESSAGES/django.po` & `skip_django_is_core-2.25.0/is_core/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/main.py` & `skip_django_is_core-2.25.0/is_core/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import sys
 
 from copy import deepcopy
 
 from collections import OrderedDict
 
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.utils.functional import cached_property
 from django.urls import reverse
 
 import import_string
 
 from is_core.auth.permissions import FieldsSetPermission
 from is_core.config import settings
```

### Comparing `skip-django-is-core-2.24.8/is_core/menu.py` & `skip_django_is_core-2.25.0/is_core/menu.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/middleware.py` & `skip_django_is_core-2.25.0/is_core/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.http.response import Http404
 from django.core.exceptions import ValidationError
-from django.utils.encoding import force_text
-from django.utils.translation import ugettext
+from django.utils.encoding import force_str
+from django.utils.translation import gettext
 from django.urls import resolve, Resolver404
 from django.conf import settings
 
 from is_core.exceptions import ResponseException
 from is_core.exceptions.response import response_exception_factory
 from is_core.utils.compatibility import MiddlewareMixin
 
@@ -26,10 +26,10 @@
 # Not working with pyston exceptions
 class HttpExceptionsMiddleware(MiddlewareMixin):
 
     def process_exception(self, request, exception):
         if isinstance(exception, ResponseException):
             return exception.get_response(request)
         if isinstance(exception, ValidationError):
-            return response_exception_factory(request, 422, ugettext('Unprocessable Entity'), exception.messages)
+            return response_exception_factory(request, 422, gettext('Unprocessable Entity'), exception.messages)
         if not settings.DEBUG and isinstance(exception, Http404):
-            return response_exception_factory(request, 404, ugettext('Not Found'), force_text(exception))
+            return response_exception_factory(request, 404, gettext('Not Found'), force_str(exception))
```

### Comparing `skip-django-is-core-2.24.8/is_core/models/patch.py` & `skip_django_is_core-2.25.0/is_core/models/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import django.db.models.options as options
 
 from django.db import models
 from django.db.models.fields import URLField
 from django.db.models.fields.related import ForeignKey, ManyToManyField, OneToOneField
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from chamber.patch import Options
 
 from .humanize import url_humanized
 
 
 options.DEFAULT_NAMES = options.DEFAULT_NAMES + ('default_fk_filter', 'default_m2m_filter', 'default_rel_filter')
```

### Comparing `skip-django-is-core-2.24.8/is_core/patterns.py` & `skip_django_is_core-2.25.0/is_core/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from collections import OrderedDict
 
-from django.conf.urls import url
+from django.urls import re_path as url
 from django.urls import reverse, resolve
 
 from is_core.utils import get_new_class_name, PK_PATTERN, NUMBER_PK_PATTERN
 
 
 logger = logging.getLogger('is-core')
```

### Comparing `skip-django-is-core-2.24.8/is_core/rest/datastructures.py` & `skip_django_is_core-2.25.0/is_core/rest/datastructures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from pyston.utils import RestFieldset, RestField
 
 from is_core.utils.field_api import get_field_descriptors_from_path, FieldIsNotRelation
 
 
 def generate_subfield(submodel, subfield_name, field_class):
@@ -63,13 +63,13 @@
 
     fields_class = ModelRestFlatField
 
     def __init__(self, *fields):
         self.fields = fields
 
     def __str__(self):
-        return ','.join(map(force_text, self.fields))
+        return ','.join(map(force_str, self.fields))
 
 
 class ModelRestFieldset(RestFieldset, ModelFlatRestFieldsMixin):
 
     fields_class = ModelRestField
```

### Comparing `skip-django-is-core-2.24.8/is_core/rest/filters.py` & `skip_django_is_core-2.25.0/is_core/rest/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/rest/paginators.py` & `skip_django_is_core-2.25.0/is_core/rest/paginators.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/rest/resource.py` & `skip_django_is_core-2.25.0/is_core/rest/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import wraps
 
 from django.conf import settings as django_settings
 from django.http.response import Http404
 from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext
-from django.utils.encoding import force_text
+from django.utils.translation import gettext
+from django.utils.encoding import force_str
 from django.urls import NoReverseMatch
 
 from pyston.conf import settings as pyston_settings
 from pyston.forms import rest_modelform_factory
 from pyston.exception import (RestException, MimerDataException, NotAllowedException, UnsupportedMediaTypeException,
                               ResourceNotFoundException, NotAllowedMethodException, DuplicateEntryException,
                               ConflictException, DataInvalidException, UnauthorizedException)
@@ -395,15 +395,15 @@
 
     @transaction.smart_atomic
     def update_bulk(self):
         qs = self._filter_queryset(self._get_queryset())
         BULK_CHANGE_LIMIT = getattr(django_settings, 'BULK_CHANGE_LIMIT', 200)
         if qs.count() > BULK_CHANGE_LIMIT:
             return RestErrorResponse(
-                msg=ugettext('Only %s objects can be changed by one request').format(BULK_CHANGE_LIMIT),
+                msg=gettext('Only %s objects can be changed by one request').format(BULK_CHANGE_LIMIT),
                 code=413)
 
         data = self.get_dict_data()
         objects, errors = zip(*(self._update_obj(obj, data) for obj in qs))
         compact_errors = tuple(err for err in errors if err)
         return RestErrorsResponse(compact_errors) if len(compact_errors) > 0 else objects
 
@@ -422,10 +422,10 @@
             raise
         except RestException as ex:
             return (None, self._format_message(obj, ex))
 
     def _format_message(self, obj, ex):
         return {
             'id': obj.pk,
-            'errors': {k: mark_safe(force_text(v)) for k, v in ex.errors.items()} if hasattr(ex, 'errors') else {},
-            '_obj_name': force_text(obj),
+            'errors': {k: mark_safe(force_str(v)) for k, v in ex.errors.items()} if hasattr(ex, 'errors') else {},
+            '_obj_name': force_str(obj),
         }
```

### Comparing `skip-django-is-core-2.24.8/is_core/site.py` & `skip_django_is_core-2.25.0/is_core/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.conf.urls import url, include
+from django.urls import re_path as url, include
 from django.core.exceptions import ImproperlyConfigured
 
 import import_string
 
 from is_core.config import settings
 
 from .patterns import RestPattern
```

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/css/app.css` & `skip_django_is_core-2.25.0/is_core/static/is_core/css/app.css`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-brands-400.eot` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-brands-400.svg` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-brands-400.ttf` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-brands-400.woff` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-brands-400.woff2` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-regular-400.eot` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-regular-400.svg` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-regular-400.ttf` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-regular-400.woff` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-regular-400.woff2` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-solid-900.eot` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-solid-900.svg` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-solid-900.ttf` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-solid-900.woff` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/fa-solid-900.woff2` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/icon-works-webfont.eot` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.eot`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/icon-works-webfont.svg` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.svg`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/icon-works-webfont.ttf` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.ttf`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/fonts/icon-works-webfont.woff` & `skip_django_is_core-2.25.0/is_core/static/is_core/fonts/icon-works-webfont.woff`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/images/arrow.png` & `skip_django_is_core-2.25.0/is_core/static/is_core/images/arrow.png`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/images/cal.png` & `skip_django_is_core-2.25.0/is_core/static/is_core/images/cal.png`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/images/select-arrow.png` & `skip_django_is_core-2.25.0/is_core/static/is_core/images/select-arrow.png`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/static/is_core/js/app.js` & `skip_django_is_core-2.25.0/is_core/static/is_core/js/app.js`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/base.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/base.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/forms/default_field.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_field.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/forms/default_fieldset.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_fieldset.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/forms/default_form.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/default_form.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/forms/inline_table.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/inline_table.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/forms/model_default_form.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/model_default_form.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/forms/responsive_inline_formset.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/responsive_inline_formset.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/forms/responsive_inline_objects.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/responsive_inline_objects.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/forms/stacked_inline_formset.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/stacked_inline_formset.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/forms/tabular_inline_formset.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/tabular_inline_formset.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/forms/tabular_inline_objects.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/forms/tabular_inline_objects.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/base_table.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/base_table.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/default_form.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/default_form.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/detail_form.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/detail_form.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/objects.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/objects.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/generic_views/readonly_fieldset.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/generic_views/readonly_fieldset.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/logged_out.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/logged_out.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/login.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/login.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templates/is_core/menu/menu.html` & `skip_django_is_core-2.25.0/is_core/templates/is_core/menu/menu.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templatetags/forms.py` & `skip_django_is_core-2.25.0/is_core/templatetags/forms.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templatetags/menu.py` & `skip_django_is_core-2.25.0/is_core/templatetags/menu.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/templatetags/permissions.py` & `skip_django_is_core-2.25.0/is_core/templatetags/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.template.base import Node, TemplateSyntaxError, NodeList, kwarg_re
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.functional import SimpleLazyObject
 from django.template import Library
 
 from is_core.utils import get_link_or_none
 
 
 register = Library()
@@ -82,15 +82,15 @@
         self.nodelist_false = nodelist_false
         self.kwargs = kwargs
 
     def render(self, context):
         pattern_name = self.pattern_name.resolve(context, True)
         request = context.get('request')
         kwargs = {
-            force_text(k, 'ascii'): v.resolve(context)
+            force_str(k, 'ascii'): v.resolve(context)
             for k, v in self.kwargs.items()
         }
 
         link = get_link_or_none(pattern_name, request, view_kwargs=kwargs)
         if link:
             return self.nodelist_true.render(context.new({'url': link}))
         else:
```

### Comparing `skip-django-is-core-2.24.8/is_core/templatetags/utils.py` & `skip_django_is_core-2.25.0/is_core/templatetags/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/tests/crawler.py` & `skip_django_is_core-2.25.0/is_core/tests/crawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from germanium.tools import assert_true, assert_not_equal
 from germanium.decorators import login
 from germanium.crawler import Crawler, LinkExtractor
 from germanium.crawler import HTMLLinkExtractor as OriginalHTMLLinkExtractor
 
 
@@ -108,15 +108,15 @@
                 headers['HTTP_X_FIELDS'] = '_rest_links,_web_links'
             if self.REST_BASE:
                 headers['HTTP_X_BASE'] = str(self.REST_BASE)
             return url, headers
 
         def post_response(url, referer, resp, exception):
             tested_urls.append(url)
-            assert_true(exception is None, msg='Received exception %s, url %s' % (force_text(exception), url))
+            assert_true(exception is None, msg='Received exception %s, url %s' % (force_str(exception), url))
             if resp.status_code != 200:
                 failed_urls.append(url)
                 self.logger.warning('Response code for url %s from referer %s should be 200 but code is %s, user %s' %
                                     (url, referer, resp.status_code, self.logged_user.user))
             assert_not_equal(resp.status_code, 500, msg='Response code for url %s from referer %s is 500, user %s' %
                              (url, referer, self.logged_user.user))
         Crawler(self.c, ('/',), self.get_exlude_urls(), pre_request, post_response,
```

### Comparing `skip-django-is-core-2.24.8/is_core/tests/data_generator_test_case.py` & `skip_django_is_core-2.25.0/is_core/tests/data_generator_test_case.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/tests/factory/fields.py` & `skip_django_is_core-2.25.0/is_core/tests/factory/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/tests/rest_generic_test_cases.py` & `skip_django_is_core-2.25.0/is_core/tests/rest_generic_test_cases.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/tests/ui_generic_test_cases.py` & `skip_django_is_core-2.25.0/is_core/tests/ui_generic_test_cases.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/utils/__init__.py` & `skip_django_is_core-2.25.0/is_core/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 
 from django.core.exceptions import ImproperlyConfigured
 from django.contrib.admin.utils import display_for_value as admin_display_for_value
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db.models import QuerySet
 from django.core.exceptions import FieldDoesNotExist
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 from django.utils.html import format_html, format_html_join
 from django.utils.formats import get_format, date_format
 from django.utils.timezone import template_localtime
 
 from chamber.utils import call_function_with_unknown_input
 
 from pyston.converters import get_converter
@@ -283,15 +283,15 @@
                         )
                     )
                     for k, v in value.items()
                 )
             )
         )
     elif isinstance(value, bool):
-        return ugettext('Yes') if value else ugettext('No')
+        return gettext('Yes') if value else gettext('No')
     elif isinstance(value, datetime.datetime):
         return date_format(template_localtime(value), (
              'DATETIME_FORMAT' if get_format('IS_CORE_VIEW_DATETIME_FORMAT') == 'IS_CORE_VIEW_DATETIME_FORMAT'
              else 'IS_CORE_VIEW_DATETIME_FORMAT'
          ))
     elif isinstance(value, datetime.date):
         return date_format(value, (
@@ -329,15 +329,15 @@
         return call_function_with_unknown_input(obj.get_absolute_url, request=request)
     else:
         return get_url_from_model_core(request, obj)
 
 
 def render_model_object_with_link(request, obj, display_value=None):
     if obj is None:
-        return '[{}]'.format(ugettext('missing object'))
+        return '[{}]'.format(gettext('missing object'))
 
     obj_url = get_obj_url(request, obj)
     display_value = str(obj) if display_value is None else str(display_value)
 
     return format_html('<a href="{}">{}</a>', obj_url, display_value) if obj_url else display_value
```

### Comparing `skip-django-is-core-2.24.8/is_core/utils/decorators.py` & `skip_django_is_core-2.25.0/is_core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/utils/field_api.py` & `skip_django_is_core-2.25.0/is_core/utils/field_api.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/is_core/utils/models.py` & `skip_django_is_core-2.25.0/is_core/utils/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.8/setup.py` & `skip_django_is_core-2.25.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,18 +29,18 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Internet :: WWW/HTTP',
     ],
     install_requires=[
-        'django>=2.2, <4.0',
+        'django>=4.2',
         'import_string>=0.1.0',
-        'skip-django-block-snippets>=2.0.2.1',
-        'skip-django-chamber>=0.6.17.1',
-        'skip-django-pyston>=2.16.5.1',
+        'skip-django-block-snippets>=2.1.0',
+        'skip-django-chamber>=0.7.2',
+        'skip-django-pyston>=2.17.0',
         'python-dateutil>=2.8.1',
         'pytz',
         'Unidecode',
     ],
     zip_safe=False
 )
```

### Comparing `skip-django-is-core-2.24.8/skip_django_is_core.egg-info/PKG-INFO` & `skip_django_is_core-2.25.0/skip_django_is_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-is-core
-Version: 2.24.8
+Version: 2.25.0
 Summary: Information systems core.
 Home-page: https://github.com/skip-pay/django-is-core
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,admin,information systems,REST
 Classifier: Development Status :: 3 - Alpha
@@ -12,19 +12,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django<4.0,>=2.2
+Requires-Dist: django>=4.2
 Requires-Dist: import_string>=0.1.0
-Requires-Dist: skip-django-block-snippets>=2.0.2.1
-Requires-Dist: skip-django-chamber>=0.6.17.1
-Requires-Dist: skip-django-pyston>=2.16.5.1
+Requires-Dist: skip-django-block-snippets>=2.1.0
+Requires-Dist: skip-django-chamber>=0.7.2
+Requires-Dist: skip-django-pyston>=2.17.0
 Requires-Dist: python-dateutil>=2.8.1
 Requires-Dist: pytz
 Requires-Dist: Unidecode
 
 Prolog
 ======
```

### Comparing `skip-django-is-core-2.24.8/skip_django_is_core.egg-info/SOURCES.txt` & `skip_django_is_core-2.25.0/skip_django_is_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

