# Comparing `tmp/django-idp-user-2.4.0.tar.gz` & `tmp/django-idp-user-2.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-idp-user-2.4.0.tar", last modified: Wed Mar 20 09:42:32 2024, max compression
+gzip compressed data, was "django-idp-user-2.5.0.dev0.tar", last modified: Fri Apr 19 16:23:41 2024, max compression
```

## Comparing `django-idp-user-2.4.0.tar` & `django-idp-user-2.5.0.dev0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-03-20 09:42:32.445471 django-idp-user-2.4.0/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/LICENSE
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6432 2024-03-20 09:42:32.445471 django-idp-user-2.4.0/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4094 2023-11-09 15:46:44.000000 django-idp-user-2.4.0/README.md
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-03-20 09:42:32.441471 django-idp-user-2.4.0/django_idp_user.egg-info/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6432 2024-03-20 09:42:32.000000 django-idp-user-2.4.0/django_idp_user.egg-info/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1436 2024-03-20 09:42:32.000000 django-idp-user-2.4.0/django_idp_user.egg-info/SOURCES.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2024-03-20 09:42:32.000000 django-idp-user-2.4.0/django_idp_user.egg-info/dependency_links.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      412 2024-03-20 09:42:32.000000 django-idp-user-2.4.0/django_idp_user.egg-info/requires.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        9 2024-03-20 09:42:32.000000 django-idp-user-2.4.0/django_idp_user.egg-info/top_level.txt
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-03-20 09:42:32.441471 django-idp-user-2.4.0/idp_user/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2024-03-19 08:53:24.000000 django-idp-user-2.4.0/idp_user/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2048 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/agents.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1018 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/apps.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-03-20 09:42:32.441471 django-idp-user-2.4.0/idp_user/auth/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      169 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/auth/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1439 2024-01-16 11:06:35.000000 django-idp-user-2.4.0/idp_user/auth/admin_authentication.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1651 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/auth/async_authentication.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3175 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/auth/authentication.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2811 2023-11-09 15:46:44.000000 django-idp-user-2.4.0/idp_user/checks.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-03-20 09:42:32.441471 django-idp-user-2.4.0/idp_user/management/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/management/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-03-20 09:42:32.441471 django-idp-user-2.4.0/idp_user/management/commands/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/management/commands/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      803 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/management/commands/put_app_entities_records_to_kafka.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-03-20 09:42:32.445471 django-idp-user-2.4.0/idp_user/migrations/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4340 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/migrations/0001_initial.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6133 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/migrations/0001_initial_squashed_0005_alter_userrole_id.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      378 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/migrations/0002_auto_20220120_1617.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      390 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/migrations/0003_auto_20220513_1025.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      579 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/migrations/0004_auto_20220817_1526.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      446 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/migrations/0005_alter_userrole_id.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1270 2024-03-19 08:55:50.000000 django-idp-user-2.4.0/idp_user/migrations/0006_userrole_organization_and_more.py
--rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/migrations/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-03-20 09:42:32.445471 django-idp-user-2.4.0/idp_user/models/
--rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)       55 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/models/__init__.py
--rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)       89 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/models/user.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)      984 2024-03-19 08:46:17.000000 django-idp-user-2.4.0/idp_user/models/user_role.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1815 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/producer.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      830 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/schema_extensions.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-03-20 09:42:32.445471 django-idp-user-2.4.0/idp_user/services/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      139 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/services/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    13090 2024-03-19 08:59:11.000000 django-idp-user-2.4.0/idp_user/services/async_user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2581 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/services/base_user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16164 2024-03-19 17:13:35.000000 django-idp-user-2.4.0/idp_user/services/user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      836 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/settings.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      132 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/signals.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       17 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/urls.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-03-20 09:42:32.445471 django-idp-user-2.4.0/idp_user/utils/
--rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/utils/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      739 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/utils/choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      311 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/utils/classes.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      435 2023-06-03 01:21:10.000000 django-idp-user-2.4.0/idp_user/utils/exceptions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2602 2023-09-29 13:46:44.000000 django-idp-user-2.4.0/idp_user/utils/functions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2906 2024-03-19 08:59:11.000000 django-idp-user-2.4.0/idp_user/utils/typing.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3789 2024-03-20 09:42:26.000000 django-idp-user-2.4.0/pyproject.toml
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       38 2024-03-20 09:42:32.445471 django-idp-user-2.4.0/setup.cfg
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       69 2023-04-27 07:58:09.000000 django-idp-user-2.4.0/setup.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.689890 django-idp-user-2.5.0.dev0/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/LICENSE
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6479 2024-04-19 16:23:41.689890 django-idp-user-2.5.0.dev0/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4094 2023-11-09 15:46:44.000000 django-idp-user-2.5.0.dev0/README.md
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6479 2024-04-19 16:23:41.000000 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1478 2024-04-19 16:23:41.000000 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/SOURCES.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2024-04-19 16:23:41.000000 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/dependency_links.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      441 2024-04-19 16:23:41.000000 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/requires.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        9 2024-04-19 16:23:41.000000 django-idp-user-2.5.0.dev0/django_idp_user.egg-info/top_level.txt
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       97 2024-03-20 09:43:22.000000 django-idp-user-2.5.0.dev0/idp_user/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2048 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/agents.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1018 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/apps.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/auth/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      306 2024-04-19 16:17:43.000000 django-idp-user-2.5.0.dev0/idp_user/auth/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1439 2024-01-16 11:06:35.000000 django-idp-user-2.5.0.dev0/idp_user/auth/admin_authentication.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1663 2024-04-19 15:51:09.000000 django-idp-user-2.5.0.dev0/idp_user/auth/async_authentication.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2290 2024-04-19 16:17:43.000000 django-idp-user-2.5.0.dev0/idp_user/auth/drf_authentication.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      925 2024-04-19 16:17:43.000000 django-idp-user-2.5.0.dev0/idp_user/auth/ninja_authentication.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2811 2023-11-09 15:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/checks.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/management/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/management/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/management/commands/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/management/commands/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      803 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/management/commands/put_app_entities_records_to_kafka.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/migrations/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4340 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0001_initial.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6133 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0001_initial_squashed_0005_alter_userrole_id.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      378 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0002_auto_20220120_1617.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      390 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0003_auto_20220513_1025.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      579 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0004_auto_20220817_1526.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      446 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0005_alter_userrole_id.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1270 2024-03-19 08:55:50.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/0006_userrole_organization_and_more.py
+-rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/migrations/__init__.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/models/
+-rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)       55 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/models/__init__.py
+-rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)       89 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/models/user.py
+-rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)      984 2024-03-19 08:46:17.000000 django-idp-user-2.5.0.dev0/idp_user/models/user_role.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1815 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/producer.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      834 2024-04-19 15:51:43.000000 django-idp-user-2.5.0.dev0/idp_user/schema_extensions.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.685890 django-idp-user-2.5.0.dev0/idp_user/services/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      139 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/services/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    13090 2024-03-19 08:59:11.000000 django-idp-user-2.5.0.dev0/idp_user/services/async_user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2581 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/services/base_user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16164 2024-03-19 17:13:35.000000 django-idp-user-2.5.0.dev0/idp_user/services/user.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      836 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/settings.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      132 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/signals.py
+-rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       17 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/urls.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-04-19 16:23:41.689890 django-idp-user-2.5.0.dev0/idp_user/utils/
+-rwxr-xr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/utils/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      739 2023-09-29 13:46:44.000000 django-idp-user-2.5.0.dev0/idp_user/utils/choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      311 2023-06-03 01:21:10.000000 django-idp-user-2.5.0.dev0/idp_user/utils/classes.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      165 2024-04-19 14:56:20.000000 django-idp-user-2.5.0.dev0/idp_user/utils/exceptions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4226 2024-04-19 16:10:01.000000 django-idp-user-2.5.0.dev0/idp_user/utils/functions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2906 2024-03-19 08:59:11.000000 django-idp-user-2.5.0.dev0/idp_user/utils/typing.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3836 2024-04-19 15:58:14.000000 django-idp-user-2.5.0.dev0/pyproject.toml
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       38 2024-04-19 16:23:41.689890 django-idp-user-2.5.0.dev0/setup.cfg
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       69 2023-04-27 07:58:09.000000 django-idp-user-2.5.0.dev0/setup.py
```

### Comparing `django-idp-user-2.4.0/LICENSE` & `django-idp-user-2.5.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/PKG-INFO` & `django-idp-user-2.5.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-idp-user
-Version: 2.4.0
+Version: 2.5.0.dev0
 Summary: A Django app that handles the communication between the IDP and the products for the authorization of users.
 Author: Mahmoud Al-Rawy, Euron Metaliaj, Klajdi Çaushi, Aleksandër Nasto, Andi Çuku, Klement Omeri, Lirim Shala
 Author-email: hello@cardoai.com
 License: Copyright 2023 CardoAI
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -25,14 +25,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: async
+Provides-Extra: drf
+Provides-Extra: ninja
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # Django IDP User
 
 [![pypi-badge]][pypi]
