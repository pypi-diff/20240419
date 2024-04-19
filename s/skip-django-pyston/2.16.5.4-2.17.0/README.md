# Comparing `tmp/skip-django-pyston-2.16.5.4.tar.gz` & `tmp/skip_django_pyston-2.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-pyston-2.16.5.4.tar", last modified: Tue Apr  2 14:13:32 2024, max compression
+gzip compressed data, was "skip_django_pyston-2.17.0.tar", last modified: Fri Apr 19 10:11:17 2024, max compression
```

## Comparing `skip-django-pyston-2.16.5.4.tar` & `skip_django_pyston-2.17.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.254338 skip-django-pyston-2.16.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-02 14:13:32.254338 skip-django-pyston-2.16.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/example/dj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/example/dj/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/example/dj/apps/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.242338 skip-django-pyston-2.16.5.4/example/dj/apps/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/elasticsearch/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/elasticsearch/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.242338 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0002_user_manual_created_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0003_auto_20170729_2305.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0004_issue_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/serializable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.242338 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/dynamo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/extra_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)    29627 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/fieldsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15447 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/standard_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.242338 skip-django-pyston-2.16.5.4/example/dj/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/dj/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.246338 skip-django-pyston-2.16.5.4/pyston/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.246338 skip-django-pyston-2.16.5.4/pyston/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.246338 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.246338 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.246338 skip-django-pyston-2.16.5.4/pyston/converters/
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/converters/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/converters/file_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15358 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/django_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    16820 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/filters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/forms/
--rw-r--r--   0 runner    (1001) docker     (127)    35083 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/forms/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/pyston/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.238338 skip-django-pyston-2.16.5.4/pyston/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/metamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/order/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/django_sorters.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/sorters.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/order/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/requested_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/requested_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/requested_fields/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/requested_fields/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    41564 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    35172 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/templates/default_pdf_table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/templates/pyston/
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/templates/pyston/html_converter.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.250338 skip-django-pyston-2.16.5.4/pyston/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/pyston/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:13:32.254338 skip-django-pyston-2.16.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-02 14:13:29.000000 skip-django-pyston-2.16.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:32.254338 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 14:13:32.000000 skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.239024 skip_django_pyston-2.17.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 10:11:17.235024 skip_django_pyston-2.17.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.219024 skip_django_pyston-2.17.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.219024 skip_django_pyston-2.17.0/example/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.219024 skip_django_pyston-2.17.0/example/dj/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.219024 skip_django_pyston-2.17.0/example/dj/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.219024 skip_django_pyston-2.17.0/example/dj/apps/app/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/dynamo/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/dynamo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.219024 skip_django_pyston-2.17.0/example/dj/apps/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/elasticsearch/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/elasticsearch/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.223024 skip_django_pyston-2.17.0/example/dj/apps/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/migrations/0002_user_manual_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/migrations/0003_auto_20170729_2305.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/migrations/0004_issue_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.223024 skip_django_pyston-2.17.0/example/dj/apps/app/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/dynamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/extra_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/fieldsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15447 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/standard_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/apps/app/tests/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.227024 skip_django_pyston-2.17.0/example/dj/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/dj/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.227024 skip_django_pyston-2.17.0/pyston/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.227024 skip_django_pyston-2.17.0/pyston/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.227024 skip_django_pyston-2.17.0/pyston/contrib/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/dynamo/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/dynamo/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/dynamo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/dynamo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.231024 skip_django_pyston-2.17.0/pyston/contrib/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/elasticsearch/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/elasticsearch/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/elasticsearch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/contrib/elasticsearch/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.231024 skip_django_pyston-2.17.0/pyston/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)    15483 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/converters/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/converters/file_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.231024 skip_django_pyston-2.17.0/pyston/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15350 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/filters/django_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16813 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/filters/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/filters/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/filters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.231024 skip_django_pyston-2.17.0/pyston/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)    35058 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/forms/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.215024 skip_django_pyston-2.17.0/pyston/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.215024 skip_django_pyston-2.17.0/pyston/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.231024 skip_django_pyston-2.17.0/pyston/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/metamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.235024 skip_django_pyston-2.17.0/pyston/order/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/order/django_sorters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/order/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11231 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/order/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/order/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/order/sorters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/order/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.235024 skip_django_pyston-2.17.0/pyston/requested_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/requested_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/requested_fields/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/requested_fields/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41559 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35166 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.235024 skip_django_pyston-2.17.0/pyston/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/templates/default_pdf_table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.235024 skip_django_pyston-2.17.0/pyston/templates/pyston/
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/templates/pyston/html_converter.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.235024 skip_django_pyston-2.17.0/pyston/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/utils/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/pyston/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:11:17.239024 skip_django_pyston-2.17.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 10:11:14.000000 skip_django_pyston-2.17.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:11:17.235024 skip_django_pyston-2.17.0/skip_django_pyston.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 10:11:17.000000 skip_django_pyston-2.17.0/skip_django_pyston.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-19 10:11:17.000000 skip_django_pyston-2.17.0/skip_django_pyston.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:11:17.000000 skip_django_pyston-2.17.0/skip_django_pyston.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:11:17.000000 skip_django_pyston-2.17.0/skip_django_pyston.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-19 10:11:17.000000 skip_django_pyston-2.17.0/skip_django_pyston.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 10:11:17.000000 skip_django_pyston-2.17.0/skip_django_pyston.egg-info/top_level.txt
```

### Comparing `skip-django-pyston-2.16.5.4/AUTHORS.txt` & `skip_django_pyston-2.17.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/LICENSE` & `skip_django_pyston-2.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/PKG-INFO` & `skip_django_pyston-2.17.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: skip-django-pyston
-Version: 2.16.5.4
+Version: 2.17.0
 Summary: Pyston is a Django mini-framework creating APIs.
 Home-page: https://github.com/skip-pay/django-pyston
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 License-File: AUTHORS.txt
-Requires-Dist: django<4.0,>=2.2
+Requires-Dist: django>=4.2
 Requires-Dist: defusedxml>=0.6.0
 Requires-Dist: pyparsing==2.4.7
 Requires-Dist: python-mimeparse>=1.6.0
-Requires-Dist: skip-django-chamber>=0.6.17.2
+Requires-Dist: skip-django-chamber>=0.7.2
 Requires-Dist: python-magic>=0.4.27
```

### Comparing `skip-django-pyston-2.16.5.4/README.md` & `skip_django_pyston-2.17.0/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/models.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/dynamo/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/dynamo/resource.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/dynamo/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/elasticsearch/models.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/elasticsearch/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0001_initial.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/migrations/0003_auto_20170729_2305.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/migrations/0003_auto_20170729_2305.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/models.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db import models
 from django.db.models import Count
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from pyston.utils.decorators import order_by, filter_class, filter_by, allow_tags, sorter_class
 from pyston.filters.filters import IntegerFilterMixin
 from pyston.filters.utils import OperatorSlug
 from pyston.filters.django_filters import CONTAINS, StringFieldFilter, SimpleMethodEqualFilter
 from pyston.order.django_sorters import ExtraDjangoSorter
