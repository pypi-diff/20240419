# Comparing `tmp/composer-0.21.2.tar.gz` & `tmp/composer-0.21.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composer-0.21.2.tar", last modified: Wed Apr  3 21:26:04 2024, max compression
+gzip compressed data, was "composer-0.21.3.tar", last modified: Fri Apr 19 15:50:47 2024, max compression
```

## Comparing `composer-0.21.2.tar` & `composer-0.21.3.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.023074 composer-0.21.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-03 21:25:51.000000 composer-0.21.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 21:25:51.000000 composer-0.21.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20625 2024-04-03 21:26:04.023074 composer-0.21.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19811 2024-04-03 21:25:51.000000 composer-0.21.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.979074 composer-0.21.2/composer/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-03 21:25:51.000000 composer-0.21.2/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 21:25:51.000000 composer-0.21.2/composer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 21:25:51.000000 composer-0.21.2/composer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/alibi/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/alibi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/_bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/augmix/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/augmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/augmix/augmix.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/augmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/blurpool/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/blurpool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/blurpool/blurpool.py
--rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/blurpool/blurpool_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/blurpool/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/channels_last/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/channels_last/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/channels_last/channels_last.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/channels_last/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/colout/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/colout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/colout/colout.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/colout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/cutmix/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutmix/cutmix.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/cutout/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutout/cutout.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/ema/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22108 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ema/ema.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ema/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/factorize/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/factorize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/factorize/factorize.py
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/factorize/factorize_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    22287 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/factorize/factorize_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/factorize/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/gated_linear_units/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gated_linear_units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gated_linear_units/gated_linear_units.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gated_linear_units/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/ghost_batchnorm/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ghost_batchnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ghost_batchnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/gradient_clipping/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gradient_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gradient_clipping/gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gradient_clipping/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/gyro_dropout/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gyro_dropout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gyro_dropout/gyro_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gyro_dropout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/label_smoothing/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/label_smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/label_smoothing/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/label_smoothing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/layer_freezing/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/layer_freezing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/layer_freezing/layer_freezing.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/layer_freezing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/low_precision_groupnorm/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_groupnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_groupnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/low_precision_layernorm/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_layernorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/mixup/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/mixup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/mixup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/mixup/mixup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/no_op_model/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/no_op_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/no_op_model/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/no_op_model/no_op_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/progressive_resizing/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/progressive_resizing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/progressive_resizing/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/progressive_resizing/progressive_resizing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/randaugment/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/randaugment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/randaugment/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/randaugment/randaugment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/sam/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/sam/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/selective_backprop/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/selective_backprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/selective_backprop/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/selective_backprop/selective_backprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/seq_length_warmup/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/seq_length_warmup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/seq_length_warmup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    19516 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/seq_length_warmup/seq_length_warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/squeeze_excite/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/squeeze_excite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/squeeze_excite/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/squeeze_excite/squeeze_excite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/stochastic_depth/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/stochastic_depth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/stochastic_depth/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/stochastic_depth/stochastic_depth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/stochastic_depth/stochastic_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/swa/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/swa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/swa/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/swa/swa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/utils/augmentation_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/utils/augmentation_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.999074 composer-0.21.2/composer/algorithms/weight_standardization/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/weight_standardization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/weight_standardization/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/weight_standardization/weight_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.999074 composer-0.21.2/composer/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/activation_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    26883 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/early_stopper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/eval_output_logging_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/export_for_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/free_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/image_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/lr_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/memory_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    17348 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/mlperf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/nan_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/oom_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/optimizer_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/runtime_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17116 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/speed_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/system_metrics_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/threshold_stopper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.999074 composer-0.21.2/composer/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 21:25:51.000000 composer-0.21.2/composer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 21:25:51.000000 composer-0.21.2/composer/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22187 2024-04-03 21:25:51.000000 composer-0.21.2/composer/cli/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.003074 composer-0.21.2/composer/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/data_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    24244 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)    83107 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    36521 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.003074 composer-0.21.2/composer/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 21:25:51.000000 composer-0.21.2/composer/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83538 2024-04-03 21:25:51.000000 composer-0.21.2/composer/datasets/in_context_learning_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-03 21:25:51.000000 composer-0.21.2/composer/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.007074 composer-0.21.2/composer/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_hpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.007074 composer-0.21.2/composer/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-03 21:25:51.000000 composer-0.21.2/composer/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.007074 composer-0.21.2/composer/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/cometml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/file_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/in_memory_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/logger_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    22266 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/mosaicml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15255 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/progress_bar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    31771 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/remote_uploader_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/slack_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.007074 composer-0.21.2/composer/loss/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loss/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.007074 composer-0.21.2/composer/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-03 21:25:51.000000 composer-0.21.2/composer/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-03 21:25:51.000000 composer-0.21.2/composer/metrics/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-03 21:25:51.000000 composer-0.21.2/composer/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    38870 2024-04-03 21:25:51.000000 composer-0.21.2/composer/metrics/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.011074 composer-0.21.2/composer/models/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    49464 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.011074 composer-0.21.2/composer/models/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/tasks/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.011074 composer-0.21.2/composer/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-03 21:25:51.000000 composer-0.21.2/composer/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18605 2024-04-03 21:25:51.000000 composer-0.21.2/composer/optim/decoupled_weight_decay.py
--rw-r--r--   0 runner    (1001) docker     (127)    39120 2024-04-03 21:25:51.000000 composer-0.21.2/composer/optim/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.011074 composer-0.21.2/composer/profiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/json_trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/json_trace_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/marker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/profiler_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/profiler_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/system_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18111 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/torch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:25:51.000000 composer-0.21.2/composer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.015074 composer-0.21.2/composer/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/_scale_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)    38951 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/dist_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/meta_safe_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/mosaic_fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    51445 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/mosaic_fsdp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   182353 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.019074 composer-0.21.2/composer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/auto_log_hparams.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/batch_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    58034 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.019074 composer-0.21.2/composer/utils/eval_client/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/eval_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/eval_client/eval_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/eval_client/lambda_eval_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/eval_client/local_eval_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/eval_client/mosaicml_lambda_eval_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    31422 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/fx_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/import_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/iter_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/module_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.019074 composer-0.21.2/composer/utils/object_store/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/gcs_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/libcloud_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/mlflow_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/oci_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/sftp_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/uc_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/retrying.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/string_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20625 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36090 2024-04-03 21:25:51.000000 composer-0.21.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:26:04.023074 composer-0.21.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-03 21:25:51.000000 composer-0.21.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.023074 composer-0.21.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_full_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_simple_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_smoketest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_split_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.894415 composer-0.21.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-19 15:50:38.000000 composer-0.21.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 15:50:38.000000 composer-0.21.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20625 2024-04-19 15:50:47.894415 composer-0.21.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19811 2024-04-19 15:50:38.000000 composer-0.21.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.842415 composer-0.21.3/composer/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-19 15:50:38.000000 composer-0.21.3/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-19 15:50:38.000000 composer-0.21.3/composer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-19 15:50:38.000000 composer-0.21.3/composer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.846415 composer-0.21.3/composer/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.846415 composer-0.21.3/composer/algorithms/alibi/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/alibi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/alibi/alibi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.846415 composer-0.21.3/composer/algorithms/alibi/attention_surgery_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/alibi/attention_surgery_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/alibi/attention_surgery_functions/_bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/alibi/attention_surgery_functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/alibi/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.846415 composer-0.21.3/composer/algorithms/augmix/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/augmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/augmix/augmix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/augmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.846415 composer-0.21.3/composer/algorithms/blurpool/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/blurpool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/blurpool/blurpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/blurpool/blurpool_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/blurpool/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.850416 composer-0.21.3/composer/algorithms/channels_last/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/channels_last/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/channels_last/channels_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/channels_last/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.850416 composer-0.21.3/composer/algorithms/colout/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/colout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/colout/colout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/colout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.850416 composer-0.21.3/composer/algorithms/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/cutmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/cutmix/cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/cutmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.850416 composer-0.21.3/composer/algorithms/cutout/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/cutout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/cutout/cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/cutout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.850416 composer-0.21.3/composer/algorithms/ema/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/ema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22108 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/ema/ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/ema/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.850416 composer-0.21.3/composer/algorithms/factorize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/factorize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/factorize/factorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/factorize/factorize_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22287 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/factorize/factorize_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/factorize/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.854416 composer-0.21.3/composer/algorithms/gated_linear_units/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/gated_linear_units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/gated_linear_units/gated_linear_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/gated_linear_units/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.854416 composer-0.21.3/composer/algorithms/ghost_batchnorm/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/ghost_batchnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/ghost_batchnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.854416 composer-0.21.3/composer/algorithms/gradient_clipping/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/gradient_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/gradient_clipping/gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/gradient_clipping/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.854416 composer-0.21.3/composer/algorithms/gyro_dropout/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/gyro_dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/gyro_dropout/gyro_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/gyro_dropout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.854416 composer-0.21.3/composer/algorithms/label_smoothing/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/label_smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/label_smoothing/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/label_smoothing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.854416 composer-0.21.3/composer/algorithms/layer_freezing/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/layer_freezing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/layer_freezing/layer_freezing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/layer_freezing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.854416 composer-0.21.3/composer/algorithms/low_precision_groupnorm/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/low_precision_groupnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/low_precision_groupnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.858415 composer-0.21.3/composer/algorithms/low_precision_layernorm/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/low_precision_layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/low_precision_layernorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.858415 composer-0.21.3/composer/algorithms/mixup/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/mixup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/mixup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/mixup/mixup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.858415 composer-0.21.3/composer/algorithms/no_op_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/no_op_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/no_op_model/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/no_op_model/no_op_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.858415 composer-0.21.3/composer/algorithms/progressive_resizing/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/progressive_resizing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/progressive_resizing/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/progressive_resizing/progressive_resizing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.858415 composer-0.21.3/composer/algorithms/randaugment/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/randaugment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/randaugment/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/randaugment/randaugment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.858415 composer-0.21.3/composer/algorithms/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/sam/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/sam/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.858415 composer-0.21.3/composer/algorithms/selective_backprop/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/selective_backprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/selective_backprop/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/selective_backprop/selective_backprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.862415 composer-0.21.3/composer/algorithms/seq_length_warmup/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/seq_length_warmup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/seq_length_warmup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19516 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/seq_length_warmup/seq_length_warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.862415 composer-0.21.3/composer/algorithms/squeeze_excite/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/squeeze_excite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/squeeze_excite/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/squeeze_excite/squeeze_excite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.862415 composer-0.21.3/composer/algorithms/stochastic_depth/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/stochastic_depth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/stochastic_depth/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/stochastic_depth/stochastic_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/stochastic_depth/stochastic_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.862415 composer-0.21.3/composer/algorithms/swa/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/swa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/swa/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/swa/swa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.862415 composer-0.21.3/composer/algorithms/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/utils/augmentation_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/utils/augmentation_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.862415 composer-0.21.3/composer/algorithms/weight_standardization/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/weight_standardization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/weight_standardization/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-19 15:50:38.000000 composer-0.21.3/composer/algorithms/weight_standardization/weight_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.866415 composer-0.21.3/composer/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/activation_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26883 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/early_stopper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/eval_output_logging_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/export_for_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/free_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/image_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/lr_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/memory_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17348 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/mlperf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/nan_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/oom_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/optimizer_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/runtime_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17116 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/speed_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/system_metrics_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-19 15:50:38.000000 composer-0.21.3/composer/callbacks/threshold_stopper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.870415 composer-0.21.3/composer/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 15:50:38.000000 composer-0.21.3/composer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-19 15:50:38.000000 composer-0.21.3/composer/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22187 2024-04-19 15:50:38.000000 composer-0.21.3/composer/cli/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.870415 composer-0.21.3/composer/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15311 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24244 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83107 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36521 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-19 15:50:38.000000 composer-0.21.3/composer/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.870415 composer-0.21.3/composer/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-19 15:50:38.000000 composer-0.21.3/composer/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83538 2024-04-19 15:50:38.000000 composer-0.21.3/composer/datasets/in_context_learning_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-19 15:50:38.000000 composer-0.21.3/composer/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.874415 composer-0.21.3/composer/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 15:50:38.000000 composer-0.21.3/composer/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-19 15:50:38.000000 composer-0.21.3/composer/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-19 15:50:38.000000 composer-0.21.3/composer/devices/device_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-19 15:50:38.000000 composer-0.21.3/composer/devices/device_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-19 15:50:38.000000 composer-0.21.3/composer/devices/device_hpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-19 15:50:38.000000 composer-0.21.3/composer/devices/device_mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-19 15:50:38.000000 composer-0.21.3/composer/devices/device_neuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-19 15:50:38.000000 composer-0.21.3/composer/devices/device_tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.874415 composer-0.21.3/composer/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-19 15:50:38.000000 composer-0.21.3/composer/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.878415 composer-0.21.3/composer/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/cometml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/file_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/in_memory_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/logger_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21704 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/mosaicml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13134 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15255 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/progress_bar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31771 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/remote_uploader_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/slack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.878415 composer-0.21.3/composer/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loss/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-19 15:50:38.000000 composer-0.21.3/composer/loss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.878415 composer-0.21.3/composer/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-19 15:50:38.000000 composer-0.21.3/composer/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-19 15:50:38.000000 composer-0.21.3/composer/metrics/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-19 15:50:38.000000 composer-0.21.3/composer/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38870 2024-04-19 15:50:38.000000 composer-0.21.3/composer/metrics/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.878415 composer-0.21.3/composer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-19 15:50:38.000000 composer-0.21.3/composer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-19 15:50:38.000000 composer-0.21.3/composer/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49464 2024-04-19 15:50:38.000000 composer-0.21.3/composer/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-19 15:50:38.000000 composer-0.21.3/composer/models/initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.878415 composer-0.21.3/composer/models/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-19 15:50:38.000000 composer-0.21.3/composer/models/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-19 15:50:38.000000 composer-0.21.3/composer/models/tasks/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.878415 composer-0.21.3/composer/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-19 15:50:38.000000 composer-0.21.3/composer/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18605 2024-04-19 15:50:38.000000 composer-0.21.3/composer/optim/decoupled_weight_decay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39120 2024-04-19 15:50:38.000000 composer-0.21.3/composer/optim/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.882415 composer-0.21.3/composer/profiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/json_trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/json_trace_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/profiler_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/profiler_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/system_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18111 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/torch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-19 15:50:38.000000 composer-0.21.3/composer/profiler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:38.000000 composer-0.21.3/composer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.882415 composer-0.21.3/composer/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-19 15:50:38.000000 composer-0.21.3/composer/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-19 15:50:38.000000 composer-0.21.3/composer/trainer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-19 15:50:38.000000 composer-0.21.3/composer/trainer/_scale_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-19 15:50:38.000000 composer-0.21.3/composer/trainer/_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41751 2024-04-19 15:50:38.000000 composer-0.21.3/composer/trainer/dist_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-19 15:50:38.000000 composer-0.21.3/composer/trainer/meta_safe_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-19 15:50:38.000000 composer-0.21.3/composer/trainer/mosaic_fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53458 2024-04-19 15:50:38.000000 composer-0.21.3/composer/trainer/mosaic_fsdp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182492 2024-04-19 15:50:38.000000 composer-0.21.3/composer/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.886415 composer-0.21.3/composer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/auto_log_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/batch_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58034 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.890415 composer-0.21.3/composer/utils/eval_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/eval_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/eval_client/eval_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/eval_client/lambda_eval_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/eval_client/local_eval_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/eval_client/mosaicml_lambda_eval_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31422 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/fx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/import_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/iter_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/module_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.890415 composer-0.21.3/composer/utils/object_store/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/object_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/object_store/gcs_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/object_store/libcloud_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/object_store/mlflow_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/object_store/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/object_store/oci_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/object_store/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/object_store/sftp_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/object_store/uc_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/retrying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/string_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-19 15:50:38.000000 composer-0.21.3/composer/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.846415 composer-0.21.3/composer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20625 2024-04-19 15:50:47.000000 composer-0.21.3/composer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-19 15:50:47.000000 composer-0.21.3/composer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 15:50:47.000000 composer-0.21.3/composer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 15:50:47.000000 composer-0.21.3/composer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-19 15:50:47.000000 composer-0.21.3/composer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 15:50:47.000000 composer-0.21.3/composer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36090 2024-04-19 15:50:38.000000 composer-0.21.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 15:50:47.894415 composer-0.21.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-19 15:50:38.000000 composer-0.21.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:50:47.894415 composer-0.21.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_full_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_simple_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_smoketest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_split_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-19 15:50:38.000000 composer-0.21.3/tests/test_time.py
```

### Comparing `composer-0.21.2/LICENSE` & `composer-0.21.3/LICENSE`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/PKG-INFO` & `composer-0.21.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.21.2
+Version: 0.21.3
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: composer Version: 0.21.2 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.21.3 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.9 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
```

