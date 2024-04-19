# Comparing `tmp/conette-0.2.2.tar.gz` & `tmp/conette-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conette-0.2.2.tar", last modified: Mon Jan 15 14:07:09 2024, max compression
+gzip compressed data, was "conette-0.3.0.tar", last modified: Fri Apr 19 07:33:04 2024, max compression
```

## Comparing `conette-0.2.2.tar` & `conette-0.3.0.tar`

### file list

```diff
@@ -1,188 +1,160 @@
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.402354 conette-0.2.2/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       76 2023-11-09 17:38:13.000000 conette-0.2.2/MANIFEST.in
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8379 2024-01-15 14:07:09.402354 conette-0.2.2/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7345 2024-01-15 14:00:54.000000 conette-0.2.2/README.md
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1773 2024-01-12 14:39:50.000000 conette-0.2.2/pyproject.toml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       61 2024-01-12 17:24:53.000000 conette-0.2.2/requirements-dev.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      479 2024-01-12 14:39:50.000000 conette-0.2.2/requirements-train.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      158 2024-01-12 14:39:50.000000 conette-0.2.2/requirements.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2024-01-15 14:07:09.402354 conette-0.2.2/setup.cfg
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2023-11-09 15:40:18.000000 conette-0.2.2/setup.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.386354 conette-0.2.2/src/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.390354 conette-0.2.2/src/conette/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1527 2024-01-15 14:00:54.000000 conette-0.2.2/src/conette/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.390354 conette-0.2.2/src/conette/callbacks/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/callbacks/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    19120 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/callbacks/aac_evaluator.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7577 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/callbacks/aac_validator.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8096 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/callbacks/custom_ckpt.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2010 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/callbacks/debug.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4255 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/callbacks/deepspeed.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5004 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/callbacks/log.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4320 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/callbacks/resume.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12540 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/callbacks/stats_saver.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4204 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/callbacks/time.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.390354 conette-0.2.2/src/conette/datamodules/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      100 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datamodules/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6940 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datamodules/aac_dm.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5219 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datamodules/collate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16482 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datamodules/common.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16730 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datamodules/hdf.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.390354 conette-0.2.2/src/conette/datasets/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datasets/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.394353 conette-0.2.2/src/conette/datasets/hdf/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      142 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datasets/hdf/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1248 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datasets/hdf/common.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10662 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datasets/hdf/dataset.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    14154 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datasets/hdf/pack.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1261 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datasets/typing.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    34423 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/datasets/utils.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.394353 conette-0.2.2/src/conette/huggingface/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/huggingface/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2844 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/huggingface/config.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9856 2024-01-15 14:00:54.000000 conette-0.2.2/src/conette/huggingface/model.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5127 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/huggingface/preprocessor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1147 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/huggingface/setup.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1154 2023-11-20 10:26:48.000000 conette-0.2.2/src/conette/info.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.394353 conette-0.2.2/src/conette/metrics/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.394353 conette-0.2.2/src/conette/metrics/classes/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5655 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/all_metrics.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2654 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/bert_score_mrefs.ign.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2299 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/diversity.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2360 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/jaccard.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1488 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/new_words.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      436 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/null.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2314 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/self_bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4644 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/tensor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1856 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/text_stats.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2646 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/classes/wmd.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3000 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/cross_referencing.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.394353 conette-0.2.2/src/conette/metrics/functional/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/functional/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6024 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/functional/bert_score_mrefs.ign.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1143 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/functional/div_n.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8569 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/functional/diversity.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1731 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/functional/jaccard.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1097 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/functional/new_words.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1768 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/functional/self_bleu.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4305 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/functional/text_stats.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9006 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/functional/torch_cider_d.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1618 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/functional/wmd.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6774 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/metrics/retrieval.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.394353 conette-0.2.2/src/conette/nn/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5427 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/cnext_ckpt_utils.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.394353 conette-0.2.2/src/conette/nn/decoders/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/decoders/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3751 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/decoders/aac_tfmer.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.394353 conette-0.2.2/src/conette/nn/decoding/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/decoding/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10394 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/decoding/beam.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1841 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/decoding/common.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2365 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/decoding/forcing.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4211 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/decoding/greedy.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.398353 conette-0.2.2/src/conette/nn/encoders/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/encoders/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16211 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/encoders/cnn10.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7126 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/encoders/cnn14.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9347 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/encoders/cnn14_decisionlevel_att.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    14062 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/encoders/convnext.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      828 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/encoders/ident.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.398353 conette-0.2.2/src/conette/nn/functional/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/functional/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2148 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/functional/crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1139 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/functional/drop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1794 2023-11-17 12:43:08.000000 conette-0.2.2/src/conette/nn/functional/get.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1496 2024-01-09 13:13:37.000000 conette-0.2.2/src/conette/nn/functional/indexes.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2635 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/functional/init.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3998 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/functional/label.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12783 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/functional/mask.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    14469 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/functional/misc.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9844 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/functional/pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      859 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/functional/repeat.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.398353 conette-0.2.2/src/conette/nn/loss/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/loss/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1110 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/loss/ce_mean.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.398353 conette-0.2.2/src/conette/nn/modules/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/modules/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1298 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/modules/crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      677 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/modules/drop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6258 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/modules/misc.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1619 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/modules/norm.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2559 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/modules/pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2787 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/modules/positional_encoding.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3050 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/nn/modules/tensor.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.398353 conette-0.2.2/src/conette/nn/pann_utils/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/pann_utils/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5212 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/pann_utils/ckpt.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2041 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/pann_utils/hub.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   126736 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/pann_utils/models.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8640 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/nn/pann_utils/pytorch_utils.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.398353 conette-0.2.2/src/conette/optim/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/optim/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8707 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/optim/cyclic_cos_decay.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2194 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/optim/optimizers.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3842 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/optim/schedulers.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.398353 conette-0.2.2/src/conette/pl_modules/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/pl_modules/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9489 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/pl_modules/base.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    14667 2024-01-15 14:00:54.000000 conette-0.2.2/src/conette/pl_modules/baseline.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9064 2023-11-20 12:41:51.000000 conette-0.2.2/src/conette/pl_modules/common.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    19146 2024-01-15 14:00:54.000000 conette-0.2.2/src/conette/pl_modules/conette.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7001 2024-01-15 14:00:54.000000 conette-0.2.2/src/conette/predict.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    21882 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/prepare.py
--rwxrwxr-x   0 labbeti   (1000) labbeti   (1000)    15113 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/retrieve.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.398353 conette-0.2.2/src/conette/tokenization/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       76 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/tokenization/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    37368 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/tokenization/aac_tokenizer.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      387 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/tokenization/constants.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6344 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/tokenization/normalizers.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.402354 conette-0.2.2/src/conette/tokenization/tokenizers/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/tokenization/tokenizers/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4335 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/tokenization/tokenizers/base.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1441 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/tokenization/tokenizers/common.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      431 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/tokenization/tokenizers/factory.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1719 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/tokenization/tokenizers/ptb.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2036 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/tokenization/tokenizers/spacy.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1507 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/tokenization/tokenizers/word.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3672 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/tokenization/tokenizers/wrapper.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    17226 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/train.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.402354 conette-0.2.2/src/conette/transforms/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/transforms/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.402354 conette-0.2.2/src/conette/transforms/audio/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/transforms/audio/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7974 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/transforms/audio/cutoutspec.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2148 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/transforms/audio/resample.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7646 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/transforms/audio/spec_aug.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3147 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/transforms/audio/speed_perturb.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3839 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/transforms/audioset_labels.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    18652 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/transforms/get.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4023 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/transforms/mixup.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2515 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/transforms/utils.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.402354 conette-0.2.2/src/conette/utils/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/utils/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1835 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/utils/cmdline.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8070 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/utils/collections.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8995 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/utils/csum.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2409 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/utils/csv_utils.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5431 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/utils/custom_logger.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4654 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/utils/dcase.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10062 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/utils/disk_cache.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2311 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/utils/func_utils.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10361 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/utils/hydra.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      935 2023-11-09 15:40:18.000000 conette-0.2.2/src/conette/utils/log_utils.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7263 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/utils/misc.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      393 2024-01-12 14:39:50.000000 conette-0.2.2/src/conette/utils/yaml_utils.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.390354 conette-0.2.2/src/conette.egg-info/
--rw-r--r--   0 labbeti   (1000) labbeti   (1000)     8379 2024-01-15 14:07:09.000000 conette-0.2.2/src/conette.egg-info/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5439 2024-01-15 14:07:09.000000 conette-0.2.2/src/conette.egg-info/SOURCES.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2024-01-15 14:07:09.000000 conette-0.2.2/src/conette.egg-info/dependency_links.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      200 2024-01-15 14:07:09.000000 conette-0.2.2/src/conette.egg-info/entry_points.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      623 2024-01-15 14:07:09.000000 conette-0.2.2/src/conette.egg-info/requires.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        8 2024-01-15 14:07:09.000000 conette-0.2.2/src/conette.egg-info/top_level.txt
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.402354 conette-0.2.2/src/conf/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      106 2024-01-12 14:39:50.000000 conette-0.2.2/src/conf/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-01-15 14:07:09.402354 conette-0.2.2/tests/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2090 2024-01-12 14:39:50.000000 conette-0.2.2/tests/test_inference.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.636976 conette-0.3.0/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       76 2023-11-09 17:38:13.000000 conette-0.3.0/MANIFEST.in
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8461 2024-04-19 07:33:04.636976 conette-0.3.0/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7457 2024-04-18 15:42:09.000000 conette-0.3.0/README.md
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1748 2024-04-18 15:42:09.000000 conette-0.3.0/pyproject.toml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2024-04-18 15:42:09.000000 conette-0.3.0/requirements-dev.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4635 2024-04-18 15:42:09.000000 conette-0.3.0/requirements-train.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      245 2024-04-18 15:42:09.000000 conette-0.3.0/requirements.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2024-04-19 07:33:04.636976 conette-0.3.0/setup.cfg
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2023-11-09 15:40:18.000000 conette-0.3.0/setup.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.620976 conette-0.3.0/src/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.620976 conette-0.3.0/src/conette/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1527 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.624976 conette-0.3.0/src/conette/callbacks/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/callbacks/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    19117 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/callbacks/aac_evaluator.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7588 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/callbacks/aac_validator.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8096 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/callbacks/custom_ckpt.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2010 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/callbacks/debug.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4258 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/callbacks/deepspeed.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5004 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/callbacks/log.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4320 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/callbacks/resume.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12547 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/callbacks/stats_saver.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4204 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/callbacks/time.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.624976 conette-0.3.0/src/conette/datamodules/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      100 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/datamodules/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6940 2024-04-10 14:13:26.000000 conette-0.3.0/src/conette/datamodules/aac_dm.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5181 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/datamodules/collate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7254 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/datamodules/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16968 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/datamodules/hdf.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.624976 conette-0.3.0/src/conette/datasets/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/datasets/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      680 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/datasets/typing.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    30071 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/datasets/utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.624976 conette-0.3.0/src/conette/huggingface/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/huggingface/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2844 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/huggingface/config.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10120 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/huggingface/model.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4850 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/huggingface/preprocessor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1154 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/huggingface/setup.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1216 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/info.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.624976 conette-0.3.0/src/conette/metrics/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/metrics/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.624976 conette-0.3.0/src/conette/metrics/classes/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/metrics/classes/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5664 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/metrics/classes/all_metrics.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2299 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/metrics/classes/diversity.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1488 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/metrics/classes/new_words.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1856 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/metrics/classes/text_stats.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2997 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/metrics/cross_referencing.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.628976 conette-0.3.0/src/conette/metrics/functional/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/metrics/functional/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8569 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/metrics/functional/diversity.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1097 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/metrics/functional/new_words.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4305 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/metrics/functional/text_stats.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.628976 conette-0.3.0/src/conette/nn/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4663 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/ckpt.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.628976 conette-0.3.0/src/conette/nn/decoders/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/decoders/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3751 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/decoders/aac_tfmer.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.628976 conette-0.3.0/src/conette/nn/decoding/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/decoding/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10367 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/nn/decoding/beam.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1841 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/decoding/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2379 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/decoding/forcing.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4192 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/nn/decoding/greedy.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.628976 conette-0.3.0/src/conette/nn/encoders/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/encoders/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16159 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/encoders/cnn10.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7126 2024-04-05 12:57:47.000000 conette-0.3.0/src/conette/nn/encoders/cnn14.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9359 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/encoders/cnn14_decisionlevel_att.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15063 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/encoders/convnext.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      828 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/encoders/ident.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.628976 conette-0.3.0/src/conette/nn/functional/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/functional/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1139 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/functional/drop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1094 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/functional/get.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2635 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/functional/init.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      417 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/nn/functional/pad.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.628976 conette-0.3.0/src/conette/nn/loss/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/loss/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1113 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/loss/ce_mean.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.628976 conette-0.3.0/src/conette/nn/modules/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/modules/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      677 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/modules/drop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5824 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/modules/misc.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1619 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/nn/modules/norm.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2787 2024-04-05 11:53:16.000000 conette-0.3.0/src/conette/nn/modules/positional_encoding.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.632976 conette-0.3.0/src/conette/nn/pann_utils/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/nn/pann_utils/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1890 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/pann_utils/hub.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)   128929 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/pann_utils/models.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8633 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/nn/pann_utils/pytorch_utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.632976 conette-0.3.0/src/conette/optim/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/optim/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8707 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/optim/cyclic_cos_decay.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2194 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/optim/optimizers.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3842 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/optim/schedulers.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.632976 conette-0.3.0/src/conette/pl_modules/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/pl_modules/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9574 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/pl_modules/base.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    14784 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/pl_modules/baseline.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8852 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/pl_modules/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    19129 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/pl_modules/conette.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7052 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/predict.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    20381 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/prepare.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.632976 conette-0.3.0/src/conette/tokenization/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       76 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/tokenization/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    37241 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/tokenization/aac_tokenizer.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      387 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/tokenization/constants.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6344 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/tokenization/normalizers.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.632976 conette-0.3.0/src/conette/tokenization/tokenizers/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/tokenization/tokenizers/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4335 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/tokenization/tokenizers/base.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1441 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/tokenization/tokenizers/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      431 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/tokenization/tokenizers/factory.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1719 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/tokenization/tokenizers/ptb.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2036 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/tokenization/tokenizers/spacy.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1507 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/tokenization/tokenizers/word.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3672 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/tokenization/tokenizers/wrapper.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    17225 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/train.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.632976 conette-0.3.0/src/conette/transforms/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/transforms/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.636976 conette-0.3.0/src/conette/transforms/audio/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/transforms/audio/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7974 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/transforms/audio/cutoutspec.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2148 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/transforms/audio/resample.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7646 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/transforms/audio/spec_aug.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3141 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/transforms/audio/speed_perturb.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3193 2024-04-19 07:32:58.000000 conette-0.3.0/src/conette/transforms/audioset_mapping.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    18706 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/transforms/get.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4023 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/transforms/mixup.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3234 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/transforms/utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.636976 conette-0.3.0/src/conette/utils/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        0 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/utils/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1003 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/utils/cmdline.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5844 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/utils/collections.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8995 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/utils/csum.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2445 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/utils/csv_utils.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5431 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/utils/custom_logger.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4654 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/utils/dcase.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10062 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/utils/disk_cache.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2311 2023-11-09 15:40:18.000000 conette-0.3.0/src/conette/utils/func_utils.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10378 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/utils/hydra.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2797 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/utils/log_utils.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7221 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/utils/misc.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      643 2024-04-18 15:42:09.000000 conette-0.3.0/src/conette/utils/type_checks.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      393 2024-01-12 14:39:50.000000 conette-0.3.0/src/conette/utils/yaml_utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.620976 conette-0.3.0/src/conette.egg-info/
+-rw-r--r--   0 labbeti   (1000) labbeti   (1000)     8461 2024-04-19 07:33:04.000000 conette-0.3.0/src/conette.egg-info/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4417 2024-04-19 07:33:04.000000 conette-0.3.0/src/conette.egg-info/SOURCES.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2024-04-19 07:33:04.000000 conette-0.3.0/src/conette.egg-info/dependency_links.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      200 2024-04-19 07:33:04.000000 conette-0.3.0/src/conette.egg-info/entry_points.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4946 2024-04-19 07:33:04.000000 conette-0.3.0/src/conette.egg-info/requires.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        8 2024-04-19 07:33:04.000000 conette-0.3.0/src/conette.egg-info/top_level.txt
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.636976 conette-0.3.0/src/conf/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      106 2024-01-12 14:39:50.000000 conette-0.3.0/src/conf/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-19 07:33:04.636976 conette-0.3.0/tests/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2090 2024-01-12 14:39:50.000000 conette-0.3.0/tests/test_inference.py
```

### Comparing `conette-0.2.2/PKG-INFO` & `conette-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,96 @@
 Metadata-Version: 2.1
 Name: conette
-Version: 0.2.2
+Version: 0.3.0
 Summary: CoNeTTE is an audio captioning system, which generate a short textual description of the sound events in any audio file.
 Author-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Project-URL: Repository, https://github.com/Labbeti/conette-audio-captioning.git
 Project-URL: Changelog, https://github.com/Labbeti/conette-audio-captioning/blob/main/CHANGELOG.md
 Keywords: audio,deep-learning,pytorch,captioning,audio-captioning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: train
