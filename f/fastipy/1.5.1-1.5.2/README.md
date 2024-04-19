# Comparing `tmp/fastipy-1.5.1.tar.gz` & `tmp/fastipy-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastipy-1.5.1.tar", last modified: Sun Apr 14 19:38:18 2024, max compression
+gzip compressed data, was "fastipy-1.5.2.tar", last modified: Fri Apr 19 17:20:15 2024, max compression
```

## Comparing `fastipy-1.5.1.tar` & `fastipy-1.5.2.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.711053 fastipy-1.5.1/
--rw-rw-rw-   0        0        0    35823 2024-04-14 01:52:52.000000 fastipy-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     7908 2024-04-14 19:38:18.709200 fastipy-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     6656 2024-04-14 19:33:49.000000 fastipy-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.648155 fastipy-1.5.1/app/
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.656710 fastipy-1.5.1/app/fastipy/
--rw-rw-rw-   0        0        0      694 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.662756 fastipy-1.5.1/app/fastipy/src/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.667752 fastipy-1.5.1/app/fastipy/src/classes/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/classes/__init__.py
--rw-rw-rw-   0        0        0      484 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/classes/decorators_base.py
--rw-rw-rw-   0        0        0     2892 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/classes/json_database.py
--rw-rw-rw-   0        0        0     4071 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/classes/mailer.py
--rw-rw-rw-   0        0        0     1764 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/classes/template_render.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.675113 fastipy-1.5.1/app/fastipy/src/constants/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/constants/__init__.py
--rw-rw-rw-   0        0        0      802 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/content_types.py
--rw-rw-rw-   0        0        0       42 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/decorators.py
--rw-rw-rw-   0        0        0      108 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/events.py
--rw-rw-rw-   0        0        0      164 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/hooks.py
--rw-rw-rw-   0        0        0      171 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/http_methods.py
--rw-rw-rw-   0        0        0     1443 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/http_status_code.py
--rw-rw-rw-   0        0        0     1024 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/serializers.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.680149 fastipy-1.5.1/app/fastipy/src/core/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/core/__init__.py
--rw-rw-rw-   0        0        0    11795 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/core/fastipy.py
--rw-rw-rw-   0        0        0    15888 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/core/reply.py
--rw-rw-rw-   0        0        0     3113 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/core/request.py
--rw-rw-rw-   0        0        0     5043 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/core/request_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.691490 fastipy-1.5.1/app/fastipy/src/exceptions/
--rw-rw-rw-   0        0        0      860 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/__init__.py
--rw-rw-rw-   0        0        0      134 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/decorator_already_exists_exception.py
--rw-rw-rw-   0        0        0      126 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/duplicate_route_exception.py
--rw-rw-rw-   0        0        0     1645 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/exception_handler.py
--rw-rw-rw-   0        0        0      411 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/fastipy_base_exception.py
--rw-rw-rw-   0        0        0      116 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/file_exception.py
--rw-rw-rw-   0        0        0      123 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/invalid_path_exception.py
--rw-rw-rw-   0        0        0      123 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/no_event_type.py
--rw-rw-rw-   0        0        0      122 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/no_hook_type.py
--rw-rw-rw-   0        0        0      124 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/no_http_method_exception.py
--rw-rw-rw-   0        0        0      117 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/reply_exception.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.696502 fastipy-1.5.1/app/fastipy/src/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/helpers/__init__.py
--rw-rw-rw-   0        0        0      531 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/helpers/async_sync_helpers.py
--rw-rw-rw-   0        0        0      318 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/helpers/content_type.py
--rw-rw-rw-   0        0        0     1144 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/helpers/route_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.698502 fastipy-1.5.1/app/fastipy/src/middlewares/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1686 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/middlewares/cors.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.701199 fastipy-1.5.1/app/fastipy/src/models/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/models/__init__.py
--rw-rw-rw-   0        0        0     1575 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/models/body.py
--rw-rw-rw-   0        0        0     2127 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/models/file.py
--rw-rw-rw-   0        0        0     2030 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/models/form.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.704198 fastipy-1.5.1/app/fastipy/src/routes/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/routes/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/routes/plugin_tree.py
--rw-rw-rw-   0        0        0     4212 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/routes/router.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.707190 fastipy-1.5.1/app/fastipy/src/types/
--rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/types/__init__.py
--rw-rw-rw-   0        0        0      225 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/types/plugins.py
--rw-rw-rw-   0        0        0      557 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/types/routes.py
-drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.708190 fastipy-1.5.1/app/fastipy.egg-info/
--rw-rw-rw-   0        0        0     7908 2024-04-14 19:38:18.000000 fastipy-1.5.1/app/fastipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2056 2024-04-14 19:38:18.000000 fastipy-1.5.1/app/fastipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 19:38:18.000000 fastipy-1.5.1/app/fastipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-14 19:38:18.000000 fastipy-1.5.1/app/fastipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-14 19:38:18.000000 fastipy-1.5.1/app/fastipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 19:38:18.711053 fastipy-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1544 2024-04-14 19:33:49.000000 fastipy-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.506116 fastipy-1.5.2/
+-rw-rw-rw-   0        0        0    35823 2024-04-14 01:52:52.000000 fastipy-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0     8007 2024-04-19 17:20:15.505123 fastipy-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6755 2024-04-19 17:19:55.000000 fastipy-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.444010 fastipy-1.5.2/app/
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.452022 fastipy-1.5.2/app/fastipy/
+-rw-rw-rw-   0        0        0      694 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.458535 fastipy-1.5.2/app/fastipy/src/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.463391 fastipy-1.5.2/app/fastipy/src/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/classes/__init__.py
+-rw-rw-rw-   0        0        0      484 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/classes/decorators_base.py
+-rw-rw-rw-   0        0        0     6074 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/classes/json_database.py
+-rw-rw-rw-   0        0        0     6751 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/classes/mailer.py
+-rw-rw-rw-   0        0        0     3843 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/classes/template_render.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.470950 fastipy-1.5.2/app/fastipy/src/constants/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/constants/__init__.py
+-rw-rw-rw-   0        0        0      802 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/constants/content_types.py
+-rw-rw-rw-   0        0        0       42 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/constants/decorators.py
+-rw-rw-rw-   0        0        0      108 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/constants/events.py
+-rw-rw-rw-   0        0        0      164 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/constants/hooks.py
+-rw-rw-rw-   0        0        0      171 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/constants/http_methods.py
+-rw-rw-rw-   0        0        0     2957 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/constants/http_status_code.py
+-rw-rw-rw-   0        0        0     1032 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/constants/serializers.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.475946 fastipy-1.5.2/app/fastipy/src/core/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/core/__init__.py
+-rw-rw-rw-   0        0        0    20996 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/core/fastipy.py
+-rw-rw-rw-   0        0        0    26458 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/core/reply.py
+-rw-rw-rw-   0        0        0     5379 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/core/request.py
+-rw-rw-rw-   0        0        0     7757 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/core/request_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.486742 fastipy-1.5.2/app/fastipy/src/exceptions/
+-rw-rw-rw-   0        0        0      918 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      121 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/decorator_already_exists_exception.py
+-rw-rw-rw-   0        0        0      113 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/duplicate_route_exception.py
+-rw-rw-rw-   0        0        0     2458 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/exception_handler.py
+-rw-rw-rw-   0        0        0      936 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/fastipy_exception.py
+-rw-rw-rw-   0        0        0      103 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/file_exception.py
+-rw-rw-rw-   0        0        0      110 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/invalid_path_exception.py
+-rw-rw-rw-   0        0        0      110 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/no_event_type.py
+-rw-rw-rw-   0        0        0      109 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/no_hook_type.py
+-rw-rw-rw-   0        0        0      111 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/no_http_method_exception.py
+-rw-rw-rw-   0        0        0      105 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/plugin_exception.py
+-rw-rw-rw-   0        0        0      104 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/exceptions/reply_exception.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.490551 fastipy-1.5.2/app/fastipy/src/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1538 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/helpers/async_sync_helpers.py
+-rw-rw-rw-   0        0        0      880 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/helpers/content_type.py
+-rw-rw-rw-   0        0        0     2236 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/helpers/route_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.492550 fastipy-1.5.2/app/fastipy/src/middlewares/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     2591 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/middlewares/cors.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.496551 fastipy-1.5.2/app/fastipy/src/models/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/models/__init__.py
+-rw-rw-rw-   0        0        0     2874 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/models/body.py
+-rw-rw-rw-   0        0        0     4535 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/models/file.py
+-rw-rw-rw-   0        0        0     2518 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/models/form.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.499111 fastipy-1.5.2/app/fastipy/src/routes/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/routes/__init__.py
+-rw-rw-rw-   0        0        0     2212 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/routes/plugin_tree.py
+-rw-rw-rw-   0        0        0     6781 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/routes/router.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.502124 fastipy-1.5.2/app/fastipy/src/types/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.2/app/fastipy/src/types/__init__.py
+-rw-rw-rw-   0        0        0      275 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/types/fastipy.py
+-rw-rw-rw-   0        0        0      225 2024-04-14 19:33:49.000000 fastipy-1.5.2/app/fastipy/src/types/plugins.py
+-rw-rw-rw-   0        0        0      683 2024-04-19 17:19:36.000000 fastipy-1.5.2/app/fastipy/src/types/routes.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:20:15.504123 fastipy-1.5.2/app/fastipy.egg-info/
+-rw-rw-rw-   0        0        0     8007 2024-04-19 17:20:15.000000 fastipy-1.5.2/app/fastipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2131 2024-04-19 17:20:15.000000 fastipy-1.5.2/app/fastipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 17:20:15.000000 fastipy-1.5.2/app/fastipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-19 17:20:15.000000 fastipy-1.5.2/app/fastipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-19 17:20:15.000000 fastipy-1.5.2/app/fastipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 17:20:15.506116 fastipy-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2024-04-19 17:19:36.000000 fastipy-1.5.2/setup.py
```

### Comparing `fastipy-1.5.1/LICENSE` & `fastipy-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.1/PKG-INFO` & `fastipy-1.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastipy
-Version: 1.5.1
+Version: 1.5.2
 Summary: Fastipy is a fast and easy-to-use open source Python library for developing RESTful APIs. Inspired by the FastAPI and Fastify syntax and powered by uvicorn ASGI web server.
 Home-page: https://github.com/Bielgomes/Fastipy
 Author: Bielgomes
 Author-email: bielgomesdasilva@hotmail.com
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/Bielgomes/Fastipy/issues
 Classifier: Development Status :: 4 - Beta
