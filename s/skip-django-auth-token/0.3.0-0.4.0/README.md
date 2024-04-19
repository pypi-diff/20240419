# Comparing `tmp/skip-django-auth-token-0.3.0.tar.gz` & `tmp/skip_django_auth_token-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-auth-token-0.3.0.tar", last modified: Wed Mar 27 08:45:48 2024, max compression
+gzip compressed data, was "skip_django_auth_token-0.4.0.tar", last modified: Fri Apr 19 10:59:38 2024, max compression
```

## Comparing `skip-django-auth-token-0.3.0.tar` & `skip_django_auth_token-0.4.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.688583 skip-django-auth-token-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-27 08:45:48.688583 skip-django-auth-token-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.672583 skip-django-auth-token-0.3.0/auth_token/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.672583 skip-django-auth-token-0.3.0/auth_token/authorization_request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/authorization_request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/authorization_request/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.672583 skip-django-auth-token-0.3.0/auth_token/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.672583 skip-django-auth-token-0.3.0/auth_token/contrib/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/admin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.672583 skip-django-auth-token-0.3.0/auth_token/contrib/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.676583 skip-django-auth-token-0.3.0/auth_token/contrib/common/auth_security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/common/auth_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/common/auth_security/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/common/auth_security/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.676583 skip-django-auth-token-0.3.0/auth_token/contrib/common/default/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/common/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/common/default/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/common/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/common/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.676583 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.676583 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/auth_security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/auth_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/auth_security/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.676583 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/default/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/default/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.676583 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/tests/auth_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.676583 skip-django-auth-token-0.3.0/auth_token/contrib/ms_sso/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/ms_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/ms_sso/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/ms_sso/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/ms_sso/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/ms_sso/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.676583 skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.668583 skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.676583 skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.668583 skip-django-auth-token-0.3.0/auth_token/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.668583 skip-django-auth-token-0.3.0/auth_token/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.676583 skip-django-auth-token-0.3.0/auth_token/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.680583 skip-django-auth-token-0.3.0/auth_token/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.680583 skip-django-auth-token-0.3.0/auth_token/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/management/commands/clean_authorization_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/management/commands/clean_authorization_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/management/commands/clean_one_time_passwords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.680583 skip-django-auth-token-0.3.0/auth_token/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0002_tokenrelatedobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0003_usertokentakeover.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0004_token_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0005_auto_20180626_1724.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0006_auto_20190312_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0007_auto_20190313_1528.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0008_auto_20190509_1401.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0009_auto_20190622_1920.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0010_auto_20190723_1410.py
--rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0011_auto_20210119_1308.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0012_auto_20210119_1308.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0013_auto_20210119_1547.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0014_auto_20210308_0918.py
--rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0015_auto_20210308_0919.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/0016_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13691 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    23542 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/auth_token/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.680583 skip-django-auth-token-0.3.0/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.680583 skip-django-auth-token-0.3.0/example/dj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.684583 skip-django-auth-token-0.3.0/example/dj/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.684583 skip-django-auth-token-0.3.0/example/dj/apps/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.684583 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/is_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/ms_sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    38228 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/apps/app/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.684583 skip-django-auth-token-0.3.0/example/dj/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/dj/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/example/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 08:45:48.688583 skip-django-auth-token-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-27 08:45:44.000000 skip-django-auth-token-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 08:45:48.684583 skip-django-auth-token-0.3.0/skip_django_auth_token.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-27 08:45:48.000000 skip-django-auth-token-0.3.0/skip_django_auth_token.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-03-27 08:45:48.000000 skip-django-auth-token-0.3.0/skip_django_auth_token.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 08:45:48.000000 skip-django-auth-token-0.3.0/skip_django_auth_token.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 08:45:48.000000 skip-django-auth-token-0.3.0/skip_django_auth_token.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-27 08:45:48.000000 skip-django-auth-token-0.3.0/skip_django_auth_token.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-27 08:45:48.000000 skip-django-auth-token-0.3.0/skip_django_auth_token.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.663020 skip_django_auth_token-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-19 10:59:38.663020 skip_django_auth_token-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/authorization_request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/authorization_request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/authorization_request/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/contrib/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/admin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/contrib/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/contrib/common/auth_security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/common/auth_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/common/auth_security/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/common/auth_security/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/contrib/common/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/common/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/common/default/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/common/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/common/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/auth_security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/auth_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/auth_security/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/default/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/tests/auth_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.651020 skip_django_auth_token-0.4.0/auth_token/contrib/ms_sso/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/ms_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/ms_sso/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/ms_sso/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/ms_sso/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/ms_sso/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.655020 skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.647020 skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.655020 skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.647020 skip_django_auth_token-0.4.0/auth_token/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.647020 skip_django_auth_token-0.4.0/auth_token/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.655020 skip_django_auth_token-0.4.0/auth_token/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.655020 skip_django_auth_token-0.4.0/auth_token/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.655020 skip_django_auth_token-0.4.0/auth_token/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/management/commands/clean_authorization_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/management/commands/clean_authorization_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/management/commands/clean_one_time_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.659020 skip_django_auth_token-0.4.0/auth_token/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0002_tokenrelatedobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0003_usertokentakeover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0004_token_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0005_auto_20180626_1724.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0006_auto_20190312_0846.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0007_auto_20190313_1528.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0008_auto_20190509_1401.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0009_auto_20190622_1920.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0010_auto_20190723_1410.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0011_auto_20210119_1308.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0012_auto_20210119_1308.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0013_auto_20210119_1547.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0014_auto_20210308_0918.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0015_auto_20210308_0919.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/0016_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13691 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23509 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/auth_token/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.659020 skip_django_auth_token-0.4.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.659020 skip_django_auth_token-0.4.0/example/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.659020 skip_django_auth_token-0.4.0/example/dj/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.659020 skip_django_auth_token-0.4.0/example/dj/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.659020 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13613 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/is_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/ms_sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38228 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/apps/app/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.659020 skip_django_auth_token-0.4.0/example/dj/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/dj/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      385 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/example/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:59:38.663020 skip_django_auth_token-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-19 10:59:35.000000 skip_django_auth_token-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:59:38.663020 skip_django_auth_token-0.4.0/skip_django_auth_token.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-19 10:59:38.000000 skip_django_auth_token-0.4.0/skip_django_auth_token.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-19 10:59:38.000000 skip_django_auth_token-0.4.0/skip_django_auth_token.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:59:38.000000 skip_django_auth_token-0.4.0/skip_django_auth_token.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:59:38.000000 skip_django_auth_token-0.4.0/skip_django_auth_token.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 10:59:38.000000 skip_django_auth_token-0.4.0/skip_django_auth_token.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 10:59:38.000000 skip_django_auth_token-0.4.0/skip_django_auth_token.egg-info/top_level.txt
```

### Comparing `skip-django-auth-token-0.3.0/LICENSE` & `skip_django_auth_token-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/PKG-INFO` & `skip_django_auth_token-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: skip-django-auth-token
-Version: 0.3.0
+Version: 0.4.0
 Summary: Django authorization via tokens.
 Home-page: https://github.com/skip-pay/django-auth-token
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
-Requires-Dist: django<4.0,>=2.2.14
+Requires-Dist: django>=4.2.0
 Requires-Dist: django-ipware>=3.0.2
 Requires-Dist: import_string==0.1.0
