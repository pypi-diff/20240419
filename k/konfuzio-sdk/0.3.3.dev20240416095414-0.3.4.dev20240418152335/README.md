# Comparing `tmp/konfuzio_sdk-0.3.3.dev20240416095414.tar.gz` & `tmp/konfuzio_sdk-0.3.4.dev20240418152335.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konfuzio_sdk-0.3.3.dev20240416095414.tar", last modified: Wed Apr 17 03:25:41 2024, max compression
+gzip compressed data, was "konfuzio_sdk-0.3.4.dev20240418152335.tar", last modified: Fri Apr 19 03:26:53 2024, max compression
```

## Comparing `konfuzio_sdk-0.3.3.dev20240416095414.tar` & `konfuzio_sdk-0.3.4.dev20240418152335.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.272364 konfuzio_sdk-0.3.3.dev20240416095414/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 03:25:30.000000 konfuzio_sdk-0.3.3.dev20240416095414/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-17 03:25:41.272364 konfuzio_sdk-0.3.3.dev20240416095414/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-17 03:25:30.000000 konfuzio_sdk-0.3.3.dev20240416095414/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.260363 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33726 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   202907 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/settings_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.264364 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.264364 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/document_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/file_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/image.py
--rw-r--r--   0 runner    (1001) docker     (127)   101643 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/information_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.268364 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 03:25:41.000000 konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 03:25:41.272364 konfuzio_sdk-0.3.3.dev20240416095414/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:25:41.268364 konfuzio_sdk-0.3.3.dev20240416095414/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22568 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   167058 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-17 03:25:31.000000 konfuzio_sdk-0.3.3.dev20240416095414/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.628459 konfuzio_sdk-0.3.4.dev20240418152335/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-19 03:26:53.628459 konfuzio_sdk-0.3.4.dev20240418152335/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.620459 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   202907 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/settings_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.620459 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.624459 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/document_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/file_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101643 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/information_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.624459 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 03:26:53.000000 konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:26:53.628459 konfuzio_sdk-0.3.4.dev20240418152335/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:26:53.624459 konfuzio_sdk-0.3.4.dev20240418152335/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22568 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167058 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-19 03:26:44.000000 konfuzio_sdk-0.3.4.dev20240418152335/tests/test_utils.py
```

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/LICENSE.md` & `konfuzio_sdk-0.3.4.dev20240418152335/LICENSE.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/PKG-INFO` & `konfuzio_sdk-0.3.4.dev20240418152335/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.3.dev20240416095414
+Version: 0.3.4.dev20240418152335
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/README.md` & `konfuzio_sdk-0.3.4.dev20240418152335/README.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/api.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -828,16 +828,15 @@
 
 
 def delete_ai_model(ai_model_id: int, ai_type: str, session=None):
     """
     Delete an AI model from the server.
 
     :param ai_model_id: an ID of the model to be deleted.
-    :param ai_type: if a model is an Extraction AI, a Categorization AI or a File Splitting AI. Should be one of the
-    following: 'filesplitting', 'extraction', 'categorization'.
+    :param ai_type: Should be one of the following: 'filesplitting', 'extraction', 'categorization'.
     :param session: session to connect to the server.
     :raises: ValueError if ai_type is not correctly specified.
     :raises: ConnectionError when a request is unsuccessful.
     """
     if session is None:
         session = konfuzio_session()
     if ai_type not in AI_TYPES:
@@ -853,16 +852,15 @@
 
 
 def update_ai_model(ai_model_id: int, ai_type: str, patch: bool = True, session=None, **kwargs):
     """
     Update an AI model from the server.
 
     :param ai_model_id: an ID of the model to be updated.
-    :param ai_type: if a model is an Extraction AI, a Categorization AI or a File Splitting AI. Should be one of the
-    following: 'filesplitting', 'extraction', 'categorization'.
+    :param ai_type: Should be one of the following: 'filesplitting', 'extraction', 'categorization'.
     :param patch: If true, adds info instead of replacing it.
     :param session: session to connect to the server.
     :raises: ValueError if ai_type is not correctly specified.
     :raises: HTTPError when a request is unsuccessful.
     """
     if session is None:
         session = konfuzio_session()
```

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/cli.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/data.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/evaluate.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/extras.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/normalize.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/regex.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/samples.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/settings_importer.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/settings_importer.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/base.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/paragraph_and_sentence.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/paragraph_and_sentence.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/tokenizer/regex.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/tokenizer/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/base.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,17 +175,19 @@
 
         We then compress the pickle file using shutil.copyfileobject which writes in chunks to avoid loading the entire
         pickle file in memory.
 
         Finally, we delete the cloudpickle file and are left with the compressed pickle file which has a .pkl.lz4 or
         .pkl.bz2 extension.
 
+        For more info on pickle serialization and including dependencies read
+        https://github.com/cloudpipe/cloudpickle#overriding-pickles-serialization-mechanism-for-importable-constructs
+
         :param output_dir: Folder to save AI model in. If None, the default Project folder is used.
-        :param include_konfuzio: Enables pickle serialization as a value, not as a reference (for more info, read
-        https://github.com/cloudpipe/cloudpickle#overriding-pickles-serialization-mechanism-for-importable-constructs).
+        :param include_konfuzio: Enables pickle serialization as a value, not as a reference.
         :param reduce_weight: Remove all non-strictly necessary parameters before saving.
         :param compression: Compression algorithm to use. Default is lz4, bz2 is also supported.
         :param max_ram: Specify maximum memory usage condition to save model.
         :raises MemoryError: When the size of the model in memory is greater than the maximum value.
         :return: Path of the saved model file.
         """
         logger.info('Saving model')
```

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/document_categorization.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/document_categorization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/file_splitting.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/file_splitting.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/image.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/image.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/information_extraction.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/information_extraction.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/tokenization.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/tokenization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/trainer/utils.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/urls.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk/utils.py` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/PKG-INFO` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.3.dev20240416095414
+Version: 0.3.4.dev20240418152335
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/SOURCES.txt` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/konfuzio_sdk.egg-info/requires.txt` & `konfuzio_sdk-0.3.4.dev20240418152335/konfuzio_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/setup.py` & `konfuzio_sdk-0.3.4.dev20240418152335/setup.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_api.py` & `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_cli.py` & `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_data.py` & `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_evaluate.py` & `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_extras.py` & `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_normalize.py` & `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_regex.py` & `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_samples.py` & `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_urls.py` & `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.3.dev20240416095414/tests/test_utils.py` & `konfuzio_sdk-0.3.4.dev20240418152335/tests/test_utils.py`

 * *Files identical despite different names*