### Comparing `composer-0.21.2/README.md` & `composer-0.21.3/README.md`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/__init__.py` & `composer-0.21.3/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/__init__.py` & `composer-0.21.3/composer/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/alibi/__init__.py` & `composer-0.21.3/composer/algorithms/alibi/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/alibi/alibi.py` & `composer-0.21.3/composer/algorithms/alibi/alibi.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/__init__.py` & `composer-0.21.3/composer/algorithms/alibi/attention_surgery_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/_bert.py` & `composer-0.21.3/composer/algorithms/alibi/attention_surgery_functions/_bert.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py` & `composer-0.21.3/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/utils.py` & `composer-0.21.3/composer/algorithms/alibi/attention_surgery_functions/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/augmix/__init__.py` & `composer-0.21.3/composer/algorithms/augmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/augmix/augmix.py` & `composer-0.21.3/composer/algorithms/augmix/augmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/blurpool/__init__.py` & `composer-0.21.3/composer/algorithms/blurpool/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/blurpool/blurpool.py` & `composer-0.21.3/composer/algorithms/blurpool/blurpool.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/blurpool/blurpool_layers.py` & `composer-0.21.3/composer/algorithms/blurpool/blurpool_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/channels_last/__init__.py` & `composer-0.21.3/composer/algorithms/channels_last/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/channels_last/channels_last.py` & `composer-0.21.3/composer/algorithms/channels_last/channels_last.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/colout/__init__.py` & `composer-0.21.3/composer/algorithms/colout/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/colout/colout.py` & `composer-0.21.3/composer/algorithms/colout/colout.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/cutmix/__init__.py` & `composer-0.21.3/composer/algorithms/cutmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/cutmix/cutmix.py` & `composer-0.21.3/composer/algorithms/cutmix/cutmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/cutout/cutout.py` & `composer-0.21.3/composer/algorithms/cutout/cutout.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/ema/ema.py` & `composer-0.21.3/composer/algorithms/ema/ema.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/factorize/__init__.py` & `composer-0.21.3/composer/algorithms/factorize/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/factorize/factorize.py` & `composer-0.21.3/composer/algorithms/factorize/factorize.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/factorize/factorize_core.py` & `composer-0.21.3/composer/algorithms/factorize/factorize_core.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/factorize/factorize_modules.py` & `composer-0.21.3/composer/algorithms/factorize/factorize_modules.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/gated_linear_units/__init__.py` & `composer-0.21.3/composer/algorithms/gated_linear_units/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py` & `composer-0.21.3/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/gated_linear_units/gated_linear_units.py` & `composer-0.21.3/composer/algorithms/gated_linear_units/gated_linear_units.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/ghost_batchnorm/__init__.py` & `composer-0.21.3/composer/algorithms/ghost_batchnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py` & `composer-0.21.3/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/gradient_clipping/gradient_clipping.py` & `composer-0.21.3/composer/algorithms/gradient_clipping/gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/gyro_dropout/gyro_dropout.py` & `composer-0.21.3/composer/algorithms/gyro_dropout/gyro_dropout.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/label_smoothing/__init__.py` & `composer-0.21.3/composer/algorithms/label_smoothing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/label_smoothing/label_smoothing.py` & `composer-0.21.3/composer/algorithms/label_smoothing/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/label_smoothing/metadata.json` & `composer-0.21.3/composer/algorithms/label_smoothing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/layer_freezing/layer_freezing.py` & `composer-0.21.3/composer/algorithms/layer_freezing/layer_freezing.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/low_precision_groupnorm/__init__.py` & `composer-0.21.3/composer/algorithms/low_precision_groupnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py` & `composer-0.21.3/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/low_precision_layernorm/__init__.py` & `composer-0.21.3/composer/algorithms/low_precision_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py` & `composer-0.21.3/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/mixup/mixup.py` & `composer-0.21.3/composer/algorithms/mixup/mixup.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/no_op_model/__init__.py` & `composer-0.21.3/composer/algorithms/no_op_model/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/no_op_model/no_op_model.py` & `composer-0.21.3/composer/algorithms/no_op_model/no_op_model.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/progressive_resizing/__init__.py` & `composer-0.21.3/composer/algorithms/progressive_resizing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/progressive_resizing/metadata.json` & `composer-0.21.3/composer/algorithms/progressive_resizing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/progressive_resizing/progressive_resizing.py` & `composer-0.21.3/composer/algorithms/progressive_resizing/progressive_resizing.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/randaugment/metadata.json` & `composer-0.21.3/composer/algorithms/randaugment/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/randaugment/randaugment.py` & `composer-0.21.3/composer/algorithms/randaugment/randaugment.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/sam/__init__.py` & `composer-0.21.3/composer/algorithms/sam/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/sam/sam.py` & `composer-0.21.3/composer/algorithms/sam/sam.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/selective_backprop/__init__.py` & `composer-0.21.3/composer/algorithms/selective_backprop/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/selective_backprop/selective_backprop.py` & `composer-0.21.3/composer/algorithms/selective_backprop/selective_backprop.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/seq_length_warmup/seq_length_warmup.py` & `composer-0.21.3/composer/algorithms/seq_length_warmup/seq_length_warmup.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/squeeze_excite/__init__.py` & `composer-0.21.3/composer/algorithms/squeeze_excite/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/squeeze_excite/squeeze_excite.py` & `composer-0.21.3/composer/algorithms/squeeze_excite/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/stochastic_depth/__init__.py` & `composer-0.21.3/composer/algorithms/stochastic_depth/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/stochastic_depth/metadata.json` & `composer-0.21.3/composer/algorithms/stochastic_depth/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/stochastic_depth/stochastic_depth.py` & `composer-0.21.3/composer/algorithms/stochastic_depth/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/stochastic_depth/stochastic_layers.py` & `composer-0.21.3/composer/algorithms/stochastic_depth/stochastic_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/swa/swa.py` & `composer-0.21.3/composer/algorithms/swa/swa.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/utils/augmentation_common.py` & `composer-0.21.3/composer/algorithms/utils/augmentation_common.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/utils/augmentation_primitives.py` & `composer-0.21.3/composer/algorithms/utils/augmentation_primitives.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/warnings.py` & `composer-0.21.3/composer/algorithms/warnings.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/algorithms/weight_standardization/weight_standardization.py` & `composer-0.21.3/composer/algorithms/weight_standardization/weight_standardization.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/__init__.py` & `composer-0.21.3/composer/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/activation_monitor.py` & `composer-0.21.3/composer/callbacks/activation_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/checkpoint_saver.py` & `composer-0.21.3/composer/callbacks/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/early_stopper.py` & `composer-0.21.3/composer/callbacks/early_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/eval_output_logging_callback.py` & `composer-0.21.3/composer/callbacks/eval_output_logging_callback.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/export_for_inference.py` & `composer-0.21.3/composer/callbacks/export_for_inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/generate.py` & `composer-0.21.3/composer/callbacks/generate.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/image_visualizer.py` & `composer-0.21.3/composer/callbacks/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/lr_monitor.py` & `composer-0.21.3/composer/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/memory_monitor.py` & `composer-0.21.3/composer/callbacks/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/memory_snapshot.py` & `composer-0.21.3/composer/callbacks/memory_snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def __init__(
         self,
         skip_batches: int = 1,
         interval: Union[int, str, Time] = '3ba',
         max_entries: int = 100000,
         folder: str = '{run_name}/torch_traces',
         filename: str = 'rank{rank}.{batch}.memory_snapshot',
