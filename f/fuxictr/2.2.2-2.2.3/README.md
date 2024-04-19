# Comparing `tmp/fuxictr-2.2.2.tar.gz` & `tmp/fuxictr-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuxictr-2.2.2.tar", last modified: Thu Apr 18 06:22:02 2024, max compression
+gzip compressed data, was "dist/fuxictr-2.2.3.tar", last modified: Fri Apr 19 13:06:21 2024, max compression
```

## Comparing `fuxictr-2.2.2.tar` & `fuxictr-2.2.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-18 06:22:02.000000 fuxictr-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-04-18 06:21:58.000000 fuxictr-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/autotuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/datasets/avazu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/datasets/criteo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/datasets/kkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/preprocess/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    18058 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/preprocess/feature_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/preprocess/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/preprocess/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/dataloaders/npz_block_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/dataloaders/npz_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/dataloaders/rank_dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/dot_product_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/target_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/factorization_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/mlp_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/feature_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/cross_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/holographic_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/inner_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/interaction_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/layers/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/pytorch/models/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/models/multitask_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/models/rank_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/pytorch/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/dataloaders/tf_dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/factorization_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/mlp_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/cross_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/inner_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/layers/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr/tensorflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/models/rank_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/tensorflow/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 06:21:58.000000 fuxictr-2.2.2/fuxictr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 06:22:02.000000 fuxictr-2.2.2/fuxictr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/model_zoo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:22:02.000000 fuxictr-2.2.2/model_zoo/multitask/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 06:21:58.000000 fuxictr-2.2.2/model_zoo/multitask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:22:02.000000 fuxictr-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-18 06:21:58.000000 fuxictr-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-19 13:06:21.000000 fuxictr-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-04-19 13:06:19.000000 fuxictr-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/autotuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/datasets/avazu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/datasets/criteo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/datasets/kkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/preprocess/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18058 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/preprocess/feature_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/preprocess/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/preprocess/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/dataloaders/npz_block_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/dataloaders/npz_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/dataloaders/rank_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/dot_product_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/target_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/factorization_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/mlp_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/feature_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/cross_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/holographic_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/inner_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/interaction_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/layers/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/pytorch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/models/multitask_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/models/rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/pytorch/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/dataloaders/tf_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/factorization_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/mlp_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/cross_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/inner_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/layers/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr/tensorflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/models/rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/tensorflow/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 13:06:19.000000 fuxictr-2.2.3/fuxictr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 13:06:21.000000 fuxictr-2.2.3/fuxictr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/model_zoo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:06:21.000000 fuxictr-2.2.3/model_zoo/multitask/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 13:06:19.000000 fuxictr-2.2.3/model_zoo/multitask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:06:21.000000 fuxictr-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-19 13:06:19.000000 fuxictr-2.2.3/setup.py
```

### Comparing `fuxictr-2.2.2/PKG-INFO` & `fuxictr-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.2.2
+Version: 2.2.3
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/reczoo/FuxiCTR
 Author: RECZOO
 Author-email: reczoo@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/reczoo/FuxiCTR/tags
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.2.2 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.2.3 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/reczoo/FuxiCTR Author: RECZOO Author-email:
 reczoo@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/reczoo/FuxiCTR/tags Description:
                                     [Logo]
   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                                    _[_L_i_c_e_n_s_e_]
```

### Comparing `fuxictr-2.2.2/README.md` & `fuxictr-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/autotuner.py` & `fuxictr-2.2.3/fuxictr/autotuner.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/datasets/avazu.py` & `fuxictr-2.2.3/fuxictr/datasets/avazu.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/datasets/criteo.py` & `fuxictr-2.2.3/fuxictr/datasets/criteo.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/datasets/kkbox.py` & `fuxictr-2.2.3/fuxictr/datasets/kkbox.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/features.py` & `fuxictr-2.2.3/fuxictr/features.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/metrics.py` & `fuxictr-2.2.3/fuxictr/metrics.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/preprocess/build_dataset.py` & `fuxictr-2.2.3/fuxictr/preprocess/build_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,21 +56,22 @@
 
 def transform_block(feature_encoder, df_block, filename):
     darray_dict = feature_encoder.transform(df_block)
     save_npz(darray_dict, os.path.join(feature_encoder.data_dir, filename))
 
 
 def transform(feature_encoder, ddf, filename, block_size=0):
