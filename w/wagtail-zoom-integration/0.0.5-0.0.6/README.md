# Comparing `tmp/wagtail-zoom-integration-0.0.5.tar.gz` & `tmp/wagtail_zoom_integration-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-zoom-integration-0.0.5.tar", last modified: Fri Aug  4 14:46:36 2023, max compression
+gzip compressed data, was "wagtail_zoom_integration-0.0.6.tar", last modified: Fri Apr 19 13:57:57 2024, max compression
```

## Comparing `wagtail-zoom-integration-0.0.5.tar` & `wagtail_zoom_integration-0.0.6.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.858104 wagtail-zoom-integration-0.0.5/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.858104 wagtail-zoom-integration-0.0.5/sandbox/home/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.858104 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0002_create_homepage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0003_eventregistrationpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0004_formfield.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.858104 wagtail-zoom-integration-0.0.5/sandbox/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/sandbox/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/search/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-08-04 14:46:36.000000 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-04 14:46:36.000000 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:46:36.000000 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 14:46:36.000000 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 14:46:36.000000 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/wagtailzoom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/wagtailzoom/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.858104 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/home/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0003_eventregistrationpage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0004_formfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      254 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/search/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 13:57:57.511942 wagtail_zoom_integration-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-19 13:57:57.000000 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-19 13:57:57.000000 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:57:57.000000 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 13:57:57.000000 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 13:57:57.000000 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/wagtailzoom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/0002_remove_zoomsettings_api_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/widgets.py
```

### Comparing `wagtail-zoom-integration-0.0.5/PKG-INFO` & `wagtail_zoom_integration-0.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: wagtail-zoom-integration
-Version: 0.0.5
-Summary: Integrate Zoom Event registration registration in Wagtail Projects.
-Home-page: https://github.com/wmo-raf/wagtail-zoom-integration
-Author: Erick Otenyo
-Author-email: otenyo.erick@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # Wagtail Zoom Integration
 
 Integrate Zoom in Wagtail Projects
 
 # Features
 
 - Integrate Zoom Events (meetings or webinars) registration to form pages created with `Wagtail Form Builder`
@@ -62,48 +41,66 @@
 
 ![Zoom Settings Admin](screenshots/zoom_settings_admin.png)
 
 The steps below explain how to configure the Zoom settings, as shown on the screenshot above
 
 1. Click on Settings
 2. Select Zoom Settings
-3. Add the Zoom API Key. See next section on how to obtain the API Key.
-4. Add the Zoom API Secret. See next section on how to obtain the API Secret.
+3. Add the Zoom OAUTH Account ID, OAUTH Client ID and OAUTH Client Secret . See next section on how to create and obtain
+   these credentials from Zoom.
 5. Save
 