-        remote_file_name: Optional[str] = '{run_name}/torch_memory_traces/rank{rank}.{batch}.memory_snapshot',
+        remote_file_name: Optional[str] = '{run_name}/torch_memory_traces',
         overwrite: bool = False,
     ) -> None:
         self.batches_left_to_skip = skip_batches
         # Check that the interval timestring is parsable and convert into time object
         self.interval = Time.from_input(interval, TimeUnit.BATCH)
         self.max_entries = max_entries
         self.folder = folder
@@ -175,15 +175,15 @@
             with open(trace_plot_file, 'w+') as fd:
                 fd.write(torch.cuda._memory_viz.trace_plot(snapshot))  # type: ignore
 
             log.info(f'Saved memory snapshot to local files with prefix = {filename}')
 
             if self.remote_path_in_bucket is not None:
                 for f in [snapshot_file, trace_plot_file]:
-                    remote_file_name = (self.remote_path_in_bucket + os.path.basename(f)).lstrip('/')
+                    remote_file_name = os.path.join(self.remote_path_in_bucket, os.path.basename(f)).lstrip('/')
                     log.info(f'Uploading memory snapshot to remote: {remote_file_name} from {f}')
                     try:
                         logger.upload_file(remote_file_name=remote_file_name, file_path=f, overwrite=self.overwrite)
                     except FileExistsError as e:
                         raise FileExistsError(
                             f'Uploading memory snapshot failed with error: {e}. overwrite was set to {self.overwrite}. To overwrite memory snapshot with Trainer, set `overwrite` to True.',
                         ) from e
```

### Comparing `composer-0.21.2/composer/callbacks/mlperf.py` & `composer-0.21.3/composer/callbacks/mlperf.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/nan_monitor.py` & `composer-0.21.3/composer/callbacks/nan_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/oom_observer.py` & `composer-0.21.3/composer/callbacks/oom_observer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,57 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Generate a memory snapshot during an OutOfMemory exception."""
+from __future__ import annotations
 
+import dataclasses
 import logging
 import os
 import pickle
 import warnings
-from typing import Optional
+from dataclasses import dataclass
+from pathlib import Path
+from typing import List, Optional
 
 import torch.cuda
 from packaging import version
 
-from composer import State
 from composer.core import Callback, State
 from composer.loggers import Logger
 from composer.utils import ensure_folder_is_empty, format_name_with_dist, format_name_with_dist_and_time, parse_uri
 
 log = logging.getLogger(__name__)
 
 __all__ = ['OOMObserver']
 
 
+@dataclass(frozen=True)
+class SnapshotFileNameConfig:
+    """Configuration for the file names of the memory snapshot visualizations."""
+    snapshot_file: str
+    trace_plot_file: str
+    segment_plot_file: str
+    segment_flamegraph_file: str
+    memory_flamegraph_file: str
+
+    @classmethod
+    def from_file_name(cls, filename: str) -> 'SnapshotFileNameConfig':
+        return cls(
+            snapshot_file=filename + '_snapshot.pickle',
+            trace_plot_file=filename + '_trace_plot.html',
+            segment_plot_file=filename + '_segment_plot.html',
+            segment_flamegraph_file=filename + '_segment_flamegraph.svg',
+            memory_flamegraph_file=filename + '_memory_flamegraph.svg',
+        )
+
+    def list_filenames(self) -> List[str]:
+        return [getattr(self, field.name) for field in dataclasses.fields(self)]
+
+
 class OOMObserver(Callback):
     """Generate visualizations of the state of allocated memory during an OutOfMemory exception.
 
     This callback registers an observer with the allocator that will be called everytime it is about to raise an OutOfMemoryError before any memory has been release while unwinding the exception. OOMObserver is attached to the Trainer at init stage. The visualizations include a snapshot of the memory state, a trace plot, a segment plot, a segment flamegraph, and a memory flamegraph.
 
     Example:
         .. doctest::
@@ -90,14 +116,16 @@
         if version.parse(torch.__version__.split('.dev')[0]) >= version.parse('2.1.0'):  # type: ignore
             # OOMObserver is only supported in torch v2.1.0 or higher
             self._enabled = True
         else:
             self._enabled = False
             warnings.warn('OOMObserver is supported after PyTorch 2.1.0. Disabling OOMObserver callback.')
 
+        self.filename_config: Optional[SnapshotFileNameConfig] = None
+
     def init(self, state: State, logger: Logger) -> None:
         if not self._enabled:
             return
         # Not relying on `torch.cuda.is_available()` since the model could be on CPU.
         model_device = next(state.model.parameters()).device
 
         if model_device.type not in ('cuda', 'meta'):
@@ -113,58 +141,47 @@
 
         def oom_observer(device: int, alloc: int, device_alloc: int, device_free: int):
             # Snapshot right after an OOM happened
             log.warning('Out Of Memory (OOM) observed')
 
             assert self.filename
             assert self.folder_name, 'folder_name must be set in init'