-Requires-Dist: skip-django-chamber>=0.6.16.3
-Requires-Dist: skip-django-generic-m2m-field>=0.0.9.3
+Requires-Dist: skip-django-chamber>=0.7.2
+Requires-Dist: skip-django-generic-m2m-field>=0.1.0
 Requires-Dist: skip-django-choice-enumfields>=1.1.3.2
-Requires-Dist: skip-django-security-logger==1.6.4
+Requires-Dist: skip-django-security-logger>=1.7.0
 Requires-Dist: tqdm>=4.62.3
 Provides-Extra: mssso
 Requires-Dist: requests>=2.26.0; extra == "mssso"
 Requires-Dist: msal>=1.20.0; extra == "mssso"
```

### Comparing `skip-django-auth-token-0.3.0/README.rst` & `skip_django_auth_token-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/authorization_request/backends.py` & `skip_django_auth_token-0.4.0/auth_token/authorization_request/backends.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/backends.py` & `skip_django_auth_token-0.4.0/auth_token/backends.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/config.py` & `skip_django_auth_token-0.4.0/auth_token/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/common/auth_security/validators.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/common/auth_security/validators.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/common/auth_security/views.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/common/auth_security/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/common/default/views.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/common/default/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,19 +56,15 @@
 
 
 class TokenLogoutView(LogoutView):
 
     @method_decorator(never_cache)
     def dispatch(self, request, *args, **kwargs):
         logout(request)