```

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/resource.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/serializable.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/serializable.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/compatibility.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/compatibility.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/cors.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/cors.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/dynamo.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/dynamo.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/elasticsearch.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/extra_resource.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/extra_resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/factories.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/factories.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/fields.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import os
 
 from django.conf import settings
 from django.test.utils import override_settings
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from germanium.decorators import data_consumer
 from germanium.tools.trivials import assert_in, assert_equal, assert_not_equal
 from germanium.tools.http import assert_http_bad_request, assert_http_created
 from germanium.tools.rest import assert_valid_JSON_created_response, assert_valid_JSON_response
 
 import responses
@@ -436,52 +436,52 @@
         }
         resp = self.post(self.USER_API_URL, data=data)
         assert_http_bad_request(resp)
         errors = self.deserialize(resp).get('messages', {}).get('errors')
         assert_in('contract', errors)
         assert_equal(
             errors['contract'],
-            ugettext('Content type cannot be evaluated from input data please send it')
+            gettext('Content type cannot be evaluated from input data please send it')
         )
 
     @data_consumer('get_users_data')
     def test_should_raise_bad_request_if_file_content_is_not_in_base64(self, number, data):
         data['contract'] = {
             'content_type': 'text/plain',
             'filename': 'contract.txt',
             'content': 'abc',
         }
         resp = self.post(self.USER_API_URL, data=data)
         assert_http_bad_request(resp)
         errors = self.deserialize(resp).get('messages', {}).get('errors')
         assert_in('contract', errors)
-        assert_equal(errors['contract']['content'], ugettext('File content must be in base64 format'))
+        assert_equal(errors['contract']['content'], gettext('File content must be in base64 format'))
 
     @data_consumer('get_users_data')
     def test_should_raise_bad_request_if_url_is_not_valid(self, number, data):
         data['contract'] = {
             'filename': 'testfile.pdf',
             'url': 'hs://foo.bar/testfile.pdf',
         }
         resp = self.post(self.USER_API_URL, data=data)
         assert_http_bad_request(resp)
         errors = self.deserialize(resp).get('messages', {}).get('errors')
         assert_in('contract', errors)
-        assert_equal(errors['contract']['url'], ugettext('Enter a valid URL.'))
+        assert_equal(errors['contract']['url'], gettext('Enter a valid URL.'))
 
     @data_consumer('get_users_data')
     def test_should_raise_bad_request_if_required_items_are_not_provided(self, number, data):
         REQUIRED_ITEMS = {'content'}
         REQUIRED_URL_ITEMS = {'url'}
         data['contract'] = {}
         resp = self.post(self.USER_API_URL, data=data)
         assert_http_bad_request(resp)
         errors = self.deserialize(resp).get('messages', {}).get('errors')
         assert_in('contract', errors)
-        msg = ugettext('File data item must contains {} or {}').format(
+        msg = gettext('File data item must contains {} or {}').format(
                   ', '.join(REQUIRED_ITEMS), ', '.join(REQUIRED_URL_ITEMS)
               )
         assert_equal(errors['contract'], msg)
 
     @data_consumer('get_users_data')
     def test_should_raise_bad_request_if_file_is_unreachable(self, number, data):
         url = 'http://foo.bar/testfile.pdf'
@@ -489,15 +489,15 @@
             'filename': 'testfile.pdf',
             'url': url,
         }
         resp = self.post(self.USER_API_URL, data=data)
         assert_http_bad_request(resp)
         errors = self.deserialize(resp).get('messages', {}).get('errors')
         assert_in('contract', errors)
-        assert_equal(errors['contract']['url'], ugettext('File is unreachable on the URL address'))
+        assert_equal(errors['contract']['url'], gettext('File is unreachable on the URL address'))
 
     @override_settings(PYSTON_FILE_SIZE_LIMIT=10)
     @data_consumer('get_users_data')
     def test_should_raise_bad_request_if_response_is_too_large(self, number, data):
         data['contract'] = {
             'content_type': 'text/plain',
             'filename': 'contract.txt',
@@ -505,15 +505,15 @@
                 ('Contract of %s code: šří+áýšé' % data['email']).encode('utf-8')
             ).decode('utf-8')
         }
         resp = self.get_file_url_response(data)
         assert_http_bad_request(resp)
         errors = self.deserialize(resp).get('messages', {}).get('errors')
         assert_in('contract', errors)
-        msg = ugettext('Response too large, maximum size is {} bytes').format(pyston_settings.FILE_SIZE_LIMIT)
+        msg = gettext('Response too large, maximum size is {} bytes').format(pyston_settings.FILE_SIZE_LIMIT)
         assert_equal(errors['contract']['url'], msg)
 
     @data_consumer('get_users_data')
     def test_filename_and_content_type_can_be_evaluated_from_file_content(self, number, data):
         data['contract'] = {
             'content': base64.b64encode(
                 ('Contract of %s code: šří+áýšé' % data['email']).encode('utf-8')
```

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/fieldsets.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/fieldsets.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/filter.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/filter.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/order.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/order.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/serializer.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/serializer.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/standard_operations.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/standard_operations.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/apps/app/tests/test_case.py` & `skip_django_pyston-2.17.0/example/dj/apps/app/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/settings/base.py` & `skip_django_pyston-2.17.0/example/dj/settings/base.py`

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

### Comparing `skip-django-pyston-2.16.5.4/example/dj/settings/settings.py` & `skip_django_pyston-2.17.0/example/dj/settings/settings.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/example/dj/urls.py` & `skip_django_pyston-2.17.0/example/dj/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.conf import settings
-from django.conf.urls import url
+from django.urls import re_path as url
 
 from app.dynamo.resource import CommentDynamoResource
 from app.elasticsearch.resource import CommentElasticsearchResource
 from app.resource import (
     IssueResource, UserResource, ExtraResource, CountIssuesPerUserResource, CountWatchersPerIssueResource,
     TestCamelCaseResource, CountWatchersPerIssueResource, UserResource, UserWithFormResource, IssueWithFormResource
 )
```

### Comparing `skip-django-pyston-2.16.5.4/example/dj/wsgi.py` & `skip_django_pyston-2.17.0/example/dj/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/cache.py` & `skip_django_pyston-2.17.0/pyston/cache.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/conf.py` & `skip_django_pyston-2.17.0/pyston/conf.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/filter.py` & `skip_django_pyston-2.17.0/pyston/contrib/dynamo/filter.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/order.py` & `skip_django_pyston-2.17.0/pyston/contrib/dynamo/order.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/paginator.py` & `skip_django_pyston-2.17.0/pyston/contrib/dynamo/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import base64
 import json
 
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from pyston.exception import RestException
 from pyston.paginator import BasePaginator
 from pyston.response import HeadersResponse
 
 
 class DynamoCursorBasedPaginator(BasePaginator):
@@ -29,30 +29,30 @@
     def _get_base(self, request):
         base = request._rest_context.get('base')
         if not base:
             return self.default_base
         elif base.isdigit():
             base_int = int(base)
             if base_int > self.max_base:
-                raise RestException(ugettext('Base must lower or equal to {}').format(self.max_base))
+                raise RestException(gettext('Base must lower or equal to {}').format(self.max_base))
             else:
                 return base_int
         else:
-            raise RestException(ugettext('Base must be natural number or empty'))
+            raise RestException(gettext('Base must be natural number or empty'))
 
     def _get_cursor(self, request):
         cursor = request._rest_context.get('cursor')
         if cursor:
             try:
                 cursor = base64.b64decode(
                     cursor.encode('ascii')
                 ).decode('ascii')
                 return json.loads(cursor)
             except json.JSONDecodeError:
-                raise RestException(ugettext('Invalid next cursor value'))
+                raise RestException(gettext('Invalid next cursor value'))
         else:
             return None
 
     def get_next_cursor(self, qs):
         return base64.b64encode(
             json.dumps(qs.next_key).encode('ascii')
         ).decode('ascii') if qs.next_key else None
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/contrib/dynamo/resource.py` & `skip_django_pyston-2.17.0/pyston/contrib/dynamo/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/filters.py` & `skip_django_pyston-2.17.0/pyston/contrib/elasticsearch/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/order.py` & `skip_django_pyston-2.17.0/pyston/contrib/elasticsearch/order.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/contrib/elasticsearch/resource.py` & `skip_django_pyston-2.17.0/pyston/contrib/elasticsearch/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/converters/__init__.py` & `skip_django_pyston-2.17.0/pyston/converters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from collections import OrderedDict
 
 from defusedxml import ElementTree as ET
 from django.core.serializers.json import DjangoJSONEncoder
 from django.http.response import HttpResponseBase
 from django.template.loader import get_template
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.xmlutils import SimplerXMLGenerator
 from django.utils.module_loading import import_string
 from django.utils.html import format_html
 
 from pyston.utils.helpers import UniversalBytesIO, serialized_data_to_python
 from pyston.utils.datastructures import FieldsetGenerator
 from pyston.conf import settings
@@ -171,15 +171,15 @@
                 xml.endElement('resource')
         elif isinstance(data, dict):
             for key, value in data.items():
                 xml.startElement(key, {})
                 self._to_xml(xml, value)
                 xml.endElement(key)
         else:
-            xml.characters(force_text(data))
+            xml.characters(force_str(data))
 
     def _encode(self, data, **kwargs):
         if data is not None:
             stream = StringIO()
 
             xml = SimplerXMLGenerator(stream, 'utf-8')
             xml.startDocument()
@@ -283,15 +283,15 @@
 
     def render_value(self, value, first=True):
         if isinstance(value, dict):
             return self._render_dict(value, first)
         elif is_collection(value):
             return self._render_iterable(value, first)
         else:
-            return force_text(value)
+            return force_str(value)
 
     def _get_value_from_row(self, data, field):
         return self.render_value(self._get_recursive_value_from_row(data, field.key_path) or '')
 
     def _render_row(self, row, field_name_list):
         return (self._get_value_from_row(row, field) for field in field_name_list)
 
@@ -302,15 +302,15 @@
 
         return (self._render_row(row, field_name_list) for row in constructed_data)
 
     def _encode_to_stream(self, output_stream, data, resource=None, requested_fields=None, direct_serialization=False,
                           **kwargs):
         fieldset = FieldsetGenerator(
             resource,
-            force_text(requested_fields) if requested_fields is not None else None,
+            force_str(requested_fields) if requested_fields is not None else None,
             direct_serialization=direct_serialization
         ).generate()
         self.generator_class().generate(
             self._render_headers(fieldset),
             self._render_content(fieldset, data),
             output_stream
         )
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/converters/extra.py` & `skip_django_pyston-2.17.0/pyston/converters/extra.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/converters/file_generators.py` & `skip_django_pyston-2.17.0/pyston/converters/file_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import csv
 import codecs
 
 from datetime import datetime, date
 from decimal import Decimal
 
 from django.conf import settings as django_settings
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.template.loader import get_template
 
 try:
     # xlsxwriter isn't standard with python.  It shouldn't be required if it
     # isn't used.
     import xlsxwriter
 except ImportError:
@@ -64,27 +64,27 @@
             prepared_row.append(value)
         return prepared_row
 
     def _prepare_value(self, value):
         if isinstance(value, float):
             value = ('%.2f' % value).replace('.', ',')
         elif isinstance(value, Decimal):
-            value = force_text(value.quantize(TWOPLACES)).replace('.', ',')
+            value = force_str(value.quantize(TWOPLACES)).replace('.', ',')
         else:
-            value = force_text(value)
+            value = force_str(value)
         return value.replace('&nbsp;', ' ')
 
 
 class StreamCSV:
 
     def __init__(self, f, dialect=csv.excel, use_bom=True, **kwargs):
         self.writer = csv.writer(f, dialect=dialect, **kwargs)
         self.stream = f
         if use_bom:
-            self.stream.write(force_text(codecs.BOM_UTF8))  # BOM for Excel
+            self.stream.write(force_str(codecs.BOM_UTF8))  # BOM for Excel
 
     def writerow(self, row):
         self.writer.writerow(row)
         self.stream.flush()
 
     def writerows(self, rows):
         for row in rows:
@@ -101,15 +101,15 @@
         for data_row in data:
             output_stream.write('\n')
             for col, val in enumerate(data_row):
                 if header:
                     output_stream.write('{}:\n'.format(header[col]))
                 if isinstance(val, str):
                     val = self._prepare_value(val)
-                output_stream.write('\t'.join(('\t' + force_text(val).lstrip()).splitlines(True)) + '\n\n')
+                output_stream.write('\t'.join(('\t' + force_str(val).lstrip()).splitlines(True)) + '\n\n')
             output_stream.write('---\n')
 
 
 if xlsxwriter:
     class XlsxGenerator:  # noqa: F811
 
         def _prepare_value(self, value):
@@ -123,15 +123,15 @@
             datetime_format = wb.add_format({'num_format': 'd. mmmm yyyy hh:mm:ss'})
             decimal_format = wb.add_format({'num_format': '0.00'})
 
             row = 0
 
             if header:
                 for col, head in enumerate(header):
-                    ws.write(row, col, force_text(head))
+                    ws.write(row, col, force_str(head))
                 row += 1
 
             for data_row in data:
                 for col, val in enumerate(data_row):
                     if isinstance(val, datetime):
                         ws.write(row, col, val.replace(tzinfo=None), datetime_format)
                     elif isinstance(val, date):
