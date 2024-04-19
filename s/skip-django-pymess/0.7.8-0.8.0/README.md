# Comparing `tmp/skip-django-pymess-0.7.8.tar.gz` & `tmp/skip_django_pymess-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-pymess-0.7.8.tar", last modified: Mon Jan 22 14:40:42 2024, max compression
+gzip compressed data, was "skip_django_pymess-0.8.0.tar", last modified: Fri Apr 19 10:04:38 2024, max compression
```

## Comparing `skip-django-pymess-0.7.8.tar` & `skip_django_pymess-0.8.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.091391 skip-django-pymess-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-22 14:40:42.091391 skip-django-pymess-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.079392 skip-django-pymess-0.7.8/pymess/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.079392 skip-django-pymess-0.7.8/pymess/backend/
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/controlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.079392 skip-django-pymess-0.7.8/pymess/backend/dialer/
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/dialer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/dialer/daktela.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/dialer/dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.079392 skip-django-pymess-0.7.8/pymess/backend/emails/
--rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/emails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/emails/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/emails/mandrill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/emails/smtp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.079392 skip-django-pymess-0.7.8/pymess/backend/push/
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/push/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/push/onesignal.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/routers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.083392 skip-django-pymess-0.7.8/pymess/backend/sms/
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12378 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/sms/ats_sms_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/sms/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/sms/sms_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/sms/sns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/backend/sms/twilio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.075392 skip-django-pymess-0.7.8/pymess/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.075392 skip-django-pymess-0.7.8/pymess/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.083392 skip-django-pymess-0.7.8/pymess/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.083392 skip-django-pymess-0.7.8/pymess/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.083392 skip-django-pymess-0.7.8/pymess/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/management/commands/check_dialer_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/management/commands/check_sms_delivery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/management/commands/dump_emails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/management/commands/pull_emails_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/management/commands/send_messages_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/management/commands/sync_emails.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.087391 skip-django-pymess-0.7.8/pymess/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0002_emailmessage_number_of_send_attempts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0003_dialer.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0004_dialermessage_is_final_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0005_push_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0006_auto_20190322_1712.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0007_auto_20190401_1145.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0008_auto_20190726_1459.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0009_20191108_2007.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0010_20191120_1002.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0011_auto_20191210_1749.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0012_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0013_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0014_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0015_auto_20200110_0904.py
--rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0016_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0017_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0018_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0019_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0020_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0021_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0022_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0023_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0024_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0025_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0026_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0027_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0028_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/0029_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.091391 skip-django-pymess-0.7.8/pymess/models/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/models/dialer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/models/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/models/push.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/models/sms.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.075392 skip-django-pymess-0.7.8/pymess/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.075392 skip-django-pymess-0.7.8/pymess/templates/pymess/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.075392 skip-django-pymess-0.7.8/pymess/templates/pymess/sms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.091391 skip-django-pymess-0.7.8/pymess/templates/pymess/sms/ats/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/templates/pymess/sms/ats/base.xml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/templates/pymess/sms/ats/delivery_request.xml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/templates/pymess/sms/ats/sms.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.091391 skip-django-pymess-0.7.8/pymess/templates/pymess/sms/sms_operator/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/templates/pymess/sms/sms_operator/base.xml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/templates/pymess/sms/sms_operator/delivery_request.xml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/templates/pymess/sms/sms_operator/sms.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.091391 skip-django-pymess-0.7.8/pymess/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/templatetags/pymess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.091391 skip-django-pymess-0.7.8/pymess/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/utils/logged_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/utils/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.091391 skip-django-pymess-0.7.8/pymess/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/pymess/webhooks/mandrill.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 14:40:42.091391 skip-django-pymess-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-22 14:40:34.000000 skip-django-pymess-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 14:40:42.091391 skip-django-pymess-0.7.8/skip_django_pymess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-22 14:40:42.000000 skip-django-pymess-0.7.8/skip_django_pymess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-01-22 14:40:42.000000 skip-django-pymess-0.7.8/skip_django_pymess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 14:40:42.000000 skip-django-pymess-0.7.8/skip_django_pymess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 14:40:41.000000 skip-django-pymess-0.7.8/skip_django_pymess.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-22 14:40:42.000000 skip-django-pymess-0.7.8/skip_django_pymess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-22 14:40:42.000000 skip-django-pymess-0.7.8/skip_django_pymess.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.331876 skip_django_pymess-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-19 10:04:38.331876 skip_django_pymess-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.319876 skip_django_pymess-0.8.0/pymess/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.319876 skip_django_pymess-0.8.0/pymess/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/controlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.319876 skip_django_pymess-0.8.0/pymess/backend/dialer/
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/dialer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/dialer/daktela.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/dialer/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.319876 skip_django_pymess-0.8.0/pymess/backend/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/emails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/emails/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/emails/mandrill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/emails/smtp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.319876 skip_django_pymess-0.8.0/pymess/backend/push/
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/push/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/push/onesignal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/routers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.323876 skip_django_pymess-0.8.0/pymess/backend/sms/
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/sms/ats_sms_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/sms/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/sms/sms_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/sms/sns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/backend/sms/twilio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.315876 skip_django_pymess-0.8.0/pymess/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.315876 skip_django_pymess-0.8.0/pymess/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.323876 skip_django_pymess-0.8.0/pymess/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.323876 skip_django_pymess-0.8.0/pymess/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.323876 skip_django_pymess-0.8.0/pymess/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/management/commands/check_dialer_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/management/commands/check_sms_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/management/commands/dump_emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/management/commands/pull_emails_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/management/commands/send_messages_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/management/commands/sync_emails.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.327876 skip_django_pymess-0.8.0/pymess/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0002_emailmessage_number_of_send_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0003_dialer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0004_dialermessage_is_final_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0005_push_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0006_auto_20190322_1712.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0007_auto_20190401_1145.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0008_auto_20190726_1459.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0009_20191108_2007.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0010_20191120_1002.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0011_auto_20191210_1749.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0012_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0013_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0014_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0015_auto_20200110_0904.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0016_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0017_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0018_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0019_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0020_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0021_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0022_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0023_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0024_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0025_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0026_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0027_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0028_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/0029_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.327876 skip_django_pymess-0.8.0/pymess/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9841 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/models/dialer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/models/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/models/push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/models/sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.315876 skip_django_pymess-0.8.0/pymess/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.315876 skip_django_pymess-0.8.0/pymess/templates/pymess/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.315876 skip_django_pymess-0.8.0/pymess/templates/pymess/sms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.331876 skip_django_pymess-0.8.0/pymess/templates/pymess/sms/ats/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/templates/pymess/sms/ats/base.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/templates/pymess/sms/ats/delivery_request.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/templates/pymess/sms/ats/sms.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.331876 skip_django_pymess-0.8.0/pymess/templates/pymess/sms/sms_operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/templates/pymess/sms/sms_operator/base.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/templates/pymess/sms/sms_operator/delivery_request.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/templates/pymess/sms/sms_operator/sms.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.331876 skip_django_pymess-0.8.0/pymess/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/templatetags/pymess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.331876 skip_django_pymess-0.8.0/pymess/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/utils/logged_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/utils/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.331876 skip_django_pymess-0.8.0/pymess/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/pymess/webhooks/mandrill.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:04:38.331876 skip_django_pymess-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-19 10:04:35.000000 skip_django_pymess-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:04:38.331876 skip_django_pymess-0.8.0/skip_django_pymess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-19 10:04:38.000000 skip_django_pymess-0.8.0/skip_django_pymess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-19 10:04:38.000000 skip_django_pymess-0.8.0/skip_django_pymess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:04:38.000000 skip_django_pymess-0.8.0/skip_django_pymess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:04:38.000000 skip_django_pymess-0.8.0/skip_django_pymess.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 10:04:38.000000 skip_django_pymess-0.8.0/skip_django_pymess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 10:04:38.000000 skip_django_pymess-0.8.0/skip_django_pymess.egg-info/top_level.txt
```

### Comparing `skip-django-pymess-0.7.8/LICENSE` & `skip_django_pymess-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/PKG-INFO` & `skip_django_pymess-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: skip-django-pymess
-Version: 0.7.8
+Version: 0.8.0
 Summary: Pymess is a Django framework for sending messages
 Home-page: https://github.com/skip-pay/django-pymess
 Author: Lubos Matl,Oskar Hollman
 Author-email: matllubos@gmail.com
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django>=3.1
-Requires-Dist: skip-django-chamber>=0.6.16.3
+Requires-Dist: django>=4.2
+Requires-Dist: skip-django-chamber>=0.7.2
 Requires-Dist: beautifulsoup4==4.8.0
 Requires-Dist: skip-django-choice-enumfields>=1.1.3.2
 
 Documentation you can find [here](http://django-pymess.readthedocs.org/)
```

### Comparing `skip-django-pymess-0.7.8/pymess/backend/__init__.py` & `skip_django_pymess-0.8.0/pymess/backend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import OrderedDict, defaultdict
 from datetime import timedelta
 
 from django.db import transaction
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _l
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 from django.utils.timezone import now
 
 from pymess.config import settings
 from pymess.config import get_router, get_backend, get_default_sender_backend_name
 from pymess.utils import fullname
 
 
@@ -43,18 +43,18 @@
 
     def is_turned_on_batch_sending(self):
         return False
 
     def publish_or_retry_message(self, message):
         backend = self.get_backend(recipient=message.recipient)
         if message.number_of_send_attempts > backend.get_batch_max_number_of_send_attempts():
-            backend._set_message_as_failed(message, error=ugettext('the number of send attempts exceeded the limit'))
+            backend._set_message_as_failed(message, error=gettext('the number of send attempts exceeded the limit'))
             return False
         elif message.created_at < now() - timedelta(seconds=self.get_batch_max_seconds_to_send()):
-            backend._set_message_as_failed(message, error=ugettext('the age of the message exceeds the send limit'))
+            backend._set_message_as_failed(message, error=gettext('the age of the message exceeds the send limit'))
             return False
         else:
             backend.publish_message(message)
             return True
 
     @transaction.atomic
     def send(self, recipient, content, related_objects=None, tag=None, template=None, send_immediately=False,
```

### Comparing `skip-django-pymess-0.7.8/pymess/backend/dialer/__init__.py` & `skip_django_pymess-0.8.0/pymess/backend/dialer/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/backend/dialer/daktela.py` & `skip_django_pymess-0.8.0/pymess/backend/dialer/daktela.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
 from django.utils import timezone as tz
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 from pymess.backend.dialer import DialerBackend
 from pymess.config import settings
 from pymess.enums import DialerMessageState
 from pymess.utils.logged_requests import generate_session
```

### Comparing `skip-django-pymess-0.7.8/pymess/backend/emails/__init__.py` & `skip_django_pymess-0.8.0/pymess/backend/emails/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/backend/emails/dummy.py` & `skip_django_pymess-0.8.0/pymess/backend/emails/dummy.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/backend/emails/mandrill.py` & `skip_django_pymess-0.8.0/pymess/backend/emails/mandrill.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import requests
 
 from json.decoder import JSONDecodeError
 
 from enum import Enum
 
 from django.utils import timezone
-from django.utils.translation import ugettext_lazy as _
-from django.utils.translation import ugettext
+from django.utils.translation import gettext_lazy as _
+from django.utils.translation import gettext
 
 import mandrill
 
 from pymess.backend.emails import EmailBackend
 from pymess.enums import EmailMessageState
 from pymess.config import settings
 from pymess.utils.logged_requests import generate_session
@@ -93,17 +93,17 @@
                     'attachments': self._serialize_attachments(message)
                 },
             )[0]
             mandrill_state = MandrillState(result['status'].upper())
             state = self.MANDRILL_STATES_MAPPING.get(mandrill_state)
             error = None
             if mandrill_state == MandrillState.INVALID:
-                error = ugettext('invalid')
+                error = gettext('invalid')
             elif mandrill_state == MandrillState.REJECTED:
-                error = ugettext('rejected, mandrill message: "{}"').format(result['reject_reason'])
+                error = gettext('rejected, mandrill message: "{}"').format(result['reject_reason'])
 
             extra_sender_data = message.extra_sender_data or {}
             extra_sender_data['result'] = result
             self._update_message_after_sending(
                 message,
                 state=state,
                 sent_at=timezone.now(),
```

### Comparing `skip-django-pymess-0.7.8/pymess/backend/emails/smtp.py` & `skip_django_pymess-0.8.0/pymess/backend/emails/smtp.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/backend/push/__init__.py` & `skip_django_pymess-0.8.0/pymess/backend/push/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/backend/push/onesignal.py` & `skip_django_pymess-0.8.0/pymess/backend/push/onesignal.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/backend/sms/__init__.py` & `skip_django_pymess-0.8.0/pymess/backend/sms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from datetime import timedelta
 
 from django.utils import timezone
 from django.utils.module_loading import import_string
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from chamber.exceptions import PersistenceException
 
 from pymess.backend import BaseBackend, BaseController
 from pymess.backend import send as _send
 from pymess.backend import send_template as _send_template
 from pymess.config import (
```

### Comparing `skip-django-pymess-0.7.8/pymess/backend/sms/ats_sms_operator.py` & `skip_django_pymess-0.8.0/pymess/backend/sms/ats_sms_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from bs4 import BeautifulSoup
 
 import requests
 
 from enum import Enum
 
 from django.utils import timezone
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.utils.safestring import mark_safe
 from django.template.loader import render_to_string
 
 from enumfields import IntegerChoicesEnum
 
 from pymess.backend.sms import SMSBackend
 from pymess.enums import OutputSMSMessageState
```

### Comparing `skip-django-pymess-0.7.8/pymess/backend/sms/sms_operator.py` & `skip_django_pymess-0.8.0/pymess/backend/sms/sms_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from bs4 import BeautifulSoup
 
 import requests
 
 from enum import Enum
 
 from django.utils import timezone
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.template.loader import render_to_string
 
 from enumfields import IntegerChoicesEnum
 
 from pymess.backend.sms import SMSBackend
 from pymess.enums import OutputSMSMessageState
 from pymess.utils.logged_requests import generate_session
```

### Comparing `skip-django-pymess-0.7.8/pymess/backend/sms/sns.py` & `skip_django_pymess-0.8.0/pymess/backend/sms/sns.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/backend/sms/twilio.py` & `skip_django_pymess-0.8.0/pymess/backend/sms/twilio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 
 from django.conf import settings
 from django.utils import timezone
-from django.utils.translation import ugettext_lazy as _l
+from django.utils.translation import gettext_lazy as _l
 
 from pymess.backend.sms import SMSBackend
 from pymess.enums import OutputSMSMessageState
 
 from twilio.rest import TwilioRestClient
```

### Comparing `skip-django-pymess-0.7.8/pymess/config.py` & `skip_django_pymess-0.8.0/pymess/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/enums.py` & `skip_django_pymess-0.8.0/pymess/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from enumfields import IntegerChoicesEnum
 
 
 class DialerMessageState(IntegerChoicesEnum):
      # numbers are matching predefined state values in Daktela
```

### Comparing `skip-django-pymess-0.7.8/pymess/locale/cs/LC_MESSAGES/django.mo` & `skip_django_pymess-0.8.0/pymess/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/locale/cs/LC_MESSAGES/django.po` & `skip_django_pymess-0.8.0/pymess/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/management/commands/dump_emails.py` & `skip_django_pymess-0.8.0/pymess/management/commands/dump_emails.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/management/commands/pull_emails_info.py` & `skip_django_pymess-0.8.0/pymess/management/commands/pull_emails_info.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/management/commands/send_messages_batch.py` & `skip_django_pymess-0.8.0/pymess/management/commands/send_messages_batch.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/management/commands/sync_emails.py` & `skip_django_pymess-0.8.0/pymess/management/commands/sync_emails.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0001_initial.py` & `skip_django_pymess-0.8.0/pymess/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0003_dialer.py` & `skip_django_pymess-0.8.0/pymess/migrations/0003_dialer.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0005_push_notifications.py` & `skip_django_pymess-0.8.0/pymess/migrations/0005_push_notifications.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0006_auto_20190322_1712.py` & `skip_django_pymess-0.8.0/pymess/migrations/0006_auto_20190322_1712.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0007_auto_20190401_1145.py` & `skip_django_pymess-0.8.0/pymess/migrations/0007_auto_20190401_1145.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0008_auto_20190726_1459.py` & `skip_django_pymess-0.8.0/pymess/migrations/0008_auto_20190726_1459.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0009_20191108_2007.py` & `skip_django_pymess-0.8.0/pymess/migrations/0009_20191108_2007.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0010_20191120_1002.py` & `skip_django_pymess-0.8.0/pymess/migrations/0010_20191120_1002.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0011_auto_20191210_1749.py` & `skip_django_pymess-0.8.0/pymess/migrations/0011_auto_20191210_1749.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0012_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0012_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0013_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0013_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0014_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0014_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0015_auto_20200110_0904.py` & `skip_django_pymess-0.8.0/pymess/migrations/0015_auto_20200110_0904.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0016_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0016_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0017_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0017_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0018_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0018_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0019_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0019_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0020_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0020_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0021_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0021_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0022_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0022_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0023_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0023_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0024_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0024_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0025_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0025_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0026_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0026_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0027_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0027_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0028_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0028_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/migrations/0029_migration.py` & `skip_django_pymess-0.8.0/pymess/migrations/0029_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/models/common.py` & `skip_django_pymess-0.8.0/pymess/models/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.core.exceptions import ValidationError
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models
 from django.db.models import Q
 from django.db.models.functions import Cast
 from django.template import Context, Template
 from django.template.exceptions import TemplateDoesNotExist, TemplateSyntaxError
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from chamber.models import SmartModel
 
 from pymess.config import settings
 
 
 class RelatedObjectQueryset(models.QuerySet):
```

### Comparing `skip-django-pymess-0.7.8/pymess/models/dialer.py` & `skip_django_pymess-0.8.0/pymess/models/dialer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.core.exceptions import ValidationError
 from django.db import models
-from django.utils.encoding import force_text
-from django.utils.translation import ugettext_lazy as _
+from django.utils.encoding import force_str
+from django.utils.translation import gettext_lazy as _
 
 from pymess.config import settings
 from pymess.enums import DialerMessageState
 from pymess.utils import normalize_phone_number
 
 from .common import BaseAbstractTemplate, BaseMessage, BaseRelatedObject
 
@@ -41,15 +41,15 @@
 
     def clean(self):
         if self.is_autodialer and not self.content:
             raise ValidationError(_('Autodialer message must contain content.'))
         super().clean()
 
     def clean_recipient(self):
-        self.recipient = normalize_phone_number(force_text(self.recipient))
+        self.recipient = normalize_phone_number(force_str(self.recipient))
 
     @property
     def failed(self):
         return self.state in {DialerMessageState.ERROR, DialerMessageState.ERROR_RETRY}
 
 
 class DialerMessage(AbstractDialerMessage):
```

### Comparing `skip-django-pymess-0.7.8/pymess/models/emails.py` & `skip_django_pymess-0.8.0/pymess/models/emails.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from chamber.models import SmartModel
 
 from django.core.exceptions import ValidationError
 from django.core.files.base import ContentFile
 from django.utils.functional import cached_property
 from django.db import models
-from django.utils.translation import ugettext, ugettext_lazy as _
+from django.utils.translation import gettext, gettext_lazy as _
 from django.template import Template, Context
 from django.template.exceptions import TemplateSyntaxError, TemplateDoesNotExist
 
 from pymess.config import settings
 from pymess.enums import EmailMessageState
 from pymess.utils.html import raise_error_if_contains_banned_tags
 
@@ -172,15 +172,15 @@
             context_data.update(import_string(context_processor_fun_name)(context_data, self, recipient))
         return context_data
 
     def clean_subject(self, context_data=None):
         try:
             self.render_subject(context_data or {})
         except (TemplateSyntaxError, TemplateDoesNotExist) as ex:
-            raise ValidationError(ugettext('Error during template subject rendering: "{}"').format(ex))
+            raise ValidationError(gettext('Error during template subject rendering: "{}"').format(ex))
 
     def get_subject(self):
         return self.subject
 
     def render_subject(self, context_data, recipient=None):
         context_data = self._update_context_data(context_data, recipient)
         return Template(self.get_subject()).render(Context(context_data))
```

### Comparing `skip-django-pymess-0.7.8/pymess/models/push.py` & `skip_django_pymess-0.8.0/pymess/models/push.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from pymess.config import settings
 from pymess.enums import PushNotificationMessageState
 
 from .common import BaseAbstractTemplate, BaseMessage, BaseRelatedObject
 
 __all__ = (
```

### Comparing `skip-django-pymess-0.7.8/pymess/models/sms.py` & `skip_django_pymess-0.8.0/pymess/models/sms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from chamber.utils import remove_accent
 from django.db import models
-from django.utils.encoding import force_text
-from django.utils.translation import ugettext_lazy as _
+from django.utils.encoding import force_str
+from django.utils.translation import gettext_lazy as _
 
 from pymess.config import settings
 from pymess.utils import normalize_phone_number
 from pymess.enums import OutputSMSMessageState
 
 from .common import BaseAbstractTemplate, BaseMessage, BaseRelatedObject
 
@@ -32,15 +32,15 @@
     sender = models.CharField(verbose_name=_('sender'), null=True, blank=True, max_length=20)
 
     class Meta(BaseMessage.Meta):
         verbose_name = _('output SMS')
         verbose_name_plural = _('output SMS')
 
     def clean_recipient(self):
-        self.recipient = normalize_phone_number(force_text(self.recipient))
+        self.recipient = normalize_phone_number(force_str(self.recipient))
 
     def clean_content(self):
         if not settings.SMS_USE_ACCENT:
             self.content = str(remove_accent(str(self.content)))
 
     @property
     def failed(self):
```

### Comparing `skip-django-pymess-0.7.8/pymess/templatetags/pymess.py` & `skip_django_pymess-0.8.0/pymess/templatetags/pymess.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import functools
 
 from django import template
 from django.conf import settings
 from django.template.base import Node, TemplateSyntaxError, render_value_in_context
 from django.template.loader import render_to_string
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.html import format_html
 
 register = template.Library()
 
 
 class RaiseIfNoneNode(Node):
 
@@ -20,17 +20,17 @@
         self.check_variable = check_variable
         self.assign_to = assign_to
 
     def render(self, context):
         value = self.variable_name.resolve(context)
         if not value and not self.check_variable.resolve(context):
             raise ValueError('Email with slug {} missing variable named {}'.format(self.email_slug.resolve(context),
-                                                                                   force_text(self.variable_name)))
+                                                                                   force_str(self.variable_name)))
         if not value:
-            value = '{{{{ {} }}}}'.format(force_text(self.variable_name))
+            value = '{{{{ {} }}}}'.format(force_str(self.variable_name))
 
         if self.assign_to:
             context[self.assign_to] = render_value_in_context(value, context)
             return ''
         else:
             return render_value_in_context(value, context)
```

### Comparing `skip-django-pymess-0.7.8/pymess/utils/__init__.py` & `skip_django_pymess-0.8.0/pymess/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/utils/html.py` & `skip_django_pymess-0.8.0/pymess/utils/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Sequence
 
 from bs4 import BeautifulSoup
 
 from pymess.config import settings
 from django.core.exceptions import ValidationError
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 
 
 def find_banned_tag(html_body: str, banned_tags: Sequence[str] = None) -> Optional[str]:
     banned_tags = banned_tags if banned_tags is not None else settings.EMAIL_TEMPLATE_BANNED_TAGS
     soup = BeautifulSoup(html_body, 'html.parser')
     return next((tag for tag in banned_tags if soup.find(tag)), None)
```

### Comparing `skip-django-pymess-0.7.8/pymess/utils/logged_requests.py` & `skip_django_pymess-0.8.0/pymess/utils/logged_requests.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/utils/migrations.py` & `skip_django_pymess-0.8.0/pymess/utils/migrations.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/pymess/webhooks/mandrill.py` & `skip_django_pymess-0.8.0/pymess/webhooks/mandrill.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.8/setup.py` & `skip_django_pymess-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Internet :: WWW/HTTP',
     ],
     install_requires=[
-        'django>=3.1',
-        'skip-django-chamber>=0.6.16.3',
+        'django>=4.2',
+        'skip-django-chamber>=0.7.2',
         'beautifulsoup4==4.8.0',
         'skip-django-choice-enumfields>=1.1.3.2',
     ],
     zip_safe=False
 )
```

### Comparing `skip-django-pymess-0.7.8/skip_django_pymess.egg-info/PKG-INFO` & `skip_django_pymess-0.8.0/skip_django_pymess.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: skip-django-pymess
-Version: 0.7.8
+Version: 0.8.0
 Summary: Pymess is a Django framework for sending messages
 Home-page: https://github.com/skip-pay/django-pymess
 Author: Lubos Matl,Oskar Hollman
 Author-email: matllubos@gmail.com
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django>=3.1
-Requires-Dist: skip-django-chamber>=0.6.16.3
+Requires-Dist: django>=4.2
+Requires-Dist: skip-django-chamber>=0.7.2
 Requires-Dist: beautifulsoup4==4.8.0
 Requires-Dist: skip-django-choice-enumfields>=1.1.3.2
 
 Documentation you can find [here](http://django-pymess.readthedocs.org/)
```

### Comparing `skip-django-pymess-0.7.8/skip_django_pymess.egg-info/SOURCES.txt` & `skip_django_pymess-0.8.0/skip_django_pymess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

