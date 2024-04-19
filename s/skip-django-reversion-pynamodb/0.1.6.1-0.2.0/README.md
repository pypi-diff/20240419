# Comparing `tmp/skip-django-reversion-pynamodb-0.1.6.1.tar.gz` & `tmp/skip_django_reversion_pynamodb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-reversion-pynamodb-0.1.6.1.tar", last modified: Mon Jan 30 01:53:16 2023, max compression
+gzip compressed data, was "skip_django_reversion_pynamodb-0.2.0.tar", last modified: Fri Apr 19 09:59:54 2024, max compression
```

## Comparing `skip-django-reversion-pynamodb-0.1.6.1.tar` & `skip_django_reversion_pynamodb-0.2.0.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.602005 skip-django-reversion-pynamodb-0.1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    25013 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-01-30 01:53:16.602005 skip-django-reversion-pynamodb-0.1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.590005 skip-django-reversion-pynamodb-0.1.6.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.590005 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/admin.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/create-revision-args.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/create-revision-atomic.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/create-revision-manage-manually.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/create-revision-using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/model-db-arg.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/post-register.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/signal-args.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/throws-registration-error.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/throws-revert-error.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/_include/throws-revision-error.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/admin.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18013 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/backends.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/common-problems.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/middleware.rst
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/signals.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/docs/views.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.590005 skip-django-reversion-pynamodb-0.1.6.1/reversion/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.590005 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.590005 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.590005 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.590005 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/management/commands/initdynamodbreversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/queryset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/management/commands/createinitialrevisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/management/commands/deleterevisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/migrations/0001_squashed_0004_auto_20160611_1202.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14979 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.586005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.594005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.582005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.586005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.586005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.586005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sl_SI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sl_SI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sl_SI/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sl_SI/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.586005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.586005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.586005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.586005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/revisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/reversion/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.586005 skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/reversion/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/reversion/change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/reversion/object_history.html
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/reversion/recover_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/reversion/recover_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/reversion/revision_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/reversion/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-30 01:53:16.602005 skip-django-reversion-pynamodb-0.1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/skip_django_reversion_pynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-01-30 01:53:16.000000 skip-django-reversion-pynamodb-0.1.6.1/skip_django_reversion_pynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-01-30 01:53:16.000000 skip-django-reversion-pynamodb-0.1.6.1/skip_django_reversion_pynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 01:53:16.000000 skip-django-reversion-pynamodb-0.1.6.1/skip_django_reversion_pynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 01:53:16.000000 skip-django-reversion-pynamodb-0.1.6.1/skip_django_reversion_pynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-30 01:53:16.000000 skip-django-reversion-pynamodb-0.1.6.1/skip_django_reversion_pynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-30 01:53:16.000000 skip-django-reversion-pynamodb-0.1.6.1/skip_django_reversion_pynamodb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.598005 skip-django-reversion-pynamodb-0.1.6.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.602005 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.602005 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.602005 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:16.602005 skip-django-reversion-pynamodb-0.1.6.1/tests/test_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_project/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_project/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-30 01:53:07.000000 skip-django-reversion-pynamodb-0.1.6.1/tests/test_project/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.522347 skip_django_reversion_pynamodb-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    25013 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-19 09:59:54.522347 skip_django_reversion_pynamodb-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.502347 skip_django_reversion_pynamodb-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.506347 skip_django_reversion_pynamodb-0.2.0/docs/_include/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/create-revision-args.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/create-revision-atomic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/create-revision-manage-manually.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/create-revision-using.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/model-db-arg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/post-register.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/signal-args.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/throws-registration-error.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/throws-revert-error.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/_include/throws-revision-error.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18013 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/common-problems.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/middleware.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/docs/views.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.506347 skip_django_reversion_pynamodb-0.2.0/reversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.506347 skip_django_reversion_pynamodb-0.2.0/reversion/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.506347 skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.506347 skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.506347 skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/management/commands/initdynamodbreversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/queryset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.506347 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.506347 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/management/commands/createinitialrevisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/management/commands/deleterevisions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/migrations/0001_squashed_0004_auto_20160611_1202.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/backends/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.494347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.494347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.510347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sl_SI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sl_SI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sl_SI/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sl_SI/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/revisions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.498347 skip_django_reversion_pynamodb-0.2.0/reversion/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.514347 skip_django_reversion_pynamodb-0.2.0/reversion/templates/reversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/templates/reversion/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/templates/reversion/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/templates/reversion/recover_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/templates/reversion/recover_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/templates/reversion/revision_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/reversion/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 09:59:54.522347 skip_django_reversion_pynamodb-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.522347 skip_django_reversion_pynamodb-0.2.0/skip_django_reversion_pynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-19 09:59:54.000000 skip_django_reversion_pynamodb-0.2.0/skip_django_reversion_pynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-19 09:59:54.000000 skip_django_reversion_pynamodb-0.2.0/skip_django_reversion_pynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:59:54.000000 skip_django_reversion_pynamodb-0.2.0/skip_django_reversion_pynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:59:54.000000 skip_django_reversion_pynamodb-0.2.0/skip_django_reversion_pynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 09:59:54.000000 skip_django_reversion_pynamodb-0.2.0/skip_django_reversion_pynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 09:59:54.000000 skip_django_reversion_pynamodb-0.2.0/skip_django_reversion_pynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.518347 skip_django_reversion_pynamodb-0.2.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.518347 skip_django_reversion_pynamodb-0.2.0/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.518347 skip_django_reversion_pynamodb-0.2.0/tests/test_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.518347 skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23503 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:54.518347 skip_django_reversion_pynamodb-0.2.0/tests/test_project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-19 09:59:47.000000 skip_django_reversion_pynamodb-0.2.0/tests/test_project/wsgi.py
```

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/CHANGELOG.rst` & `skip_django_reversion_pynamodb-0.2.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/LICENSE` & `skip_django_reversion_pynamodb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/PKG-INFO` & `skip_django_reversion_pynamodb-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-reversion-pynamodb
-Version: 0.1.6.1
+Version: 0.2.0
 Summary: An extension to the Django web framework that provides version control for model instances.
 Home-page: http://github.com/skip-pay/django-reversion-pynamodb
 Author: Dave Hall,Lubos Matl
 Author-email: dave@etianen.com, matllubos@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -12,17 +12,21 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
-Requires-Python: >=3.6
-Provides-Extra: dynamodb
+Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: django>=4.2
+Requires-Dist: import_string>=0.1.0
+Provides-Extra: dynamodb
+Requires-Dist: skip-pydjamodb>=0.1.0; extra == "dynamodb"
+Requires-Dist: pynamodb==5.3.4; extra == "dynamodb"
 
 =========================
 django-reversion-pynamodb
 =========================
 
 |PyPI latest| |PyPI Version| |PyPI License| |TravisCI| |Docs|
```

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/README.rst` & `skip_django_reversion_pynamodb-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/docs/admin.rst` & `skip_django_reversion_pynamodb-0.2.0/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/docs/api.rst` & `skip_django_reversion_pynamodb-0.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/docs/backends.rst` & `skip_django_reversion_pynamodb-0.2.0/docs/backends.rst`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/docs/commands.rst` & `skip_django_reversion_pynamodb-0.2.0/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/docs/common-problems.rst` & `skip_django_reversion_pynamodb-0.2.0/docs/common-problems.rst`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/docs/conf.py` & `skip_django_reversion_pynamodb-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/docs/index.rst` & `skip_django_reversion_pynamodb-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/docs/middleware.rst` & `skip_django_reversion_pynamodb-0.2.0/docs/middleware.rst`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/docs/views.rst` & `skip_django_reversion_pynamodb-0.2.0/docs/views.rst`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/__init__.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,8 @@
         create_revision,
         register,
         is_registered,
         unregister,
         get_registered_models,
     )
 
