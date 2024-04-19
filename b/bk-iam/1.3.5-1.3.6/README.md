# Comparing `tmp/bk-iam-1.3.5.tar.gz` & `tmp/bk-iam-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bk-iam-1.3.5.tar", last modified: Thu Nov  9 03:18:16 2023, max compression
+gzip compressed data, was "dist/bk-iam-1.3.6.tar", last modified: Fri Apr 19 06:59:16 2024, max compression
```

## Comparing `bk-iam-1.3.5.tar` & `bk-iam-1.3.6.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/
--rw-r--r--   0 root         (0) root         (0)       47 2023-11-09 03:15:57.000000 bk-iam-1.3.5/iam/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/api/
--rw-r--r--   0 root         (0) root         (0)    16124 2023-03-07 08:22:34.000000 bk-iam-1.3.5/iam/api/client.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5536 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/api/http.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/meta.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/objects.py
--rw-r--r--   0 root         (0) root         (0)    10156 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/dummy_iam.py
--rw-r--r--   0 root         (0) root         (0)    23130 2023-03-07 08:59:27.000000 bk-iam-1.3.5/iam/iam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/apply/
--rw-r--r--   0 root         (0) root         (0)     7594 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/apply/models.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/apply/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5232 2023-11-09 03:15:57.000000 bk-iam-1.3.5/iam/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/eval/
--rw-r--r--   0 root         (0) root         (0)     1803 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/eval/constants.py
--rw-r--r--   0 root         (0) root         (0)     2079 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/eval/object.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/eval/expression.py
--rw-r--r--   0 root         (0) root         (0)    11845 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/eval/operators.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/eval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/model/
--rw-r--r--   0 root         (0) root         (0)     3470 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/model/models.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/collection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/iam_migration/
--rw-r--r--   0 root         (0) root         (0)      951 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/apps.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/iam_migration/templates/
--rw-r--r--   0 root         (0) root         (0)      570 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/templates/migration.tmpl
--rw-r--r--   0 root         (0) root         (0)      845 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1343 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/iam_migration/utils/
--rw-r--r--   0 root         (0) root         (0)    25878 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/utils/do_migrate.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2805 2023-07-01 07:56:46.000000 bk-iam-1.3.5/iam/contrib/iam_migration/migrator.py
--rw-r--r--   0 root         (0) root         (0)      818 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/iam_migration/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/iam_migration/management/commands/
--rw-r--r--   0 root         (0) root         (0)     3756 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/management/commands/iam_makemigrations.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/iam_migration/migrations/
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/iam_migration/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/django/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/django/dispatcher/
--rw-r--r--   0 root         (0) root         (0)      923 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/django/dispatcher/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9990 2023-11-09 03:15:57.000000 bk-iam-1.3.5/iam/contrib/django/dispatcher/dispatchers.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/django/dispatcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/django/middlewares.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/django/response.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/django/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/converter/
--rw-r--r--   0 root         (0) root         (0)     2226 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/converter/base.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/converter/queryset.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/converter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5814 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/converter/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/contrib/tastypie/
--rw-r--r--   0 root         (0) root         (0)     4177 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/tastypie/resource.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/tastypie/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8012 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/tastypie/authorization.py
--rw-r--r--   0 root         (0) root         (0)     2090 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/tastypie/shortcuts.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/contrib/http.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/resource/
--rw-r--r--   0 root         (0) root         (0)     3430 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/resource/provider.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/resource/constants.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/resource/dispatcher.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/resource/utils.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/resource/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1179 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/shortcuts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/iam/auth/
--rw-r--r--   0 root         (0) root         (0)    14884 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/auth/models.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-03-07 02:07:52.000000 bk-iam-1.3.5/iam/cache.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-09 03:18:16.000000 bk-iam-1.3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      194 2023-03-07 02:07:52.000000 bk-iam-1.3.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     3109 2023-11-09 03:15:57.000000 bk-iam-1.3.5/readme_en.md
--rw-r--r--   0 root         (0) root         (0)      220 2023-03-07 02:07:52.000000 bk-iam-1.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      758 2023-11-09 03:18:16.000000 bk-iam-1.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1249 2023-07-01 07:56:46.000000 bk-iam-1.3.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 03:18:16.000000 bk-iam-1.3.5/bk_iam.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1948 2023-11-09 03:18:15.000000 bk-iam-1.3.5/bk_iam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-09 03:18:15.000000 bk-iam-1.3.5/bk_iam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-11-09 03:18:15.000000 bk-iam-1.3.5/bk_iam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-11-09 03:18:15.000000 bk-iam-1.3.5/bk_iam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      758 2023-11-09 03:18:15.000000 bk-iam-1.3.5/bk_iam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3752 2023-11-09 03:15:57.000000 bk-iam-1.3.5/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-19 06:54:19.000000 bk-iam-1.3.6/iam/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/api/
+-rw-r--r--   0 root         (0) root         (0)    16124 2023-03-07 08:22:34.000000 bk-iam-1.3.6/iam/api/client.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/api/http.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/meta.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/objects.py
+-rw-r--r--   0 root         (0) root         (0)    10156 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/dummy_iam.py
+-rw-r--r--   0 root         (0) root         (0)    23130 2023-03-07 08:59:27.000000 bk-iam-1.3.6/iam/iam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/apply/
+-rw-r--r--   0 root         (0) root         (0)     7594 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/apply/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/apply/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5878 2024-04-19 06:54:19.000000 bk-iam-1.3.6/iam/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/eval/
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/eval/constants.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/eval/object.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/eval/expression.py
+-rw-r--r--   0 root         (0) root         (0)    11845 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/eval/operators.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/eval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/model/
+-rw-r--r--   0 root         (0) root         (0)     3470 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/model/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/collection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/iam_migration/
+-rw-r--r--   0 root         (0) root         (0)      951 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/apps.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/iam_migration/templates/
+-rw-r--r--   0 root         (0) root         (0)      570 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/templates/migration.tmpl
+-rw-r--r--   0 root         (0) root         (0)      845 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/iam_migration/utils/
+-rw-r--r--   0 root         (0) root         (0)    25878 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/utils/do_migrate.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-07-01 07:56:46.000000 bk-iam-1.3.6/iam/contrib/iam_migration/migrator.py
+-rw-r--r--   0 root         (0) root         (0)      818 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/iam_migration/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/iam_migration/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     3756 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/management/commands/iam_makemigrations.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/iam_migration/migrations/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/iam_migration/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/django/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/django/dispatcher/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/django/dispatcher/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9990 2023-11-09 03:15:57.000000 bk-iam-1.3.6/iam/contrib/django/dispatcher/dispatchers.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/django/dispatcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/django/middlewares.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/django/response.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/django/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/converter/
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/converter/base.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/converter/queryset.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/converter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5814 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/converter/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/contrib/tastypie/
+-rw-r--r--   0 root         (0) root         (0)     4177 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/tastypie/resource.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/tastypie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/tastypie/authorization.py
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/tastypie/shortcuts.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/contrib/http.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/resource/
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/resource/provider.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/resource/constants.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/resource/dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/resource/utils.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/resource/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/shortcuts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/iam/auth/
+-rw-r--r--   0 root         (0) root         (0)    14884 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/auth/models.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-03-07 02:07:52.000000 bk-iam-1.3.6/iam/cache.py
+-rw-r--r--   0 root         (0) root         (0)       59 2024-04-19 06:59:16.000000 bk-iam-1.3.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      194 2023-03-07 02:07:52.000000 bk-iam-1.3.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     3109 2024-04-19 06:54:19.000000 bk-iam-1.3.6/readme_en.md
+-rw-r--r--   0 root         (0) root         (0)      220 2023-03-07 02:07:52.000000 bk-iam-1.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      565 2024-04-19 06:59:16.000000 bk-iam-1.3.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-07-01 07:56:46.000000 bk-iam-1.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:59:16.000000 bk-iam-1.3.6/bk_iam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1948 2024-04-19 06:59:16.000000 bk-iam-1.3.6/bk_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 06:59:16.000000 bk-iam-1.3.6/bk_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-19 06:59:16.000000 bk-iam-1.3.6/bk_iam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-19 06:59:16.000000 bk-iam-1.3.6/bk_iam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      565 2024-04-19 06:59:16.000000 bk-iam-1.3.6/bk_iam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3752 2024-04-19 06:54:19.000000 bk-iam-1.3.6/readme.md
```

### Comparing `bk-iam-1.3.5/iam/api/client.py` & `bk-iam-1.3.6/iam/api/client.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/api/__init__.py` & `bk-iam-1.3.6/iam/api/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/api/http.py` & `bk-iam-1.3.6/iam/api/http.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/meta.py` & `bk-iam-1.3.6/iam/meta.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/exceptions.py` & `bk-iam-1.3.6/iam/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/objects.py` & `bk-iam-1.3.6/iam/objects.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/dummy_iam.py` & `bk-iam-1.3.6/iam/dummy_iam.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/iam.py` & `bk-iam-1.3.6/iam/iam.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/apply/models.py` & `bk-iam-1.3.6/iam/apply/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/apply/__init__.py` & `bk-iam-1.3.6/iam/apply/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/utils.py` & `bk-iam-1.3.6/iam/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 Copyright (C) 2017-2021 THL A29 Limited, a Tencent company. All rights reserved.
 Licensed under the MIT License (the "License"); you may not use this file except in compliance with the License.
 You may obtain a copy of the License at http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