+    ddf = ddf.collect().to_pandas()
     if block_size > 0:
         pool = mp.Pool(mp.cpu_count() // 2)
         block_id = 0
         for idx in range(0, len(ddf), block_size):
             df_block = ddf.iloc[idx:(idx + block_size)]
             pool.apply_async(
-                transform_block, 
+                transform_block,
                 args=(feature_encoder,
                       df_block,
                       '{}/part_{:05d}.npz'.format(filename, block_id))
             )
             block_id += 1
         pool.close()
         pool.join()
```

### Comparing `fuxictr-2.2.2/fuxictr/preprocess/feature_processor.py` & `fuxictr-2.2.3/fuxictr/preprocess/feature_processor.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/preprocess/normalizer.py` & `fuxictr-2.2.3/fuxictr/preprocess/normalizer.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/preprocess/tokenizer.py` & `fuxictr-2.2.3/fuxictr/preprocess/tokenizer.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/dataloaders/npz_block_dataloader.py` & `fuxictr-2.2.3/fuxictr/pytorch/dataloaders/npz_block_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/dataloaders/npz_dataloader.py` & `fuxictr-2.2.3/fuxictr/pytorch/dataloaders/npz_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/dataloaders/rank_dataloader.py` & `fuxictr-2.2.3/fuxictr/pytorch/dataloaders/rank_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/activations.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/activations.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/dot_product_attention.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/dot_product_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/squeeze_excitation.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/attentions/target_attention.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/attentions/target_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/factorization_machine.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/logistic_regression.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/blocks/mlp_block.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/feature_embedding.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/bilinear_interaction.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/bilinear_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/cross_net.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/holographic_interaction.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/holographic_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/inner_product.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/interactions/interaction_machine.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/interactions/interaction_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/layers/pooling.py` & `fuxictr-2.2.3/fuxictr/pytorch/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/models/multitask_model.py` & `fuxictr-2.2.3/fuxictr/pytorch/models/multitask_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/models/rank_model.py` & `fuxictr-2.2.3/fuxictr/pytorch/models/rank_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/pytorch/torch_utils.py` & `fuxictr-2.2.3/fuxictr/pytorch/torch_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/dataloaders/tf_dataloader.py` & `fuxictr-2.2.3/fuxictr/tensorflow/dataloaders/tf_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/factorization_machine.py` & `fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/linear.py` & `fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/linear.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/logistic_regression.py` & `fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/layers/blocks/mlp_block.py` & `fuxictr-2.2.3/fuxictr/tensorflow/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/layers/embeddings/feature_embedding.py` & `fuxictr-2.2.3/fuxictr/tensorflow/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/cross_net.py` & `fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/layers/interactions/inner_product.py` & `fuxictr-2.2.3/fuxictr/tensorflow/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/layers/pooling.py` & `fuxictr-2.2.3/fuxictr/tensorflow/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/models/rank_model.py` & `fuxictr-2.2.3/fuxictr/tensorflow/models/rank_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/tensorflow/tf_utils.py` & `fuxictr-2.2.3/fuxictr/tensorflow/tf_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr/utils.py` & `fuxictr-2.2.3/fuxictr/utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/fuxictr.egg-info/PKG-INFO` & `fuxictr-2.2.3/fuxictr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.2.2
+Version: 2.2.3
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/reczoo/FuxiCTR
 Author: RECZOO
 Author-email: reczoo@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/reczoo/FuxiCTR/tags
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.2.2 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.2.3 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/reczoo/FuxiCTR Author: RECZOO Author-email:
 reczoo@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/reczoo/FuxiCTR/tags Description:
                                     [Logo]
   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                                    _[_L_i_c_e_n_s_e_]
```

### Comparing `fuxictr-2.2.2/fuxictr.egg-info/SOURCES.txt` & `fuxictr-2.2.3/fuxictr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.2/setup.py` & `fuxictr-2.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setuptools.setup(
     name="fuxictr",
-    version="2.2.2",
+    version="2.2.3",
     author="RECZOO",
     author_email="reczoo@users.noreply.github.com",
     description="A configurable, tunable, and reproducible library for CTR prediction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/reczoo/FuxiCTR",
     download_url='https://github.com/reczoo/FuxiCTR/tags',
```