@@ -51,31 +51,31 @@
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 # Routes can be async or sync functions, but reply send functions are async
 # The handler returns the default HTTP status code 200
-@app.get('/')
+@app.get("/")
 def home(req: Request, _):
   # Get query params age
-  age = req.query['age']
+  age = req.query["age"]
   # Example: Recovery all persons from database with this age and print the html
   print("<h1>Retrieving all persons</h1><ul><li>A Person</li></ul>")
 ```
 
 ### Example for GET Route with Params, CORS and multiple methods
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy().cors()
 
-@app.get('/user/:id')
-@app.post('/user/:id')
+@app.get("/user/:id")
+@app.post("/user/:id")
 async def getUser(req: Request, reply: Reply):
   # get users from database
   for i in users:
     if i["id"] == req.params["id"]:
       # All response functions are asynchronous
       return await reply.send(i)
 
@@ -85,43 +85,43 @@
 ### Example for POST Route with Body
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
-@app.post('/user')
+@app.post("/user")
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Save user in database
   await reply.code(201).send("Created")
 ```
 
 ### Example for PUT Route with Body
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
-@app.put('/user')
+@app.put("/user")
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Update user in database
   await reply.type("text/html").code(201).send("<h1>Created</h1>")
 ```
 
 ### Example for GET Route with file stream
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
-@app.get('/stream')
+@app.get("/stream")
 async def streamFile(_, reply: Reply):
   # It could be an asynchronous generator
   def generator():
     with open("file.txt") as f:
         for line in f:
             yield line
 
@@ -141,93 +141,112 @@
 )
 
 @app.get("/")
 async def customSerializer(_, reply: Reply):
     await reply.code(404).send("Field not found")
 ```
 