-        next_page = self.get_next_page()
-        if next_page:
-            # Redirect to this page until the session has been cleared.
-            return HttpResponseRedirect(next_page)
-        return super(LogoutView, self).dispatch(request, *args, **kwargs)
+        return super().dispatch(request, *args, **kwargs)
 
 
 class InputLogMixin:
 
     def log_successful_request(self):
         pass
```

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/common/forms.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/common/forms.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/common/views.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/common/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/auth_security/resource.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/auth_security/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/default/resource.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/default/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/forms.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/forms.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/tests/auth_test_cases.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/tests/auth_test_cases.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/is_core_auth/views.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/is_core_auth/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/ms_sso/backends.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/ms_sso/backends.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/ms_sso/helpers.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/ms_sso/helpers.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/ms_sso/views.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/ms_sso/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/authentication.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/authentication.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         # CSRF passed with authenticated user
         return (user, None)
 
     def enforce_csrf(self, request):
         """
         Enforce CSRF validation for session based authentication.
         """
-        reason = CSRFCheck().process_view(request, None, (), {})
+
+        def dummy_get_response(_):  # pragma: no cover
+            return None
+        reason = CSRFCheck(dummy_get_response).process_view(request, None, (), {})
         if reason:
             # CSRF failed, bail with explicit error message
             raise exceptions.PermissionDenied('CSRF Failed: %s' % reason)
 
     def authenticate_header(self, request):
         return settings.HEADER_TOKEN_TYPE
```

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/serializers.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/login.html` & `skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/templates/rest_framework_auth/login.html`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/contrib/rest_framework_auth/views.py` & `skip_django_auth_token-0.4.0/auth_token/contrib/rest_framework_auth/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/enums.py` & `skip_django_auth_token-0.4.0/auth_token/enums.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/locale/cs/LC_MESSAGES/django.mo` & `skip_django_auth_token-0.4.0/auth_token/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/locale/cs/LC_MESSAGES/django.po` & `skip_django_auth_token-0.4.0/auth_token/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/management/commands/clean_authorization_requests.py` & `skip_django_auth_token-0.4.0/auth_token/management/commands/clean_authorization_requests.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/management/commands/clean_authorization_tokens.py` & `skip_django_auth_token-0.4.0/auth_token/management/commands/clean_authorization_tokens.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/management/commands/clean_one_time_passwords.py` & `skip_django_auth_token-0.4.0/auth_token/management/commands/clean_one_time_passwords.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/middleware.py` & `skip_django_auth_token-0.4.0/auth_token/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import timedelta
 import time
 
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.functional import SimpleLazyObject
 from django.utils.http import http_date
 
 from auth_token.utils import header_name_to_django, dont_enforce_csrf_checks, get_auth_token_age, get_token
 from auth_token.utils import get_user as utils_get_user
 from auth_token.config import settings
 from auth_token.models import compute_authorization_token_expires_at
@@ -43,15 +43,15 @@
     def _update_token_and_cookie(self, request, response, max_age, expires):
         expires_at = compute_authorization_token_expires_at(
             get_auth_token_age(request, request.token.user, request.token.auth_slug),
         )
         if expires_at - request.token.expires_at >= timedelta(seconds=settings.EXPIRATION_DELTA):
             request.token.change_and_save(expires_at=expires_at, update_only_changed_fields=True)
         if settings.COOKIE and request.token.allowed_cookie:
-            response.set_cookie(settings.COOKIE_NAME, force_text(request.token.secret_key), max_age=max_age,
+            response.set_cookie(settings.COOKIE_NAME, force_str(request.token.secret_key), max_age=max_age,
                                 expires=expires, httponly=settings.COOKIE_HTTPONLY,
                                 secure=settings.COOKIE_SECURE, domain=settings.COOKIE_DOMAIN)
         return response
 
     def _set_auth_expiration_header(self, request, response):
         response[settings.EXPIRATION_HEADER] = str(request.token.time_to_expiration)
```

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0001_initial.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0002_tokenrelatedobject.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0002_tokenrelatedobject.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0003_usertokentakeover.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0003_usertokentakeover.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0005_auto_20180626_1724.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0005_auto_20180626_1724.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0006_auto_20190312_0846.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0006_auto_20190312_0846.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0007_auto_20190313_1528.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0007_auto_20190313_1528.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0008_auto_20190509_1401.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0008_auto_20190509_1401.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0009_auto_20190622_1920.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0009_auto_20190622_1920.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0010_auto_20190723_1410.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0010_auto_20190723_1410.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0011_auto_20210119_1308.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0011_auto_20210119_1308.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0012_auto_20210119_1308.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0012_auto_20210119_1308.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0013_auto_20210119_1547.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0013_auto_20210119_1547.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0014_auto_20210308_0918.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0014_auto_20210308_0918.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/migrations/0015_auto_20210308_0919.py` & `skip_django_auth_token-0.4.0/auth_token/migrations/0015_auto_20210308_0919.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/models.py` & `skip_django_auth_token-0.4.0/auth_token/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/signals.py` & `skip_django_auth_token-0.4.0/auth_token/signals.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/auth_token/utils.py` & `skip_django_auth_token-0.4.0/auth_token/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     Returns:
         hashed value
     """
     return salted_hmac(
         settings.HASH_SALT,
         key,
         secret='|'.join((salt or '', django_settings.SECRET_KEY)),
-        algorithm=django_settings.DEFAULT_HASHING_ALGORITHM,
+        algorithm="sha256",
     ).hexdigest()
 
 
 def header_name_to_django(header_name):
     """
     Convert header into Django format with HTTP prefix.
     Args:
```

### Comparing `skip-django-auth-token-0.3.0/example/dj/apps/app/tests/admin.py` & `skip_django_auth_token-0.4.0/example/dj/apps/app/tests/admin.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/example/dj/apps/app/tests/commands.py` & `skip_django_auth_token-0.4.0/example/dj/apps/app/tests/commands.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/example/dj/apps/app/tests/is_core.py` & `skip_django_auth_token-0.4.0/example/dj/apps/app/tests/is_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import timedelta
 from unittest.mock import patch
 
 from django.contrib.auth.hashers import make_password
 from django.test import override_settings
 from django.utils import timezone
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from nose.tools import assert_equal
 
 from auth_token.config import settings
 from auth_token.models import AuthorizationToken
 from freezegun import freeze_time
 from germanium.decorators import data_consumer
 from germanium.test_cases.client import ClientTestCase
```

### Comparing `skip-django-auth-token-0.3.0/example/dj/apps/app/tests/middleware.py` & `skip_django_auth_token-0.4.0/example/dj/apps/app/tests/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/example/dj/apps/app/tests/models.py` & `skip_django_auth_token-0.4.0/example/dj/apps/app/tests/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/example/dj/apps/app/tests/ms_sso.py` & `skip_django_auth_token-0.4.0/example/dj/apps/app/tests/ms_sso.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/example/dj/apps/app/tests/rest_framework.py` & `skip_django_auth_token-0.4.0/example/dj/apps/app/tests/rest_framework.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/example/dj/apps/app/tests/utils.py` & `skip_django_auth_token-0.4.0/example/dj/apps/app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/example/dj/settings/base.py` & `skip_django_auth_token-0.4.0/example/dj/settings/base.py`

 * *Files 0% similar despite different names*

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

### Comparing `skip-django-auth-token-0.3.0/example/dj/settings/settings.py` & `skip_django_auth_token-0.4.0/example/dj/settings/settings.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/example/dj/urls.py` & `skip_django_auth_token-0.4.0/example/dj/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.conf import settings
-from django.conf.urls import url, include
+from django.urls import re_path as url, include
 from django.contrib import admin
 
 from app.resource import SimpleAPI
 from auth_token.contrib.admin.views import LoginView as AdminLoginView
 from auth_token.contrib.admin.views import LogoutView as AdminLogoutView
 from auth_token.contrib.is_core_auth.views import LoginCodeVerificationView, TwoFactorLoginView
 from auth_token.contrib.rest_framework_auth.views import LoginView as RestFrameworkLoginView