```

### Comparing `django-idp-user-2.4.0/README.md` & `django-idp-user-2.5.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/django_idp_user.egg-info/PKG-INFO` & `django-idp-user-2.5.0.dev0/django_idp_user.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-idp-user
-Version: 2.4.0
+Version: 2.5.0.dev0
 Summary: A Django app that handles the communication between the IDP and the products for the authorization of users.
 Author: Mahmoud Al-Rawy, Euron Metaliaj, Klajdi Çaushi, Aleksandër Nasto, Andi Çuku, Klement Omeri, Lirim Shala
 Author-email: hello@cardoai.com
 License: Copyright 2023 CardoAI
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -25,14 +25,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: async
+Provides-Extra: drf
+Provides-Extra: ninja
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # Django IDP User
 
 [![pypi-badge]][pypi]
```

### Comparing `django-idp-user-2.4.0/django_idp_user.egg-info/SOURCES.txt` & `django-idp-user-2.5.0.dev0/django_idp_user.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 idp_user/schema_extensions.py
 idp_user/settings.py
 idp_user/signals.py
 idp_user/urls.py
 idp_user/auth/__init__.py
 idp_user/auth/admin_authentication.py
 idp_user/auth/async_authentication.py
-idp_user/auth/authentication.py
+idp_user/auth/drf_authentication.py
+idp_user/auth/ninja_authentication.py
 idp_user/management/__init__.py
 idp_user/management/commands/__init__.py
 idp_user/management/commands/put_app_entities_records_to_kafka.py
 idp_user/migrations/0001_initial.py
 idp_user/migrations/0001_initial_squashed_0005_alter_userrole_id.py
 idp_user/migrations/0002_auto_20220120_1617.py
 idp_user/migrations/0003_auto_20220513_1025.py
