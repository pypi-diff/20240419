# Comparing `tmp/spacy-curated-transformers-2.0.0.dev0.tar.gz` & `tmp/spacy-curated-transformers-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-curated-transformers-2.0.0.dev0.tar", last modified: Wed Apr 10 14:57:48 2024, max compression
+gzip compressed data, was "spacy-curated-transformers-2.0.0.dev1.tar", last modified: Fri Apr 12 14:13:33 2024, max compression
```

## Comparing `spacy-curated-transformers-2.0.0.dev0.tar` & `spacy-curated-transformers-2.0.0.dev1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.824855 spacy-curated-transformers-2.0.0.dev0/
--rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     2810 2024-04-10 14:57:48.824855 spacy-curated-transformers-2.0.0.dev0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     5236 2024-04-10 14:57:48.824855 spacy-curated-transformers-2.0.0.dev0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      210 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.812855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      570 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.816855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4113 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/cli/debug_pieces.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18116 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/cli/fill_config_transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.816855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (127)      633 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    45883 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25094 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/listeners.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3784 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/output.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4016 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/pooling.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.816855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/pytorch/
--rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/pytorch/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2516 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/pytorch/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2384 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/remove_eos_bos.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4830 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2665 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/types.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7876 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10513 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.816855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17826 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/pipeline/transformer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/schedules.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.820855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2341 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)       45 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.820855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3352 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_hf_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2653 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_listeners.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4556 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_pooling.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1425 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6351 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3195 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4326 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.820855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26511 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/pipeline/test_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2703 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
--rw-r--r--   0 vsts      (1001) docker     (127)    10074 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3106 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (127)      501 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/test_schedules.py
--rw-r--r--   0 vsts      (1001) docker     (127)      794 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/test_torchscript_wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.820855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3411 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4116 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/test_char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2716 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7953 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4908 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)      138 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/toy-chars.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     4690 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    14493 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (127)   253270 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/toy.model
--rw-r--r--   0 vsts      (1001) docker     (127)     4968 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (127)      906 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.824855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (127)      568 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3745 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6014 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2483 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/sentencepiece_adapters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3807 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/types.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5880 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3036 2024-04-10 14:57:41.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 14:57:48.824855 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2810 2024-04-10 14:57:48.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3676 2024-04-10 14:57:48.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 14:57:48.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     4375 2024-04-10 14:57:48.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-04-10 14:57:48.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-04-10 14:57:48.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 14:57:48.000000 spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/zip-safe
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.648449 spacy-curated-transformers-2.0.0.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      107 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     2815 2024-04-12 14:13:33.648449 spacy-curated-transformers-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     5241 2024-04-12 14:13:33.648449 spacy-curated-transformers-2.0.0.dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      210 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.640449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      570 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.640449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4113 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/cli/debug_pieces.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18116 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/cli/fill_config_transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.644449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)      633 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46285 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      931 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25094 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3784 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/output.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4016 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/pooling.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.644449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/pytorch/
+-rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/pytorch/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2516 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/pytorch/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2384 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/remove_eos_bos.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4830 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2665 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7876 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10513 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.644449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17826 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/pipeline/transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1586 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/schedules.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.644449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2315 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       45 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.644449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3352 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_hf_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2653 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4556 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1425 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7519 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3195 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4326 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.644449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26511 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/pipeline/test_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2703 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
+-rw-r--r--   0 vsts      (1001) docker     (127)    10074 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3106 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      501 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/test_schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      794 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/test_torchscript_wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.648449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3411 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4116 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/test_char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2716 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7953 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4908 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      138 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/toy-chars.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     4690 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    14493 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (127)   253270 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (127)     4968 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (127)      906 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.648449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (127)      568 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3745 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6014 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2483 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/sentencepiece_adapters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3807 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      556 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5880 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3036 2024-04-12 14:13:26.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 14:13:33.648449 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2815 2024-04-12 14:13:33.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3676 2024-04-12 14:13:33.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 14:13:33.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     4375 2024-04-12 14:13:33.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-04-12 14:13:33.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-04-12 14:13:33.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 14:13:33.000000 spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/zip-safe
```

### Comparing `spacy-curated-transformers-2.0.0.dev0/LICENSE` & `spacy-curated-transformers-2.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/PKG-INFO` & `spacy-curated-transformers-2.0.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spacy-curated-transformers
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: Curated transformer models for spaCy pipelines
 Home-page: https://github.com/explosion/spacy-curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: curated-transformers<3.0.0,>=2.0.0.dev2