+### Running
+
+Running Fastipy application in development is easy
+
+```py
+import uvicorn
+
+if __name__ == "__main__":
+  # main:app indicates the FILE:VARIABLE
+
+  # The file is the main file where Fastipy() is instantiated
+  # The variable is the name of the variable that contains the instance of Fastipy()
+
+  # You can find more configurations here https://www.uvicorn.org/
+
+  # set reload to True for automatic reloading!
+  uvicorn.run("main:app", log_level="debug", port=8000, reload=True, loop="asyncio")
+```
+
 ### See more examples in **[examples](https://github.com/Bielgomes/Fastipy/tree/main/examples)** folder
 
 ## Creating plugins
 
 ```py
 # chat.py
 from fastipy import FastipyInstance, Reply
 
 # Plugins can be asynchronous or synchronized functions
 # Plugins have access to the main instance, which means they can use all of Fastipy's functions
 def chatRoutes(app: FastipyInstance, options: dict):
-  @app.get('/')
+  @app.get("/")
   async def index(_, reply: Reply):
     await reply.send_code(200)
 
-  @app.get('/chat')
+  @app.get("/chat")
   async def test(_, reply: Reply):
     await reply.send_code(200)
 ```
 
 ```py
 # message.py
 from fastipy import FastipyInstance, Reply
 
 async def messageRoutes(app: FastipyInstance, options: dict):
-  @message.get('/')
+  @message.get("/")
   async def index(_, reply: Reply):
     await reply.send_code(200)
 
-  @message.get('/message')
+  @message.get("/message")
   async def test(_, reply: Reply):
     await reply.send_code(200)
 
-  app.name('custom plugin name')
+  app.name("custom plugin name")
 ```
 
 ```py
 # main.py
 from fastipy import Fastipy
 
 from message import messageRoutes
 from chat import chatRoutes
 
 app = Fastipy().cors()
 
-app.register(messageRoutes, {'prefix': '/message'})
-app.register(chatRoutes, {'prefix': '/chat'})
+app.register(messageRoutes, {"prefix": "/message"})
+app.register(chatRoutes, {"prefix": "/chat"})
 ```
 
 ## Hooks
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 # The preHandler hook is called before the request handler
-@app.hook('preHandler')
+@app.hook("preHandler")
 def preHandler(req: Request, reply: Reply):
-  print('onRequest hook')
+  print("onRequest hook")
 
 # The onRequest hook is called when the request is handled
-@app.hook('onRequest')
+@app.hook("onRequest")
 def onRequest(req: Request, reply: Reply):
-  print('onRequest hook')
+  print("onRequest hook")
 
 # The onResponse hook is called when the reply sends a response
-@app.hook('onResponse')
+@app.hook("onResponse")
 def onResponse(req: Request, reply: Reply):
-  print('onResponse hook')
+  print("onResponse hook")
 
 # The onError hook is called when an error occurs
-@app.hook('onError')
+@app.hook("onError")
 def onError(error: Exception, req: Request, reply: Reply):
-  print(f'onError hook exception: {error}')
+  print(f"onError hook exception: {error}")
 
 # A hook will only be linked to a route if its declaration precedes the route
 # The order of hooks of the same type is important
-@app.get('/')
+@app.get("/")
 async def index(_, reply: Reply):
   await reply.send_code(200)
 ```
 
 ## End to End tests
 
 ```py