@@ -159,14 +159,14 @@
                 }
                 for k, v in urls.items():
                     if (uri.startswith(v)):
                         return os.path.join(k, uri.replace(v, ""))
                 return ''
 
             pisa.pisaDocument(
-                force_text(
+                force_str(
                     get_template(settings.PDF_EXPORT_TEMPLATE).render(
                         {'pagesize': 'A4', 'headers': header, 'data': data}
                     )
                 ),
                 output_stream, encoding=self.encoding, link_callback=fetch_resources
             )
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/data_processor.py` & `skip_django_pyston-2.17.0/pyston/data_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import base64
 import inspect
 
 from io import BytesIO
 
 from django.forms.fields import FileField
-from django.utils.translation import ugettext_lazy as _, ugettext
+from django.utils.translation import gettext_lazy as _, gettext
 from django.core.files.uploadedfile import InMemoryUploadedFile
 from django.core.validators import URLValidator
 from django.core.exceptions import ValidationError
 
 from requests.exceptions import RequestException
 
 from pyston.conf import settings as pyston_settings
@@ -78,15 +78,15 @@
 
 @data_preprocessors.register(BaseModelResource)
 class FileDataPreprocessor(DataProcessor):
 
     def _validate_not_empty(self, data_item, key, item):
         if not data_item.get(item):
             error = self.errors.get(key, RestDictError())
-            error.update(RestDictError({item: RestValidationError(ugettext('This field is required'))}))
+            error.update(RestDictError({item: RestValidationError(gettext('This field is required'))}))
             self.errors[key] = error
 
     def _get_content_type(self, content_type, filename, file_content):
         if content_type:
             return content_type
         elif filename:
             return get_content_type_from_filename(filename)
@@ -102,19 +102,19 @@
     def _process_file_data(self, data, files, key, data_item, file_content):
         filename = data_item.get('filename')
         content_type = data_item.get('content_type')
 
         content_type = self._get_content_type(content_type, filename, file_content)
         filename = self._get_filename(content_type, filename)
         if not content_type:
-            self.errors[key] = RestValidationError(ugettext(
+            self.errors[key] = RestValidationError(gettext(
                 'Content type cannot be evaluated from input data please send it'
             ))
         elif not filename:
-            self.errors[key] = RestValidationError(ugettext(
+            self.errors[key] = RestValidationError(gettext(
                 'File name cannot be evaluated from input data please send it'
             ))
         else:
             filename = self._get_filename(content_type, filename)
             charset = data_item.get('charset')
             files[key] = InMemoryUploadedFile(
                 file_content, field_name=key, name=filename, content_type=content_type,
@@ -124,15 +124,15 @@
 
     def _process_file_data_field(self, data, files, key, data_item):
         try:
             file_content = BytesIO(base64.b64decode(data_item.get('content').encode('utf-8')))
             self._process_file_data(data, files, key, data_item, file_content)
         except (TypeError, binascii.Error):
             self.errors[key] = RestDictError({'content': RestValidationError(
-                ugettext('File content must be in base64 format')
+                gettext('File content must be in base64 format')
             )})
 
     def _process_file_data_url_field(self, data, files, key, data_item):
         url = data_item.get('url')
         try:
             file_name, content_type, file_content = get_file_name_type_and_content_from_url(
                 url, pyston_settings.FILE_SIZE_LIMIT
@@ -140,21 +140,21 @@
 
             data_item['filename'] = data_item.get('filename', file_name)
             data_item['content_type'] = data_item.get('content_type', content_type)
 
             self._process_file_data(data, files, key, data_item, file_content)
         except RequestDataTooBig:
             self.errors[key] = RestDictError({'url': RestValidationError(
-                ugettext('Response too large, maximum size is {} bytes').format(
+                gettext('Response too large, maximum size is {} bytes').format(
                     pyston_settings.FILE_SIZE_LIMIT
                 ))
             })
         except (RequestException, InvalidResponseStatusCode):
             self.errors[key] = RestDictError({'url': RestValidationError(
-                ugettext('File is unreachable on the URL address')
+                gettext('File is unreachable on the URL address')
             )})
         try:
             url_validator(url)
         except ValidationError as e:
             self.errors[key] = RestDictError({'url': RestValidationError(e.messages[0])})
 
     def _process_field(self, data, files, key, data_item):
@@ -173,15 +173,15 @@
                 for item in REQUIRED_URL_ITEMS:
                     self._validate_not_empty(data_item, key, item)
 
                 if not self.errors:
                     self._process_file_data_url_field(data, files, key, data_item)
             else:
                 self.errors[key] = RestValidationError(
-                    ugettext('File data item must contains {} or {}').format(
+                    gettext('File data item must contains {} or {}').format(
                         ', '.join(REQUIRED_ITEMS), ', '.join(REQUIRED_URL_ITEMS)
                     )
                 )
 
 
 class ModelResourceDataProcessor(DataProcessor):
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/exception.py` & `skip_django_pyston-2.17.0/pyston/exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class UnsupportedMediaTypeException(Exception):
     """
     Raised if the content_type has unsupported media type
     """
     pass
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/filters/django_filters.py` & `skip_django_pyston-2.17.0/pyston/filters/django_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.db.models import (
     Q, AutoField, DateField, DateTimeField, DecimalField, GenericIPAddressField, IPAddressField, BooleanField,
     TextField, CharField, IntegerField, FloatField, SlugField, EmailField, NullBooleanField, UUIDField, JSONField
 )
 from django.db.models.fields.related import ForeignKey, ManyToManyField, ForeignObjectRel
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from pyston.utils import LOOKUP_SEP
 
 from .filters import (
     OperatorQuery, BooleanFilterMixin, NullBooleanFilterMixin, OperatorsModelFieldFilter,
     FloatFilterMixin, IntegerFilterMixin, DecimalFilterMixin,
     IPAddressFilterMixin, GenericIPAddressFilterMixin, DateFilterMixin,
@@ -57,30 +57,30 @@
     def _clean_list_values(self, filter, operator_slug, request, values):
         cleaned_values = []
         i = 0
         for value in values:
             try:
                 cleaned_values.append(filter.clean_value(value, operator_slug, request))
             except FilterValueError as ex:
-                raise FilterValueError(ugettext('Invalid value inside list at position {}, {}').format(i, ex))
+                raise FilterValueError(gettext('Invalid value inside list at position {}, {}').format(i, ex))
             i += 1
         return cleaned_values
 
 
 class SimpleListOperatorQuery(ListOperatorMixin, OperatorQuery):
     """
     The operator object is alternative to the Simple operator. It only accepts data in list format.
     """
 
     def __init__(self, orm_operator):
         self.orm_operator = orm_operator
 
     def get_q(self, filter, values, operator_slug, request):
         if not isinstance(values, list):
-            raise FilterValueError(ugettext('Value must be list'))
+            raise FilterValueError(gettext('Value must be list'))
         else:
             values = self._clean_list_values(filter, operator_slug, request, values)
         q = Q(**{
             '{}__{}'.format(filter.get_full_filter_key(), self.orm_operator): {v for v in values if values is not None}
         })
         if None in values:
             q |= Q(**{'{}__isnull'.format(filter.get_full_filter_key()): True})
@@ -90,28 +90,28 @@
 class RangeOperatorQuery(ListOperatorMixin, OperatorQuery):
     """
     Operator filters range between two input values.
     """
 
     def get_q(self, filter, values, operator_slug, request):
         if not isinstance(values, list) or not len(values) != 2:
-            raise FilterValueError(ugettext('Value must be list with two values'))
+            raise FilterValueError(gettext('Value must be list with two values'))
         else:
             values = self._clean_list_values(filter, operator_slug, request, values)
         return Q(**{'{}__range'.format(filter.get_full_filter_key()): values})
 
 
 class AllListOperatorQuery(ListOperatorMixin, OperatorQuery):
     """
     Operator that is used for filtering m2m or m2o relations. All sent values must be related.
     """
 
     def get_q(self, filter, values, operator_slug, request):
         if not isinstance(values, list):
-            raise FilterValueError(ugettext('Value must be list'))
+            raise FilterValueError(gettext('Value must be list'))
         else:
             values = self._clean_list_values(filter, operator_slug, request, values)
 
         qs_obj_with_all_values = filter.field.model.objects.all()
         for v in set(values):
             qs_obj_with_all_values = qs_obj_with_all_values.filter(**{filter.identifiers[-1]: v})
         return Q(
@@ -305,15 +305,15 @@
 
     def clean_value(self, value, operator_slug, request):
         if value is None or operator_slug in {OperatorSlug.CONTAINS, OperatorSlug.ICONTAINS}:
             return value
         try:
             return self.get_last_rel_field(self.field).get_prep_value(value)
         except ValueError:
-            raise FilterValueError(ugettext('Object with this PK cannot be found'))
+            raise FilterValueError(gettext('Object with this PK cannot be found'))
 
 
 class ManyToManyFieldFilter(RelatedFieldFilter):
 
     operators = (
         (OperatorSlug.EQ, EQ),
         (OperatorSlug.IN, IN),
@@ -326,15 +326,15 @@
         if value is None or operator_slug in {OperatorSlug.CONTAINS, OperatorSlug.ICONTAINS}:
             return value
         try:
             return self.get_last_rel_field(
                 self.field.related_model._meta.get_field(self.field.related_model._meta.pk.name)
             ).get_prep_value(value)
         except ValueError:
-            raise FilterValueError(ugettext('Object with this PK cannot be found'))
+            raise FilterValueError(gettext('Object with this PK cannot be found'))
 
 
 class ForeignObjectRelFilter(RelatedFieldFilter):
 
     operators = (
         (OperatorSlug.EQ, EQ),
         (OperatorSlug.IN, IN),
@@ -347,15 +347,15 @@
         if value is None or operator_slug in {OperatorSlug.CONTAINS, OperatorSlug.ICONTAINS}:
             return value
         try:
             return self.get_last_rel_field(
                 self.field.related_model._meta.get_field(self.field.related_model._meta.pk.name)
             ).get_prep_value(value)
         except ValueError:
-            raise FilterValueError(ugettext('Object with this PK cannot be found'))
+            raise FilterValueError(gettext('Object with this PK cannot be found'))
 
 
 class SimpleFilterMixin:
     """
     Helper that is used for implementation all simple custom filters.
     """
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/filters/filters.py` & `skip_django_pyston-2.17.0/pyston/filters/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from decimal import Decimal, InvalidOperation
 
 from django.core.validators import validate_ipv4_address, validate_ipv46_address
 from django.core.exceptions import ValidationError
-from django.utils.translation import ugettext
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext
+from django.utils.translation import gettext_lazy as _
 from django.utils.timezone import make_aware
 
 from dateutil.parser import DEFAULTPARSER
 
 from pyston.utils import LOOKUP_SEP
 
 from .exceptions import FilterValueError, OperatorFilterError
@@ -156,15 +156,15 @@
         if isinstance(value, bool):
             return value
         elif value in {'true', 'false'}:
             return value == 'true'
         elif value in {'0', '1'}:
             return value == '1'
         else:
-            raise FilterValueError(ugettext('Value must be boolean'))
+            raise FilterValueError(gettext('Value must be boolean'))
 
 
 class NullBooleanFilterMixin(BooleanFilterMixin):
     """
     Helper that contains cleaner for boolean input values where value can be None.
     """
 
@@ -188,94 +188,94 @@
 
     def clean_value(self, value, operator_slug, request):
         if value is None:
             return value
         try:
             return int(value)
         except (ValueError, TypeError):
-            raise FilterValueError(ugettext('Value must be integer'))
+            raise FilterValueError(gettext('Value must be integer'))
 
 
 class FloatFilterMixin:
 
     def clean_value(self, value, operator_slug, request):
         if value is None:
             return value
         try:
             return float(value)
         except (ValueError, TypeError):
-            raise FilterValueError(ugettext('Value must be float'))
+            raise FilterValueError(gettext('Value must be float'))
 
 
 class DecimalFilterMixin:
 
     def clean_value(self, value, operator_slug, request):
         if value is None:
             return value
         try:
             return Decimal(value)
         except InvalidOperation:
-            raise FilterValueError(ugettext('Value must be decimal'))
+            raise FilterValueError(gettext('Value must be decimal'))
 
 
 class IPAddressFilterMixin:
 
     def clean_value(self, value, operator_slug, request):
         if value is None:
             return value
         elif operator_slug not in {OperatorSlug.CONTAINS, OperatorSlug.EXACT,
                                    OperatorSlug.STARTSWITH, OperatorSlug.ENDSWITH}:
             try:
                 validate_ipv4_address(value)
             except ValidationError:
-                raise FilterValueError(ugettext('Value must be in format IPv4.'))
+                raise FilterValueError(gettext('Value must be in format IPv4.'))
         return value
 
 
 class GenericIPAddressFilterMixin:
 
     def clean_value(self, value, operator_slug, request):
         if value is None:
             return value
         elif operator_slug not in {OperatorSlug.CONTAINS, OperatorSlug.EXACT,
                                    OperatorSlug.STARTSWITH, OperatorSlug.ENDSWITH}:
             try:
                 validate_ipv46_address(value)
             except ValidationError:
-                raise FilterValueError(ugettext('Value must be in format IPv4 or IPv6.'))
+                raise FilterValueError(gettext('Value must be in format IPv4 or IPv6.'))
         return value
 
 
 class DateFilterMixin:
 
     suffixes = {
         'day', 'month', 'year'
     }
 
     def _clean_datetime_to_parts(self, value):
         value = DEFAULTPARSER._parse(value, dayfirst='-' not in value)
         value = value[0] if isinstance(value, tuple) else value
 
         if value is None:
-            raise FilterValueError(ugettext('Value cannot be parsed to partial datetime'))
+            raise FilterValueError(gettext('Value cannot be parsed to partial datetime'))
         else:
             return value
 
     def _clean_integer(self, value):
         try:
             return int(value)
         except ValueError:
-            raise FilterValueError(ugettext('Value must be integer'))
+            raise FilterValueError(gettext('Value must be integer'))
 
     def _clean_datetime(self, value):
         try:
             datetime_value = DEFAULTPARSER.parse(value, dayfirst='-' not in value)
             return make_aware(datetime_value, is_dst=True) if datetime_value.tzinfo is None else datetime_value
         except ValueError:
-            raise FilterValueError(ugettext('Value must be in format ISO 8601.'))
+            raise FilterValueError(gettext('Value must be in format ISO 8601.'))
 
     def clean_value(self, value, operator_slug, request):
         suffix = self.identifiers_suffix[0] if self.identifiers_suffix else None
         if suffix in self.suffixes:
             return self._clean_integer(value)
         elif operator_slug == OperatorSlug.CONTAINS:
             return self._clean_datetime_to_parts(value)
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/filters/managers.py` & `skip_django_pyston-2.17.0/pyston/filters/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.db.models import Q
 from django.core.exceptions import FieldDoesNotExist
 from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from pyston.exception import RestException
 from pyston.utils import rfs, LOOKUP_SEP
 from pyston.utils.helpers import get_field_or_none, get_method_or_none
 from pyston.serializer import get_resource_or_none
 
 from .exceptions import FilterValueError, OperatorFilterError, FilterIdentifierError
@@ -257,21 +257,21 @@
 
 
 class BaseParserModelFilterManager(BaseModelFilterManager):
 
     parsers = [DefaultFilterParser(), QueryStringFilterParser()]
 
     def _logical_conditions_and(self, condition_a, condition_b):
-        raise RestException(ugettext('More filter terms combination are not supported'))
+        raise RestException(gettext('More filter terms combination are not supported'))
 
     def _logical_conditions_or(self, condition_a, condition_b):
-        raise RestException(ugettext('More filter terms combination are not supported'))
+        raise RestException(gettext('More filter terms combination are not supported'))
 
     def _logical_conditions_negation(self, condition):
-        raise RestException(ugettext('Filter term negation are not supported'))
+        raise RestException(gettext('Filter term negation are not supported'))
 
     def _convert_logical_conditions(self, condition, resource, request):
         """
         Method that recursive converts condition tree to the django models Q objects.
         """
         if condition.is_composed and condition.operator_slug == LogicalOperatorSlug.NOT:
             return self._logical_conditions_negation(
@@ -290,23 +290,23 @@
         else:
             try:
                 return self.get_filter(condition.identifiers, resource, request).get_q(
                     condition.value, condition.operator_slug, request
                 )
             except FilterIdentifierError:
                 raise RestException(
-                    mark_safe(ugettext('Invalid identifier of condition "{}"').format(condition.source))
+                    mark_safe(gettext('Invalid identifier of condition "{}"').format(condition.source))
                 )
             except FilterValueError as ex:
                 raise RestException(
-                    mark_safe(ugettext('Invalid value of condition "{}". {}').format(condition.source, ex))
+                    mark_safe(gettext('Invalid value of condition "{}". {}').format(condition.source, ex))
                 )
             except OperatorFilterError:
                 raise RestException(
-                    mark_safe(ugettext('Invalid operator of condition "{}"').format(condition.source))
+                    mark_safe(gettext('Invalid operator of condition "{}"').format(condition.source))
                 )
 
     def _is_required_distinct(self, qs, q):
         for lookup in get_flat_lookups(q):
             if is_required_distinct_for_lookup(qs.model, lookup):
                 return True
         return False
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/filters/parser.py` & `skip_django_pyston-2.17.0/pyston/filters/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 
 import pyparsing as pp
 
 from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from .utils import LogicalOperatorSlug, OperatorSlug
 
 
 class FilterParserError(Exception):
     """
     Exception that is raised if filter input is invalid.
@@ -177,15 +177,15 @@
 
         try:
             return self._parse_to_conditions(
                 expr.parseString(input, parseAll=True).asList()[0], list(condition_positions), condition, input
             )
         except pp.ParseException:
             raise FilterParserError(
-                mark_safe(ugettext('Invalid filter value "{}"').format(input))
+                mark_safe(gettext('Invalid filter value "{}"').format(input))
             )
 
 
 class FlatAndFilterParser(FilterParser):
     """
     Helper used to implement parsers that join terms only with AND operator.
     """
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/filters/utils.py` & `skip_django_pyston-2.17.0/pyston/filters/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/forms/__init__.py` & `skip_django_pyston-2.17.0/pyston/forms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from collections import OrderedDict
 
 from django import forms
 from django.core.exceptions import NON_FIELD_ERRORS, ValidationError
 from django.http.response import Http404
 from django.forms.models import ModelFormMetaclass, modelform_factory
-from django.utils.translation import ugettext
-from django.utils.encoding import force_text, force_str
+from django.utils.translation import gettext
+from django.utils.encoding import force_str
 
 from chamber.shortcuts import get_object_or_none
 
 from pyston.exception import DataInvalidException, RestException
 from pyston.validators import ISODateTimeValidator
 from pyston.utils.compatibility import (
     get_reverse_field_name, get_model_from_relation, is_reverse_many_to_many, is_reverse_one_to_one,
@@ -185,32 +185,32 @@
 
     def _flat_object_to_pk(self, pk_field_name, data):
         if isinstance(data, dict):
             try:
                 return data[pk_field_name]
             except KeyError:
                 raise RestValidationError(
-                    ugettext('Data must contain primary key: {}').format(pk_field_name), code='invalid_structure'
+                    gettext('Data must contain primary key: {}').format(pk_field_name), code='invalid_structure'
                 )
         else:
             return data
 
     def _delete_related_object(self, resource, data, via):
         try:
             resource.delete_obj_with_pk(self._flat_object_to_pk(resource.pk_field_name, data), via)
         except DataInvalidException as ex:
             raise ex.errors
         except RestException as ex:
             raise RestValidationError(ex.message)
         except Http404:
-            raise RestValidationError(ugettext('Object does not exist'), code='invalid_structure')
+            raise RestValidationError(gettext('Object does not exist'), code='invalid_structure')
 
     def _create_or_update_related_object(self, resource, data, via, partial_update):
         if not isinstance(data, dict):
-            raise RestValidationError(ugettext('Data must be object'), code='invalid_structure')
+            raise RestValidationError(gettext('Data must be object'), code='invalid_structure')
 
         try:
             return resource.create_or_update(resource.update_data(data), via, partial_update)
         except DataInvalidException as ex:
             raise ex.errors
         except RestException as ex:
             raise RestValidationError(ex.errors)
@@ -233,15 +233,15 @@
 
     def _create_and_return_new_object_pk_list(self, resource, parent_inst, via, data, partial_update,
                                               created_via_field_name=None):
         errors = RestListError()
         result = []
         for i, obj_data in enumerate(data):
             if not isinstance(obj_data, dict):
-                obj_data = {resource.pk_field_name: force_text(obj_data)}
+                obj_data = {resource.pk_field_name: force_str(obj_data)}
 
             try:
                 if created_via_field_name:
                     obj_data = self._add_parent_inst_to_obj_data(parent_inst, created_via_field_name, obj_data)
 
                 if set(obj_data.keys()) ^ {resource.pk_field_name}:
                     result.append(self._create_or_update_related_object(resource, obj_data, via, partial_update).pk)
@@ -272,39 +272,39 @@
 
     def clean(self, data, request, parent_inst):
         if data is None:
             return data
 
         cleaned_data = copy.deepcopy(data)
         if not self._is_allowed_foreign_key and not isinstance(data, dict):
-            raise RestValidationError(ugettext('Invalid format'), code='invalid_structure')
+            raise RestValidationError(gettext('Invalid format'), code='invalid_structure')
 
         resource = self._get_resource(self._get_model(parent_inst), request)
         if not self._is_allowed_foreign_key and resource.pk_field_name in data:
             del cleaned_data[resource.pk_field_name]
         return cleaned_data
 
 
 class MultipleRelatedfieldValidationMixin(SingleRelatedfieldValidationMixin):
 
     def clean(self, data, request, parent_inst):
         if not isinstance(data, (tuple, list)):
-            raise RestValidationError(ugettext('Data must be a collection'), code='invalid_structure')
+            raise RestValidationError(gettext('Data must be a collection'), code='invalid_structure')
 
         errors = RestListError()
 
         cleaned_data = []
 
         for i, obj_data in enumerate(data):
             try:
                 cleaned_data.append(super().clean(obj_data, request, parent_inst))
                 if obj_data is None:
                     errors.append(
                         RestDictIndexError(
-                            i, {'error': RestValidationError(ugettext('Invalid format'), code='invalid_structure')}
+                            i, {'error': RestValidationError(gettext('Invalid format'), code='invalid_structure')}
                         )
                     )
             except RestError as ex:
                 errors.append(
                     RestDictIndexError(i, {'error': ex})
                 )
 
@@ -317,15 +317,15 @@
 
     def clean(self, data, request, parent_inst):
         if isinstance(data, dict):
             cleaned_data = {}
 
             if 'set' in data and {'remove', 'add'} & set(data.keys()):
                 raise RestValidationError(
-                    ugettext('set cannot be together with add or remove'), code='invalid_structure'
+                    gettext('set cannot be together with add or remove'), code='invalid_structure'
                 )
 
             errors = RestDictError()
             for k in ('add', 'remove', 'set'):
                 if k in data:
                     try:
                         cleaned_data[k] = super().clean(data[k], request, parent_inst)
@@ -359,22 +359,22 @@
         return self._update_related_objects(resource, parent_inst, via, data, partial_update, form)
 
 
 class MultipleStructuredRelatedField(MultipleStructuredRelatedfieldValidationMixin, MultipleRelatedField):
 
     def _remove_related_objects(self, resource, parent_inst, via, data, values):
         errors = RestListError()
-        result = [force_text(val) for val in values]
+        result = [force_str(val) for val in values]
         for i, obj in enumerate(data):
             try:
-                pk = force_text(self._flat_object_to_pk(resource.pk_field_name, obj))
+                pk = force_str(self._flat_object_to_pk(resource.pk_field_name, obj))
                 if pk in result:
                     result.remove(pk)
                 else:
-                    errors.append({'error': ugettext('Object does not exist in selected data'), '_index': i})
+                    errors.append({'error': gettext('Object does not exist in selected data'), '_index': i})
             except RestDictError as ex:
                 errors.append(RestDictIndexError(i, ex))
             except RestError as ex:
                 errors.append(RestDictIndexError(i, {'error': ex}))
 
         if errors:
             raise errors
@@ -445,15 +445,15 @@
     def _remove(self, resource, parent_inst, related_obj, field_name, via):
         self._delete_related_object(
             resource, {resource.pk_field_name: related_obj.pk}, via
         )
 
     def _create_or_update(self, resource, parent_inst, related_obj, field_name, via, data, partial_update):
         if not isinstance(data, dict):
-            obj_data = {resource.pk_field_name: force_text(data)}
+            obj_data = {resource.pk_field_name: force_str(data)}
         else:
             obj_data = data.copy()
 
         extra_data = self._get_extra_data(parent_inst)
         if extra_data:
             obj_data.update(extra_data)
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/forms/postgres.py` & `skip_django_pyston-2.17.0/pyston/forms/postgres.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.core.exceptions import ValidationError
 from django.contrib.postgres.utils import prefix_validation_error
 from django.contrib.postgres.forms.array import SimpleArrayField
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 
 class RestSimpleArrayField(SimpleArrayField):
     """
     Django array form field doesn't accept list. Therefore we must rewrite to_python method
     """
 
@@ -25,15 +25,15 @@
                         prefix=self.error_messages['item_invalid'],
                         code='item_invalid',
                         params={'nth': index},
                     ))
             if errors:
                 raise ValidationError(errors)
         else:
-            raise ValidationError(ugettext('Enter a list.'))
+            raise ValidationError(gettext('Enter a list.'))
         return values
 
     def clean(self, value):
         if value is None:
             return value
         else:
             return super().clean(value)
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/locale/cs/LC_MESSAGES/django.mo` & `skip_django_pyston-2.17.0/pyston/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/locale/cs/LC_MESSAGES/django.po` & `skip_django_pyston-2.17.0/pyston/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/metamodel.py` & `skip_django_pyston-2.17.0/pyston/metamodel.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/order/django_sorters.py` & `skip_django_pyston-2.17.0/pyston/order/django_sorters.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/order/managers.py` & `skip_django_pyston-2.17.0/pyston/order/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.utils.safestring import mark_safe
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from pyston.exception import RestException
 from pyston.utils import rfs, LOOKUP_SEP
 from pyston.utils.helpers import get_field_or_none, get_method_or_none
 from pyston.serializer import get_resource_or_none
 
 from .exceptions import OrderIdentifierError
@@ -180,15 +180,15 @@
         """
         sorters = []
         for ordering_term in parsed_order_terms:
             try:
                 sorters.append(self.get_sorter(ordering_term.identifiers, ordering_term.direction, resource, request))
             except OrderIdentifierError:
                 raise RestException(
-                    mark_safe(ugettext('Invalid identifier of ordering "{}"').format(ordering_term.source))
+                    mark_safe(gettext('Invalid identifier of ordering "{}"').format(ordering_term.source))
                 )
         return sorters
 
     def _convert_order_terms(self, sorters):
         """
         Converts sorters to the django query order strings.
         """
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/order/parsers.py` & `skip_django_pyston-2.17.0/pyston/order/parsers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/paginator.py` & `skip_django_pyston-2.17.0/pyston/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import reduce
 from operator import or_
 
 from chamber.shortcuts import get_object_or_none
 
 from django.db.models import Q
 from django.db.models.expressions import OrderBy
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from .forms import RestValidationError
 from .exception import RestException
 from .utils.compatibility import get_last_parent_pk_field_name
 from .utils.helpers import ModelIterableIteratorHelper
 from .response import HeadersResponse
 
@@ -47,32 +47,32 @@
         raise NotImplementedError
 
     def _get_offset(self, qs, request):
         offset = request._rest_context.get('offset', '0')
         if offset.isdigit():
             offset_int = int(offset)
             if offset_int > self.max_offset:
-                raise RestException(ugettext('Offset must be lower or equal to {}').format(self.max_offset))
+                raise RestException(gettext('Offset must be lower or equal to {}').format(self.max_offset))
             else:
                 return offset_int
         else:
-            raise RestException(ugettext('Offset must be natural number'))
+            raise RestException(gettext('Offset must be natural number'))
 
     def _get_base(self, qs, request):
         base = request._rest_context.get('base')
         if not base:
             return self.default_base
         elif base.isdigit():
             base_int = int(base)
             if base_int > self.max_base:
-                raise RestException(ugettext('Base must lower or equal to {}').format(self.max_base))
+                raise RestException(gettext('Base must lower or equal to {}').format(self.max_base))
             else:
                 return base_int
         else:
-            raise RestException(ugettext('Base must be natural number or empty'))
+            raise RestException(gettext('Base must be natural number or empty'))
 
     def _get_next_offset(self, iterable, offset, base):
         return offset + base if len(iterable) > base else None
 
     def _get_prev_offset(self, iterable, offset, base):
         return None if offset == 0 or not base else max(offset - base, 0)
 
@@ -197,29 +197,29 @@
         qs = qs.order_by(*ordering)
 
         if cursor:
             current_row = get_object_or_none(qs, pk=cursor)
             if current_row:
                 qs = qs.filter(self._get_page_filter_kwargs(current_row))
             else:
-                raise RestException(RestValidationError(ugettext('Cursor object was not found')))
+                raise RestException(RestValidationError(gettext('Cursor object was not found')))
         return self._get_page(qs, base)
 
     def _get_base(self, request):
         base = request._rest_context.get('base')
         if not base:
             return self.default_base
         elif base.isdigit():
             base_int = int(base)
             if base_int > self.max_base:
-                raise RestException(ugettext('Base must lower or equal to {}').format(self.max_base))
+                raise RestException(gettext('Base must lower or equal to {}').format(self.max_base))
             else:
                 return base_int
         else:
-            raise RestException(ugettext('Base must be natural number or empty'))
+            raise RestException(gettext('Base must be natural number or empty'))
 
     def _get_cursor(self, request):
         return request._rest_context.get('cursor')
 
     def _get_ordering(self, request, qs):
         pk_field_name = get_last_parent_pk_field_name(qs.model)
         query_ordering = list(qs.query.order_by) or list(qs.model._meta.ordering)
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/patch.py` & `skip_django_pyston-2.17.0/pyston/patch.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/requested_fields/managers.py` & `skip_django_pyston-2.17.0/pyston/requested_fields/managers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/requested_fields/parser.py` & `skip_django_pyston-2.17.0/pyston/requested_fields/parser.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/resource.py` & `skip_django_pyston-2.17.0/pyston/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from collections import OrderedDict
 
 from django.conf import settings as django_settings
 from django.core.exceptions import ValidationError
 from django.http.response import HttpResponse, HttpResponseBase
 from django.utils.decorators import classonlymethod
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.db.models.fields import DateTimeField
 from django.http.response import Http404
 from django.core.exceptions import ObjectDoesNotExist
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.utils.module_loading import import_string
 
 from functools import update_wrapper
 
 from chamber.shortcuts import get_object_or_none
 from chamber.utils import remove_accent, transaction
 
@@ -384,15 +384,15 @@
         if rm in {'PUT', 'PATCH'}:
             coerce_rest_request_method(self.request)
 
         if rm in {'POST', 'PUT', 'PATCH'}:
             try:
                 converter = get_converter_from_request(self.request, self.converters, True)
                 self.request.data = self.serializer(self).deserialize(
-                    converter.decode(force_text(self.request.body), resource=self)
+                    converter.decode(force_str(self.request.body), resource=self)
                 )
             except (TypeError, ValueError):
                 raise MimerDataException
             except NotImplementedError:
                 raise UnsupportedMediaTypeException
         return self.request
 
@@ -1048,15 +1048,15 @@
     def _get_exclude(self, obj=None):
         return []
 
     def _get_form_class(self, inst):
         return self.form_class
 
     def _get_name(self):
-        return force_text(remove_accent(force_text(self.model._meta.verbose_name_plural)))
+        return force_str(remove_accent(force_str(self.model._meta.verbose_name_plural)))
 
     def formfield_for_dbfield(self, db_field, **kwargs):
         if isinstance(db_field, DateTimeField):
             kwargs.update({'form_class': ISODateTimeField})
         return db_field.formfield(**kwargs)
 
     def _get_instance(self, data):
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/response.py` & `skip_django_pyston-2.17.0/pyston/response.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/serializer.py` & `skip_django_pyston-2.17.0/pyston/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import enum
 from collections import OrderedDict
 
 from django.db.models import Model
 from django.db.models.fields.files import FieldFile
 from django.db.models.query import QuerySet
 from django.utils import formats, timezone
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.html import conditional_escape
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from chamber.utils import get_class_method
 
 from .conf import settings
 from .converters import get_converter
 from .exception import NotAllowedException, UnsupportedMediaTypeException
 from .forms import RestDictError, RestDictIndexError, RestListError
@@ -543,22 +543,22 @@
             return None
 
 
 @register(str)
 class StringSerializer(Serializer):
 
     def serialize(self, data, serialization_format, allow_tags=False, **kwargs):
-        serialized_string = force_text(data, strings_only=True)
+        serialized_string = force_str(data, strings_only=True)
         return serialized_string if allow_tags or settings.ALLOW_TAGS else conditional_escape(serialized_string)
 
 
 class DefaultSerializer(Serializer):
 
     def serialize(self, data, serialization_format, **kwargs):
-        return force_text(data, strings_only=True)
+        return force_str(data, strings_only=True)
 
 
 class BaseRawVerboseValueSerializer(Serializer):
 
     def _get_verbose_value(self, data, **kwargs):
         raise NotImplementedError
 
@@ -604,15 +604,15 @@
         return timezone.localtime(data) if timezone.is_aware(data) else data
 
 
 @register(bool)
 class BoolSerializer(BaseRawVerboseValueSerializer):
 
     def _get_verbose_value(self, data, **kwargs):
-        return ugettext('Yes') if data else ugettext('No')
+        return gettext('Yes') if data else gettext('No')
 
 
 @register(dict)
 class DictSerializer(Serializer):
 
     def serialize(self, data, serialization_format, requested_fieldset=None,
                   extended_fieldset=None, exclude_fields=None, **kwargs):
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/templates/default_pdf_table.html` & `skip_django_pyston-2.17.0/pyston/templates/default_pdf_table.html`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/templates/pyston/html_converter.html` & `skip_django_pyston-2.17.0/pyston/templates/pyston/html_converter.html`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/utils/__init__.py` & `skip_django_pyston-2.17.0/pyston/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from enum import Enum
 
 from collections import OrderedDict
 
 from django.template.defaultfilters import lower
 from django.db import models
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from copy import deepcopy
 
 
 LOOKUP_SEP = '__'
 
 
@@ -142,15 +142,15 @@
     def intersection(self, rest_field):
         self.subfieldset = self.subfieldset.intersection(rest_field.subfieldset)
         return self
 
     def __str__(self):
         if self.subfieldset:
             return '{}({})'.format(self.name, self.subfieldset)
-        return force_text(self.name)
+        return force_str(self.name)
 
 
 class RestFieldset:
 
     @classmethod
     def create_from_string(cls, fields_string):
         fields = []
@@ -253,15 +253,15 @@
 
         return self
 
     def __deepcopy__(self, memo):
         return self.__class__(*map(deepcopy, self.fields))
 
     def __str__(self):
-        return ','.join(map(force_text, self.fields))
+        return ','.join(map(force_str, self.fields))
 
     def __add__(self, rest_fieldset):
         a_rfs = deepcopy(self)
         return a_rfs.join(rest_fieldset)
 
     def __bool__(self):
         return bool(self.fields_map)
```

### Comparing `skip-django-pyston-2.16.5.4/pyston/utils/compatibility.py` & `skip_django_pyston-2.17.0/pyston/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/utils/datastructures.py` & `skip_django_pyston-2.17.0/pyston/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/utils/decorators.py` & `skip_django_pyston-2.17.0/pyston/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/utils/files.py` & `skip_django_pyston-2.17.0/pyston/utils/files.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/pyston/utils/helpers.py` & `skip_django_pyston-2.17.0/pyston/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.4/setup.py` & `skip_django_pyston-2.17.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Internet :: WWW/HTTP',
     ],
     install_requires=[
-        'django>=2.2, <4.0',
+        'django>=4.2',
         'defusedxml>=0.6.0',
         'pyparsing==2.4.7',
         'python-mimeparse>=1.6.0',
-        'skip-django-chamber>=0.6.17.2',
+        'skip-django-chamber>=0.7.2',
         'python-magic>=0.4.27',
     ],
     zip_safe=False
 )
```

### Comparing `skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/PKG-INFO` & `skip_django_pyston-2.17.0/skip_django_pyston.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: skip-django-pyston
-Version: 2.16.5.4
+Version: 2.17.0
 Summary: Pyston is a Django mini-framework creating APIs.
 Home-page: https://github.com/skip-pay/django-pyston
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 License-File: AUTHORS.txt
-Requires-Dist: django<4.0,>=2.2
+Requires-Dist: django>=4.2
 Requires-Dist: defusedxml>=0.6.0
 Requires-Dist: pyparsing==2.4.7
 Requires-Dist: python-mimeparse>=1.6.0
-Requires-Dist: skip-django-chamber>=0.6.17.2
+Requires-Dist: skip-django-chamber>=0.7.2
 Requires-Dist: python-magic>=0.4.27
```

### Comparing `skip-django-pyston-2.16.5.4/skip_django_pyston.egg-info/SOURCES.txt` & `skip_django_pyston-2.17.0/skip_django_pyston.egg-info/SOURCES.txt`

 * *Files identical despite different names*