-Requires-Dist: curated-tokenizers<1.0.0,>=0.9.2
+Requires-Dist: curated-transformers<3.0.0,>=2.0.0.dev3
+Requires-Dist: curated-tokenizers<3.0.0,>=2.0.0.dev0
 Requires-Dist: fsspec>=2023.5.0
 Requires-Dist: spacy<5.0.0,>=4.0.0.dev2
 Requires-Dist: thinc<9.1.0,>=9.0.0.dev4
 Requires-Dist: torch>=1.12.0
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: spacy-curated-transformers Version: 2.0.0.dev0
+Metadata-Version: 2.1 Name: spacy-curated-transformers Version: 2.0.0.dev1
 Summary: Curated transformer models for spaCy pipelines Home-page: https://
 github.com/explosion/spacy-curated-transformers Author: Explosion Author-email:
 contact@explosion.ai License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: curated-
-transformers<3.0.0,>=2.0.0.dev2 Requires-Dist: curated-tokenizers<1.0.0,>=0.9.2
-Requires-Dist: fsspec>=2023.5.0 Requires-Dist: spacy<5.0.0,>=4.0.0.dev2
-Requires-Dist: thinc<9.1.0,>=9.0.0.dev4 Requires-Dist: torch>=1.12.0 _[_h_t_t_p_s_:_/_/
-_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/_l_o_g_o_._s_v_g_]# ð« ð¤ spaCy Curated Transformers This
-package provides [spaCy](https://github.com/explosion/spaCy) components and
-architectures to use a curated set of transformer models via [`curated-
-transformers`](https://github.com/explosion/curated-transformers) in spaCy. [!
-[PyPi](https://img.shields.io/pypi/v/spacy-curated-transformers.svg?style=flat-
-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-curated-
-transformers) [![GitHub](https://img.shields.io/github/release/explosion/spacy-
-curated-transformers/all.svg?style=flat-square&logo=github)](https://
-github.com/explosion/spacy-curated-transformers/releases) ## Features - Use
-pretrained models based on one of the following architectures to power your
-spaCy pipeline: - ALBERT - BERT - CamemBERT - RoBERTa - XLM-RoBERTa - All the
-nice features supported by [`spacy-transformers`](https://github.com/explosion/
-spacy-transformers) such as support for Hugging Face Hub, **multi-task
-learning**, the extensible config system and out-of-the-box serialization -
-Deep integration into spaCy, which lays the groundwork for deployment-focused
-features such as distillation and quantization - Minimal dependencies ## â³
-Installation Installing the package from pip will automatically install all
-dependencies. ```bash pip install spacy-curated-transformers ``` ## ð
-Quickstart An example project is provided in the [`project`](project)
-directory. ## ð Documentation - ð [Layers and Model Architectures](https:
-//spacy.io/usage/layers-architectures): Power spaCy components with custom
-neural networks - ð [`CuratedTransformer`](https://spacy.io/api/
-curatedtransformer): Pipeline component API reference - ð [Transformer
-architectures](https://spacy.io/api/architectures#curated-trf): Architectures
-and registered functions ## Bug reports and other issues Please use [spaCy's
-issue tracker](https://github.com/explosion/spaCy/issues) to report a bug, or
-open a new thread on the [discussion board](https://github.com/explosion/spaCy/
-discussions) for any other issue.
+transformers<3.0.0,>=2.0.0.dev3 Requires-Dist: curated-
+tokenizers<3.0.0,>=2.0.0.dev0 Requires-Dist: fsspec>=2023.5.0 Requires-Dist:
+spacy<5.0.0,>=4.0.0.dev2 Requires-Dist: thinc<9.1.0,>=9.0.0.dev4 Requires-Dist:
+torch>=1.12.0 _[_h_t_t_p_s_:_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/_l_o_g_o_._s_v_g_]# ð« ð¤ spaCy
+Curated Transformers This package provides [spaCy](https://github.com/
+explosion/spaCy) components and architectures to use a curated set of
+transformer models via [`curated-transformers`](https://github.com/explosion/
+curated-transformers) in spaCy. [![PyPi](https://img.shields.io/pypi/v/spacy-
+curated-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://
+pypi.python.org/pypi/spacy-curated-transformers) [![GitHub](https://
+img.shields.io/github/release/explosion/spacy-curated-transformers/
+all.svg?style=flat-square&logo=github)](https://github.com/explosion/spacy-
+curated-transformers/releases) ## Features - Use pretrained models based on one
+of the following architectures to power your spaCy pipeline: - ALBERT - BERT -
+CamemBERT - RoBERTa - XLM-RoBERTa - All the nice features supported by [`spacy-
+transformers`](https://github.com/explosion/spacy-transformers) such as support
+for Hugging Face Hub, **multi-task learning**, the extensible config system and
+out-of-the-box serialization - Deep integration into spaCy, which lays the
+groundwork for deployment-focused features such as distillation and
+quantization - Minimal dependencies ## â³ Installation Installing the package
+from pip will automatically install all dependencies. ```bash pip install
+spacy-curated-transformers ``` ## ð Quickstart An example project is
+provided in the [`project`](project) directory. ## ð Documentation - ð
+[Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
+Power spaCy components with custom neural networks - ð
+[`CuratedTransformer`](https://spacy.io/api/curatedtransformer): Pipeline
+component API reference - ð [Transformer architectures](https://spacy.io/
+api/architectures#curated-trf): Architectures and registered functions ## Bug
+reports and other issues Please use [spaCy's issue tracker](https://github.com/
+explosion/spaCy/issues) to report a bug, or open a new thread on the
+[discussion board](https://github.com/explosion/spaCy/discussions) for any
+other issue.
```

### Comparing `spacy-curated-transformers-2.0.0.dev0/README.md` & `spacy-curated-transformers-2.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/setup.cfg` & `spacy-curated-transformers-2.0.0.dev1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
-version = 2.0.0.dev0
+version = 2.0.0.dev1
 description = Curated transformer models for spaCy pipelines
 url = https://github.com/explosion/spacy-curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 zip_safe = true
 include_package_data = true
 python_requires = >=3.9
 install_requires = 
-	curated-transformers>=2.0.0.dev2,<3.0.0
-	curated-tokenizers>=0.9.2,<1.0.0
+	curated-transformers>=2.0.0.dev3,<3.0.0
+	curated-tokenizers>=2.0.0.dev0,<3.0.0
 	fsspec>=2023.5.0
 	spacy>=4.0.0.dev2,<5.0.0
 	thinc>=9.0.0.dev4,<9.1.0
 	torch>=1.12.0
 
 [options.entry_points]
 spacy_factories =
```

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/_compat.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/cli/debug_pieces.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/cli/debug_pieces.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/cli/fill_config_transformer.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/cli/fill_config_transformer.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/__init__.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/architectures.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/architectures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, List, Optional, Tuple, Union, cast
 
 import torch
+import torch.nn as nn
 from curated_transformers.layers import Activation, AttentionMask
 from curated_transformers.models import (
     ALBERTConfig,
     ALBERTEncoder,
     BERTConfig,
     BERTEncoder,
     CamemBERTEncoder,
@@ -1177,15 +1178,15 @@
         # Create a new, mutable dict instance.
         grad_scaler_config = {}
 
     if "enabled" not in grad_scaler_config:
         grad_scaler_config["enabled"] = mixed_precision
 
     model = PyTorchWrapper_v2(
-        encoder,
+        _EncoderWrapper(encoder),
         convert_inputs=partial(
             _convert_inputs,
             max_model_seq_len=model_max_length,
             padding_idx=padding_idx,
         ),
         convert_outputs=_convert_outputs,
         mixed_precision=mixed_precision,
@@ -1307,21 +1308,34 @@
 
     path (Path):
         Path to the directory containing the checkpoint.
     """
 
     def load(model, X=None, Y=None):
         device = get_torch_default_device()
-        encoder = model.shims[0]._model
+        encoder = model.shims[0]._model.curated_encoder
         assert isinstance(encoder, FromHFHub)
         fs = LocalFileSystem()
         encoder.from_fsspec_(fs=fs, model_path=path, device=device)
         return model
 
     return load
 
 
 def _torch_dtype_from_str(dtype_as_str: str):
     dtype = getattr(torch, dtype_as_str, None)
     if not isinstance(dtype, torch.dtype):
         raise ValueError(f"Invalid torch dtype `{dtype_as_str}`")
     return dtype
+
+
+class _EncoderWrapper(nn.Module):
+    """Small wrapper to add a prefix that can be used by eg. learning rate
+    schedules.
+    """
+
+    def __init__(self, encoder: nn.Module):
+        super().__init__()
+        self.curated_encoder = encoder
+
+    def forward(self, *args, **kwargs):
+        return self.curated_encoder.forward(*args, **kwargs)
```

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/hf_loader.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/hf_loader.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,14 @@
     name (str):
         Name of the HuggingFace model.
     revision (str):
         Name of the model revision/branch.
     """
 
     def load(model, X=None, Y=None):
-        encoder = model.shims[0]._model
+        encoder = model.shims[0]._model.curated_encoder
         assert isinstance(encoder, FromHFHub)
         device = model.shims[0].device
         encoder.from_hf_hub_(name=name, revision=revision, device=device)
         return model
 
     return load
```

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/listeners.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/listeners.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/output.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/output.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/pooling.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/pooling.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/pytorch/scalar_weight.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/pytorch/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/remove_eos_bos.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/remove_eos_bos.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/scalar_weight.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/types.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/types.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/with_non_ws_tokens.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/models/with_strided_spans.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/models/with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/pipeline/transformer.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/pipeline/transformer.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/schedules.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/schedules.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/conftest.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     for opt in ["slow"]:
         if opt in item.keywords and not getopt(opt):
             pytest.skip(f"need --{opt} option to run")
 
 
 @pytest.fixture
 def test_dir(request):
-    print(request.fspath)
     return Path(request.fspath).parent
 
 
 @pytest.fixture
 def sample_docs_with_spaces():
     nlp = spacy.blank("en")
     doc1 = nlp.make_doc("I saw a girl    with a telescope.")
```

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_hf_model.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_hf_model.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_listeners.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_listeners.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_pooling.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_pooling.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_scalar_weight.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_scalar_weight.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_transformer_model.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_transformer_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -174,7 +174,48 @@
     model = model_factory(
         piece_encoder=piece_encoder, vocab_size=vocab_size, with_spans=with_spans
     )
     model.get_ref("transformer").init = registry.model_loaders.get(
         "spacy-curated-transformers.PyTorchCheckpointLoader.v1"
     )(path=Path(checkpoint_path))
     model.initialize()
+
+
+@pytest.mark.parametrize(
+    "test_config",
+    [
+        (
+            build_albert_transformer_model_v1,
+            build_sentencepiece_encoder_v1(),
+            1000,
+        ),
+        (
+            build_bert_transformer_model_v1,
+            build_bert_wordpiece_encoder_v1(),
+            1000,
+        ),
+        (
+            build_roberta_transformer_model_v1,
+            build_byte_bpe_encoder_v1(),
+            1000,
+        ),
+    ],
+)
+def test_encoder_prefix(test_config):
+    model_factory, piece_encoder, vocab_size = test_config
+
+    # Curated Transformers needs the config to get the model hyperparameters.
+    with_spans = build_with_strided_spans_v1(stride=96, window=128)
+    model = model_factory(
+        hidden_width=32,
+        intermediate_width=37,
+        num_hidden_layers=4,
+        num_attention_heads=4,
+        piece_encoder=piece_encoder,
+        vocab_size=vocab_size,
+        with_spans=with_spans,
+    )
+
+    for name, _ in model.get_ref("transformer").shims[0]._model.named_parameters():
+        assert name.startswith(
+            "curated_encoder."
+        ), f"Parameter name '{name} does not start with 'curated_encoder'"
```

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/models/test_with_strided_spans.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/models/test_with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/pipeline/test_transformer.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/pipeline/test_transformer.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/test_cli_app.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/test_cli_app.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/test_registry.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/test_torchscript_wrapper.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/test_torchscript_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/test_char_encoder.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/test_char_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/toy-merges.txt` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/toy-vocab.json` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/toy.model` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/toy.model`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/tokenization/toy.wordpieces` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/tokenization/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tests/util.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tests/util.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/__init__.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/bbpe_encoder.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/bbpe_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/char_encoder.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/char_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/hf_loader.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/hf_loader.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/sentencepiece_adapters.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/sentencepiece_adapters.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/sentencepiece_encoder.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/types.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/types.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/tokenization/wordpiece_encoder.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/tokenization/wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers/util.py` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers/util.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/PKG-INFO` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spacy-curated-transformers
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: Curated transformer models for spaCy pipelines
 Home-page: https://github.com/explosion/spacy-curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: curated-transformers<3.0.0,>=2.0.0.dev2
-Requires-Dist: curated-tokenizers<1.0.0,>=0.9.2
+Requires-Dist: curated-transformers<3.0.0,>=2.0.0.dev3
+Requires-Dist: curated-tokenizers<3.0.0,>=2.0.0.dev0
 Requires-Dist: fsspec>=2023.5.0
 Requires-Dist: spacy<5.0.0,>=4.0.0.dev2
 Requires-Dist: thinc<9.1.0,>=9.0.0.dev4
 Requires-Dist: torch>=1.12.0
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: spacy-curated-transformers Version: 2.0.0.dev0
+Metadata-Version: 2.1 Name: spacy-curated-transformers Version: 2.0.0.dev1
 Summary: Curated transformer models for spaCy pipelines Home-page: https://
 github.com/explosion/spacy-curated-transformers Author: Explosion Author-email:
 contact@explosion.ai License: MIT Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: curated-
-transformers<3.0.0,>=2.0.0.dev2 Requires-Dist: curated-tokenizers<1.0.0,>=0.9.2
-Requires-Dist: fsspec>=2023.5.0 Requires-Dist: spacy<5.0.0,>=4.0.0.dev2
-Requires-Dist: thinc<9.1.0,>=9.0.0.dev4 Requires-Dist: torch>=1.12.0 _[_h_t_t_p_s_:_/_/
-_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/_l_o_g_o_._s_v_g_]# ð« ð¤ spaCy Curated Transformers This
-package provides [spaCy](https://github.com/explosion/spaCy) components and
-architectures to use a curated set of transformer models via [`curated-
-transformers`](https://github.com/explosion/curated-transformers) in spaCy. [!
-[PyPi](https://img.shields.io/pypi/v/spacy-curated-transformers.svg?style=flat-
-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-curated-
-transformers) [![GitHub](https://img.shields.io/github/release/explosion/spacy-
-curated-transformers/all.svg?style=flat-square&logo=github)](https://
-github.com/explosion/spacy-curated-transformers/releases) ## Features - Use
-pretrained models based on one of the following architectures to power your
-spaCy pipeline: - ALBERT - BERT - CamemBERT - RoBERTa - XLM-RoBERTa - All the
-nice features supported by [`spacy-transformers`](https://github.com/explosion/
-spacy-transformers) such as support for Hugging Face Hub, **multi-task
-learning**, the extensible config system and out-of-the-box serialization -
-Deep integration into spaCy, which lays the groundwork for deployment-focused
-features such as distillation and quantization - Minimal dependencies ## â³
-Installation Installing the package from pip will automatically install all
-dependencies. ```bash pip install spacy-curated-transformers ``` ## ð
-Quickstart An example project is provided in the [`project`](project)
-directory. ## ð Documentation - ð [Layers and Model Architectures](https:
-//spacy.io/usage/layers-architectures): Power spaCy components with custom
-neural networks - ð [`CuratedTransformer`](https://spacy.io/api/
-curatedtransformer): Pipeline component API reference - ð [Transformer
-architectures](https://spacy.io/api/architectures#curated-trf): Architectures
-and registered functions ## Bug reports and other issues Please use [spaCy's
-issue tracker](https://github.com/explosion/spaCy/issues) to report a bug, or
-open a new thread on the [discussion board](https://github.com/explosion/spaCy/
-discussions) for any other issue.
+transformers<3.0.0,>=2.0.0.dev3 Requires-Dist: curated-
+tokenizers<3.0.0,>=2.0.0.dev0 Requires-Dist: fsspec>=2023.5.0 Requires-Dist:
+spacy<5.0.0,>=4.0.0.dev2 Requires-Dist: thinc<9.1.0,>=9.0.0.dev4 Requires-Dist:
+torch>=1.12.0 _[_h_t_t_p_s_:_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/_l_o_g_o_._s_v_g_]# ð« ð¤ spaCy
+Curated Transformers This package provides [spaCy](https://github.com/
+explosion/spaCy) components and architectures to use a curated set of
+transformer models via [`curated-transformers`](https://github.com/explosion/
+curated-transformers) in spaCy. [![PyPi](https://img.shields.io/pypi/v/spacy-
+curated-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://
+pypi.python.org/pypi/spacy-curated-transformers) [![GitHub](https://
+img.shields.io/github/release/explosion/spacy-curated-transformers/
+all.svg?style=flat-square&logo=github)](https://github.com/explosion/spacy-
+curated-transformers/releases) ## Features - Use pretrained models based on one
+of the following architectures to power your spaCy pipeline: - ALBERT - BERT -
+CamemBERT - RoBERTa - XLM-RoBERTa - All the nice features supported by [`spacy-
+transformers`](https://github.com/explosion/spacy-transformers) such as support
+for Hugging Face Hub, **multi-task learning**, the extensible config system and
+out-of-the-box serialization - Deep integration into spaCy, which lays the
+groundwork for deployment-focused features such as distillation and
+quantization - Minimal dependencies ## â³ Installation Installing the package
+from pip will automatically install all dependencies. ```bash pip install
+spacy-curated-transformers ``` ## ð Quickstart An example project is
+provided in the [`project`](project) directory. ## ð Documentation - ð
+[Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
+Power spaCy components with custom neural networks - ð
+[`CuratedTransformer`](https://spacy.io/api/curatedtransformer): Pipeline
+component API reference - ð [Transformer architectures](https://spacy.io/
+api/architectures#curated-trf): Architectures and registered functions ## Bug
+reports and other issues Please use [spaCy's issue tracker](https://github.com/
+explosion/spaCy/issues) to report a bug, or open a new thread on the
+[discussion board](https://github.com/explosion/spaCy/discussions) for any
+other issue.
```

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/SOURCES.txt` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-2.0.0.dev0/spacy_curated_transformers.egg-info/entry_points.txt` & `spacy-curated-transformers-2.0.0.dev1/spacy_curated_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