@@ -238,56 +257,38 @@
 client = TestClient(app)
 
 response = client.post("/")
 assert response.status_code == 200
 assert response.text == "Hello World"
 ```
 
-## Running
-
-Running Fastipy application in development is easy
-
-```py
-import uvicorn
-
-if __name__ == "__main__":
-  # main:app indicates the FILE:VARIABLE
-
-  # The file is the main file where Fastipy() is instantiated
-  # The variable is the name of the variable that contains the instance of Fastipy()
-
-  # You can find more configurations here https://www.uvicorn.org/
-
-  config = uvicorn.Config('main:app', log_level='debug', port=3000)
-  server = uvicorn.Server(config)
-  server.run()
-```
-
 # Application Deploy
 
 For production deployment, please refer to this **[uvicorn guide](https://www.uvicorn.org/deployment/)**.
 
 # Change Log
 
-## Development Version 1.5.1
+## Version 1.5.2
 
 ### Added
 
-- [X] Added the possibility of printing middleware routes in the router's print tree.
-- [X] Added a customizable mail module.
-- [X] Added jinja2 lib to render templates.
-- [x] Add integration to end-to-end tests.
+- [x] Added Fastipy config.
+- [x] Added Plugin timeout configuration.
+- [x] Added typing for options in print routes function.
+- [x] Added types to request handler functions parameters.
+- [x] Added the option to automatically create folders when saving files.
+- [x] Added shortcut form property inside Request class to facilitate usability.
+- [x] Added documentation for most methods and classes.
 
 ### Changed
 
-- [X] Error imports are now centralized in the exceptions module.
-- [X] Improved error handling flow, now error handling hooks are executed first rather than the default error handling.
-- [X] Apply code reuse to generate logs.
-- [X] Refactored file stream in reply send file function.
-- [X] Reply send function now automatically serializes the value sent to it and sets a content type
+- [x] Renaming the fastipy base exception to the fastipy exception to make it easier to handle.
+- [x] Fixed problem in the error handler for python 3.11.
+- [x] Fixed the function of saving files securely, to save them in the correct path.
+- [x] Loading text and json from body files on demand.
 
 # Contributors
 
 <a href="https://github.com/Bielgomes/Fastipy/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=Bielgomes/Fastipy"/>
 </a>
```

### Comparing `fastipy-1.5.1/README.md` & `fastipy-1.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 # Routes can be async or sync functions, but reply send functions are async
 # The handler returns the default HTTP status code 200
-@app.get('/')
+@app.get("/")
 def home(req: Request, _):
   # Get query params age
-  age = req.query['age']
+  age = req.query["age"]
   # Example: Recovery all persons from database with this age and print the html
   print("<h1>Retrieving all persons</h1><ul><li>A Person</li></ul>")
 ```
 
 ### Example for GET Route with Params, CORS and multiple methods
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy().cors()
 
-@app.get('/user/:id')
-@app.post('/user/:id')
+@app.get("/user/:id")
+@app.post("/user/:id")
 async def getUser(req: Request, reply: Reply):
   # get users from database
   for i in users:
     if i["id"] == req.params["id"]:
       # All response functions are asynchronous
       return await reply.send(i)
 
@@ -57,43 +57,43 @@
 ### Example for POST Route with Body
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
-@app.post('/user')
+@app.post("/user")
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Save user in database
   await reply.code(201).send("Created")
 ```
 
 ### Example for PUT Route with Body
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
-@app.put('/user')
+@app.put("/user")
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Update user in database
   await reply.type("text/html").code(201).send("<h1>Created</h1>")
 ```
 
 ### Example for GET Route with file stream
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
-@app.get('/stream')
+@app.get("/stream")
 async def streamFile(_, reply: Reply):
   # It could be an asynchronous generator
   def generator():
     with open("file.txt") as f:
         for line in f:
             yield line
 
@@ -113,93 +113,112 @@
 )
 
 @app.get("/")
 async def customSerializer(_, reply: Reply):
     await reply.code(404).send("Field not found")
 ```
 
+### Running
+
+Running Fastipy application in development is easy
+
+```py
+import uvicorn
+
+if __name__ == "__main__":
+  # main:app indicates the FILE:VARIABLE
+
+  # The file is the main file where Fastipy() is instantiated
+  # The variable is the name of the variable that contains the instance of Fastipy()
+
+  # You can find more configurations here https://www.uvicorn.org/
+
+  # set reload to True for automatic reloading!
+  uvicorn.run("main:app", log_level="debug", port=8000, reload=True, loop="asyncio")
+```
+
 ### See more examples in **[examples](https://github.com/Bielgomes/Fastipy/tree/main/examples)** folder
 
 ## Creating plugins
 
 ```py
 # chat.py
 from fastipy import FastipyInstance, Reply
 
 # Plugins can be asynchronous or synchronized functions
 # Plugins have access to the main instance, which means they can use all of Fastipy's functions
 def chatRoutes(app: FastipyInstance, options: dict):
-  @app.get('/')
+  @app.get("/")
   async def index(_, reply: Reply):
     await reply.send_code(200)
 
-  @app.get('/chat')
+  @app.get("/chat")
   async def test(_, reply: Reply):
     await reply.send_code(200)
 ```
 
 ```py
 # message.py
 from fastipy import FastipyInstance, Reply
 
 async def messageRoutes(app: FastipyInstance, options: dict):
-  @message.get('/')
+  @message.get("/")
   async def index(_, reply: Reply):
     await reply.send_code(200)
 
-  @message.get('/message')
+  @message.get("/message")
   async def test(_, reply: Reply):
     await reply.send_code(200)
 
-  app.name('custom plugin name')
+  app.name("custom plugin name")
 ```
 
 ```py
 # main.py
 from fastipy import Fastipy
 
 from message import messageRoutes
 from chat import chatRoutes
 
 app = Fastipy().cors()
 
-app.register(messageRoutes, {'prefix': '/message'})
-app.register(chatRoutes, {'prefix': '/chat'})
+app.register(messageRoutes, {"prefix": "/message"})
+app.register(chatRoutes, {"prefix": "/chat"})
 ```
 
 ## Hooks
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 # The preHandler hook is called before the request handler
-@app.hook('preHandler')
+@app.hook("preHandler")
 def preHandler(req: Request, reply: Reply):
