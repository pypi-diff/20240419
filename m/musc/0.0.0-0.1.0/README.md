# Comparing `tmp/musc-0.0.0.tar.gz` & `tmp/musc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musc-0.0.0.tar", last modified: Wed Mar 27 16:42:47 2024, max compression
+gzip compressed data, was "musc-0.1.0.tar", last modified: Fri Apr 19 03:08:53 2024, max compression
```

## Comparing `musc-0.0.0.tar` & `musc-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,36 @@
--rw-r--r--   0        0        0        8 2024-03-27 16:39:32.481747 musc-0.0.0/README.md
--rw-r--r--   0        0        0      105 2024-03-27 16:33:29.909031 musc-0.0.0/musc/__init__.py
--rw-r--r--   0        0        0      352 2024-03-27 16:42:47.254780 musc-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      199 1970-01-01 00:00:00.000000 musc-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2024-04-02 06:41:46.000000 musc-0.1.0/README.md
+-rw-r--r--   0        0        0      125 2024-04-02 06:41:46.000000 musc-0.1.0/musc/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-02 06:41:46.000000 musc-0.1.0/musc/adaptors/drift_detectors/a.py
+-rw-r--r--   0        0        0     2963 2024-04-02 06:41:46.000000 musc-0.1.0/musc/adaptors/drift_detectors/river/a.py
+-rw-r--r--   0        0        0     2103 2024-04-02 06:41:46.000000 musc-0.1.0/musc/adaptors/drift_detectors/river/with_kdp/__init__.py
+-rw-r--r--   0        0        0     4139 2024-04-02 06:41:46.000000 musc-0.1.0/musc/adaptors/models.py
+-rw-r--r--   0        0        0     2070 2024-04-02 06:41:46.000000 musc-0.1.0/musc/commons.py
+-rw-r--r--   0        0        0     3123 2024-04-02 06:41:46.000000 musc-0.1.0/musc/evaluator/a.py
+-rw-r--r--   0        0        0     8188 2024-04-02 06:41:46.000000 musc-0.1.0/musc/evaluator/a2.py
+-rw-r--r--   0        0        0     1288 2024-04-02 06:41:46.000000 musc-0.1.0/musc/evaluator/active_count.py
+-rw-r--r--   0        0        0     3205 2024-04-02 06:41:46.000000 musc-0.1.0/musc/evaluator/high_level.py
+-rw-r--r--   0        0        0     1195 2024-04-02 06:41:46.000000 musc-0.1.0/musc/high_level/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-02 06:41:46.000000 musc-0.1.0/musc/high_level/drift_detectors/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-02 06:41:46.000000 musc-0.1.0/musc/high_level/drift_detectors/river/__init__.py
+-rw-r--r--   0        0        0    12350 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/a.py
+-rw-r--r--   0        0        0     7120 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/distr/a.py
+-rw-r--r--   0        0        0     2223 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/distr/high_level.py
+-rw-r--r--   0        0        0    26682 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/high_level/a.py
+-rw-r--r--   0        0        0     2362 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/high_level/helper.py
+-rw-r--r--   0        0        0      378 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/res_pool/base.py
+-rw-r--r--   0        0        0     2730 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/res_pool/global_.py
+-rw-r--r--   0        0        0     1079 2024-04-02 06:41:46.000000 musc-0.1.0/musc/hpo/res_pool/torch_device.py
+-rw-r--r--   0        0        0     2312 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/a.py
+-rw-r--r--   0        0        0     4384 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/concepts/a.py
+-rw-r--r--   0        0        0     5591 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/concepts/high_level/a.py
+-rw-r--r--   0        0        0      666 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/concepts/high_level/no_clone.py
+-rw-r--r--   0        0        0      283 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/errors.py
+-rw-r--r--   0        0        0     3900 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/high_level.py
+-rw-r--r--   0        0        0     1549 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/data_history/base.py
+-rw-r--r--   0        0        0     4418 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/data_history/in_memory.py
+-rw-r--r--   0        0        0     5582 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/dd_process/a.py
+-rw-r--r--   0        0        0     6651 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/dd_process/dh_walker.py
+-rw-r--r--   0        0        0     1203 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/dd_process/stats.py
+-rw-r--r--   0        0        0     3468 2024-04-02 06:41:46.000000 musc-0.1.0/musc/service/impl/model_wrapper.py
+-rw-r--r--   0        0        0      532 2024-04-19 03:08:53.747504 musc-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 musc-0.1.0/PKG-INFO
```

