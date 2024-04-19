# Comparing `tmp/happy_vllm-1.1.0.tar.gz` & `tmp/happy_vllm-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happy_vllm-1.1.0.tar", last modified: Mon Apr 15 09:37:02 2024, max compression
+gzip compressed data, was "happy_vllm-1.1.1.tar", last modified: Fri Apr 19 08:57:49 2024, max compression
```

## Comparing `happy_vllm-1.1.0.tar` & `happy_vllm-1.1.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.794080 happy_vllm-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-15 09:37:02.794080 happy_vllm-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:37:02.794080 happy_vllm-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.782080 happy_vllm-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.786080 happy_vllm-1.1.0/src/happy_vllm/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.786080 happy_vllm-1.1.0/src/happy_vllm/core/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/core/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.786080 happy_vllm-1.1.0/src/happy_vllm/logits_processors/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/logits_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/logits_processors/json_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/logits_processors/response_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/logits_processors/utils_parse_logits_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.786080 happy_vllm-1.1.0/src/happy_vllm/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/middlewares/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/src/happy_vllm/model/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/model/model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/model/openai_serving_chat_fixed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/src/happy_vllm/routers/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/examples/request.json
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/examples/response.json
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/schemas/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/routers/technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/src/happy_vllm/utils_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/src/happy_vllm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 09:37:02.000000 happy_vllm-1.1.0/src/happy_vllm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:37:02.790080 happy_vllm-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_json_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_model_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_response_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_routers_functionnal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_routers_technical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_schemas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_utils_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-15 09:36:58.000000 happy_vllm-1.1.0/tests/test_utils_parse_logits_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 09:37:00.000000 happy_vllm-1.1.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    31709 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.368431 happy_vllm-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/core/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/logits_processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/logits_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/logits_processors/json_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/logits_processors/response_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/logits_processors/utils_parse_logits_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/middlewares/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/model/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15713 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/model/openai_serving_chat_fixed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.372431 happy_vllm-1.1.1/src/happy_vllm/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16949 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/examples/request.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/examples/response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/schemas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/routers/technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/src/happy_vllm/utils_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/src/happy_vllm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 08:57:49.000000 happy_vllm-1.1.1/src/happy_vllm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:57:49.376431 happy_vllm-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_json_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_response_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_routers_functionnal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_routers_technical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_schemas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_utils_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-19 08:57:42.000000 happy_vllm-1.1.1/tests/test_utils_parse_logits_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 08:57:47.000000 happy_vllm-1.1.1/version.txt
```

### Comparing `happy_vllm-1.1.0/LICENSE` & `happy_vllm-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/PKG-INFO` & `happy_vllm-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happy_vllm
-Version: 1.1.0
+Version: 1.1.1
 Summary: happy_vllm is a REST API for vLLM, production ready
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: vllm<1.0,>=0.4.0
 Requires-Dist: fastapi<1.0,>=0.110.1
 Requires-Dist: pydantic_settings<3.0,>=2.2.1