-  print('onRequest hook')
+  print("onRequest hook")
 
 # The onRequest hook is called when the request is handled
-@app.hook('onRequest')
+@app.hook("onRequest")
 def onRequest(req: Request, reply: Reply):
-  print('onRequest hook')
+  print("onRequest hook")
 
 # The onResponse hook is called when the reply sends a response
-@app.hook('onResponse')
+@app.hook("onResponse")
 def onResponse(req: Request, reply: Reply):
-  print('onResponse hook')
+  print("onResponse hook")
 
 # The onError hook is called when an error occurs
-@app.hook('onError')
+@app.hook("onError")
 def onError(error: Exception, req: Request, reply: Reply):
-  print(f'onError hook exception: {error}')
+  print(f"onError hook exception: {error}")
 
 # A hook will only be linked to a route if its declaration precedes the route
 # The order of hooks of the same type is important
-@app.get('/')
+@app.get("/")
 async def index(_, reply: Reply):
   await reply.send_code(200)
 ```
 
 ## End to End tests
 
 ```py
@@ -210,56 +229,38 @@
 client = TestClient(app)
 
 response = client.post("/")
 assert response.status_code == 200
 assert response.text == "Hello World"
 ```
 
-## Running
-
-Running Fastipy application in development is easy
-
-```py
-import uvicorn
-
-if __name__ == "__main__":
-  # main:app indicates the FILE:VARIABLE
-
-  # The file is the main file where Fastipy() is instantiated
-  # The variable is the name of the variable that contains the instance of Fastipy()
-
-  # You can find more configurations here https://www.uvicorn.org/
-
-  config = uvicorn.Config('main:app', log_level='debug', port=3000)
-  server = uvicorn.Server(config)
-  server.run()
-```
-
 # Application Deploy
 
 For production deployment, please refer to this **[uvicorn guide](https://www.uvicorn.org/deployment/)**.
 
 # Change Log
 
-## Development Version 1.5.1
+## Version 1.5.2
 
 ### Added
 
-- [X] Added the possibility of printing middleware routes in the router's print tree.
-- [X] Added a customizable mail module.
-- [X] Added jinja2 lib to render templates.
-- [x] Add integration to end-to-end tests.
+- [x] Added Fastipy config.
+- [x] Added Plugin timeout configuration.
+- [x] Added typing for options in print routes function.
+- [x] Added types to request handler functions parameters.
+- [x] Added the option to automatically create folders when saving files.
+- [x] Added shortcut form property inside Request class to facilitate usability.
+- [x] Added documentation for most methods and classes.
 
 ### Changed
 
-- [X] Error imports are now centralized in the exceptions module.
-- [X] Improved error handling flow, now error handling hooks are executed first rather than the default error handling.
-- [X] Apply code reuse to generate logs.
-- [X] Refactored file stream in reply send file function.
-- [X] Reply send function now automatically serializes the value sent to it and sets a content type
+- [x] Renaming the fastipy base exception to the fastipy exception to make it easier to handle.
+- [x] Fixed problem in the error handler for python 3.11.
+- [x] Fixed the function of saving files securely, to save them in the correct path.
+- [x] Loading text and json from body files on demand.
 
 # Contributors
 
 <a href="https://github.com/Bielgomes/Fastipy/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=Bielgomes/Fastipy"/>
 </a>
```

### Comparing `fastipy-1.5.1/app/fastipy/__init__.py` & `fastipy-1.5.2/app/fastipy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.5.1"
+__version__ = "1.5.2"
 
 from .src.core.fastipy import Fastipy, FastipyInstance
 
 from .src.types.plugins import PluginOptions
 
 from .src.core.request import Request
 from .src.core.reply import Reply
```

### Comparing `fastipy-1.5.1/app/fastipy/src/constants/content_types.py` & `fastipy-1.5.2/app/fastipy/src/constants/content_types.py`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.1/app/fastipy/src/constants/serializers.py` & `fastipy-1.5.2/app/fastipy/src/constants/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
 
-def validate_json(data: any):
+def validate_json(data: any) -> bool:
     try:
         return bool(json.loads(data))
     except:
         return False
 
 
 SERIALIZERS = [
```

### Comparing `fastipy-1.5.1/app/fastipy/src/exceptions/__init__.py` & `fastipy-1.5.2/app/fastipy/src/exceptions/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from .decorator_already_exists_exception import DecoratorAlreadyExistsException
 from .duplicate_route_exception import DuplicateRouteException
 from .exception_handler import ExceptionHandler
