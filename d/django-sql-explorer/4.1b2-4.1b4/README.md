# Comparing `tmp/django_sql_explorer-4.1b2.tar.gz` & `tmp/django_sql_explorer-4.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sql_explorer-4.1b2.tar", last modified: Wed Apr 17 19:28:58 2024, max compression
+gzip compressed data, was "django_sql_explorer-4.1b4.tar", last modified: Thu Apr 18 16:44:21 2024, max compression
```

## Comparing `django_sql_explorer-4.1b2.tar` & `django_sql_explorer-4.1b4.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.681993 django_sql_explorer-4.1b2/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-17 19:28:58.681993 django_sql_explorer-4.1b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.681993 django_sql_explorer-4.1b2/django_sql_explorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-17 19:28:58.000000 django_sql_explorer-4.1b2/django_sql_explorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-17 19:28:58.000000 django_sql_explorer-4.1b2/django_sql_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:28:58.000000 django_sql_explorer-4.1b2/django_sql_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:28:58.000000 django_sql_explorer-4.1b2/django_sql_explorer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-17 19:28:58.000000 django_sql_explorer-4.1b2/django_sql_explorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 19:28:58.000000 django_sql_explorer-4.1b2/django_sql_explorer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.661993 django_sql_explorer-4.1b2/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.665993 django_sql_explorer-4.1b2/explorer/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/assistant/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/assistant/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/assistant/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/assistant/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/assistant/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.657993 django_sql_explorer-4.1b2/explorer/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.657993 django_sql_explorer-4.1b2/explorer/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.665993 django_sql_explorer-4.1b2/explorer/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.657993 django_sql_explorer-4.1b2/explorer/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.665993 django_sql_explorer-4.1b2/explorer/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.665993 django_sql_explorer-4.1b2/explorer/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0002_auto_20150501_1515.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0003_query_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0004_querylog_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0005_auto_20160105_2052.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0006_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0007_querylog_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0008_auto_20190308_1642.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0009_auto_20201009_0547.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0010_sql_required.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0011_query_favorites.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0013_querylog_error_querylog_success.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/0014_promptlog.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.657993 django_sql_explorer-4.1b2/explorer/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.669993 django_sql_explorer-4.1b2/explorer/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/assistant.js
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/codemirror-config.js
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/csrf.js
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/explorer.js
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/favorites.js
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/pivot-setup.js
--rw-r--r--   0 runner    (1001) docker     (127)    77235 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/pivot.js
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/query-list.js
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/schema.js
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/js/table-to-csv.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.669993 django_sql_explorer-4.1b2/explorer/src/scss/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/scss/assistant.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/scss/explorer.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/scss/pivot.css
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/scss/styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/src/scss/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.657993 django_sql_explorer-4.1b2/explorer/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.673993 django_sql_explorer-4.1b2/explorer/static/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)   176088 2024-04-17 19:28:55.000000 django_sql_explorer-4.1b2/explorer/static/explorer/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   130648 2024-04-17 19:28:55.000000 django_sql_explorer-4.1b2/explorer/static/explorer/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   546668 2024-04-17 19:28:55.000000 django_sql_explorer-4.1b2/explorer/static/explorer/explorer.js
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-17 19:28:55.000000 django_sql_explorer-4.1b2/explorer/static/explorer/favorites.js
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-17 19:28:55.000000 django_sql_explorer-4.1b2/explorer/static/explorer/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    84338 2024-04-17 19:28:55.000000 django_sql_explorer-4.1b2/explorer/static/explorer/main.js
--rw-r--r--   0 runner    (1001) docker     (127)    66999 2024-04-17 19:28:55.000000 django_sql_explorer-4.1b2/explorer/static/explorer/pivot-setup.js
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-17 19:28:55.000000 django_sql_explorer-4.1b2/explorer/static/explorer/query-list.js
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-17 19:28:55.000000 django_sql_explorer-4.1b2/explorer/static/explorer/schema.js
--rw-r--r--   0 runner    (1001) docker     (127)   308829 2024-04-17 19:28:55.000000 django_sql_explorer-4.1b2/explorer/static/explorer/styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.657993 django_sql_explorer-4.1b2/explorer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.673993 django_sql_explorer-4.1b2/explorer/templates/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/assistant.html
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/export_buttons.html
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/fullscreen.html
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/params.html
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/pdf_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/play.html
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/preview_pane.html
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/query.html
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/query_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/query_favorite_button.html
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/query_favorites.html
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/query_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/querylog_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/schema.html
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templates/explorer/schema_building.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.677993 django_sql_explorer-4.1b2/explorer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templatetags/explorer_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/templatetags/vite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.677993 django_sql_explorer-4.1b2/explorer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_csrf_cookie_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32207 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:28:58.681993 django_sql_explorer-4.1b2/explorer/views/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/format_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/query_favorite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/explorer/views/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-17 19:28:58.681993 django_sql_explorer-4.1b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-17 19:28:42.000000 django_sql_explorer-4.1b2/vite.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.060423 django_sql_explorer-4.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-18 16:44:21.060423 django_sql_explorer-4.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.060423 django_sql_explorer-4.1b4/django_sql_explorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-18 16:44:21.000000 django_sql_explorer-4.1b4/django_sql_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-18 16:44:21.000000 django_sql_explorer-4.1b4/django_sql_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:44:21.000000 django_sql_explorer-4.1b4/django_sql_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:44:20.000000 django_sql_explorer-4.1b4/django_sql_explorer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-18 16:44:21.000000 django_sql_explorer-4.1b4/django_sql_explorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 16:44:21.000000 django_sql_explorer-4.1b4/django_sql_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.040423 django_sql_explorer-4.1b4/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.040423 django_sql_explorer-4.1b4/explorer/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/assistant/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/assistant/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/assistant/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/assistant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/assistant/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.032422 django_sql_explorer-4.1b4/explorer/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.032422 django_sql_explorer-4.1b4/explorer/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.040423 django_sql_explorer-4.1b4/explorer/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.032422 django_sql_explorer-4.1b4/explorer/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.040423 django_sql_explorer-4.1b4/explorer/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.044423 django_sql_explorer-4.1b4/explorer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0002_auto_20150501_1515.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0003_query_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0004_querylog_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0005_auto_20160105_2052.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0006_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0007_querylog_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0008_auto_20190308_1642.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0009_auto_20201009_0547.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0010_sql_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0011_query_favorites.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0013_querylog_error_querylog_success.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/0014_promptlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.032422 django_sql_explorer-4.1b4/explorer/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.044423 django_sql_explorer-4.1b4/explorer/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/assistant.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/codemirror-config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/csrf.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/explorer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/favorites.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/pivot-setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)    77235 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/pivot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/query-list.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/schema.js
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/js/table-to-csv.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.048423 django_sql_explorer-4.1b4/explorer/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/scss/assistant.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/scss/explorer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/scss/pivot.css
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/scss/styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/src/scss/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.032422 django_sql_explorer-4.1b4/explorer/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.052423 django_sql_explorer-4.1b4/explorer/static/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)   176088 2024-04-18 16:44:17.000000 django_sql_explorer-4.1b4/explorer/static/explorer/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   130648 2024-04-18 16:44:17.000000 django_sql_explorer-4.1b4/explorer/static/explorer/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   546668 2024-04-18 16:44:17.000000 django_sql_explorer-4.1b4/explorer/static/explorer/explorer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-18 16:44:17.000000 django_sql_explorer-4.1b4/explorer/static/explorer/favorites.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-18 16:44:17.000000 django_sql_explorer-4.1b4/explorer/static/explorer/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84338 2024-04-18 16:44:17.000000 django_sql_explorer-4.1b4/explorer/static/explorer/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)    66999 2024-04-18 16:44:17.000000 django_sql_explorer-4.1b4/explorer/static/explorer/pivot-setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-18 16:44:17.000000 django_sql_explorer-4.1b4/explorer/static/explorer/query-list.js
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-18 16:44:17.000000 django_sql_explorer-4.1b4/explorer/static/explorer/schema.js
+-rw-r--r--   0 runner    (1001) docker     (127)   308829 2024-04-18 16:44:17.000000 django_sql_explorer-4.1b4/explorer/static/explorer/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.032422 django_sql_explorer-4.1b4/explorer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.052423 django_sql_explorer-4.1b4/explorer/templates/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/assistant.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/export_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/fullscreen.html
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/params.html
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/pdf_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/play.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/preview_pane.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/query_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/query_favorite_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/query_favorites.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/query_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/querylog_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/schema.html
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templates/explorer/schema_building.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.052423 django_sql_explorer-4.1b4/explorer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templatetags/explorer_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/templatetags/vite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.056423 django_sql_explorer-4.1b4/explorer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_csrf_cookie_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32207 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:44:21.060423 django_sql_explorer-4.1b4/explorer/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/format_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/query_favorite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/explorer/views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-18 16:44:21.060423 django_sql_explorer-4.1b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-18 16:44:04.000000 django_sql_explorer-4.1b4/vite.config.js
```

### Comparing `django_sql_explorer-4.1b2/AUTHORS` & `django_sql_explorer-4.1b4/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/LICENSE` & `django_sql_explorer-4.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/PKG-INFO` & `django_sql_explorer-4.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sql-explorer
-Version: 4.1b2
+Version: 4.1b4
 Summary: A pluggable app that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://www.sqlexplorer.io
 Author: Chris Clark
 Author-email: chris@untrod.com
 Maintainer: Mark Walker
 Maintainer-email: theshow@gmail.com
 License: MIT