```

### Comparing `happy_vllm-1.1.0/README.md` & `happy_vllm-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/pyproject.toml` & `happy_vllm-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/__init__.py` & `happy_vllm-1.1.1/src/happy_vllm/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/application.py` & `happy_vllm-1.1.1/src/happy_vllm/application.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/core/__init__.py` & `happy_vllm-1.1.1/src/happy_vllm/core/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/core/config.py` & `happy_vllm-1.1.1/src/happy_vllm/core/config.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/core/logtools.py` & `happy_vllm-1.1.1/src/happy_vllm/core/logtools.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/core/resources.py` & `happy_vllm-1.1.1/src/happy_vllm/core/resources.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/launch.py` & `happy_vllm-1.1.1/src/happy_vllm/launch.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/logits_processors/__init__.py` & `happy_vllm-1.1.1/src/happy_vllm/logits_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/logits_processors/json_format.py` & `happy_vllm-1.1.1/src/happy_vllm/logits_processors/json_format.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/logits_processors/response_pool.py` & `happy_vllm-1.1.1/src/happy_vllm/logits_processors/response_pool.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/logits_processors/utils_parse_logits_processors.py` & `happy_vllm-1.1.1/src/happy_vllm/logits_processors/utils_parse_logits_processors.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/middlewares/exception.py` & `happy_vllm-1.1.1/src/happy_vllm/middlewares/exception.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/model/__init__.py` & `happy_vllm-1.1.1/src/happy_vllm/model/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/model/model_base.py` & `happy_vllm-1.1.1/src/happy_vllm/model/model_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,18 +247,18 @@
 
     def __init__(self, tokenizer, app_name: str = "happy_vllm"):
         self.tokenizer = tokenizer
         self.app_name = app_name
 
     async def generate(self, prompt, sampling_params, request_id):
         stream_txts = [f"n={i} "*i + prompt + " This is the generated text. I find it really good don't you ?" for i in range(sampling_params.n)]
-        stream_ids = [self.tokenizer(stream_txt, add_special_tokens=False, truncation=True, max_length=sampling_params.max_tokens)['input_ids'] for stream_txt in stream_txts]
+        stream_ids = [self.tokenizer(stream_txt, truncation=True, max_length=sampling_params.max_tokens)['input_ids'] for stream_txt in stream_txts]
         max_length = max([len(element) for element in stream_ids]) + 1
-        stream_tmp = [[self.tokenizer.decode(text[:i]) for text in stream_ids] for i in range(max_length)]
-        stream = [MockGenerateResponse(prompt, texts) for texts in stream_tmp]
+        stream_tmp = [[self.tokenizer.decode(text[:i], skip_special_tokens=True) for text in stream_ids] for i in range(max_length)]
+        stream = [MockGenerateResponse(prompt, texts, self.tokenizer) for texts in stream_tmp]
         # Mock the length finish_reason
         for i in range(sampling_params.n):
             if stream[-1].outputs[i].finish_reason is None:
                 stream[-1].outputs[i].finish_reason = "length"
         stream = self.async_iter(stream)
         async for outputs in stream:
             yield outputs
@@ -266,23 +266,25 @@
     async def async_iter(self, my_list):
         for element in my_list:
             yield element
 
 
 class MockGenerateResponse():
 
-    def __init__(self, prompt, outputs):
+    def __init__(self, prompt, outputs, tokenizer):
         self.prompt = prompt
-        outputs = [MockOutput(output) for output in outputs]
+        outputs = [MockOutput(output, tokenizer) for output in outputs]
         self.outputs = outputs
+        self.prompt_token_ids = tokenizer(self.prompt)['input_ids']
 
 
 class MockOutput():
     
-    def __init__(self, text):
+    def __init__(self, text, tokenizer):
         self.text = text
+        self.token_ids = tokenizer(text)['input_ids']
         if text[-len("don't you ?"):] == "don't you ?":
             self.finish_reason = "stop"
         else:
             self.finish_reason = None
```

### Comparing `happy_vllm-1.1.0/src/happy_vllm/model/openai_serving_chat_fixed.py` & `happy_vllm-1.1.1/src/happy_vllm/model/openai_serving_chat_fixed.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/routers/__init__.py` & `happy_vllm-1.1.1/src/happy_vllm/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/routers/functional.py` & `happy_vllm-1.1.1/src/happy_vllm/routers/functional.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,17 +152,22 @@
             return Response(status_code=499)
         final_output = request_output
 
     if final_output is None:
         raise ValueError('The final ouput is None')
     prompt = final_output.prompt
     text_outputs = [output.text for output in final_output.outputs]