-from .fastipy_base_exception import FastipyBaseException
+from .fastipy_exception import FastipyException
 from .file_exception import FileException
 from .invalid_path_exception import InvalidPathException
 from .no_event_type import NoEventTypeException
 from .no_hook_type import NoHookTypeException
 from .no_http_method_exception import NoHTTPMethodException
+from .plugin_exception import PluginException
 from .reply_exception import ReplyException
 
 __all__ = [
     "DecoratorAlreadyExistsException",
     "DuplicateRouteException",
     "ExceptionHandler",
-    "FastipyBaseException",
+    "FastipyException",
     "FileException",
     "InvalidPathException",
     "NoEventTypeException",
     "NoHookTypeException",
     "NoHTTPMethodException",
+    "PluginException",
     "ReplyException",
 ]
```

### Comparing `fastipy-1.5.1/app/fastipy/src/helpers/async_sync_helpers.py` & `fastipy-1.5.2/app/fastipy/src/helpers/async_sync_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,46 @@
 import asyncio
+from typing import Optional
 
 from ..types.routes import FunctionType
 
 
-def run_sync_or_async(function: FunctionType, *args, **kwargs):
+def run_sync_or_async(
+    function: FunctionType, timeout: Optional[float] = None, *args, **kwargs
+) -> Optional[Exception]:
+    """
+    Run a function synchronously or asynchronously.
+
+    Args:
+        function (FunctionType): The function to be executed.
+        timeout (Optional[float], optional): Timeout duration for asynchronous functions. Defaults to None.
+        *args: Variable length argument list.
+        **kwargs: Arbitrary keyword arguments.
+
+    Returns:
+        Exception or None: If an error occurs during execution, returns the exception; otherwise, returns None.
+    """
     if asyncio.iscoroutinefunction(function):
         loop = asyncio.get_event_loop()
-        loop.run_until_complete(function(*args, **kwargs))
+        try:
+            loop.run_until_complete(
+                asyncio.wait_for(function(*args, **kwargs), timeout=timeout)
+            )
+        except (asyncio.TimeoutError, asyncio.CancelledError) as error:
+            return error
     else:
         function(*args, **kwargs)
 
 
-async def run_async_or_sync(function: FunctionType, *args, **kwargs):
+async def run_async_or_sync(function: FunctionType, *args, **kwargs) -> None:
+    """
+    Run a function asynchronously or synchronously.
+
+    Args:
+        function (FunctionType): The function to be executed.
+        *args: Variable length argument list.
+        **kwargs: Arbitrary keyword arguments.
+    """
     if asyncio.iscoroutinefunction(function):
         await function(*args, **kwargs)
     else:
         function(*args, **kwargs)
```

### Comparing `fastipy-1.5.1/app/fastipy/src/models/body.py` & `fastipy-1.5.2/app/fastipy/src/models/body.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,99 @@
 from typing import Union
 import json
 
 from .form import Form
 
 
 class Body:
+    """
+    Represents the body of an HTTP request, providing access to its content and metadata.
+    """
+
     def __init__(self, scope, receive) -> None:
+        """
+        Initialize the Body object.
+
+        Args:
+            scope: The scope of the request.
+            receive: The receive function.
+        """
         self.__scope = scope
         self.__receive = receive
 
         self._content = None
         self._raw_content = None
         self._content_type = self.__scope["headers"].get("content-type", None)
         self._content_length = int(self.__scope["headers"].get("content-length", 0))
         self._json = None
 
     @property
     def type(self) -> Union[str, None]:
+        """
+        Get the content type of the body.
+
+        Returns:
+            Union[str, None]: The content type.
+        """
         return self._content_type
 
     @property
     def length(self) -> int:
+        """
+        Get the length of the body content.
+
+        Returns:
+            int: The length of the body content.
+        """
         return self._content_length
 
     @property
     def content(self) -> str:
+        """
+        Get the content of the body as a string.
+
+        Returns:
+            str: The content of the body.
+        """
         return self._content
 
     @property
     def raw_content(self) -> bytes:
+        """
+        Get the raw content of the body.
+
+        Returns:
+            bytes: The raw content of the body.
+        """
         return self._raw_content
 
     @property
     def json(self) -> dict:
+        """
+        Get the JSON representation of the body content.
+
+        Returns:
+            dict: The JSON representation of the body content.
+        """
         return self._json
 
     @property
     def form(self) -> "Form":
+        """
+        Get the form representation of the body content.
+
+        Returns:
+            Form: The form representation of the body content.
+        """
         return self._form
 
     async def load(self):
+        """
+        Load the body content.
+        """
         content = await self.__receive()
         self._raw_content = content["body"]
 
         while content.get("more_body"):
             content = await self.__receive()
             self._raw_content += content["body"]
 
@@ -53,12 +103,15 @@
             pass
 
         self.__json()
 
         self._form = Form(self)
 
     def __json(self) -> None:
+        """
+        Convert the body content to JSON.
+        """
         if self._content_type == "application/json":
             try:
                 self._json = json.loads(self._raw_content)
             except:
                 pass
```

### Comparing `fastipy-1.5.1/app/fastipy/src/types/routes.py` & `fastipy-1.5.2/app/fastipy/src/types/routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,8 +12,13 @@
 class RouteHookType(TypedDict):
     onRequest: NotRequired[List[FunctionType]]
     preHandler: NotRequired[List[FunctionType]]
     onResponse: NotRequired[List[FunctionType]]
     onError: NotRequired[List[FunctionType]]
 
 