```

### Comparing `django-idp-user-2.4.0/idp_user/agents.py` & `django-idp-user-2.5.0.dev0/idp_user/agents.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/apps.py` & `django-idp-user-2.5.0.dev0/idp_user/apps.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/auth/admin_authentication.py` & `django-idp-user-2.5.0.dev0/idp_user/auth/admin_authentication.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/auth/async_authentication.py` & `django-idp-user-2.5.0.dev0/idp_user/auth/async_authentication.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         user = await self._get_user(username)
         if user:
             scope["user"] = user
             scope["authorization_access_token"] = authorization_access_token
 
         return await self.app(scope, receive, send)
 
-    async def _get_username(self, access_token):
+    @staticmethod
+    async def _get_username(access_token):
         headers = {"Authorization": f"Bearer {access_token}"}
         async with aiohttp.ClientSession(headers=headers) as session:
             async with session.get(f"{IDP_URL}/api/users/me/") as resp:
                 if resp.status != 200:
                     return None
                 response = await resp.json()
                 return response.get("username")
```

### Comparing `django-idp-user-2.4.0/idp_user/checks.py` & `django-idp-user-2.5.0.dev0/idp_user/checks.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/management/commands/put_app_entities_records_to_kafka.py` & `django-idp-user-2.5.0.dev0/idp_user/management/commands/put_app_entities_records_to_kafka.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/migrations/0001_initial.py` & `django-idp-user-2.5.0.dev0/idp_user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/migrations/0001_initial_squashed_0005_alter_userrole_id.py` & `django-idp-user-2.5.0.dev0/idp_user/migrations/0001_initial_squashed_0005_alter_userrole_id.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/migrations/0004_auto_20220817_1526.py` & `django-idp-user-2.5.0.dev0/idp_user/migrations/0004_auto_20220817_1526.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/migrations/0006_userrole_organization_and_more.py` & `django-idp-user-2.5.0.dev0/idp_user/migrations/0006_userrole_organization_and_more.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/models/user_role.py` & `django-idp-user-2.5.0.dev0/idp_user/models/user_role.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/producer.py` & `django-idp-user-2.5.0.dev0/idp_user/producer.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/schema_extensions.py` & `django-idp-user-2.5.0.dev0/idp_user/schema_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from drf_spectacular.extensions import OpenApiAuthenticationExtension
 from drf_spectacular.openapi import AutoSchema
 from drf_spectacular.utils import OpenApiParameter
 