-            filename = os.path.join(
-                self.folder_name,
+            filename = Path(self.folder_name) / Path(
                 format_name_with_dist_and_time(self.filename, run_name=state.run_name, timestamp=state.timestamp),
             )
 
             try:
-                snapshot_file = filename + '_snapshot.pickle'
-                trace_plot_file = filename + '_trace_plot.html'
-                segment_plot_file = filename + '_segment_plot.html'
-                segment_flamegraph_file = filename + '_segment_flamegraph.svg'
-                memory_flamegraph_file = filename + '_memory_flamegraph.svg'
+                self.filename_config = SnapshotFileNameConfig.from_file_name(str(filename))
                 log.info(f'Dumping OOMObserver visualizations')
 
                 snapshot = torch.cuda.memory._snapshot()
                 # No data was recorded - avoids a `ValueError` in `trace_plot`
                 if all(len(t) == 0 for t in snapshot['device_traces']):
                     log.info(f'No allocation is recorded in memory snapshot)')
                     return
 
-                with open(snapshot_file, 'wb') as fd:
+                with open(self.filename_config.snapshot_file, 'wb') as fd:
                     pickle.dump(snapshot, fd)
 
-                with open(trace_plot_file, 'w+') as fd:
+                with open(self.filename_config.trace_plot_file, 'w+') as fd:
                     fd.write(torch.cuda._memory_viz.trace_plot(snapshot))  # type: ignore
 
-                with open(segment_plot_file, 'w+') as fd:
+                with open(self.filename_config.segment_plot_file, 'w+') as fd:
                     fd.write(torch.cuda._memory_viz.segment_plot(snapshot))  # type: ignore
 
-                with open(segment_flamegraph_file, 'w+') as fd:
+                with open(self.filename_config.segment_flamegraph_file, 'w+') as fd:
                     fd.write(torch.cuda._memory_viz.segments(snapshot))  # type: ignore
 
-                with open(memory_flamegraph_file, 'w+') as fd:
+                with open(self.filename_config.memory_flamegraph_file, 'w+') as fd:
                     fd.write(torch.cuda._memory_viz.memory(snapshot))  # type: ignore
 
                 log.info(f'Saved memory visualizations to local files with prefix = {filename} during OOM')
 
                 if self.remote_path_in_bucket is not None:
-                    for f in [
-                        snapshot_file,
-                        trace_plot_file,
-                        segment_plot_file,
-                        segment_flamegraph_file,
-                        memory_flamegraph_file,
-                    ]:
+                    for f in self.filename_config.list_filenames():
                         base_file_name = os.path.basename(f)
                         remote_file_name = os.path.join(self.remote_path_in_bucket, base_file_name)
                         remote_file_name = remote_file_name.lstrip('/')  # remove leading slashes
                         log.info(f'Uploading memory visualization to remote: {remote_file_name} from {f}')
                         try:
                             logger.upload_file(remote_file_name=remote_file_name, file_path=f, overwrite=self.overwrite)
                         except FileExistsError as e:
```

### Comparing `composer-0.21.2/composer/callbacks/optimizer_monitor.py` & `composer-0.21.3/composer/callbacks/optimizer_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/runtime_estimator.py` & `composer-0.21.3/composer/callbacks/runtime_estimator.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/speed_monitor.py` & `composer-0.21.3/composer/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/system_metrics_monitor.py` & `composer-0.21.3/composer/callbacks/system_metrics_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/callbacks/threshold_stopper.py` & `composer-0.21.3/composer/callbacks/threshold_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/cli/launcher.py` & `composer-0.21.3/composer/cli/launcher.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/__init__.py` & `composer-0.21.3/composer/core/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/algorithm.py` & `composer-0.21.3/composer/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/callback.py` & `composer-0.21.3/composer/core/callback.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/data_spec.py` & `composer-0.21.3/composer/core/data_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
                     'does not have an active iterator, so CPU dataset augmentations can be '
                     'correctly inserted. To fix, please do not iterate over the dataloader before passing it into '
                     'the Trainer.'
                 ))
             world_size = dist.get_world_size()
             # Check for Distributed Sampler if not using IterableDataset on more than 1 GPU
             if world_size > 1 and not isinstance(dataloader.dataset, torch.utils.data.IterableDataset):