+    prompt_nb_tokens = len(final_output.prompt_token_ids)
+    nb_tokens_outputs = [len(output.token_ids) for output in final_output.outputs]
+    usages = [{"prompt_tokens": prompt_nb_tokens,
+               "completion_tokens": completion_tokens,
+               "total_tokens": prompt_nb_tokens + completion_tokens } for completion_tokens in nb_tokens_outputs]
     finish_reasons = [output.finish_reason for output in request_output.outputs]
     finish_reasons = ["None" if finish_reason is None else finish_reason for finish_reason in finish_reasons]
-    ret = {"responses": text_outputs, "finish_reasons": finish_reasons}
+    ret = {"responses": text_outputs, "finish_reasons": finish_reasons, "usages": usages}
     if prompt_in_response:
         ret['prompt'] = prompt
     return JSONResponse(ret)
 
 
 @router.post("/v1/generate_stream", response_model=functional_schema.ResponseGenerate)
 async def generate_stream(request: Request,
@@ -187,15 +192,20 @@
         async for request_output in results_generator:
             prompt = request_output.prompt
             text_outputs = [
                 output.text for output in request_output.outputs
             ]
             finish_reasons = [output.finish_reason for output in request_output.outputs]
             finish_reasons = ["None" if finish_reason is None else finish_reason for finish_reason in finish_reasons]
-            ret = {"responses": text_outputs, "finish_reasons": finish_reasons}
+            prompt_nb_tokens = len(request_output.prompt_token_ids)
+            nb_tokens_outputs = [len(output.token_ids) for output in request_output.outputs]
+            usages = [{"prompt_tokens": prompt_nb_tokens,
+                    "completion_tokens": completion_tokens,
+                    "total_tokens": prompt_nb_tokens + completion_tokens } for completion_tokens in nb_tokens_outputs]
+            ret = {"responses": text_outputs, "finish_reasons": finish_reasons, "usages": usages}
             if prompt_in_response:
                 ret['prompt'] = prompt
             yield (json.dumps(ret) + "\n")#.encode("utf-8")
 
     return StreamingResponse(stream_results())
```

### Comparing `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/__init__.py` & `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/examples/request.json` & `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/examples/request.json`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/examples/response.json` & `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/examples/response.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692307%*

 * *Differences: {"'generate'": "{'usages': [OrderedDict([('prompt_tokens', 17), ('completion_tokens', 17), "*

 * *               "('total_tokens', 34)])]}",*

 * * "'generate_stream'": "{'usages': [OrderedDict([('prompt_tokens', 17), ('completion_tokens', 17), "*

 * *                      "('total_tokens', 34)])]}"}*

```diff
@@ -57,23 +57,37 @@
     "generate": {
         "finish_reasons": [
             "stop"
         ],
         "prompt": "This is a prompt example. Please complete it with a joke. JOKE:",
         "responses": [
             "Why don't scientists trust atoms? \n Because they make up everything!"
+        ],
+        "usages": [
+            {
+                "completion_tokens": 17,
+                "prompt_tokens": 17,
+                "total_tokens": 34
+            }
         ]
     },
     "generate_stream": {
         "finish_reasons": [
             "stop"
         ],
         "prompt": "This is a prompt example. Please complete it with a joke. JOKE:",
         "responses": [
             "Why don't scientists trust atoms? \n Because they make up everything!"
+        ],
+        "usages": [
+            {
+                "completion_tokens": 17,
+                "prompt_tokens": 17,
+                "total_tokens": 34
+            }
         ]
     },
     "information": {
         "application": "happy_vllm",
         "max_length": 32768,
         "model_name": "my_model",
         "truncation_side": "right",
```

### Comparing `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/functional.py` & `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/functional.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/technical.py` & `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/technical.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/routers/schemas/utils.py` & `happy_vllm-1.1.1/src/happy_vllm/routers/schemas/utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/routers/technical.py` & `happy_vllm-1.1.1/src/happy_vllm/routers/technical.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/utils.py` & `happy_vllm-1.1.1/src/happy_vllm/utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm/utils_args.py` & `happy_vllm-1.1.1/src/happy_vllm/utils_args.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/src/happy_vllm.egg-info/PKG-INFO` & `happy_vllm-1.1.1/src/happy_vllm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happy_vllm
-Version: 1.1.0
+Version: 1.1.1
 Summary: happy_vllm is a REST API for vLLM, production ready
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: vllm<1.0,>=0.4.0
 Requires-Dist: fastapi<1.0,>=0.110.1
 Requires-Dist: pydantic_settings<3.0,>=2.2.1
```

### Comparing `happy_vllm-1.1.0/src/happy_vllm.egg-info/SOURCES.txt` & `happy_vllm-1.1.1/src/happy_vllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/tests/test_json_format.py` & `happy_vllm-1.1.1/tests/test_json_format.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/tests/test_model_base.py` & `happy_vllm-1.1.1/tests/test_model_base.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/tests/test_response_pool.py` & `happy_vllm-1.1.1/tests/test_response_pool.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/tests/test_routers_functionnal.py` & `happy_vllm-1.1.1/tests/test_routers_functionnal.py`

 * *Files 5% similar despite different names*

```diff
@@ -170,83 +170,101 @@
 def test_generate(test_complete_client: TestClient):
     """Test the route /v1/generate thanks to the test_complete_client we created in conftest.py"""
     model = init_model()
     tokenizer = model._tokenizer
 
     def get_response(tokenizer, prompt, i, max_tokens):
         prompt_tot = f"n={i} "*i + prompt + " This is the generated text. I find it really good don't you ?"
-        token_ids = tokenizer(prompt_tot, add_special_tokens=False)['input_ids']
+        token_ids = tokenizer(prompt_tot)['input_ids']
         token_ids = token_ids[:max_tokens]
-        return tokenizer.decode(token_ids)
+        return tokenizer.decode(token_ids, skip_special_tokens=True), len(token_ids)
     
     # Nominal case
     max_tokens = 500
     prompt = "Hey"
     body = {"prompt": prompt, "max_tokens": max_tokens}
     response = test_complete_client.post("/tests/v1/generate", json=body)
     assert response.status_code == 200
     response_json = response.json()
-    assert response_json["responses"] == [get_response(tokenizer, prompt, 0, max_tokens)]
+    nb_token_prompt = len(tokenizer(prompt)['input_ids'])
+    response, completion_tokens = get_response(tokenizer, prompt, 0, max_tokens)
+    assert response_json["responses"] == [response]
     assert response_json["finish_reasons"] == ["stop"]
-    assert set(response_json) == {"responses", "finish_reasons"}
+    assert response_json["usages"] == [{"prompt_tokens": nb_token_prompt,
+                                        "completion_tokens": completion_tokens,
+                                        "total_tokens": nb_token_prompt + completion_tokens }]
+    assert set(response_json) == {"responses", "finish_reasons", "usages"}
 
     # Several responses and prompt_in_response
     max_tokens = 500
     prompt = "Hello there"
     body = {"prompt": prompt, "max_tokens": max_tokens, "n": 3, "prompt_in_response": True}
     response = test_complete_client.post("/tests/v1/generate", json=body)
     assert response.status_code == 200
     response_json = response.json()
+    nb_token_prompt = len(tokenizer(prompt)['input_ids'])
     assert len(response_json["responses"]) == 3
     assert len(response_json["finish_reasons"]) == 3
+    assert len(response_json["usages"]) == 3
     for i in [0, 1, 2]:
-        target_response = get_response(tokenizer, prompt, i, max_tokens)
+        target_response, target_completion_tokens = get_response(tokenizer, prompt, i, max_tokens)
         assert response_json["responses"][i] == target_response
         if target_response[-4:] == "ou ?":
             assert response_json["finish_reasons"][i] == "stop"
         else:
             assert response_json["finish_reasons"][i] == "length"
+        assert response_json["usages"][i] == {"prompt_tokens": nb_token_prompt,
+                                        "completion_tokens": target_completion_tokens,
+                                        "total_tokens": nb_token_prompt + target_completion_tokens } 
     assert response_json["prompt"] == "Hello there"
-    assert set(response_json) == {"responses", "finish_reasons", "prompt"}
+    assert set(response_json) == {"responses", "finish_reasons", "prompt", "usages"}
 
     # Generations stopped
     max_tokens = 5
     prompt = "Hey"
     body = {"prompt": prompt, "max_tokens": max_tokens, "n": 3}
     response = test_complete_client.post("/tests/v1/generate", json=body)
     assert response.status_code == 200
     response_json = response.json()
+    nb_token_prompt = len(tokenizer(prompt)['input_ids'])
     assert len(response_json["responses"]) == 3
     assert len(response_json["finish_reasons"]) == 3
     for i in [0, 1, 2]:
-        target_response = get_response(tokenizer, prompt, i, max_tokens)
+        target_response, target_completion_tokens = get_response(tokenizer, prompt, i, max_tokens)
         assert response_json["responses"][i] == target_response
         if target_response[-4:] == "ou ?":
             assert response_json["finish_reasons"][i] == "stop"
         else:
             assert response_json["finish_reasons"][i] == "length"
-    assert set(response_json) == {"responses", "finish_reasons"}
+        assert response_json["usages"][i] == {"prompt_tokens": nb_token_prompt,
+                                        "completion_tokens": target_completion_tokens,
+                                        "total_tokens": nb_token_prompt + target_completion_tokens } 
+    assert set(response_json) == {"responses", "finish_reasons", "usages"}
 
     # Some Generation stopped
     max_tokens = 18
     prompt = "Hey"
     body = {"prompt": prompt, "max_tokens": max_tokens, "n": 3}
     response = test_complete_client.post("/tests/v1/generate", json=body)
     assert response.status_code == 200
     response_json = response.json()
+    nb_token_prompt = len(tokenizer(prompt)['input_ids'])
     assert len(response_json["responses"]) == 3
     assert len(response_json["finish_reasons"]) == 3
     for i in [0, 1, 2]:
-        target_response = get_response(tokenizer, prompt, i, max_tokens)
+        target_response, target_completion_tokens = get_response(tokenizer, prompt, i, max_tokens)
         assert response_json["responses"][i] == target_response
         if target_response[-4:] == "ou ?":
             assert response_json["finish_reasons"][i] == "stop"
         else:
             assert response_json["finish_reasons"][i] == "length"
-    assert set(response_json) == {"responses", "finish_reasons"}
+        assert response_json["usages"][i] == {"prompt_tokens": nb_token_prompt,
+                                        "completion_tokens": target_completion_tokens,
+                                        "total_tokens": nb_token_prompt + target_completion_tokens } 
+    assert set(response_json) == {"responses", "finish_reasons", "usages"}
 
 
 def test_tokenizer(test_complete_client: TestClient):
     """Test the functional route /v1/tokenizer"""
     model = init_model()
     # Vanilla
     for text in ["How do you do?", "I am Lliam. How are you ?", "Marvelous, it works !"]:
```

### Comparing `happy_vllm-1.1.0/tests/test_routers_technical.py` & `happy_vllm-1.1.1/tests/test_routers_technical.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/tests/test_schemas_utils.py` & `happy_vllm-1.1.1/tests/test_schemas_utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/tests/test_utils.py` & `happy_vllm-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/tests/test_utils_args.py` & `happy_vllm-1.1.1/tests/test_utils_args.py`

 * *Files identical despite different names*

### Comparing `happy_vllm-1.1.0/tests/test_utils_parse_logits_processors.py` & `happy_vllm-1.1.1/tests/test_utils_parse_logits_processors.py`

 * *Files identical despite different names*