```

### Comparing `django_sql_explorer-4.1b2/README.rst` & `django_sql_explorer-4.1b4/README.rst`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/django_sql_explorer.egg-info/PKG-INFO` & `django_sql_explorer-4.1b4/django_sql_explorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sql-explorer
-Version: 4.1b2
+Version: 4.1b4
 Summary: A pluggable app that allows users (admins) to execute SQL, view, and export the results.
 Home-page: https://www.sqlexplorer.io
 Author: Chris Clark
 Author-email: chris@untrod.com
 Maintainer: Mark Walker
 Maintainer-email: theshow@gmail.com
 License: MIT
```

### Comparing `django_sql_explorer-4.1b2/django_sql_explorer.egg-info/SOURCES.txt` & `django_sql_explorer-4.1b4/django_sql_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/__init__.py` & `django_sql_explorer-4.1b4/explorer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __version_info__ = {
     "major": 4,
     "minor": 1,
     "patch": 0,
     "releaselevel": "beta",
-    "serial": 2
+    "serial": 4
 }
 
 
 def get_version(short=False):
     assert __version_info__["releaselevel"] in ("alpha", "beta", "final")
     vers = ["%(major)i.%(minor)i" % __version_info__, ]
     if __version_info__["patch"]:
```

### Comparing `django_sql_explorer-4.1b2/explorer/actions.py` & `django_sql_explorer-4.1b4/explorer/actions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/app_settings.py` & `django_sql_explorer-4.1b4/explorer/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/apps.py` & `django_sql_explorer-4.1b4/explorer/apps.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.apps import AppConfig
 from django.core.exceptions import ImproperlyConfigured
 from django.db import connections as djcs