-from idp_user.auth.authentication import AuthenticationBackend
+from idp_user.auth.drf_authentication import AuthenticationBackend
 
 
 class BearerTokenScheme(OpenApiAuthenticationExtension):
     target_class = AuthenticationBackend  # full import path OR class ref
     name = "IDPAuthentication"  # name used in the schema
 
     def get_security_definition(self, auto_schema):
```

### Comparing `django-idp-user-2.4.0/idp_user/services/async_user.py` & `django-idp-user-2.5.0.dev0/idp_user/services/async_user.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/services/base_user.py` & `django-idp-user-2.5.0.dev0/idp_user/services/base_user.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/services/user.py` & `django-idp-user-2.5.0.dev0/idp_user/services/user.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/settings.py` & `django-idp-user-2.5.0.dev0/idp_user/settings.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/utils/choices.py` & `django-idp-user-2.5.0.dev0/idp_user/utils/choices.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/idp_user/utils/typing.py` & `django-idp-user-2.5.0.dev0/idp_user/utils/typing.py`

 * *Files identical despite different names*

### Comparing `django-idp-user-2.4.0/pyproject.toml` & `django-idp-user-2.5.0.dev0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-idp-user"
 description = "A Django app that handles the communication between the IDP and the products for the authorization of users."
 requires-python = ">=3.9"
-version = "2.4.0"
+version = "2.5.0.dev0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Intended Audience :: Developers",
@@ -25,16 +25,14 @@
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "Pyjwt ==2.6.0",
     "boto3",
     "Django",
-    "djangorestframework",
-    "drf-spectacular",
     "faust-streaming",
     "requests",
     "kafka-python",
 ]
 
 [project.license]
 file = "LICENSE"
@@ -61,17 +59,24 @@
 name = "Klement Omeri"
 
 [[project.authors]]
 name = "Lirim Shala"
 
 [project.optional-dependencies]
 async = [
-    "aiohttp ==3.8.4",
-    "aiokafka ==0.8.1",
-    "Django ==4.2.1",
+    "aiohttp >=3.8.4",
+    "aiokafka >=0.8.1",
+    "Django >=4.2.1",
+]
+drf = [
+    "djangorestframework",
+    "drf-spectacular",
+]
+ninja = [
+    "django-ninja",
 ]
 dev = [
     "black ==23.3.0",
     "build ==0.10.0",
     "coverage ==7.2.5",
     "Faker ==18.9.0",
     "pre-commit ==3.3.2",
```