-__version__ = VERSION = (0, 1, 6, 1)
+__version__ = VERSION = (0, 2, 0)
```

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/management/commands/initdynamodbreversion.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/management/commands/initdynamodbreversion.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/models.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/dynamodb/queryset.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/backends/dynamodb/queryset.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/admin.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.contrib.contenttypes.admin import GenericInlineModelAdmin
 from django.contrib.contenttypes.fields import GenericRelation
 from django.core.exceptions import PermissionDenied, ImproperlyConfigured
 from django.shortcuts import get_object_or_404, render, redirect
 from django.urls import reverse, re_path
 from django.utils.text import capfirst
 from django.utils.timezone import template_localtime
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.utils.encoding import force_str
 from django.utils.formats import localize
 from reversion.errors import RevertError
 from reversion.revisions import is_active, register, is_registered, set_comment, create_revision, set_user
 from reversion.views import _RollBackRevisionView
 
 from .models import Version
```

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/management/commands/__init__.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/management/commands/createinitialrevisions.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/management/commands/createinitialrevisions.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/management/commands/deleterevisions.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/management/commands/deleterevisions.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/migrations/0001_squashed_0004_auto_20160611_1202.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/migrations/0001_squashed_0004_auto_20160611_1202.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/sql/models.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/backends/sql/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from django.core import serializers
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import IntegrityError, connections, models, router, transaction
 from django.db.models.deletion import Collector
 from django.db.models.functions import Cast
 from django.utils.encoding import force_str
 from django.utils.functional import cached_property
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 from django.utils.translation import gettext_lazy as _
 
 from reversion.backends.utils import get_object_version, get_local_field_dict, get_raw_field_dict
 from reversion.errors import RevertError
 from reversion.revisions import _follow_relations_recursive, _get_content_type
 from reversion.signals import pre_revision_commit, post_revision_commit
 