-
-
-from collections import OrderedDict
+import itertools
+from collections import OrderedDict, defaultdict
 
 from . import meta
 
 
 # flake8: noqa: C901
 def gen_perms_apply_data(system, subject, action_to_resources_list):
     """
@@ -57,72 +56,80 @@
             for resource in resources:
                 system_resources.setdefault(resource.system, []).append(resource)
 
             # 2. append to system_resources_list e.g.g {"system1": [[r1, r2]], "system2": [[r3]]}
             for system_id, resources in system_resources.items():
                 system_resources_list.setdefault(system_id, []).append(resources)
 
+        # 2. aggregate resources by resource type, generate related_resource_type
         related_resource_types = []
         for system_id, resources_list in system_resources_list.items():
-            # get resource type from last resource in resources
-            a_resource = resources_list[0][-1]
-            resource_types = {
-                "system_id": system_id,
-                "system_name": meta.get_system_name(system_id),
-                "type": a_resource.type,
-                "type_name": meta.get_resource_name(system_id, a_resource.type),
-            }
-            instances = []
+            if not resources_list:
+                continue
 
-            for resources in resources_list:
+            # aggregate resources by resource type
+            resource_type__resources = defaultdict(list)
+            for resource in list(itertools.chain(*resources_list)):
+                resource_type__resources[resource.type].append(resource)
+
+            # get the list of resource instances of the same type
+            for __, resources in resource_type__resources.items():
+                a_resource = resources[0]
+                resource_types = {
+                    "system_id": system_id,
+                    "system_name": meta.get_system_name(system_id),
+                    "type": a_resource.type,
+                    "type_name": meta.get_resource_name(system_id, a_resource.type),
+                }
+                instances = []
+
+                # arrange instances according to topo level
                 for resource in resources:
                     inst_item = []
-                    topo_path = None
-
-                    if resource.attribute:
-                        topo_path = resource.attribute.get("_bk_iam_path_")
-
-                    if topo_path:
-                        for part in topo_path[1:-1].split("/"):
-                            # NOTE: old _bk_iam_path_ is like /set,1/host,2/
-                            # while the new _bk_iam_path_ is like /bk_cmdb,set,1/bk_cmdb,host,2/
-                            node_parts = part.split(",")
-                            # NOTE: topo resources should be considered to belong to different systems
-                            rsystem, rtype, rid = system_id, "", ""
-                            if len(node_parts) == 2:
-                                rtype, rid = node_parts[0], node_parts[1]
-                            elif len(node_parts) == 3:
-                                rsystem, rtype, rid = node_parts[0], node_parts[1], node_parts[2]
-                                # NOTE: currently, keep the name of /bk_cmdb,set,1/ same as /set,1/
-                                part = ",".join(node_parts[1:])
-                            else:
-                                raise Exception("Invalid _bk_iam_path_: %s" % topo_path)
-
-                            inst_item.append(
-                                {
-                                    "type": rtype,
-                                    "type_name": meta.get_resource_name(rsystem, rtype),
-                                    "id": rid,
-                                    "name": part,
-                                }
-                            )
-
+                    topo_path = []
+                    # get the topo level of the resource
+                    if resource.attribute and resource.attribute.get("_bk_iam_path_"):
+                        bk_iam_path = resource.attribute["_bk_iam_path_"]
+                        topo_path = bk_iam_path[1:-1].split("/")
+                    # append paernt topo instance
+                    for part in topo_path:
+                        # NOTE: old _bk_iam_path_ is like /set,1/host,2/
+                        # while the new _bk_iam_path_ is like /bk_cmdb,set,1/bk_cmdb,host,2/
+                        node_parts = part.split(",")
+                        # NOTE: topo resources should be considered to belong to different systems
+                        rsystem, rtype, rid = system_id, "", ""
+                        if len(node_parts) == 2:
+                            rtype, rid = node_parts[0], node_parts[1]
+                        elif len(node_parts) == 3:
+                            rsystem, rtype, rid = node_parts[0], node_parts[1], node_parts[2]
+                            # NOTE: currently, keep the name of /bk_cmdb,set,1/ same as /set,1/
+                            part = ",".join(node_parts[1:])
+                        else:
+                            raise Exception("Invalid _bk_iam_path_: %s" % topo_path)
+                        inst_item.append(
+                            {
+                                "type": rtype,
+                                "type_name": meta.get_resource_name(rsystem, rtype),
+                                "id": rid,
+                                "name": part,
+                            }
+                        )
+                    # lastly, append self
                     inst_item.append(
                         {
                             "type": resource.type,
                             "type_name": meta.get_resource_name(system_id, resource.type),
                             "id": resource.id,
                             "name": resource.attribute.get("name", "") if resource.attribute else "",
                         }
                     )
-
                     instances.append(inst_item)
 
-            resource_types["instances"] = instances
-            related_resource_types.append(resource_types)
+                resource_types["instances"] = instances
+                related_resource_types.append(resource_types)
 
         action["related_resource_types"] = related_resource_types
         actions.append(action)
 
     data["actions"] = actions
 
     return data
```

### Comparing `bk-iam-1.3.5/iam/eval/constants.py` & `bk-iam-1.3.6/iam/eval/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/eval/object.py` & `bk-iam-1.3.6/iam/eval/object.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/eval/expression.py` & `bk-iam-1.3.6/iam/eval/expression.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/eval/operators.py` & `bk-iam-1.3.6/iam/eval/operators.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/eval/__init__.py` & `bk-iam-1.3.6/iam/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/model/models.py` & `bk-iam-1.3.6/iam/model/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/model/__init__.py` & `bk-iam-1.3.6/iam/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/collection.py` & `bk-iam-1.3.6/iam/collection.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/apps.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/apps.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/constants.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/templates/migration.tmpl` & `bk-iam-1.3.6/iam/contrib/iam_migration/templates/migration.tmpl`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/exceptions.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/template.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/template.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/utils/do_migrate.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/utils/do_migrate.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/utils/__init__.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/migrator.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/migrator.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/__init__.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/management/commands/iam_makemigrations.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/management/commands/iam_makemigrations.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/management/commands/__init__.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/management/__init__.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/migrations/__init__.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/iam_migration/conf.py` & `bk-iam-1.3.6/iam/contrib/iam_migration/conf.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/django/dispatcher/exceptions.py` & `bk-iam-1.3.6/iam/contrib/django/dispatcher/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/django/dispatcher/dispatchers.py` & `bk-iam-1.3.6/iam/contrib/django/dispatcher/dispatchers.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/django/dispatcher/__init__.py` & `bk-iam-1.3.6/iam/contrib/django/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/django/middlewares.py` & `bk-iam-1.3.6/iam/contrib/django/middlewares.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/django/response.py` & `bk-iam-1.3.6/iam/contrib/django/response.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/django/__init__.py` & `bk-iam-1.3.6/iam/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/converter/base.py` & `bk-iam-1.3.6/iam/contrib/converter/base.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/converter/queryset.py` & `bk-iam-1.3.6/iam/contrib/converter/queryset.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/converter/__init__.py` & `bk-iam-1.3.6/iam/contrib/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/converter/sql.py` & `bk-iam-1.3.6/iam/contrib/converter/sql.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/tastypie/resource.py` & `bk-iam-1.3.6/iam/contrib/tastypie/resource.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/tastypie/__init__.py` & `bk-iam-1.3.6/iam/contrib/tastypie/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/tastypie/authorization.py` & `bk-iam-1.3.6/iam/contrib/tastypie/authorization.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/tastypie/shortcuts.py` & `bk-iam-1.3.6/iam/contrib/tastypie/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/__init__.py` & `bk-iam-1.3.6/iam/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/contrib/http.py` & `bk-iam-1.3.6/iam/contrib/http.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/__init__.py` & `bk-iam-1.3.6/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/resource/provider.py` & `bk-iam-1.3.6/iam/resource/provider.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/resource/constants.py` & `bk-iam-1.3.6/iam/resource/constants.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/resource/dispatcher.py` & `bk-iam-1.3.6/iam/resource/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/resource/utils.py` & `bk-iam-1.3.6/iam/resource/utils.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/resource/__init__.py` & `bk-iam-1.3.6/iam/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/shortcuts.py` & `bk-iam-1.3.6/iam/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/auth/models.py` & `bk-iam-1.3.6/iam/auth/models.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/auth/__init__.py` & `bk-iam-1.3.6/iam/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/iam/cache.py` & `bk-iam-1.3.6/iam/cache.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/readme_en.md` & `bk-iam-1.3.6/readme_en.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![](docs/resource/img/bk_iam_en.png)
 ---
 
-[![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/iam-python-sdk/blob/master/LICENSE.txt) [![Release Version](https://img.shields.io/badge/release-1.3.5-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/pulls) [![BK Pipelines Status](https://api.bkdevops.qq.com/process/api/external/pipelines/projects/iam/p-5c359e750bb9457984ab84656651d843/badge?X-DEVOPS-PROJECT-ID=iam)](http://devops.oa.com/process/api-html/user/builds/projects/iam/pipelines/p-5c359e750bb9457984ab84656651d843/latestFinished?X-DEVOPS-PROJECT-ID=iam)
+[![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/iam-python-sdk/blob/master/LICENSE.txt) [![Release Version](https://img.shields.io/badge/release-1.3.6-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/pulls) [![BK Pipelines Status](https://api.bkdevops.qq.com/process/api/external/pipelines/projects/iam/p-5c359e750bb9457984ab84656651d843/badge?X-DEVOPS-PROJECT-ID=iam)](http://devops.oa.com/process/api-html/user/builds/projects/iam/pipelines/p-5c359e750bb9457984ab84656651d843/latestFinished?X-DEVOPS-PROJECT-ID=iam)
 
 ## Overview
 
 iam-python-sdk is the SDK of blueking IAM(BK-IAM), your system can use BK-IAM easily via SDK.
 
 ## Features
```

### Comparing `bk-iam-1.3.5/setup.py` & `bk-iam-1.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/bk_iam.egg-info/SOURCES.txt` & `bk-iam-1.3.6/bk_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bk-iam-1.3.5/readme.md` & `bk-iam-1.3.6/readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![](docs/resource/img/bk_iam_zh.png)
 ---
 
-[![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/iam-python-sdk/blob/master/LICENSE.txt) [![Release Version](https://img.shields.io/badge/release-1.3.5-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/pulls) [![BK Pipelines Status](https://api.bkdevops.qq.com/process/api/external/pipelines/projects/iam/p-5c359e750bb9457984ab84656651d843/badge?X-DEVOPS-PROJECT-ID=iam)](http://devops.oa.com/process/api-html/user/builds/projects/iam/pipelines/p-5c359e750bb9457984ab84656651d843/latestFinished?X-DEVOPS-PROJECT-ID=iam)
+[![license](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://github.com/TencentBlueKing/iam-python-sdk/blob/master/LICENSE.txt) [![Release Version](https://img.shields.io/badge/release-1.3.6-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/releases) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/iam-python-sdk/pulls) [![BK Pipelines Status](https://api.bkdevops.qq.com/process/api/external/pipelines/projects/iam/p-5c359e750bb9457984ab84656651d843/badge?X-DEVOPS-PROJECT-ID=iam)](http://devops.oa.com/process/api-html/user/builds/projects/iam/pipelines/p-5c359e750bb9457984ab84656651d843/latestFinished?X-DEVOPS-PROJECT-ID=iam)
 
 [(English Documents Available)](readme_en.md)
 
 ## Overview
 
 iam-python-sdk 是蓝鲸权限中心(BK-IAM)提供的用于快速接入权限体系的python SDK
```