+class PrintTreeOptionsType(TypedDict):
+    include_hooks: NotRequired[bool]
+    include_middlewares: NotRequired[bool]
+
+
 RouteMiddlewareType = List[FunctionType]
```

### Comparing `fastipy-1.5.1/app/fastipy.egg-info/PKG-INFO` & `fastipy-1.5.2/app/fastipy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastipy
-Version: 1.5.1
+Version: 1.5.2
 Summary: Fastipy is a fast and easy-to-use open source Python library for developing RESTful APIs. Inspired by the FastAPI and Fastify syntax and powered by uvicorn ASGI web server.
 Home-page: https://github.com/Bielgomes/Fastipy
 Author: Bielgomes
 Author-email: bielgomesdasilva@hotmail.com
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/Bielgomes/Fastipy/issues
 Classifier: Development Status :: 4 - Beta
@@ -51,31 +51,31 @@
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 # Routes can be async or sync functions, but reply send functions are async
 # The handler returns the default HTTP status code 200
-@app.get('/')
+@app.get("/")
 def home(req: Request, _):
   # Get query params age
-  age = req.query['age']
+  age = req.query["age"]
   # Example: Recovery all persons from database with this age and print the html
   print("<h1>Retrieving all persons</h1><ul><li>A Person</li></ul>")
 ```
 
 ### Example for GET Route with Params, CORS and multiple methods
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy().cors()
 
-@app.get('/user/:id')
-@app.post('/user/:id')
+@app.get("/user/:id")
+@app.post("/user/:id")
 async def getUser(req: Request, reply: Reply):
   # get users from database
   for i in users:
     if i["id"] == req.params["id"]:
       # All response functions are asynchronous
       return await reply.send(i)
 
@@ -85,43 +85,43 @@
 ### Example for POST Route with Body
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
-@app.post('/user')
+@app.post("/user")
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Save user in database
   await reply.code(201).send("Created")
 ```
 
 ### Example for PUT Route with Body
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
-@app.put('/user')
+@app.put("/user")
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Update user in database
   await reply.type("text/html").code(201).send("<h1>Created</h1>")
 ```
 
 ### Example for GET Route with file stream
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
-@app.get('/stream')
+@app.get("/stream")
 async def streamFile(_, reply: Reply):
   # It could be an asynchronous generator
   def generator():
     with open("file.txt") as f:
         for line in f:
             yield line
 
@@ -141,93 +141,112 @@
 )
 
 @app.get("/")
 async def customSerializer(_, reply: Reply):
     await reply.code(404).send("Field not found")
 ```
 
+### Running
+
+Running Fastipy application in development is easy
+
+```py
+import uvicorn
+
+if __name__ == "__main__":
+  # main:app indicates the FILE:VARIABLE
+
+  # The file is the main file where Fastipy() is instantiated
+  # The variable is the name of the variable that contains the instance of Fastipy()
+
+  # You can find more configurations here https://www.uvicorn.org/
+
+  # set reload to True for automatic reloading!
+  uvicorn.run("main:app", log_level="debug", port=8000, reload=True, loop="asyncio")
+```
+
 ### See more examples in **[examples](https://github.com/Bielgomes/Fastipy/tree/main/examples)** folder
 
 ## Creating plugins
 
 ```py
 # chat.py
 from fastipy import FastipyInstance, Reply
 
 # Plugins can be asynchronous or synchronized functions
 # Plugins have access to the main instance, which means they can use all of Fastipy's functions
 def chatRoutes(app: FastipyInstance, options: dict):
-  @app.get('/')
+  @app.get("/")
   async def index(_, reply: Reply):
     await reply.send_code(200)
 
-  @app.get('/chat')
+  @app.get("/chat")
   async def test(_, reply: Reply):
     await reply.send_code(200)
 ```
 
 ```py
 # message.py
 from fastipy import FastipyInstance, Reply
 
 async def messageRoutes(app: FastipyInstance, options: dict):
-  @message.get('/')
+  @message.get("/")
   async def index(_, reply: Reply):
     await reply.send_code(200)
 
-  @message.get('/message')
+  @message.get("/message")
   async def test(_, reply: Reply):
     await reply.send_code(200)
 
-  app.name('custom plugin name')
+  app.name("custom plugin name")
 ```
 
 ```py
 # main.py
 from fastipy import Fastipy
 
 from message import messageRoutes
 from chat import chatRoutes
 
 app = Fastipy().cors()
 
-app.register(messageRoutes, {'prefix': '/message'})
-app.register(chatRoutes, {'prefix': '/chat'})
+app.register(messageRoutes, {"prefix": "/message"})
+app.register(chatRoutes, {"prefix": "/chat"})
 ```
 
 ## Hooks
 
 ```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 # The preHandler hook is called before the request handler
-@app.hook('preHandler')
+@app.hook("preHandler")
 def preHandler(req: Request, reply: Reply):
-  print('onRequest hook')
+  print("onRequest hook")
 
 # The onRequest hook is called when the request is handled
-@app.hook('onRequest')
+@app.hook("onRequest")
 def onRequest(req: Request, reply: Reply):
-  print('onRequest hook')
+  print("onRequest hook")
 
 # The onResponse hook is called when the reply sends a response
-@app.hook('onResponse')
+@app.hook("onResponse")
 def onResponse(req: Request, reply: Reply):
-  print('onResponse hook')
+  print("onResponse hook")
 
 # The onError hook is called when an error occurs
-@app.hook('onError')
+@app.hook("onError")
 def onError(error: Exception, req: Request, reply: Reply):
-  print(f'onError hook exception: {error}')
+  print(f"onError hook exception: {error}")
 
 # A hook will only be linked to a route if its declaration precedes the route
 # The order of hooks of the same type is important
-@app.get('/')
+@app.get("/")
 async def index(_, reply: Reply):
   await reply.send_code(200)
 ```
 
 ## End to End tests
 
 ```py
@@ -238,56 +257,38 @@
 client = TestClient(app)
 
 response = client.post("/")
 assert response.status_code == 200
 assert response.text == "Hello World"
 ```
 