@@ -26,15 +26,15 @@
     for version in versions:
         try:
             with transaction.atomic(using=version.db):
                 version.revert()
         except (IntegrityError, ObjectDoesNotExist):
             unreverted_versions.append(version)
     if len(unreverted_versions) == len(versions):
-        raise RevertError(ugettext("Could not save %(object_repr)s version - missing dependency.") % {
+        raise RevertError(gettext("Could not save %(object_repr)s version - missing dependency.") % {
             "object_repr": unreverted_versions[0],
         })
     if unreverted_versions:
         _safe_revert(unreverted_versions)
 
 
 class Revision(models.Model):
```

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/backends/utils.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/backends/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from django.core import serializers
 from django.core.serializers.base import DeserializationError
 from django.db import models
 from django.utils.encoding import force_str
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 
 from reversion.errors import RevertError
 from reversion.revisions import _get_options
 from reversion.serializers import deserialize_instance, deserialize_raw_fields
 
 
 def get_object_version(model, data, object_repr, format):
     version_options = _get_options(model)
     data = force_str(data.encode('utf8'))
     try:
         return deserialize_instance(format, data, use_natural_foreign_keys=version_options.use_natural_foreign_keys)
     except DeserializationError:
-        raise RevertError(ugettext('Could not load %(object_repr)s version - incompatible version data.') % {
+        raise RevertError(gettext('Could not load %(object_repr)s version - incompatible version data.') % {
             'object_repr': object_repr,
         })
     except serializers.SerializerDoesNotExist:
-        raise RevertError(ugettext('Could not load %(object_repr)s version - unknown serializer %(format)s.') % {
+        raise RevertError(gettext('Could not load %(object_repr)s version - unknown serializer %(format)s.') % {
             'object_repr': object_repr,
             'format': format,
         })
 
 
 def get_local_field_dict(model, object_version):
     """
@@ -45,15 +45,15 @@
     return field_dict
 
 
 def get_raw_field_dict(data, object_repr, format):
     try:
         return deserialize_raw_fields(format, data)
     except DeserializationError:
-        raise RevertError(ugettext('Could not load %(object_repr)s version - incompatible version data.') % {
+        raise RevertError(gettext('Could not load %(object_repr)s version - incompatible version data.') % {
             'object_repr': object_repr,
         })
     except serializers.SerializerDoesNotExist:
-        raise RevertError(ugettext('Could not load %(object_repr)s version - unknown serializer %(format)s.') % {
+        raise RevertError(gettext('Could not load %(object_repr)s version - unknown serializer %(format)s.') % {
             'object_repr': object_repr,
             'format': format,
         })
```

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ar/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ar/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/cs/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/cs/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/da/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/da/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/de/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/de/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es_AR/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/es_AR/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/fr/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/fr/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/he/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/he/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/it/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/it/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nb/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nb/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nl/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/nl/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pl/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pl/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pt_BR/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/pt_BR/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ru/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/ru/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sk/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sk/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sl_SI/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/sl_SI/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sl_SI/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/sl_SI/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sv/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/sv/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/uk/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/uk/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_CN/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_CN/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_Hans/LC_MESSAGES/django.mo` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/locale/zh_Hans/LC_MESSAGES/django.po` & `skip_django_reversion_pynamodb-0.2.0/reversion/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/middleware.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/models.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/revisions.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/revisions.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/serializers/__init__.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/reversion/object_history.html` & `skip_django_reversion_pynamodb-0.2.0/reversion/templates/reversion/object_history.html`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/reversion/recover_form.html` & `skip_django_reversion_pynamodb-0.2.0/reversion/templates/reversion/recover_form.html`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/reversion/recover_list.html` & `skip_django_reversion_pynamodb-0.2.0/reversion/templates/reversion/recover_list.html`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/templates/reversion/revision_form.html` & `skip_django_reversion_pynamodb-0.2.0/reversion/templates/reversion/revision_form.html`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/reversion/views.py` & `skip_django_reversion_pynamodb-0.2.0/reversion/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/setup.py` & `skip_django_reversion_pynamodb-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     url="http://github.com/skip-pay/django-reversion-pynamodb",
     zip_safe=False,
     packages=find_packages(),
     package_data={
         "reversion": ["locale/*/LC_MESSAGES/django.*", "templates/reversion/*.html"]},
     cmdclass=cmdclass,
     install_requires=[
-        "django>=2.2, <4.0",
+        "django>=4.2",
         "import_string>=0.1.0",
     ],
     extras_require={
-        'dynamodb': ['skip-pydjamodb>=0.0.9.2', 'pynamodb>=5.3.4'],
+        'dynamodb': ['skip-pydjamodb>=0.1.0', 'pynamodb==5.3.4'],
     },
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/skip_django_reversion_pynamodb.egg-info/PKG-INFO` & `skip_django_reversion_pynamodb-0.2.0/skip_django_reversion_pynamodb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-reversion-pynamodb
-Version: 0.1.6.1
+Version: 0.2.0
 Summary: An extension to the Django web framework that provides version control for model instances.
 Home-page: http://github.com/skip-pay/django-reversion-pynamodb
 Author: Dave Hall,Lubos Matl
 Author-email: dave@etianen.com, matllubos@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -12,17 +12,21 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
-Requires-Python: >=3.6
-Provides-Extra: dynamodb
+Requires-Python: >=3.8
 License-File: LICENSE
+Requires-Dist: django>=4.2
+Requires-Dist: import_string>=0.1.0
+Provides-Extra: dynamodb
+Requires-Dist: skip-pydjamodb>=0.1.0; extra == "dynamodb"
+Requires-Dist: pynamodb==5.3.4; extra == "dynamodb"
 
 =========================
 django-reversion-pynamodb
 =========================
 
 |PyPI latest| |PyPI Version| |PyPI License| |TravisCI| |Docs|
```

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/skip_django_reversion_pynamodb.egg-info/SOURCES.txt` & `skip_django_reversion_pynamodb-0.2.0/skip_django_reversion_pynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/manage.py` & `skip_django_reversion_pynamodb-0.2.0/tests/manage.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/migrations/0001_initial.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/models.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_app/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/base.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_admin.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_api.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_commands.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_middleware.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_models.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/tests/test_views.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_app/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_app/views.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_app/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-reversion-pynamodb-0.1.6.1/tests/test_project/settings.py` & `skip_django_reversion_pynamodb-0.2.0/tests/test_project/settings.py`

 * *Files identical despite different names*