```

### Comparing `skip-django-auth-token-0.3.0/example/dj/wsgi.py` & `skip_django_auth_token-0.4.0/example/dj/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-auth-token-0.3.0/setup.py` & `skip_django_auth_token-0.4.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,21 +20,21 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Internet :: WWW/HTTP',
     ],
     install_requires=[
-        'django>=2.2.14, <4.0',
+        'django>=4.2.0',
         'django-ipware>=3.0.2',
         'import_string==0.1.0',
-        'skip-django-chamber>=0.6.16.3',
-        'skip-django-generic-m2m-field>=0.0.9.3',
+        'skip-django-chamber>=0.7.2',
+        'skip-django-generic-m2m-field>=0.1.0',
         'skip-django-choice-enumfields>=1.1.3.2',
-        'skip-django-security-logger==1.6.4',
+        'skip-django-security-logger>=1.7.0',
         'tqdm>=4.62.3',
     ],
     extras_require={
         'mssso': ['requests>=2.26.0', 'msal>=1.20.0'],
     },
     zip_safe=False
 )
```

### Comparing `skip-django-auth-token-0.3.0/skip_django_auth_token.egg-info/PKG-INFO` & `skip_django_auth_token-0.4.0/skip_django_auth_token.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: skip-django-auth-token
-Version: 0.3.0
+Version: 0.4.0
 Summary: Django authorization via tokens.
 Home-page: https://github.com/skip-pay/django-auth-token
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,authorization
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
-Requires-Dist: django<4.0,>=2.2.14
+Requires-Dist: django>=4.2.0
 Requires-Dist: django-ipware>=3.0.2
 Requires-Dist: import_string==0.1.0
-Requires-Dist: skip-django-chamber>=0.6.16.3
-Requires-Dist: skip-django-generic-m2m-field>=0.0.9.3
+Requires-Dist: skip-django-chamber>=0.7.2
+Requires-Dist: skip-django-generic-m2m-field>=0.1.0
 Requires-Dist: skip-django-choice-enumfields>=1.1.3.2
-Requires-Dist: skip-django-security-logger==1.6.4
+Requires-Dist: skip-django-security-logger>=1.7.0
 Requires-Dist: tqdm>=4.62.3
 Provides-Extra: mssso
 Requires-Dist: requests>=2.26.0; extra == "mssso"
 Requires-Dist: msal>=1.20.0; extra == "mssso"
```

### Comparing `skip-django-auth-token-0.3.0/skip_django_auth_token.egg-info/SOURCES.txt` & `skip_django_auth_token-0.4.0/skip_django_auth_token.egg-info/SOURCES.txt`

 * *Files identical despite different names*