+Provides-Extra: test
 
 <div align="center">
 
 # CoNeTTE model for Audio Captioning
 
 [![](<https://img.shields.io/badge/-Python 3.10+-blue?style=for-the-badge&logo=python&logoColor=white>)](https://www.python.org/)
 [![](<https://img.shields.io/badge/-PyTorch 1.10.1+-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white>)](https://pytorch.org/get-started/locally/)
 [![](https://img.shields.io/badge/code%20style-black-black.svg?style=for-the-badge&labelColor=gray)](https://black.readthedocs.io/en/stable/)
 [![](https://img.shields.io/github/actions/workflow/status/Labbeti/conette-audio-captioning/inference.yaml?branch=main&style=for-the-badge&logo=github)](https://github.com/Labbeti/conette-audio-captioning/actions)
 
 </div>
 
-CoNeTTE is an audio captioning system, which generate a short textual description of the sound events in any audio file. The architecture and training are explained in the corresponding [paper](https://arxiv.org/pdf/2309.00454.pdf). The model has been developped by me ([Étienne Labbé](https://labbeti.github.io/)) during my PhD. A simple interface to test CoNeTTE is available on [HuggingFace website](https://huggingface.co/spaces/Labbeti/conette).
+CoNeTTE is an audio captioning system, which generate a short textual description of the sound events in any audio file. The architecture and training are explained in the [corresponding paper](https://arxiv.org/pdf/2309.00454.pdf). The model has been developped by me ([Étienne Labbé](https://labbeti.github.io/)) during my PhD. A simple interface to test CoNeTTE is available on [HuggingFace website](https://huggingface.co/spaces/Labbeti/conette).
 
-## Inference
+## Training
+### Requirements
+- Intended for Ubuntu 20.04 only. Requires **java** < 1.13, **ffmpeg**, **yt-dlp**, and **zip** commands.
+- Recommanded GPU: NVIDIA V100 with 32GB VRAM.
+- WavCaps dataset might requires more than 2 TB of disk storage. Other datasets requires less than 50 GB.
+
+### Installation
+By default, **only the pip inference requirements are installed for conette**. To install training requirements you need to use the following command:
+```bash
+python -m pip install conette[train]
+```
+If you already installed conette for inference, it is **highly recommanded to create another environment** before installing conette for training.
+
+### Download external models and data
+These steps might take a while (few hours to download and prepare everything depending on your CPU, GPU and SSD/HDD).
+
+First, download the ConvNeXt, NLTK and spacy models :
+```bash
+conette-prepare data=none default=true pack_to_hdf=false csum_in_hdf_name=false pann=false
+```
+
+Then download the 4 datasets used to train CoNeTTE :
+```bash
+common_args="data.download=true pack_to_hdf=true audio_t=resample_mean_convnext audio_t.pretrain_path=cnext_bl_75 post_hdf_name=bl pretag=cnext_bl_75"
+
+conette-prepare data=audiocaps audio_t.src_sr=32000 ${common_args}
+conette-prepare data=clotho audio_t.src_sr=44100 ${common_args}
+conette-prepare data=macs audio_t.src_sr=48000 ${common_args}
+conette-prepare data=wavcaps audio_t.src_sr=32000 ${common_args} datafilter.min_audio_size=0.1 datafilter.max_audio_size=30.0 datafilter.sr=32000
+```
+
+### Train a model
+CNext-trans (baseline) on CL only (~3 hours on 1 GPU V100-32G)
+```bash
+conette-train expt=[clotho_cnext_bl] pl=baseline
+```
+
+CoNeTTE on AC+CL+MA+WC, specialized for CL (~4 hours on 1 GPU V100-32G)
+```bash
+conette-train expt=[camw_cnext_bl_for_c,task_ds_src_camw] pl=conette
+```
+
+CoNeTTE on AC+CL+MA+WC, specialized for AC (~3 hours on 1 GPU V100-32G)
+```bash
+conette-train expt=[camw_cnext_bl_for_a,task_ds_src_camw] pl=conette
+```
+
+Note 1: any training using AC data cannot be exactly reproduced because a part of this data is deleted from the YouTube source, and I cannot share my own audio files.
+Note 2: paper results are averaged scores over 5 seeds (1234-1238). The default training only uses seed 1234.
+
+## Inference only (without training)
 
 ### Installation
 ```bash
-python -m pip install conette
+python -m pip install conette[test]
 ```
 
 ### Usage with python
 ```py
 from conette import CoNeTTEConfig, CoNeTTEModel
 
 config = CoNeTTEConfig.from_pretrained("Labbeti/conette")
@@ -88,90 +138,40 @@
 ```
 
 ### Performance
 The model has been trained on AudioCaps (AC), Clotho (CL), MACS (MA) and WavCaps (WC). The performance on the test subsets are :
 
 | Test data | SPIDEr (%) | SPIDEr-FL (%) | FENSE (%) | Vocab | Outputs | Scores |
 | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
-| AC-test | 44.14 | 43.98 | 60.81 | 309 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/outputs_audiocaps_test.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/scores_audiocaps_test.yaml) |
-| CL-eval | 30.97 | 30.87 | 51.72 | 636 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/outputs_clotho_eval.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/scores_clotho_eval.yaml) |
+| AC-test | 44.14 | 43.98 | 60.81 | 309 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/outputs_audiocaps_test.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/scores_audiocaps_test.yaml) |
+| CL-eval | 30.97 | 30.87 | 51.72 | 636 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/outputs_clotho_eval.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/scores_clotho_eval.yaml) |
 
 This model checkpoint has been trained with focus on the Clotho dataset, but it can also reach a good performance on AudioCaps with the "audiocaps" task.
 
 ### Limitations
 - The model expected audio sampled at **32 kHz**. The model automatically resample up or down the input audio files. However, it might give worse results, especially when using audio with lower sampling rates.
 - The model has been trained on audio lasting from **1 to 30 seconds**. It can handle longer audio files, but it might require more memory and give worse results.
 
-## Train a model
-### Requirements
-- Intended for Ubuntu 20.04 only. Requires **java** < 1.13, **ffmpeg**, **yt-dlp**, and **zip** commands.
-- Recommanded GPU: NVIDIA V100 with 32GB VRAM.
-- WavCaps dataset might requires more than 2 TB of disk storage. Other datasets requires less than 50 GB.
-
-### Installation
-By default, **only the inference requirements are installed for conette**. To install training requirements you need to use the following command:
-```bash
-python -m pip install conette[train]
-```
-If you already installed conette for inference, it is **highly recommanded to create another environment** before installing conette for training.
-
-### Download external models and data
-These steps might take a while (few hours to download and prepare everything depending on your CPU, GPU and SSD/HDD).
-
-First, download the ConvNeXt, NLTK and spacy models :
-```bash
-conette-prepare data=none default=true pack_to_hdf=false csum_in_hdf_name=false pann=false
-```
-
-Then download the 4 datasets used to train CoNeTTE :
-```bash
-cnext_bl_path="$HOME/.cache/torch/hub/checkpoints/convnext_tiny_465mAP_BL_AC.pth"
-common_args="data.download=true pack_to_hdf=true audio_t=resample_mean_convnext audio_t.pretrain_path=${cnext_bl_path} post_hdf_name=bl pretag=cnext_bl"
-
-conette-prepare data=audiocaps audio_t.src_sr=32000 ${common_args}
-conette-prepare data=clotho audio_t.src_sr=44100 ${common_args}
-conette-prepare data=macs audio_t.src_sr=48000 ${common_args}
-conette-prepare data=wavcaps audio_t.src_sr=32000 ${common_args} datafilter.min_audio_size=0.1 datafilter.max_audio_size=30.0 datafilter.sr=32000
-```
-
-### Train a model
-CNext-trans (baseline) on CL only (~3 hours on 1 GPU V100-32G)
-```bash
-conette-train expt=[clotho_cnext_bl] pl=baseline
-```
-
-CoNeTTE on AC+CL+MA+WC, specialized for CL (~4 hours on 1 GPU V100-32G)
-```bash
-conette-train expt=[camw_cnext_bl_for_c,task_ds_src_camw] pl=conette
-```
-
-CoNeTTE on AC+CL+MA+WC, specialized for AC (~3 hours on 1 GPU V100-32G)
-```bash
-conette-train expt=[camw_cnext_bl_for_a,task_ds_src_camw] pl=conette
-```
-
-**About reproducibility** : any training with AC data cannot be reproduced because a part of this data is deleted from the YouTube source, and I cannot share my own audio files.
-
 ## Citation
 The preprint version of the paper describing CoNeTTE is available on arxiv: https://arxiv.org/pdf/2309.00454.pdf
 
 ```bibtex
-@misc{labbé2023conette,
+@misc{labbe2023conette,
 	title        = {CoNeTTE: An efficient Audio Captioning system leveraging multiple datasets with Task Embedding},
 	author       = {Étienne Labbé and Thomas Pellegrini and Julien Pinquier},
 	year         = 2023,
 	journal      = {arXiv preprint arXiv:2309.00454},
 	url          = {https://arxiv.org/pdf/2309.00454.pdf},
 	eprint       = {2309.00454},
 	archiveprefix = {arXiv},
 	primaryclass = {cs.SD}
 }
 ```
 
 ## Additional information
 - CoNeTTE stands for **Co**nv**Ne**Xt-**T**ransformer with **T**ask **E**mbedding.
 - Model weights are available on HuggingFace: https://huggingface.co/Labbeti/conette
-- The weights of the encoder part of the architecture is based on a ConvNeXt model for audio classification, available here: https://zenodo.org/record/8020843 under the filename "convnext_tiny_465mAP_BL_AC_70kit.pth".
+- The weights of the encoder part of the architecture is based on a ConvNeXt model for audio classification, available here: https://zenodo.org/records/10987498 under the filename "convnext_tiny_465mAP_BL_AC_75kit.pth".
 
 ## Contact
 Maintainer:
-- Etienne Labbé "Labbeti": labbeti.pub@gmail.com
+- [Étienne Labbé](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

### Comparing `conette-0.2.2/README.md` & `conette-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,71 @@
 [![](<https://img.shields.io/badge/-Python 3.10+-blue?style=for-the-badge&logo=python&logoColor=white>)](https://www.python.org/)
 [![](<https://img.shields.io/badge/-PyTorch 1.10.1+-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white>)](https://pytorch.org/get-started/locally/)
 [![](https://img.shields.io/badge/code%20style-black-black.svg?style=for-the-badge&labelColor=gray)](https://black.readthedocs.io/en/stable/)
 [![](https://img.shields.io/github/actions/workflow/status/Labbeti/conette-audio-captioning/inference.yaml?branch=main&style=for-the-badge&logo=github)](https://github.com/Labbeti/conette-audio-captioning/actions)
 
 </div>
 
-CoNeTTE is an audio captioning system, which generate a short textual description of the sound events in any audio file. The architecture and training are explained in the corresponding [paper](https://arxiv.org/pdf/2309.00454.pdf). The model has been developped by me ([Étienne Labbé](https://labbeti.github.io/)) during my PhD. A simple interface to test CoNeTTE is available on [HuggingFace website](https://huggingface.co/spaces/Labbeti/conette).
+CoNeTTE is an audio captioning system, which generate a short textual description of the sound events in any audio file. The architecture and training are explained in the [corresponding paper](https://arxiv.org/pdf/2309.00454.pdf). The model has been developped by me ([Étienne Labbé](https://labbeti.github.io/)) during my PhD. A simple interface to test CoNeTTE is available on [HuggingFace website](https://huggingface.co/spaces/Labbeti/conette).
 
-## Inference
+## Training
+### Requirements
+- Intended for Ubuntu 20.04 only. Requires **java** < 1.13, **ffmpeg**, **yt-dlp**, and **zip** commands.
+- Recommanded GPU: NVIDIA V100 with 32GB VRAM.
+- WavCaps dataset might requires more than 2 TB of disk storage. Other datasets requires less than 50 GB.
+
+### Installation
+By default, **only the pip inference requirements are installed for conette**. To install training requirements you need to use the following command:
+```bash
+python -m pip install conette[train]
+```
+If you already installed conette for inference, it is **highly recommanded to create another environment** before installing conette for training.
+
+### Download external models and data
+These steps might take a while (few hours to download and prepare everything depending on your CPU, GPU and SSD/HDD).
+
+First, download the ConvNeXt, NLTK and spacy models :
+```bash
+conette-prepare data=none default=true pack_to_hdf=false csum_in_hdf_name=false pann=false
+```
+
+Then download the 4 datasets used to train CoNeTTE :
+```bash
+common_args="data.download=true pack_to_hdf=true audio_t=resample_mean_convnext audio_t.pretrain_path=cnext_bl_75 post_hdf_name=bl pretag=cnext_bl_75"
+
+conette-prepare data=audiocaps audio_t.src_sr=32000 ${common_args}
+conette-prepare data=clotho audio_t.src_sr=44100 ${common_args}
+conette-prepare data=macs audio_t.src_sr=48000 ${common_args}
+conette-prepare data=wavcaps audio_t.src_sr=32000 ${common_args} datafilter.min_audio_size=0.1 datafilter.max_audio_size=30.0 datafilter.sr=32000
+```
+
+### Train a model
+CNext-trans (baseline) on CL only (~3 hours on 1 GPU V100-32G)
+```bash
+conette-train expt=[clotho_cnext_bl] pl=baseline
+```
+
+CoNeTTE on AC+CL+MA+WC, specialized for CL (~4 hours on 1 GPU V100-32G)
+```bash
+conette-train expt=[camw_cnext_bl_for_c,task_ds_src_camw] pl=conette
+```
+
+CoNeTTE on AC+CL+MA+WC, specialized for AC (~3 hours on 1 GPU V100-32G)
+```bash
+conette-train expt=[camw_cnext_bl_for_a,task_ds_src_camw] pl=conette
+```
+
+Note 1: any training using AC data cannot be exactly reproduced because a part of this data is deleted from the YouTube source, and I cannot share my own audio files.
+Note 2: paper results are averaged scores over 5 seeds (1234-1238). The default training only uses seed 1234.
+
+## Inference only (without training)
 
 ### Installation
 ```bash
-python -m pip install conette
+python -m pip install conette[test]
 ```
 
 ### Usage with python
 ```py
 from conette import CoNeTTEConfig, CoNeTTEModel
 
 config = CoNeTTEConfig.from_pretrained("Labbeti/conette")
@@ -67,90 +117,40 @@
 ```
 
 ### Performance
 The model has been trained on AudioCaps (AC), Clotho (CL), MACS (MA) and WavCaps (WC). The performance on the test subsets are :
 
 | Test data | SPIDEr (%) | SPIDEr-FL (%) | FENSE (%) | Vocab | Outputs | Scores |
 | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
-| AC-test | 44.14 | 43.98 | 60.81 | 309 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/outputs_audiocaps_test.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/scores_audiocaps_test.yaml) |
-| CL-eval | 30.97 | 30.87 | 51.72 | 636 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/outputs_clotho_eval.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/scores_clotho_eval.yaml) |
+| AC-test | 44.14 | 43.98 | 60.81 | 309 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/outputs_audiocaps_test.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/scores_audiocaps_test.yaml) |
+| CL-eval | 30.97 | 30.87 | 51.72 | 636 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/outputs_clotho_eval.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/scores_clotho_eval.yaml) |
 
 This model checkpoint has been trained with focus on the Clotho dataset, but it can also reach a good performance on AudioCaps with the "audiocaps" task.
 
 ### Limitations
 - The model expected audio sampled at **32 kHz**. The model automatically resample up or down the input audio files. However, it might give worse results, especially when using audio with lower sampling rates.
 - The model has been trained on audio lasting from **1 to 30 seconds**. It can handle longer audio files, but it might require more memory and give worse results.
 
-## Train a model
-### Requirements
-- Intended for Ubuntu 20.04 only. Requires **java** < 1.13, **ffmpeg**, **yt-dlp**, and **zip** commands.
-- Recommanded GPU: NVIDIA V100 with 32GB VRAM.
-- WavCaps dataset might requires more than 2 TB of disk storage. Other datasets requires less than 50 GB.
-
-### Installation
-By default, **only the inference requirements are installed for conette**. To install training requirements you need to use the following command:
-```bash
-python -m pip install conette[train]
-```
-If you already installed conette for inference, it is **highly recommanded to create another environment** before installing conette for training.
-
-### Download external models and data
-These steps might take a while (few hours to download and prepare everything depending on your CPU, GPU and SSD/HDD).
-
-First, download the ConvNeXt, NLTK and spacy models :
-```bash
-conette-prepare data=none default=true pack_to_hdf=false csum_in_hdf_name=false pann=false
-```
-
-Then download the 4 datasets used to train CoNeTTE :
-```bash
-cnext_bl_path="$HOME/.cache/torch/hub/checkpoints/convnext_tiny_465mAP_BL_AC.pth"
-common_args="data.download=true pack_to_hdf=true audio_t=resample_mean_convnext audio_t.pretrain_path=${cnext_bl_path} post_hdf_name=bl pretag=cnext_bl"
-
-conette-prepare data=audiocaps audio_t.src_sr=32000 ${common_args}
-conette-prepare data=clotho audio_t.src_sr=44100 ${common_args}
-conette-prepare data=macs audio_t.src_sr=48000 ${common_args}
-conette-prepare data=wavcaps audio_t.src_sr=32000 ${common_args} datafilter.min_audio_size=0.1 datafilter.max_audio_size=30.0 datafilter.sr=32000
-```
-
-### Train a model
-CNext-trans (baseline) on CL only (~3 hours on 1 GPU V100-32G)
-```bash
-conette-train expt=[clotho_cnext_bl] pl=baseline
-```
-
-CoNeTTE on AC+CL+MA+WC, specialized for CL (~4 hours on 1 GPU V100-32G)
-```bash
-conette-train expt=[camw_cnext_bl_for_c,task_ds_src_camw] pl=conette
-```
-
-CoNeTTE on AC+CL+MA+WC, specialized for AC (~3 hours on 1 GPU V100-32G)
-```bash
-conette-train expt=[camw_cnext_bl_for_a,task_ds_src_camw] pl=conette
-```
-
-**About reproducibility** : any training with AC data cannot be reproduced because a part of this data is deleted from the YouTube source, and I cannot share my own audio files.
-
 ## Citation
 The preprint version of the paper describing CoNeTTE is available on arxiv: https://arxiv.org/pdf/2309.00454.pdf
 
 ```bibtex
-@misc{labbé2023conette,
+@misc{labbe2023conette,
 	title        = {CoNeTTE: An efficient Audio Captioning system leveraging multiple datasets with Task Embedding},
 	author       = {Étienne Labbé and Thomas Pellegrini and Julien Pinquier},
 	year         = 2023,
 	journal      = {arXiv preprint arXiv:2309.00454},
 	url          = {https://arxiv.org/pdf/2309.00454.pdf},
 	eprint       = {2309.00454},
 	archiveprefix = {arXiv},
 	primaryclass = {cs.SD}
 }
 ```
 
 ## Additional information
 - CoNeTTE stands for **Co**nv**Ne**Xt-**T**ransformer with **T**ask **E**mbedding.
 - Model weights are available on HuggingFace: https://huggingface.co/Labbeti/conette
-- The weights of the encoder part of the architecture is based on a ConvNeXt model for audio classification, available here: https://zenodo.org/record/8020843 under the filename "convnext_tiny_465mAP_BL_AC_70kit.pth".
+- The weights of the encoder part of the architecture is based on a ConvNeXt model for audio classification, available here: https://zenodo.org/records/10987498 under the filename "convnext_tiny_465mAP_BL_AC_75kit.pth".
 
 ## Contact
 Maintainer:
-- Etienne Labbé "Labbeti": labbeti.pub@gmail.com
+- [Étienne Labbé](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

### Comparing `conette-0.2.2/pyproject.toml` & `conette-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 keywords = ["audio", "deep-learning", "pytorch", "captioning", "audio-captioning"]
 license = {file = "LICENSE"}
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 maintainers = [
     {name = "Etienne Labbé (Labbeti)", email = "labbeti.pub@gmail.com"},
 ]
 dynamic = ["version", "dependencies", "optional-dependencies"]
@@ -35,11 +34,11 @@
 [tool.setuptools.packages.find]
 where = ["src"]  # list of folders that contain the packages (["."] by default)
 include = ["conette*"]  # package names should match these glob patterns (["*"] by default)
 
 [tool.setuptools.dynamic]
 version = {attr = "conette.__version__"}
 dependencies = {file = ["requirements.txt"]}
-optional-dependencies = { dev = { file = ["requirements-dev.txt"] }, train = { file = ["requirements-train.txt"]}}
+optional-dependencies = { dev = { file = ["requirements-dev.txt"] }, train = { file = ["requirements-train.txt"]}, test = { file = []}}
 
 [tool.ruff]
 ignore = ["E501", "E402"]
```

### Comparing `conette-0.2.2/src/conette/__init__.py` & `conette-0.3.0/src/conette/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 __name__ = "conette"
 __author__ = "Etienne Labbé (Labbeti)"
 __author_email__ = "labbeti.pub@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "Etienne Labbé (Labbeti)"
 __status__ = "Development"
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 
 
 from pathlib import Path
 from typing import Any, Optional
 
 from conette.huggingface.config import CoNeTTEConfig  # noqa: F401
 from conette.huggingface.model import CoNeTTEModel  # noqa: F401
```

### Comparing `conette-0.2.2/src/conette/callbacks/aac_evaluator.py` & `conette-0.3.0/src/conette/callbacks/aac_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,38 +3,34 @@
 
 import csv
 import logging
 import os
 import os.path as osp
 import tempfile
 import time
-
 from typing import Any, Optional, Union
 
 import torch
 import yaml
-
+from aac_metrics.utils.checks import is_mono_sents, is_mult_sents
+from aac_metrics.utils.collections import flat_list, unflat_list
 from pytorch_lightning import LightningModule
 from pytorch_lightning.callbacks.callback import Callback
 from pytorch_lightning.loggers import TensorBoardLogger
 from torch import Tensor
 from torch.utils.data.dataloader import DataLoader
-
-from aac_metrics.utils.checks import is_mono_sents, is_mult_sents
-from aac_metrics.utils.collections import flat_list, unflat_list
+from torchoutil.nn.functional import move_to_rec
+from torchoutil.utils.collections import all_eq
 
 from conette.metrics.classes.all_metrics import AllMetrics
-from conette.nn.functional.misc import move_to_rec
 from conette.tokenization.aac_tokenizer import AACTokenizer
-from conette.utils.collections import all_eq
 from conette.utils.custom_logger import CustomTensorboardLogger
 from conette.utils.dcase import export_to_dcase_task6a_csv
 from conette.utils.log_utils import warn_once
 
-
 pylog = logging.getLogger(__name__)
 
 
 class AACEvaluator(Callback):
     """Callback which stores candidates and references during testing to produce AAC scores.
 
     Include metrics : BLEU1, BLEU2, BLEU3, BLEU4, METEOR, ROUGE-L, CIDEr, SPICE, SPIDEr.
```

### Comparing `conette-0.2.2/src/conette/callbacks/aac_validator.py` & `conette-0.3.0/src/conette/callbacks/aac_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Any, Iterable, Optional, Union
 
 import torch
-
+from aac_metrics.classes.cider_d import CIDErD
+from aac_metrics.classes.fense import FENSE
 from pytorch_lightning import LightningModule
 from pytorch_lightning.callbacks.callback import Callback
 from torch import nn
 
-from aac_metrics.classes.cider_d import CIDErD
-from aac_metrics.classes.fense import FENSE
-
 from conette.metrics.classes.diversity import Diversity
 from conette.metrics.classes.text_stats import TextStats
 from conette.nn.functional.get import get_device
 
 
 class AACValidator(Callback):
     def __init__(
         self,
         monitors: Union[str, Iterable[str]],
         metrics_keys: Union[str, Iterable[str]] = (),
-        computation_device: Union[str, torch.device, None] = "auto",
+        computation_device: Union[str, torch.device, None] = "cuda_if_available",
         other_device: Union[str, torch.device, None] = "cpu",
         build_on_start: bool = False,
     ) -> None:
         if isinstance(metrics_keys, str):
             metrics_keys = [metrics_keys]
         else:
             metrics_keys = list(metrics_keys)
```

### Comparing `conette-0.2.2/src/conette/callbacks/custom_ckpt.py` & `conette-0.3.0/src/conette/callbacks/custom_ckpt.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/callbacks/debug.py` & `conette-0.3.0/src/conette/callbacks/debug.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/callbacks/deepspeed.py` & `conette-0.3.0/src/conette/callbacks/deepspeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-
 from typing import Any
 
 from deepspeed.profiling.flops_profiler import get_model_profile
 from pytorch_lightning import LightningModule
 from pytorch_lightning.callbacks.callback import Callback
 from torch import Tensor
+from torchoutil.nn.functional.others import move_to_rec
 
-from conette.nn.functional.misc import move_to_rec
 from conette.utils.csum import csum_any
 
-
 pylog = logging.getLogger(__name__)
 
 
 class DeepSpeedCallback(Callback):
     def __init__(self, single_input: bool = False, verbose: int = 0) -> None:
         super().__init__()
         self._single_input = single_input
```

### Comparing `conette-0.2.2/src/conette/callbacks/log.py` & `conette-0.3.0/src/conette/callbacks/log.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/callbacks/resume.py` & `conette-0.3.0/src/conette/callbacks/resume.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/callbacks/stats_saver.py` & `conette-0.3.0/src/conette/callbacks/stats_saver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import csv
 import logging
 import os
 import os.path as osp
-
 from argparse import Namespace
 from typing import Any, Iterable, Optional, Union
 
 import yaml
-
 from hydra.core.hydra_config import HydraConfig
 from omegaconf import DictConfig
 from pytorch_lightning import LightningDataModule, LightningModule, Trainer
 from pytorch_lightning.callbacks.callback import Callback
 from pytorch_lightning.callbacks.checkpoint import Checkpoint
 from pytorch_lightning.core.saving import save_hparams_to_yaml
 from torch import Tensor
+from torchoutil.nn.functional import count_parameters
 
 from conette.callbacks.time import TimeTrackerCallback
 from conette.info import get_install_info
-from conette.nn.functional.misc import count_params
 from conette.tokenization.aac_tokenizer import AACTokenizer
 from conette.utils.csum import csum_module
 from conette.utils.custom_logger import CustomTensorboardLogger
 from conette.utils.misc import get_current_git_hash, save_conda_env, save_micromamba_env
 
-
 pylog = logging.getLogger(__name__)
 
 
 class StatsSaver(Callback):
     """Callback for saving some stats about the training in the pylog."""
 
     def __init__(
@@ -224,16 +221,16 @@
 
     if pl_module is not None:
         save_hparams_to_yaml(
             osp.join(hp_dpath, "pl_module.yaml"),
             pl_module.hparams_initial,
         )
         other_metrics |= {
-            "total_params": count_params(pl_module, only_trainable=False),
-            "train_params": count_params(pl_module, only_trainable=True),
+            "total_params": count_parameters(pl_module, only_trainable=False),
+            "train_params": count_parameters(pl_module, only_trainable=True),
         }
 
     if datamodule is not None:
         save_hparams_to_yaml(
             osp.join(hp_dpath, "datamodule.yaml"),
             datamodule.hparams_initial,
         )
```

### Comparing `conette-0.2.2/src/conette/callbacks/time.py` & `conette-0.3.0/src/conette/callbacks/time.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/datamodules/aac_dm.py` & `conette-0.3.0/src/conette/datamodules/aac_dm.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/datamodules/collate.py` & `conette-0.3.0/src/conette/datamodules/collate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-
 from typing import Any, Iterable, Optional
 
 import torch
-
 from torch import Tensor
-
-from conette.datasets.hdf.common import SHAPE_SUFFIX
-from conette.nn.functional.misc import can_be_stacked
-from conette.nn.functional.pad import pad_sequence_rec
-from conette.utils.collections import all_eq
-
+from torchoutil.nn.functional import can_be_stacked, pad_and_stack_rec
+from torchoutil.utils.collections import all_eq
+from torchoutil.utils.hdf.common import SHAPE_SUFFIX
 
 pylog = logging.getLogger(__name__)
 
 
 class CollateDict:
     """Collate list of dict into a dict of list WITHOUT auto-padding."""
 
@@ -95,15 +90,15 @@
                         )
                         continue
 
                     shapes = torch.as_tensor(shapes)
                     batch_dic[key_shape] = shapes
 
                 pad_value = self._pad_values[key]
-                items = pad_sequence_rec(items, pad_value=pad_value)
+                items = pad_and_stack_rec(items, pad_value=pad_value)
 
             elif (
                 not key.endswith(SHAPE_SUFFIX)
                 and all(isinstance(item, Tensor) for item in items)
                 and can_be_stacked(items)
             ):
                 items = torch.stack(items)
```

### Comparing `conette-0.2.2/src/conette/datamodules/common.py` & `conette-0.3.0/src/conette/datamodules/hdf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,517 +1,456 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-import math
-import random
-import re
-import os
 import os.path as osp
+from typing import Iterable, Optional, Union
 
-from collections import Counter
-from typing import Any, Callable, Iterable, Optional, Union
-
-import torch
-import yaml
-
-from nltk.util import ngrams
-from torch import Generator, Tensor
-from torch.utils.data.dataset import ConcatDataset
-
-from aac_datasets.datasets.audiocaps import AudioCaps
-
-from conette.tokenization.aac_tokenizer import AACTokenizer
-from conette.datasets.hdf import HDFDataset
-from conette.datasets.typing import SizedDatasetLike
+import tqdm
+from torch import nn
+from torch.utils.data.dataloader import DataLoader
+from torchoutil.utils.data.dataloader import get_auto_num_cpus
+from torchoutil.utils.data.dataset import TransformWrapper
+from torchoutil.utils.hdf import HDFDataset
+
+from conette.datamodules.aac_dm import AACDataModule
+from conette.datamodules.collate import AdvancedCollateDict
+from conette.datamodules.common import OnlineEncodeCaptionsTransform
 from conette.datasets.utils import (
-    TransformWrapper,
-    ZipDataset,
+    AACConcat,
+    AACDuplicate,
+    AACSelectColumnsWrapper,
+    WrapperSampler,
 )
-
+from conette.tokenization.aac_tokenizer import AACTokenizer
+from conette.utils.csum import csum_any
 
 pylog = logging.getLogger(__name__)
 
 
-def get_hdf_fpaths(
-    dataname: str,
-    subsets: Iterable[str],
-    hdf_root: str,
-    hdf_suffix: Optional[str],
-    hdf_dname: str = "HDF",
-) -> dict[str, str]:
-    """Returns the dictionary of HDF datasets filepaths for each subset :
-    ```
-    {
-        {subset_1}: {hdf_root}/{hdf_dname}/{dataname}_{subset_1}_{hdf_suffix}.hdf
-        {subset_2}: {hdf_root}/{hdf_dname}/{dataname}_{subset_2}_{hdf_suffix}.hdf
-        ...
-    }
-    ```
-    If hdf_suffix is None, returns an empty dict.
-    """
-    if hdf_suffix is None:
-        return {}
-
-    dataname = dataname.lower()
-    subsets = list(map(str.lower, subsets))
-    pattern = re.compile(
-        r"(?P<dataname>[a-z]+)_(?P<subset>[a-z]+)_(?P<hdf_suffix>.+)\.hdf"
+DEFAULT_TRAIN_COLS = ("audio", "audio_shape", "captions")
+DEFAULT_VAL_COLS = ("audio", "audio_shape", "captions")
+DEFAULT_TEST_COLS = (
+    "audio",
+    "audio_shape",
+    "captions",
+    "dataset",
+    "subset",
+    "fname",
+    "index",
+)
+
+
+class HDFDataModule(AACDataModule):
+    TUNE_MODE = False
+    _IGNORE_ARGS = (
+        "train_audio_tfm",
+        "val_audio_tfm",
+        "test_audio_tfm",
+        "train_tokenizer",
     )
-    hdf_root = osp.expandvars(hdf_root)
+    AUDIO_PADDINGS = ("batch", "longest", "crop")
 
-    if not osp.isdir(osp.join(hdf_root, hdf_dname)):
-        raise FileNotFoundError(f"Cannot find {hdf_dname} directory in {hdf_root=}.")
+    def __init__(
+        self,
+        # AACDataModule params
+        root: str = "data",
+        bsize: int = 512,
+        n_workers: Optional[int] = 0,
+        pin_memory: bool = True,
+        train_drop_last: bool = False,
+        verbose: int = 1,
+        train_cols: Iterable[str] = DEFAULT_TRAIN_COLS,
+        val_cols: Iterable[str] = DEFAULT_VAL_COLS,
+        test_cols: Iterable[str] = DEFAULT_TEST_COLS,
+        train_audio_tfm: Optional[nn.Module] = None,
+        val_audio_tfm: Optional[nn.Module] = None,
+        test_audio_tfm: Optional[nn.Module] = None,
+        train_tokenizer: Optional[AACTokenizer] = None,
+        # Other params
+        train_hdfs: Union[str, Iterable[str]] = (),
+        val_hdfs: Union[str, Iterable[str]] = (),
+        test_hdfs: Union[str, Iterable[str]] = (),
+        predict_hdfs: Union[str, Iterable[str]] = (),
+        audio_padding: str = "batch",
+        main_hdf_duplicate: Optional[str] = None,
+        main_hdf_min: Optional[str] = None,
+        main_hdf_balanced: Optional[Iterable[str]] = None,
+        n_added_data: Optional[int] = None,
+    ) -> None:
+        """Initialize the AudioCaps datamodule for building dataloaders.
 
-    hdf_fpaths = {}
+        :param root: The dataset parent directory. defaults to "data".
+        :param bsize: The batch size of the dataloaders. defaults to 512.
+        :param n_workers: The number of workers of the dataloaders. defaults to 0.
+        :param pin_memory: If True, the dataloaders will pin memory of tensors. defaults to True.
+        :param verbose: Verbose level. defaults to 1.
+        :param train_cols: The columns to extract from the original HDF dataset source during training.
+        :param val_cols: The columns to extract from the original HDF dataset source during validation.
+        :param test_cols: The columns to extract from the original HDF dataset source during testing.
+        :param train_audio_tfm: The train audio transform to apply to each item. defaults to None.
+        :param val_audio_tfm: The val audio transform to apply to each item. defaults to None.
+        :param test_audio_tfm: The test audio transform to apply to each item. defaults to None.
+        :param train_tokenizer: The AACTokenizer for train captions. None will create a default AACTokenizer. defaults to None.
+        :param train_hdfs: List of HDF filenames for training. defaults to ().
+        :param val_hdfs: List of HDF filenames for validation. defaults to ().
+        :param test_hdfs: List of HDF filenames for testing. defaults to ().
+        :param predict_hdfs: List of HDF filenames for prediction. defaults to ().
+        :param audio_padding: Audio batch padding mode. Can be one of ("batch", "crop", "longest"). defaults to "batch".
+        :param main_hdf_duplicate: Duplicate the main train dataset to have the same length than the sum of other datasets added. defaults to None.
+        :param main_hdf_min: Reduce other added per epoch to have the same length than the main train dataset. defaults to None.
+        """
+        # Process args
+        root = osp.expanduser(osp.expandvars(root))
+
+        if n_workers is None:
+            n_workers = get_auto_num_cpus()
+            if verbose >= 1:
+                pylog.info(f"Found {n_workers} CPU that will be used for DataLoaders.")
+
+        train_cols = list(train_cols)
+        val_cols = list(val_cols)
+        test_cols = list(test_cols)
+
+        def process_hdfs_args(hdfs: Union[str, Iterable[str]]) -> list[str]:
+            if isinstance(hdfs, str):
+                return [hdfs]
+            else:
+                return list(hdfs)
 
-    for subset in subsets:
-        hdf_fname = f"{dataname}_{subset}_{hdf_suffix}.hdf"
-        hdf_fpath = osp.join(hdf_root, hdf_dname, hdf_fname)
-
-        if not osp.isfile(hdf_fpath):
-            names = os.listdir(osp.join(hdf_root, hdf_dname))
-            matches = [re.match(pattern, name) for name in names]
-            availables_hdf_suffix = [
-                match["hdf_suffix"]
-                for match in matches
-                if match is not None
-                and match["dataname"] == dataname
-                and match["subset"] == subset
-            ]
+        train_hdfs = process_hdfs_args(train_hdfs)
+        val_hdfs = process_hdfs_args(val_hdfs)
+        test_hdfs = process_hdfs_args(test_hdfs)
+        predict_hdfs = process_hdfs_args(predict_hdfs)
+
+        if train_tokenizer is None:
+            train_tokenizer = AACTokenizer()
+
+        # Check args
+        if main_hdf_duplicate is not None and main_hdf_min is not None:
+            raise ValueError(
+                f"Cannot use arguments {main_hdf_duplicate=} and {main_hdf_min=} at the same time."
+            )
+        if main_hdf_duplicate is not None and main_hdf_duplicate not in train_hdfs:
+            raise ValueError(
+                f"Invalid argument {main_hdf_duplicate=}. (expected one of train hdf files {train_hdfs})"
+            )
 
-            pylog.error(
-                f"Cannot find HDF file '{hdf_fpath}' with {hdf_suffix=}.\n"
-                f"Maybe run conette-prepare before and use another hdf_suffix for {dataname}.\n"
-                f"Available hdf_suffix for '{dataname}_{subset}' are:\n{yaml.dump(availables_hdf_suffix, sort_keys=False)}"
+        if main_hdf_min is not None and main_hdf_min not in train_hdfs:
+            raise ValueError(
+                f"Invalid argument {main_hdf_min=}. (expected one of train hdf files {train_hdfs})"
             )
-        hdf_fpaths[subset] = hdf_fpath
 
-    return hdf_fpaths
+        if audio_padding not in self.AUDIO_PADDINGS:
+            raise ValueError(
+                f"Invalid argument {audio_padding=}. (expected one of {self.AUDIO_PADDINGS})"
+            )
 
+        if (
+            main_hdf_min is None
+            and main_hdf_balanced is None
+            and n_added_data is not None
+        ):
+            raise ValueError(
+                f"Invalid argument {n_added_data=} with {main_hdf_min=} and {main_hdf_balanced=}."
+            )
 
-class PreEncodedCaptionsTransform:
-    def __init__(
-        self,
-        audio_tfm: Optional[Callable],
-        ref_selection: Union[str, int, slice],
-        add_raw_refs: bool,
-        mult_captions: Union[list, Tensor],
-        mrefs_src_key: str = "captions",
-    ) -> None:
-        super().__init__()
-        self.audio_tfm = audio_tfm
-        self.ref_selection = ref_selection
-        self.mult_captions = mult_captions
-        self.add_raw_refs = add_raw_refs
-        self.mrefs_src_key = mrefs_src_key
-
-    def __call__(self, item: dict[str, Any]) -> dict[str, Any]:
-        item_idx = item["index"]
-        captions = self.mult_captions[item_idx]
-        references = item[self.mrefs_src_key]
-
-        if self.audio_tfm is not None:
-            item["audio"] = self.audio_tfm(item["audio"])
-
-        if isinstance(self.ref_selection, str):
-            if self.ref_selection == "random":
-                idxs = random.randint(0, len(captions) - 1)
-            else:
-                raise ValueError(f"Invalid argument {self.ref_selection=}.")
-        else:
-            idxs = self.ref_selection
+        if main_hdf_balanced is not None and not all(
+            hdf_name in train_hdfs for hdf_name in main_hdf_balanced
+        ):
+            raise ValueError(f"Invalid argument {main_hdf_balanced=}.")
+
+        super().__init__(
+            root=root,
+            bsize=bsize,
+            n_workers=n_workers,
+            pin_memory=pin_memory,
+            train_drop_last=train_drop_last,
+            verbose=verbose,
+            train_cols=train_cols,
+            val_cols=val_cols,
+            test_cols=test_cols,
+        )
+        self._train_audio_tfm = train_audio_tfm
+        self._val_audio_tfm = val_audio_tfm
+        self._test_audio_tfm = test_audio_tfm
+        self._train_tokenizer = train_tokenizer
+
+        self._wrapper_samplers: list[WrapperSampler] = []
+
+    def train_dataloader(self) -> DataLoader:
+        for wrapper_sampler in self._wrapper_samplers:
+            prev_csum = csum_any(wrapper_sampler.indexes)
+            wrapper_sampler.reset_indexes()
+            if self.hp.verbose >= 2:
+                csum = csum_any(wrapper_sampler.indexes)
+                pylog.debug(f"Indexes has been shuffled. ({prev_csum}, {csum})")
+        return super().train_dataloader()
+
+    # Other methods
+    def _setup_fit(self) -> None:
+        keep_padding = (
+            ("audio",) if self.hp.audio_padding in ("crop", "longest") else ()
+        )
+        train_dsets_lst = [
+            HDFDataset(
+                osp.join(self.hp.root, "HDF", fname),
+                keep_padding=keep_padding,
+                return_added_columns=True,
+            )
+            for fname in self.hp.train_hdfs
+        ]
+        val_dsets_lst = [
+            HDFDataset(
+                osp.join(self.hp.root, "HDF", fname),
+                keep_padding=keep_padding,
+                return_added_columns=True,
+            )
+            for fname in self.hp.val_hdfs
+        ]
+        if self.hp.verbose >= 2:
+            pylog.debug(
+                f"HDF datasets loaded. (train={len(train_dsets_lst)}, val={len(val_dsets_lst)})"
+            )
 
-        if isinstance(idxs, int):
-            caption = captions[idxs]
-            reference = references[idxs]
-
-            item["captions"] = caption
-            if self.add_raw_refs:
-                item["references"] = reference
-
-        elif idxs == slice(None):
-            item.pop("captions")
-            item["mult_captions"] = captions
-            if self.add_raw_refs:
-                item["mult_references"] = references
+        train_dsets_lst = [
+            AACSelectColumnsWrapper(dset, include=self.hp.train_cols)
+            for dset in train_dsets_lst
+        ]
+        val_dsets_lst = [
+            AACSelectColumnsWrapper(dset, include=self.hp.val_cols)
+            for dset in val_dsets_lst
+        ]
 
-        else:
-            raise ValueError(f"Invalid argument {idxs=} with {self.ref_selection=}.")
+        train_mrefs: list[list[str]] = [
+            refs
+            for train_dset_i in tqdm.tqdm(
+                train_dsets_lst,
+                disable=self.hp.verbose < 1,
+                desc="Loading captions for build id-to-token mappings...",
+            )
+            for refs in train_dset_i.at(None, "captions")
+        ]
 
-        return item
+        if self.hp.main_hdf_duplicate is not None:
+            tgt_idx = self.hp.train_hdfs.index(self.hp.main_hdf_duplicate)
+            tgt_dset = train_dsets_lst[tgt_idx]
+            other_sum = sum(
+                len(dset) for i, dset in enumerate(train_dsets_lst) if i != tgt_idx
+            )
 
+            if self.hp.verbose >= 1:
+                pylog.info(
+                    f"Duplicate dataset {self.hp.main_hdf_duplicate} from {len(tgt_dset)} to {other_sum}."
+                )
 
-class OnlineEncodeCaptionsTransform:
-    def __init__(
-        self,
-        audio_tfm: Optional[Callable[[Tensor], Tensor]],
-        ref_selection: Union[str, int, slice],
-        add_raw_refs: bool,
-        tokenizer: AACTokenizer,
-        encode_kwargs: dict[str, Any],
-        mrefs_src_key: Optional[str] = "captions",
-        audio_time_dim: int = -2,
-        ref_tfm: Optional[Callable[[str], str]] = None,
-    ) -> None:
-        super().__init__()
-        self.audio_tfm = audio_tfm
-        self.ref_selection = ref_selection
-        self.add_raw_refs = add_raw_refs
-        self.tokenizer = tokenizer
-        self.encode_kwargs = encode_kwargs
-        self.mrefs_src_key = mrefs_src_key
-        self.audio_time_dim = audio_time_dim
-        self.ref_tfm = ref_tfm
-
-    def __call__(self, item: dict[str, Any]) -> dict[str, Any]:
-        if self.audio_tfm is not None:
-            audio = item["audio"]
-            audio_shape = item["audio_shape"]
-            audio_len = audio_shape[self.audio_time_dim]
-            if audio_len < audio.shape[self.audio_time_dim]:
-                mask = [slice(None) for _ in range(audio.ndim)]
-                mask[self.audio_time_dim] = slice(audio_len)
-                audio[mask] = self.audio_tfm(audio[mask])
-            else:
-                audio = self.audio_tfm(audio)
-            item["audio"] = audio.contiguous()
+            if len(tgt_dset) < other_sum:
+                train_dsets_lst[tgt_idx] = AACDuplicate(tgt_dset, other_sum)  # type: ignore
 
-        if self.mrefs_src_key is not None:
-            refs = item[self.mrefs_src_key]
+        elif self.hp.main_hdf_min is not None:
+            tgt_idx = self.hp.train_hdfs.index(self.hp.main_hdf_min)
+            tgt_dset = train_dsets_lst[tgt_idx]
+            other_dsets = [
+                dset for i, dset in enumerate(train_dsets_lst) if i != tgt_idx
+            ]
+            other_dsets = AACConcat(*other_dsets)
 
-            if isinstance(self.ref_selection, str):
-                if self.ref_selection == "random":
-                    idxs = random.randint(0, len(refs) - 1)
-                else:
-                    raise ValueError(f"Invalid argument {self.ref_selection=}.")
+            if self.hp.n_added_data is not None:
+                n_added_data = self.hp.n_added_data
             else:
-                idxs = self.ref_selection
+                n_added_data = len(tgt_dset)
 
-            if isinstance(idxs, int):
-                ref = refs[idxs]
-                if self.ref_tfm is not None:
-                    ref = self.ref_tfm(ref)
-
-                cap = self.tokenizer.encode_single(
-                    ref,
-                    **self.encode_kwargs,
+            if self.hp.verbose >= 1:
+                pylog.info(
+                    f"Minimize others datasets from {len(other_dsets)} to {n_added_data}."
                 )
 
-                item["captions"] = cap
-                if self.add_raw_refs:
-                    item["references"] = ref
-
-            elif idxs == slice(None):
-                item.pop("captions")
-
-                if self.ref_tfm is not None:
-                    refs = [self.ref_tfm(ref) for ref in refs]
-
-                mcaps = self.tokenizer.encode_batch(
-                    refs,
-                    **self.encode_kwargs,
-                )
-                item["mult_captions"] = mcaps
+            other_dsets = WrapperSampler(other_dsets, n_added_data)
+            self._wrapper_samplers = [other_dsets]
+            train_dsets_lst = [tgt_dset, other_dsets]
+
+        elif self.hp.main_hdf_balanced is not None:
+            train_hdf_fnames: list[str] = list(self.hp.train_hdfs)
+            main_hdf_balanced: list[str] = list(self.hp.main_hdf_balanced)
+
+            tgt_idxs = [
+                train_hdf_fnames.index(hdf_name) for hdf_name in main_hdf_balanced
+            ]
+            tgt_dsets = [train_dsets_lst[tgt_idx] for tgt_idx in tgt_idxs]
+            other_dsets = [
+                dset for i, dset in enumerate(train_dsets_lst) if i not in tgt_idxs
+            ]
+            other_dsets = AACConcat(*other_dsets)
+
+            max_ds_size = max(map(len, tgt_dsets + [other_dsets]))
 
-                if self.add_raw_refs:
-                    item["mult_references"] = refs
+            train_dsets_lst = []
+            wrapper_samplers = []
 
+            if self.hp.n_added_data is not None:
+                n_added_data = self.hp.n_added_data
             else:
-                raise ValueError(
-                    f"Invalid argument {idxs=} with {self.ref_selection=}."
+                n_added_data = max_ds_size
+            del max_ds_size
+
+            if self.hp.verbose >= 1:
+                pylog.info(
+                    f"Minimize others datasets from {len(other_dsets)} to {n_added_data}."
                 )
 
-        return item
+            for tgt_ds in tgt_dsets + [other_dsets]:
+                if len(tgt_ds) == n_added_data:
+                    train_dsets_lst.append(tgt_ds)
+                elif len(tgt_ds) < n_added_data:
+                    train_dsets_lst.append(AACDuplicate(tgt_ds, n_added_data))
+                else:  # >
+                    wrapped = WrapperSampler(tgt_ds, n_added_data)
+                    train_dsets_lst.append(wrapped)
+                    wrapper_samplers.append(wrapped)
 
+            self._wrapper_samplers = wrapper_samplers
 
-class OnlineEncodeCaptionsTransformWithEmbs:
-    def __init__(
-        self,
-        audio_tfm: Optional[Callable],
-        ref_selection: Union[str, int, slice],
-        add_raw_refs: bool,
-        tokenizer: AACTokenizer,
-        encode_kwargs: dict[str, Any],
-        mrefs_src_key: str = "captions",
-        mrefs_embs_src_key: str = "captions_embs",
-    ) -> None:
-        super().__init__()
-        self.audio_tfm = audio_tfm
-        self.ref_selection = ref_selection
-        self.add_raw_refs = add_raw_refs
-        self.tokenizer = tokenizer
-        self.encode_kwargs = encode_kwargs
-        self.mrefs_src_key = mrefs_src_key
-        self.mrefs_embs_src_key = mrefs_embs_src_key
-
-    def __call__(self, item: dict[str, Any]) -> dict[str, Any]:
-        references = item[self.mrefs_src_key]
-        references_embs = item[self.mrefs_embs_src_key]
-
-        if self.audio_tfm is not None:
-            item["audio"] = self.audio_tfm(item["audio"])
-
-        if isinstance(self.ref_selection, str):
-            if self.ref_selection == "random":
-                idxs = random.randint(0, len(references) - 1)
-            else:
-                raise ValueError(f"Invalid argument {self.ref_selection=}.")
         else:
-            idxs = self.ref_selection
-
-        if isinstance(idxs, int):
-            reference = references[idxs]
-            caption = self.tokenizer.encode_single(
-                reference,
-                **self.encode_kwargs,
-            )
-
-            item["captions"] = caption
-            item[self.mrefs_embs_src_key] = references_embs[idxs]
-            if self.add_raw_refs:
-                item["references"] = reference
-
-        elif idxs == slice(None):
-            item.pop("captions")
-            mult_captions = self.tokenizer.encode_batch(
-                references,
-                **self.encode_kwargs,
-            )
-
-            item["mult_captions"] = mult_captions
-            item[f"mult_{self.mrefs_embs_src_key}"] = references_embs[idxs]
-            if self.add_raw_refs:
-                item["mult_references"] = references
+            if self.hp.verbose >= 1:
+                pylog.info("No change applied to added datasets.")
 
+        if len(train_dsets_lst) == 1:
+            train_dset = train_dsets_lst[0]
         else:
-            raise ValueError(f"Invalid argument {idxs=} with {self.ref_selection=}.")
+            train_dset = AACConcat(*train_dsets_lst)
 
-        return item
+        if len(val_dsets_lst) == 1:
+            val_dset = val_dsets_lst[0]
+        else:
+            val_dset = AACConcat(*val_dsets_lst)
 
+        del train_dsets_lst, val_dsets_lst
 
-def split_indexes(
-    indexes: Iterable[int],
-    ratios: Iterable[float],
-) -> list[list[int]]:
-    assert 0 <= sum(ratios) <= 1.0 + 1e-20, f"Found {sum(ratios)=} not in [0, 1]."
-    indexes = list(indexes)
-    ratio_cumsum = 0.0
-    outs = []
-    for ratio in ratios:
-        start = math.floor(ratio_cumsum * len(indexes))
-        end = math.floor((ratio_cumsum + ratio) * len(indexes))
-        sub_indexes = indexes[start:end]
-        outs.append(sub_indexes)
-        ratio_cumsum += ratio
-    return outs
-
-
-def generate_random_split(
-    size: int, ratios: Iterable[float], seed: Union[int, None, Generator]
-) -> list[list[int]]:
-    if isinstance(seed, int):
-        generator = Generator().manual_seed(seed)
-    else:
-        generator = seed
-
-    indexes = torch.randperm(size, generator=generator).tolist()
-    splitted_indexes = split_indexes(indexes, ratios)
-    return splitted_indexes
-
-
-def get_auto_num_cpus() -> int:
-    return len(os.sched_getaffinity(0))
-
-
-def auto_n_workers(n_workers: Optional[int]) -> int:
-    if n_workers is None:
-        num_cpus = get_auto_num_cpus()
-        return num_cpus
-    else:
-        return n_workers
-
-
-def build_mult_task_train_dataset(
-    train_dset: SizedDatasetLike,
-    train_tokenizer: AACTokenizer,
-    root: str,
-    audio_padding: str,
-    task_hdfs: list[str],
-    task_tag_types: list[str],
-    idx_to_name_dicts: list[dict[int, str]],
-    task_data_add: str,
-) -> SizedDatasetLike:
-    def tfm_task_0(item: dict) -> dict:
-        item["task"] = torch.as_tensor(0)
-        return item
-
-    def get_tfm_task_1(
-        task_tag_type: str,
-        idx_to_name: dict[int, str],
-    ) -> Callable:
-        assert task_tag_type in ("audioset", "fsd50k")
-
-        def tfm_task_1(item: dict) -> dict:
-            tags = item["tags"].tolist()
-
-            indexes = torch.randperm(len(tags))
-            tags = [tags[idx] for idx in indexes]
-            joined_tags_names = ", ".join(idx_to_name[tag] for tag in tags)
-            encoded_tags = train_tokenizer.encode_single(
-                joined_tags_names, default=False
-            )
-            item["captions"] = encoded_tags
-            item["task"] = torch.as_tensor(1)
-
-            return item
-
-        return tfm_task_1
-
-    train_dset_task_0 = TransformWrapper(train_dset, tfm_task_0)
-
-    train_dsets = [train_dset_task_0]
-    keep_padding = ("audio",) if audio_padding in ("crop", "longest") else ()
-
-    for task_hdf, task_tag_type, idx_to_name in zip(task_hdfs, task_tag_types, idx_to_name_dicts):  # type: ignore
-        hdf_fpath = osp.join(root, "HDF", task_hdf)  # type: ignore
-        hdf_dset = HDFDataset(
-            hdf_fpath,
-            get_tfm_task_1(task_tag_type, idx_to_name),
-            keep_padding=keep_padding,
+        if not self._train_tokenizer.is_fit():
+            train_mrefs_flat = [ref for refs in train_mrefs for ref in refs]
+            self._train_tokenizer.fit(train_mrefs_flat)
+
+        train_tfm = OnlineEncodeCaptionsTransform(
+            self._train_audio_tfm,
+            "random",
+            False,
+            self._train_tokenizer,
+            dict(add_bos_eos=True, default=None, padding=None),
+        )
+        val_tfm = OnlineEncodeCaptionsTransform(
+            self._val_audio_tfm,
+            slice(None),
+            True,
+            self._train_tokenizer,
+            dict(
+                add_bos_eos=True,
+                default=self._train_tokenizer.unk_token,
+                padding="batch",
+            ),
         )
-        train_dsets.append(hdf_dset)  # type: ignore
 
-    if task_data_add == "cat":
-        train_dset = ConcatDataset(train_dsets)
-    elif task_data_add == "cat_lim":
-        # train_dsets = [train_dset_task_0] + [
-        #     WrapperSampler(dset, len(train_dset_task_0)) for dset in train_dsets[1:]
-        # ]
-        raise NotImplementedError
-    elif task_data_add == "zip_max":
-        train_dset = ZipDataset(*train_dsets, mode="max")
-    elif task_data_add == "zip_min":
-        train_dset = ZipDataset(*train_dsets, mode="min")
-    else:
-        raise ValueError(f"Invalid argument {task_data_add=}.")
-
-    return train_dset
-
-
-def get_counter(sents: list[list[str]], nmax: int) -> Counter[tuple[str, ...]]:
-    assert nmax > 0
-    counter = Counter()
-    for n in range(1, nmax + 1):
-        for sent in sents:
-            for ngram in ngrams(sent, n):
-                assert len(ngram) == n
-                counter[ngram] += 1
-    return counter
-
-
-def build_caps_complexity_scores(
-    sents: list[list[str]], nmax: int, mode: str = "ign_ngram_sup"
-) -> Tensor:
-    assert mode in ("ign_ngram_sup", "zero_ngram_sup")
-    counter = dict(get_counter(sents, nmax))
-    count_per_ngram = [
-        sum(count for ngram, count in counter.items() if len(ngram) == n)
-        for n in range(1, nmax + 1)
-    ]
-    scores = torch.stack(
-        [
-            torch.as_tensor(
-                [
-                    (
-                        (
-                            torch.as_tensor(
-                                [
-                                    count_per_ngram[n - 1] / counter[ngram]
-                                    for ngram in ngrams(sent, n)
-                                ]
-                            ).mean()
-                        )
-                        if mode != "zero_ngram_sup" or len(sent) >= n
-                        else 0.0
-                    )
-                    for n in range(1, nmax + 1)
-                    if mode != "ign_ngram_sup" or len(sent) >= n
-                ]
-            ).mean()
-            for sent in sents
-        ]
-    )
-    max_score = scores.max().item()
-    scores = scores / max_score
-    scores = scores.numpy()
-    return scores
-
-
-def _get_unscaled_score(
-    tok_sent: list[str],
-    counter: dict[tuple[str, ...], int],
-    count_per_ngram: list[int],
-    nmax: int,
-    mode: str,
-) -> Tensor:
-    ngram_scores = []
-    for n in range(1, nmax + 1):
-        if len(tok_sent) < n:
-            if mode == "ign_ngram_sup":
-                continue
-            elif mode == "zero_ngram_sup":
-                ngram_scores.append(0.0)
-            else:
-                raise ValueError(f"Invalid argument {mode=}.")
-        else:
-            ngram_score = torch.as_tensor(
-                [
-                    count_per_ngram[n - 1] / counter[ngram]
-                    for ngram in ngrams(tok_sent, n)
-                ]
-            ).mean()
-            ngram_scores.append(ngram_score)
-    score = torch.as_tensor(ngram_scores).mean()
-    return score
-
-
-class CapsComplexity:
-    def __init__(self, nmax: int, mode: str = "ign_ngram_sup") -> None:
-        super().__init__()
-        self._nmax = nmax
-        self._mode = mode
-
-        self._counter = {}
-        self._count_per_ngram = []
-        self._max_score = 1.0
-
-    def fit(self, tok_sents: list[list[str]]) -> Tensor:
-        counter = dict(get_counter(tok_sents, self._nmax))
-        count_per_ngram = [
-            sum(count for ngram, count in counter.items() if len(ngram) == n)
-            for n in range(1, self._nmax + 1)
-        ]
+        train_dset = TransformWrapper(train_dset, train_tfm)
+        val_dset = TransformWrapper(val_dset, val_tfm)
 
-        unscaled_scores = [
-            _get_unscaled_score(sent, counter, count_per_ngram, self._nmax, self._mode)
-            for sent in tok_sents
-        ]
-        unscaled_scores = torch.as_tensor(unscaled_scores)
-        max_score = unscaled_scores.max().item()
+        self._train_dset = train_dset
+        self._val_dset = val_dset
 
-        self._counter = counter
-        self._count_per_ngram = count_per_ngram
-        self._max_score = max_score
-
-        return self.get_scores(tok_sents)
-
-    def get_scores(self, tok_sents: list[list[str]]) -> Tensor:
-        scores = torch.as_tensor([self.get_score(tok_sent) for tok_sent in tok_sents])
-        return scores
-
-    def get_score(self, tok_sent: list[str]) -> Tensor:
-        score = _get_unscaled_score(
-            tok_sent, self._counter, self._count_per_ngram, self._nmax, self._mode
+        pad_values = {
+            "captions": self._train_tokenizer.pad_token_id,
+            "mult_captions": self._train_tokenizer.pad_token_id,
+        }
+        if self.hp.audio_padding == "batch":
+            pad_values["audio"] = 0.0  # type: ignore
+
+        crop_keys = ("audio",) if self.hp.audio_padding == "crop" else ()
+        self._train_collate = AdvancedCollateDict(pad_values, crop_keys)
+        self._val_collate = AdvancedCollateDict(pad_values, crop_keys)
+
+        if self.hp.verbose >= 1:
+            vocab_size = self._train_tokenizer.get_vocab_size()
+            pylog.info(f"Train dataset size: {len(train_dset)}")
+            pylog.info(f"Validation dataset size: {len(val_dset)}")
+            pylog.info(f"Vocabulary size: {vocab_size}")
+
+    def _setup_test(self) -> None:
+        keep_padding = (
+            ("audio",) if self.hp.audio_padding in ("crop", "longest") else ()
         )
-        score = score / self._max_score
-        return score
+        dsets = {
+            fname: HDFDataset(
+                osp.join(self.hp.root, "HDF", fname),
+                keep_padding=keep_padding,
+                return_added_columns=True,
+            )
+            for fname in self.hp.test_hdfs
+        }
+        test_tfm = OnlineEncodeCaptionsTransform(
+            self._test_audio_tfm,
+            slice(None),
+            True,
+            self._train_tokenizer,
+            dict(
+                add_bos_eos=True,
+                default=self._train_tokenizer.unk_token,
+                padding="batch",
+            ),
+        )
+
+        dsets = {
+            fname: AACSelectColumnsWrapper(dset, include=self.hp.test_cols)
+            for fname, dset in dsets.items()
+        }
+        dsets = {
+            fname: TransformWrapper(dset, test_tfm) for fname, dset in dsets.items()
+        }
+
+        self._test_dsets = dsets
+
+        pad_values = {
+            "captions": self._train_tokenizer.pad_token_id,
+            "mult_captions": self._train_tokenizer.pad_token_id,
+        }
+        if self.hp.audio_padding == "batch":
+            pad_values["audio"] = 0.0  # type: ignore
+
+        crop_keys = ("audio",) if self.hp.audio_padding == "crop" else ()
+        self._test_collate = AdvancedCollateDict(pad_values, crop_keys)
+
+    def _setup_predict(self) -> None:
+        keep_padding = (
+            ("audio",) if self.hp.audio_padding in ("crop", "longest") else ()
+        )
+        dsets = {
+            fname: HDFDataset(
+                osp.join(self.hp.root, "HDF", fname),
+                keep_padding=keep_padding,
+                return_added_columns=True,
+            )
+            for fname in self.hp.predict_hdfs
+        }
+        test_tfm = OnlineEncodeCaptionsTransform(
+            self._test_audio_tfm,
+            slice(None),
+            True,
+            self._train_tokenizer,
+            dict(),
+            mrefs_src_key=None,
+        )
+
+        dsets = {
+            fname: AACSelectColumnsWrapper(
+                dset, include=self.hp.test_cols, exclude=("captions",)
+            )
+            for fname, dset in dsets.items()
+        }
+        dsets = {
+            fname: TransformWrapper(dset, test_tfm) for fname, dset in dsets.items()
+        }
+
+        self._predict_dsets = dsets
+
+        pad_values = {}
+        if self.hp.audio_padding == "batch":
+            pad_values["audio"] = 0.0  # type: ignore
+
+        crop_keys = ("audio",) if self.hp.audio_padding == "crop" else ()
+        self._predict_collate = AdvancedCollateDict(pad_values, crop_keys)
```

### Comparing `conette-0.2.2/src/conette/datasets/utils.py` & `conette-0.3.0/src/conette/datasets/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import math
 import os.path as osp
-import time
-
 from functools import cache
 from typing import (
     Any,
     Callable,
     Generic,
     Iterable,
     Mapping,
-    MutableMapping,
     Optional,
-    Sequence,
     Sized,
     TypeVar,
     Union,
 )
 
 import torch
 import torchaudio
 import tqdm
-
 from torch import Tensor
 from torch.utils.data.dataset import Dataset
 from torchaudio.backend.common import AudioMetaData
+from torchoutil.utils.data.dataset import SizedDatasetLike
 
-from conette.datasets.typing import AACDatasetLike, SizedDatasetLike
+from conette.datasets.typing import AACDatasetLike
 from conette.utils.disk_cache import disk_cache
 from conette.utils.log_utils import warn_once
 from conette.utils.misc import pass_filter
 
-
 pylog = logging.getLogger(__name__)
 T = TypeVar("T")
 
 
 def _process_idx(
     idx: Union[int, Iterable[int], Tensor, slice, None],
 ) -> Union[int, list[int], slice]:
@@ -56,24 +51,14 @@
         return idx.tolist()
     elif isinstance(idx, Iterable):
         return list(idx)
     else:
         raise TypeError(f"Invalid argument type {type(idx)=}.")
 
 
-class EmptyDataset(Generic[T], Dataset[T]):
-    def __getitem__(self, *args, **kwargs) -> None:
-        raise NotImplementedError(
-            f"Invalid call of getitem for {self.__class__.__name__}."
-        )
-
-    def __len__(self) -> int:
-        return 0
-
-
 class LambdaDataset(Generic[T], Dataset[T]):
     def __init__(
         self,
         fn: Callable[[int], Any],
         length: int,
         fn_kws: Optional[dict[str, Any]] = None,
     ) -> None:
@@ -296,69 +281,14 @@
             column = None
         return self.at(idx, column)  # type: ignore
 
     def __len__(self) -> int:
         return sum(map(len, self._source))
 
 
-class TransformWrapper(Wrapper):
-    def __init__(
-        self,
-        dataset: SizedDatasetLike,
-        transforms: Union[Callable, Iterable[Callable], None],
-        index: Union[None, int, str] = None,
-        default_kwargs: Optional[dict[str, Any]] = None,
-    ) -> None:
-        """Wrap a dataset method `getitem` with a transform."""
-        if transforms is None:
-            transforms = []
-        elif isinstance(transforms, Callable):
-            transforms = [transforms]
-        else:
-            transforms = list(transforms)
-
-        if default_kwargs is None:
-            default_kwargs = {}
-        super().__init__(dataset)
-        self._transforms = transforms
-        self._index = index
-        self._default_kwargs = default_kwargs
-
-    def apply_transform(self, item: Any) -> Any:
-        for tfm in self._transforms:
-            item = tfm(item, **self._default_kwargs)
-        return item
-
-    def __getitem__(self, idx: Any) -> Any:
-        item = self._source.__getitem__(idx)
-        if self._index is None:
-            return self.apply_transform(item)
-
-        elif isinstance(item, MutableMapping):
-            item[self._index] = self.apply_transform(
-                item[self._index], **self._default_kwargs
-            )
-            return item
-
-        elif isinstance(item, Iterable):
-            return tuple(
-                (
-                    self.apply_transform(sub_item, **self._default_kwargs)
-                    if i == self._index
-                    else sub_item
-                )
-                for i, sub_item in enumerate(item)
-            )
-
-        else:
-            raise TypeError(
-                f"Invalid item type {type(item)}. (expected dict or iterable)"
-            )
-
-
 class CacheWrap(Wrapper):
     def __init__(self, dataset: Any) -> None:
         super().__init__(dataset)
 
     @cache
     def __getitem__(self, idx: int) -> tuple:
         return self._source.__getitem__(idx)
@@ -729,96 +659,14 @@
     for lst_i in lst_of_lst[1:]:
         out = [name for name in out if name in lst_i]
         if len(out) == 0:
             break
     return out
 
 
-class Cacher(Wrapper):
-    def __init__(
-        self,
-        source: AACDatasetLike,
-        cache_keys: Optional[dict[str, str]] = None,
-    ) -> None:
-        super().__init__(source)
-
-        if cache_keys is None:
-            cache_keys = {}
-        if not all(v in ("get_raw", "get") for v in cache_keys.values()):
-            raise ValueError
-
-        null_value = "NULL"
-
-        self._cache_keys = cache_keys
-        self._caches = {
-            k: [null_value for _ in range(len(source))] for k in cache_keys.keys()
-        }
-        self._null_value = null_value
-
-    def at(self, idx: int, column: str) -> Any:
-        return self._get_cache(idx, column, "get_field")
-
-    def _get_cache(self, idx: int, column: str, type_: str) -> Any:
-        if self._cache_keys.get(column) == type_:
-            cached_value = self._caches[column][idx]
-            if cached_value != self._null_value:
-                return cached_value
-            else:
-                value = self._source.at(idx, column)
-                self._caches[column][idx] = value
-                return value
-        else:
-            value = self._source.at(idx, column)
-            return value
-
-
-class DatasetList(Dataset[T]):
-    def __init__(
-        self,
-        items: Iterable[T],
-        transform: Optional[Callable[[T], Any]] = None,
-    ) -> None:
-        if not isinstance(items, Sequence):
-            items = list(items)
-
-        super().__init__()
-        self._items = items
-        self._transform = transform
-
-    def __getitem__(self, idx: int) -> Any:
-        item = self._items[idx]
-        if self._transform is not None:
-            item = self._transform(item)
-        return item
-
-    def __len__(self) -> int:
-        return len(self._items)
-
-
-class DebugTracker(Wrapper):
-    def __init__(self, source: SizedDatasetLike) -> None:
-        super().__init__(source)
-        self._delta_sum = 0.0
-        self._delta_count = 0
-
-    def __getitem__(self, idx: int) -> Any:
-        start = time.perf_counter()
-        item = super().__getitem__(idx)
-        end = time.perf_counter()
-        self._delta_sum += end - start
-        self._delta_count += 1
-        return item
-
-    def get_average(self) -> float:
-        if self._delta_count == 0:
-            return 0.0
-        else:
-            return self._delta_sum / self._delta_count
-
-
 class AACSelectColumnsWrapper(Wrapper[AACDatasetLike]):
     """Wrapper to filter columns in AACDatasetLike.
 
     ```python
     >>> dset = ...
     >>> dset = AACSelectColumnsWrapper(dset, include=("captions",))
     >>> dset[0]
```

### Comparing `conette-0.2.2/src/conette/huggingface/config.py` & `conette-0.3.0/src/conette/huggingface/config.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/huggingface/model.py` & `conette-0.3.0/src/conette/huggingface/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-
+import pickle
 from typing import Any, Iterable, Optional, TypedDict, Union
-from typing_extensions import NotRequired
 
-import pickle
 import torch
-
 from torch import Size, Tensor
+from torchoutil.nn.functional.get import get_device
+from torchoutil.nn.functional.multilabel import probs_to_names
 from transformers import PreTrainedModel
+from typing_extensions import NotRequired
 
 from conette.huggingface.config import CoNeTTEConfig
 from conette.huggingface.preprocessor import CoNeTTEPreprocessor
 from conette.huggingface.setup import setup_other_models
-from conette.nn.functional.get import get_device
 from conette.pl_modules.base import AACLightningModule
 from conette.pl_modules.conette import CoNeTTEPLM
 from conette.tokenization.aac_tokenizer import AACTokenizer
-from conette.transforms.audioset_labels import probs_to_labels
-
+from conette.transforms.audioset_mapping import load_audioset_idx_to_name
 
 pylog = logging.getLogger(__name__)
 
 
 class CoNeTTEOutput(TypedDict):
     cands: list[str]
     preds: Tensor
@@ -39,15 +37,15 @@
 
 class CoNeTTEModel(PreTrainedModel):
     """CoNeTTE PreTrainedModel for inference."""
 
     def __init__(
         self,
         config: CoNeTTEConfig,
-        device: Union[str, torch.device, None] = "auto",
+        device: Union[str, torch.device, None] = "cuda_if_available",
         inference: bool = True,
         offline: bool = False,
         model_override: Optional[AACLightningModule] = None,
     ) -> None:
         setup_other_models(offline)
 
         preprocessor = CoNeTTEPreprocessor(verbose=config.verbose)
@@ -86,18 +84,23 @@
                 sched_n_steps=config.sched_n_steps,
                 sched_interval=config.sched_interval,
                 sched_freq=config.sched_freq,
                 train_tokenizer=tokenizer,
                 verbose=config.verbose,
             )
 
+        audioset_idx_to_name = load_audioset_idx_to_name(
+            offline=offline, verbose=config.verbose
+        )
+
         super().__init__(config)
         self.config: CoNeTTEConfig
         self.preprocessor = preprocessor
         self.model = model
+        self.audioset_idx_to_name = audioset_idx_to_name
 
         self._register_load_state_dict_pre_hook(self._pre_hook_load_state_dict)
 
         device = get_device(device)
         self.to(device=device)  # type: ignore
 
         if inference:
@@ -194,15 +197,15 @@
         max_pred_size: Optional[int] = None,
         forbid_rep_mode: Optional[str] = None,
     ) -> CoNeTTEOutput:
         # Preprocessing (load data + encode features)
         if preprocess:
             batch = self.preprocessor(x, sr, x_shapes)
             clip_probs = batch.pop("clip_probs")
-            tags = probs_to_labels(clip_probs, threshold, True, self.config.verbose)
+            tags = probs_to_names(clip_probs, threshold, self.audioset_idx_to_name)
         else:
             assert isinstance(x, Tensor) and isinstance(x_shapes, Tensor)
             batch: dict[str, Any] = {
                 "audio": x.to(self.device),
                 "audio_shape": x_shapes.to(self.device),
             }
             clip_probs = None
```

### Comparing `conette-0.2.2/src/conette/huggingface/preprocessor.py` & `conette-0.3.0/src/conette/huggingface/preprocessor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-
-from typing import Any, Iterable, TypeGuard, Union
+from typing import Any, Iterable, Union
 
 import torch
 import torchaudio
-
 from torch import Size, Tensor, nn
 from torchaudio.functional import resample
+from torchoutil.utils.collections import all_eq
 
 from conette.nn.encoders.convnext import convnext_tiny
 from conette.nn.functional.pad import pad_and_stack
-from conette.utils.collections import all_eq, unzip
-
+from conette.utils.collections import unzip
+from conette.utils.type_checks import is_iter_tensor, is_iterable_str, is_list_tensor
 
 pylog = logging.getLogger(__name__)
 
 
 class CoNeTTEPreprocessor(nn.Module):
     def __init__(self, verbose: int = 0) -> None:
         encoder = convnext_tiny(
@@ -83,15 +82,15 @@
     def _load_resample(
         self,
         x: Union[Tensor, str, Iterable[str], Iterable[Tensor]],
         sr: Union[None, int, Iterable[int]] = None,
         x_shapes: Union[Tensor, None, list[Size]] = None,
     ) -> tuple[Tensor, Tensor]:
         # LOAD
-        if _is_iter_str(x):
+        if is_iterable_str(x, accept_str=True):
             if isinstance(x, str):
                 x = [x]
             gen = (self._load(xi) for xi in x)
             x, sr = unzip(gen)
 
         else:
             if isinstance(x, Tensor):
@@ -110,29 +109,29 @@
             if isinstance(sr, int):
                 sr = [sr]
             elif sr is None:
                 sr = [self.target_sr]
             else:
                 sr = list(sr)
 
-        assert _is_list_tensor(x) or isinstance(x, Tensor), f"{type(x)=}"
+        assert is_list_tensor(x) or isinstance(x, Tensor), f"{type(x)=}"
 
         if len(sr) == 1 and len(x) != len(sr):
             sr = sr * len(x)
 
         if self.verbose >= 2:
             pylog.debug(f"Found {sr=}.")
 
         assert len(x) == len(sr) and len(x) > 0
-        assert _is_iter_tensor(x) or isinstance(x, Tensor)
+        assert is_iter_tensor(x) or isinstance(x, Tensor)
 
         # MOVE TO DEVICE
         if isinstance(x, Tensor):
             x = x.to(device=self.device)
-        elif _is_iter_tensor(x):
+        elif is_iter_tensor(x):
             x = [xi.to(device=self.device) for xi in x]
 
         # RESAMPLE + MEAN
         if any(sri != self.target_sr for sri in sr):
             if x_shapes is not None:
                 raise ValueError(f"Invalid argument {x_shapes=}.")
 
@@ -149,19 +148,7 @@
         # SHAPES + STACK
         if x_shapes is None:
             x_shapes = [xi.shape for xi in x]
         x_shapes = torch.as_tensor(x_shapes, device=self.device)
         x = pad_and_stack(x)
 
         return x, x_shapes
-
-
-def _is_iter_str(x: Any) -> TypeGuard[Iterable[str]]:
-    return isinstance(x, Iterable) and all(isinstance(xi, str) for xi in x)
-
-
-def _is_list_tensor(x: Any) -> TypeGuard[list[Tensor]]:
-    return isinstance(x, list) and all(isinstance(xi, Tensor) for xi in x)
-
-
-def _is_iter_tensor(x: Any) -> TypeGuard[Iterable[Tensor]]:
-    return isinstance(x, Iterable) and all(isinstance(xi, Tensor) for xi in x)
```

### Comparing `conette-0.2.2/src/conette/huggingface/setup.py` & `conette-0.3.0/src/conette/huggingface/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import subprocess
 import sys
-
 from subprocess import CalledProcessError
 
 import nltk
 
-from conette.transforms.audioset_labels import download_audioset_mapping
-
+from conette.transforms.audioset_mapping import download_audioset_mapping
 
 pylog = logging.getLogger(__name__)
 
 
 def setup_other_models(offline: bool = False, verbose: int = 0) -> None:
     if offline:
         return None
@@ -32,8 +30,8 @@
         )
 
     # Download stopwords list for constrained beam search
     nltk_model = "stopwords"
     nltk.download(nltk_model, quiet=verbose <= 0)
 
     # Download Audioset mapping ids in cache
-    download_audioset_mapping(verbose)
+    download_audioset_mapping(verbose=verbose)
```

### Comparing `conette-0.2.2/src/conette/info.py` & `conette-0.3.0/src/conette/info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import platform
 import sys
-
 from pathlib import Path
 
 import pytorch_lightning
 import torch
+import torchoutil
 import yaml
 
 import conette
-
 from conette import get_sample_path
 
 
 def get_package_repository_path() -> str:
     """Return the absolute path where the source code of this package is installed."""
     return str(Path(__file__).parent.parent.parent)
 
@@ -25,14 +24,15 @@
     return {
         "conette": conette.__version__,
         "python": f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}",
         "os": platform.system(),
         "architecture": platform.architecture()[0],
         "torch": str(torch.__version__),
         "lightning": pytorch_lightning.__version__,  # type: ignore
+        "torchoutil": torchoutil.__version__,
         "package_path": get_package_repository_path(),
         "sample_path": get_sample_path(),
     }
 
 
 def print_install_info() -> None:
     """Show main packages versions and paths."""
```

### Comparing `conette-0.2.2/src/conette/metrics/classes/all_metrics.py` & `conette-0.3.0/src/conette/metrics/classes/all_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import tempfile
 import time
-
 from typing import Iterable, Optional, Union
 
 import torch
-
-from torch import Tensor
-from torch.nn.parameter import Parameter
-
 from aac_metrics.classes.bert_score_mrefs import BERTScoreMRefs
 from aac_metrics.classes.bleu import BLEU
-from aac_metrics.classes.meteor import METEOR
-from aac_metrics.classes.rouge_l import ROUGEL
 from aac_metrics.classes.evaluate import Evaluate
 from aac_metrics.classes.fense import FENSE
+from aac_metrics.classes.meteor import METEOR
+from aac_metrics.classes.rouge_l import ROUGEL
 from aac_metrics.classes.spider import SPIDEr
 from aac_metrics.functional.spider_fl import _spider_fl_from_outputs
+from torch import Tensor
+from torch.nn.parameter import Parameter
 
 from conette.metrics.classes.diversity import Diversity
 from conette.metrics.classes.new_words import NewWords
 from conette.metrics.classes.text_stats import TextStats
 from conette.nn.functional.get import get_device
 
-
 pylog = logging.getLogger(__name__)
 
 
 class AllMetrics(Evaluate):
     def __init__(
         self,
         preprocess: bool = True,
-        device: Union[str, torch.device, None] = "auto",
+        device: Union[str, torch.device, None] = "cuda_if_available",
         cache_path: str = "~/.cache",
         java_path: str = "java",
         tmp_path: str = tempfile.gettempdir(),
         meteor_java_max_memory: str = "2G",
         spice_n_threads: Optional[int] = None,
         spice_java_max_memory: str = "8G",
         spice_timeout: Union[None, int, Iterable[int]] = None,
```

### Comparing `conette-0.2.2/src/conette/metrics/classes/diversity.py` & `conette-0.3.0/src/conette/metrics/classes/diversity.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/metrics/classes/jaccard.py` & `conette-0.3.0/src/conette/metrics/classes/text_stats.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,71 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from typing import Any, Optional, Union
+from typing import Callable, Union
+
+import torch
 
-from nltk.stem import SnowballStemmer
 from torch import Tensor
-from torchmetrics import Metric
 
-from conette.metrics.functional.jaccard import jaccard
+from aac_metrics.classes.base import AACMetric
 
+from conette.metrics.functional.text_stats import text_stats
 
-class Jaccard(Metric):
-    """Jaccard similarity, also known as "intersection over union"."""
 
-    is_differentiable = False
-    higher_is_better = True
+class TextStats(AACMetric):
     full_state_update = False
-
-    min_value = 0.0
-    max_value = 1.0
+    higher_is_better = True
+    is_differentiable = False
 
     def __init__(
         self,
         return_all_scores: bool = True,
-        stemmer_lang: Optional[str] = "english",
+        seed: Union[None, int, torch.Generator] = 123,
+        tokenizer: Callable[[str], list[str]] = str.split,
     ) -> None:
-        if stemmer_lang is not None:
-            stemmer = SnowballStemmer(stemmer_lang)
-        else:
-            stemmer = None
-
         super().__init__()
-        self.return_all_scores = return_all_scores
-        self.stemmer_lang = stemmer_lang
-        self.stemmer = stemmer
+        self._return_all_scores = return_all_scores
+        self._seed = seed
+        self._tokenizer = tokenizer
 
-        self.candidates = []
-        self.mult_references = []
+        self._candidates = []
+        self._mult_references = []
 
     # Metric methods
-    def compute(self) -> Union[Tensor, tuple[dict[str, Tensor], dict[str, Tensor]]]:
-        return jaccard(
-            self.candidates,
-            self.mult_references,
-            self.return_all_scores,
-            self.stemmer,
+    def compute(self) -> Union[tuple[dict[str, Tensor], dict[str, Tensor]], Tensor]:
+        return text_stats(
+            self._candidates,
+            self._mult_references,
+            self._return_all_scores,
+            self._seed,
+            self._tokenizer,
         )
 
     def get_output_names(self) -> tuple[str, ...]:
-        return ("jaccard",)
+        return (
+            "sent_len.cands",
+            "sent_len.mrefs",
+            "sent_len.ratio",
+            "vocab_len.cands",
+            "vocab_len.mrefs_full",
+            "vocab_len.ratio_full",
+            "vocab_len.mrefs_avg",
+            "vocab_len.ratio_avg",
+            "vocab_coverage",
+            "vocab_in_ref_len",
+            "vocab_in_ref_ratio",
+            "empty_sents",
+        )
 
     def reset(self) -> None:
-        self.candidates = []
-        self.mult_references = []
+        self._candidates = []
+        self._mult_references = []
         return super().reset()
 
     def update(
         self,
         candidates: list[str],
         mult_references: list[list[str]],
     ) -> None:
-        self.candidates += candidates
-        self.mult_references += mult_references
-
-    # Magic methods
-    def __getstate__(self) -> dict[str, Any]:
-        return {
-            "return_all_scores": self.return_all_scores,
-            "stemmer_lang": self.stemmer_lang,
-            "candidates": self.candidates,
-            "mult_references": self.mult_references,
-        }
-
-    def __setstate__(self, state: dict[str, Any]) -> None:
-        self.return_all_scores = state["return_all_scores"]
-        self.stemmer_lang = state["stemmer_lang"]
-        self.candidates = state["candidates"]
-        self.mult_references = state["mult_references"]
-
-        if self.stemmer_lang is not None:
-            stemmer = SnowballStemmer(self.stemmer_lang)
-        else:
-            stemmer = None
-        self.stemmer = stemmer
+        self._candidates += candidates
+        self._mult_references += mult_references
```

### Comparing `conette-0.2.2/src/conette/metrics/classes/new_words.py` & `conette-0.3.0/src/conette/metrics/classes/new_words.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/metrics/cross_referencing.py` & `conette-0.3.0/src/conette/metrics/cross_referencing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import sys
-
 from typing import Union
 
 import torch
 import tqdm
-
-from torch import Tensor
-
 from aac_metrics.classes.base import AACMetric
 from aac_metrics.utils.tokenization import preprocess_mult_sents
-from conette.metrics.classes.all_metrics import AllMetrics
+from torch import Tensor
 
+from conette.metrics.classes.all_metrics import AllMetrics
 
 pylog = logging.getLogger(__name__)
 MODES = ("random", "columns")
 
 
 def compute_cross_referencing(
     msents: list[list[str]],
```

### Comparing `conette-0.2.2/src/conette/metrics/functional/div_n.py` & `conette-0.3.0/src/conette/metrics/functional/new_words.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 
-from typing import Callable, Union
+from typing import Callable, Iterable, Union
 
 import torch
 
-from nltk.util import ngrams
 from torch import Tensor
 
 
 pylog = logging.getLogger(__name__)
 
 
-def div_n(
+def new_words(
     candidates: list[str],
     mult_references: list[list[str]],
     return_all_scores: bool = True,
-    n: int = 1,
+    train_vocab: Iterable[str] = (),
     tokenizer: Callable[[str], list[str]] = str.split,
 ) -> Union[tuple[dict[str, Tensor], dict[str, Tensor]], Tensor]:
     tok_cands = list(map(tokenizer, candidates))
-    del candidates
+    del candidates, mult_references
+
+    train_vocab = dict.fromkeys(train_vocab)
 
     dtype = torch.float64
-    diversities = _compute_div_n(tok_cands, n, dtype)
-    diversity = diversities.mean()
+    new_words_lst = [set(tokens).difference(train_vocab) for tokens in tok_cands]
+    new_words_counts = torch.as_tensor(list(map(len, new_words_lst)), dtype=dtype)
+    new_words_total = new_words_counts.mean()
 
     if return_all_scores:
         corpus_scores = {
-            "div": diversity,
+            "new_words": new_words_total,
         }
         sents_scores = {
-            "div": diversities,
+            "new_words": new_words_counts,
         }
         return corpus_scores, sents_scores
     else:
-        return diversity
-
-
-def _compute_div_n(
-    sentences: list[list[str]],
-    n: int,
-    dtype: torch.dtype,
-) -> Tensor:
-    diversities = [len(set(ngrams(sent, n))) / len(sent) for sent in sentences]
-    diversities = torch.as_tensor(diversities, dtype=dtype)
-    return diversities
+        return new_words_total
```

### Comparing `conette-0.2.2/src/conette/metrics/functional/diversity.py` & `conette-0.3.0/src/conette/metrics/functional/diversity.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/metrics/functional/text_stats.py` & `conette-0.3.0/src/conette/metrics/functional/text_stats.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/nn/decoders/aac_tfmer.py` & `conette-0.3.0/src/conette/nn/decoders/aac_tfmer.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/nn/decoding/beam.py` & `conette-0.3.0/src/conette/nn/decoding/beam.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import math
-
 from typing import Any, Optional, Union
 
 import torch
-
-from torch import nn, Tensor
-
-from conette.nn.decoding.common import AACDecoder
-from conette.nn.functional.label import ints_to_multihots
-from conette.nn.functional.mask import (
+from torch import Tensor, nn
+from torchoutil.nn.functional import (
     generate_square_subsequent_mask,
+    indices_to_multihot,
+    repeat_interleave_nd,
     tensor_to_lengths,
 )
-from conette.nn.functional.repeat import repeat_interleave_nd
 
+from conette.nn.decoding.common import AACDecoder
 
 pylog = logging.getLogger(__name__)
 
 
 @torch.no_grad()
 def generate(
     decoder: AACDecoder,
@@ -102,15 +99,15 @@
     sum_lprobs = torch.zeros((bsize * beam_size,), **fkwds)
 
     global_preds_out = torch.full((bsize * beam_size, max_pred_size), pad_id, **ikwds)
     global_is_finished = torch.full((bsize * beam_size,), False, **bkwds)
     global_avg_lprobs = torch.zeros((bsize * beam_size,), **fkwds)
 
     arange = torch.arange(bsize, **ikwds)
-    caps_in_sq_mask = generate_square_subsequent_mask(max_pred_size, device)
+    caps_in_sq_mask = generate_square_subsequent_mask(max_pred_size, device=device)
     if forbid_rep_mask is None:
         forbid_rep_mask = torch.zeros((vocab_size,), **bkwds)
     use_forbid_rep = forbid_rep_mask.eq(True).any().item()
 
     pred_size = max_pred_size
 
     for i in range(max_pred_size):
@@ -145,15 +142,17 @@
             logits_ij = logits_i[mask_ij]
             sum_lprobs_ij = sum_lprobs[mask_ij]
             # logits_ij shape: (beam_size_ij, vocab_size)
 
             if use_forbid_rep:
                 prev_preds = preds[mask_ij, : i + 1]
                 # prev_preds shape: (beam_size_ij, i+1)
-                prev_preds_mult_hot = ints_to_multihots(prev_preds, vocab_size, **bkwds)
+                prev_preds_mult_hot = indices_to_multihot(
+                    prev_preds, vocab_size, **bkwds
+                )
                 # prev_preds_ohot shape: (beam_size_ij, vocab_size)
                 prev_preds_mult_hot = prev_preds_mult_hot.logical_and_(
                     forbid_rep_mask.unsqueeze(dim=0)
                 )
                 logits_ij[prev_preds_mult_hot] = -math.inf
 
             prev_beam_idxs, next_word_idxs, sum_lprobs_ij = _select_k_next_toks(
```

### Comparing `conette-0.2.2/src/conette/nn/decoding/common.py` & `conette-0.3.0/src/conette/nn/decoding/common.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/nn/decoding/forcing.py` & `conette-0.3.0/src/conette/nn/decoding/forcing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Optional
 
 from torch import Tensor
+from torchoutil.nn.functional import generate_square_subsequent_mask, tensor_to_pad_mask
 
 from conette.nn.decoding.common import AACDecoder
-from conette.nn.functional.mask import (
-    generate_square_subsequent_mask,
-    tensor_to_pad_mask,
-)
 
 
 def teacher_forcing(
     decoder: AACDecoder,
     pad_id: int,
     bos_id: int,
     eos_id: int,
@@ -48,15 +45,17 @@
             raise ValueError(
                 "Invalid combinaison of arguments captions_pad_mask=None with captions floating-point embs."
             )
         caps_in_pad_mask = tensor_to_pad_mask(caps_in, pad_value=pad_id)
 
     if caps_in_sq_mask is None:
         caps_size = caps_in.shape[1]
-        caps_in_sq_mask = generate_square_subsequent_mask(caps_size, caps_in.device)
+        caps_in_sq_mask = generate_square_subsequent_mask(
+            caps_size, device=caps_in.device
+        )
 
     if not caps_in.is_floating_point():
         caps_in = caps_in.permute(1, 0)
     else:
         caps_in = caps_in.permute(1, 0, 2)
 
     logits = decoder(
```

### Comparing `conette-0.2.2/src/conette/nn/decoding/greedy.py` & `conette-0.3.0/src/conette/nn/decoding/greedy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import math
-
 from typing import Any, Optional
 
 import torch
-
 from torch import Tensor
+from torchoutil.nn.functional import (
+    generate_square_subsequent_mask,
+    indices_to_multihot,
+)
 
 from conette.nn.decoding.common import AACDecoder
-from conette.nn.functional.label import ints_to_multihots
-from conette.nn.functional.mask import generate_square_subsequent_mask
 
 
 @torch.no_grad()
 def greedy_search(
     decoder: AACDecoder,
     pad_id: int,
     bos_id: int,
@@ -64,15 +64,15 @@
     global_logits_out = torch.full(
         (bsize, vocab_size, max_pred_size),
         -math.inf,
         **fkwds,
     )
     global_logits_out[:, pad_id, :] = 0
 
-    caps_in_sq_mask = generate_square_subsequent_mask(max_pred_size, device)
+    caps_in_sq_mask = generate_square_subsequent_mask(max_pred_size, device=device)
     if forbid_rep_mask is None:
         forbid_rep_mask = torch.zeros((vocab_size,), **bkwds)
     use_forbid_rep = forbid_rep_mask.eq(True).any()
 
     # unfinished sentence mask
     # unfinished_mask = torch.full((bsize,), True, device=device, dtype=torch.bool)
     pred_size = max_pred_size
@@ -94,15 +94,15 @@
         # logits_i : (cur_size, vocab_size)
 
         if i < min_pred_size:
             logits_i[:, eos_id] = -math.inf
 
         if use_forbid_rep:
             prev_preds = preds[:, : i + 1]
-            prev_preds_ohot = ints_to_multihots(prev_preds, vocab_size, **bkwds)
+            prev_preds_ohot = indices_to_multihot(prev_preds, vocab_size, **bkwds)
             prev_preds_ohot = prev_preds_ohot.logical_and_(
                 forbid_rep_mask.unsqueeze(dim=0)
             )
             logits_i[prev_preds_ohot] = -math.inf
 
         next_toks_i = logits_i.argmax(dim=-1)
         # next_toks_i shape: (cur_size,)
```

### Comparing `conette-0.2.2/src/conette/nn/encoders/cnn10.py` & `conette-0.3.0/src/conette/nn/encoders/cnn10.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # BASED ON Cnn10 class from https://github.com/qiuqiangkong/audioset_tagging_cnn/blob/master/pytorch/models.py#L484
 
 import logging
-
 from typing import Any, Optional
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import yaml
-
 from torch import Tensor
-from torchlibrosa.stft import Spectrogram, LogmelFilterBank
 from torchlibrosa.augmentation import SpecAugmentation
+from torchlibrosa.stft import LogmelFilterBank, Spectrogram
 
-from conette.nn.pann_utils.models import init_bn, init_layer, do_mixup
-from conette.nn.pann_utils.models import ConvBlock
-from conette.nn.pann_utils.ckpt import pann_load_state_dict
-
+from conette.nn.ckpt import PANN_REGISTRY
+from conette.nn.pann_utils.models import ConvBlock, do_mixup, init_bn, init_layer
 
 pylog = logging.getLogger(__name__)
 
 
 class Cnn10(nn.Module):
     AUDIOSET_NUM_CLASSES = 527
     CONV_FEATURES_EMB_SIZE = 512
@@ -204,15 +200,15 @@
 
     def load_pretrained_weights(
         self,
         strict: bool = False,
         exclude_spectro_params: bool = False,
     ) -> None:
         device = self.bn0.weight.device
-        state_dict = pann_load_state_dict("Cnn10", device, offline=False)
+        state_dict = PANN_REGISTRY.load_state_dict("Cnn10", device, offline=False)
 
         if exclude_spectro_params:
             state_dict = {
                 key: weight
                 for key, weight in state_dict.items()
                 if all(
                     not key.startswith(prefix)
```

### Comparing `conette-0.2.2/src/conette/nn/encoders/cnn14.py` & `conette-0.3.0/src/conette/nn/encoders/cnn14.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/nn/encoders/cnn14_decisionlevel_att.py` & `conette-0.3.0/src/conette/nn/encoders/cnn14_decisionlevel_att.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Optional
 
 import torch
-
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.nn import functional as F
-from torchlibrosa.stft import Spectrogram, LogmelFilterBank
 from torchlibrosa.augmentation import SpecAugmentation
+from torchlibrosa.stft import LogmelFilterBank, Spectrogram
 
+from conette.nn.ckpt import PANN_REGISTRY
+from conette.nn.pann_utils.models import AttBlock, ConvBlock, init_bn, init_layer
 from conette.nn.pann_utils.pytorch_utils import (
     do_mixup,
     interpolate,
     pad_framewise_output,
 )
-from conette.nn.pann_utils.models import AttBlock, ConvBlock, init_bn, init_layer
-from conette.nn.pann_utils.ckpt import pann_load_state_dict
 from conette.transforms.audio.cutoutspec import CutOutSpec
 from conette.transforms.mixup import Mixup, sample_lambda
 
 
 class Cnn14_DecisionLevelAtt(nn.Module):
     def __init__(
         self,
@@ -119,15 +118,17 @@
         if pretrained:
             self.load_pretrained_weights()
 
         self.freeze_weights(freeze_weight)
 
     def load_pretrained_weights(self, strict: bool = False) -> None:
         device = self.fc1.weight.device
-        state_dict = pann_load_state_dict("Cnn14_DecisionLevelAtt", device, True)
+        state_dict = PANN_REGISTRY.load_state_dict(
+            "Cnn14_DecisionLevelAtt", device, True
+        )
         self.load_state_dict(state_dict, strict=strict)
 
     def init_weight(self) -> None:
         init_bn(self.bn0)
         init_layer(self.fc1)
 
     def freeze_weights(self, freeze_mode: str) -> None:
```

### Comparing `conette-0.2.2/src/conette/nn/encoders/convnext.py` & `conette-0.3.0/src/conette/nn/encoders/convnext.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from typing import Iterable, Optional
+import logging
+from typing import Any, Iterable, Optional
 
 import torch
-
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.nn.parameter import Parameter
-from torchlibrosa.stft import Spectrogram, LogmelFilterBank
 from torchlibrosa.augmentation import SpecAugmentation
+from torchlibrosa.stft import LogmelFilterBank, Spectrogram
 
 from conette.nn.functional.init import trunc_normal_
 from conette.nn.modules.drop import DropPath
 from conette.nn.modules.norm import LayerNorm
-from conette.transforms.mixup import pann_mixup
 from conette.transforms.audio.speed_perturb import SpeedPerturbation
+from conette.transforms.mixup import pann_mixup
+
+pylog = logging.getLogger(__name__)
 
 
 class ConvNeXtBlock(nn.Module):
     r"""ConvNeXt Block. There are two equivalent implementations:
     (1) DwConv -> LayerNorm (channels_first) -> 1x1 Conv -> GELU -> 1x1 Conv; all in (N, C, H, W)
     (2) DwConv -> Permute to (N, H, W, C); LayerNorm (channels_last) -> Linear -> GELU -> Linear; Permute back
     We use (2) as we find it slightly faster in PyTorch
@@ -26,15 +28,18 @@
     Args:
         dim (int): Number of input channels.
         drop_path (float): Stochastic depth rate. Default: 0.0
         layer_scale_init_value (float): Init value for Layer Scale. Default: 1e-6.
     """
 
     def __init__(
-        self, dim: int, drop_path: float = 0.0, layer_scale_init_value: float = 1e-6
+        self,
+        dim: int,
+        drop_path: float = 0.0,
+        layer_scale_init_value: float = 1e-6,
     ) -> None:
         super().__init__()
         self.dwconv = nn.Conv2d(
             dim, dim, kernel_size=7, padding=3, groups=dim
         )  # depthwise conv
         self.norm = LayerNorm(dim, eps=1e-6)
         self.pwconv1 = nn.Linear(
@@ -45,14 +50,18 @@
         self.scale_layer = (
             Parameter(layer_scale_init_value * torch.ones((dim)), requires_grad=True)
             if layer_scale_init_value > 0
             else None
         )
         self.drop_path = DropPath(drop_path) if drop_path > 0.0 else nn.Identity()
 
+        self._register_load_state_dict_pre_hook(
+            self._pre_hook_load_state_dict,
+        )
+
     def forward(self, x: Tensor) -> Tensor:
         input_ = x
         x = self.dwconv(x)
         x = x.permute(0, 2, 3, 1)  # (N, C, H, W) -> (N, H, W, C)
         x = self.norm(x)
         x = self.pwconv1(x)
         x = self.act(x)
@@ -60,14 +69,42 @@
         if self.scale_layer is not None:
             x = self.scale_layer * x
         x = x.permute(0, 3, 1, 2)  # (N, H, W, C) -> (N, C, H, W)
 
         x = input_ + self.drop_path(x)
         return x
 
+    def _pre_hook_load_state_dict(
+        self,
+        state_dict: dict[str, Tensor],
+        prefix,
+        local_metadata,
+        strict,
+        *args,
+        **kwargs,
+    ) -> Any:
+        keys = list(state_dict.keys())
+        num_fixes = 0
+        for key in keys:
+            if "gamma" not in key:
+                continue
+
+            new_key = key.replace("gamma", "scale_layer")
+            if new_key in state_dict:
+                raise RuntimeError(
+                    f"Invalid state_dict conversion. (found {key} and {new_key} at the same time)"
+                )
+            num_fixes += 1
+            state_dict[new_key] = state_dict.pop(key)
+
+        if num_fixes > 0:
+            pylog.debug(
+                f"{num_fixes} keys has been modified during loading state dict."
+            )
+
 
 class ConvNeXt(nn.Module):
     r"""ConvNeXt
         A PyTorch impl of : `A ConvNet for the 2020s`  -
           https://arxiv.org/pdf/2201.03545.pdf
 
     Args:
```

### Comparing `conette-0.2.2/src/conette/nn/encoders/ident.py` & `conette-0.3.0/src/conette/nn/encoders/ident.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/nn/functional/drop.py` & `conette-0.3.0/src/conette/nn/functional/drop.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/nn/functional/init.py` & `conette-0.3.0/src/conette/nn/functional/init.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/nn/loss/ce_mean.py` & `conette-0.3.0/src/conette/nn/loss/ce_mean.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Iterable, Optional, Union
 
-from torch import nn, Tensor
-
-from conette.nn.functional.mask import masked_mean
+from torch import Tensor, nn
+from torchoutil.nn.functional.mask import masked_mean
 
 
 class CrossEntropyLossMean(nn.CrossEntropyLoss):
     def __init__(
         self,
         weight: Optional[Tensor] = None,
         ignore_index: int = -100,
         label_smoothing: float = 0.0,
         dim: Union[int, Iterable[int], None] = None,
     ) -> None:
         """CrossEntropyLoss with dim option to average specific dimension(s) in output."""
         if isinstance(dim, Iterable):
             dim = tuple(dim)
+
         super().__init__(
             weight=weight,
             ignore_index=ignore_index,
             reduction="none",
             label_smoothing=label_smoothing,
         )
         self.dim = dim
```

### Comparing `conette-0.2.2/src/conette/nn/modules/drop.py` & `conette-0.3.0/src/conette/nn/modules/drop.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/nn/modules/misc.py` & `conette-0.3.0/src/conette/nn/modules/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import inspect
-import tqdm
-
 from dataclasses import asdict, astuple
 from typing import Any, Callable, Iterable, Mapping, Optional
 
 import torch
-
-from torch import nn, Tensor
+import tqdm
+from torch import Tensor, nn
 
 
 class AmplitudeToLog(nn.Module):
     def __init__(self, eps: float = torch.finfo(torch.float).eps) -> None:
         super().__init__()
         self.eps = eps
 
@@ -66,28 +64,14 @@
         x_out = x
         if self._preprocess is not None:
             x = self._preprocess(x)
         print(f"{self._prefix}{x=}")
         return x_out
 
 
-class AsTensor(nn.Module):
-    def __init__(self, **kwargs) -> None:
-        super().__init__()
-        self.kwargs = kwargs
-
-    def forward(self, inp: list, *args, **kwargs) -> Tensor:
-        kwargs = self.kwargs | kwargs
-        return torch.as_tensor(inp, *args, **kwargs)
-
-    def extra_repr(self) -> str:
-        kwargs_str = ",".join(f"{k}={v}" for k, v in self.kwargs.items())
-        return f"kwargs=dict({kwargs_str})"
-
-
 class ParallelDict(nn.ModuleDict):
     """Compute output of each submodule value when forward(.) is called."""
 
     def __init__(
         self, modules: Optional[dict[str, nn.Module]] = None, verbose: bool = False
     ) -> None:
         super().__init__(modules)
```

### Comparing `conette-0.2.2/src/conette/nn/modules/norm.py` & `conette-0.3.0/src/conette/nn/modules/norm.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/nn/modules/pad.py` & `conette-0.3.0/src/conette/transforms/audio/speed_perturb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,66 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import math
 import random
+from typing import Tuple, Union
 
-from torch import nn, Tensor
+from torch import Tensor, nn
+from torchoutil.nn.modules import CropDim, PadDim
 
-from conette.nn.functional.pad import (
-    pad_dim,
-)
+from conette.transforms.audio.resample import ResampleNearest
 
 
-class PadDim(nn.Module):
-    ALIGNS = ("left", "right", "center", "random")
-
+class SpeedPerturbation(nn.Module):
     def __init__(
         self,
-        target_length: int,
-        align: str = "left",
+        rates: Tuple[float, float] = (0.9, 1.1),
+        target_length: Union[int, str, None] = "same",
+        align: str = "random",
         fill_value: float = 0.0,
         dim: int = -1,
-        mode: str = "constant",
         p: float = 1.0,
     ) -> None:
-        """PadDim on tensor with alignment option.
-
-        Example :
+        """Resample, Pad and Crop a signal.
 
-        >>> import torch; from torch import tensor
-        >>> x = torch.ones(6)
-        >>> zero_pad = Pad(10, align='right')
-        >>> zero_pad(x)
-        ... tensor([0, 0, 0, 0, 1, 1, 1, 1, 1, 1])
-
-        :param target_length: The target length of the dimension.
-        :param align: The alignment type. Can be 'left', 'right', 'center' or 'random'. (default: 'left')
-        :param fill_value: The fill value used for constant padding. (default: 0.0)
-        :param dim: The dimension to pad. (default: -1)
-        :param mode: The padding mode. Can be 'constant', 'reflect', 'replicate' or 'circular'. (default: 'constant')
-        :param p: The probability to apply the transform. (default: 1.0)
+        :param rates: The ratio of the signal used for resize. defaults to (0.9, 1.1).
+        :param target_length: Optional target length of the signal dimension.
+                If 'same', the output will have the same shape than the input.
+                defaults to "same".
+        :param align: Alignment to use for cropping and padding. Can be 'left', 'right', 'center' or 'random'.
+                defaults to "random".
+        :param fill_value: The fill value when padding the waveform. defaults to 0.0.
+        :param dim: The dimension to stretch and pad or crop. defaults to -1.
+        :param p: The probability to apply the transform. defaults to 1.0.
         """
-        if align not in PadDim.ALIGNS:
-            raise ValueError(
-                f"Invalid argument {align=}. (expected one of {PadDim.ALIGNS})"
-            )
+        assert 0.0 <= p
+        rates = tuple(rates)  # type: ignore
 
         super().__init__()
-        self.target_length = target_length
+        self.rates = rates
+        self._target_length = target_length
         self.align = align
         self.fill_value = fill_value
         self.dim = dim
-        self.mode = mode
         self.p = p
 
+        target_length = self.target_length if isinstance(self.target_length, int) else 1
+        self.resampler = ResampleNearest(rates, dim=dim)
+        self.pad = PadDim(target_length, align, fill_value, dim, mode="constant")  # type: ignore
+        self.crop = CropDim(target_length, align, dim)  # type: ignore
+
     # nn.Module methods
     def extra_repr(self) -> str:
         hparams = {
+            "rates": self.rates,
             "target_length": self.target_length,
             "align": self.align,
             "fill_value": self.fill_value,
             "dim": self.dim,
-            "mode": self.mode,
             "p": self.p,
         }
         return ", ".join(f"{k}={v}" for k, v in hparams.items())
 
     def forward(self, x: Tensor) -> Tensor:
         floor_p = math.floor(self.p)
         for _ in range(floor_p):
@@ -75,10 +71,22 @@
             return self.apply_transform(x)
         else:
             return x
 
     # Other methods
     def apply_transform(self, x: Tensor) -> Tensor:
         """Apply the transform without taking into account the probability p."""
-        return pad_dim(
-            x, self.target_length, self.align, self.fill_value, self.dim, self.mode
-        )
+        if self.target_length == "same":
+            target_length = x.shape[self.dim]
+            self.pad.target_length = target_length
+            self.crop.target_length = target_length
+
+        x = self.resampler(x)
+
+        if self.target_length is not None:
+            x = self.pad(x)
+            x = self.crop(x)
+        return x
+
+    @property
+    def target_length(self) -> Union[int, str, None]:
+        return self._target_length
```

### Comparing `conette-0.2.2/src/conette/nn/modules/positional_encoding.py` & `conette-0.3.0/src/conette/nn/modules/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/nn/pann_utils/hub.py` & `conette-0.3.0/src/conette/nn/pann_utils/hub.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Any, Optional, Union
 
 import torch
-
 from torch import nn
+from torchoutil.nn.functional import get_device
 
+from conette.nn.ckpt import PANN_REGISTRY
 from conette.nn.pann_utils import models
-from conette.nn.pann_utils.ckpt import (
-    PANN_PRETRAINED_URLS,
-    pann_load_state_dict,
-)
 
 
 def build_pann_model(
     model_name: str,
     pretrained: bool = True,
     model_kwargs: Optional[dict[str, Any]] = None,
-    device: Union[str, torch.device, None] = "auto",
+    device: Union[str, torch.device, None] = "cuda_if_available",
     offline: bool = False,
     verbose: int = 0,
     strict_load: bool = True,
 ) -> nn.Module:
     """Build pretrained PANN model from name.
 
     :param model_name: PANN model name. (case sensitive)
     :param pretrained: If True, load pretrained weights. defaults to True.
     :param model_kwargs: Optional keywords arguments passed to PANN model initializer. defaults to None.
-    :param device: Output device of the model. defaults to "auto".
+    :param device: Output device of the model. defaults to "cuda_if_available".
     :param offline: If True, disable automatic checkpoint downloading. defaults to False.
     :param verbose: Verbose level during model build. defaults to 0.
     :param strict_load: If True, check if checkpoint entirely corresponds to the initialized model. defaults to True.
     :returns: The PANN model built as nn.Module.
     """
-    if model_name not in PANN_PRETRAINED_URLS:
+    if model_name not in PANN_REGISTRY.names:
         raise ValueError(
-            f"Invalid argument {model_name=}. (expected one of {tuple(PANN_PRETRAINED_URLS.keys())})"
+            f"Invalid argument {model_name=}. (expected one of {tuple(PANN_REGISTRY.names)})"
         )
 
     if model_kwargs is None:
         model_kwargs = {}
 
-    if device == "auto":
-        device = "cuda" if torch.cuda.is_available() else "cpu"
-    if isinstance(device, str):
-        device = torch.device(device)
+    device = get_device(device)
 
     classpath = f"{models.__name__}.{model_name}"
     classtype = eval(classpath)
     model: nn.Module = classtype(**model_kwargs)
 
     if pretrained:
-        state_dict = pann_load_state_dict(
-            model_name_or_path=model_name,
-            offline=offline,
-            verbose=verbose,
+        state_dict = PANN_REGISTRY.load_state_dict(
+            model_name, offline=offline, verbose=verbose
         )
         model.load_state_dict(state_dict, strict=strict_load)
 
     model = model.to(device=device)
     return model
```

### Comparing `conette-0.2.2/src/conette/nn/pann_utils/models.py` & `conette-0.3.0/src/conette/nn/pann_utils/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import torch
-
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.nn import functional as F
-from torchlibrosa.stft import Spectrogram, LogmelFilterBank
 from torchlibrosa.augmentation import SpecAugmentation
+from torchlibrosa.stft import LogmelFilterBank, Spectrogram
 
 from conette.nn.pann_utils.pytorch_utils import (
     do_mixup,
     interpolate,
     pad_framewise_output,
 )
 
@@ -162,16 +161,23 @@
             return x
         elif self.activation == "sigmoid":
             return torch.sigmoid(x)
 
 
 class Cnn14(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -271,16 +277,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn14_no_specaug(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_no_specaug, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -369,16 +382,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn14_no_dropout(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_no_dropout, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -472,16 +492,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn6(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn6, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -575,16 +602,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn10(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn10, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -937,16 +971,23 @@
         x = self.layer4(x)
 
         return x
 
 
 class ResNet22(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(ResNet22, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -1043,16 +1084,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class ResNet38(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(ResNet38, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -1149,16 +1197,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class ResNet54(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(ResNet54, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -1255,16 +1310,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn14_emb512(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_emb512, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -1364,16 +1426,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn14_emb128(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_emb128, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -1473,16 +1542,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn14_emb32(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_emb32, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -1582,16 +1658,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class MobileNetV1(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(MobileNetV1, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -1775,16 +1858,23 @@
             return x + self.conv(x)
         else:
             return self.conv(x)
 
 
 class MobileNetV2(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(MobileNetV2, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -1956,25 +2046,25 @@
         if pool_size != 1:
             x = F.max_pool1d(x, kernel_size=pool_size, padding=pool_size // 2)
         return x
 
 
 class LeeNet11(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(LeeNet11, self).__init__()
 
-        window = "hann"
-        center = True
-        pad_mode = "reflect"
-        ref = 1.0
-        amin = 1e-10
-        top_db = None
-
         self.conv_block1 = LeeNetConvBlock(1, 64, 3, 3)
         self.conv_block2 = LeeNetConvBlock(64, 64, 3, 1)
         self.conv_block3 = LeeNetConvBlock(64, 64, 3, 1)
         self.conv_block4 = LeeNetConvBlock(64, 128, 3, 1)
         self.conv_block5 = LeeNetConvBlock(128, 128, 3, 1)
         self.conv_block6 = LeeNetConvBlock(128, 128, 3, 1)
         self.conv_block7 = LeeNetConvBlock(128, 128, 3, 1)
@@ -2062,25 +2152,25 @@
         if pool_size != 1:
             x = F.max_pool1d(x, kernel_size=pool_size, padding=pool_size // 2)
         return x
 
 
 class LeeNet24(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(LeeNet24, self).__init__()
 
-        window = "hann"
-        center = True
-        pad_mode = "reflect"
-        ref = 1.0
-        amin = 1e-10
-        top_db = None
-
         self.conv_block1 = LeeNetConvBlock2(1, 64, 3, 3)
         self.conv_block2 = LeeNetConvBlock2(64, 96, 3, 1)
         self.conv_block3 = LeeNetConvBlock2(96, 128, 3, 1)
         self.conv_block4 = LeeNetConvBlock2(128, 128, 3, 1)
         self.conv_block5 = LeeNetConvBlock2(128, 256, 3, 1)
         self.conv_block6 = LeeNetConvBlock2(256, 256, 3, 1)
         self.conv_block7 = LeeNetConvBlock2(256, 512, 3, 1)
@@ -2220,25 +2310,25 @@
         if pool_size != 1:
             x = F.max_pool1d(x, kernel_size=pool_size, padding=pool_size // 2)
         return x
 
 
 class DaiNet19(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(DaiNet19, self).__init__()
 
-        window = "hann"
-        center = True
-        pad_mode = "reflect"
-        ref = 1.0
-        amin = 1e-10
-        top_db = None
-
         self.conv0 = nn.Conv1d(
             in_channels=1,
             out_channels=64,
             kernel_size=80,
             stride=4,
             padding=0,
             bias=False,
@@ -2481,25 +2571,25 @@
         x = self.layer7(x)
 
         return x
 
 
 class Res1dNet31(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Res1dNet31, self).__init__()
 
-        window = "hann"
-        center = True
-        pad_mode = "reflect"
-        ref = 1.0
-        amin = 1e-10
-        top_db = None
-
         self.conv0 = nn.Conv1d(
             in_channels=1,
             out_channels=64,
             kernel_size=11,
             stride=5,
             padding=5,
             bias=False,
@@ -2543,25 +2633,25 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Res1dNet51(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Res1dNet51, self).__init__()
 
-        window = "hann"
-        center = True
-        pad_mode = "reflect"
-        ref = 1.0
-        amin = 1e-10
-        top_db = None
-
         self.conv0 = nn.Conv1d(
             in_channels=1,
             out_channels=64,
             kernel_size=11,
             stride=5,
             padding=5,
             bias=False,
@@ -2648,25 +2738,25 @@
         x = F.max_pool1d(x, kernel_size=pool_size)
 
         return x
 
 
 class Wavegram_Cnn14(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Wavegram_Cnn14, self).__init__()
 
-        window = "hann"
-        center = True
-        pad_mode = "reflect"
-        ref = 1.0
-        amin = 1e-10
-        top_db = None
-
         self.pre_conv0 = nn.Conv1d(
             in_channels=1,
             out_channels=64,
             kernel_size=11,
             stride=5,
             padding=5,
             bias=False,
@@ -2747,16 +2837,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Wavegram_Logmel_Cnn14(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Wavegram_Logmel_Cnn14, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -2886,16 +2983,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Wavegram_Logmel128_Cnn14(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Wavegram_Logmel128_Cnn14, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -3025,16 +3129,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn14_16k(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_16k, self).__init__()
 
         assert sample_rate == 16000
         assert window_size == 512
         assert hop_size == 160
         assert mel_bins == 64
         assert fmin == 50
@@ -3141,16 +3252,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn14_8k(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_8k, self).__init__()
 
         assert sample_rate == 8000
         assert window_size == 256
         assert hop_size == 80
         assert mel_bins == 64
         assert fmin == 50
@@ -3257,16 +3375,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn14_mixup_time_domain(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_mixup_time_domain, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -3368,16 +3493,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn14_mel32(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_mel32, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -3477,16 +3609,23 @@
         output_dict = {"clipwise_output": clipwise_output, "embedding": embedding}
 
         return output_dict
 
 
 class Cnn14_mel128(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_mel128, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -3587,16 +3726,23 @@
 
         return output_dict
 
 
 ############
 class Cnn14_DecisionLevelMax(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_DecisionLevelMax, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -3708,16 +3854,23 @@
         }
 
         return output_dict
 
 
 class Cnn14_DecisionLevelAvg(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_DecisionLevelAvg, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
@@ -3833,16 +3986,23 @@
         }
 
         return output_dict
 
 
 class Cnn14_DecisionLevelAtt(nn.Module):
     def __init__(
-        self, sample_rate, window_size, hop_size, mel_bins, fmin, fmax, classes_num
-    ):
+        self,
+        sample_rate: int,
+        window_size: int,
+        hop_size: int,
+        mel_bins: int,
+        fmin: float,
+        fmax: float,
+        classes_num: int,
+    ) -> None:
         super(Cnn14_DecisionLevelAtt, self).__init__()
 
         window = "hann"
         center = True
         pad_mode = "reflect"
         ref = 1.0
         amin = 1e-10
```

### Comparing `conette-0.2.2/src/conette/nn/pann_utils/pytorch_utils.py` & `conette-0.3.0/src/conette/nn/pann_utils/pytorch_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import time
 
 import numpy as np
 import torch
-
 from torch import nn
 
 
 def move_data_to_device(x, device):
     if "float" in str(x.dtype):
         x = torch.Tensor(x)
     elif "int" in str(x.dtype):
@@ -274,15 +273,15 @@
 
     # Register hook
     foo(model)
 
     device = device = next(model.parameters()).device
     input = torch.rand(1, audio_length).to(device)
 
-    out = model(input)
+    model(input)
 
     total_flops = (
         sum(list_conv2d)
         + sum(list_conv1d)
         + sum(list_linear)
         + sum(list_bn)
         + sum(list_relu)
```

### Comparing `conette-0.2.2/src/conette/optim/cyclic_cos_decay.py` & `conette-0.3.0/src/conette/optim/cyclic_cos_decay.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/optim/optimizers.py` & `conette-0.3.0/src/conette/optim/optimizers.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/optim/schedulers.py` & `conette-0.3.0/src/conette/optim/schedulers.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/pl_modules/base.py` & `conette-0.3.0/src/conette/pl_modules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-
 from abc import abstractmethod
 from argparse import Namespace
 from typing import Any, Callable, ClassVar, Iterable, Mapping, Optional, Union
 
 import torch
-
-from pytorch_lightning import LightningModule, LightningDataModule, Trainer
+from pytorch_lightning import LightningDataModule, LightningModule, Trainer
 from pytorch_lightning.utilities.types import _METRIC_COLLECTION
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.nn.modules.module import _IncompatibleKeys
+from torchoutil.nn.functional import count_parameters
 
 from conette.pl_modules.common import (
-    count_params,
-    default_get_example,
+    ON_EPOCH_KWARGS,
     default_configure_optimizers,
+    default_get_example,
     has_datamodule,
     has_trainer,
-    ON_EPOCH_KWARGS,
 )
 from conette.tokenization.aac_tokenizer import AACTokenizer
 from conette.utils.csum import csum_module
 from conette.utils.log_utils import warn_once
 
-
 pylog = logging.getLogger(__name__)
 
 
 class AACLightningModule(LightningModule):
     ON_EPOCH_KWARGS: ClassVar[dict[str, Any]] = ON_EPOCH_KWARGS
 
     def __init__(
@@ -112,15 +109,19 @@
 
     @abstractmethod
     def is_built(self) -> bool:
         raise NotImplementedError("Abstract method.")
 
     @abstractmethod
     def encode_audio(
-        self, audio: Tensor, audio_shape: Tensor, *args, **kwargs
+        self,
+        audio: Tensor,
+        audio_shape: Tensor,
+        *args,
+        **kwargs,
     ) -> dict[str, Tensor]:
         raise NotImplementedError("Abstract method.")
 
     @abstractmethod
     def decode_audio(
         self,
         encoder_outs: dict[str, Tensor],
@@ -266,15 +267,15 @@
     def detokenize_text(self, *args, **kwargs) -> Any:
         return self.tokenizer.detokenize_rec(*args, **kwargs)
 
     def csum_module(self, only_trainable: bool = False) -> int:
         return csum_module(self, only_trainable=only_trainable)
 
     def count_params(self, only_trainable: bool = False) -> int:
-        return count_params(self, only_trainable)
+        return count_parameters(self, only_trainable=only_trainable)
 
     def has_datamodule(self) -> bool:
         return has_datamodule(self)
 
     def has_trainer(self) -> bool:
         return has_trainer(self)
```

### Comparing `conette-0.2.2/src/conette/pl_modules/baseline.py` & `conette-0.3.0/src/conette/pl_modules/baseline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-
 from typing import Any, Optional
 
 import torch
-
-from torch import nn, Tensor
+from torch import Tensor, nn
+from torchoutil.nn.functional import (
+    lengths_to_pad_mask,
+    randperm_diff,
+    tensor_to_pad_mask,
+)
 
 from conette.nn.decoders.aac_tfmer import AACTransformerDecoder
 from conette.nn.decoding.beam import generate
 from conette.nn.decoding.forcing import teacher_forcing
 from conette.nn.decoding.greedy import greedy_search
 from conette.nn.encoders.ident import FrameIdentEncoder
-from conette.nn.functional.indexes import randperm_diff
-from conette.nn.functional.mask import (
-    lengths_to_pad_mask,
-    tensor_to_pad_mask,
-)
 from conette.nn.loss.ce_mean import CrossEntropyLossMean
 from conette.pl_modules.base import AACLightningModule
 from conette.pl_modules.common import (
-    build_proj_lin,
-    get_forbid_rep_mask,
+    TestBatch,
     TrainBatch,
     ValBatch,
-    TestBatch,
+    build_proj_lin,
+    get_forbid_rep_mask,
 )
 from conette.tokenization.aac_tokenizer import AACTokenizer
 from conette.transforms.mixup import sample_lambda
 
-
 pylog = logging.getLogger(__name__)
 
 
 class BaselinePLM(AACLightningModule):
     def __init__(
         self,
         # Model params
@@ -99,48 +96,53 @@
                 pylog.info(f"Auto-detect value {self.hp.max_pred_size=}.")
         else:
             if self.hp.verbose >= 1:
                 pylog.info(
                     f"Set {self.hp.max_pred_size=}. (with tokenizer max={tok_max_sent_size})"
                 )
 
-        self.train_criterion = nn.CrossEntropyLoss(
+        train_criterion = nn.CrossEntropyLoss(
             ignore_index=self.pad_id,
             label_smoothing=self.hp.label_smoothing,
         )
-        self.val_criterion = CrossEntropyLossMean(ignore_index=self.pad_id, dim=1)
-        self.encoder = FrameIdentEncoder()
+        val_criterion = CrossEntropyLossMean(ignore_index=self.pad_id, dim=1)
+        encoder = FrameIdentEncoder()
 
         if self.hp.proj_name == "lin2048":
-            self.projection = build_proj_lin(2048, self.hp.d_model, False)
+            projection = build_proj_lin(2048, self.hp.d_model, False)
         elif self.hp.proj_name == "lin768":
-            self.projection = build_proj_lin(768, self.hp.d_model, False)
+            projection = build_proj_lin(768, self.hp.d_model, False)
         else:
             raise ValueError(f"Invalid argument {self.hp.proj_name=}.")
 
-        self.decoder = AACTransformerDecoder(
+        decoder = AACTransformerDecoder(
             vocab_size=self.tokenizer.get_vocab_size(),
             bos_id=self.bos_id,
             eos_id=self.eos_id,
             pad_id=self.pad_id,
             acti_name=self.hp.acti_name,
             d_model=self.hp.d_model,
             dim_feedforward=self.hp.dim_feedforward,
             dropout=self.hp.decoder_dropout_p,
             nhead=self.hp.nhead,
             num_decoder_layers=self.hp.num_decoder_layers,
         )
-
         forbid_rep_mask = get_forbid_rep_mask(
             "content_words",
             self.tokenizer,
             self.device,
             self.hp.verbose,
         )
 
+        self.train_criterion = train_criterion
+        self.val_criterion = val_criterion
+        self.encoder = encoder
+        self.projection = projection
+        self.decoder = decoder
+
         self.forbid_rep_mask: Optional[Tensor]
         self.register_buffer("forbid_rep_mask", forbid_rep_mask)
 
     def is_built(self) -> bool:
         return self.decoder is not None
 
     # --- Train, val and test methods
```

### Comparing `conette-0.2.2/src/conette/pl_modules/common.py` & `conette-0.3.0/src/conette/pl_modules/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """Common functions and arguments used in my PyTorch Lightning Modules."""
 
 import logging
-
 from typing import Any, Iterator, Mapping, Optional, TypedDict, Union
 
 import torch
 import yaml
-
 from nltk.corpus import stopwords
 from pytorch_lightning import LightningModule
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torch.optim import Optimizer
+from torchoutil.nn.modules.tensor import Transpose
 
-from conette.nn.modules.tensor import Transpose
 from conette.nn.functional.get import get_activation_module, get_device
 from conette.optim.optimizers import get_optimizer
 from conette.optim.schedulers import get_scheduler_list
 from conette.tokenization.aac_tokenizer import AACTokenizer
 
-
 pylog = logging.getLogger(__name__)
 
 ON_EPOCH_KWARGS = {
     "on_step": False,
     "on_epoch": True,
     "sync_dist": True,
 }
@@ -55,22 +52,14 @@
     mult_references: list[list[str]]
     dataset: str
     subset: str
     fname: str
     source: Optional[str]
 
 
-def count_params(model: nn.Module, only_trainable: bool = False) -> int:
-    return sum(
-        param.numel()
-        for param in model.parameters()
-        if not only_trainable or param.requires_grad
-    )
-
-
 def build_proj_lin(
     in_features: int,
     out_features: int,
     transpose_start: bool,
     dropout_p: float = 0.5,
     activation: str = "relu",
 ) -> nn.Module:
```

### Comparing `conette-0.2.2/src/conette/pl_modules/conette.py` & `conette-0.3.0/src/conette/pl_modules/conette.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
-
 from typing import Any, Iterable, Optional
 
 import torch
-
-from torch import nn, Tensor
+from torch import Tensor, nn
+from torchoutil.nn.functional import (
+    lengths_to_pad_mask,
+    randperm_diff,
+    tensor_to_pad_mask,
+)
 
 from conette.nn.decoders.aac_tfmer import AACTransformerDecoder
 from conette.nn.decoding.beam import generate
 from conette.nn.decoding.forcing import teacher_forcing
 from conette.nn.encoders.ident import FrameIdentEncoder
-from conette.nn.functional.indexes import randperm_diff
-from conette.nn.functional.mask import (
-    lengths_to_pad_mask,
-    tensor_to_pad_mask,
-)
 from conette.nn.loss.ce_mean import CrossEntropyLossMean
 from conette.pl_modules.base import AACLightningModule
 from conette.pl_modules.common import (
-    build_proj_lin,
-    get_forbid_rep_mask,
+    TestBatch,
     TrainBatch,
     ValBatch,
-    TestBatch,
+    build_proj_lin,
+    get_forbid_rep_mask,
 )
 from conette.tokenization.aac_tokenizer import AACTokenizer
 from conette.transforms.mixup import sample_lambda
 
-
 pylog = logging.getLogger(__name__)
 
 
 class CoNeTTEPLM(AACLightningModule):
     """CoNeTTE pytorch lightning module class."""
 
     def __init__(
@@ -102,15 +99,17 @@
     def build_model(self) -> None:
         if self.is_built():
             raise RuntimeError("Cannot build model twice.")
 
         # Add task emb tokens
         task_name_to_token_id = {}
         task_id_to_token_id = torch.zeros(
-            (len(self.hp.task_names),), dtype=torch.long, device=self.tch_device
+            (len(self.hp.task_names),),
+            dtype=torch.long,
+            device=self.tch_device,
         )
 
         if self.hp.task_mode == "none":
             pass
         elif self.hp.task_mode in ("ds", "ds_src"):
             for i, task_name in enumerate(self.hp.task_names):
                 token = f"<bos_{task_name}>"
```

### Comparing `conette-0.2.2/src/conette/predict.py` & `conette-0.3.0/src/conette/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import csv
 import logging
 import os.path as osp
-
 from argparse import ArgumentParser, Namespace
 from typing import Optional, Union
 
 import torch
 import transformers
 import yaml
-
 from lightning_fabric.utilities.seed import seed_everything
-from omegaconf import OmegaConf, DictConfig
+from omegaconf import DictConfig, OmegaConf
 
-from conette.nn.functional.get import get_device
 from conette.huggingface.model import CoNeTTEConfig, CoNeTTEModel
+from conette.nn.functional.get import get_device
 from conette.pl_modules.baseline import BaselinePLM
 from conette.pl_modules.conette import CoNeTTEPLM
-from conette.utils.cmdline import _str_to_opt_str, _str_to_opt_int, _setup_logging
+from conette.utils.cmdline import _str_to_opt_int, _str_to_opt_str
 from conette.utils.csum import csum_module
-
+from conette.utils.log_utils import setup_logging_verbose
 
 pylog = logging.getLogger(__name__)
 
 
 def get_predict_args() -> Namespace:
     """Return main_predict arguments."""
     parser = ArgumentParser(
@@ -58,15 +56,15 @@
         help="Path to trained model directory.",
         default=None,
     )
     parser.add_argument(
         "--device",
         type=str,
         help="Torch device used to run the model.",
-        default="auto",
+        default="cuda_if_available",
     )
     parser.add_argument(
         "--token",
         type=_str_to_opt_str,
         help="Optional access token.",
         default=None,
     )
@@ -179,15 +177,15 @@
         pylog.info(f"Model from '{model_path}' is initialized.")
     return hf_model
 
 
 def main_predict() -> None:
     """Main entrypoint for CoNeTTE predict."""
     args = get_predict_args()
-    _setup_logging("conette", verbose=args.verbose, set_format=False)
+    setup_logging_verbose("conette", verbose=args.verbose, fmt=None)
     seed_everything(args.seed)
 
     fpaths = list(args.audio)
     tasks = args.task
 
     if args.model_path is not None:
         hf_model = _load_model_from_path(args.model_path, args.device, args.verbose)
```

### Comparing `conette-0.2.2/src/conette/prepare.py` & `conette-0.3.0/src/conette/prepare.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,64 +7,59 @@
 os.environ["NUMEXPR_NUM_THREADS"] = "2"
 os.environ["OMP_NUM_THREADS"] = "2"
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 os.environ["TRANSFORMERS_OFFLINE"] = "FALSE"
 os.environ["HF_HUB_OFFLINE"] = "FALSE"
 
+import copy
 import logging
 import math
 import os.path as osp
 import random
 import subprocess
 import sys
 import time
-
 from subprocess import CalledProcessError
 from typing import Any
 
 import hydra
 import nltk
 import spacy
 import torch
 import torchaudio
 import yaml
-
-from hydra.core.hydra_config import HydraConfig
-from omegaconf import DictConfig
-from torch import nn
-from torch.hub import download_url_to_file
-from torchaudio.backend.common import AudioMetaData
-
-from aac_datasets.datasets.audiocaps import AudioCaps, AudioCapsCard, _AUDIOCAPS_LINKS
+from aac_datasets.datasets.audiocaps import AudioCaps, AudioCapsCard
 from aac_datasets.datasets.clotho import Clotho, ClothoCard
 from aac_datasets.datasets.macs import MACS, MACSCard
 from aac_datasets.datasets.wavcaps import WavCaps
 from aac_metrics.download import download_metrics as download_aac_metrics
+from hydra.core.hydra_config import HydraConfig
+from omegaconf import DictConfig
+from torch import nn
+from torchaudio.backend.common import AudioMetaData
+from torchoutil.nn.functional import count_parameters
+from torchoutil.utils.data.dataset import TransformWrapper
+from torchoutil.utils.hdf import HDFDataset, pack_to_hdf
 
 from conette.callbacks.stats_saver import save_to_dir
 from conette.datamodules.common import get_hdf_fpaths
-from conette.datasets.hdf import HDFDataset, pack_to_hdf
 from conette.datasets.typing import AACDatasetLike
 from conette.datasets.utils import (
-    AACSubset,
     AACSelectColumnsWrapper,
-    TransformWrapper,
+    AACSubset,
     load_audio_metadata,
 )
-from conette.nn.functional.misc import count_params
-from conette.nn.cnext_ckpt_utils import CNEXT_PRETRAINED_URLS
-from conette.nn.pann_utils.hub import PANN_PRETRAINED_URLS
-from conette.transforms.utils import DictTransform
+from conette.nn.ckpt import CNEXT_REGISTRY, PANN_REGISTRY
+from conette.train import setup_run, teardown_run
+from conette.transforms.utils import PreSaveTransform
 from conette.utils.collections import unzip
 from conette.utils.csum import csum_any
 from conette.utils.disk_cache import disk_cache
-from conette.utils.hydra import setup_resolvers, get_subrun_path
-from conette.train import setup_run, teardown_run
-
+from conette.utils.hydra import get_subrun_path, setup_resolvers
 
 pylog = logging.getLogger(__name__)
 
 # Note: this function must be called globally
 setup_resolvers()
 
 
@@ -83,15 +78,15 @@
             nltk.download(model_name)
 
     if cfg.spacy:
         # Download spaCy model for AACTokenizer
         SPACY_MODELS = ("en_core_web_sm", "fr_core_news_sm", "xx_ent_wiki_sm")
         for model_name in SPACY_MODELS:
             try:
-                _model = spacy.load(model_name)
+                spacy.load(model_name)
                 pylog.info(f"Model '{model_name}' for spacy is already downloaded.")
             except OSError:
                 command = [sys.executable, "-m", "spacy", "download", model_name]
                 try:
                     subprocess.check_call(
                         command,
                         stdout=subprocess.DEVNULL,
@@ -100,16 +95,14 @@
                     pylog.info(f"Model '{model_name}' for spacy has been downloaded.")
                 except (CalledProcessError, PermissionError) as err:  # type: ignore
                     pylog.error(
                         f"Cannot download spaCy model '{model_name}' for tokenizer. (command '{command}' with error={err})"
                     )
 
     if str(cfg.pann).lower() != "none":
-        ckpt_dir = osp.join(torch.hub.get_dir(), "checkpoints")
-        os.makedirs(ckpt_dir, exist_ok=True)
 
         def can_download(name: str, pattern: Any) -> bool:
             if pattern == "all":
                 return True
             elif isinstance(pattern, str):
                 return name.lower() == pattern.lower()
             elif isinstance(pattern, list):
@@ -117,54 +110,34 @@
             elif isinstance(pattern, (bool, int)):
                 return can_download(name, "all" if pattern else "none")
             else:
                 raise TypeError(
                     f"Invalid cfg.pann argument. Must be a string, a list of strings, a bool or an int, found {pattern.__class__.__name__}."
                 )
 
-        urls = {
-            name: model_info
-            for name, model_info in PANN_PRETRAINED_URLS.items()
-            if can_download(name, cfg.pann)
-        }
+        register = PANN_REGISTRY
+        names = [
+            model_name
+            for model_name in register.names
+            if can_download(model_name, cfg.pann)
+        ]
 
-        for i, (name, model_info) in enumerate(urls.items()):
-            fpath = osp.join(ckpt_dir, model_info["fname"])
-
-            if osp.isfile(fpath):
-                pylog.info(
-                    f"Model '{name}' already downloaded in '{fpath}'. ({i+1}/{len(urls)})"
-                )
-            else:
-                pylog.info(
-                    f"Start downloading pre-trained PANN model '{name}' ({i+1}/{len(urls)})..."
-                )
-                download_url_to_file(
-                    model_info["url"], fpath, progress=cfg.verbose >= 1
-                )
-                pylog.info(f"Model '{name}' downloaded in '{fpath}'.")
+        for i, model_name in enumerate(names):
+            pylog.info(
+                f"Start downloading pre-trained PANN model '{model_name}' ({i+1}/{len(names)})..."
+            )
+            register.download_file(model_name, verbose=cfg.verbose)
 
     if cfg.cnext:
-        ckpt_dpath = osp.join(torch.hub.get_dir(), "checkpoints")
-        urls = CNEXT_PRETRAINED_URLS
-
-        for i, (name, info) in enumerate(urls.items()):
-            url = info["url"]
-            fname = info["fname"]
-            fpath = osp.join(ckpt_dpath, fname)
-
-            if osp.isfile(fpath):
-                pylog.info(
-                    f"Model '{name}' already downloaded in '{fpath}'. ({i+1}/{len(urls)})"
-                )
-            else:
-                pylog.info(
-                    f"Start downloading pre-trained CNext model '{name}' ({i+1}/{len(urls)})..."
-                )
-                download_url_to_file(url, fpath, progress=cfg.verbose >= 1)
+        register = CNEXT_REGISTRY
+        for i, model_name in enumerate(register.names):
+            pylog.info(
+                f"Start downloading pre-trained CNext model '{model_name}' ({i+1}/{len(register.names)})..."
+            )
+            register.download_file(model_name, verbose=cfg.verbose)
 
 
 def download_dataset(cfg: DictConfig) -> dict[str, AACDatasetLike]:
     # Download a dataset
     hydra_cfg = HydraConfig.get()
     dataname = hydra_cfg.runtime.choices["data"]
 
@@ -179,39 +152,14 @@
         AudioCaps.FORCE_PREPARE_DATA = False
 
         if cfg.data.subsets is None:
             subsets = AudioCapsCard.SUBSETS
         else:
             subsets = cfg.data.subsets
 
-        if cfg.data.audiocaps_caps_fix_fpath is not None:
-            if "train" not in subsets:
-                pylog.error(
-                    f"Invalid combinaison of arguments {cfg.data.audiocaps_caps_fix_fpath=} with {subsets=}."
-                )
-            else:
-                subsets = list(subsets)
-                subsets.remove("train")
-                new_subset = osp.basename(cfg.data.audiocaps_caps_fix_fpath)[:-4]
-                subsets.append(new_subset)
-
-                AudioCaps.SUBSETS = AudioCaps.SUBSETS + (new_subset,)  # type: ignore
-                _AUDIOCAPS_LINKS.update(
-                    {
-                        new_subset: {
-                            "captions": {
-                                "url": None,
-                                "fname": osp.basename(
-                                    cfg.data.audiocaps_caps_fix_fpath
-                                ),
-                            },
-                        },
-                    }
-                )
-
         for subset in subsets:
             dsets[subset] = AudioCaps(
                 dataroot,
                 subset,
                 download=cfg.data.download,
                 verbose=cfg.verbose,
                 with_tags=cfg.data.with_tags,
@@ -251,22 +199,33 @@
                 dataroot,
                 subset=subset,
                 download=cfg.data.download,
                 verbose=cfg.verbose,
             )
 
         if cfg.data.tags_to_str:
+
+            class TagToStr(nn.Module):
+                def forward(self, item: dict[str, Any]) -> dict[str, Any]:
+                    item = copy.copy(item)
+                    item["tags"] = str(item["tags"])
+                    return item
+
+            transform = TagToStr()
             dsets = {
-                subset: TransformWrapper(dset, str, "tags")
+                subset: TransformWrapper(dset, transform)
                 for subset, dset in dsets.items()
             }
 
     elif dataname == "hdf":
         hdf_fpaths = get_hdf_fpaths(
-            cfg.data.name, cfg.data.subsets, dataroot, cfg.data.hdf_suffix
+            cfg.data.name,
+            cfg.data.subsets,
+            dataroot,
+            cfg.data.hdf_suffix,
         )
         dsets = {}
         for subset, hdf_fpath in hdf_fpaths.items():
             ds = HDFDataset(hdf_fpath)
             ds = AACSelectColumnsWrapper(ds, include=cfg.data.include_columns)
             dsets[subset] = ds
 
@@ -283,15 +242,15 @@
                 download=cfg.data.download,
                 hf_cache_dir=cfg.data.hf_cache_dir,
                 verbose=cfg.verbose,
             )
             for subset in subsets
         }
 
-    elif dataname in ("none",):
+    elif dataname in ("none", None, "null"):
         dsets = {}
 
     else:
         accepted_datasets = (
             "audiocaps",
             "clotho",
             "hdf",
@@ -337,16 +296,19 @@
     meta_dic: dict[str, list[AudioMetaData]] = {}
 
     if use_duration_filt or use_sr_filt:
         for subset, ds in dsets.items():
             fpaths = ds[:, "fpath"]
             if cfg.verbose >= 2:
                 pylog.debug(f"Loading durations from {len(ds)} audio files...")
+
             meta_lst = disk_cache(
-                load_audio_metadata, fpaths, cache_path=cfg.path.cache
+                load_audio_metadata,
+                fpaths,
+                cache_path=cfg.path.cache,
             )
             meta_dic[subset] = list(meta_lst.values())
 
     if use_range_filt:
         if cfg.verbose >= 1:
             pylog.info(
                 f"Limit datasets in [{cfg.datafilter.imin}, {cfg.datafilter.imax}]."
@@ -396,15 +358,15 @@
 
             n_excluded = prev_size - len(indexes)
             if cfg.verbose >= 1:
                 pylog.info(
                     f"Exclude {n_excluded}/{prev_size} files with sample_rate != {cfg.datafilter.sr} Hz in {subset=}."
                 )
 
-    dsets = {subset: AACSubset(ds, indexes_dic[subset]) for subset, ds in dsets.items()}
+    dsets = {subset: AACSubset(ds, indexes_dic[subset]) for subset, ds in dsets.items()}  # type: ignore
     return dsets
 
 
 def pack_dsets_to_hdf(cfg: DictConfig, dsets: dict[str, Any]) -> None:
     if not cfg.pack_to_hdf:
         return None
 
@@ -446,19 +408,19 @@
         audio_transform_params = dict(cfg.audio_t)
         sentence_transform_params = dict(cfg.text_t)
 
         audio_tfm = hydra.utils.instantiate(audio_transform_params)
         text_tfm = hydra.utils.instantiate(sentence_transform_params)
 
         if isinstance(audio_tfm, nn.Module) and cfg.verbose >= 1:
-            n_params = count_params(audio_tfm, only_trainable=False)
+            n_params = count_parameters(audio_tfm, only_trainable=False)
             pylog.info(f"Nb params in audio transform: {n_params}")
 
         if isinstance(text_tfm, nn.Module) and cfg.verbose >= 1:
-            n_params = count_params(text_tfm, only_trainable=False)
+            n_params = count_parameters(text_tfm, only_trainable=False)
             pylog.info(f"Nb params in text transform: {n_params}")
 
         pre_save_transforms = {
             "audio": audio_tfm,
             "captions": text_tfm,
         }
         transforms_params = {
@@ -492,27 +454,30 @@
             }
             if hasattr(cfg.audio_t, "tgt_sr"):
                 metadata["sr"] = cfg.audio_t.tgt_sr
 
             if cfg.verbose >= 1:
                 pylog.debug(yaml.dump({"Metadata": metadata}))
 
-            pre_save_transform = DictTransform(pre_save_transforms)
+            pre_save_transform = PreSaveTransform(pre_save_transforms)
+
+            num_workers = cfg.data.n_workers
+            if num_workers is None:
+                num_workers = "auto"
 
             hdf_dset = pack_to_hdf(
                 dset,
                 hdf_fpath,
                 pre_save_transform,  # type: ignore
                 overwrite=cfg.overwrite_hdf,
                 metadata=str(metadata),
                 verbose=cfg.verbose,
-                loader_bsize=cfg.data.bsize,
-                loader_n_workers=cfg.data.n_workers,
+                batch_size=cfg.data.bsize,
+                num_workers=num_workers,
             )
-            hdf_dset.open()
         else:
             if cfg.verbose >= 1:
                 pylog.info(
                     f"Dataset {dataname}_{subset} is already packed to hdf in {hdf_fpath=}."
                 )
 
             hdf_dset = HDFDataset(hdf_fpath)
```

### Comparing `conette-0.2.2/src/conette/tokenization/aac_tokenizer.py` & `conette-0.3.0/src/conette/tokenization/aac_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import json
 import logging
 import pickle
 import sys
-
 from functools import cache
 from typing import Any, Iterable, Mapping, Sized, Union
 
 import torch
 import yaml
-
-from torch import nn, Tensor
+from torch import Tensor, nn
+from torchoutil.nn.functional import get_device
 
 from conette.tokenization.normalizers import (
     CleanDoubleSpaces,
     CleanHyphenSpaces,
     CleanPunctuation,
     CleanSpacesBeforePunctuation,
     CleanSpecialTokens,
     Lowercase,
     NormalizerI,
     ReplaceRarePuncChars,
     Strip,
 )
-from conette.tokenization.tokenizers.wrapper import TokenizerWrapper
 from conette.tokenization.tokenizers.common import is_tokenized_sent_single
-from conette.tokenization.tokenizers.factory import (
-    _pre_tokenizer_factory,
-)
-
+from conette.tokenization.tokenizers.factory import _pre_tokenizer_factory
+from conette.tokenization.tokenizers.wrapper import TokenizerWrapper
 
 pylog = logging.getLogger(__name__)
 
 
 class AACTokenizer(nn.Module, TokenizerWrapper):
     """Main tokenizer facade. Provide function to encode/decode sentences to Tensor.
 
@@ -448,18 +444,15 @@
                     )
 
             tokenized_sentences = [
                 [self.token_to_id(token, default) for token in sentence]
                 for sentence in tokenized_sentences
             ]
             if out_type in ("Tensor", "pt"):
-                if device == "auto":
-                    device = "cuda" if torch.cuda.is_available() else "cpu"
-                if isinstance(device, str):
-                    device = torch.device(device)
+                device = get_device(device)
 
                 if len(tokenized_sentences) == 0 or all(
                     len(sentence) == len(tokenized_sentences[0])
                     for sentence in tokenized_sentences
                 ):
                     tokenized_sentences = torch.as_tensor(
                         tokenized_sentences,
```

### Comparing `conette-0.2.2/src/conette/tokenization/normalizers.py` & `conette-0.3.0/src/conette/tokenization/normalizers.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/tokenization/tokenizers/base.py` & `conette-0.3.0/src/conette/tokenization/tokenizers/base.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/tokenization/tokenizers/common.py` & `conette-0.3.0/src/conette/tokenization/tokenizers/common.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/tokenization/tokenizers/ptb.py` & `conette-0.3.0/src/conette/tokenization/tokenizers/ptb.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/tokenization/tokenizers/spacy.py` & `conette-0.3.0/src/conette/tokenization/tokenizers/spacy.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/tokenization/tokenizers/word.py` & `conette-0.3.0/src/conette/tokenization/tokenizers/word.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/tokenization/tokenizers/wrapper.py` & `conette-0.3.0/src/conette/tokenization/tokenizers/wrapper.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/train.py` & `conette-0.3.0/src/conette/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,51 +12,46 @@
 os.environ["HF_HUB_OFFLINE"] = "TRUE"
 
 import logging
 import math
 import os.path as osp
 import sys
 import time
-
 from typing import Callable, Optional, Union
 
 import colorlog
 import hydra
 import torch
 import yaml
-
 from hydra.utils import instantiate
 from lightning_fabric.plugins.environments import LightningEnvironment
 from omegaconf import DictConfig, OmegaConf
 from pytorch_lightning import LightningDataModule, LightningModule, Trainer
 from pytorch_lightning.callbacks import (
     Callback,
     DeviceStatsMonitor,
     EarlyStopping,
     ModelCheckpoint,
     ModelSummary,
 )
 from transformers import logging as tfmers_logging
 
-import conette
-
 from conette.callbacks.aac_evaluator import AACEvaluator
 from conette.callbacks.aac_validator import AACValidator
 from conette.callbacks.debug import PrintDebug
 from conette.callbacks.deepspeed import DeepSpeedCallback
-from conette.callbacks.log import LogGCCallback, LogLRCallback, LogGradNorm, LogRngState
+from conette.callbacks.log import LogGCCallback, LogGradNorm, LogLRCallback, LogRngState
 from conette.callbacks.resume import ResumeCallback
 from conette.callbacks.stats_saver import StatsSaver
 from conette.tokenization.aac_tokenizer import AACTokenizer
 from conette.utils.custom_logger import CustomTensorboardLogger
-from conette.utils.hydra import setup_resolvers, get_subrun_path, CustomFileHandler
-from conette.utils.log_utils import set_loglevel
+from conette.utils.hydra import CustomFileHandler, get_subrun_path, setup_resolvers
+from conette.utils.log_utils import setup_logging_level
 from conette.utils.misc import copy_slurm_logs, reset_seed
 
-
 # Note: this function must be called globally
 setup_resolvers()
 
 pylog = logging.getLogger(__name__)
 
 
 # Public functions
@@ -97,16 +92,16 @@
         other_level = logging.ERROR
         tfmers_logging.set_verbosity_error()
     else:
         pkg_level = logging.WARNING
         other_level = logging.ERROR
         tfmers_logging.set_verbosity_error()
 
-    set_loglevel(("sentence_transformers",), other_level)
-    set_loglevel((conette,), pkg_level)
+    setup_logging_level("sentence_transformers", other_level)
+    setup_logging_level("conette", pkg_level)
     pylog.setLevel(pkg_level)
 
     # Redirect PyTorch lightning outputs to a file
     os.makedirs(subrun_path, exist_ok=True)
 
     fpath_pl_outputs = osp.join(subrun_path, "logs", "lightning_outputs.log")
     handler = CustomFileHandler(fpath_pl_outputs)
@@ -323,14 +318,15 @@
             if not isinstance(ckpt, ModelCheckpoint) or ckpt.best_model_path == "":
                 continue
 
             if cfg.verbose >= 1:
                 pylog.info(
                     f"Test using best model file '{osp.basename(ckpt.best_model_path)}'..."
                 )
+
             ckpt_data = torch.load(
                 ckpt.best_model_path,
                 map_location=pl_module.device,
             )
             pl_module.load_state_dict(ckpt_data["state_dict"])
 
             if ckpt.monitor is not None:
```

### Comparing `conette-0.2.2/src/conette/transforms/audio/cutoutspec.py` & `conette-0.3.0/src/conette/transforms/audio/cutoutspec.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/transforms/audio/resample.py` & `conette-0.3.0/src/conette/transforms/audio/resample.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/transforms/audio/spec_aug.py` & `conette-0.3.0/src/conette/transforms/audio/spec_aug.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/transforms/get.py` & `conette-0.3.0/src/conette/transforms/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import os.path as osp
 import pickle
-
 from pathlib import Path
 from typing import Any, Optional, Union
 
 import torch
 import yaml
-
 from nnAudio.features import Gammatonegram
-from torch import nn, Tensor
+from torch import Tensor, nn
 from torchaudio.transforms import Resample
-from torchlibrosa.stft import Spectrogram, LogmelFilterBank
+from torchlibrosa.stft import LogmelFilterBank, Spectrogram
+from torchoutil.nn.modules.tensor import Mean, Permute, Squeeze, TensorTo, Unsqueeze
 
-from conette.nn.encoders.convnext import convnext_tiny
+from conette.nn.ckpt import CNEXT_REGISTRY, PANN_REGISTRY
 from conette.nn.encoders.cnn10 import Cnn10
-from conette.nn.encoders.cnn14_decisionlevel_att import Cnn14_DecisionLevelAtt
 from conette.nn.encoders.cnn14 import Cnn14
+from conette.nn.encoders.cnn14_decisionlevel_att import Cnn14_DecisionLevelAtt
+from conette.nn.encoders.convnext import convnext_tiny
 from conette.nn.functional.get import get_device
-from conette.nn.modules.misc import (
-    Lambda,
-    Standardize,
-)
-from conette.nn.modules.tensor import (
-    Mean,
-    Permute,
-    Squeeze,
-    TensorTo,
-    Unsqueeze,
-)
-from conette.nn.pann_utils.ckpt import pann_load_state_dict
+from conette.nn.modules.misc import Lambda, Standardize
 from conette.transforms.audio.spec_aug import SpecAugment
 
-
 pylog = logging.getLogger(__name__)
 
 
 def get_none() -> None:
     # Returns None. Can be used for hydra instantiations.
     return None
 
@@ -76,15 +64,15 @@
 def get_resample_mean_cnn10(
     src_sr: int,
     tgt_sr: int,
     mean_dim: Optional[int] = 0,
     window_size: int = 1024,
     hop_size: int = 320,
     mel_bins: int = 64,
-    device: Union[str, torch.device, None] = "auto",
+    device: Union[str, torch.device, None] = "cuda_if_available",
     transpose_frame_embs: bool = True,
 ) -> nn.Sequential:
     if not isinstance(src_sr, int):
         error_message = _get_error_message(src_sr)
         pylog.error(error_message)
         raise ValueError(error_message)
 
@@ -100,15 +88,15 @@
         pretrained=False,
         waveform_input=True,
     )
     for p in encoder.parameters():
         p.requires_grad_(False)
     encoder.eval()
 
-    state_dict = pann_load_state_dict("Cnn10", "cpu", offline=False)
+    state_dict = PANN_REGISTRY.load_state_dict("Cnn10", device="cpu", offline=False)
     encoder.load_state_dict(state_dict)
 
     encoder = encoder.to(device)
 
     def get_cnn10_embs(wave: Tensor) -> dict[str, Tensor]:
         wave = wave.unsqueeze_(dim=0)
         wave_shape = torch.as_tensor(wave.shape[1:]).unsqueeze_(dim=0)
@@ -132,15 +120,15 @@
 def get_resample_mean_cnn14_att(
     src_sr: int,
     tgt_sr: int,
     mean_dim: Optional[int] = 0,
     window_size: int = 1024,
     hop_size: int = 320,
     mel_bins: int = 64,
-    device: Union[str, torch.device, None] = "auto",
+    device: Union[str, torch.device, None] = "cuda_if_available",
     transpose_frame_embs: bool = True,
     only_frame_embs: bool = True,
 ) -> nn.Sequential:
     if not isinstance(src_sr, int):
         error_message = _get_error_message(src_sr)
         pylog.error(error_message)
         raise ValueError(error_message)
@@ -188,18 +176,18 @@
 def get_resample_mean_cnn14(
     src_sr: int,
     tgt_sr: int,
     mean_dim: Optional[int] = 0,
     window_size: int = 1024,
     hop_size: int = 320,
     mel_bins: int = 64,
-    device: Union[str, torch.device, None] = "auto",
+    device: Union[str, torch.device, None] = "cuda_if_available",
     transpose_frame_embs: bool = True,
     only_frame_embs: bool = True,
-    pretrain_path: Optional[str] = None,
+    pretrain_path: str = "Cnn14",
 ) -> nn.Sequential:
     if not isinstance(src_sr, int):
         error_message = _get_error_message(src_sr)
         pylog.error(error_message)
         raise ValueError(error_message)
 
     device = get_device(device)
@@ -210,18 +198,15 @@
         mel_bins=mel_bins,
         waveform_input=True,
         use_specaug=False,
         return_clip_outputs=True,
         return_frame_outputs=True,
     )
 
-    if pretrain_path is None:
-        state_dict = pann_load_state_dict("Cnn14", device, offline=False)
-    else:
-        state_dict = pann_load_state_dict(pretrain_path, device)
+    state_dict = PANN_REGISTRY.load_state_dict(pretrain_path, device=device)
     encoder.load_state_dict(state_dict)
 
     for p in encoder.parameters():
         p.requires_grad_(False)
     encoder.eval()
     encoder = encoder.to(device=device)
 
@@ -252,25 +237,26 @@
     )
 
 
 def get_resample_mean_convnext(
     src_sr: int,
     tgt_sr: int,
     mean_dim: Optional[int] = 0,
-    device: Union[str, torch.device, None] = "auto",
+    device: Union[str, torch.device, None] = "cuda_if_available",
     transpose_frame_embs: bool = True,
     only_frame_embs: bool = True,
-    pretrain_path: Optional[str] = None,
+    pretrain_path: Union[str, Path] = "cnext_bl_75",
+    strict: bool = True,
 ) -> nn.Sequential:
     if not isinstance(src_sr, int):
         error_message = _get_error_message(src_sr)
         pylog.error(error_message)
         raise ValueError(error_message)
 
-    if not isinstance(pretrain_path, str):
+    if not isinstance(pretrain_path, (str, Path)):
         raise ValueError(
             f"Invalid argument type {type(pretrain_path)=}. (expected str)"
         )
 
     device = get_device(device)
     encoder = convnext_tiny(
         pretrained=False,
@@ -280,17 +266,21 @@
         use_speed_perturb=False,
         waveform_input=True,
         use_specaug=False,
         return_clip_outputs=True,
         return_frame_outputs=True,
     )
 
-    data = torch.load(pretrain_path, map_location=torch.device("cpu"))
-    state_dict = data["model"]
-    encoder.load_state_dict(state_dict, strict=False)
+    cpu_device = torch.device("cpu")
+    state_dict = CNEXT_REGISTRY.load_state_dict(
+        pretrain_path,
+        device=cpu_device,
+        offline=False,
+    )
+    encoder.load_state_dict(state_dict, strict=strict)
 
     for p in encoder.parameters():
         p.requires_grad_(False)
     encoder.eval()
     encoder = encoder.to(device=device)
 
     def get_model_outputs(wave: Tensor) -> Any:
@@ -332,15 +322,15 @@
     center: bool = True,
     pad_mode: str = "reflect",
     ref: float = 1.0,
     amin: float = 1e-10,
     top_db: Optional[float] = None,
     freeze_parameters: bool = True,
     mean_dim: Optional[int] = 0,
-    device: Union[str, torch.device, None] = "auto",
+    device: Union[str, torch.device, None] = "cuda_if_available",
 ) -> nn.Sequential:
     if not isinstance(src_sr, int):
         error_message = _get_error_message(src_sr)
         pylog.error(error_message)
         raise ValueError(error_message)
 
     device = get_device(device)
@@ -453,15 +443,15 @@
     center: bool = True,
     pad_mode: str = "reflect",
     ref: float = 1.0,
     amin: float = 1e-10,
     top_db: Optional[float] = None,
     freeze_parameters: bool = True,
     mean_dim: Optional[int] = 0,
-    device: Union[str, torch.device, None] = "auto",
+    device: Union[str, torch.device, None] = "cuda_if_available",
 ) -> nn.Sequential:
     if not isinstance(src_sr, int):
         error_message = _get_error_message(src_sr)
         pylog.error(error_message)
         raise ValueError(error_message)
 
     device = get_device(device)
```

### Comparing `conette-0.2.2/src/conette/transforms/mixup.py` & `conette-0.3.0/src/conette/transforms/mixup.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/transforms/utils.py` & `conette-0.3.0/src/conette/transforms/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+import copy
 from typing import Any, Callable, Iterable, Mapping, Optional
 
-from torch import Tensor
+from torch import Tensor, nn
 
 from conette.utils.misc import pass_filter
 
 
+class PreSaveTransform(nn.ModuleDict):
+    def __init__(self, transforms: dict[str, nn.Module]) -> None:
+        super().__init__(transforms)
+
+    def forward(self, item: dict[str, Any]) -> dict[str, Any]:
+        item = copy.copy(item)
+        for name, tfm in self.items():
+            value = item[name]
+            value = tfm(value)
+            if not isinstance(value, dict):
+                item[name] = value
+            else:
+                item.pop(name)
+                for subname, subvalue in value.items():
+                    if subname == "":
+                        item[name] = subvalue
+                    else:
+                        item[subname] = subvalue
+        return item
+
+
 class DictTransform(dict[str, Optional[Callable]]):
     def __init__(
         self,
         transforms_dict: Optional[Mapping[str, Optional[Callable]]] = None,
         **transforms_kwargs: Optional[Callable],
     ) -> None:
         """Wrap a dictionary of transforms to apply to each value of a dictionary input at a corresponding key.
```

### Comparing `conette-0.2.2/src/conette/utils/collections.py` & `conette-0.3.0/src/conette/utils/collections.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,46 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import re
-
 from typing import (
     Any,
     Callable,
     Iterable,
     Mapping,
     Optional,
     Sequence,
     TypeVar,
     Union,
     overload,
 )
 
 import numpy as np
+from torchoutil.utils.collections import all_eq
 
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 W = TypeVar("W")
 
 
-def all_eq(it: Iterable[T], eq_fn: Optional[Callable[[T, T], bool]] = None) -> bool:
-    """Returns true if all elements in inputs are equal."""
-    it = list(it)
-    first = it[0]
-    if eq_fn is None:
-        return all(first == elt for elt in it)
-    else:
-        return all(eq_fn(first, elt) for elt in it)
-
-
 def all_ne(it: Iterable[T], ne_fn: Optional[Callable[[T, T], bool]] = None) -> bool:
     """Returns true if all elements in inputs are differents."""
     it = list(it)
     if ne_fn is None:
         return all(
             it[i] != it[j] for i in range(len(it)) for j in range(i + 1, len(it))
         )
     else:
         return all(
             ne_fn(it[i], it[j]) for i in range(len(it)) for j in range(i + 1, len(it))
         )
 
 
-def list_dict_to_dict_list(
-    lst: Sequence[dict[str, T]],
-    default_val: U = None,
-    error_on_missing_key: bool = False,
-) -> dict[str, list[Union[T, U]]]:
-    """Convert a list of dicts to a dict of lists.
-
-    Example 1
-    ----------
-    >>> lst = [{'a': 1, 'b': 2}, {'a': 4, 'b': 3, 'c': 5}]
-    >>> output = list_dict_to_dict_list(lst, default_val=0)
-    {'a': [1, 4], 'b': [2, 3], 'c': [0, 5]}
-    """
-    if len(lst) == 0:
-        return {}
-
-    if error_on_missing_key:
-        keys = set(lst[0])
-        for dic in lst:
-            if keys != set(dic.keys()):
-                raise ValueError(
-                    f"Invalid dict keys for list_dict_to_dict_list. (found {keys} and {dic.keys()})"
-                )
-
-    keys = {}
-    for dic in lst:
-        keys = keys | dict.fromkeys(dic.keys())
-
-    out = {
-        key: [
-            lst[i][key] if key in lst[i].keys() else default_val
-            for i in range(len(lst))
-        ]
-        for key in keys
-    }
-    return out
-
-
-def dict_list_to_list_dict(dic: dict[str, list[T]]) -> list[dict[str, T]]:
+def dict_list_to_list_dict(dic: Mapping[str, Sequence[T]]) -> list[dict[str, T]]:
     """Convert dict of lists with same sizes to list of dicts.
 
     Example 1
     ----------
     ```
     >>> dic = {"a": [1, 2], "b": [3, 4]}
     >>> dict_list_to_list_dict(dic)
@@ -96,49 +48,14 @@
     ```
     """
     assert all_eq(map(len, dic.values()))
     length = len(next(iter(dic.values())))
     return [{k: v[i] for k, v in dic.items()} for i in range(length)]
 
 
-def flat_dict_of_dict(
-    nested_dic: Mapping[str, Any],
-    sep: str = ".",
-    flat_iterables: bool = False,
-) -> dict[str, Any]:
-    """Flat a nested dictionary.
-    Example
-    ----------
-    ```
-    >>> dic = {
-    ...     "a": 1,
-    ...     "b": {
-    ...         "a": 2,
-    ...         "b": 10,
-    ...     },
-    ... }
-    >>> flat_dict(dic)
-    ... {"a": 1, "b.a": 2, "b.b": 10}
-    ```
-    """
-    output = {}
-    for k, v in nested_dic.items():
-        if isinstance(v, Mapping) and all(isinstance(kv, str) for kv in v.keys()):
-            v = flat_dict_of_dict(v, sep, flat_iterables)
-            output |= {f"{k}{sep}{kv}": vv for kv, vv in v.items()}
-        elif flat_iterables and isinstance(v, Iterable) and not isinstance(v, str):
-            output |= {
-                f"{k}{sep}{i}": flat_dict_of_dict(vv, sep, flat_iterables)
-                for i, vv in enumerate(v)
-            }
-        else:
-            output[k] = v
-    return output
-
-
 def unflat_dict_of_dict(dic: Mapping[str, Any], sep: str = ".") -> dict[str, Any]:
     """Unflat a dictionary.
 
     Example 1
     ----------
     ```
     >>> dic = {
```

### Comparing `conette-0.2.2/src/conette/utils/csum.py` & `conette-0.3.0/src/conette/utils/csum.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/utils/csv_utils.py` & `conette-0.3.0/src/conette/utils/csv_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import csv
 import os.path as osp
-
 from pathlib import Path
 from typing import Any, Iterable, Mapping, Union
 
-from conette.utils.collections import dict_list_to_list_dict, list_dict_to_dict_list
+from torchoutil.utils.collections import list_dict_to_dict_list
+
+from conette.utils.collections import dict_list_to_list_dict
 
 
 def load_csv_dict(
     fpath: Union[str, Path],
     has_fieldnames: bool = True,
     cast: bool = False,
 ) -> dict[str, list[Any]]:
     data = load_csv_list(fpath, has_fieldnames, cast)
-    data = list_dict_to_dict_list(data, None, True)
+    data = list_dict_to_dict_list(data, "same")
     return data
 
 
 def load_csv_list(
     fpath: Union[str, Path],
     has_fieldnames: bool = True,
     cast: bool = False,
```

### Comparing `conette-0.2.2/src/conette/utils/custom_logger.py` & `conette-0.3.0/src/conette/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/utils/dcase.py` & `conette-0.3.0/src/conette/utils/dcase.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/utils/disk_cache.py` & `conette-0.3.0/src/conette/utils/disk_cache.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/utils/func_utils.py` & `conette-0.3.0/src/conette/utils/func_utils.py`

 * *Files identical despite different names*

### Comparing `conette-0.2.2/src/conette/utils/hydra.py` & `conette-0.3.0/src/conette/utils/hydra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import os
 import os.path as osp
 import pickle
-
 from functools import cache
 from logging import FileHandler
 from pathlib import Path
 from typing import Any, Optional, Union
 
 from hydra.core.hydra_config import HydraConfig
 from hydra.types import RunMode
 from omegaconf import DictConfig, OmegaConf
 from omegaconf.errors import ConfigAttributeError
+from torchoutil.utils.collections import flat_dict_of_dict
 
-from conette.utils.collections import flat_dict_of_dict
 from conette.utils.yaml_utils import load_yaml
 
-
 pylog = logging.getLogger(__name__)
 
 
 class CustomFileHandler(FileHandler):
     """FileHandler which builds intermediate directories.
 
     Used for export hydra logs to a file contained in a folder that does not exists yet at the start of the program.
@@ -213,16 +211,16 @@
         elif key in choices:
             options[key] = choices[key]
         elif key in choices_clean:
             options[key] = choices_clean[key]
         else:
             value = OmegaConf.select(_root_, key, default="NOTFOUND")
             if value == "NOTFOUND":
-                dic = OmegaConf.to_container(_root_)
-                flatten = flat_dict_of_dict(dic)  # type: ignore
+                dic: dict[str, Any] = OmegaConf.to_container(_root_)  # type: ignore
+                flatten = flat_dict_of_dict(dic)
                 matches = [k for k in flatten.keys() if k.endswith(key)]
 
                 if len(matches) == 1:
                     value = OmegaConf.select(_root_, matches[0], default="NOTFOUND")
                     if value == "NOTFOUND":
                         pylog.error(
                             f"INTERNAL ERROR: Cannot find {matches[0]=} in config."
```

### Comparing `conette-0.2.2/src/conette/utils/misc.py` & `conette-0.3.0/src/conette/utils/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import datetime
-import inspect
 import logging
 import os
 import os.path as osp
 import re
 import shutil
 import subprocess
 import zipfile
-
 from pathlib import Path
 from subprocess import CalledProcessError
-from typing import (
-    Any,
-    Callable,
-    Iterable,
-    Optional,
-    TypeVar,
-    Union,
-)
+from typing import Any, Callable, Iterable, Optional, TypeVar, Union
 from zipfile import ZipFile
 
 import torch
 import tqdm
-
-from pytorch_lightning.utilities.seed import seed_everything
-
+from lightning_fabric.utilities.seed import seed_everything
 
 pylog = logging.getLogger(__name__)
 T = TypeVar("T")
 
 
 def get_none() -> None:
     # Returns None. Can be used for hydra instantiations.
@@ -67,15 +56,15 @@
     torch.backends.cudnn.deterministic = True  # type: ignore
     return seed
 
 
 def save_conda_env(fpath: str, conda_path: str = "conda", verbose: int = 1) -> bool:
     try:
         cmd = [conda_path, "env", "export", "-f", fpath]
-        _output = subprocess.check_output(cmd)
+        subprocess.check_output(cmd)
         return True
     except (CalledProcessError, PermissionError, FileNotFoundError) as err:
         if verbose >= 0:
             pylog.warning(f"Cannot save conda env in {fpath}. ({err=})")
         return False
 
 
@@ -213,15 +202,15 @@
 
     job_id = os.environ["SLURM_JOB_ID"]
     replaces = {
         "%j": job_id,
         "%A": job_id,
     }
     for pattern, value in replaces.items():
-        fpaths = [fpath.replace(pattern, value) for fpath in fpaths]
+        fpaths = [fpath.replace(pattern, value) for fpath in fpaths]  # type: ignore
     fpaths = [fpath for fpath in fpaths if osp.isfile(fpath)]
 
     if len(fpaths) == 0:
         return None
 
     tgt_dpath = osp.join(subrun_dpath, "logs")
     os.makedirs(tgt_dpath, exist_ok=True)
```

### Comparing `conette-0.2.2/src/conette.egg-info/PKG-INFO` & `conette-0.3.0/src/conette.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,96 @@
 Metadata-Version: 2.1
 Name: conette
-Version: 0.2.2
+Version: 0.3.0
 Summary: CoNeTTE is an audio captioning system, which generate a short textual description of the sound events in any audio file.
 Author-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Etienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Project-URL: Repository, https://github.com/Labbeti/conette-audio-captioning.git
 Project-URL: Changelog, https://github.com/Labbeti/conette-audio-captioning/blob/main/CHANGELOG.md
 Keywords: audio,deep-learning,pytorch,captioning,audio-captioning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: train
+Provides-Extra: test
 
 <div align="center">
 
 # CoNeTTE model for Audio Captioning
 
 [![](<https://img.shields.io/badge/-Python 3.10+-blue?style=for-the-badge&logo=python&logoColor=white>)](https://www.python.org/)
 [![](<https://img.shields.io/badge/-PyTorch 1.10.1+-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white>)](https://pytorch.org/get-started/locally/)
 [![](https://img.shields.io/badge/code%20style-black-black.svg?style=for-the-badge&labelColor=gray)](https://black.readthedocs.io/en/stable/)
 [![](https://img.shields.io/github/actions/workflow/status/Labbeti/conette-audio-captioning/inference.yaml?branch=main&style=for-the-badge&logo=github)](https://github.com/Labbeti/conette-audio-captioning/actions)
 
 </div>
 
-CoNeTTE is an audio captioning system, which generate a short textual description of the sound events in any audio file. The architecture and training are explained in the corresponding [paper](https://arxiv.org/pdf/2309.00454.pdf). The model has been developped by me ([Étienne Labbé](https://labbeti.github.io/)) during my PhD. A simple interface to test CoNeTTE is available on [HuggingFace website](https://huggingface.co/spaces/Labbeti/conette).
+CoNeTTE is an audio captioning system, which generate a short textual description of the sound events in any audio file. The architecture and training are explained in the [corresponding paper](https://arxiv.org/pdf/2309.00454.pdf). The model has been developped by me ([Étienne Labbé](https://labbeti.github.io/)) during my PhD. A simple interface to test CoNeTTE is available on [HuggingFace website](https://huggingface.co/spaces/Labbeti/conette).
 
-## Inference
+## Training
+### Requirements
+- Intended for Ubuntu 20.04 only. Requires **java** < 1.13, **ffmpeg**, **yt-dlp**, and **zip** commands.
+- Recommanded GPU: NVIDIA V100 with 32GB VRAM.
+- WavCaps dataset might requires more than 2 TB of disk storage. Other datasets requires less than 50 GB.
+
+### Installation
+By default, **only the pip inference requirements are installed for conette**. To install training requirements you need to use the following command:
+```bash
+python -m pip install conette[train]
+```
+If you already installed conette for inference, it is **highly recommanded to create another environment** before installing conette for training.
+
+### Download external models and data
+These steps might take a while (few hours to download and prepare everything depending on your CPU, GPU and SSD/HDD).
+
+First, download the ConvNeXt, NLTK and spacy models :
+```bash
+conette-prepare data=none default=true pack_to_hdf=false csum_in_hdf_name=false pann=false
+```
+
+Then download the 4 datasets used to train CoNeTTE :
+```bash
+common_args="data.download=true pack_to_hdf=true audio_t=resample_mean_convnext audio_t.pretrain_path=cnext_bl_75 post_hdf_name=bl pretag=cnext_bl_75"
+
+conette-prepare data=audiocaps audio_t.src_sr=32000 ${common_args}
+conette-prepare data=clotho audio_t.src_sr=44100 ${common_args}
+conette-prepare data=macs audio_t.src_sr=48000 ${common_args}
+conette-prepare data=wavcaps audio_t.src_sr=32000 ${common_args} datafilter.min_audio_size=0.1 datafilter.max_audio_size=30.0 datafilter.sr=32000
+```
+
+### Train a model
+CNext-trans (baseline) on CL only (~3 hours on 1 GPU V100-32G)
+```bash
+conette-train expt=[clotho_cnext_bl] pl=baseline
+```
+
+CoNeTTE on AC+CL+MA+WC, specialized for CL (~4 hours on 1 GPU V100-32G)
+```bash
+conette-train expt=[camw_cnext_bl_for_c,task_ds_src_camw] pl=conette
+```
+
+CoNeTTE on AC+CL+MA+WC, specialized for AC (~3 hours on 1 GPU V100-32G)
+```bash
+conette-train expt=[camw_cnext_bl_for_a,task_ds_src_camw] pl=conette
+```
+
+Note 1: any training using AC data cannot be exactly reproduced because a part of this data is deleted from the YouTube source, and I cannot share my own audio files.
+Note 2: paper results are averaged scores over 5 seeds (1234-1238). The default training only uses seed 1234.
+
+## Inference only (without training)
 
 ### Installation
 ```bash
-python -m pip install conette
+python -m pip install conette[test]
 ```
 
 ### Usage with python
 ```py
 from conette import CoNeTTEConfig, CoNeTTEModel
 
 config = CoNeTTEConfig.from_pretrained("Labbeti/conette")
@@ -88,90 +138,40 @@
 ```
 
 ### Performance
 The model has been trained on AudioCaps (AC), Clotho (CL), MACS (MA) and WavCaps (WC). The performance on the test subsets are :
 
 | Test data | SPIDEr (%) | SPIDEr-FL (%) | FENSE (%) | Vocab | Outputs | Scores |
 | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
-| AC-test | 44.14 | 43.98 | 60.81 | 309 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/outputs_audiocaps_test.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/scores_audiocaps_test.yaml) |
-| CL-eval | 30.97 | 30.87 | 51.72 | 636 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/outputs_clotho_eval.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/conette/scores_clotho_eval.yaml) |
+| AC-test | 44.14 | 43.98 | 60.81 | 309 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/outputs_audiocaps_test.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/scores_audiocaps_test.yaml) |
+| CL-eval | 30.97 | 30.87 | 51.72 | 636 | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/outputs_clotho_eval.csv) | [Link](https://github.com/Labbeti/conette-audio-captioning/blob/main/results/detailed_outputs/scores_clotho_eval.yaml) |
 
 This model checkpoint has been trained with focus on the Clotho dataset, but it can also reach a good performance on AudioCaps with the "audiocaps" task.
 
 ### Limitations
 - The model expected audio sampled at **32 kHz**. The model automatically resample up or down the input audio files. However, it might give worse results, especially when using audio with lower sampling rates.
 - The model has been trained on audio lasting from **1 to 30 seconds**. It can handle longer audio files, but it might require more memory and give worse results.
 
-## Train a model
-### Requirements
-- Intended for Ubuntu 20.04 only. Requires **java** < 1.13, **ffmpeg**, **yt-dlp**, and **zip** commands.
-- Recommanded GPU: NVIDIA V100 with 32GB VRAM.
-- WavCaps dataset might requires more than 2 TB of disk storage. Other datasets requires less than 50 GB.
-
-### Installation
-By default, **only the inference requirements are installed for conette**. To install training requirements you need to use the following command:
-```bash
-python -m pip install conette[train]
-```
-If you already installed conette for inference, it is **highly recommanded to create another environment** before installing conette for training.
-
-### Download external models and data
-These steps might take a while (few hours to download and prepare everything depending on your CPU, GPU and SSD/HDD).
-
-First, download the ConvNeXt, NLTK and spacy models :
-```bash
-conette-prepare data=none default=true pack_to_hdf=false csum_in_hdf_name=false pann=false
-```
-
-Then download the 4 datasets used to train CoNeTTE :
-```bash
-cnext_bl_path="$HOME/.cache/torch/hub/checkpoints/convnext_tiny_465mAP_BL_AC.pth"
-common_args="data.download=true pack_to_hdf=true audio_t=resample_mean_convnext audio_t.pretrain_path=${cnext_bl_path} post_hdf_name=bl pretag=cnext_bl"
-
-conette-prepare data=audiocaps audio_t.src_sr=32000 ${common_args}
-conette-prepare data=clotho audio_t.src_sr=44100 ${common_args}
-conette-prepare data=macs audio_t.src_sr=48000 ${common_args}
-conette-prepare data=wavcaps audio_t.src_sr=32000 ${common_args} datafilter.min_audio_size=0.1 datafilter.max_audio_size=30.0 datafilter.sr=32000
-```
-
-### Train a model
-CNext-trans (baseline) on CL only (~3 hours on 1 GPU V100-32G)
-```bash
-conette-train expt=[clotho_cnext_bl] pl=baseline
-```
-
-CoNeTTE on AC+CL+MA+WC, specialized for CL (~4 hours on 1 GPU V100-32G)
-```bash
-conette-train expt=[camw_cnext_bl_for_c,task_ds_src_camw] pl=conette
-```
-
-CoNeTTE on AC+CL+MA+WC, specialized for AC (~3 hours on 1 GPU V100-32G)
-```bash
-conette-train expt=[camw_cnext_bl_for_a,task_ds_src_camw] pl=conette
-```
-
-**About reproducibility** : any training with AC data cannot be reproduced because a part of this data is deleted from the YouTube source, and I cannot share my own audio files.
-
 ## Citation
 The preprint version of the paper describing CoNeTTE is available on arxiv: https://arxiv.org/pdf/2309.00454.pdf
 
 ```bibtex
-@misc{labbé2023conette,
+@misc{labbe2023conette,
 	title        = {CoNeTTE: An efficient Audio Captioning system leveraging multiple datasets with Task Embedding},
 	author       = {Étienne Labbé and Thomas Pellegrini and Julien Pinquier},
 	year         = 2023,
 	journal      = {arXiv preprint arXiv:2309.00454},
 	url          = {https://arxiv.org/pdf/2309.00454.pdf},
 	eprint       = {2309.00454},
 	archiveprefix = {arXiv},
 	primaryclass = {cs.SD}
 }
 ```
 
 ## Additional information
 - CoNeTTE stands for **Co**nv**Ne**Xt-**T**ransformer with **T**ask **E**mbedding.
 - Model weights are available on HuggingFace: https://huggingface.co/Labbeti/conette
-- The weights of the encoder part of the architecture is based on a ConvNeXt model for audio classification, available here: https://zenodo.org/record/8020843 under the filename "convnext_tiny_465mAP_BL_AC_70kit.pth".
+- The weights of the encoder part of the architecture is based on a ConvNeXt model for audio classification, available here: https://zenodo.org/records/10987498 under the filename "convnext_tiny_465mAP_BL_AC_75kit.pth".
 
 ## Contact
 Maintainer:
-- Etienne Labbé "Labbeti": labbeti.pub@gmail.com
+- [Étienne Labbé](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

### Comparing `conette-0.2.2/src/conette.egg-info/SOURCES.txt` & `conette-0.3.0/src/conette.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 requirements-train.txt
 requirements.txt
 setup.py
 src/conette/__init__.py
 src/conette/info.py
 src/conette/predict.py
 src/conette/prepare.py
-src/conette/retrieve.py
 src/conette/train.py
 src/conette.egg-info/PKG-INFO
 src/conette.egg-info/SOURCES.txt
 src/conette.egg-info/dependency_links.txt
 src/conette.egg-info/entry_points.txt
 src/conette.egg-info/requires.txt
 src/conette.egg-info/top_level.txt
@@ -31,85 +30,58 @@
 src/conette/datamodules/aac_dm.py
 src/conette/datamodules/collate.py
 src/conette/datamodules/common.py
 src/conette/datamodules/hdf.py
 src/conette/datasets/__init__.py
 src/conette/datasets/typing.py
 src/conette/datasets/utils.py
-src/conette/datasets/hdf/__init__.py
-src/conette/datasets/hdf/common.py
-src/conette/datasets/hdf/dataset.py
-src/conette/datasets/hdf/pack.py
 src/conette/huggingface/__init__.py
 src/conette/huggingface/config.py
 src/conette/huggingface/model.py
 src/conette/huggingface/preprocessor.py
 src/conette/huggingface/setup.py
 src/conette/metrics/__init__.py
 src/conette/metrics/cross_referencing.py
-src/conette/metrics/retrieval.py
 src/conette/metrics/classes/__init__.py
 src/conette/metrics/classes/all_metrics.py
-src/conette/metrics/classes/bert_score_mrefs.ign.py
 src/conette/metrics/classes/diversity.py
-src/conette/metrics/classes/jaccard.py
 src/conette/metrics/classes/new_words.py
-src/conette/metrics/classes/null.py
-src/conette/metrics/classes/self_bleu.py
-src/conette/metrics/classes/tensor.py
 src/conette/metrics/classes/text_stats.py
-src/conette/metrics/classes/wmd.py
 src/conette/metrics/functional/__init__.py
-src/conette/metrics/functional/bert_score_mrefs.ign.py
-src/conette/metrics/functional/div_n.py
 src/conette/metrics/functional/diversity.py
-src/conette/metrics/functional/jaccard.py
 src/conette/metrics/functional/new_words.py
-src/conette/metrics/functional/self_bleu.py
 src/conette/metrics/functional/text_stats.py
-src/conette/metrics/functional/torch_cider_d.py
-src/conette/metrics/functional/wmd.py
 src/conette/nn/__init__.py
-src/conette/nn/cnext_ckpt_utils.py
+src/conette/nn/ckpt.py
 src/conette/nn/decoders/__init__.py
 src/conette/nn/decoders/aac_tfmer.py
 src/conette/nn/decoding/__init__.py
 src/conette/nn/decoding/beam.py
 src/conette/nn/decoding/common.py
 src/conette/nn/decoding/forcing.py
 src/conette/nn/decoding/greedy.py
 src/conette/nn/encoders/__init__.py
 src/conette/nn/encoders/cnn10.py
 src/conette/nn/encoders/cnn14.py
 src/conette/nn/encoders/cnn14_decisionlevel_att.py
 src/conette/nn/encoders/convnext.py
 src/conette/nn/encoders/ident.py
 src/conette/nn/functional/__init__.py
-src/conette/nn/functional/crop.py
 src/conette/nn/functional/drop.py
 src/conette/nn/functional/get.py
-src/conette/nn/functional/indexes.py
 src/conette/nn/functional/init.py
-src/conette/nn/functional/label.py
-src/conette/nn/functional/mask.py
-src/conette/nn/functional/misc.py
 src/conette/nn/functional/pad.py
-src/conette/nn/functional/repeat.py
 src/conette/nn/loss/__init__.py
 src/conette/nn/loss/ce_mean.py
 src/conette/nn/modules/__init__.py
-src/conette/nn/modules/crop.py
 src/conette/nn/modules/drop.py
 src/conette/nn/modules/misc.py
 src/conette/nn/modules/norm.py
-src/conette/nn/modules/pad.py
 src/conette/nn/modules/positional_encoding.py
-src/conette/nn/modules/tensor.py
 src/conette/nn/pann_utils/__init__.py
-src/conette/nn/pann_utils/ckpt.py
 src/conette/nn/pann_utils/hub.py
 src/conette/nn/pann_utils/models.py
 src/conette/nn/pann_utils/pytorch_utils.py
 src/conette/optim/__init__.py
 src/conette/optim/cyclic_cos_decay.py
 src/conette/optim/optimizers.py
 src/conette/optim/schedulers.py
@@ -127,15 +99,15 @@
 src/conette/tokenization/tokenizers/common.py
 src/conette/tokenization/tokenizers/factory.py
 src/conette/tokenization/tokenizers/ptb.py
 src/conette/tokenization/tokenizers/spacy.py
 src/conette/tokenization/tokenizers/word.py
 src/conette/tokenization/tokenizers/wrapper.py
 src/conette/transforms/__init__.py
-src/conette/transforms/audioset_labels.py
+src/conette/transforms/audioset_mapping.py
 src/conette/transforms/get.py
 src/conette/transforms/mixup.py
 src/conette/transforms/utils.py
 src/conette/transforms/audio/__init__.py
 src/conette/transforms/audio/cutoutspec.py
 src/conette/transforms/audio/resample.py
 src/conette/transforms/audio/spec_aug.py
@@ -148,10 +120,11 @@
 src/conette/utils/custom_logger.py
 src/conette/utils/dcase.py
 src/conette/utils/disk_cache.py
 src/conette/utils/func_utils.py
 src/conette/utils/hydra.py
 src/conette/utils/log_utils.py
 src/conette/utils/misc.py
+src/conette/utils/type_checks.py
 src/conette/utils/yaml_utils.py
 src/conf/__init__.py
 tests/test_inference.py
```

### Comparing `conette-0.2.2/tests/test_inference.py` & `conette-0.3.0/tests/test_inference.py`

 * *Files identical despite different names*