-### Obtaining Zoom API Key and API Secret
+### Create a Server-to-Server OAuth app
+
+The account administrator or a developer with permissions to create server-to-server OAuth apps can create these apps in
+an account.
+
+#### Prerequisites
+
+- [A Zoom account](https://support.zoom.us/hc/en-us/articles/360034967471-Getting-started-guide-for-new-users)
+- [Permissions to view and edit server-to-server OAuth apps](https://developers.zoom.us/docs/internal-apps/#enable-the-server-to-server-oauth-role)
+- [Permissions for scopes that you will add to the app](https://developers.zoom.us/docs/internal-apps/#assign-permissions-to-access-scopes)
+
+#### Steps to create a Server-to-Server OAuth app
 
-`Note`: The Zoom Account user that generates the API credentials should have the permissions to:
+1. Go to the [Zoom App Marketplace](https://marketplace.zoom.us/). Click Develop in the dropdown menu in the top-right
+   corner of the page and select **Build Server-to-Server App**.
 
-- Read and write meetings
-- Read and write webinars
+2. Add a name for your app and click **Create**.
 
-First, log into [marketplace.zoom.us](https://marketplace.zoom.us)
+![Create Server-to-Server OAuth App](screenshots/create_app.webp)
 
-![Create Zoom JWT App](screenshots/create_zoom_jwt_app.png)
+3. **App credentials**: View your account ID, client ID and client secret. You'll use these credentials to authenticate
+   with Zoom.
+4. **Information:** Add information about your app, such as a short description, company name, and developer contact
+   information (name and email address required for activation).
+5. **Feature:** Toggle whether you’d like to enable event subscriptions. If enabled, choose the event subscriptions
+   you'd like to use. See Using Zoom Webhooks for details.
+6. **Scopes:** Scopes define the API methods this app is allowed to call, and thus which information and capabilities
+   are available on Zoom. You should limit the scopes you request to only those needed by your app.
+   See [OAuth scopes](https://developers.zoom.us/docs/internal-apps/oauth-scopes-overview/) to learn more.
 
-After logging into [marketplace.zoom.us](https://marketplace.zoom.us), the interface will appear similar to above
-screenshot
+![Search Scopes](screenshots/search_scopes.webp)
 
-Follow the steps below to create a JWT app, to get the API credentials:
+Choose **Add Scopes** to search for and add scopes:
 
-1. Go to the 'Develop' dropdown button right next to the manage button,
-2. Click 'Build App'
-3. On the 'Choose your app' type page, click `Create` from within the JWT box
+![Add Scopes](screenshots/add_scopes.webp)
 
-- A modal will appear to name your app — name your app and proceed.
+7. **Activation:** Your app should be activated. If you see errors that prevent activation, please address them. You
+   will not be able to generate an access token to make API calls unless your app is activated. If your app is
+   deactivated, existing tokens will no longer work.
 
-- On the next page, under Information, fill out a Company Name, Developer Name, and Developer Email.
+### Get app credentials
 
-![Zoom JWT App Credentials](screenshots/zoom_api_credentials.png)
+**App credentials** are the client credentials, including the **account ID, client ID, and client secret**, which Zoom
+provides to app developers to access the Zoom platform. You can get these credentials for the detail page of your app in
+the Zoom App Marketplace.
 
-1. Once completed filling company details, your API Key and Secret will be generated automatically under the App
-   Credentials tab
-2. Copy the API key, and add to the Zoom settings in the Wagtail Admin
-3. Copy the API Secret. and add to the Zoom Settings in the Wagtail Admin
+More information on how to get the app credentials can be
+found [here](https://developers.zoom.us/docs/internal-apps/create/)
 
 ### Integrating Zoom Meeting/Webinar registration to custom form pages
 
 #### Use Case
 
 - You have a single-page form that
   uses [Wagtail Form Builder](https://docs.wagtail.org/en/latest/reference/contrib/forms/).
```

### Comparing `wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0001_initial.py` & `wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0002_create_homepage.py` & `wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0003_eventregistrationpage.py` & `wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0003_eventregistrationpage.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0004_formfield.py` & `wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0004_formfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/sandbox/home/models.py` & `wagtail_zoom_integration-0.0.6/sandbox/home/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/base.py` & `wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/sandbox/sandbox/urls.py` & `wagtail_zoom_integration-0.0.6/sandbox/sandbox/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/sandbox/search/views.py` & `wagtail_zoom_integration-0.0.6/sandbox/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/setup.cfg` & `wagtail_zoom_integration-0.0.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = wagtail-zoom-integration
-version = 0.0.5
+version = 0.0.6
 description = Integrate Zoom Event registration registration in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
-url = https://github.com/wmo-raf/wagtail-zoom-integration
+url = https://github.com/erick-otenyo/wagtail-zoom-integration
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
 	Intended Audience :: Developers
@@ -23,14 +23,13 @@
 [options]
 packages = find:
 include_package_data = true
 python_requires = >=3.9
 install_requires = 
 	wagtail>=4.2.2
 	requests>=2.31.0
-	pyjwt>=2.7.0
 	iso8601>=1.1.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/PKG-INFO` & `wagtail_zoom_integration-0.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: wagtail-zoom-integration
-Version: 0.0.5
+Version: 0.0.6
 Summary: Integrate Zoom Event registration registration in Wagtail Projects.
-Home-page: https://github.com/wmo-raf/wagtail-zoom-integration
+Home-page: https://github.com/erick-otenyo/wagtail-zoom-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: wagtail>=4.2.2
+Requires-Dist: requests>=2.31.0
+Requires-Dist: iso8601>=1.1.0
 
 # Wagtail Zoom Integration
 
 Integrate Zoom in Wagtail Projects
 
 # Features
 
@@ -62,48 +65,66 @@
 
 ![Zoom Settings Admin](screenshots/zoom_settings_admin.png)
 
 The steps below explain how to configure the Zoom settings, as shown on the screenshot above
 
 1. Click on Settings
 2. Select Zoom Settings
-3. Add the Zoom API Key. See next section on how to obtain the API Key.
-4. Add the Zoom API Secret. See next section on how to obtain the API Secret.
+3. Add the Zoom OAUTH Account ID, OAUTH Client ID and OAUTH Client Secret . See next section on how to create and obtain
+   these credentials from Zoom.
 5. Save
 
-### Obtaining Zoom API Key and API Secret
+### Create a Server-to-Server OAuth app
 
-`Note`: The Zoom Account user that generates the API credentials should have the permissions to:
+The account administrator or a developer with permissions to create server-to-server OAuth apps can create these apps in
+an account.
 
-- Read and write meetings
-- Read and write webinars
+#### Prerequisites
 
-First, log into [marketplace.zoom.us](https://marketplace.zoom.us)
+- [A Zoom account](https://support.zoom.us/hc/en-us/articles/360034967471-Getting-started-guide-for-new-users)
+- [Permissions to view and edit server-to-server OAuth apps](https://developers.zoom.us/docs/internal-apps/#enable-the-server-to-server-oauth-role)
+- [Permissions for scopes that you will add to the app](https://developers.zoom.us/docs/internal-apps/#assign-permissions-to-access-scopes)
 
-![Create Zoom JWT App](screenshots/create_zoom_jwt_app.png)
+#### Steps to create a Server-to-Server OAuth app
 
-After logging into [marketplace.zoom.us](https://marketplace.zoom.us), the interface will appear similar to above
-screenshot
+1. Go to the [Zoom App Marketplace](https://marketplace.zoom.us/). Click Develop in the dropdown menu in the top-right
+   corner of the page and select **Build Server-to-Server App**.
 
-Follow the steps below to create a JWT app, to get the API credentials:
+2. Add a name for your app and click **Create**.
 
-1. Go to the 'Develop' dropdown button right next to the manage button,
-2. Click 'Build App'
-3. On the 'Choose your app' type page, click `Create` from within the JWT box
+![Create Server-to-Server OAuth App](screenshots/create_app.webp)
 
-- A modal will appear to name your app — name your app and proceed.
+3. **App credentials**: View your account ID, client ID and client secret. You'll use these credentials to authenticate
+   with Zoom.
+4. **Information:** Add information about your app, such as a short description, company name, and developer contact
+   information (name and email address required for activation).
+5. **Feature:** Toggle whether you’d like to enable event subscriptions. If enabled, choose the event subscriptions
+   you'd like to use. See Using Zoom Webhooks for details.
+6. **Scopes:** Scopes define the API methods this app is allowed to call, and thus which information and capabilities
+   are available on Zoom. You should limit the scopes you request to only those needed by your app.
+   See [OAuth scopes](https://developers.zoom.us/docs/internal-apps/oauth-scopes-overview/) to learn more.
 
-- On the next page, under Information, fill out a Company Name, Developer Name, and Developer Email.
+![Search Scopes](screenshots/search_scopes.webp)
 
-![Zoom JWT App Credentials](screenshots/zoom_api_credentials.png)
+Choose **Add Scopes** to search for and add scopes:
 
-1. Once completed filling company details, your API Key and Secret will be generated automatically under the App
-   Credentials tab
-2. Copy the API key, and add to the Zoom settings in the Wagtail Admin
-3. Copy the API Secret. and add to the Zoom Settings in the Wagtail Admin
+![Add Scopes](screenshots/add_scopes.webp)
+
+7. **Activation:** Your app should be activated. If you see errors that prevent activation, please address them. You
+   will not be able to generate an access token to make API calls unless your app is activated. If your app is
+   deactivated, existing tokens will no longer work.
+
+### Get app credentials
+
+**App credentials** are the client credentials, including the **account ID, client ID, and client secret**, which Zoom
+provides to app developers to access the Zoom platform. You can get these credentials for the detail page of your app in
+the Zoom App Marketplace.
+
+More information on how to get the app credentials can be
+found [here](https://developers.zoom.us/docs/internal-apps/create/)
 
 ### Integrating Zoom Meeting/Webinar registration to custom form pages
 
 #### Use Case
 
 - You have a single-page form that
   uses [Wagtail Form Builder](https://docs.wagtail.org/en/latest/reference/contrib/forms/).
```

### Comparing `wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/SOURCES.txt` & `wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -33,11 +33,12 @@
 wagtailzoom/forms.py
 wagtailzoom/models.py
 wagtailzoom/tests.py
 wagtailzoom/views.py
 wagtailzoom/wagtail_hooks.py
 wagtailzoom/widgets.py
 wagtailzoom/migrations/0001_initial.py
+wagtailzoom/migrations/0002_remove_zoomsettings_api_key_and_more.py
 wagtailzoom/migrations/__init__.py
 wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
 wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
 wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
```

### Comparing `wagtail-zoom-integration-0.0.5/wagtailzoom/api.py` & `wagtail_zoom_integration-0.0.6/wagtailzoom/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-from datetime import datetime, timedelta
-import iso8601
+import base64
 
-import jwt
+import iso8601
 import requests
 
 from wagtailzoom.errors import ZoomApiCredentialsError
 
-JWT_EXP_DELTA_SECONDS = 60 * 2  # 2 minutes
-
 
 def get_created_time(d):
     return iso8601.parse_date(d["created_at"])
 
 
 class ZoomApi:
-    def __init__(self, api_key, api_secret):
+    def __init__(self, oauth_account_id, oauth_client_id, oauth_client_secret):
         self.is_active = False
         self.headers = {}
         self.base_url = "https://api.zoom.us/v2"
 
-        if not api_key:
-            raise ZoomApiCredentialsError(
-                "No Zoom API Key provided. Please set API Key from Zoom Settings under settings")
-
-        if not api_secret:
-            raise ZoomApiCredentialsError(
-                "No Zoom API Secret provided. Please set API Secret from Zoom Settings under settings")
-
-        self.init_api(api_key, api_secret)
-
-    def init_api(self, api_key, api_secret):
-        payload = {
-            'iss': api_key,
-            'exp': datetime.utcnow() + timedelta(seconds=JWT_EXP_DELTA_SECONDS)
-        }
+        if not oauth_account_id and not oauth_client_id and not oauth_client_secret:
+            raise ZoomApiCredentialsError("Missing Zoom API OAUTH credentials")
+
+        self.init_api(oauth_account_id, oauth_client_id, oauth_client_secret)
+
+    def init_api(self, oauth_account_id, oauth_client_id, oauth_client_secret):
+        auth_str = f"{oauth_client_id}:{oauth_client_secret}"
+        encoded_auth_str = base64.b64encode(auth_str.encode()).decode('utf-8')
+
+        r = requests.post(f'https://zoom.us/oauth/token?grant_type=account_credentials&account_id={oauth_account_id}',
+                          headers={'Authorization': f'Basic {encoded_auth_str}'})
+
+        r.raise_for_status()
+
+        res = r.json()
+        access_token = res.get("access_token")
 
-        jwt_token = jwt.encode(payload, api_secret)
-        self.headers["Authorization"] = "Bearer {}".format(jwt_token)
+        self.headers["Authorization"] = f"Bearer {access_token}"
 
         self.is_active = True
 
     def _get(self, url):
         headers = {**self.headers}
 
         response = requests.get(url, headers=headers)
@@ -64,14 +61,15 @@
 
         if meetings and limit > 1:
             meetings = meetings[:limit]
             meetings = sorted(meetings, key=get_created_time, reverse=True)
 
             for index, meeting in enumerate(meetings):
                 meetings[index]["event_type"] = "meeting"
+                meetings[index]["event_type_label"] = "Meeting"
 
         return meetings
 
     def get_webinars(self, limit=10):
         url = "{}/users/me/webinars".format(self.base_url)
         response = self._get(url)
 
@@ -82,14 +80,15 @@
 
         if webinars and limit > 1:
             webinars = webinars[:limit]
             webinars = sorted(webinars, key=get_created_time, reverse=True)
 
             for index, webinar in enumerate(webinars):
                 webinars[index]["event_type"] = "webinar"
+                webinars[index]["event_type_label"] = "Webinar"
 
         return webinars
 
     def get_events(self):
         meetings = self.get_meetings(limit=5)
 
         try:
```

### Comparing `wagtail-zoom-integration-0.0.5/wagtailzoom/forms.py` & `wagtail_zoom_integration-0.0.6/wagtailzoom/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/wagtailzoom/migrations/0001_initial.py` & `wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/wagtailzoom/models.py` & `wagtail_zoom_integration-0.0.6/wagtailzoom/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,32 +11,40 @@
 
 from .api import ZoomApi
 from .widgets import ZoomEventSelectWidget
 
 
 @register_setting
 class ZoomSettings(BaseSiteSetting):
-    api_key = models.CharField(
+    oauth_account_id = models.CharField(
         max_length=256,
         null=True,
         blank=True,
-        verbose_name=_("Zoom API Key"),
-        help_text=_("API Key obtained from Zoom"),
+        verbose_name=_("Zoom OAUTH Account ID"),
+        help_text=_("Account ID obtained from Zoom Server-to-Server OAuth"),
     )
-    api_secret = models.CharField(
+    oauth_client_id = models.CharField(
         max_length=256,
         null=True,
         blank=True,
-        verbose_name=_("Zoom API Secret"),
-        help_text=_("API Secret obtained from Zoom"),
+        verbose_name=_("Zoom OAUTH Client ID"),
+        help_text=_("Client ID obtained from Zoom Server-to-Server OAuth"),
+    )
+    oauth_client_secret = models.CharField(
+        max_length=256,
+        null=True,
+        blank=True,
+        verbose_name=_("Zoom OAUTH Client Secret"),
+        help_text=_("Client Secret obtained from Zoom Server-to-Server OAuth"),
     )
 
     panels = [
-        FieldPanel("api_key"),
-        FieldPanel("api_secret"),
+        FieldPanel("oauth_account_id"),
+        FieldPanel("oauth_client_id"),
+        FieldPanel("oauth_client_secret"),
     ]
 
 
 class AbstractZoomIntegrationForm(AbstractForm):
     zoom_event = models.TextField(blank=True, null=True, verbose_name=_('Zoom Event'), help_text=_('Select Zoom Event'))
     zoom_reg_fields_mapping = models.TextField(blank=True, null=True)
 
@@ -107,15 +115,16 @@
         success = False
         response = None
         request = kwargs.get('request', None)
 
         if self.zoom_event_id and self.zoom_merge_fields:
             try:
                 zoom_settings = ZoomSettings.for_request(request)
-                zoom = ZoomApi(api_key=zoom_settings.api_key, api_secret=zoom_settings.api_secret)
+                zoom = ZoomApi(zoom_settings.oauth_account_id, zoom_settings.oauth_client_id,
+                               zoom_settings.oauth_client_secret)
 
                 rendered_dictionary = self.render_zoom_dictionary(
                     self.format_zoom_form_submission(kwargs['form']),
                 )
                 dict_data = json.loads(rendered_dictionary)
 
                 # check if meeting or webinar
```

### Comparing `wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html` & `wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <select name="list-selection-{{ widget.name }}">
     <option value="">
         -- None --
     </option>
     {% for event in widget.selectable_events %}
         {% if event.id == widget.stored_event_id %} selected{% endif %}
         <option value="{{ event.id }}" {% if event.id|stringformat:"i" == widget.stored_event_id %} selected{% endif %}>
-            {{ event.topic }}
+            {{ event.event_type_label }} - {{ event.topic }}
         </option>
     {% endfor %}
 </select>
 {% if widget.zoom_error %}
     <div style="margin-top: 10px;color: red">{{ widget.zoom_error }}</div>
 {% endif %}
```

### Comparing `wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html` & `wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html` & `wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/wagtailzoom/views.py` & `wagtail_zoom_integration-0.0.6/wagtailzoom/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,16 @@
         zoom_event_db = json.loads(form_page.zoom_event)
         event_id = zoom_event_db.get("event_id", None)
         event_type = zoom_event_db.get("event_type", None)
 
         if event_id:
             try:
                 zoom_settings = ZoomSettings.for_request(request)
-                zoom_api = ZoomApi(api_key=zoom_settings.api_key, api_secret=zoom_settings.api_secret)
+                zoom_api = ZoomApi(zoom_settings.oauth_account_id, zoom_settings.oauth_client_id,
+                                   zoom_settings.oauth_client_secret)
 
                 if event_type == "meeting":
                     zoom_event = zoom_api.get_meeting(event_id)
                 else:
                     zoom_event = zoom_api.get_webinar(event_id)
 
                 if zoom_event:
```

### Comparing `wagtail-zoom-integration-0.0.5/wagtailzoom/wagtail_hooks.py` & `wagtail_zoom_integration-0.0.6/wagtailzoom/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.5/wagtailzoom/widgets.py` & `wagtail_zoom_integration-0.0.6/wagtailzoom/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,12 +75,12 @@
 
     def get_zoom_events(self):
         from .models import ZoomSettings
 
         current_site = Site.objects.get(is_default_site=True)
 
         zoom_settings = ZoomSettings.for_site(current_site)
-
-        api = ZoomApi(api_key=zoom_settings.api_key, api_secret=zoom_settings.api_secret)
+        api = ZoomApi(zoom_settings.oauth_account_id, zoom_settings.oauth_client_id,
+                      zoom_settings.oauth_client_secret)
         events = api.get_events()
 
         return events
```