-## Running
-
-Running Fastipy application in development is easy
-
-```py
-import uvicorn
-
-if __name__ == "__main__":
-  # main:app indicates the FILE:VARIABLE
-
-  # The file is the main file where Fastipy() is instantiated
-  # The variable is the name of the variable that contains the instance of Fastipy()
-
-  # You can find more configurations here https://www.uvicorn.org/
-
-  config = uvicorn.Config('main:app', log_level='debug', port=3000)
-  server = uvicorn.Server(config)
-  server.run()
-```
-
 # Application Deploy
 
 For production deployment, please refer to this **[uvicorn guide](https://www.uvicorn.org/deployment/)**.
 
 # Change Log
 
-## Development Version 1.5.1
+## Version 1.5.2
 
 ### Added
 
-- [X] Added the possibility of printing middleware routes in the router's print tree.
-- [X] Added a customizable mail module.
-- [X] Added jinja2 lib to render templates.
-- [x] Add integration to end-to-end tests.
+- [x] Added Fastipy config.
+- [x] Added Plugin timeout configuration.
+- [x] Added typing for options in print routes function.
+- [x] Added types to request handler functions parameters.
+- [x] Added the option to automatically create folders when saving files.
+- [x] Added shortcut form property inside Request class to facilitate usability.
+- [x] Added documentation for most methods and classes.
 
 ### Changed
 
-- [X] Error imports are now centralized in the exceptions module.
-- [X] Improved error handling flow, now error handling hooks are executed first rather than the default error handling.
-- [X] Apply code reuse to generate logs.
-- [X] Refactored file stream in reply send file function.
-- [X] Reply send function now automatically serializes the value sent to it and sets a content type
+- [x] Renaming the fastipy base exception to the fastipy exception to make it easier to handle.
+- [x] Fixed problem in the error handler for python 3.11.
+- [x] Fixed the function of saving files securely, to save them in the correct path.
+- [x] Loading text and json from body files on demand.
 
 # Contributors
 
 <a href="https://github.com/Bielgomes/Fastipy/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=Bielgomes/Fastipy"/>
 </a>
```

### Comparing `fastipy-1.5.1/app/fastipy.egg-info/SOURCES.txt` & `fastipy-1.5.2/app/fastipy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,21 @@
 app/fastipy/src/core/reply.py
 app/fastipy/src/core/request.py
 app/fastipy/src/core/request_handler.py
 app/fastipy/src/exceptions/__init__.py
 app/fastipy/src/exceptions/decorator_already_exists_exception.py
 app/fastipy/src/exceptions/duplicate_route_exception.py
 app/fastipy/src/exceptions/exception_handler.py
-app/fastipy/src/exceptions/fastipy_base_exception.py
+app/fastipy/src/exceptions/fastipy_exception.py
 app/fastipy/src/exceptions/file_exception.py
 app/fastipy/src/exceptions/invalid_path_exception.py
 app/fastipy/src/exceptions/no_event_type.py
 app/fastipy/src/exceptions/no_hook_type.py
 app/fastipy/src/exceptions/no_http_method_exception.py
+app/fastipy/src/exceptions/plugin_exception.py
 app/fastipy/src/exceptions/reply_exception.py
 app/fastipy/src/helpers/__init__.py
 app/fastipy/src/helpers/async_sync_helpers.py
 app/fastipy/src/helpers/content_type.py
 app/fastipy/src/helpers/route_helpers.py
 app/fastipy/src/middlewares/__init__.py
 app/fastipy/src/middlewares/cors.py
@@ -47,9 +48,10 @@
 app/fastipy/src/models/body.py
 app/fastipy/src/models/file.py
 app/fastipy/src/models/form.py
 app/fastipy/src/routes/__init__.py
 app/fastipy/src/routes/plugin_tree.py
 app/fastipy/src/routes/router.py
 app/fastipy/src/types/__init__.py
+app/fastipy/src/types/fastipy.py
 app/fastipy/src/types/plugins.py
 app/fastipy/src/types/routes.py
```

### Comparing `fastipy-1.5.1/setup.py` & `fastipy-1.5.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="fastipy",
-    version="1.5.1",
+    version="1.5.2",
     description="Fastipy is a fast and easy-to-use open source Python library for developing RESTful APIs. Inspired by the FastAPI and Fastify syntax and powered by uvicorn ASGI web server.",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bielgomes/Fastipy",
     author="Bielgomes",
```

