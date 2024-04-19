# Comparing `tmp/platform_plugin_aspects-0.7.1.tar.gz` & `tmp/platform_plugin_aspects-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform_plugin_aspects-0.7.1.tar", last modified: Wed Apr 17 16:59:35 2024, max compression
+gzip compressed data, was "platform_plugin_aspects-0.7.2.tar", last modified: Fri Apr 19 16:22:31 2024, max compression
```

## Comparing `platform_plugin_aspects-0.7.1.tar` & `platform_plugin_aspects-0.7.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.953396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.953396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.953396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.953396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/load_test_tracking_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.949396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.949396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 16:59:35.000000 platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-17 16:59:35.957396 platform_plugin_aspects-0.7.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-04-17 16:59:32.000000 platform_plugin_aspects-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.476232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.476232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.476232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.476232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.476232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.472232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.472232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11427 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 16:22:31.000000 platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-19 16:22:31.480232 platform_plugin_aspects-0.7.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-04-19 16:22:27.000000 platform_plugin_aspects-0.7.2/setup.py
```

### Comparing `platform_plugin_aspects-0.7.1/CHANGELOG.rst` & `platform_plugin_aspects-0.7.2/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.7.2 - 2024-04-19
+******************
+
+Fixed
+=====
+
+* Fixed cms url configuration
+
 0.7.1 - 2024-04-17
 ******************
 
 Fixed
 =====
 
 * Fixed issue with embedded dashboards throwing javascript errors
```

### Comparing `platform_plugin_aspects-0.7.1/LICENSE` & `platform_plugin_aspects-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/PKG-INFO` & `platform_plugin_aspects-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.7.1
+Version: 0.7.2
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -276,14 +276,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.7.2 - 2024-04-19
+******************
+
+Fixed
+=====
+
+* Fixed cms url configuration
+
 0.7.1 - 2024-04-17
 ******************
 
 Fixed
 =====
 
 * Fixed issue with embedded dashboards throwing javascript errors
```

### Comparing `platform_plugin_aspects-0.7.1/README.rst` & `platform_plugin_aspects-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/apps.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/apps.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,19 @@
     plugin_app = {
         PluginURLs.CONFIG: {
             "lms.djangoapp": {
                 PluginURLs.NAMESPACE: "",
                 PluginURLs.REGEX: r"^aspects/",
                 PluginURLs.RELATIVE_PATH: "urls",
             },
+            "cms.djangoapp": {
+                PluginURLs.NAMESPACE: "",
+                PluginURLs.REGEX: r"^aspects/",
+                PluginURLs.RELATIVE_PATH: "urls",
+            },
         },
         PluginSettings.CONFIG: {
             "lms.djangoapp": {
                 "production": {PluginSettings.RELATIVE_PATH: "settings.production"},
                 "common": {PluginSettings.RELATIVE_PATH: "settings.common"},
             },
             "cms.djangoapp": {
```

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/extensions/filters.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/extensions/filters.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/load_test_tracking_events.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/load_test_tracking_events.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/common.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/common.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/settings/production.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/settings/production.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/signals.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/signals.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/base_sink.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/external_id_sink.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/serializers.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/css/superset.css` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/html/superset.html` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/html/superset.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/embed_dashboard.js` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/embed_dashboard.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/static/js/superset.js` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/static/js/superset.js`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/tasks.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/urls.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/urls.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/utils.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/utils.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/views.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/views.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects/xblock.py` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects/xblock.py`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/PKG-INFO` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.7.1
+Version: 0.7.2
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -276,14 +276,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.7.2 - 2024-04-19
+******************
+
+Fixed
+=====
+
+* Fixed cms url configuration
+
 0.7.1 - 2024-04-17
 ******************
 
 Fixed
 =====
 
 * Fixed issue with embedded dashboards throwing javascript errors
```

### Comparing `platform_plugin_aspects-0.7.1/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform_plugin_aspects-0.7.2/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/requirements/constraints.txt` & `platform_plugin_aspects-0.7.2/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `platform_plugin_aspects-0.7.1/setup.py` & `platform_plugin_aspects-0.7.2/setup.py`

 * *Files identical despite different names*