-                is_sampler_distributed = dataloader.sampler and isinstance(dataloader.sampler, DistributedSampler)
+                is_sampler_distributed = isinstance(dataloader.sampler, DistributedSampler)
                 is_batch_sampler_distributed = dataloader.batch_sampler is not None and isinstance(
                     dataloader.batch_sampler,
                     DistributedSampler,
                 )
                 if not is_sampler_distributed and not is_batch_sampler_distributed:
                     raise ValueError(
                         f'The world_size({world_size}) > 1 but dataloader does not use '
```

### Comparing `composer-0.21.2/composer/core/engine.py` & `composer-0.21.3/composer/core/engine.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/evaluator.py` & `composer-0.21.3/composer/core/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,16 @@
                 raise ValueError(f'``metric_names`` should be a list of strings, not a {type(metric_names)}')
         self.metric_names = metric_names
 
         self.subset_num_batches = subset_num_batches
         self._eval_interval = None
         self.eval_interval = eval_interval
         self.auto_microbatching = _is_auto_microbatching(device_eval_microbatch_size)
+        if self.auto_microbatching and hasattr(self.dataloader, 'seq_parallel_world_size'):
+            raise ValueError('`device_eval_microbatch_size="auto"` is not compatible with sequence parallelism.')
         self.device_eval_microbatch_size = _get_initial_device_eval_microbatch_size(
             device_eval_microbatch_size,
             self.auto_microbatching,
             self.dataloader.dataloader,
         )
 
     @property
@@ -173,11 +175,11 @@
                 raise AttributeError(
                     textwrap.dedent(
                         '`device_eval_microbatch_size` is not set and `dataloader` does not have a `batch_size` attribute. '
                         'Please either set `device_eval_microbatch_size` or `dataloader.batch_size`.',
                     ),
                 ) from e
         return batch_size
-    elif isinstance(device_eval_microbatch_size, int):
+    elif isinstance(device_eval_microbatch_size, Union[int, float]):
         return device_eval_microbatch_size
     else:
         raise ValueError("device_eval_microbatch_size must be an int or ``'auto'``")
```

### Comparing `composer-0.21.2/composer/core/event.py` & `composer-0.21.3/composer/core/event.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/passes.py` & `composer-0.21.3/composer/core/passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/precision.py` & `composer-0.21.3/composer/core/precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/serializable.py` & `composer-0.21.3/composer/core/serializable.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/state.py` & `composer-0.21.3/composer/core/state.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/time.py` & `composer-0.21.3/composer/core/time.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/core/types.py` & `composer-0.21.3/composer/core/types.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/datasets/__init__.py` & `composer-0.21.3/composer/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/datasets/in_context_learning_evaluation.py` & `composer-0.21.3/composer/datasets/in_context_learning_evaluation.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/datasets/utils.py` & `composer-0.21.3/composer/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/devices/__init__.py` & `composer-0.21.3/composer/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/devices/device.py` & `composer-0.21.3/composer/devices/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/devices/device_cpu.py` & `composer-0.21.3/composer/devices/device_cpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/devices/device_gpu.py` & `composer-0.21.3/composer/devices/device_gpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/devices/device_hpu.py` & `composer-0.21.3/composer/devices/device_hpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/devices/device_mps.py` & `composer-0.21.3/composer/devices/device_mps.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/devices/device_neuron.py` & `composer-0.21.3/composer/devices/device_neuron.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/devices/device_tpu.py` & `composer-0.21.3/composer/devices/device_tpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/functional/__init__.py` & `composer-0.21.3/composer/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/__init__.py` & `composer-0.21.3/composer/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/cometml_logger.py` & `composer-0.21.3/composer/loggers/cometml_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/console_logger.py` & `composer-0.21.3/composer/loggers/console_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/file_logger.py` & `composer-0.21.3/composer/loggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/in_memory_logger.py` & `composer-0.21.3/composer/loggers/in_memory_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/logger.py` & `composer-0.21.3/composer/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/logger_destination.py` & `composer-0.21.3/composer/loggers/logger_destination.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/mlflow_logger.py` & `composer-0.21.3/composer/loggers/mlflow_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         del logger  # unused
 
         if self.run_name is None:
             self.run_name = state.run_name
 
         # Store the Composer run name in the MLFlow run tags so it can be retrieved for autoresume.
         self.tags = self.tags or {}
-        self.tags['run_name'] = state.run_name
+        self.tags['run_name'] = os.environ.get('RUN_NAME', state.run_name)
 
         # Adjust name and group based on `rank_zero_only`.
         if not self._rank_zero_only:
             self.run_name += f'-rank{dist.get_global_rank()}'
 
         # Start run
         if self._enabled:
@@ -167,24 +167,14 @@
                 assert self._experiment_id is not None
                 existing_runs = mlflow.search_runs(
                     experiment_ids=[self._experiment_id],
                     filter_string=f'tags.run_name = "{state.run_name}"',
                     output_format='list',
                 )
 
-                # Check for the old tag (`composer_run_name`) For backwards compatibility in case a run using the old
-                # tag fails and the run is resumed with a newer version of Composer that uses `run_name` instead of
-                # `composer_run_name`.
-                if len(existing_runs) == 0:
-                    existing_runs = mlflow.search_runs(
-                        experiment_ids=[self._experiment_id],
-                        filter_string=f'tags.composer_run_name = "{state.run_name}"',
-                        output_format='list',
-                    )
-
                 if len(existing_runs) > 0:
                     self._run_id = existing_runs[0].info.run_id
                 else:
                     new_run = self._mlflow_client.create_run(
                         experiment_id=self._experiment_id,
                         run_name=self.run_name,
                     )
```

### Comparing `composer-0.21.2/composer/loggers/mosaicml_logger.py` & `composer-0.21.3/composer/loggers/mosaicml_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/neptune_logger.py` & `composer-0.21.3/composer/loggers/neptune_logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,120 +5,123 @@
 
 __all__ = ['NeptuneLogger']
 
 import os
 import pathlib
 import warnings
 from functools import partial
-from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Set, Union
+from importlib.metadata import version
+from typing import TYPE_CHECKING, Any, Dict, Literal, Optional, Sequence, Set, Union
 
 import numpy as np
 import torch
+from packaging.version import Version
 
 from composer._version import __version__
 from composer.loggers import LoggerDestination
-from composer.utils import MissingConditionalImportError, dist
+from composer.utils import MissingConditionalImportError, VersionedDeprecationWarning, dist
 
 if TYPE_CHECKING:
     from composer import Logger
     from composer.core import State
 
+NEPTUNE_MODE_TYPE = Literal['async', 'sync', 'offline', 'read-only', 'debug']
+NEPTUNE_VERSION_WITH_PROGRESS_BAR = Version('1.9.0')
+
 
 class NeptuneLogger(LoggerDestination):
     """Log to `neptune.ai <https://neptune.ai/>`_.
 
-    For more, see the [Neptune-Composer integration guide](https://docs.neptune.ai/integrations/composer/).
+    For instructions, see the
+    `integration guide <https://docs.neptune.ai/integrations/mosaicml_composer/>`_.
 
     Args:
         project (str, optional): The name of your Neptune project,
             in the form "workspace-name/project-name". If you leave it empty, the
             ``NEPTUNE_PROJECT`` environment variable will be used.
         api_token (str, optional): Your Neptune API token.
             You can leave out this argument if you save your token to the
             ``NEPTUNE_API_TOKEN`` environment variable (recommended).
             You can find your API token in the user menu of the Neptune web app.
-        rank_zero_only (bool, optional): Whether to log only on the rank-zero process.
-            (default: ``True``).
-        upload_artifacts (bool, optional): Whether the logger should upload artifacts to Neptune.
+        rank_zero_only (bool): Whether to log only on the rank-zero process (default: ``True``).
+        upload_artifacts (bool, optional): Deprecated. See ``upload_checkpoints``.
+        upload_checkpoints (bool): Whether the logger should upload checkpoints to Neptune
             (default: ``False``).
-        base_namespace (str, optional): The name of the base namespace to log the metadata to.
-            (default: "training").
+        base_namespace (str, optional): The name of the base namespace where the metadata
+            is logged (default: "training").
         neptune_kwargs (Dict[str, Any], optional): Any additional keyword arguments to the
             ``neptune.init_run()`` function. For options, see the
-            `Run API reference <https://docs.neptune.ai/api/neptune/#init_run>`_ in the
-            Neptune docs.
+            `Run API reference <https://docs.neptune.ai/api/neptune/#init_run>`_.
     """
     metric_namespace = 'metrics'
     hyperparam_namespace = 'hyperparameters'
     trace_namespace = 'traces'
     integration_version_key = 'source_code/integrations/neptune-MosaicML'
 
     def __init__(
         self,
         *,
         project: Optional[str] = None,
         api_token: Optional[str] = None,
         rank_zero_only: bool = True,
-        upload_artifacts: bool = False,
+        upload_artifacts: Optional[bool] = None,
+        upload_checkpoints: bool = False,
         base_namespace: str = 'training',
+        mode: Optional[NEPTUNE_MODE_TYPE] = None,
         **neptune_kwargs,
     ) -> None:
         try:
             from neptune.internal.utils import verify_type
         except ImportError as e:
             raise MissingConditionalImportError(
                 extra_deps_group='neptune',
                 conda_package='neptune',
                 conda_channel='conda-forge',
             ) from e
 
         verify_type('project', project, (str, type(None)))
         verify_type('api_token', api_token, (str, type(None)))
         verify_type('rank_zero_only', rank_zero_only, bool)
-        verify_type('upload_artifacts', upload_artifacts, bool)
+        verify_type('upload_artifacts', upload_artifacts, (bool, type(None)))
+        verify_type('upload_checkpoints', upload_checkpoints, bool)
         verify_type('base_namespace', base_namespace, str)
 
         if not base_namespace:
             raise ValueError("Argument 'base_namespace' cannot be an empty string.")
 
         self._project = project
         self._api_token = api_token
         self._rank_zero_only = rank_zero_only
-        self._upload_artifacts = upload_artifacts
+
+        if upload_artifacts is not None:
+            _warn_about_deprecated_upload_artifacts()
+            self._upload_checkpoints = upload_artifacts
+        else:
+            self._upload_checkpoints = upload_checkpoints
+
         self._base_namespace = base_namespace
         self._neptune_kwargs = neptune_kwargs
 
-        mode = self._neptune_kwargs.pop('mode', 'async')
-
         self._enabled = (not rank_zero_only) or dist.get_global_rank() == 0
 
-        self._mode = mode if self._enabled else 'debug'
+        self._mode: Optional[NEPTUNE_MODE_TYPE] = mode if self._enabled else 'debug'
 
         self._neptune_run = None
         self._base_handler = None
 
         self._metrics_dict: Dict[str, int] = {}  # used to prevent duplicate step logging
 
         super().__init__()
 
     @property
     def neptune_run(self):
         """Gets the Neptune run object from a NeptuneLogger instance.
 
-        You can log additional metadata to the run by accessing a path inside the run and assigning metadata to it
-        with "=" or [Neptune logging methods](https://docs.neptune.ai/logging/methods/).
-
-        Example:
-                from composer import Trainer
-                from composer.loggers import NeptuneLogger
-                neptune_logger = NeptuneLogger()
-                trainer = Trainer(loggers=neptune_logger, ...)
-                trainer.fit()
-                neptune_logger.neptune_run["some_metric"] = 1
-                trainer.close()
+        To log additional metadata to the run, access a path inside the run and assign metadata
+        with ``=`` or other `Neptune logging methods <https://docs.neptune.ai/logging/methods/>`_.
         """
         from neptune import Run
 
         if not self._neptune_run:
             self._neptune_run = Run(
                 project=self._project,
                 api_token=self._api_token,
@@ -127,27 +130,18 @@
             )
         return self._neptune_run
 
     @property
     def base_handler(self):
         """Gets a handler for the base logging namespace.
 
-        Use the handler to log extra metadata to the run and organize it under the base namespace (default: "training").
-        You can operate on it like a run object: Access a path inside the handler and assign metadata to it with "=" or
-        other [Neptune logging methods](https://docs.neptune.ai/logging/methods/).
-
-        Example:
-                from composer import Trainer
-                from composer.loggers import NeptuneLogger
-                neptune_logger = NeptuneLogger()
-                trainer = Trainer(loggers=neptune_logger, ...)
-                trainer.fit()
-                neptune_logger.base_handler["some_metric"] = 1
-                trainer.close()
-            Result: The value `1` is organized under "training/some_metric" inside the run.
+        Use the handler to log extra metadata to the run and organize it under the base namespace
+        (default: "training"). You can operate on it like a run object: Access a path inside the
+        handler and assign metadata to it with ``=`` or other
+        `Neptune logging methods <https://docs.neptune.ai/logging/methods/>`_.
         """
         return self.neptune_run[self._base_namespace]
 
     def init(self, state: 'State', logger: 'Logger') -> None:
         del logger  # unused
 
         self.base_handler['rank'] = dist.get_global_rank()
@@ -209,47 +203,53 @@
 
         from neptune.utils import stringify_unsupported
 
         self.base_handler[NeptuneLogger.trace_namespace] = stringify_unsupported(traces)
 
     def can_upload_files(self) -> bool:
         """Whether the logger supports uploading files."""
-        return self._enabled and self._upload_artifacts
+        return self._enabled and self._upload_checkpoints
 
     def upload_file(
         self,
         state: 'State',
         remote_file_name: str,
         file_path: pathlib.Path,
         *,
         overwrite: bool = False,
     ):
         if not self.can_upload_files():
             return
 
+        if file_path.is_symlink() or file_path.suffix.lower() == '.symlink':
+            return  # skip symlinks
+
         neptune_path = f'{self._base_namespace}/{remote_file_name}'
         if self.neptune_run.exists(neptune_path) and not overwrite:
 
             warnings.warn(
                 f"The file '{neptune_path}' already exists and overwrite is set to False."
                 'No action will be taken.',
             )
             return
 
         del state  # unused
-        self.base_handler[remote_file_name].upload(str(file_path))
+
+        from neptune.types import File
+
+        with open(str(file_path), 'rb') as fp:
+            self.base_handler[remote_file_name] = File.from_stream(fp, extension=file_path.suffix)
 
     def download_file(
         self,
         remote_file_name: str,
         destination: str,
         overwrite: bool = False,
         progress_bar: bool = True,
     ):
-        del progress_bar  # not supported
 
         if not self._enabled:
             return
 
         if os.path.exists(
             os.path.join(
                 destination,
@@ -262,15 +262,19 @@
             )
             return
 
         file_path = f'{self._base_namespace}/{remote_file_name}'
         if not self.neptune_run.exists(file_path):
             raise FileNotFoundError(f'File {file_path} not found')
 
-        self.base_handler[remote_file_name].download(destination=destination)
+        if _is_progress_bar_enabled():
+            self.base_handler[remote_file_name].download(destination=destination, progress_bar=progress_bar)
+        else:
+            del progress_bar
+            self.base_handler[remote_file_name].download(destination=destination)
 
     def log_images(
         self,
         images: Union[np.ndarray, torch.Tensor, Sequence[Union[np.ndarray, torch.Tensor]]],
         name: str = 'Images',
         channels_last: bool = False,
         step: Optional[int] = None,
@@ -308,8 +312,46 @@
     # Error out for empty arrays or weird arrays of dimension 0.
     if np.any(np.equal(img_numpy.shape, 0)):
         raise ValueError(f'Got an image (shape {img_numpy.shape}) with at least one dimension being 0! ')
 
     if not channels_last:
         img_numpy = np.moveaxis(img_numpy, 0, -1)
 
-    return img_numpy
+    return _validate_image_value_range(img_numpy)
+
+
+def _validate_image_value_range(img: np.ndarray) -> np.ndarray:
+    array_min = img.min()
+    array_max = img.max()
+
+    if (array_min >= 0 and 1 < array_max <= 255) or (array_min >= 0 and array_max <= 1):
+        return img
+
+    from neptune.common.warnings import NeptuneWarning, warn_once
+
+    warn_once(
+        'Image value range is not in the expected range of [0.0, 1.0] or [0, 255]. '
+        'This might be due to the presence of `transforms.Normalize` in the data pipeline. '
+        'Logged images may not display correctly in Neptune.',
+        exception=NeptuneWarning,
+    )
+
+    return _scale_image_to_0_255(img, array_min, array_max)
+
+
+def _scale_image_to_0_255(img: np.ndarray, array_min: Union[int, float], array_max: Union[int, float]) -> np.ndarray:
+    scaled_image = 255 * (img - array_min) / (array_max - array_min)
+    return scaled_image.astype(np.uint8)
+
+
+def _warn_about_deprecated_upload_artifacts() -> None:
+    warnings.warn(
+        VersionedDeprecationWarning(
+            'The \'upload_artifacts\' parameter is deprecated and will be removed in the next version. '
+            'Use the \'upload_checkpoints\' parameter instead.',
+            remove_version='0.23',
+        ),
+    )
+
+
+def _is_progress_bar_enabled() -> bool:
+    return Version(version('neptune')) >= NEPTUNE_VERSION_WITH_PROGRESS_BAR
```

### Comparing `composer-0.21.2/composer/loggers/progress_bar_logger.py` & `composer-0.21.3/composer/loggers/progress_bar_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/remote_uploader_downloader.py` & `composer-0.21.3/composer/loggers/remote_uploader_downloader.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/slack_logger.py` & `composer-0.21.3/composer/loggers/slack_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/tensorboard_logger.py` & `composer-0.21.3/composer/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loggers/wandb_logger.py` & `composer-0.21.3/composer/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loss/loss.py` & `composer-0.21.3/composer/loss/loss.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/loss/utils.py` & `composer-0.21.3/composer/loss/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/metrics/__init__.py` & `composer-0.21.3/composer/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/metrics/map.py` & `composer-0.21.3/composer/metrics/map.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/metrics/metrics.py` & `composer-0.21.3/composer/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/metrics/nlp.py` & `composer-0.21.3/composer/metrics/nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/models/__init__.py` & `composer-0.21.3/composer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/models/base.py` & `composer-0.21.3/composer/models/base.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/models/huggingface.py` & `composer-0.21.3/composer/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/models/initializers.py` & `composer-0.21.3/composer/models/initializers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/models/tasks/classification.py` & `composer-0.21.3/composer/models/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/optim/__init__.py` & `composer-0.21.3/composer/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/optim/decoupled_weight_decay.py` & `composer-0.21.3/composer/optim/decoupled_weight_decay.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/optim/scheduler.py` & `composer-0.21.3/composer/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/__init__.py` & `composer-0.21.3/composer/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/json_trace_handler.py` & `composer-0.21.3/composer/profiler/json_trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/json_trace_merger.py` & `composer-0.21.3/composer/profiler/json_trace_merger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/marker.py` & `composer-0.21.3/composer/profiler/marker.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/profiler.py` & `composer-0.21.3/composer/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/profiler_action.py` & `composer-0.21.3/composer/profiler/profiler_action.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/profiler_schedule.py` & `composer-0.21.3/composer/profiler/profiler_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/system_profiler.py` & `composer-0.21.3/composer/profiler/system_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/torch_profiler.py` & `composer-0.21.3/composer/profiler/torch_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/trace_handler.py` & `composer-0.21.3/composer/profiler/trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/profiler/utils.py` & `composer-0.21.3/composer/profiler/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/trainer/_deepspeed.py` & `composer-0.21.3/composer/trainer/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/trainer/_scale_schedule.py` & `composer-0.21.3/composer/trainer/_scale_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/trainer/_scaler.py` & `composer-0.21.3/composer/trainer/_scaler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/trainer/dist_strategy.py` & `composer-0.21.3/composer/trainer/dist_strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,14 +143,16 @@
 
 
 def set_fsdp_default(fsdp_config: Dict[str, Any]):
     """Modify fsdp_config to set default values for missing keys."""
     fsdp_config.setdefault('activation_checkpointing', False)
     fsdp_config.setdefault('activation_checkpointing_reentrant', True)
     fsdp_config.setdefault('activation_cpu_offload', False)
+    fsdp_config.setdefault('te_checkpoint_wrapper', False)
+    fsdp_config.setdefault('te_shard_fp8_weight', False)
     fsdp_config.setdefault('backward_prefetch', 'BACKWARD_POST')
     fsdp_config.setdefault('backward_prefetch_limit', 1)
     fsdp_config.setdefault('cpu_offload', False)
     fsdp_config.setdefault('forward_prefetch', False)
     fsdp_config.setdefault('forward_prefetch_limit', 1)
     fsdp_config.setdefault('ignored_modules', None)
     fsdp_config.setdefault('keep_low_precision_grads', False)
@@ -210,24 +212,26 @@
 def prepare_fsdp_module(
     model: torch.nn.Module,
     optimizers: Optional[Union[torch.optim.Optimizer, Sequence[torch.optim.Optimizer]]],
     fsdp_config: Dict[str, Any],
     precision: Precision,
     device: Device,
     auto_microbatching: bool,
+    te_rng_seed: int = 1234,
 ) -> None:
     """Prepare a module (assumed ComposerModel) and optimizer for use with :class:`torch.distributed.fsdp.FullyShardedDataParallel`.
 
     Args:
         model (torch.nn.Module): The model to wrap.
         optimizers (torch.optim.Optimizer | Sequence[torch.optim.Optimizer], optional): The optimizer for `model`, assumed to have a single param group := model.parameters().
         fsdp_config (Dict[str, Any]): The FSDP config.
         precision: (Precision): The precision being used by the Trainer, used to fill in defaults for FSDP `mixed_precision` settings.
         device (Device): The device being used by the Trainer.
         auto_microbatching (bool, optional): Whether or not auto microbatching is enabled.
+        te_rng_seed(int): The seed to use for the Transformer Engine activation checkpointing RNG. Defaults to 1234.
     """
     patch_pytorch()
 
     set_fsdp_default(fsdp_config)
 
     # Check sync_module_states is True for mixed initialization or HSDP
     if fsdp_config['sync_module_states'] == False:
@@ -384,14 +388,16 @@
     activation_cpu_offload = fsdp_config['activation_cpu_offload']
     sync_module_states = fsdp_config['sync_module_states']
     forward_prefetch = fsdp_config['forward_prefetch']
     limit_all_gathers = fsdp_config['limit_all_gathers']
     ignored_modules = fsdp_config['ignored_modules']
     state_dict_type = fsdp_config['state_dict_type']
     activation_checkpointing_reentrant = fsdp_config['activation_checkpointing_reentrant']
+    te_checkpoint_wrapper = fsdp_config['te_checkpoint_wrapper'] if precision == Precision.AMP_FP8 else False
+    te_shard_fp8_weight = fsdp_config['te_shard_fp8_weight'] if precision == Precision.AMP_FP8 else False
     sharded_ckpt_prefix_dir = fsdp_config['sharded_ckpt_prefix_dir']
     use_orig_params = fsdp_config['use_orig_params']
 
     # We choose to not wrap the ComposerModel directly, but instead wrap any submodules like `ComposerModel.model`
     # This makes it safer to call ComposerModel-specific functions like 'eval_forward' that
     # may make calls to sharded submodules. If we only wrap the submodules, then any call that ComposerModel makes
     # to a FSDP-wrapped submodule's `forward()` function will be safe and all-gather the necessary weights before `forward()`.
@@ -594,14 +600,22 @@
                 sync_module_states=sync_module_states,
                 forward_prefetch=forward_prefetch,
                 limit_all_gathers=limit_all_gathers,
                 use_orig_params=use_orig_params,
                 **kwargs,
             )
 
+            if te_shard_fp8_weight:
+                try:
+                    from transformer_engine.pytorch.distributed import prepare_te_modules_for_fsdp
+                except ModuleNotFoundError:
+                    raise ModuleNotFoundError('Please install transformer-engine to use prepare_te_modules_for_fsdp')
+                log.info(f'Calling prepare_te_modules_for_fsdp to enable TE weights sharding')
+                prepare_te_modules_for_fsdp(fsdp_obj)
+
             if hasattr(fsdp_obj, '_exec_order_data'):
                 if hasattr(fsdp_obj._exec_order_data, '_forward_prefetch_limit'):
                     fsdp_obj._exec_order_data._forward_prefetch_limit = fsdp_config['forward_prefetch_limit']
                 else:
                     warnings.warn(
                         'FSDP._exec_order_data does not have attribute _forward_prefetch_limit '
                         'which is unexpected and will result in `forward_prefetch_limit` from FSDP '
@@ -620,29 +634,59 @@
                     'FSDP does not have attribute _exec_order_data which is unexpected and will '
                     'result in `forward_prefetch_limit` and `backward_prefetch_limit` from FSDP '
                     'config being ignored. Please open an issue to Composer to report this.',
                 )
 
             # Activation Checkpointing
             if activation_checkpointing or activation_cpu_offload:
+                # FP8 TE requires using the TE checkpoint function, FSDP activation checkpointing only works with TE non-reentrant checkpointing
+                if te_checkpoint_wrapper:
+                    assert not activation_checkpointing_reentrant, 'TE checkpoint only works with non-reentrant checkpointing'
                 if version.parse(torch.__version__) > version.parse('2.1.0.dev'):
                     from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import offload_wrapper
                     if not activation_checkpointing_reentrant:
-                        first_wrap_fn = lambda m: checkpoint_wrapper(
-                            m,
-                            checkpoint_impl=CheckpointImpl.NO_REENTRANT,
-                        ) if activation_checkpointing else (lambda module: module)
+                        if te_checkpoint_wrapper:
+                            try:
+                                import transformer_engine.pytorch as te
+                            except ModuleNotFoundError:
+                                raise ModuleNotFoundError(
+                                    'Please install transformer-engine to use TE checkpoint wrapper',
+                                )
+
+                            # RNG state tracker for checkpointing
+                            CUDA_RNG_STATES_TRACKER = te.distributed.CudaRNGStatesTracker()
+                            CUDA_RNG_STATES_TRACKER.add('fsdp-rng', te_rng_seed)
+
+                            def get_cuda_rng_tracker():
+                                return CUDA_RNG_STATES_TRACKER
+
+                            first_wrap_fn = lambda m: checkpoint_wrapper(
+                                m,
+                                context_fn=te.distributed.get_activation_recompute_contexts,
+                                checkpoint_fn=te.distributed.checkpoint,
+                                use_reentrant=False,
+                                get_rng_state_tracker=get_cuda_rng_tracker,
+                            )
+                        else:
+                            first_wrap_fn = lambda m: checkpoint_wrapper(
+                                m,
+                                checkpoint_impl=CheckpointImpl.NO_REENTRANT,
+                            ) if activation_checkpointing else (lambda module: module)
                         second_wrap_fn = (
                             lambda module: offload_wrapper(
                                 first_wrap_fn(module)
                                 if activation_checkpointing else module,  # type: ignore reportGeneralTypeIssues
                             )
                         ) if activation_cpu_offload else first_wrap_fn
                     else:
-                        first_wrap_fn = checkpoint_wrapper if activation_checkpointing else (lambda module: module)
+
+                        first_wrap_fn = lambda m: checkpoint_wrapper(
+                            m,
+                            checkpoint_impl=CheckpointImpl.REENTRANT,
+                        ) if activation_checkpointing else (lambda module: module)
                         second_wrap_fn = (
                             lambda module: offload_wrapper(
                                 first_wrap_fn(module)
                                 if activation_checkpointing else module,  # type: ignore reportGeneralTypeIssues
                             )
                         ) if activation_cpu_offload else first_wrap_fn
                 else:
@@ -695,14 +739,16 @@
         log.info(f'FSDP: Wrapped model: {model}')
         log.info(f'FSDP: Using sharding_strategy={sharding_strategy}')
         log.info(f'FSDP: Using cpu_offload={cpu_offload}')
         log.info(f'FSDP: Using mixed_precision={mixed_precision}')
         log.info(f'FSDP: Using backward_prefetch={backward_prefetch}')
         log.info(f'FSDP: Using activation_checkpointing={activation_checkpointing}')
         log.info(f'FSDP: Using activation_cpu_offload={activation_cpu_offload}')
+        log.info(f'FSDP: Using te_checkpoint_wrapper={te_checkpoint_wrapper}')
+        log.info(f'FSDP: Using te_shard_fp8_weight={te_shard_fp8_weight}')
         log.info(f'FSDP: Using sync_module_states={sync_module_states}')
         log.info(f'FSDP: Using forward_prefetch={forward_prefetch}')
         log.info(f'FSDP: Using limit_all_gathers={limit_all_gathers}')
         log.info(f'FSDP: Using state_dict_type={state_dict_type}')
         log.info(f'FSDP: Using sharded_ckpt_prefix_dir={sharded_ckpt_prefix_dir}')
 
     # Rebuild optimizer now that parameters are sharded
```

### Comparing `composer-0.21.2/composer/trainer/meta_safe_apply.py` & `composer-0.21.3/composer/trainer/meta_safe_apply.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/trainer/mosaic_fsdp.py` & `composer-0.21.3/composer/trainer/mosaic_fsdp.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,15 +59,21 @@
 
         # Allow 2D HSDP
         from torch.distributed.fsdp import _runtime_utils
         _runtime_utils._validate_and_get_hybrid_shard_state = lambda *args, **kwargs: None
 
     elif version.parse(torch.__version__) < version.parse('2.2.9'):
         # Monkey patch for torch < 2.3.0 ie torch == 2.2.1/2.2.2 currently
-        pass
+
+        # Fix memory leak for FSDP.optim_state_dict_to_load
+        # https://github.com/pytorch/pytorch/issues/116553
+        from torch.distributed.fsdp import _optim_utils
+
+        from composer.trainer.mosaic_fsdp_utils import _shard_orig_param_state
+        _optim_utils._shard_orig_param_state = _shard_orig_param_state
 
     elif version.parse(torch.__version__) < version.parse('2.3.1'):
         # Monkey patch for torch < 2.3.1 ie torch == 2.3.0
         # Note: this is the same patch as 2.2.0, we are just making a new if branch
         # for clarity and modularity of changes.
 
         # Allow 2D HSDP
@@ -92,7 +98,14 @@
 
         # Monkeypatch checkpointing full state dict
         from torch.distributed.fsdp import _state_dict_utils
 
         from composer.trainer.mosaic_fsdp_utils import _full_pre_state_dict_hook, _set_use_dtensor
         _state_dict_utils._full_pre_state_dict_hook = _full_pre_state_dict_hook
         _state_dict_utils._set_use_dtensor = _set_use_dtensor
+
+        # Monkeypatch _flat_param.py to fix 2D with SHARD_GRAD_OP
+        # Issue: https://github.com/pytorch/pytorch/issues/123272
+        from torch.distributed.fsdp import _flat_param
+
+        from composer.trainer.mosaic_fsdp_utils import _same_storage
+        _flat_param._same_storage = _same_storage
```

### Comparing `composer-0.21.2/composer/trainer/mosaic_fsdp_utils.py` & `composer-0.21.3/composer/trainer/mosaic_fsdp_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1112,7 +1112,54 @@
                     'DeviceMesh is not compatible with LOCAL_STATE_DICT.',
                     'Please set state_dict_type to SHARDED_STATE_DICT to get DTensor state_dict.',
                 )
             elif state_dict_type == StateDictType.FULL_STATE_DICT:
                 pass
             else:
                 fsdp_state._state_dict_config._use_dtensor = True  # type: ignore
+
+    @no_type_check
+    def _same_storage(a, b):
+        if isinstance(a, DTensor):
+            a = a._local_tensor
+        if isinstance(b, DTensor):
+            b = b._local_tensor
+        return a.untyped_storage().data_ptr() == b.untyped_storage().data_ptr()
+
+if version.parse(torch.__version__) >= version.parse('2.2.1') and version.parse(
+        torch.__version__,) < version.parse('2.2.9'):
+
+    from torch.distributed.fsdp._optim_utils import FSDPParamInfo
+    from torch.distributed.checkpoint._state_dict_utils import _gather_state_dict
+
+    @no_type_check
+    def _shard_orig_param_state(
+        fsdp_param_info: FSDPParamInfo,
+        fqn: str,
+        optim_state: Dict[str, Any],
+    ) -> Dict[str, Any]:
+        if not optim_state:
+            return {}
+        fsdp_state = fsdp_param_info.state
+        flat_param = fsdp_param_info.handle.flat_param
+        param_idx = fsdp_param_info.param_indices[fqn]
+        shard_param_info = flat_param._shard_param_infos[param_idx]  # type: ignore[attr-defined]
+        optim_state = _gather_state_dict(
+            optim_state, pg=fsdp_state.process_group, device=fsdp_state.compute_device,
+        )
+        if not shard_param_info.in_shard:
+            return {}
+        # Flatten and shard the state.
+        new_optim_state: Dict[str, Any] = {}
+        intra_param_start_idx = shard_param_info.intra_param_start_idx
+        intra_param_end_idx = shard_param_info.intra_param_end_idx
+        for state_name, value in optim_state.items():
+            if (
+                torch.is_tensor(value)
+                and value.dim() > 0
+                and fsdp_state.sharding_strategy != ShardingStrategy.NO_SHARD
+            ):
+                # This clone() is the patch to fix the OOM
+                # https://github.com/pytorch/pytorch/pull/117261
+                value = value.flatten()[intra_param_start_idx : intra_param_end_idx + 1].clone()  # type: ignore[operator]
+            new_optim_state[state_name] = value
+        return new_optim_state
```

### Comparing `composer-0.21.2/composer/trainer/trainer.py` & `composer-0.21.3/composer/trainer/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         raise ValueError(
             'Auto microbatching on evaluators is not compatible with sequence parallelism. '
             'Please manually set device_eval_microbatch_size or disable sequence parallelism .',
         )
     if hasattr(
         evaluator.dataloader,
         'seq_parallel_world_size',
-    ) and evaluator.dataloader.seq_parallel_world_size > 1 and evaluator.dataloader.batch_size * evaluator.dataloader.seq_parallel_world_size != 1:  # type: ignore
+    ) and evaluator.dataloader.seq_parallel_world_size > 1 and evaluator.dataloader.device_eval_batch_size * evaluator.dataloader.seq_parallel_world_size != 1:  # type: ignore
         raise ValueError(
             'Sequence parallelism requires a microbatch size of 1 distributed over the sequence parallel group.',
         )
 
 
 def _distribute_and_get_random_seed(seed: Optional[int], device: Device):
     if seed is None:
@@ -1546,15 +1546,23 @@
         # If using DeepSpeed, the engine must be initialized before the model is loaded.
         # If using FSDP, the model must be wrapped and then loaded unless loading a monolith
         # checkpoint on rank 0 only, in which case the model be loaded before it is wrapped.
 
         # FSDP wrap if not using monolith checkpoint on rank 0 only
         if self.state.fsdp_config is not None and fsdp_auto_wrap and not self.state.load_fsdp_monolith_rank0_only:
             with reproducibility.seed_context(self.state.rank_zero_seed):
-                prepare_fsdp_module(model, optimizers, self.state.fsdp_config, precision, device, auto_microbatching)
+                prepare_fsdp_module(
+                    model,
+                    optimizers,
+                    self.state.fsdp_config,
+                    precision,
+                    device,
+                    auto_microbatching,
+                    self.state.seed,
+                )
 
         # Configure Deepspeed
         if self.state.deepspeed_config is not None:
             for callback in self.state.callbacks:
                 if isinstance(callback, OptimizerMonitor):
                     raise ValueError(
                         'OptimizerMonitor is not supported with DeepSpeed because DeepSpeed clears '
@@ -2235,22 +2243,20 @@
                     metric_data = getattr(metric, key)
                     if isinstance(metric_data, torch.Tensor) and metric_data.dtype == torch.float16:
                         metric_data = metric_data.to(torch.float32)  # type: ignore
                         setattr(metric, key, metric_data)
         return metrics
 
     def _compute_and_log_metrics(self, dataloader_label: str, metrics: Dict[str, Metric]):
-        """Computes metrics, logs the results, and updates the state with the deep-copied metrics.
+        """Computes metrics, logs the results, and updates the state with the metrics.
 
         Args:
             dataloader_label (str): The dataloader label.
             metrics (Dict[str, Metric]): The metrics to compute.
         """
-        metrics = deepcopy(metrics)
-
         # log computed metrics
         computed_metrics = {}
         for metric_name, metric in metrics.items():
             computed_metrics[metric_name] = metric.compute()
 
         self.logger.log_metrics({f'metrics/{dataloader_label}/{name}': val for (name, val) in computed_metrics.items()
                                 },)
```

### Comparing `composer-0.21.2/composer/utils/__init__.py` & `composer-0.21.3/composer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/auto_log_hparams.py` & `composer-0.21.3/composer/utils/auto_log_hparams.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/batch_helpers.py` & `composer-0.21.3/composer/utils/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/checkpoint.py` & `composer-0.21.3/composer/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/collect_env.py` & `composer-0.21.3/composer/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/compression.py` & `composer-0.21.3/composer/utils/compression.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/device.py` & `composer-0.21.3/composer/utils/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/dist.py` & `composer-0.21.3/composer/utils/dist.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/eval_client/__init__.py` & `composer-0.21.3/composer/utils/eval_client/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/eval_client/eval_client.py` & `composer-0.21.3/composer/utils/eval_client/eval_client.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/eval_client/lambda_eval_client.py` & `composer-0.21.3/composer/utils/eval_client/lambda_eval_client.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/eval_client/local_eval_client.py` & `composer-0.21.3/composer/utils/eval_client/local_eval_client.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/eval_client/mosaicml_lambda_eval_client.py` & `composer-0.21.3/composer/utils/eval_client/mosaicml_lambda_eval_client.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/file_helpers.py` & `composer-0.21.3/composer/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/fx_utils.py` & `composer-0.21.3/composer/utils/fx_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/import_helpers.py` & `composer-0.21.3/composer/utils/import_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/inference.py` & `composer-0.21.3/composer/utils/inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/iter_helpers.py` & `composer-0.21.3/composer/utils/iter_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/misc.py` & `composer-0.21.3/composer/utils/misc.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/module_surgery.py` & `composer-0.21.3/composer/utils/module_surgery.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/object_store/__init__.py` & `composer-0.21.3/composer/utils/object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/object_store/gcs_object_store.py` & `composer-0.21.3/composer/utils/object_store/gcs_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/object_store/libcloud_object_store.py` & `composer-0.21.3/composer/utils/object_store/libcloud_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/object_store/mlflow_object_store.py` & `composer-0.21.3/composer/utils/object_store/mlflow_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/object_store/object_store.py` & `composer-0.21.3/composer/utils/object_store/object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/object_store/oci_object_store.py` & `composer-0.21.3/composer/utils/object_store/oci_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/object_store/s3_object_store.py` & `composer-0.21.3/composer/utils/object_store/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/object_store/sftp_object_store.py` & `composer-0.21.3/composer/utils/object_store/sftp_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/object_store/uc_object_store.py` & `composer-0.21.3/composer/utils/object_store/uc_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/reproducibility.py` & `composer-0.21.3/composer/utils/reproducibility.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/retrying.py` & `composer-0.21.3/composer/utils/retrying.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/string_enum.py` & `composer-0.21.3/composer/utils/string_enum.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer/utils/warnings.py` & `composer-0.21.3/composer/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer.egg-info/PKG-INFO` & `composer-0.21.3/composer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.21.2
+Version: 0.21.3
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: composer Version: 0.21.2 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.21.3 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.9 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
```

### Comparing `composer-0.21.2/composer.egg-info/SOURCES.txt` & `composer-0.21.3/composer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/composer.egg-info/requires.txt` & `composer-0.21.3/composer.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,92 +11,92 @@
 tabulate==0.9.0
 py-cpuinfo<10,>=8.0.0
 packaging<24.1,>=21.3.0
 importlib-metadata<7,>=5.0.0
 mosaicml-cli<0.7,>=0.5.25
 
 [all]
-recommonmark==0.7.1
-pillow==9.3.0
-onnx<2,>=1.12.0
+comet_ml<4.0.0,>=3.31.12
+sphinx==4.4.0
+paramiko<3,>=2.11.0
+sphinxcontrib-images==0.9.4
+traitlets==5.14.2
+sphinxcontrib-serializinghtml==1.1.5
 sphinxcontrib-devhelp==1.0.0
-ipython==8.11.0
-yamllint==1.35.1
-pynvml<12,>=11.5.0
-onnxruntime<2,>=1.12.1
+pandoc==2.3
+sphinx_panels==0.6.0
+coverage[toml]==7.4.4
+pytest==7.4.4
+custom_inherit==2.4.1
+sphinxext.opengraph==0.9.1
+GitPython==3.1.43
+slack_sdk<4,>=3.19.5
+myst-parser==0.16.1
+tensorboard<3.0.0,>=2.9.1
+transformers!=4.34.0,<4.41,>=4.11
+py-cpuinfo<10,>=8.0.0
+mlflow<3.0,>=2.11.1
+furo==2022.9.29
+sphinxcontrib.katex==0.9.6
+oci<3.0.0,>=2.88.2
 ipykernel==6.29.2
-jupyter==1.0.0
+nbsphinx==0.9.1
+fasteners==0.18
+setuptools<=59.5.0
+databricks-sdk==0.25.1
+sphinx_markdown_tables==0.0.17
 sphinxemoji==0.2.0
+neptune<2.0.0,>=1.6.2
+pypandoc==1.13
+docutils==0.17.1
+moto[s3]<5,>=4.0.1
+deepspeed==0.8.3
 protobuf<5.27
-sphinxcontrib-serializinghtml==1.1.5
-databricks-sdk==0.23.0
-oci<3.0.0,>=2.88.2
-sphinxcontrib.katex==0.9.6
-pytest==7.4.4
-pandoc==2.3
+pytest_codeblocks==0.17.0
+testbook==0.4.2
+onnx<2,>=1.12.0
+sphinxcontrib-applehelp==1.0.0
+pandas<3.0,>=2.0.0
+pillow==9.3.0
+yamllint==1.35.1
 junitparser==3.1.2
-pypandoc==1.13
-neptune<2.0.0,>=1.6.2
-mlflow<3.0,>=2.11.1
+datasets<3,>=2.4
+pre-commit<4,>=3.4.0
+ipython==8.11.0
+onnxruntime<2,>=1.12.1
+peft<0.8,>=0.7.0
+mock-ssh-server==0.9.1
+sphinxcontrib-htmlhelp==2.0.0
 mosaicml-streaming<1.0
-boto3<2,>=1.21.45
+pynvml<12,>=11.5.0
+wandb<0.17,>=0.13.2
 google-cloud-storage<3.0,>=2.0.0
-fasteners==0.18
-transformers!=4.34.0,<4.40,>=4.11
-apache-libcloud<4,>=3.3.1
-sphinxcontrib-images==0.9.4
+recommonmark==0.7.1
+boto3<2,>=1.21.45
 pydantic<2,>=1.0
-pytest-httpserver<1.1,>=1.0.4
-myst-parser==0.16.1
-nbsphinx==0.9.1
-pre-commit<4,>=3.4.0
-cryptography==41.0.5
 sentencepiece==0.2.0
-py-cpuinfo<10,>=8.0.0
-sphinx_markdown_tables==0.0.17
-furo==2022.9.29
-sphinx-copybutton==0.5.2
-mock-ssh-server==0.9.1
-peft<0.8,>=0.7.0
-sphinxcontrib-htmlhelp==2.0.0
-coverage[toml]==7.4.4
-paramiko<3,>=2.11.0
-pytest_codeblocks==0.17.0
-sphinxext.opengraph==0.9.1
-sphinx_panels==0.6.0
-docutils==0.17.1
-traitlets==5.14.2
+pytest-httpserver<1.1,>=1.0.4
 sphinx-argparse==0.4.0
 sphinxcontrib-qthelp==1.0.0
-GitPython==3.1.43
-slack_sdk<4,>=3.19.5
-deepspeed==0.8.3
-pandas<3.0,>=2.0.0
-tensorboard<3.0.0,>=2.9.1
-custom_inherit==2.4.1
-moto[s3]<5,>=4.0.1
-sphinxcontrib-applehelp==1.0.0
-comet_ml<4.0.0,>=3.31.12
-setuptools<=59.5.0
-wandb<0.17,>=0.13.2
+sphinx-copybutton==0.5.2
+cryptography==41.0.5
+apache-libcloud<4,>=3.3.1
 pycocotools<3,>=2.0.4
-sphinx==4.4.0
-datasets<3,>=2.4
-testbook==0.4.2
+jupyter==1.0.0
 
 [base]
 
 [coco]
 pycocotools<3,>=2.0.4
 
 [comet_ml]
 comet_ml<4.0.0,>=3.31.12
 
 [databricks]
-databricks-sdk==0.23.0
+databricks-sdk==0.25.1
 
 [deepspeed]
 deepspeed==0.8.3
 pydantic<2,>=1.0
 
 [dev]
 custom_inherit==2.4.1
@@ -153,15 +153,15 @@
 [mlperf]
 py-cpuinfo<10,>=8.0.0
 
 [neptune]
 neptune<2.0.0,>=1.6.2
 
 [nlp]
-transformers!=4.34.0,<4.40,>=4.11
+transformers!=4.34.0,<4.41,>=4.11
 datasets<3,>=2.4
 
 [oci]
 oci<3.0.0,>=2.88.2
 
 [onnx]
 onnx<2,>=1.12.0
```

### Comparing `composer-0.21.2/pyproject.toml` & `composer-0.21.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/setup.py` & `composer-0.21.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 ]
 
 extra_deps['coco'] = [
     'pycocotools>=2.0.4,<3',
 ]
 
 extra_deps['nlp'] = [
-    'transformers>=4.11,!=4.34.0,<4.40',
+    'transformers>=4.11,!=4.34.0,<4.41',
     'datasets>=2.4,<3',
 ]
 
 extra_deps['peft'] = [
     'peft>=0.7.0,<0.8',
 ]
 
@@ -223,15 +223,15 @@
 
 extra_deps['mlflow'] = [
     'mlflow>=2.11.1,<3.0',
 ]
 
 extra_deps['pandas'] = ['pandas>=2.0.0,<3.0']
 
-extra_deps['databricks'] = ['databricks-sdk==0.23.0']
+extra_deps['databricks'] = ['databricks-sdk==0.25.1']
 
 extra_deps['all'] = {dep for deps in extra_deps.values() for dep in deps}
 
 composer_data_files = ['py.typed']
 composer_data_files += package_files('composer', 'yamls', '.yaml')
 composer_data_files += package_files('composer', 'algorithms', '.json')
```

### Comparing `composer-0.21.2/tests/test_cli.py` & `composer-0.21.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_device.py` & `composer-0.21.3/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_docs.py` & `composer-0.21.3/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_engine.py` & `composer-0.21.3/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_events.py` & `composer-0.21.3/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_full_nlp.py` & `composer-0.21.3/tests/test_full_nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_loss.py` & `composer-0.21.3/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_notebooks.py` & `composer-0.21.3/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_passes.py` & `composer-0.21.3/tests/test_passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_precision.py` & `composer-0.21.3/tests/test_precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_simple_nlp.py` & `composer-0.21.3/tests/test_simple_nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_smoketest.py` & `composer-0.21.3/tests/test_smoketest.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_split_batch.py` & `composer-0.21.3/tests/test_split_batch.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_state.py` & `composer-0.21.3/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.2/tests/test_time.py` & `composer-0.21.3/tests/test_time.py`

 * *Files identical despite different names*