-from django.db.utils import OperationalError
+from django.db.utils import DatabaseError
 from django.utils.translation import gettext_lazy as _
 
 
 class ExplorerAppConfig(AppConfig):
 
     name = "explorer"
     verbose_name = _("SQL Explorer")
@@ -57,12 +57,12 @@
     # Django runs (and e.g. in test runs) because no tables have yet been created. The intuitive way to handle this with
     # Django would be to tie into the post_migrate signal in ready() and run this function on post_migrate. But that
     # doesn't work because that signal is only called if indeed a migrations has been applied. If the app restarts and
     # there are no new migrations, the signal never fires. So instead we check if the Query table exists, and if it
     # does, we're good to gather stats.
     try:
         Query.objects.first()
-    except OperationalError:
+    except DatabaseError:
         return
     else:
         payload = gather_summary_stats()
         Stat(StatNames.STARTUP_STATS, payload).track()
```

### Comparing `django_sql_explorer-4.1b2/explorer/assistant/models.py` & `django_sql_explorer-4.1b4/explorer/assistant/models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/assistant/prompts.py` & `django_sql_explorer-4.1b4/explorer/assistant/prompts.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/assistant/tests.py` & `django_sql_explorer-4.1b4/explorer/assistant/tests.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/assistant/utils.py` & `django_sql_explorer-4.1b4/explorer/assistant/utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/assistant/views.py` & `django_sql_explorer-4.1b4/explorer/assistant/views.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/charts.py` & `django_sql_explorer-4.1b4/explorer/charts.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/connections.py` & `django_sql_explorer-4.1b4/explorer/connections.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/exporters.py` & `django_sql_explorer-4.1b4/explorer/exporters.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/forms.py` & `django_sql_explorer-4.1b4/explorer/forms.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/locale/ru/LC_MESSAGES/django.mo` & `django_sql_explorer-4.1b4/explorer/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/locale/ru/LC_MESSAGES/django.po` & `django_sql_explorer-4.1b4/explorer/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_sql_explorer-4.1b4/explorer/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/locale/zh_Hans/LC_MESSAGES/django.po` & `django_sql_explorer-4.1b4/explorer/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/migrations/0001_initial.py` & `django_sql_explorer-4.1b4/explorer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/migrations/0009_auto_20201009_0547.py` & `django_sql_explorer-4.1b4/explorer/migrations/0009_auto_20201009_0547.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/migrations/0011_query_favorites.py` & `django_sql_explorer-4.1b4/explorer/migrations/0011_query_favorites.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py` & `django_sql_explorer-4.1b4/explorer/migrations/0012_alter_queryfavorite_query_alter_queryfavorite_user.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/migrations/0013_querylog_error_querylog_success.py` & `django_sql_explorer-4.1b4/explorer/migrations/0013_querylog_error_querylog_success.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/migrations/0014_promptlog.py` & `django_sql_explorer-4.1b4/explorer/migrations/0014_promptlog.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/models.py` & `django_sql_explorer-4.1b4/explorer/models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/permissions.py` & `django_sql_explorer-4.1b4/explorer/permissions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/schema.py` & `django_sql_explorer-4.1b4/explorer/schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/js/assistant.js` & `django_sql_explorer-4.1b4/explorer/src/js/assistant.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/js/codemirror-config.js` & `django_sql_explorer-4.1b4/explorer/src/js/codemirror-config.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/js/explorer.js` & `django_sql_explorer-4.1b4/explorer/src/js/explorer.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/js/favorites.js` & `django_sql_explorer-4.1b4/explorer/src/js/favorites.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/js/main.js` & `django_sql_explorer-4.1b4/explorer/src/js/main.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/js/pivot-setup.js` & `django_sql_explorer-4.1b4/explorer/src/js/pivot-setup.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/js/pivot.js` & `django_sql_explorer-4.1b4/explorer/src/js/pivot.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/js/query-list.js` & `django_sql_explorer-4.1b4/explorer/src/js/query-list.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/js/schema.js` & `django_sql_explorer-4.1b4/explorer/src/js/schema.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/js/table-to-csv.js` & `django_sql_explorer-4.1b4/explorer/src/js/table-to-csv.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/scss/assistant.scss` & `django_sql_explorer-4.1b4/explorer/src/scss/assistant.scss`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/scss/explorer.scss` & `django_sql_explorer-4.1b4/explorer/src/scss/explorer.scss`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/src/scss/pivot.css` & `django_sql_explorer-4.1b4/explorer/src/scss/pivot.css`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/static/explorer/bootstrap-icons.woff` & `django_sql_explorer-4.1b4/explorer/static/explorer/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/static/explorer/bootstrap-icons.woff2` & `django_sql_explorer-4.1b4/explorer/static/explorer/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/static/explorer/explorer.js` & `django_sql_explorer-4.1b4/explorer/static/explorer/explorer.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/static/explorer/favorites.js` & `django_sql_explorer-4.1b4/explorer/static/explorer/favorites.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/static/explorer/index.js` & `django_sql_explorer-4.1b4/explorer/static/explorer/index.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/static/explorer/main.js` & `django_sql_explorer-4.1b4/explorer/static/explorer/main.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/static/explorer/pivot-setup.js` & `django_sql_explorer-4.1b4/explorer/static/explorer/pivot-setup.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/static/explorer/query-list.js` & `django_sql_explorer-4.1b4/explorer/static/explorer/query-list.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/static/explorer/schema.js` & `django_sql_explorer-4.1b4/explorer/static/explorer/schema.js`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/static/explorer/styles.css` & `django_sql_explorer-4.1b4/explorer/static/explorer/styles.css`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tasks.py` & `django_sql_explorer-4.1b4/explorer/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/assistant.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/assistant.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/base.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/base.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/export_buttons.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/export_buttons.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/fullscreen.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/fullscreen.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/params.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/params.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/pdf_template.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/pdf_template.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/play.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/play.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/preview_pane.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/preview_pane.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/query.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/query.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/query_confirm_delete.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/query_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/query_favorites.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/query_favorites.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/query_list.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/query_list.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/querylog_list.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/querylog_list.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templates/explorer/schema.html` & `django_sql_explorer-4.1b4/explorer/templates/explorer/schema.html`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templatetags/explorer_tags.py` & `django_sql_explorer-4.1b4/explorer/templatetags/explorer_tags.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/templatetags/vite.py` & `django_sql_explorer-4.1b4/explorer/templatetags/vite.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/factories.py` & `django_sql_explorer-4.1b4/explorer/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/settings.py` & `django_sql_explorer-4.1b4/explorer/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_actions.py` & `django_sql_explorer-4.1b4/explorer/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_apps.py` & `django_sql_explorer-4.1b4/explorer/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_csrf_cookie_name.py` & `django_sql_explorer-4.1b4/explorer/tests/test_csrf_cookie_name.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_exporters.py` & `django_sql_explorer-4.1b4/explorer/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_forms.py` & `django_sql_explorer-4.1b4/explorer/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_models.py` & `django_sql_explorer-4.1b4/explorer/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_schema.py` & `django_sql_explorer-4.1b4/explorer/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_tasks.py` & `django_sql_explorer-4.1b4/explorer/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_tracker.py` & `django_sql_explorer-4.1b4/explorer/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_utils.py` & `django_sql_explorer-4.1b4/explorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tests/test_views.py` & `django_sql_explorer-4.1b4/explorer/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/tracker.py` & `django_sql_explorer-4.1b4/explorer/tracker.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/urls.py` & `django_sql_explorer-4.1b4/explorer/urls.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/utils.py` & `django_sql_explorer-4.1b4/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/__init__.py` & `django_sql_explorer-4.1b4/explorer/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/auth.py` & `django_sql_explorer-4.1b4/explorer/views/auth.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/create.py` & `django_sql_explorer-4.1b4/explorer/views/create.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/download.py` & `django_sql_explorer-4.1b4/explorer/views/download.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/email.py` & `django_sql_explorer-4.1b4/explorer/views/email.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/export.py` & `django_sql_explorer-4.1b4/explorer/views/export.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/list.py` & `django_sql_explorer-4.1b4/explorer/views/list.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/mixins.py` & `django_sql_explorer-4.1b4/explorer/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/query.py` & `django_sql_explorer-4.1b4/explorer/views/query.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/query_favorite.py` & `django_sql_explorer-4.1b4/explorer/views/query_favorite.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/schema.py` & `django_sql_explorer-4.1b4/explorer/views/schema.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/stream.py` & `django_sql_explorer-4.1b4/explorer/views/stream.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/explorer/views/utils.py` & `django_sql_explorer-4.1b4/explorer/views/utils.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/package.json` & `django_sql_explorer-4.1b4/package.json`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/setup.cfg` & `django_sql_explorer-4.1b4/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/setup.py` & `django_sql_explorer-4.1b4/setup.py`

 * *Files identical despite different names*

### Comparing `django_sql_explorer-4.1b2/vite.config.js` & `django_sql_explorer-4.1b4/vite.config.js`

 * *Files identical despite different names*

