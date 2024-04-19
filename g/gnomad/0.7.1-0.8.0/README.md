# Comparing `tmp/gnomad-0.7.1.tar.gz` & `tmp/gnomad-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnomad-0.7.1.tar", last modified: Tue Oct 31 18:53:11 2023, max compression
+gzip compressed data, was "gnomad-0.8.0.tar", last modified: Fri Apr 19 14:23:00 2024, max compression
```

## Comparing `gnomad-0.7.1.tar` & `gnomad-0.8.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:53:11.801990 gnomad-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-10-31 18:50:46.000000 gnomad-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2023-10-31 18:53:11.797990 gnomad-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-10-31 18:50:46.000000 gnomad-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:53:11.793990 gnomad-0.7.1/gnomad/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:53:11.793990 gnomad-0.7.1/gnomad/assessment/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/assessment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27616 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/assessment/summary_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    49812 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/assessment/validity_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:53:11.793990 gnomad-0.7.1/gnomad/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:53:11.793990 gnomad-0.7.1/gnomad/resources/grch37/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/grch37/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/grch37/gnomad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/grch37/gnomad_ld.py
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/grch37/reference_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:53:11.797990 gnomad-0.7.1/gnomad/resources/grch38/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/grch38/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16280 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/grch38/gnomad.py
--rw-r--r--   0 runner    (1001) docker     (127)    15062 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/grch38/reference_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/import_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    25334 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/resources/resource_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:53:11.797990 gnomad-0.7.1/gnomad/sample_qc/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/sample_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17449 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/sample_qc/ancestry.py
--rw-r--r--   0 runner    (1001) docker     (127)    25487 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/sample_qc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)    31967 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/sample_qc/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/sample_qc/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    55151 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/sample_qc/relatedness.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/sample_qc/sex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:53:11.797990 gnomad-0.7.1/gnomad/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96224 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    56307 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24807 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/gen_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/liftover.py
--rw-r--r--   0 runner    (1001) docker     (127)    26422 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/reference_genome.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/release.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    47242 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/sparse_mt.py
--rw-r--r--   0 runner    (1001) docker     (127)    50385 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/vcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    28759 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/utils/vep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:53:11.797990 gnomad-0.7.1/gnomad/variant_qc/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/variant_qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16095 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/variant_qc/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/variant_qc/ld.py
--rw-r--r--   0 runner    (1001) docker     (127)    18486 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/variant_qc/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    19471 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/variant_qc/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2023-10-31 18:50:46.000000 gnomad-0.7.1/gnomad/variant_qc/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:53:11.793990 gnomad-0.7.1/gnomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2023-10-31 18:53:11.000000 gnomad-0.7.1/gnomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-10-31 18:53:11.000000 gnomad-0.7.1/gnomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 18:53:11.000000 gnomad-0.7.1/gnomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-10-31 18:53:11.000000 gnomad-0.7.1/gnomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-31 18:53:11.000000 gnomad-0.7.1/gnomad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-10-31 18:50:46.000000 gnomad-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 18:53:11.801990 gnomad-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-10-31 18:50:46.000000 gnomad-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:00.636622 gnomad-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-19 14:20:50.000000 gnomad-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-19 14:23:00.636622 gnomad-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-19 14:20:50.000000 gnomad-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:00.628622 gnomad-0.8.0/gnomad/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:00.628622 gnomad-0.8.0/gnomad/assessment/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/assessment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27616 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/assessment/summary_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52093 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/assessment/validity_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:00.628622 gnomad-0.8.0/gnomad/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:00.632622 gnomad-0.8.0/gnomad/resources/grch37/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/grch37/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/grch37/gnomad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/grch37/gnomad_ld.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14200 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/grch37/reference_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:00.632622 gnomad-0.8.0/gnomad/resources/grch38/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/grch38/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19219 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/grch38/gnomad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/grch38/reference_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/import_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27251 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/resources/resource_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:00.632622 gnomad-0.8.0/gnomad/sample_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/sample_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/sample_qc/ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/sample_qc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31967 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/sample_qc/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/sample_qc/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55152 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/sample_qc/relatedness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18465 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/sample_qc/sex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:00.636622 gnomad-0.8.0/gnomad/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107903 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61590 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27417 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/gen_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/liftover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26422 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/reference_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57632 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/sparse_mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16269 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/transcript_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57862 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/vcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34298 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/utils/vep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:00.636622 gnomad-0.8.0/gnomad/variant_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/variant_qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16095 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/variant_qc/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/variant_qc/ld.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18486 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/variant_qc/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19471 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/variant_qc/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-19 14:20:50.000000 gnomad-0.8.0/gnomad/variant_qc/training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:23:00.636622 gnomad-0.8.0/gnomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-19 14:23:00.000000 gnomad-0.8.0/gnomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-19 14:23:00.000000 gnomad-0.8.0/gnomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:23:00.000000 gnomad-0.8.0/gnomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 14:23:00.000000 gnomad-0.8.0/gnomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 14:23:00.000000 gnomad-0.8.0/gnomad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-19 14:20:50.000000 gnomad-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:23:00.636622 gnomad-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-19 14:20:50.000000 gnomad-0.8.0/setup.py
```

### Comparing `gnomad-0.7.1/LICENSE` & `gnomad-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/PKG-INFO` & `gnomad-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnomad
-Version: 0.7.1
+Version: 0.8.0
 Summary: Hail utilities for the Genome Aggregation Database
 Home-page: https://github.com/broadinstitute/gnomad_methods
 Author: The Genome Aggregation Database
 Author-email: gnomad@broadinstitute.org
 Project-URL: Documentation, https://broadinstitute.github.io/gnomad_methods/
 Project-URL: Source Code, https://github.com/broadinstitute/gnomad_methods
 Project-URL: Issues, https://github.com/broadinstitute/gnomad_methods/issues
```

### Comparing `gnomad-0.7.1/README.md` & `gnomad-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/assessment/summary_stats.py` & `gnomad-0.8.0/gnomad/assessment/summary_stats.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/assessment/validity_checks.py` & `gnomad-0.8.0/gnomad/assessment/validity_checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # noqa: D100
 
 import logging
 from pprint import pprint
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import hail as hl
 from hail.utils.misc import new_temp_file
 
 from gnomad.resources.grch38.gnomad import CURRENT_MAJOR_RELEASE, POPS, SEXES
 from gnomad.utils.vcf import HISTS, SORT_ORDER, make_label_combos
 
@@ -44,30 +44,32 @@
     :param cond_expr: Optional logical expression referring to annotations in ht to be checked.
     :param verbose: If True, show top values of annotations being checked, including checks that pass; if False, show only top values of annotations that fail checks.
     :param show_percent_sites: Show percentage of sites that fail checks. Default is False.
     :param n_fail: Optional number of sites that fail the conditional checks (previously computed). If not supplied, `cond_expr` is used to filter the Table and obtain the count of sites that fail the checks.
     :param ht_count: Optional number of sites within hail Table (previously computed). If not supplied, a count of sites in the Table is performed.
     :return: None
     """
-    if (n_fail is None and cond_expr is None) or (n_fail and cond_expr):
-        raise ValueError("One and only one of n_fail or cond_expr must be defined!")
+    if n_fail is None and cond_expr is None:
+        raise ValueError("At least one of n_fail or cond_expr must be defined!")
 
-    if cond_expr:
+    if n_fail is None and cond_expr is not None:
         n_fail = ht.filter(cond_expr).count()
 
     if show_percent_sites and (ht_count is None):
         ht_count = ht.count()
 
     if n_fail > 0:
         logger.info("Found %d sites that fail %s check:", n_fail, check_description)
         if show_percent_sites:
             logger.info(
                 "Percentage of sites that fail: %.2f %%", 100 * (n_fail / ht_count)
             )
-        ht.select(**display_fields).show()
+        if cond_expr is not None:
+            ht = ht.select(_fail=cond_expr, **display_fields)
+            ht.filter(ht._fail).drop("_fail").show()
     else:
         logger.info("PASSED %s check", check_description)
         if verbose:
             ht.select(**display_fields).show()
 
 
 def make_filters_expr_dict(
@@ -193,17 +195,16 @@
     for metric in metrics:
         if metric_first_field:
             check_field_left = f"{metric}{delimiter}{subset}{group}"
         else:
             check_field_left = f"{subset}{metric}{delimiter}{group}"
         check_field_right = f"sum{delimiter}{check_field_left}{delimiter}{sum_group}"
         field_check_expr[f"{check_field_left} = {check_field_right}"] = {
-            "expr": hl.agg.count_where(
-                t.info[check_field_left] != annot_dict[check_field_right]
-            ),
+            "expr": t.info[check_field_left] != annot_dict[check_field_right],
+            "agg_func": hl.agg.count_where,
             "display_fields": hl.struct(
                 **{
                     check_field_left: t.info[check_field_left],
                     check_field_right: annot_dict[check_field_right],
                 }
             ),
         }
@@ -306,54 +307,42 @@
         t.group_by(**group_exprs).aggregate(
             **make_filters_expr_dict(t, extra_filter_checks, variant_filter_field)
         ).order_by(hl.desc("n")).show(n_rows, n_cols)
 
     logger.info(
         "Checking distributions of filtered variants amongst variant filters..."
     )
-    _filter_agg_order(t, {"is_filtered": t.is_filtered})
-
-    logger.info("Checking distributions of variant type amongst variant filters...")
-    _filter_agg_order(t, {"allele_type": t.info.allele_type})
+    _filter_agg_order(t, {"is_filtered": t.is_filtered}, n_rows, n_cols)
 
-    logger.info(
-        "Checking distributions of variant type and region type amongst variant"
-        " filters..."
-    )
-    _filter_agg_order(
-        t,
-        {
-            "allele_type": t.info.allele_type,
-            "in_problematic_region": t.in_problematic_region,
-        },
-        n_rows,
-        n_cols,
-    )
+    add_agg_expr = {}
+    if "allele_type" in t.info:
+        logger.info("Checking distributions of variant type amongst variant filters...")
+        add_agg_expr["allele_type"] = t.info.allele_type
+        _filter_agg_order(t, add_agg_expr, n_rows, n_cols)
+
+    if "in_problematic_region" in t.row:
+        logger.info(
+            "Checking distributions of variant type and region type amongst variant"
+            " filters..."
+        )
+        add_agg_expr["in_problematic_region"] = t.in_problematic_region
+        _filter_agg_order(t, add_agg_expr, n_rows, n_cols)
 
-    logger.info(
-        "Checking distributions of variant type, region type, and number of alt alleles"
-        " amongst variant filters..."
-    )
-    _filter_agg_order(
-        t,
-        {
-            "allele_type": t.info.allele_type,
-            "in_problematic_region": t.in_problematic_region,
-            "n_alt_alleles": t.info.n_alt_alleles,
-        },
-        n_rows,
-        n_cols,
-    )
+    if "n_alt_alleles" in t.info:
+        logger.info(
+            "Checking distributions of variant type, region type, and number of alt alleles"
+            " amongst variant filters..."
+        )
+        add_agg_expr["n_alt_alleles"] = t.info.n_alt_alleles
+        _filter_agg_order(t, add_agg_expr, n_rows, n_cols)
 
 
 def generic_field_check_loop(
     ht: hl.Table,
-    field_check_expr: Dict[
-        str, Dict[str, Union[hl.expr.Int64Expression, hl.expr.StructExpression]]
-    ],
+    field_check_expr: Dict[str, Dict[str, Any]],
     verbose: bool,
     show_percent_sites: bool = False,
     ht_count: int = None,
 ) -> None:
     """
     Loop through all conditional checks for a given hail Table.
 
@@ -363,22 +352,23 @@
     :param field_check_expr: Dictionary whose keys are conditions being checked and values are the expressions for filtering to condition.
     :param verbose: If True, show top values of annotations being checked, including checks that pass; if False, show only top values of annotations that fail checks.
     :param show_percent_sites: Show percentage of sites that fail checks. Default is False.
     :param ht_count: Previously computed sum of sites within hail Table. Default is None.
     :return: None
     """
     ht_field_check_counts = ht.aggregate(
-        hl.struct(**{k: v["expr"] for k, v in field_check_expr.items()})
+        hl.struct(**{k: v["agg_func"](v["expr"]) for k, v in field_check_expr.items()})
     )
     for check_description, n_fail in ht_field_check_counts.items():
         generic_field_check(
             ht,
             check_description=check_description,
             n_fail=n_fail,
             display_fields=field_check_expr[check_description]["display_fields"],
+            cond_expr=field_check_expr[check_description]["expr"],
             verbose=verbose,
             show_percent_sites=show_percent_sites,
             ht_count=ht_count,
         )
 
 
 def compare_subset_freqs(
@@ -429,17 +419,16 @@
                         )
                     else:
                         check_field_right = (
                             f"{subset}{delimiter}{metric}{delimiter}{group}"
                         )
 
                     field_check_expr[f"{check_field_left} != {check_field_right}"] = {
-                        "expr": hl.agg.count_where(
-                            t.info[check_field_left] == t.info[check_field_right]
-                        ),
+                        "expr": t.info[check_field_left] == t.info[check_field_right],
+                        "agg_func": hl.agg.count_where,
                         "display_fields": hl.struct(
                             **{
                                 check_field_left: t.info[check_field_left],
                                 check_field_right: t.info[check_field_right],
                             }
                         ),
                     }
@@ -458,15 +447,15 @@
     logger.info("Total defined raw AC count: %s", total_defined_raw_ac)
 
 
 def sum_group_callstats(
     t: Union[hl.MatrixTable, hl.Table],
     sexes: List[str] = SEXES,
     subsets: List[str] = [""],
-    pops: List[str] = POPS[CURRENT_MAJOR_RELEASE],
+    pops: List[str] = POPS[CURRENT_MAJOR_RELEASE]["exomes"],
     groups: List[str] = ["adj"],
     additional_subsets_and_pops: Dict[str, List[str]] = None,
     verbose: bool = False,
     sort_order: List[str] = SORT_ORDER,
     delimiter: str = "-",
     metric_first_field: bool = True,
     metrics: List[str] = ["AC", "AN", "nhomalt"],
@@ -476,15 +465,15 @@
 
     Displays results from checking the sum of the specified annotations in stdout.
     Also checks that annotations for all expected sample populations are present.
 
     :param t: Input Table.
     :param sexes: List of sexes in table.
     :param subsets: List of sample subsets that contain pops passed in pops parameter. An empty string, e.g. "", should be passed to test entire callset. Default is [""].
-    :param pops: List of pops contained within the subsets. Default is POPS[CURRENT_MAJOR_RELEASE].
+    :param pops: List of pops contained within the subsets. Default is POPS[CURRENT_MAJOR_RELEASE]["exomes"].
     :param groups: List of callstat groups, e.g. "adj" and "raw" contained within the callset. gnomAD does not store the raw callstats for the pop or sex groupings of any subset. Default is ["adj"]
     :param sample_sum_sets_and_pops: Dict with subset (keys) and list of the subset's specific populations (values). Default is None.
     :param verbose: If True, show top values of annotations being checked, including checks that pass; if False, show only top values of annotations that fail checks. Default is False.
     :param sort_order: List containing order to sort label group combinations. Default is SORT_ORDER.
     :param delimiter: String to use as delimiter when making group label combinations. Default is "-".
     :param metric_first_field: If True, metric precedes label group, e.g. AC-afr-male. If False, label group precedes metric, afr-male-AC. Default is True.
     :param metrics: List of metrics to sum and compare to annotationed versions. Default is ["AC", "AN", "nhomalt"].
@@ -587,40 +576,89 @@
     :param delimiter: String to use as delimiter when making group label combinations. Default is "-".
     :param metric_first_field: If True, metric precedes label group, e.g. AC-afr-male. If False, label group precedes metric, afr-male-AC. Default is True.
     :return: None
     """
     t = t.rows() if isinstance(t, hl.MatrixTable) else t
 
     field_check_expr = {}
+
+    for group in ["raw", "adj"]:
+        # Check AC and nhomalt missing if AN is missing and defined if AN is defined.
+        for subfield in ["AC", "nhomalt"]:
+            check_field = f"{subfield}{delimiter}{group}"
+            an_field = f"AN{delimiter}{group}"
+            field_check_expr[
+                f"{check_field} defined when AN defined and missing when AN missing"
+            ] = {
+                "expr": hl.if_else(
+                    hl.is_missing(t.info[an_field]),
+                    hl.is_defined(t.info[check_field]),
+                    hl.is_missing(t.info[check_field]),
+                ),
+                "agg_func": hl.agg.count_where,
+                "display_fields": hl.struct(
+                    **{an_field: t.info[an_field], check_field: t.info[check_field]}
+                ),
+            }
+
+        # Check AF missing if AN is missing and defined if AN is defined and > 0.
+        check_field = f"AF{delimiter}{group}"
+        an_field = f"AN{delimiter}{group}"
+        field_check_expr[
+            f"{check_field} defined when AN defined (and > 0) and missing when AN missing"
+        ] = {
+            "expr": hl.if_else(
+                hl.is_missing(t.info[an_field]),
+                hl.is_defined(t.info[check_field]),
+                (t.info[an_field] > 0) & hl.is_missing(t.info[check_field]),
+            ),
+            "agg_func": hl.agg.count_where,
+            "display_fields": hl.struct(
+                **{an_field: t.info[an_field], check_field: t.info[check_field]}
+            ),
+        }
+
+        # Check raw and adj AF missing if AN is 0.
+        check_field = f"AF{delimiter}{group}"
+        an_field = f"AN{delimiter}{group}"
+        field_check_expr[f"{check_field} missing when AN 0"] = {
+            "expr": (t.info[an_field] == 0) & hl.is_defined(t.info[check_field]),
+            "agg_func": hl.agg.count_where,
+            "display_fields": hl.struct(
+                **{an_field: t.info[an_field], check_field: t.info[check_field]}
+            ),
+        }
+
     for subfield in ["AC", "AF"]:
         # Check raw AC, AF > 0
         check_field = f"{subfield}{delimiter}raw"
-
         field_check_expr[f"{check_field} > 0"] = {
-            "expr": hl.agg.count_where(t.info[check_field] <= 0),
+            "expr": t.info[check_field] <= 0,
+            "agg_func": hl.agg.count_where,
             "display_fields": hl.struct(**{check_field: t.info[check_field]}),
         }
+
         # Check adj AC, AF > 0
         check_field = f"{subfield}{delimiter}adj"
         field_check_expr[f"{check_field} >= 0"] = {
-            "expr": hl.agg.count_where(t.info[check_field] < 0),
+            "expr": t.info[check_field] < 0,
+            "agg_func": hl.agg.count_where,
             "display_fields": hl.struct(
                 **{check_field: t.info[check_field], "filters": t.filters}
             ),
         }
 
     # Check overall gnomad's raw subfields >= adj
     for subfield in ["AC", "AN", "nhomalt"]:
         check_field_left = f"{subfield}{delimiter}raw"
         check_field_right = f"{subfield}{delimiter}adj"
 
         field_check_expr[f"{check_field_left} >= {check_field_right}"] = {
-            "expr": hl.agg.count_where(
-                t.info[check_field_left] < t.info[check_field_right]
-            ),
+            "expr": t.info[check_field_left] < t.info[check_field_right],
+            "agg_func": hl.agg.count_where,
             "display_fields": hl.struct(
                 **{
                     check_field_left: t.info[check_field_left],
                     check_field_right: t.info[check_field_right],
                 }
             ),
         }
@@ -634,17 +672,16 @@
                 if metric_first_field
                 else f"{subset}{subfield}{delimiter}"
             )
             check_field_left = f"{field_check_label}raw"
             check_field_right = f"{field_check_label}adj"
 
             field_check_expr[f"{check_field_left} >= {check_field_right}"] = {
-                "expr": hl.agg.count_where(
-                    t.info[check_field_left] < t.info[check_field_right]
-                ),
+                "expr": t.info[check_field_left] < t.info[check_field_right],
+                "agg_func": hl.agg.count_where,
                 "display_fields": hl.struct(
                     **{
                         check_field_left: t.info[check_field_left],
                         check_field_right: t.info[check_field_right],
                     }
                 ),
             }
@@ -711,17 +748,17 @@
 
     field_check_expr = {}
     for metric in xx_metrics:
         standard_field = metric.replace(f"{delimiter}XX", "")
         check_field_left = f"{metric}"
         check_field_right = f"{standard_field}"
         field_check_expr[f"{check_field_left} == {check_field_right}"] = {
-            "expr": hl.agg.count_where(
-                t_xnonpar.info[check_field_left] != t_xnonpar.info[check_field_right]
-            ),
+            "expr": t_xnonpar.info[check_field_left]
+            != t_xnonpar.info[check_field_right],
+            "agg_func": hl.agg.count_where,
             "display_fields": hl.struct(
                 **{
                     check_field_left: t_xnonpar.info[check_field_left],
                     check_field_right: t_xnonpar.info[check_field_right],
                 }
             ),
         }
@@ -916,15 +953,15 @@
     global_pprint = {g: hl.eval(t[g]) for g in t.globals}
     pprint(global_pprint, sort_dicts=False)
 
 
 def validate_release_t(
     t: Union[hl.MatrixTable, hl.Table],
     subsets: List[str] = [""],
-    pops: List[str] = POPS[CURRENT_MAJOR_RELEASE],
+    pops: List[str] = POPS[CURRENT_MAJOR_RELEASE]["exomes"],
     missingness_threshold: float = 0.5,
     site_gt_check_expr: Dict[str, hl.expr.BooleanExpression] = None,
     verbose: bool = False,
     show_percent_sites: bool = True,
     delimiter: str = "-",
     metric_first_field: bool = True,
     sum_metrics: List[str] = ["AC", "AN", "nhomalt"],
@@ -956,15 +993,15 @@
     - Checks that subgroup annotation values add up to the supergroup annotation values
     - Checks on sex-chromosome annotations; and summaries of % missingness in variant annotations
 
     All annotations must be within an info struct, e.g. t.info.AC-raw.
 
     :param t: Input MatrixTable or Table containing variant annotations to check.
     :param subsets: List of subsets to be checked.
-    :param pops: List of pops within main callset.
+    :param pops: List of pops within main callset. Default is POPS[CURRENT_MAJOR_RELEASE]["exomes"].
     :param missingness_threshold: Upper cutoff for allowed amount of missingness. Default is 0.5.
     :param site_gt_check_expr: Optional boolean expression or dictionary of strings and boolean expressions typically used to log how many monoallelic or 100% heterozygous sites are in the Table.
     :param verbose: If True, display top values of relevant annotations being checked, regardless of whether check conditions are violated; if False, display only top values of relevant annotations if check conditions are violated.
     :param show_percent_sites: Show percentage of sites that fail checks. Default is False.
     :param delimiter: String to use as delimiter when making group label combinations. Default is "-".
     :param metric_first_field: If True, metric precedes label group, e.g. AC-afr-male. If False, label group precedes metric, afr-male-AC. Default is True.
     :param sum_metrics: List of metrics to sum and compare to annotationed versions and between subsets and entire callset. Default is ["AC", "AN", "nhomalt"].
```

### Comparing `gnomad-0.7.1/gnomad/resources/config.py` & `gnomad-0.8.0/gnomad/resources/config.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/resources/grch37/gnomad.py` & `gnomad-0.8.0/gnomad/resources/grch37/gnomad.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/resources/grch37/gnomad_ld.py` & `gnomad-0.8.0/gnomad/resources/grch37/gnomad_ld.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,34 +17,30 @@
     version: Optional[str] = None,
 ):
     if version is None:
         version = (
             CURRENT_EXOME_RELEASE if data_type == "exomes" else CURRENT_GENOME_RELEASE
         )
     subdir = "sv/" if data_type == "genomes_snv_sv" else ""
-    return (
-        f'gs://gnomad-public-requester-pays/release/{version}/ld/{subdir}gnomad.{data_type}.r{version}.{pop}.{"common." if common_only else ""}{"adj." if adj else ""}ld.bm'
-    )
+    return f'gs://gnomad-public-requester-pays/release/{version}/ld/{subdir}gnomad.{data_type}.r{version}.{pop}.{"common." if common_only else ""}{"adj." if adj else ""}ld.bm'
 
 
 def _ld_index_path(
     data_type: str,
     pop: str,
     common_only: bool = True,
     adj: bool = True,
     version: Optional[str] = None,
 ):
     if version is None:
         version = (
             CURRENT_EXOME_RELEASE if data_type == "exomes" else CURRENT_GENOME_RELEASE
         )
     subdir = "sv/" if data_type == "genomes_snv_sv" else ""
-    return (
-        f'gs://gnomad-public-requester-pays/release/{version}/ld/{subdir}gnomad.{data_type}.r{version}.{pop}.{"common." if common_only else ""}{"adj." if adj else ""}ld.variant_indices.ht'
-    )
+    return f'gs://gnomad-public-requester-pays/release/{version}/ld/{subdir}gnomad.{data_type}.r{version}.{pop}.{"common." if common_only else ""}{"adj." if adj else ""}ld.variant_indices.ht'
 
 
 def _ld_snv_sv_path(pop):
     return f"gs://gnomad-public-requester-pays/release/2.1.1/ld/sv/gnomad.genomes_snv_sv.r2.1.1.{pop}.snv_sv.ld.ht"
 
 
 def _ld_snv_sv_index_path(pop, type):
@@ -58,29 +54,25 @@
     adj: bool = True,
     version: Optional[str] = None,
 ):
     if version is None:
         version = (
             CURRENT_EXOME_RELEASE if data_type == "exomes" else CURRENT_GENOME_RELEASE
         )
-    return (
-        f'gs://gnomad-public-requester-pays/release/{version}/ld/scores/gnomad.{data_type}.r{version}.{pop1}.{pop2}.{"adj." if adj else ""}ld_scores.ht'
-    )
+    return f'gs://gnomad-public-requester-pays/release/{version}/ld/scores/gnomad.{data_type}.r{version}.{pop1}.{pop2}.{"adj." if adj else ""}ld_scores.ht'
 
 
 def _ld_scores_path(
     data_type: str, pop: str, adj: bool = True, version: Optional[str] = None
 ):
     if version is None:
         version = (
             CURRENT_EXOME_RELEASE if data_type == "exomes" else CURRENT_GENOME_RELEASE
         )
-    return (
-        f'gs://gnomad-public-requester-pays/release/{version}/ld/scores/gnomad.{data_type}.r{version}.{pop}.{"adj." if adj else ""}ld_scores.ht'
-    )
+    return f'gs://gnomad-public-requester-pays/release/{version}/ld/scores/gnomad.{data_type}.r{version}.{pop}.{"adj." if adj else ""}ld_scores.ht'
 
 
 def ld_matrix(pop: str) -> GnomadPublicBlockMatrixResource:
     """Get resource for the LD matrix for the given population."""
     return GnomadPublicBlockMatrixResource(path=_ld_matrix_path("genomes", pop))
```

### Comparing `gnomad-0.7.1/gnomad/resources/grch38/gnomad.py` & `gnomad-0.8.0/gnomad/resources/grch38/gnomad.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,35 +10,40 @@
     GnomadPublicMatrixTableResource,
     GnomadPublicTableResource,
     VersionedMatrixTableResource,
     VersionedTableResource,
 )
 from gnomad.sample_qc.ancestry import POP_NAMES
 from gnomad.utils.annotations import add_gks_va, add_gks_vrs
-from gnomad.utils.vcf import FAF_POPS
 
 logging.basicConfig(
     format="%(asctime)s (%(name)s %(lineno)s): %(message)s",
     datefmt="%m/%d/%Y %I:%M:%S %p",
 )
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
-CURRENT_EXOME_RELEASE = "4.0"
-CURRENT_GENOME_RELEASE = "3.1.2"
+CURRENT_EXOME_RELEASE = "4.1"
+CURRENT_GENOME_RELEASE = "4.1"
 
 CURRENT_EXOME_COVERAGE_RELEASE = "4.0"
 CURRENT_GENOME_COVERAGE_RELEASE = "3.0.1"
 
-EXOME_RELEASES = ["4.0"]
-GENOME_RELEASES = ["3.0", "3.1", "3.1.1", "3.1.2"]
+CURRENT_EXOME_AN_RELEASE = "4.1"
+CURRENT_GENOME_AN_RELEASE = "4.1"
+
+EXOME_RELEASES = ["4.0", "4.1"]
+GENOME_RELEASES = ["3.0", "3.1", "3.1.1", "3.1.2", "4.0", "4.1"]
 
 EXOME_COVERAGE_RELEASES = ["4.0"]
 GENOME_COVERAGE_RELEASES = ["3.0", "3.0.1"]
 
+EXOME_AN_RELEASES = ["4.1"]
+GENOME_AN_RELEASES = ["4.1"]
+
 DATA_TYPES = ["exomes", "genomes"]
 MAJOR_RELEASES = ["v3", "v4"]
 CURRENT_MAJOR_RELEASE = MAJOR_RELEASES[-1]
 
 
 GENOME_POPS = ["AFR", "AMI", "AMR", "ASJ", "EAS", "FIN", "NFE", "SAS", "OTH"]
 SUBSETS = {
@@ -70,26 +75,53 @@
 """
 Sample sexes used in VCF export.
 
 Used to stratify frequency annotations (AC, AN, AF) for each sex.
 """
 
 POPS = {
-    "v3": ["afr", "ami", "amr", "asj", "eas", "fin", "nfe", "oth", "sas", "mid"],
-    "v4": [
-        "afr",
-        "amr",
-        "asj",
-        "eas",
-        "fin",
-        "mid",
-        "nfe",
-        "remaining",
-        "sas",
-    ],
+    "v3": {
+        "genomes": [
+            "afr",
+            "ami",
+            "amr",
+            "asj",
+            "eas",
+            "fin",
+            "nfe",
+            "oth",
+            "sas",
+            "mid",
+        ]
+    },
+    "v4": {
+        "exomes": [
+            "afr",
+            "amr",
+            "asj",
+            "eas",
+            "fin",
+            "mid",
+            "nfe",
+            "remaining",
+            "sas",
+        ],
+        "genomes": [
+            "afr",
+            "ami",
+            "amr",
+            "asj",
+            "eas",
+            "fin",
+            "mid",
+            "nfe",
+            "remaining",
+            "sas",
+        ],
+    },
 }
 """
 Global ancestry groups in gnomAD by version.
 """
 
 COHORTS_WITH_POP_STORED_AS_SUBPOP = ["tgp", "hgdp"]
 """
@@ -217,15 +249,18 @@
     "itu": "Indian Telugu",
 }
 """
 1000 Genomes Project (1KG/TGP) pop label map.
 """
 
 POPS_STORED_AS_SUBPOPS = TGP_POPS + HGDP_POPS
-POPS_TO_REMOVE_FOR_POPMAX = {"asj", "fin", "oth", "ami", "mid", "remaining"}
+POPS_TO_REMOVE_FOR_POPMAX = {
+    "v3": {"asj", "fin", "mid", "oth", "ami", "remaining"},
+    "v4": {"asj", "fin", "oth", "ami", "remaining"},
+}
 """
 Populations that are removed before popmax calculations.
 """
 
 DOWNSAMPLINGS = {
     "v3": [
         10,
@@ -301,24 +336,33 @@
     :param version: One of the release versions of gnomAD on GRCh38
     :return: Path to release Table
     """
     version_prefix = "r" if version.startswith("3.0") else "v"
     return f"gs://gnomad-public-requester-pays/release/{version}/ht/{data_type}/gnomad.{data_type}.{version_prefix}{version}.sites.ht"
 
 
-def _public_coverage_ht_path(data_type: str, version: str) -> str:
+def _public_coverage_ht_path(
+    data_type: str, version: str, coverage_type="coverage"
+) -> str:
     """
     Get public coverage hail table.
 
     :param data_type: One of "exomes" or "genomes"
     :param version: One of the release versions of gnomAD on GRCh38
+    :param coverage_type: One of "coverage" or "allele_number"
     :return: path to coverage Table
     """
+    if coverage_type not in ["coverage", "allele_number"]:
+        raise ValueError(
+            "coverage_type must be one of 'coverage' or 'allele_number', not"
+            f" {coverage_type}!"
+        )
+
     version_prefix = "r" if version.startswith("3.0") else "v"
-    return f"gs://gnomad-public-requester-pays/release/{version}/coverage/{data_type}/gnomad.{data_type}.{version_prefix}{version}.coverage.ht"
+    return f"gs://gnomad-public-requester-pays/release/{version}/coverage/{data_type}/gnomad.{data_type}.{version_prefix}{version}.{coverage_type}.ht"
 
 
 def public_release(data_type: str) -> VersionedTableResource:
     """
     Retrieve publicly released versioned table resource.
 
     :param data_type: One of "exomes" or "genomes"
@@ -375,14 +419,45 @@
                 path=_public_coverage_ht_path(data_type, release)
             )
             for release in releases
         },
     )
 
 
+def all_sites_an(data_type: str) -> VersionedTableResource:
+    """
+    Retrieve gnomAD's all sites allele number table by data_type.
+
+    :param data_type: One of "exomes" or "genomes"
+    :return: All sites allele number VersionedTableResource
+    """
+    if data_type not in DATA_TYPES:
+        raise DataException(
+            f"{data_type} not in {DATA_TYPES}, please select a data type from"
+            f" {DATA_TYPES}"
+        )
+
+    if data_type == "exomes":
+        current_release = CURRENT_EXOME_AN_RELEASE
+        releases = EXOME_AN_RELEASES
+    else:
+        current_release = CURRENT_GENOME_AN_RELEASE
+        releases = GENOME_AN_RELEASES
+
+    return VersionedTableResource(
+        current_release,
+        {
+            release: GnomadPublicTableResource(
+                path=_public_coverage_ht_path(data_type, release, "allele_number")
+            )
+            for release in releases
+        },
+    )
+
+
 def coverage_tsv_path(data_type: str, version: Optional[str] = None) -> str:
     """
     Retrieve gnomAD's coverage table by data_type.
 
     :param data_type: One of "exomes" or "genomes"
     :return: Coverage Table
     """
@@ -426,14 +501,40 @@
         )
 
     contig = f".{contig}" if contig else ""
     version_prefix = "r" if version.startswith("3.0") else "v"
     return f"gs://gcp-public-data--gnomad/release/{version}/vcf/{data_type}/gnomad.{data_type}.{version_prefix}{version}.sites{contig}.vcf.bgz"
 
 
+def add_grpMaxFAF95_v4(ht: hl.Table) -> hl.Table:
+    """
+    Add a grpMaxFAF95 struct with 'popmax' and 'popmax_population'.
+
+    Also includes a jointGrpMaxFAF95 annotation using the v4 fafmax and joint_fafmax structures.
+
+    :param ht: Input hail table.
+    :return: Annotated hail table.
+    """
+    if "gnomad" in ht.fafmax:
+        fafmax_field = ht.fafmax.gnomad
+    else:
+        fafmax_field = ht.fafmax
+    ht = ht.annotate(
+        grpMaxFAF95=hl.struct(
+            popmax=fafmax_field.faf95_max,
+            popmax_population=fafmax_field.faf95_max_gen_anc,
+        ),
+        jointGrpMaxFAF95=hl.struct(
+            popmax=ht.joint_fafmax.faf95_max,
+            popmax_population=ht.joint_fafmax.faf95_max_gen_anc,
+        ),
+    )
+    return ht
+
+
 def gnomad_gks(
     locus_interval: hl.IntervalExpression,
     version: str,
     data_type: str = "genomes",
     by_ancestry_group: bool = False,
     by_sex: bool = False,
     vrs_only: bool = False,
@@ -457,105 +558,110 @@
     :param skip_checkpoint: Bool to pass to skip checkpointing selected fields
         (checkpointing may be desirable for large datasets by reducing data copies across the cluster).
     :param skip_coverage: Bool to pass to skip adding coverage statistics.
     :param custom_coverage_ht: Custom table to use for coverage statistics instead of the release coverage table.
     :return: List of dictionaries containing VRS information
         (and freq info split by ancestry groups and sex if desired) for specified variant.
     """
-    # Read public_release table if no custom table provided
+    # Obtain the high level version number and verify that it is 4.
+    high_level_version = f"v{version.split('.')[0]}"
+    if high_level_version != "v4":
+        raise NotImplementedError(
+            "gnomad_gks() is currently only implemented for gnomAD v4."
+        )
+
+    # Read public_release table if no custom table provided.
     if custom_ht:
         ht = custom_ht
     else:
         ht = hl.read_table(public_release(data_type).versions[version].path)
 
-    high_level_version = f"v{version.split('.')[0]}"
-
-    # Read coverage statistics if requested
-    if high_level_version == "v3":
-        coverage_version = "3.0.1"
+    # Read coverage statistics if requested.
+    coverage_version_3_0_1 = "3.0.1"  # v4 genomes coverage
+    coverage_version_4_0 = "4.0"  # v4 exomes coverage
+
+    # In v4, exomes have coverage in v4 coverage table,
+    #   genomes have coverage in v3 coverage table.
+    if data_type == "genomes":
+        coverage_version = coverage_version_3_0_1
     else:
-        raise NotImplementedError(
-            "gnomad_gks() is currently only implemented for gnomAD v3."
-        )
+        coverage_version = coverage_version_4_0
 
     coverage_ht = None
 
     if not skip_coverage:
         if custom_coverage_ht:
             coverage_ht = custom_coverage_ht
         else:
             coverage_ht = hl.read_table(
-                coverage("genomes").versions[coverage_version].path
+                coverage(data_type).versions[coverage_version].path
             )
         ht = ht.annotate(mean_depth=coverage_ht[ht.locus].mean)
+        ht = ht.annotate(fraction_cov_over_20=coverage_ht[ht.locus].over_20)
 
     # Retrieve ancestry groups from the imported POPS dictionary.
-    pops_list = list(POPS[high_level_version]) if by_ancestry_group else None
+    pops_list = list(POPS[high_level_version][data_type]) if by_ancestry_group else None
 
     # Throw warnings if contradictory arguments are passed.
     if by_ancestry_group and vrs_only:
         logger.warning(
             "Both 'vrs_only' and 'by_ancestry_groups' have been specified. Ignoring"
             " 'by_ancestry_groups' list and returning only VRS information."
         )
     elif by_sex and not by_ancestry_group:
         logger.warning(
             "Splitting whole database by sex is not yet supported. If using 'by_sex',"
             " please also specify 'by_ancestry_group' to stratify by."
         )
 
-    # Call and return add_gks_vrs and add_gks_va for chosen arguments.
-
     # Select relevant fields, checkpoint, and filter to interval before adding
-    # annotations
-    ht = ht.annotate(
-        faf95=hl.rbind(
-            hl.sorted(
-                hl.array(
-                    [
-                        hl.struct(
-                            faf=ht.faf[ht.faf_index_dict[f"{pop}-adj"]].faf95,
-                            population=pop,
-                        )
-                        for pop in FAF_POPS
-                    ]
-                ),
-                key=lambda f: (-f.faf, f.population),
-            ),
-            lambda fafs: hl.if_else(
-                hl.len(fafs) > 0,
-                hl.struct(
-                    popmax=fafs[0].faf,
-                    popmax_population=hl.if_else(
-                        fafs[0].faf == 0, hl.missing(hl.tstr), fafs[0].population
-                    ),
-                ),
-                hl.struct(
-                    popmax=hl.missing(hl.tfloat), popmax_population=hl.missing(hl.tstr)
-                ),
-            ),
-        )
-    )
+    # annotations.
 
-    keep_fields = [ht.freq, ht.info.vrs, ht.faf95]
+    # Pull up LCR flag and make referrable in the same field.
+    ht = ht.annotate(lcr=ht.region_flags.lcr)
+
+    # Pull up allele balance histogram arrays.
+    ht = ht.annotate(ab_hist_alt=ht.histograms.qual_hists.ab_hist_alt)
+
+    ht = add_grpMaxFAF95_v4(ht)
+
+    ht = ht.annotate(in_autosome_or_par=ht.locus.in_autosome_or_par())
+
+    keep_fields = [
+        ht.freq,
+        ht.info.vrs,
+        ht.info.monoallelic,
+        ht.grpMaxFAF95,
+        ht.filters,
+        ht.lcr,
+        ht.ab_hist_alt,
+        ht.in_autosome_or_par,
+    ]
 
     if not skip_coverage:
         keep_fields.append(ht.mean_depth)
+        keep_fields.append(ht.fraction_cov_over_20)
+
+    if "jointGrpMaxFAF95" in ht.row:
+        keep_fields.append(ht.jointGrpMaxFAF95)
 
     ht = ht.select(*keep_fields)
 
     # Checkpoint narrower set of columns if not skipped.
     ht = hl.filter_intervals(ht, [locus_interval])
     if not skip_checkpoint:
         ht = ht.checkpoint(hl.utils.new_temp_file("vrs_checkpoint", extension="ht"))
 
     # Collect all variants as structs, so all dictionary construction can be
-    # done in native Python
+    # done in native Python.
     variant_list = ht.collect()
     ht_freq_index_dict = ht.freq_index_dict.collect()[0]
+    # gnomad v4 renamed freq_index_dict keys to use underscores instead of dashes.
+    # Use underscores for v3 as well.
+    ht_freq_index_dict = {k.replace("-", "_"): v for k, v in ht_freq_index_dict.items()}
 
     # Assemble output dicts with VRS and optionally frequency, append to list,
     # then return list
     outputs = []
     for variant in variant_list:
         vrs_variant = add_gks_vrs(variant.locus, variant.vrs)
```

### Comparing `gnomad-0.7.1/gnomad/resources/grch38/reference_data.py` & `gnomad-0.8.0/gnomad/resources/grch38/reference_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from gnomad.resources.resource_utils import (
     DBSNP_B154_CHR_CONTIG_RECODING,
     NO_CHR_TO_CHR_CONTIG_RECODING,
     GnomadPublicMatrixTableResource,
     GnomadPublicTableResource,
     VersionedMatrixTableResource,
     VersionedTableResource,
+    import_gencode,
     import_sites_vcf,
 )
 from gnomad.utils.vep import vep_or_lookup_vep
 
 
 def _import_purcell_5k(path) -> hl.Table:
     p5k = hl.import_locus_intervals(path, reference_genome="GRCh37")
@@ -379,7 +380,24 @@
         .select(hapmap=True)
         .join(kgp_omni.ht().select(omni=True), how="outer")
         .join(kgp.versions["phase_1_hc"].ht().select(kgp_phase1_hc=True), how="outer")
         .join(mills.ht().select(mills=True), how="outer")
         .repartition(200, shuffle=False)
         .persist()
     )
+
+
+gencode = VersionedTableResource(
+    default_version="v39",
+    versions={
+        "v39": GnomadPublicTableResource(
+            path="gs://gnomad-public-requester-pays/resources/grch38/gencode/gencode.v39.annotation.ht",
+            import_func=import_gencode,
+            import_args={
+                "gtf_path": "gs://gcp-public-data--gnomad/resources/grch38/gencode/gencode.v39.annotation.gtf.gz",
+                "reference_genome": "GRCh38",
+                "force_bgz": True,
+                "min_partitions": 100,
+            },
+        ),
+    },
+)
```

### Comparing `gnomad-0.7.1/gnomad/resources/import_resources.py` & `gnomad-0.8.0/gnomad/resources/import_resources.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/resources/resource_utils.py` & `gnomad-0.8.0/gnomad/resources/resource_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,24 +105,31 @@
     :param path: The Table path (typically ending in .ht)
     :param import_args: Any sources that are required for the import and need to be kept track of and/or passed to the import_func (e.g. .vcf path for an imported VCF)
     :param import_func: A function used to import the Table. `import_func` will be passed the `import_args` dictionary as kwargs.
     """
 
     expected_file_extensions: List[str] = [".ht"]
 
-    def ht(self, force_import: bool = False) -> hl.Table:
+    def ht(
+        self,
+        force_import: bool = False,
+        read_args: Optional[Dict[str, Any]] = None,
+    ) -> hl.Table:
         """
         Read and return the Hail Table resource.
 
+        :param force_import: If ``True``, force the import of the resource even if it
+            already exists.
+        :param read_args: Any additional arguments to pass to hl.read_table.
         :return: Hail Table resource
         """
         if self.path is None or force_import:
             return self.import_func(**self.import_args)
         else:
-            return hl.read_table(self.path)
+            return hl.read_table(self.path, **(read_args or {}))
 
     def import_resource(self, overwrite: bool = True, **kwargs) -> None:
         """
         Import the TableResource using its import_func and writes it in its path.
 
         :param overwrite: If ``True``, overwrite an existing file at the destination.
         :param kwargs: Any other parameters to be passed to hl.Table.write
@@ -140,24 +147,31 @@
     :param path: The MatrixTable path (typically ending in .mt)
     :param import_args: Any sources that are required for the import and need to be kept track of and/or passed to the import_func (e.g. .vcf path for an imported VCF)
     :param import_func: A function used to import the MatrixTable. `import_func` will be passed the `import_args` dictionary as kwargs.
     """
 
     expected_file_extensions: List[str] = [".mt"]
 
-    def mt(self, force_import: bool = False) -> hl.MatrixTable:
+    def mt(
+        self,
+        force_import: bool = False,
+        read_args: Optional[Dict[str, Any]] = None,
+    ) -> hl.MatrixTable:
         """
         Read and return the Hail MatrixTable resource.
 
+        :param force_import: If ``True``, force the import of the resource even if it
+            already exists.
+        :param read_args: Any additional arguments to pass to hl.read_matrix_table.
         :return: Hail MatrixTable resource
         """
         if self.path is None or force_import:
             return self.import_func(**self.import_args)
         else:
-            return hl.read_matrix_table(self.path)
+            return hl.read_matrix_table(self.path, **(read_args or {}))
 
     def import_resource(self, overwrite: bool = True, **kwargs) -> None:
         """
         Import the MatrixTable resource using its import_func and writes it in its path.
 
         :param overwrite: If set, existing file(s) will be overwritten
         :param kwargs: Any other parameters to be passed to hl.MatrixTable.write
@@ -175,24 +189,31 @@
     :param path: The VariantDataset path (typically ending in .vds)
     :param import_args: Any sources that are required for the import and need to be kept track of and/or passed to the import_func (e.g. .vcf path for an imported VCF)
     :param import_func: A function used to import the VariantDataset. `import_func` will be passed the `import_args` dictionary as kwargs.
     """
 
     expected_file_extensions: List[str] = [".vds"]
 
-    def vds(self, force_import: bool = False) -> hl.vds.VariantDataset:
+    def vds(
+        self,
+        force_import: bool = False,
+        read_args: Optional[Dict[str, Any]] = None,
+    ) -> hl.vds.VariantDataset:
         """
         Read and return the Hail VariantDataset resource.
 
+        :param force_import: If ``True``, force the import of the resource even if it
+            already exists.
+        :param read_args: Any additional arguments to pass to hl.vds.read_vds.
         :return: Hail VariantDataset resource
         """
         if self.path is None or force_import:
             return self.import_func(**self.import_args)
         else:
-            return hl.vds.read_vds(self.path)
+            return hl.vds.read_vds(self.path, **(read_args or {}))
 
     def import_resource(self, overwrite: bool = True, **kwargs) -> None:
         """
         Import the VariantDataset resource using its import_func and writes it in its path.
 
         :param overwrite: If set, existing file(s) will be overwritten
         :param kwargs: Any other parameters to be passed to hl.vds.VariantDataset.write
@@ -279,21 +300,22 @@
     :param path: The BlockMatrix path (typically ending in .bm)
     :param import_args: Any sources that are required for the import and need to be kept track of and/or passed to the import_func.
     :param import_func: A function used to import the BlockMatrix. `import_func` will be passed the `import_args` dictionary as kwargs.
     """
 
     expected_file_extensions: List[str] = [".bm"]
 
-    def bm(self) -> BlockMatrix:
+    def bm(self, read_args: Optional[Dict[str, Any]] = None) -> BlockMatrix:
         """
         Read and return the Hail MatrixTable resource.
 
+        :param read_args: Any additional arguments to pass to BlockMatrix.read.
         :return: Hail MatrixTable resource
         """
-        return BlockMatrix.read(self.path)
+        return BlockMatrix.read(self.path, **(read_args or {}))
 
     def import_resource(self, overwrite: bool = True, **kwargs) -> None:
         """
         Import the BlockMatrixResource using its import_func and writes it in its path.
 
         :param overwrite: If ``True``, overwrite an existing file at the destination.
         :param kwargs: Any additional parameters to be passed to BlockMatrix.write
@@ -314,24 +336,31 @@
         VCF).
     :param import_func: A function used to import the Expression. `import_func` will be
         passed the `import_args` dictionary as kwargs.
     """
 
     expected_file_extensions: List[str] = [".he"]
 
-    def he(self, force_import: bool = False) -> hl.expr.Expression:
+    def he(
+        self,
+        force_import: bool = False,
+        read_args: Optional[Dict[str, Any]] = None,
+    ) -> hl.expr.Expression:
         """
         Read and return the Hail Expression resource.
 
+        :param force_import: If ``True``, force the import of the resource even if it
+            already exists.
+        :param read_args: Any additional arguments to pass to hl.experimental.read_expression.
         :return: Hail Expression resource.
         """
         if self.path is None or force_import:
             return self.import_func(**self.import_args)
         else:
-            return hl.experimental.read_expression(self.path)
+            return hl.experimental.read_expression(self.path, **(read_args or {}))
 
     def import_resource(self, overwrite: bool = True, **kwargs) -> None:
         """
         Import the Expression resource using its import_func and writes it in its path.
 
         :param overwrite: If set, existing file(s) will be overwritten.
         :param kwargs: Any other parameters to be passed to hl.experimental.
@@ -683,7 +712,25 @@
     "NC_000024.10": "chrY",
 }
 
 
 def import_sites_vcf(**kwargs) -> hl.Table:
     """Import site-level data from a VCF into a Hail Table."""
     return hl.import_vcf(**kwargs).rows()
+
+
+def import_gencode(gtf_path: str, **kwargs) -> hl.Table:
+    """
+    Import GENCODE annotations GTF file as a Hail Table.
+
+    :param gtf_path: Path to GENCODE GTF file.
+    :return: Table with GENCODE annotation information.
+    """
+    ht = hl.experimental.import_gtf(gtf_path, **kwargs)
+
+    # Only get gene and transcript stable IDs (without version numbers if they
+    # exist), early versions of GENCODE have no version numbers but later ones do.
+    ht = ht.annotate(
+        gene_id=ht.gene_id.split("\\.")[0],
+        transcript_id=ht.transcript_id.split("\\.")[0],
+    )
+    return ht
```

### Comparing `gnomad-0.7.1/gnomad/sample_qc/ancestry.py` & `gnomad-0.8.0/gnomad/sample_qc/ancestry.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,25 @@
 logging.basicConfig(format="%(levelname)s (%(name)s %(lineno)s): %(message)s")
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 POP_NAMES = {
     "afr": "African/African-American",
     "ami": "Amish",
-    "amr": "Latino",
+    "amr": "Admixed American",
     "asj": "Ashkenazi Jewish",
     "eas": "East Asian",
     "eur": "European",
     "fin": "Finnish",
     # NOTE: mde is kept for historical purposes, in gnomAD v3.1 mid was used instead
     "mde": "Middle Eastern",
     "mid": "Middle Eastern",
     "nfe": "Non-Finnish European",
     "oth": "Other",
+    "remaining": "Remaining individuals",
     "sas": "South Asian",
     "uniform": "Uniform",
     "sas_non_consang": "South Asian (F < 0.05)",
     "consanguineous": "South Asian (F > 0.05)",
     "exac": "ExAC",
     "bgr": "Bulgarian (Eastern European)",
     "est": "Estonian",
@@ -77,14 +78,15 @@
     "kor": "#4891D9",
     "sgp": "darkred",
     "jpn": "#BC002D",
     "oea": "#108C44",
     "oeu": "#6AA5CD",
     "onf": "#6AA5CD",
     "unk": "#ABB9B9",
+    "remaining": "#ABB9B9",
     "": "#ABB9B9",
 }
 
 
 def pc_project(
     mt: hl.MatrixTable,
     loadings_ht: hl.Table,
```

### Comparing `gnomad-0.7.1/gnomad/sample_qc/filtering.py` & `gnomad-0.8.0/gnomad/sample_qc/filtering.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,16 @@
         )
 
     metrics_stats_expr = ht.qc_metrics_stats[ht._strata]
     select_expr.update(
         **{
             f"fail_{metric}": (
                 ht._qc_metrics[metric] <= metrics_stats_expr[metric].lower
-            ) | (ht._qc_metrics[metric] >= metrics_stats_expr[metric].upper)
+            )
+            | (ht._qc_metrics[metric] >= metrics_stats_expr[metric].upper)
             for metric in qc_metrics
         }
     )
     ht = ht.select(**select_expr)
 
     stratified_filters = hl.set(
         hl.filter(
```

### Comparing `gnomad-0.7.1/gnomad/sample_qc/pipeline.py` & `gnomad-0.8.0/gnomad/sample_qc/pipeline.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/sample_qc/platform.py` & `gnomad-0.8.0/gnomad/sample_qc/platform.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/sample_qc/relatedness.py` & `gnomad-0.8.0/gnomad/sample_qc/relatedness.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
     :param i_col: Column containing the 1st sample of the pair in the relationship table
     :param j_col: Column containing the 2nd sample of the pair in the relationship table
     :param relationship_col: Column contatining the relationship for the sample pair as defined in this module constants.
     :return: Pedigree of complete trios
     """
 
     def group_parent_child_pairs_by_fam(
-        parent_child_pairs: Iterable[Tuple[str, str]]
+        parent_child_pairs: Iterable[Tuple[str, str]],
     ) -> List[List[Tuple[str, str]]]:
         """
         Group parent-child pairs into a list of families.
 
         A family here is defined as a list of sample-pairs which all share at least one sample with at least one other
         sample-pair in the list.
```

### Comparing `gnomad-0.7.1/gnomad/sample_qc/sex.py` & `gnomad-0.8.0/gnomad/sample_qc/sex.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import List, Optional, Tuple, Union
 
 import hail as hl
 import numpy as np
 import pandas as pd
 from sklearn.mixture import GaussianMixture
 
+from gnomad.utils.annotations import annotate_and_index_source_mt_for_sex_ploidy
+
 logging.basicConfig(format="%(levelname)s (%(name)s %(lineno)s): %(message)s")
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 SEXES = {"Male": "Male", "Female": "Female"}
 
 
@@ -19,33 +21,43 @@
     locus_expr: hl.expr.LocusExpression,
     gt_expr: hl.expr.CallExpression,
     karyotype_expr: hl.expr.StringExpression,
     xy_karyotype_str: str = "XY",
     xx_karyotype_str: str = "XX",
 ) -> hl.expr.CallExpression:
     """
-    Create an entry expression to convert males to haploid on non-PAR X/Y and females to missing on Y.
+    Create an entry expression to convert XY to haploid on non-PAR X/Y and XX to missing on Y.
 
-    :param locus_expr: Locus
-    :param gt_expr: Genotype
-    :param karyotype_expr: Karyotype
-    :param xy_karyotype_str: Male sex karyotype representation
-    :param xx_karyotype_str: Female sex karyotype representation
-    :return: Genotype adjusted for sex ploidy
+    :param locus_expr: Locus expression.
+    :param gt_expr: Genotype expression.
+    :param karyotype_expr: Sex karyotype expression.
+    :param xy_karyotype_str: String representing XY karyotype. Default is "XY".
+    :param xx_karyotype_str: String representing XX karyotype. Default is "XX".
+    :return: Genotype adjusted for sex ploidy.
     """
-    male = karyotype_expr == xy_karyotype_str
-    female = karyotype_expr == xx_karyotype_str
-    x_nonpar = locus_expr.in_x_nonpar()
-    y_par = locus_expr.in_y_par()
-    y_nonpar = locus_expr.in_y_nonpar()
+    # An optimization that annotates the locus's source matrix table with the
+    # fields in the case statements below, so they are not re-computed for every entry.
+    col_idx, row_idx = annotate_and_index_source_mt_for_sex_ploidy(
+        locus_expr, karyotype_expr, xy_karyotype_str, xx_karyotype_str
+    )
+
     return (
         hl.case(missing_false=True)
-        .when(female & (y_par | y_nonpar), hl.null(hl.tcall))
-        .when(male & (x_nonpar | y_nonpar) & gt_expr.is_het(), hl.null(hl.tcall))
-        .when(male & (x_nonpar | y_nonpar), hl.call(gt_expr[0], phased=False))
+        # Added to reduce the checks by entry.
+        .when(row_idx.in_autosome, gt_expr)
+        .when((row_idx.y_par | row_idx.y_nonpar) & col_idx.xx, hl.missing(hl.tcall))
+        .when(~row_idx.in_non_par, gt_expr)
+        .when(
+            (row_idx.x_nonpar | row_idx.y_nonpar) & col_idx.xy & gt_expr.is_het(),
+            hl.missing(hl.tcall),
+        )
+        .when(
+            (row_idx.x_nonpar | row_idx.y_nonpar) & col_idx.xy,
+            hl.call(gt_expr[0], phased=False),
+        )
         .default(gt_expr)
     )
 
 
 def adjust_sex_ploidy(
     mt: hl.MatrixTable,
     sex_expr: hl.expr.StringExpression,
```

### Comparing `gnomad-0.7.1/gnomad/utils/annotations.py` & `gnomad-0.8.0/gnomad/utils/annotations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 # noqa: D100
 
-import csv
 import itertools
-import json
 import logging
-from timeit import default_timer as timer
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
 import hail as hl
-from hail.utils.misc import new_temp_file
 
 import gnomad.utils.filtering as filter_utils
 from gnomad.utils.gen_stats import to_phred
 
 logging.basicConfig(
     format="%(asctime)s (%(name)s %(lineno)s): %(message)s",
     datefmt="%m/%d/%Y %I:%M:%S %p",
@@ -598,14 +594,177 @@
         .when((AF >= 0.2) & (AF < 0.5), "binned_0.5")
         .when((AF >= 0.5) & (AF <= 1), "binned_1")
         .default(hl.null(hl.tstr))
     )
     return bin_expr
 
 
+def annotate_and_index_source_mt_for_sex_ploidy(
+    locus_expr: hl.expr.LocusExpression,
+    karyotype_expr: hl.expr.StringExpression,
+    xy_karyotype_str: str = "XY",
+    xx_karyotype_str: str = "XX",
+) -> Tuple[hl.expr.StructExpression, hl.expr.StructExpression]:
+    """
+    Prepare relevant ploidy annotations for downstream calculations on a matrix table.
+
+    This method is used as an optimization for the `get_is_haploid_expr` and
+    `adjusted_sex_ploidy_expr` methods.
+
+    This method annotates the `locus_expr` source matrix table with the following
+    fields:
+
+        - `xy`: Boolean indicating if the sample is XY.
+        - `xx`: Boolean indicating if the sample is XX.
+        - `in_non_par`: Boolean indicating if the locus is in a non-PAR region.
+        - `x_nonpar`: Boolean indicating if the locus is in a non-PAR region of the X
+          chromosome.
+        - `y_par`: Boolean indicating if the locus is in a PAR region of the Y
+          chromosome.
+        - `y_nonpar`: Boolean indicating if the locus is in a non-PAR region of the Y
+          chromosome.
+
+    :param locus_expr: Locus expression.
+    :param karyotype_expr: Karyotype expression.
+    :param xy_karyotype_str: String representing XY karyotype. Default is "XY".
+    :param xx_karyotype_str: String representing XX karyotype. Default is "XX".
+    :return: Tuple of index expressions for columns and rows.
+    """
+    source_mt = locus_expr._indices.source
+    col_ht = source_mt.annotate_cols(
+        xy=karyotype_expr.upper() == xy_karyotype_str,
+        xx=karyotype_expr.upper() == xx_karyotype_str,
+    ).cols()
+    row_ht = source_mt.annotate_rows(
+        in_non_par=~locus_expr.in_autosome_or_par(),
+        in_autosome=locus_expr.in_autosome(),
+        x_nonpar=locus_expr.in_x_nonpar(),
+        y_par=locus_expr.in_y_par(),
+        y_nonpar=locus_expr.in_y_nonpar(),
+    ).rows()
+    col_idx = col_ht[source_mt.col_key]
+    row_idx = row_ht[source_mt.row_key]
+
+    return col_idx, row_idx
+
+
+def get_is_haploid_expr(
+    gt_expr: Optional[hl.expr.CallExpression] = None,
+    locus_expr: Optional[hl.expr.LocusExpression] = None,
+    karyotype_expr: Optional[hl.expr.StringExpression] = None,
+    xy_karyotype_str: str = "XY",
+    xx_karyotype_str: str = "XX",
+) -> hl.expr.BooleanExpression:
+    """
+    Determine if a genotype or locus and karyotype combination is haploid.
+
+    .. note::
+
+        One of `gt_expr` or `locus_expr` and `karyotype_expr` is required.
+
+    :param gt_expr: Optional genotype expression.
+    :param locus_expr: Optional locus expression.
+    :param karyotype_expr: Optional sex karyotype expression.
+    :param xy_karyotype_str: String representing XY karyotype. Default is "XY".
+    :param xx_karyotype_str: String representing XX karyotype. Default is "XX".
+    :return: Boolean expression indicating if the genotype is haploid.
+    """
+    if gt_expr is None and locus_expr is None and karyotype_expr is None:
+        raise ValueError(
+            "One of 'gt_expr' or 'locus_expr' and 'karyotype_expr' is required."
+        )
+
+    if gt_expr is not None:
+        return gt_expr.is_haploid()
+
+    if locus_expr is None or karyotype_expr is None:
+        raise ValueError(
+            "Both 'locus_expr' and 'karyotype_expr' are required if no 'gt_expr' is "
+            "supplied."
+        )
+    # An optimization that annotates the locus's matrix table with the
+    # fields in the case statements below as an optimization step
+    col_idx, row_idx = annotate_and_index_source_mt_for_sex_ploidy(
+        locus_expr, karyotype_expr, xy_karyotype_str, xx_karyotype_str
+    )
+
+    return row_idx.in_non_par & hl.or_missing(
+        ~(col_idx.xx & (row_idx.y_par | row_idx.y_nonpar)),
+        col_idx.xy & (row_idx.x_nonpar | row_idx.y_nonpar),
+    )
+
+
+def get_gq_dp_adj_expr(
+    gq_expr: Union[hl.expr.Int32Expression, hl.expr.Int64Expression],
+    dp_expr: Union[hl.expr.Int32Expression, hl.expr.Int64Expression],
+    gt_expr: Optional[hl.expr.CallExpression] = None,
+    locus_expr: Optional[hl.expr.LocusExpression] = None,
+    karyotype_expr: Optional[hl.expr.StringExpression] = None,
+    adj_gq: int = 20,
+    adj_dp: int = 10,
+    haploid_adj_dp: int = 5,
+) -> hl.expr.BooleanExpression:
+    """
+    Get adj annotation using only GQ and DP.
+
+    Default thresholds correspond to gnomAD values.
+
+    .. note::
+
+        This function can be used to annotate adj taking into account only GQ and DP.
+        It is useful for cases where the GT field is not available, such as in the
+        reference data of a VariantDataset.
+
+    .. note::
+
+        One of `gt_expr` or `locus_expr` and `karyotype_expr` is required.
+
+    :param gq_expr: GQ expression.
+    :param dp_expr: DP expression.
+    :param gt_expr: Optional genotype expression.
+    :param locus_expr: Optional locus expression.
+    :param karyotype_expr: Optional sex karyotype expression.
+    :param adj_gq: GQ threshold for adj. Default is 20.
+    :param adj_dp: DP threshold for adj. Default is 10.
+    :param haploid_adj_dp: Haploid DP threshold for adj. Default is 5.
+    :return: Boolean expression indicating adj filter.
+    """
+    return (gq_expr >= adj_gq) & hl.if_else(
+        get_is_haploid_expr(gt_expr, locus_expr, karyotype_expr),
+        dp_expr >= haploid_adj_dp,
+        dp_expr >= adj_dp,
+    )
+
+
+def get_het_ab_adj_expr(
+    gt_expr: hl.expr.CallExpression,
+    dp_expr: Union[hl.expr.Int32Expression, hl.expr.Int64Expression],
+    ad_expr: hl.expr.ArrayNumericExpression,
+    adj_ab: float = 0.2,
+) -> hl.expr.BooleanExpression:
+    """
+    Get adj het AB annotation.
+
+    :param gt_expr: Genotype expression.
+    :param dp_expr: DP expression.
+    :param ad_expr: AD expression.
+    :param adj_ab: AB threshold for adj. Default is 0.2.
+    :return: Boolean expression indicating adj het AB filter.
+    """
+    return (
+        hl.case()
+        .when(~gt_expr.is_het(), True)
+        .when(gt_expr.is_het_ref(), ad_expr[gt_expr[1]] / dp_expr >= adj_ab)
+        .default(
+            (ad_expr[gt_expr[0]] / dp_expr >= adj_ab)
+            & (ad_expr[gt_expr[1]] / dp_expr >= adj_ab)
+        )
+    )
+
+
 def get_adj_expr(
     gt_expr: hl.expr.CallExpression,
     gq_expr: Union[hl.expr.Int32Expression, hl.expr.Int64Expression],
     dp_expr: Union[hl.expr.Int32Expression, hl.expr.Int64Expression],
     ad_expr: hl.expr.ArrayNumericExpression,
     adj_gq: int = 20,
     adj_dp: int = 10,
@@ -613,27 +772,22 @@
     haploid_adj_dp: int = 5,
 ) -> hl.expr.BooleanExpression:
     """
     Get adj genotype annotation.
 
     Defaults correspond to gnomAD values.
     """
-    return (
-        (gq_expr >= adj_gq)
-        & hl.if_else(gt_expr.is_haploid(), dp_expr >= haploid_adj_dp, dp_expr >= adj_dp)
-        & (
-            hl.case()
-            .when(~gt_expr.is_het(), True)
-            .when(gt_expr.is_het_ref(), ad_expr[gt_expr[1]] / dp_expr >= adj_ab)
-            .default(
-                (ad_expr[gt_expr[0]] / dp_expr >= adj_ab)
-                & (ad_expr[gt_expr[1]] / dp_expr >= adj_ab)
-            )
-        )
-    )
+    return get_gq_dp_adj_expr(
+        gq_expr,
+        dp_expr,
+        gt_expr=gt_expr,
+        adj_gq=adj_gq,
+        adj_dp=adj_dp,
+        haploid_adj_dp=haploid_adj_dp,
+    ) & get_het_ab_adj_expr(gt_expr, dp_expr, ad_expr, adj_ab)
 
 
 def annotate_adj(
     mt: hl.MatrixTable,
     adj_gq: int = 20,
     adj_dp: int = 10,
     adj_ab: float = 0.2,
@@ -893,15 +1047,15 @@
     # Return null if counts <= `min_count`
     return hl.or_missing(
         sb_sum > min_count, hl.max(0, fs_expr)  # Needed to avoid -0.0 values
     )
 
 
 def sor_from_sb(
-    sb: Union[hl.expr.ArrayNumericExpression, hl.expr.ArrayExpression]
+    sb: Union[hl.expr.ArrayNumericExpression, hl.expr.ArrayExpression],
 ) -> hl.expr.Float64Expression:
     """
     Compute `SOR` (Symmetric Odds Ratio test) annotation from  the `SB` (strand balance table) field.
 
     .. note::
 
         This function can either take
@@ -1897,88 +2051,236 @@
         in array lengths of 'group_membership'+1. If True, the second element of each
         added annotation is still the 'raw' group, but the group membership is
         determined by the values in the second element of 'group_membership', and the
         output annotations will be the same length as 'group_membership'. Default is
         True.
     :return: Table or MatrixTable with allele frequencies by strata.
     """
+    if not group_membership_includes_raw_group:
+        # Add the 'raw' group to the 'group_membership' annotation.
+        mt = mt.annotate_cols(
+            group_membership=hl.array([mt.group_membership[0]]).extend(
+                mt.group_membership
+            )
+        )
+
+    # Add adj_groups global annotation indicating that the second element in
+    # group_membership is 'raw' and all others are 'adj'.
+    mt = mt.annotate_globals(
+        adj_groups=hl.range(hl.len(mt.group_membership.take(1)[0])).map(
+            lambda x: x != 1
+        )
+    )
+
     if entry_agg_funcs is None:
         entry_agg_funcs = {}
+
+    def _get_freq_expr(gt_expr: hl.expr.CallExpression) -> hl.expr.StructExpression:
+        """
+        Get struct expression with call statistics.
+
+        :param gt_expr: CallExpression to compute call statistics on.
+        :return: StructExpression with call statistics.
+        """
+        # Get the source Table for the CallExpression to grab alleles.
+        ht = gt_expr._indices.source
+        freq_expr = hl.agg.call_stats(gt_expr, ht.alleles)
+        # Select non-ref allele (assumes bi-allelic).
+        freq_expr = freq_expr.annotate(
+            AC=freq_expr.AC[1],
+            AF=freq_expr.AF[1],
+            homozygote_count=freq_expr.homozygote_count[1],
+        )
+
+        return freq_expr
+
+    entry_agg_funcs["freq"] = (lambda x: x.GT, _get_freq_expr)
+
+    return agg_by_strata(mt, entry_agg_funcs, select_fields).drop("adj_groups")
+
+
+def agg_by_strata(
+    mt: hl.MatrixTable,
+    entry_agg_funcs: Dict[str, Tuple[Callable, Callable]],
+    select_fields: Optional[List[str]] = None,
+    group_membership_ht: Optional[hl.Table] = None,
+    entry_agg_group_membership: Optional[Dict[str, List[dict]]] = None,
+) -> hl.Table:
+    """
+    Get row expression for annotations of each entry aggregation function(s) by strata.
+
+    The entry aggregation functions are applied to the MatrixTable entries and
+    aggregated. If no `group_membership_ht` (like the one returned by
+    `generate_freq_group_membership_array`) is supplied, `mt` must contain a
+    'group_membership' annotation that is a list of bools to aggregate the columns by.
+
+    :param mt: Input MatrixTable.
+    :param entry_agg_funcs: Dict of entry aggregation functions where the
+        keys of the dict are the names of the annotations and the values are tuples
+        of functions. The first function is used to transform the `mt` entries in some
+        way, and the second function is used to aggregate the output from the first
+        function.
+    :param select_fields: Optional list of row fields from `mt` to keep on the output
+        Table.
+    :param group_membership_ht: Optional Table containing group membership annotations
+        to stratify the aggregations by. If not provided, the 'group_membership'
+        annotation is expected to be present on `mt`.
+    :param entry_agg_group_membership: Optional dict indicating the subset of group
+        strata in 'freq_meta' to run the entry aggregation functions on. The keys of
+        the dict can be any of the keys in `entry_agg_funcs` and the values are lists
+        of dicts. Each dict in the list contains the strata in 'freq_meta' to use for
+        the corresponding entry aggregation function. If provided, 'freq_meta' must be
+        present in `group_membership_ht` or `mt` and represent the same strata as those
+        in 'group_membership'. If not provided, all entries of the 'group_membership'
+        annotation will have the entry aggregation functions applied to them.
+    :return: Table with annotations of stratified aggregations.
+    """
+    if group_membership_ht is None and "group_membership" not in mt.col:
+        raise ValueError(
+            "The 'group_membership' annotation is not found in the input MatrixTable "
+            "and 'group_membership_ht' is not specified."
+        )
+
     if select_fields is None:
         select_fields = []
 
-    n_samples = mt.count_cols()
+    if group_membership_ht is None:
+        logger.info(
+            "'group_membership_ht' is not specified, using sample stratification "
+            "indicated by the 'group_membership' annotation on the input MatrixTable."
+        )
+        group_globals = mt.index_globals()
+    else:
+        logger.info(
+            "'group_membership_ht' is specified, using sample stratification indicated "
+            "by its 'group_membership' annotation."
+        )
+        group_globals = group_membership_ht.index_globals()
+        mt = mt.annotate_cols(
+            group_membership=group_membership_ht[mt.col_key].group_membership
+        )
+
+    global_expr = {}
     n_groups = len(mt.group_membership.take(1)[0])
+    if "adj_groups" in group_globals:
+        logger.info(
+            "Using the 'adj_groups' global annotation to determine adj filtered "
+            "stratification groups."
+        )
+        global_expr["adj_groups"] = group_globals.adj_groups
+    elif "freq_meta" in group_globals:
+        logger.info(
+            "No 'adj_groups' global annotation found, using the 'freq_meta' global "
+            "annotation to determine adj filtered stratification groups."
+        )
+        global_expr["adj_groups"] = group_globals.freq_meta.map(
+            lambda x: x.get("group", "NA") == "adj"
+        )
+    else:
+        logger.info(
+            "No 'adj_groups' or 'freq_meta' global annotations found. All groups will "
+            "be considered non-adj."
+        )
+        global_expr["adj_groups"] = hl.range(n_groups).map(lambda x: False)
+
+    if entry_agg_group_membership is not None and "freq_meta" not in group_globals:
+        raise ValueError(
+            "The 'freq_meta' global annotation must be supplied when the"
+            " 'entry_agg_group_membership' is specified."
+        )
+
+    entry_agg_group_membership = entry_agg_group_membership or {}
+    entry_agg_group_membership = {
+        ann: [group_globals["freq_meta"].index(s) for s in strata]
+        for ann, strata in entry_agg_group_membership.items()
+    }
+
+    n_adj_groups = hl.eval(hl.len(global_expr["adj_groups"]))
+    if n_adj_groups != n_groups:
+        raise ValueError(
+            f"The number of elements in the 'adj_groups' ({n_adj_groups}) global "
+            "annotation does not match the number of elements in the "
+            f"'group_membership' annotation ({n_groups})!",
+        )
+
+    # Keep only the entries needed for the aggregation functions.
+    select_expr = {**{ann: f[0](mt) for ann, f in entry_agg_funcs.items()}}
+    has_adj = hl.eval(hl.any(global_expr["adj_groups"]))
+    if has_adj:
+        select_expr["adj"] = mt.adj
+
+    mt = mt.select_entries(**select_expr)
+
+    # Convert MT to HT with a row annotation that is an array of all samples entries
+    # for that variant.
     ht = mt.localize_entries("entries", "cols")
-    ht = ht.annotate_globals(
-        indices_by_group=hl.range(n_groups).map(
-            lambda g_i: hl.range(n_samples).filter(
-                lambda s_i: ht.cols[s_i].group_membership[g_i]
-            )
+
+    # For each stratification group in group_membership, determine the indices of the
+    # samples that belong to that group.
+    global_expr["indices_by_group"] = hl.range(n_groups).map(
+        lambda g_i: hl.range(mt.count_cols()).filter(
+            lambda s_i: ht.cols[s_i].group_membership[g_i]
         )
     )
+    ht = ht.annotate_globals(**global_expr)
+
     # Pull out each annotation that will be used in the array aggregation below as its
     # own ArrayExpression. This is important to prevent memory issues when performing
     # the below array aggregations.
     ht = ht.select(
         *select_fields,
-        adj_array=ht.entries.map(lambda e: e.adj),
-        gt_array=ht.entries.map(lambda e: e.GT),
-        **{
-            ann: hl.map(lambda e, s: f[0](e, s), ht.entries, ht.cols)
-            for ann, f in entry_agg_funcs.items()
-        },
+        **{ann: ht.entries.map(lambda e: e[ann]) for ann in select_expr.keys()},
     )
 
     def _agg_by_group(
-        ht: hl.Table, agg_func: Callable, ann_expr: hl.expr.ArrayExpression, *args
+        indices_by_group_expr: hl.expr.ArrayExpression,
+        adj_groups_expr: hl.expr.ArrayExpression,
+        agg_func: Callable,
+        ann_expr: hl.expr.ArrayExpression,
     ) -> hl.expr.ArrayExpression:
         """
         Aggregate `agg_expr` by group using the `agg_func` function.
 
-        :param ht: Input Hail Table.
-        :param agg_func: Aggregation function to apply to `agg_expr`.
-        :param agg_expr: Expression to aggregate by group.
-        :param args: Additional arguments to pass to the `agg_func`.
+        :param indices_by_group_expr: ArrayExpression of indices of samples in each group.
+        :param adj_groups_expr: ArrayExpression indicating whether each group is adj.
+        :param agg_func: Aggregation function to apply to `ann_expr`.
+        :param ann_expr: Expression to aggregate by group.
         :return: Aggregated array expression.
         """
-        adj_agg_expr = ht.indices_by_group.map(
-            lambda s_indices: s_indices.aggregate(
-                lambda i: hl.agg.filter(ht.adj_array[i], agg_func(ann_expr[i], *args))
+        f_no_adj = lambda i, *args: agg_func(ann_expr[i])
+        if has_adj:
+            f = lambda i, adj: hl.if_else(
+                adj, hl.agg.filter(ht.adj[i], f_no_adj(i)), f_no_adj(i)
             )
-        )
-        # Create final agg list by inserting or changing the "raw" group,
-        # representing all samples, in the adj_agg_list.
-        raw_agg_expr = ann_expr.aggregate(lambda x: agg_func(x, *args))
-        if group_membership_includes_raw_group:
-            extend_idx = 2
         else:
-            extend_idx = 1
+            f = f_no_adj
 
-        adj_agg_expr = (
-            adj_agg_expr[:1].append(raw_agg_expr).extend(adj_agg_expr[extend_idx:])
+        return hl.map(
+            lambda s_indices, adj: s_indices.aggregate(lambda i: f(i, adj)),
+            indices_by_group_expr,
+            adj_groups_expr,
         )
 
-        return adj_agg_expr
-
-    freq_expr = _agg_by_group(ht, hl.agg.call_stats, ht.gt_array, ht.alleles)
-
-    # Select non-ref allele (assumes bi-allelic).
-    freq_expr = freq_expr.map(
-        lambda cs: cs.annotate(
-            AC=cs.AC[1],
-            AF=cs.AF[1],
-            homozygote_count=cs.homozygote_count[1],
-        )
-    )
     # Add annotations for any supplied entry transform and aggregation functions.
+    # Filter groups to only those in entry_agg_group_membership if specified.
+    # If there are no specific entry group indices for an annotation, use ht[g]
+    # to consider all groups without filtering.
     ht = ht.select(
         *select_fields,
-        **{ann: _agg_by_group(ht, f[1], ht[ann]) for ann, f in entry_agg_funcs.items()},
-        freq=freq_expr,
+        **{
+            ann: _agg_by_group(
+                *[
+                    [ht[g][i] for i in entry_agg_group_membership.get(ann, [])] or ht[g]
+                    for g in ["indices_by_group", "adj_groups"]
+                ],
+                agg_func=f[1],
+                ann_expr=ht[ann],
+            )
+            for ann, f in entry_agg_funcs.items()
+        },
     )
 
     return ht.drop("cols")
 
 
 def update_structured_annotations(
     ht: hl.Table,
@@ -2042,95 +2344,14 @@
                 )
             }
         )
 
     return ht.annotate(**updated_rows)
 
 
-def gks_compute_seqloc_digest(
-    ht: hl.Table,
-    export_tmpfile: Optional[str] = None,
-    computed_tmpfile: Optional[str] = None,
-):
-    """
-    Compute sequence location digest-based id for a hail variant Table.
-
-    Exports table to tsv, computes SequenceLocation digests, reimports and replaces
-    the vrs_json field with the result. Input table must have a .vrs field, like the
-    one added by add_gks_vrs, that can be used to construct ga4gh.vrs models.
-
-    :param ht: hail table with VRS annotation
-    :param export_tmpfile: Optional file path to export the table to.
-    :param computed_tmpfile: Optional file path to write the updated rows to,
-        which is then imported as a hail table
-    :return: a hail table with the VRS annotation updated with the new SequenceLocations
-    """
-    # NOTE: The pinned ga4gh.vrs module breaks logging when this annotations module is
-    # imported. Importing ga4gh here to avoid this issue.
-    import ga4gh.core as ga4gh_core
-    import ga4gh.vrs as ga4gh_vrs
-
-    if export_tmpfile is None:
-        export_tmpfile = new_temp_file("gks-seqloc-pre.tsv")
-    if computed_tmpfile is None:
-        computed_tmpfile = new_temp_file("gks-seqloc-post.tsv")
-
-    logger.info("Exporting ht to %s", export_tmpfile)
-    ht.select("vrs_json").export(export_tmpfile, header=True)
-
-    logger.info(
-        "Computing SequenceLocation digests and writing to %s", computed_tmpfile
-    )
-    start = timer()
-    counter = 0
-    with open(computed_tmpfile, "w", encoding="utf-8") as f_out:
-        with open(export_tmpfile, "r", encoding="utf-8") as f:
-            reader = csv.reader(f, delimiter="\t")
-            header = None
-            for line in reader:
-                if header is None:
-                    header = line
-                    f_out.write("\t".join(header))
-                    f_out.write("\n")
-                    continue
-                else:
-                    locus, alleles, vrs_json = line
-                    vrs_variant = json.loads(vrs_json)
-                    location = vrs_variant["location"]
-                    location.pop("_id")
-                    location_id = ga4gh_core._internal.identifiers.ga4gh_identify(
-                        ga4gh_vrs.models.SequenceLocation(**location)
-                    )
-                    vrs_variant["location"]["_id"] = location_id
-                    # serialize outputs to JSON and write to TSV
-                    vrs_json = json.dumps(vrs_variant)
-                    alleles = json.dumps(json.loads(alleles))
-                    f_out.write("\t".join([locus, alleles, vrs_json]))
-                    f_out.write("\n")
-                    counter += 1
-    end = timer()
-    logger.info(
-        "Computed %s SequenceLocation digests in %s seconds", counter, (end - start)
-    )
-    logger.info("Importing VRS records with computed SequenceLocation digests")
-    ht_with_location = hl.import_table(
-        computed_tmpfile, types={"locus": "tstr", "alleles": "tstr", "vrs_json": "tstr"}
-    )
-    ht_with_location_parsed = ht_with_location.annotate(
-        locus=hl.locus(
-            contig=ht_with_location.locus.split(":")[0],
-            pos=hl.int32(ht_with_location.locus.split(":")[1]),
-            reference_genome="GRCh38",
-        ),
-        alleles=hl.parse_json(ht_with_location.alleles, dtype=hl.tarray(hl.tstr)),
-    ).key_by("locus", "alleles")
-
-    return ht.drop("vrs_json").join(ht_with_location_parsed, how="left")
-
-
 def add_gks_vrs(
     input_locus: hl.locus,
     input_vrs: hl.struct,
 ) -> dict:
     """
     Generate a dictionary containing VRS information from a given locus and struct of VRS information.
 
@@ -2222,15 +2443,14 @@
     pos = input_struct.locus.position
     ref = input_struct.alleles[0]
     var = input_struct.alleles[1]
     gnomad_id = f"{contig}-{pos}-{ref}-{var}"
 
     # Define function to return a frequency report dictionary for a given group
     def _create_group_dicts(
-        group_index: int,
         group_id: str,
         group_label: str,
         group_sex: str = None,
     ) -> dict:
         """
         Generate a dictionary containing the frequency information of a given variant for a given group.
 
@@ -2240,63 +2460,79 @@
         :param group_label: String containing the full name of genetic ancestry group requested.
             - Example: "African/African American".
         :param group_sex: String indicating the sex of the group.
             - Example: "XX" or "XY".
         :return: Dictionary containing variant frequency information,
             - (by genetic ancestry group and sex if desired) for specified variant.
         """
+        if group_sex:
+            cohort_id = f"{group_id.upper()}.{group_sex}"
+            freq_index_key = f"{group_id}_{group_sex}_adj"
+        else:
+            cohort_id = f"{group_id.upper()}"
+            freq_index_key = f"{group_id}_adj"
+        record_id = f"{gnomad_id}.{cohort_id}"
+
         # Obtain frequency information for the specified variant.
-        group_freq = input_struct.freq[group_index]
+        group_freq = input_struct.freq[freq_index_dict[freq_index_key]]
 
         # Cohort characteristics.
         characteristics = []
         characteristics.append({"name": "genetic ancestry", "value": group_label})
         if group_sex is not None:
             characteristics.append({"name": "biological sex", "value": group_sex})
 
         # Dictionary to be returned containing information for a specified group.
         freq_record = {
-            "id": f"{gnomad_id},{group_id.upper()}",
+            "id": record_id,
             "type": "CohortAlleleFrequency",
             "label": f"{group_label} Cohort Allele Frequency for {gnomad_id}",
             "focusAllele": "#/focusAllele",
             "focusAlleleCount": group_freq["AC"],
             "locusAlleleCount": group_freq["AN"],
-            "alleleFrequency": group_freq["AF"],
-            "cohort": {"id": group_id.upper(), "characteristics": characteristics},
+            "alleleFrequency": (
+                group_freq["AF"] if group_freq["AF"] is not None else 0.0
+            ),
+            "cohort": {"id": cohort_id, "characteristics": characteristics},
             "ancillaryResults": {"homozygotes": group_freq["homozygote_count"]},
         }
 
+        # Add hemizygote allele count if variant is non-autosomal/non-PAR.
+        # Only XY groups can be hemizygous. Other group AC is mixed homo/hetero.
+        # If not a by_sex group, include the XY hemizygote count for XY subgroup.
+        if not input_struct.in_autosome_or_par:
+            if group_sex == "XY":
+                freq_record["ancillaryResults"]["hemizygotes"] = group_freq.AC
+            elif group_sex is None:
+                # Group is not by_sex, but still need to report hemizygotes.
+                hemi_group_freq = input_struct.freq[
+                    freq_index_dict[f"{group_id}_XY_adj"]
+                ]
+                freq_record["ancillaryResults"]["hemizygotes"] = hemi_group_freq.AC
+
         return freq_record
 
     # Create a list to then add the dictionaries for frequency reports for
     # different ancestry groups to.
     list_of_group_info_dicts = []
 
     # Iterate through provided groups and generate dictionaries.
     if ancestry_groups:
         for group in ancestry_groups:
-            key = f"{group}-adj"
-            index_value = freq_index_dict.get(key)
             group_result = _create_group_dicts(
-                group_index=index_value,
                 group_id=group,
                 group_label=ancestry_groups_dict[group],
             )
 
             # If specified, stratify group information by sex.
             if by_sex:
                 sex_list = []
                 for sex in ["XX", "XY"]:
-                    sex_key = f"{group}-{sex}-adj"
-                    sex_index_value = freq_index_dict.get(sex_key)
-                    sex_id = f"{group}.{sex}"
                     sex_result = _create_group_dicts(
-                        group_index=sex_index_value,
-                        group_id=sex_id,
+                        group_id=group,
                         group_label=ancestry_groups_dict[group],
                         group_sex=sex,
                     )
                     sex_list.append(sex_result)
 
                 group_result["subcohortFrequency"] = sex_list
 
@@ -2318,40 +2554,95 @@
             "version": f"{label_version}",
         },
         "focusAllele": (
             ""
         ),  # Information can be populated with the result of add_gks_vrs()
         "focusAlleleCount": overall_freq["AC"],
         "locusAlleleCount": overall_freq["AN"],
-        "alleleFrequency": overall_freq["AF"],
+        "alleleFrequency": (
+            overall_freq["AF"] if overall_freq["AF"] is not None else 0.0
+        ),
         "cohort": {"id": "ALL"},
     }
 
-    # Create ancillaryResults for additional frequency and popMaxFAF95 information
+    # Create ancillaryResults for additional frequency and popMaxFAF95 information.
     ancillaryResults = {
         "homozygotes": overall_freq["homozygote_count"],
-        "popMaxFAF95": {
-            "frequency": input_struct.faf95.popmax,
-            "confidenceInterval": 0.95,
-        },
     }
 
-    if input_struct.faf95.popmax_population is not None:
-        ancillaryResults["popMaxFAF95"][
-            "popFreqID"
-        ] = f"{gnomad_id}.{input_struct.faf95.popmax_population.upper()}"
-    else:
-        ancillaryResults["popMaxFAF95"]["popFreqID"] = None
+    # Add hemizygote count if not autosomal or PAR.
+    if not input_struct.in_autosome_or_par:
+        hemizygote_count = input_struct.freq[freq_index_dict["XY_adj"]].AC
+        ancillaryResults["hemizygotes"] = hemizygote_count
+
+    # Add group max FAF if it exists
+    if input_struct.grpMaxFAF95.popmax_population is not None:
+        ancillaryResults["grpMaxFAF95"] = {
+            "frequency": input_struct.grpMaxFAF95.popmax,
+            "confidenceInterval": 0.95,
+            "groupId": (
+                f"{gnomad_id}.{input_struct.grpMaxFAF95.popmax_population.upper()}"
+            ),
+        }
+
+    # Add joint group max FAF if it exists.
+    if (
+        "jointGrpMaxFAF95" in input_struct
+        and input_struct.jointGrpMaxFAF95.popmax_population is not None
+    ):
+        ancillaryResults["jointGrpMaxFAF95"] = {
+            "frequency": input_struct.jointGrpMaxFAF95.popmax,
+            "confidenceInterval": 0.95,
+            "groupId": (
+                f"{gnomad_id}.{input_struct.jointGrpMaxFAF95.popmax_population.upper()}"
+            ),
+        }
 
-    # Add mean coverage depth statistics if the input was annotated
+    final_freq_dict["ancillaryResults"] = ancillaryResults
+
+    # Check allele balance for heterozygotes values.
+    # Flagged allele balance values are those in bins > 0.90.
+    # Each bin is 0.05, so flagged values are in the last 2 bins.
+    if len(input_struct.ab_hist_alt.bin_freq) != 20:
+        raise ValueError(
+            f"{gnomad_id} ab_hist_alt.bin_freq had "
+            f"{len(input_struct.ab_hist_alt.bin_freq)} items, expected 20"
+        )
+    # The bin_freq should be in order but we can verify the order from bin_edges.
+    ab_bin_freq = list(
+        map(
+            lambda x: x[1],
+            sorted(
+                zip(
+                    input_struct.ab_hist_alt.bin_edges,
+                    input_struct.ab_hist_alt.bin_freq,
+                ),
+                key=lambda x: x[0],
+            ),
+        )
+    )
+
+    qualityMeasures = {
+        "qcFilters": list(input_struct.filters),
+        "lowComplexityRegion": input_struct.lcr,
+        "heterozygousSkewedAlleleCount": sum(ab_bin_freq[-2:]),
+    }
+
+    # Add coverage depth statistics if the input was annotated
     # with coverage information.
     if "mean_depth" in input_struct:
-        ancillaryResults["meanDepth"] = input_struct.mean_depth
+        qualityMeasures["meanDepth"] = input_struct.mean_depth
 
-    final_freq_dict["ancillaryResults"] = ancillaryResults
+    if "fraction_cov_over_20" in input_struct:
+        qualityMeasures["fractionCoverage20x"] = input_struct.fraction_cov_over_20
+
+    # Add monoallelic flag (all samples homozygous for alternate allele)
+    qualityMeasures["monoallelic"] = input_struct.monoallelic
+
+    final_freq_dict["qualityMeasures"] = qualityMeasures
 
     # If ancestry_groups were passed, add the ancestry group dictionary to the
     # final frequency dictionary to be returned.
     if ancestry_groups:
         final_freq_dict["subcohortFrequency"] = list_of_group_info_dicts
 
     return final_freq_dict
```

### Comparing `gnomad-0.7.1/gnomad/utils/constraint.py` & `gnomad-0.8.0/gnomad/utils/constraint.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 def count_variants_by_group(
     ht: hl.Table,
     freq_expr: Optional[hl.expr.ArrayExpression] = None,
     freq_meta_expr: Optional[hl.expr.ArrayExpression] = None,
     count_singletons: bool = False,
     count_downsamplings: Tuple[str] = (),
+    downsamplings: Optional[List[int]] = None,
     additional_grouping: Tuple[str] = (),
     partition_hint: int = 100,
     omit_methylation: bool = False,
     use_table_group_by: bool = False,
     singleton_expr: Optional[hl.expr.BooleanExpression] = None,
     max_af: Optional[float] = None,
 ) -> Union[hl.Table, Any]:
@@ -125,14 +126,16 @@
     :param freq_meta_expr: ArrayExpression of meta dictionaries corresponding to
         `freq_expr`. If `count_downsamplings` and `freq_meta_expr` is None,
         `freq_meta_expr` would be `ht.freq_meta`.
     :param count_singletons: Whether to count singletons (defined by `singleton_expr`).
         Default is False.
     :param count_downsamplings: Tuple of populations to use for downsampling counts.
         Default is ().
+    :param downsamplings: Optional List of integers specifying what downsampling
+        indices to obtain. Default is None, which will return all downsampling counts.
     :param additional_grouping: Additional features to group by. e.g. 'exome_coverage'.
         Default is ().
     :param partition_hint: Target number of partitions for aggregation. Default is 100.
     :param omit_methylation: Whether to omit 'methylation_level' from the grouping when
         counting variants. Default is False.
     :param use_table_group_by: Whether to group `ht` before aggregating the variant
         counts. If `use_table_group_by` is False, function will return a hl.
@@ -200,25 +203,34 @@
         logger.info(
             "Counting variants in downsamplings for population '%s', and adding as"
             " 'downsampling_counts_%s' annotation.",
             pop,
             pop,
         )
         agg[f"downsampling_counts_{pop}"] = downsampling_counts_expr(
-            freq_expr, freq_meta_expr, pop, max_af=max_af
+            freq_expr,
+            freq_meta_expr,
+            pop,
+            max_af=max_af,
+            downsamplings=downsamplings,
         )
         if count_singletons:
             logger.info(
                 "Counting singleton variants in downsamplings for population '%s', and"
                 " adding as 'singleton_downsampling_counts_%s' annotation.",
                 pop,
                 pop,
             )
             agg[f"singleton_downsampling_counts_{pop}"] = downsampling_counts_expr(
-                freq_expr, freq_meta_expr, pop, singleton=True
+                freq_expr,
+                freq_meta_expr,
+                pop,
+                max_af=max_af,
+                downsamplings=downsamplings,
+                singleton=True,
             )
     # Apply each variant count aggregation in `agg` to get counts for all
     # combinations of `grouping`.
     if use_table_group_by:
         return ht.group_by(**grouping).partition_hint(partition_hint).aggregate(**agg)
     else:
         return ht.aggregate(
@@ -226,69 +238,118 @@
         )
 
 
 def get_downsampling_freq_indices(
     freq_meta_expr: hl.expr.ArrayExpression,
     pop: str = "global",
     variant_quality: str = "adj",
+    genetic_ancestry_label: Optional[str] = None,
+    subset: Optional[str] = None,
+    downsamplings: Optional[List[int]] = None,
 ) -> hl.expr.ArrayExpression:
     """
-    Get indices of dictionaries in meta dictionaries that only have the "downsampling" key with specified "pop" and "variant_quality" values.
+    Get indices of dictionaries in meta dictionaries that only have the "downsampling" key with specified `genetic_ancestry_label` and "variant_quality" values.
 
     :param freq_meta_expr: ArrayExpression containing the set of groupings for each
         element of the `freq_expr` array (e.g., [{'group': 'adj'}, {'group': 'adj',
         'pop': 'nfe'}, {'downsampling': '5000', 'group': 'adj', 'pop': 'global'}]).
-    :param pop: Population to use for filtering by the 'pop' key in `freq_meta_expr`.
-        Default is 'global'.
+    :param pop: Population to use for filtering by the `genetic_ancestry_label` key in
+        `freq_meta_expr`. Default is 'global'.
     :param variant_quality: Variant quality to use for filtering by the 'group' key in
         `freq_meta_expr`. Default is 'adj'.
+    :param genetic_ancestry_label: Label defining the genetic ancestry groups. If None,
+        "gen_anc" or "pop" is used (in that order of preference) if present. Default is
+        None.
+    :param subset: Subset to use for filtering by the 'subset' key in `freq_meta_expr`.
+        Default is None, which will return all downsampling indices without a 'subset'
+        key in `freq_meta_expr`.
+    :param downsamplings: Optional List of integers specifying what downsampling
+        indices to obtain. Default is None, which will return all downsampling indices.
+    :return: ArrayExpression of indices of dictionaries in `freq_meta_expr` that only
+        have the "downsampling" key with specified `genetic_ancestry_label` and
+        "variant_quality" values.
     """
-    indices = hl.enumerate(freq_meta_expr).filter(
-        lambda f: (f[1].get("group") == variant_quality)
-        & (f[1].get("pop") == pop)
-        & f[1].contains("downsampling")
-    )
+    if genetic_ancestry_label is None:
+        gen_anc = ["gen_anc", "pop"]
+    else:
+        gen_anc = [genetic_ancestry_label]
+
+    def _get_filter_expr(m: hl.expr.StructExpression) -> hl.expr.BooleanExpression:
+        filter_expr = (
+            (m.get("group") == variant_quality)
+            & (hl.any([m.get(l, "") == pop for l in gen_anc]))
+            & m.contains("downsampling")
+        )
+        if downsamplings is not None:
+            filter_expr &= hl.literal(downsamplings).contains(
+                hl.int(m.get("downsampling", "0"))
+            )
+        if subset is None:
+            filter_expr &= ~m.contains("subset")
+        else:
+            filter_expr &= m.get("subset", "") == subset
+        return filter_expr
+
+    indices = hl.enumerate(freq_meta_expr).filter(lambda f: _get_filter_expr(f[1]))
+
     # Get an array of indices and meta dictionaries sorted by "downsampling" key.
     return hl.sorted(indices, key=lambda f: hl.int(f[1]["downsampling"]))
 
 
 def downsampling_counts_expr(
     freq_expr: hl.expr.ArrayExpression,
     freq_meta_expr: hl.expr.ArrayExpression,
     pop: str = "global",
     variant_quality: str = "adj",
     singleton: bool = False,
     max_af: Optional[float] = None,
+    genetic_ancestry_label: Optional[str] = None,
+    subset: Optional[str] = None,
+    downsamplings: Optional[List[int]] = None,
 ) -> hl.expr.ArrayExpression:
     """
     Return an aggregation expression to compute an array of counts of all downsamplings found in `freq_expr` where specified criteria is met.
 
     The frequency metadata (`freq_meta_expr`) should be in a similar format to the
     `freq_meta` annotation added by `annotate_freq()`. Each downsampling should have
-    'group', 'pop', and 'downsampling' keys. Included downsamplings are those where
-    'group' == `variant_quality` and 'pop' == `pop`.
+    'group', `genetic_ancestry_label`, and 'downsampling' keys. Included downsamplings
+    are those where 'group' == `variant_quality` and `genetic_ancestry_label` == `pop`.
 
     :param freq_expr: ArrayExpression of Structs with 'AC' and 'AF' annotations.
     :param freq_meta_expr: ArrayExpression containing the set of groupings for each
         element of the `freq_expr` array (e.g., [{'group': 'adj'}, {'group': 'adj',
         'pop': 'nfe'}, {'downsampling': '5000', 'group': 'adj', 'pop': 'global'}]).
-    :param pop: Population to use for filtering by the 'pop' key in `freq_meta_expr`.
-        Default is 'global'.
+    :param pop: Population to use for filtering by the `genetic_ancestry_label` key in
+        `freq_meta_expr`. Default is 'global'.
     :param variant_quality: Variant quality to use for filtering by the 'group' key in
         `freq_meta_expr`. Default is 'adj'.
     :param singleton: Whether to filter to only singletons before counting (AC == 1).
         Default is False.
     :param max_af: Maximum variant allele frequency to keep. By default no allele
         frequency cutoff is applied.
+    :param genetic_ancestry_label: Label defining the genetic ancestry groups. If None,
+        "gen_anc" or "pop" is used (in that order of preference) if present. Default is
+        None.
+    :param subset: Subset to use for filtering by the 'subset' key in `freq_meta_expr`.
+        Default is None, which will return all downsampling counts without a 'subset'
+        key in `freq_meta_expr`. If specified, only downsamplings with the specified
+        subset will be included.
+    :param downsamplings: Optional List of integers specifying what downsampling
+        indices to obtain. Default is None, which will return all downsampling counts.
     :return: Aggregation Expression for an array of the variant counts in downsamplings
         for specified population.
     """
     # Get an array of indices sorted by "downsampling" key.
     sorted_indices = get_downsampling_freq_indices(
-        freq_meta_expr, pop, variant_quality
+        freq_meta_expr,
+        pop,
+        variant_quality,
+        genetic_ancestry_label,
+        subset,
+        downsamplings,
     ).map(lambda x: x[0])
 
     def _get_criteria(i: hl.expr.Int32Expression) -> hl.expr.Int32Expression:
         """
         Return 1 when variant meets specified criteria (`singleton` or `max_af`), if requested, or with an AC > 0.
 
         :param i: The index of a downsampling.
@@ -405,15 +466,15 @@
         return t.annotate(
             mutation_type=mutation_type_expr,
             mutation_type_model=mutation_type_model_expr,
         )
 
 
 def trimer_from_heptamer(
-    t: Union[hl.MatrixTable, hl.Table]
+    t: Union[hl.MatrixTable, hl.Table],
 ) -> Union[hl.MatrixTable, hl.Table]:
     """
     Trim heptamer context to create trimer context.
 
     :param t: Input MatrixTable or Table with context annotation.
     :return: MatrixTable or Table with trimer context annotated.
     """
@@ -422,15 +483,15 @@
         t.annotate_rows(context=trimer_expr)
         if isinstance(t, hl.MatrixTable)
         else t.annotate(context=trimer_expr)
     )
 
 
 def collapse_strand(
-    t: Union[hl.Table, hl.MatrixTable]
+    t: Union[hl.Table, hl.MatrixTable],
 ) -> Union[hl.Table, hl.MatrixTable]:
     """
     Return the deduplicated context by collapsing DNA strands.
 
     Function returns the reverse complement for 'ref, 'alt', and 'context' if the
     reference allele is either 'G' or 'T'.
 
@@ -786,24 +847,27 @@
             `vep_annotation_expr`, or "None" if neither is defined
         - gene - 'gene_symbol' annotation inside `vep_annotation_expr`
         - coverage - exome coverage if `coverage_expr` is specified
         - transcript - id from 'transcript_id' in `vep_annotation_expr` (added when
             `include_transcript_group` is True)
         - canonical from `vep_annotation_expr` (added when `include_canonical_group` is
             True)
+        - mane_select from `vep_annotation_expr` (added when `include_mane_select_group` is
+            True)
 
     .. note::
         This function expects that the following fields are present in
         `vep_annotation_expr`:
         - lof
         - polyphen_prediction
         - most_severe_consequence
         - gene_symbol
         - transcript_id (if `include_transcript_group` is True)
         - canonical (if `include_canonical_group` is True)
+        - mane_select (if `include_mane_select_group` is True)
 
     :param vep_annotation_expr: StructExpression of VEP annotation.
     :param coverage_expr: Optional Int32Expression of exome coverage. Default is None.
     :param include_transcript_group: Whether to include the transcript annotation in the
         groupings. Default is True.
     :param include_canonical_group: Whether to include canonical annotation in the
         groupings. Default is True.
@@ -817,14 +881,15 @@
     polyphen_prediction_expr = vep_annotation_expr.polyphen_prediction
 
     # Create constraint annotations to be used for groupings.
     groupings = {
         "annotation": vep_annotation_expr.most_severe_consequence,
         "modifier": hl.coalesce(lof_expr, polyphen_prediction_expr, "None"),
         "gene": vep_annotation_expr.gene_symbol,
+        "gene_id": vep_annotation_expr.gene_id,
     }
     if coverage_expr is not None:
         groupings["coverage"] = coverage_expr
 
     # Add 'transcript' and 'canonical' annotation if requested.
     if include_transcript_group:
         groupings["transcript"] = vep_annotation_expr.transcript_id
@@ -855,14 +920,16 @@
             `vep_annotation`, or "None" if neither is defined
         - gene - 'gene_symbol' annotation inside `vep_annotation`
         - coverage - exome coverage in `ht`
         - transcript - id from 'transcript_id' in `vep_annotation` (added when
             `include_transcript_group` is True)
         - canonical from `vep_annotation` (added when `include_canonical_group` is
             True)
+        - mane_select from `vep_annotation` (added when `include_mane_select_group` is
+            True)
 
     .. note::
         This function expects that the following annotations are present in `ht`:
         - vep
         - exome_coverage
 
     :param t: Input Table or MatrixTable.
@@ -913,26 +980,28 @@
 
 
 def compute_expected_variants(
     ht: hl.Table,
     plateau_models_expr: hl.StructExpression,
     mu_expr: hl.Float64Expression,
     cov_corr_expr: hl.Float64Expression,
+    possible_variants_expr: hl.Int64Expression,
     cpg_expr: hl.BooleanExpression,
     pop: Optional[str] = None,
 ) -> Dict[str, Union[hl.Float64Expression, hl.Int64Expression]]:
     """
     Apply plateau models for all sites and for a population (if specified) to compute predicted proportion observed ratio and expected variant counts.
 
     :param ht: Input Table.
     :param plateau_models_expr: Linear models (output of `build_models()`, with the values
         of the dictionary formatted as a StructExpression of intercept and slope, that
         calibrates mutation rate to proportion observed for high coverage exomes. It
-        includes models for CpG, non-CpG sites, and each population in `POPS`.
+        includes models for CpG, non-CpG sites, and each population if specified.
     :param mu_expr: Float64Expression of mutation rate.
+    :param possible_variants_expr: Int64Expression of possible variant counts.
     :param cov_corr_expr: Float64Expression of corrected coverage expression.
     :param cpg_expr: BooleanExpression noting whether a site is a CPG site.
     :param pop: Optional population to use when applying plateau model. Default is
         None.
     :return: A dictionary with predicted proportion observed ratio and expected variant
         counts.
     """
@@ -954,15 +1023,17 @@
     # Apply plateau models for specified population.
     ppo_expr = mu_expr * slope + intercept
 
     # Generate sum aggregators for 'predicted_proportion_observed' and
     # 'expected_variants', for specified population.
     agg_expr = {
         f"predicted_proportion_observed{pop}": agg_func(ppo_expr),
-        f"expected_variants{pop}": agg_func(ppo_expr * cov_corr_expr),
+        f"expected_variants{pop}": agg_func(
+            ppo_expr * cov_corr_expr * possible_variants_expr
+        ),
     }
 
     # Generate sum aggregators for 'observed_variants' and 'possible_variants' on
     # the entire dataset if pop is None, and for 'downsampling_counts' for
     # specified population if pop is not None.
     agg_expr.update({ann: agg_func(ht[ann]) for ann in ann_to_sum})
 
@@ -1273,7 +1344,69 @@
         sd_expr = hl.agg.explode(
             lambda x: hl.agg.stats(x), [raw_z_expr, -raw_z_expr]
         ).stdev
     else:
         sd_expr = hl.agg.stats(raw_z_expr).stdev
 
     return hl.agg.filter(filter_expr, sd_expr)
+
+
+def add_gencode_transcript_annotations(
+    ht: hl.Table,
+    gencode_ht: hl.Table,
+    annotations: List[str] = ["level", "transcript_type"],
+) -> hl.Table:
+    """
+    Add GENCODE annotations to Table based on transcript id.
+
+    .. note::
+        Added annotations by default are:
+        - level
+        - transcript_type
+
+        Computed annotations are:
+        - chromosome
+        - cds_length
+        - num_coding_exons
+
+    :param ht: Input Table.
+    :param gencode_ht: Table with GENCODE annotations.
+    :param annotations: List of GENCODE annotations to add. Default is ["level", "transcript_type"].
+        Added annotations also become keys for the group by when computing "cds_length" and "num_coding_exons".
+    :return: Table with transcript annotations from GENCODE added.
+    """
+    gencode_ht = gencode_ht.annotate(
+        length=gencode_ht.interval.end.position
+        - gencode_ht.interval.start.position
+        + 1,
+        chromosome=gencode_ht.interval.start.contig,
+    )
+
+    # Obtain CDS annotations from GENCODE file and calculate CDS length and
+    # number of exons.
+    annotations_to_add = set(annotations + ["chromosome", "transcript_id", "length"])
+
+    gencode_cds = (
+        gencode_ht.filter(gencode_ht.feature == "CDS")
+        .select(*annotations_to_add)
+        .key_by("transcript_id")
+        .drop("interval")
+    )
+
+    annotations_to_add.remove("length")
+
+    gencode_cds = (
+        gencode_cds.group_by(*annotations_to_add)
+        .aggregate(
+            cds_length=hl.agg.sum(gencode_cds.length), num_coding_exons=hl.agg.count()
+        )
+        .key_by("transcript_id")
+    )
+
+    gencode_cds = gencode_cds.checkpoint(
+        new_temp_file(prefix="gencode_cds", extension="ht")
+    )
+
+    # Add GENCODE annotations to input Table.
+    ht = ht.annotate(**gencode_cds[ht.transcript])
+
+    return ht
```

### Comparing `gnomad-0.7.1/gnomad/utils/file_utils.py` & `gnomad-0.8.0/gnomad/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/utils/filtering.py` & `gnomad-0.8.0/gnomad/utils/filtering.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         else:
             mt = mt.filter(filter_criteria)
 
     return mt
 
 
 def filter_to_autosomes(
-    t: Union[hl.MatrixTable, hl.Table]
+    t: Union[hl.MatrixTable, hl.Table],
 ) -> Union[hl.MatrixTable, hl.Table]:
     """
     Filter the Table or MatrixTable to autosomes only.
 
     This assumes that the input contains a field named `locus` of type Locus
 
     :param t: Input MT/HT
@@ -379,14 +379,82 @@
     logger.info(
         "Found %d variants after filtering to clinvar pathogenic variants.",
         t.count_rows() if isinstance(t, hl.MatrixTable) else t.count(),
     )
     return t
 
 
+def filter_to_gencode_cds(
+    t: Union[hl.MatrixTable, hl.Table], gencode_ht: Optional[hl.Table] = None
+) -> hl.Table:
+    """
+    Filter a Table/MatrixTable to only Gencode CDS regions in protein coding transcripts.
+
+    Example use:
+
+    .. code-block:: python
+
+        from gnomad.resources.grch37.reference_data import gencode
+        gencode_ht = gencode.ht()
+        gencode_ht = filter_gencode_to_cds(gencode_ht)
+
+    .. note::
+
+        If no Gencode Table is provided, the default version of the Gencode Table
+        resource for the genome build of the input Table/MatrixTable will be used.
+
+    .. warning::
+
+        This Gencode CDS interval filter does not take into account the
+        transcript_id, it filters to any locus that is found in a CDS interval for
+        any protein coding transcript. Therefore, if downstream analyses require
+        filtering to CDS intervals by transcript, an additional step must be taken.
+        For example, when filtering VEP transcript consequences, there may be cases
+        where a variant is retained with this filter, but is considered outside the
+        CDS intervals of the transcript per the VEP predicted consequence of the
+        variant.
+
+    :param t: Input Table/MatrixTable to filter.
+    :param gencode_ht: Gencode Table to use for filtering the input Table/MatrixTable
+        to CDS regions. Default is None, which will use the default version of the
+        Gencode Table resource.
+    :return: Table/MatrixTable filtered to loci in Gencode CDS intervals.
+    """
+    if gencode_ht is None:
+        build = get_reference_genome(t.locus).name
+        if build == "GRCh37":
+            from gnomad.resources.grch37.reference_data import gencode
+        elif build == "GRCh38":
+            from gnomad.resources.grch38.reference_data import gencode
+        else:
+            raise ValueError(f"Unsupported reference genome build: {build}")
+
+        logger.info(
+            "No Gencode Table was supplied, using Gencode version %s",
+            gencode.default_version,
+        )
+        gencode_ht = gencode.ht()
+
+    gencode_ht = gencode_ht.filter(
+        (gencode_ht.feature == "CDS") & (gencode_ht.transcript_type == "protein_coding")
+    )
+    logger.warning(
+        "This Gencode CDS interval filter does not filter by transcript! Please see the"
+        " documentation for more details to confirm it's being used as intended."
+    )
+    filter_expr = hl.is_defined(gencode_ht[t.locus])
+
+    if isinstance(t, hl.MatrixTable):
+        t = t.filter_rows(filter_expr)
+    else:
+        t = t.filter(filter_expr)
+
+    return t
+
+
 def remove_fields_from_constant(
     constant: List[str], fields_to_remove: List[str]
 ) -> List[str]:
     """
     Remove fields from a list and display any field(s) missing from the original list.
 
     :param constant: List of fields
@@ -398,15 +466,15 @@
         else:
             logger.info("%s missing from %s", field, constant)
 
     return constant
 
 
 def filter_x_nonpar(
-    t: Union[hl.Table, hl.MatrixTable]
+    t: Union[hl.Table, hl.MatrixTable],
 ) -> Union[hl.Table, hl.MatrixTable]:
     """
     Filter to loci that are in non-PAR regions on chromosome X.
 
     :param t: Input Table or MatrixTable.
     :return: Filtered Table or MatrixTable.
     """
@@ -424,15 +492,15 @@
         t.filter(non_par_expr)
         if isinstance(t, hl.Table)
         else t.filter_rows(non_par_expr)
     )
 
 
 def filter_y_nonpar(
-    t: Union[hl.Table, hl.MatrixTable]
+    t: Union[hl.Table, hl.MatrixTable],
 ) -> Union[hl.Table, hl.MatrixTable]:
     """
     Filter to loci that are in non-PAR regions on chromosome Y.
 
     :param t: Input Table or MatrixTable.
     :return: Filtered Table or MatrixTable.
     """
```

### Comparing `gnomad-0.7.1/gnomad/utils/gen_stats.py` & `gnomad-0.8.0/gnomad/utils/gen_stats.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/utils/intervals.py` & `gnomad-0.8.0/gnomad/utils/intervals.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/utils/liftover.py` & `gnomad-0.8.0/gnomad/utils/liftover.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 GRCH38_TO_GRCH37_CHAIN = "gs://hail-common/references/grch38_to_grch37.over.chain.gz"
 """
 Path to chain file required to lift data from GRCh38 to GRCh37.
 """
 
 
 def get_liftover_genome(
-    t: Union[hl.MatrixTable, hl.Table]
+    t: Union[hl.MatrixTable, hl.Table],
 ) -> Tuple[hl.genetics.ReferenceGenome, hl.genetics.ReferenceGenome]:
     """
     Infer reference genome build of input data and assume destination reference genome build.
 
     Adds liftover chain to source reference genome and sequence to destination reference genome.
     Returns tuple containing both reference genomes in preparation for liftover.
```

### Comparing `gnomad-0.7.1/gnomad/utils/plotting.py` & `gnomad-0.8.0/gnomad/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/utils/reference_genome.py` & `gnomad-0.8.0/gnomad/utils/reference_genome.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/utils/release.py` & `gnomad-0.8.0/gnomad/utils/release.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
 def make_faf_index_dict(
     faf_meta: List[Dict[str, str]],
     groups: List[str] = ["adj"],
-    pops: List[str] = POPS[CURRENT_MAJOR_RELEASE],
+    pops: List[str] = POPS[CURRENT_MAJOR_RELEASE]["exomes"],
     sexes: List[str] = SEXES,
     label_delimiter: str = "_",
 ) -> Dict[str, int]:
     """
     Create a look-up Dictionary for entries contained in the filter allele frequency annotation array.
 
     :param faf_meta: Global annotation containing the set of groupings for each element of the faf array
         (e.g., [{'group': 'adj'}, {'group': 'adj', 'pop': 'nfe'}])
     :param groups: List of sample groups [adj, raw]. Default is GROUPS
-    :param pops: List of sample global population names for gnomAD genomes. Default is POPS[CURRENT_MAJOR_RELEASE]
+    :param pops: List of sample global population names for gnomAD data type. Default is POPS[CURRENT_MAJOR_RELEASE]["exomes"].
     :param sexes: List of sample sexes used in VCF export. Default is SEXES
     :param label_delimiter: String used as delimiter when making group label combinations
     :return: Dictionary of faf annotation population groupings, where values are the corresponding 0-based indices for the
         groupings in the faf_meta array
     """
 
     def _get_index(label_groups):
@@ -53,15 +53,15 @@
     }
     return index_dict
 
 
 def make_freq_index_dict(
     freq_meta: List[Dict[str, str]],
     groups: List[str] = GROUPS,
-    pops: List[str] = POPS[CURRENT_MAJOR_RELEASE],
+    pops: List[str] = POPS[CURRENT_MAJOR_RELEASE]["exomes"],
     sexes: List[str] = SEXES,
     subsets: List[str] = SUBSETS[CURRENT_MAJOR_RELEASE],
     downsamplings: Optional[List[int]] = None,
     label_delimiter: str = "_",
 ) -> Dict[str, int]:
     """
     Create a look-up Dictionary for entries contained in the frequency annotation array.
@@ -69,15 +69,15 @@
     .. note:
 
         Downsampling groupings are only computed on 'adj'-filtered genotypes
 
     :param freq_meta: List containing the set of groupings for each element of the freq array
         (e.g., [{'group': 'adj'}, {'group': 'adj', 'pop': 'nfe'}])
     :param groups: List of sample groups [adj, raw]. Default is GROUPS
-    :param pops: List of sample global population names for gnomAD genomes. Default is POPS[CURRENT_MAJOR_RELEASE]
+    :param pops: List of sample global population names for gnomAD data type. Default is POPS[CURRENT_MAJOR_RELEASE]["exomes"].
     :param sexes: List of sample sexes used in VCF export. Default is SEXES
     :param subsets: List of sample subsets in dataset. Default is SUBSETS[CURRENT_MAJOR_RELEASE]
     :param downsamplings: List of downsampling cohort sizes present in global frequency array
     :param label_delimiter: String used as delimiter when making group label combinations
     :return: Dictionary keyed by the grouping combinations found in the frequency array, where values are the corresponding
         0-based indices for the groupings in the freq_meta array
     """
```

### Comparing `gnomad-0.7.1/gnomad/utils/slack.py` & `gnomad-0.8.0/gnomad/utils/slack.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/utils/vcf.py` & `gnomad-0.8.0/gnomad/utils/vcf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # noqa: D100
 
 import copy
 import itertools
 import logging
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 import hail as hl
 
 from gnomad.sample_qc.ancestry import POP_NAMES
 
 logging.basicConfig(format="%(levelname)s (%(name)s %(lineno)s): %(message)s")
 logger = logging.getLogger(__name__)
@@ -35,15 +35,18 @@
 """
 
 HISTS = ["gq_hist_alt", "gq_hist_all", "dp_hist_alt", "dp_hist_all", "ab_hist_alt"]
 """
 Quality histograms used in VCF export.
 """
 
-FAF_POPS = ["afr", "amr", "eas", "nfe", "sas"]
+FAF_POPS = {
+    "v3": ["afr", "amr", "eas", "nfe", "sas"],
+    "v4": ["afr", "amr", "eas", "mid", "nfe", "sas"],
+}
 """
 Global populations that are included in filtering allele frequency (faf) calculations. Used in VCF export.
 """
 
 SEXES = ["XX", "XY"]
 """
 Sample sexes used in VCF export.
@@ -100,14 +103,27 @@
 """
 Annotations about variant region type.
 
 .. note::
     decoy resource files do not currently exist for GRCh38/hg38.
 """
 
+JOINT_REGION_FLAG_FIELDS = [
+    "fail_interval_qc",
+    "outside_broad_capture_region",
+    "outside_ukb_capture_region",
+    "outside_broad_calling_region",
+    "outside_ukb_calling_region",
+    "not_called_in_exomes",
+    "not_called_in_genomes",
+]
+"""
+Annotations about variant region type that are specifically created for joint dataset of exomes and genomes from gnomAD v4.1.
+"""
+
 RF_FIELDS = [
     "rf_positive_label",
     "rf_negative_label",
     "rf_label",
     "rf_train",
     "rf_tp_probability",
 ]
@@ -320,14 +336,49 @@
         ),
     },
 }
 """
 Dictionary used during VCF export to export row (variant) annotations.
 """
 
+JOINT_REGION_FLAGS_INFO_DICT = {
+    "fail_interval_qc": {
+        "Description": (
+            "Less than 85 percent of samples meet 20X coverage if variant is in"
+            " autosomal or PAR regions or 10X coverage for non-PAR regions of"
+            " chromosomes X and Y."
+        )
+    },
+    "outside_ukb_capture_region": {
+        "Description": "Variant falls outside of the UK Biobank exome capture regions."
+    },
+    "outside_broad_capture_region": {
+        "Description": "Variant falls outside of the Broad exome capture regions."
+    },
+    "outside_ukb_calling_region": {
+        "Description": (
+            "Variant falls outside of the UK Biobank exome capture regions plus 150 bp"
+            " padding."
+        )
+    },
+    "outside_broad_calling_region": {
+        "Description": (
+            "Variant falls outside of the Broad exome capture regions plus 150 bp"
+            " padding."
+        )
+    },
+    "not_called_in_exomes": {
+        "Description": "Variant was not called in the gnomAD exomes."
+    },
+    "not_called_in_genomes": {
+        "Description": "Variant was not called in the gnomAD genomes."
+    },
+}
+
+
 IN_SILICO_ANNOTATIONS_INFO_DICT = {
     "cadd_raw_score": {
         "Number": "1",
         "Description": (
             "Raw CADD scores are interpretable as the extent to which the annotation"
             " profile for a given variant suggests that the variant is likely to be"
             " 'observed' (negative values) vs 'simulated' (positive values). Larger"
@@ -557,24 +608,35 @@
         if ft == hl.dtype("int64"):
             logger.warning(
                 "Coercing field info.%s from int64 to int32 for VCF output. Value"
                 " will be capped at int32 max value.",
                 f,
             )
             info_type_convert_expr.update(
-                {f: hl.int32(hl.min(2**31 - 1, ht.info[f]))}
+                {
+                    f: hl.or_missing(
+                        hl.is_defined(ht.info[f]),
+                        hl.int32(hl.min(2**31 - 1, ht.info[f])),
+                    )
+                }
             )
         elif ft == hl.dtype("array<int64>"):
             logger.warning(
                 "Coercing field info.%s from array<int64> to array<int32> for VCF"
                 " output. Array values will be capped at int32 max value.",
                 f,
             )
             info_type_convert_expr.update(
-                {f: ht.info[f].map(lambda x: hl.int32(hl.min(2**31 - 1, x)))}
+                {
+                    f: ht.info[f].map(
+                        lambda x: hl.or_missing(
+                            hl.is_defined(x), hl.int32(hl.min(2**31 - 1, x))
+                        )
+                    )
+                }
             )
 
     ht = ht.annotate(info=ht.info.annotate(**info_type_convert_expr))
 
     info_expr = {}
 
     # Make sure to pipe-delimit fields that need to.
@@ -665,15 +727,15 @@
     combo_dict: Dict[str, str],
     pop_names: Dict[str, str],
 ) -> str:
     """
     Programmatically generate text to populate the VCF header description for a given variant annotation with specific groupings and subset.
 
     For example, if preposition is "for", group_types is ["group", "pop", "sex"], and combo_fields is ["adj", "afr", "female"],
-    this function will return the string " for female samples of African-American/African ancestry".
+    this function will return the string " for female samples in the African-American/African genetic ancestry group".
 
     :param preposition: Relevant preposition to precede automatically generated text.
     :param combo_dict: Dict with grouping types as keys and values for grouping type as values. This function generates text for these values.
         Possible grouping types are: "group", "pop", "sex", and "subpop".
         Example input: {"pop": "afr", "sex": "female"}
     :param pop_names: Dict with global population names (keys) and population descriptions (values).
     :return: String with automatically generated description text for a given set of combo fields.
@@ -688,19 +750,23 @@
         header_text = header_text + " " + combo_dict["sex"]
 
     header_text = header_text + " samples"
 
     if "subpop" in combo_dict or "pop" in combo_dict:
         if "subpop" in combo_dict:
             header_text = (
-                header_text + f" of {pop_names[combo_dict['subpop']]} ancestry"
+                header_text
+                + f" in the {pop_names[combo_dict['subpop']]} genetic ancestry subgroup"
             )
 
         else:
-            header_text = header_text + f" of {pop_names[combo_dict['pop']]} ancestry"
+            header_text = (
+                header_text
+                + f" in the {pop_names[combo_dict['pop']]} genetic ancestry group"
+            )
 
     if "group" in combo_dict:
         if combo_dict["group"] == "raw":
             header_text = header_text + ", before removing low-confidence genotypes"
 
     return header_text
 
@@ -741,14 +807,17 @@
     label_delimiter: str = "_",
     bin_edges: Dict[str, str] = None,
     faf: bool = False,
     popmax: bool = False,
     grpmax: bool = False,
     fafmax: bool = False,
     callstats: bool = False,
+    freq_ctt: bool = False,
+    freq_cmh: bool = False,
+    freq_stat_union: bool = False,
     description_text: str = "",
     age_hist_distribution: str = None,
     sort_order: List[str] = SORT_ORDER,
 ) -> Dict[str, Dict[str, str]]:
     """
     Generate dictionary of Number and Description attributes of VCF INFO fields.
 
@@ -768,14 +837,18 @@
         e.g. "sex" or "pop", and value is a list of all possible values for that grouping (e.g. ["male", "female"] or ["afr", "nfe", "amr"]).
     :param label_delimiter: String to use as delimiter when making group label combinations.
     :param bin_edges: Dictionary keyed by annotation type, with values that reflect the bin edges corresponding to the annotation.
     :param faf: If True, use alternate logic to auto-populate dictionary values associated with filter allele frequency annotations.
     :param popmax: If True, use alternate logic to auto-populate dictionary values associated with popmax annotations.
     :param grpmax: If True, use alternate logic to auto-populate dictionary values associated with grpmax annotations.
     :param fafmax: If True, use alternate logic to auto-populate dictionary values associated with fafmax annotations.
+    :param callstats: If True, use alternate logic to auto-populate dictionary values associated with callstats annotations.
+    :param freq_ctt: If True, use alternate logic to auto-populate dictionary values associated with frequency contingency table test (CTT) annotations.
+    :param freq_cmh: If True, use alternate logic to auto-populate dictionary values associated with frequency Cochran-Mantel-Haenszel (CMH) annotations.
+    :param freq_stat_union: If True, use alternate logic to auto-populate dictionary values associated with the union of the contingency table and Cochran-Mantel-Haenszel tests.
     :param description_text: Optional text to append to the end of descriptions. Needs to start with a space if specified.
     :param str age_hist_distribution: Pipe-delimited string of overall age distribution.
     :param sort_order: List containing order to sort label group combinations. Default is SORT_ORDER.
     :return: Dictionary keyed by VCF INFO annotations, where values are dictionaries of Number and Description attributes.
     """
     if prefix != "":
         prefix = f"{prefix}{label_delimiter}"
@@ -920,78 +993,68 @@
 
     if fafmax:
         fafmax_dict = {
             f"{prefix}fafmax{label_delimiter}faf95{label_delimiter}max{suffix}": {
                 "Number": "A",
                 "Description": (
                     "Maximum filtering allele frequency (using Poisson 95% CI)"
-                    f" across genetic_ancestry groups{description_text}"
+                    f" across genetic ancestry groups{description_text}"
                 ),
             },
             f"{prefix}fafmax{label_delimiter}faf95{label_delimiter}max{label_delimiter}gen{label_delimiter}anc{suffix}": {
                 "Number": "A",
                 "Description": (
                     "Genetic ancestry group with maximum filtering allele"
                     f" frequency (using Poisson 95% CI){description_text}"
                 ),
             },
             f"{prefix}fafmax{label_delimiter}faf99{label_delimiter}max{suffix}": {
                 "Number": "A",
                 "Description": (
                     "Maximum filtering allele frequency (using Poisson 99% CI)"
-                    f" across genetic_ancestry groups{description_text}"
+                    f" across genetic ancestry groups{description_text}"
                 ),
             },
             f"{prefix}fafmax{label_delimiter}faf99{label_delimiter}max{label_delimiter}gen{label_delimiter}anc{suffix}": {
                 "Number": "A",
                 "Description": (
                     "Genetic ancestry group with maximum filtering allele"
                     f" frequency (using Poisson 99% CI){description_text}"
                 ),
             },
         }
-        if prefix == "joint_" or suffix == "_joint":
-            fafmax_dict.update(
-                {
-                    f"{prefix}fafmax{label_delimiter}data{label_delimiter}type{suffix}": {
-                        "Number": "A",
-                        "Description": (
-                            "Data type with maximum filtering allele frequency"
-                            f" {description_text}"
-                        ),
-                    },
-                }
-            )
 
         info_dict.update(fafmax_dict)
 
-    if callstats or faf:
+    if callstats or faf or freq_ctt:
         group_types = sorted(label_groups.keys(), key=lambda x: sort_order.index(x))
         combos = make_label_combos(label_groups, label_delimiter=label_delimiter)
 
         for combo in combos:
             combo_fields = combo.split(label_delimiter)
             group_dict = dict(zip(group_types, combo_fields))
 
             for_combo = make_combo_header_text("for", group_dict, pop_names)
             in_combo = make_combo_header_text("in", group_dict, pop_names)
 
             metrics = ["AC", "AN", "AF", "nhomalt", "faf95", "faf99"]
+            if freq_ctt:
+                metrics += ["CTT_odds_ratio", "CTT_p_value"]
             if prefix_before_metric:
                 metric_label_dict = {
                     metric: f"{prefix}{metric}{label_delimiter}{combo}{suffix}"
                     for metric in metrics
                 }
             else:
                 metric_label_dict = {
                     metric: f"{metric}{label_delimiter}{prefix}{combo}{suffix}"
                     for metric in metrics
                 }
 
-            if not faf:
+            if callstats:
                 combo_dict = {
                     metric_label_dict["AC"]: {
                         "Number": "A",
                         "Description": (
                             f"Alternate allele count{for_combo}{description_text}"
                         ),
                     },
@@ -1011,15 +1074,15 @@
                         "Number": "A",
                         "Description": (
                             "Count of homozygous"
                             f" individuals{in_combo}{description_text}"
                         ),
                     },
                 }
-            else:
+            elif faf:
                 if ("XX" in combo_fields) | ("XY" in combo_fields):
                     faf_description_text = (
                         description_text + " in non-PAR regions of sex chromosomes only"
                     )
                 else:
                     faf_description_text = description_text
                 combo_dict = {
@@ -1034,15 +1097,76 @@
                         "Number": "A",
                         "Description": (
                             "Filtering allele frequency (using Poisson 99%"
                             f" CI){for_combo}{faf_description_text}"
                         ),
                     },
                 }
+            else:
+                combo_dict = {
+                    metric_label_dict["CTT_odds_ratio"]: {
+                        "Number": "A",
+                        "Description": (
+                            "Odds ratio from from Hail's contingency_table_test with"
+                            " `min_cell_count=100` comparing allele frequencies"
+                            f" between exomes and genomes{for_combo}{description_text}"
+                        ),
+                    },
+                    metric_label_dict["CTT_p_value"]: {
+                        "Number": "A",
+                        "Description": (
+                            "P-value from Hail's contingency_table_test with"
+                            " `min_cell_count=100` comparing allele frequencies"
+                            f" between exomes and genomes{for_combo}{description_text}"
+                        ),
+                    },
+                }
             info_dict.update(combo_dict)
+    if freq_cmh:
+        cmh_dict = {
+            f"{prefix}CMH_chisq{suffix}": {
+                "Number": "A",
+                "Description": (
+                    "Chi-squared test statistic from the Cochran-Mantel-Haenszel test"
+                    " comparing allele frequencies between exomes and genomes"
+                    f" stratified by genetic ancestry group{description_text}"
+                ),
+            },
+            f"{prefix}CMH_p_value{suffix}": {
+                "Number": "A",
+                "Description": (
+                    "Odds ratio from Cochran-Mantel-Haenszel test comparing allele"
+                    " frequencies between exomes and genomes stratified by genetic"
+                    f" ancestry group{description_text}"
+                ),
+            },
+        }
+        info_dict.update(cmh_dict)
+    if freq_stat_union:
+        freq_stat_union_dict = {
+            f"{prefix}stat_union_p_value{suffix}": {
+                "Number": "A",
+                "Description": (
+                    f"p-value from the contingency table or Cochran-Mantel-Haenszel tests{description_text}"
+                ),
+            },
+            f"{prefix}stat_union_test_name{suffix}": {
+                "Number": "A",
+                "Description": (
+                    f"Name of the test, either contingency_table_test or cochran_mantel_haenszel_test, used to compare allele frequencies between exomes and genomes{description_text}"
+                ),
+            },
+            f"{prefix}stat_union_gen_ancs{suffix}": {
+                "Number": "A",
+                "Description": (
+                    f"List of genetic ancestry groups included in the test. If stat_union_test_name is contingency_table_test, the length of gen_ancs is one and if stat_union_test_name is 'cochran_mantel_haenszel_test', the length of 'gen_ancs' is greater than one{description_text}"
+                ),
+            },
+        }
+        info_dict.update(freq_stat_union_dict)
 
     return info_dict
 
 
 def add_as_info_dict(
     info_dict: Dict[str, Dict[str, str]] = INFO_DICT, as_fields: List[str] = AS_FIELDS
 ) -> Dict[str, Dict[str, str]]:
@@ -1136,83 +1260,128 @@
 
     return filter_dict
 
 
 def make_hist_bin_edges_expr(
     ht: hl.Table,
     hists: List[str] = HISTS,
+    ann_with_hists: Optional[str] = None,
     prefix: str = "",
     label_delimiter: str = "_",
     include_age_hists: bool = True,
 ) -> Dict[str, str]:
     """
     Create dictionaries containing variant histogram annotations and their associated bin edges, formatted into a string separated by pipe delimiters.
 
     :param ht: Table containing histogram variant annotations.
     :param hists: List of variant histogram annotations. Default is HISTS.
+    :param ann_with_hists: Name of row annotation containing histogram data. In exomes or
+        genomes release HT, `histograms` is a row, but in the joint release HT, it's
+        under the row of `exomes`, `genomes`, or `joint`.
     :param prefix: Prefix text for age histogram bin edges.  Default is empty string.
     :param label_delimiter: String used as delimiter between prefix and histogram annotation.
     :param include_age_hists: Include age histogram annotations.
-    :return: Dictionary keyed by histogram annotation name, with corresponding reformatted bin edges for values.
+    :return: Dictionary keyed by histogram annotation name, with corresponding
+        reformatted bin edges for values.
     """
     # Add underscore to prefix if it isn't empty
-    if prefix != "":
+    if prefix:
         prefix += label_delimiter
 
     edges_dict = {}
+
     if include_age_hists:
-        edges_dict.update(
-            {
-                f"{prefix}{call_type}": "|".join(
-                    map(
-                        lambda x: f"{x:.1f}",
-                        ht.head(1)
-                        .histograms.age_hists[f"age_hist_{call_type}"]
-                        .collect()[0]
-                        .bin_edges,
+        for call_type in ["het", "hom"]:
+            if ann_with_hists:
+                bin_edges = (
+                    ht.filter(
+                        hl.is_defined(
+                            ht[ann_with_hists]
+                            .histograms.age_hists[f"age_hist_{call_type}"]
+                            .bin_edges
+                        )
+                    )[ann_with_hists]
+                    .histograms.age_hists[f"age_hist_{call_type}"]
+                    .bin_edges.take(1)[0]
+                )
+            else:
+                bin_edges = (
+                    ht.filter(
+                        hl.is_defined(
+                            ht.histograms.age_hists[f"age_hist_{call_type}"].bin_edges
+                        )
                     )
+                    .histograms.age_hists[f"age_hist_{call_type}"]
+                    .bin_edges.take(1)[0]
+                )
+
+            if bin_edges:
+                edges_dict[f"{prefix}{call_type}"] = "|".join(
+                    map(lambda x: f"{x:.1f}", bin_edges)
                 )
-                for call_type in ["het", "hom"]
-            }
-        )
 
     for hist in hists:
         # Parse hists calculated on both raw and adj-filtered data
         for hist_type in [f"{prefix}raw_qual_hists", f"{prefix}qual_hists"]:
-            hist_name = hist
-            if "raw" in hist_type:
-                hist_name = f"{prefix}{hist}_raw"
-
-            edges_dict[hist_name] = "|".join(
-                map(
-                    lambda x: f"{x:.2f}" if "ab" in hist else str(int(x)),
-                    ht.head(1).histograms[hist_type][hist].collect()[0].bin_edges,
+            hist_name = hist if "raw" not in hist_type else f"{prefix}{hist}_raw"
+
+            if ann_with_hists:
+                bin_edges = (
+                    ht.filter(
+                        hl.is_defined(
+                            ht[ann_with_hists].histograms[hist_type][hist].bin_edges
+                        )
+                    )[ann_with_hists]
+                    .histograms[hist_type][hist]
+                    .bin_edges.take(1)[0]
+                )
+            else:
+                bin_edges = (
+                    ht.filter(hl.is_defined(ht.histograms[hist_type][hist].bin_edges))
+                    .histograms[hist_type][hist]
+                    .bin_edges.take(1)[0]
+                )
+            if bin_edges:
+                edges_dict[hist_name] = "|".join(
+                    map(
+                        lambda x: f"{x:.2f}" if "ab" in hist else str(int(x)), bin_edges
+                    )
                 )
-            )
 
     return edges_dict
 
 
 def make_hist_dict(
     bin_edges: Dict[str, Dict[str, str]],
     adj: bool,
     hist_metric_list: List[str] = HISTS,
     label_delimiter: str = "_",
     drop_n_smaller_larger: bool = False,
+    prefix: str = "",
+    suffix: str = "",
+    description_text: str = "",
 ) -> Dict[str, str]:
     """
     Generate dictionary of Number and Description attributes to be used in the VCF header, specifically for histogram annotations.
 
     :param bin_edges: Dictionary keyed by histogram annotation name, with corresponding string-reformatted bin edges for values.
     :param adj: Whether to create a header dict for raw or adj quality histograms.
     :param hist_metric_list: List of hists for which to build hist info dict
     :param label_delimiter: String used as delimiter in values stored in hist_metric_list.
     :param drop_n_smaller_larger: Whether to drop n_smaller and n_larger annotations from header dict. Default is False.
+    :param prefix: Prefix text for histogram annotations. Default is empty string.
+    :param suffix: Suffix text for histogram annotations. Default is empty string.
+    :param description_text: Optional text to append to the end of descriptions. Needs to start with a space if specified.
     :return: Dictionary keyed by VCF INFO annotations, where values are Dictionaries of Number and Description attributes.
     """
+    if prefix != "":
+        prefix = f"{prefix}{label_delimiter}"
+    if suffix != "":
+        suffix = f"{label_delimiter}{suffix}"
+
     header_hist_dict = {}
     for hist in hist_metric_list:
         # Get hists for both raw and adj data
         # Add "_raw" to quality histograms calculated on raw data
         if not adj:
             hist = f"{hist}_raw"
 
@@ -1222,49 +1391,52 @@
 
         if hist_fields[2] == "alt":
             hist_text = hist_text + " in heterozygous individuals"
         if adj:
             hist_text = hist_text + " calculated on high quality genotypes"
 
         hist_dict = {
-            f"{hist}_bin_freq": {
+            f"{prefix}{hist}_bin_freq{suffix}": {
                 "Number": "A",
-                "Description": f"Histogram for {hist_text}; bin edges are: {edges}",
+                "Description": (
+                    f"Histogram for {hist_text}{description_text}; bin edges are:"
+                    f" {edges}"
+                ),
             },
         }
         # These annotations are frequently zero and are dropped from gnomad
         # releases for most histograms.
         if not drop_n_smaller_larger:
             hist_dict.update(
                 {
-                    f"{hist}_n_smaller": {
+                    f"{prefix}{hist}_n_smaller{suffix}": {
                         "Number": "A",
                         "Description": (
                             f"Count of {hist_fields[0].upper()} values falling below"
-                            f" lowest histogram bin edge {hist_text}"
+                            f" lowest histogram bin edge {hist_text}{description_text}"
                         ),
                     },
-                    f"{hist}_n_larger": {
+                    f"{prefix}{hist}_n_larger{suffix}": {
                         "Number": "A",
                         "Description": (
                             f"Count of {hist_fields[0].upper()} values falling above"
-                            f" highest histogram bin edge {hist_text}"
+                            f" highest histogram bin edge {hist_text}{description_text}"
                         ),
                     },
                 }
             )
         # Only add n_larger for dp qual histograms.
         if "dp" in hist:
             hist_dict.update(
                 {
-                    f"{hist}_n_larger": {
+                    f"{prefix}{hist}_n_larger{suffix}": {
                         "Number": "A",
                         "Description": (
                             f"Count of {hist_fields[0].upper()} values falling above"
-                            f" highest histogram bin edge {hist_text}"
+                            f" highest histogram bin edge {hist_text}{description_text}"
                         ),
                     },
                 }
             )
 
         header_hist_dict.update(hist_dict)
```

### Comparing `gnomad-0.7.1/gnomad/utils/vep.py` & `gnomad-0.8.0/gnomad/utils/vep.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # noqa: D100
 
 import json
 import logging
 import os
 import subprocess
-from typing import List, Optional, Union
+from typing import Callable, List, Optional, Union
 
 import hail as hl
 
 from gnomad.resources.resource_utils import VersionedTableResource
 from gnomad.utils.filtering import combine_functions
 
 logging.basicConfig(format="%(levelname)s (%(name)s %(lineno)s): %(message)s")
@@ -77,14 +77,28 @@
 CSQ_ORDER = (
     CSQ_CODING_HIGH_IMPACT
     + CSQ_CODING_MEDIUM_IMPACT
     + CSQ_CODING_LOW_IMPACT
     + CSQ_NON_CODING
 )
 
+CSQ_CODING = CSQ_CODING_HIGH_IMPACT + CSQ_CODING_MEDIUM_IMPACT + CSQ_CODING_LOW_IMPACT
+"""
+Constant containing all coding consequences.
+"""
+
+CSQ_SPLICE = [
+    "splice_acceptor_variant",
+    "splice_donor_variant",
+    "splice_region_variant",
+]
+"""
+Constant containing all splice consequences.
+"""
+
 POSSIBLE_REFS = ("GRCh37", "GRCh38")
 """
 Constant containing supported references
 """
 
 VEP_CONFIG_PATH = "file:///vep_data/vep-gcloud.json"
 """
@@ -271,59 +285,70 @@
     )
 
 
 def process_consequences(
     mt: Union[hl.MatrixTable, hl.Table],
     vep_root: str = "vep",
     penalize_flags: bool = True,
+    csq_order: Optional[List[str]] = None,
+    has_polyphen: bool = True,
 ) -> Union[hl.MatrixTable, hl.Table]:
     """
     Add most_severe_consequence into [vep_root].transcript_consequences, and worst_csq_by_gene, any_lof into [vep_root].
 
     `most_severe_consequence` is the worst consequence for a transcript.
 
-    :param mt: Input MT
-    :param vep_root: Root for vep annotation (probably vep)
-    :param penalize_flags: Whether to penalize LOFTEE flagged variants, or treat them as equal to HC
-    :return: MT with better formatted consequences
-    """
-    csqs = hl.literal(CSQ_ORDER)
-    csq_dict = hl.literal(dict(zip(CSQ_ORDER, range(len(CSQ_ORDER)))))
+    .. note::
+        From gnomAD v4.0 on, the PolyPhen annotation was removed from the VEP Struct
+        in the release HTs. When using this function with gnomAD v4.0 or later,
+        set `has_polyphen` to False.
+
+    :param mt: Input Table or MatrixTable.
+    :param vep_root: Root for VEP annotation (probably "vep").
+    :param penalize_flags: Whether to penalize LOFTEE flagged variants, or treat them
+        as equal to HC.
+    :param csq_order: Optional list indicating the order of VEP consequences, sorted
+        from high to low impact. Default is None, which uses the value of the
+        `CSQ_ORDER` global.
+    :param has_polyphen: Whether the input VEP Struct has a PolyPhen annotation which
+        will be used to modify the consequence score. Default is True.
+    :return: MT with better formatted consequences.
+    """
+    if csq_order is None:
+        csq_order = CSQ_ORDER
+    csqs = hl.literal(csq_order)
+    csq_dict = hl.literal(dict(zip(csq_order, range(len(csq_order)))))
+
+    def _csq_score(tc: hl.expr.StructExpression) -> int:
+        return csq_dict[tc.most_severe_consequence]
+
+    flag_score = 500
+    no_flag_score = flag_score * (1 + penalize_flags)
+
+    def _csq_score_modifier(tc: hl.expr.StructExpression) -> float:
+        modifier = _csq_score(tc)
+        flag_condition = (tc.lof == "HC") & (tc.lof_flags != "")
+        modifier -= hl.if_else(flag_condition, flag_score, no_flag_score)
+        modifier -= hl.if_else(tc.lof == "OS", 20, 0)
+        modifier -= hl.if_else(tc.lof == "LC", 10, 0)
+        if has_polyphen:
+            modifier -= (
+                hl.case()
+                .when(tc.polyphen_prediction == "probably_damaging", 0.5)
+                .when(tc.polyphen_prediction == "possibly_damaging", 0.25)
+                .when(tc.polyphen_prediction == "benign", 0.1)
+                .default(0)
+            )
+        return modifier
 
     def find_worst_transcript_consequence(
         tcl: hl.expr.ArrayExpression,
     ) -> hl.expr.StructExpression:
-        """Get worst transcript_consequence from an array of em."""
-        flag_score = 500
-        no_flag_score = flag_score * (1 + penalize_flags)
-
-        def csq_score(tc):
-            return csq_dict[csqs.find(lambda x: x == tc.most_severe_consequence)]
-
         tcl = tcl.map(
-            lambda tc: tc.annotate(
-                csq_score=hl.case(missing_false=True)
-                .when(
-                    (tc.lof == "HC") & (tc.lof_flags == ""),
-                    csq_score(tc) - no_flag_score,
-                )
-                .when(
-                    (tc.lof == "HC") & (tc.lof_flags != ""), csq_score(tc) - flag_score
-                )
-                .when(tc.lof == "OS", csq_score(tc) - 20)
-                .when(tc.lof == "LC", csq_score(tc) - 10)
-                .when(
-                    tc.polyphen_prediction == "probably_damaging", csq_score(tc) - 0.5
-                )
-                .when(
-                    tc.polyphen_prediction == "possibly_damaging", csq_score(tc) - 0.25
-                )
-                .when(tc.polyphen_prediction == "benign", csq_score(tc) - 0.1)
-                .default(csq_score(tc))
-            )
+            lambda tc: tc.annotate(csq_score=_csq_score(tc) - _csq_score_modifier(tc))
         )
         return hl.or_missing(hl.len(tcl) > 0, hl.sorted(tcl, lambda x: x.csq_score)[0])
 
     transcript_csqs = mt[vep_root].transcript_consequences.map(
         add_most_severe_consequence_to_consequence
     )
 
@@ -419,14 +444,53 @@
     :return: Table or MatrixTable with VEP transcript consequences filtered.
     """
     return filter_vep_transcript_csqs(
         mt, vep_root, canonical=False, filter_empty_csq=filter_empty_csq
     )
 
 
+def filter_vep_to_gene_list(
+    t: Union[hl.MatrixTable, hl.Table],
+    genes: List[str],
+    match_by_gene_symbol: bool = False,
+    vep_root: str = "vep",
+    filter_empty_csq: bool = False,
+):
+    """
+    Filter VEP transcript consequences to those in a set of genes.
+
+    .. note::
+
+       Filtering to a list of genes by their 'gene_id' or 'gene_symbol' will filter to
+       all variants that are annotated to the gene, including
+       ['upstream_gene_variant', 'downstream_gene_variant'], which will not be the
+       same as if you filter to a gene interval. If you only want variants inside
+       certain gene boundaries and a faster filter, you can first filter `t` to an
+       interval list and then apply this filter.
+
+    :param t: Input Table or MatrixTable.
+    :param genes: Genes of interest to filter VEP transcript consequences to.
+    :param match_by_gene_symbol: Whether to match values in `genes` to VEP transcript
+        consequences by 'gene_symbol' instead of 'gene_id'. Default is False.
+    :param vep_root: Name used for VEP annotation. Default is 'vep'.
+    :param filter_empty_csq: Whether to filter out rows where 'transcript_consequences'
+        is empty. Default is False.
+    :return: Table or MatrixTable with VEP transcript consequences filtered.
+    """
+    return filter_vep_transcript_csqs(
+        t,
+        vep_root,
+        synonymous=False,
+        canonical=False,
+        filter_empty_csq=filter_empty_csq,
+        genes=genes,
+        match_by_gene_symbol=match_by_gene_symbol,
+    )
+
+
 def vep_struct_to_csq(
     vep_expr: hl.expr.StructExpression,
     csq_fields: str = VEP_CSQ_FIELDS[CURRENT_VEP_VERSION],
     has_polyphen_sift: bool = True,
 ) -> hl.expr.ArrayExpression:
     """
     Given a VEP Struct, returns and array of VEP VCF CSQ strings (one per consequence in the struct).
@@ -474,40 +538,54 @@
                 ),
                 "variant_class": vep_expr.variant_class,
             }
         )
 
         # Add exception for transcripts
         if feature_type == "Transcript":
-            fields.update(
-                {
-                    "canonical": hl.if_else(element.canonical == 1, "YES", ""),
-                    "ensp": element.protein_id,
-                    "gene": element.gene_id,
-                    "symbol": element.gene_symbol,
-                    "symbol_source": element.gene_symbol_source,
-                    "cdna_position": hl.str(element.cdna_start) + hl.if_else(
-                        element.cdna_start == element.cdna_end,
-                        "",
-                        "-" + hl.str(element.cdna_end),
-                    ),
-                    "cds_position": hl.str(element.cds_start) + hl.if_else(
-                        element.cds_start == element.cds_end,
-                        "",
-                        "-" + hl.str(element.cds_end),
-                    ),
-                    "mirna": hl.delimit(element.mirna, "&"),
-                    "protein_position": hl.str(element.protein_start) + hl.if_else(
-                        element.protein_start == element.protein_end,
-                        "",
-                        "-" + hl.str(element.protein_end),
-                    ),
-                    "uniprot_isoform": hl.delimit(element.uniprot_isoform, "&"),
-                }
-            )
+            transcript_dict = {
+                "canonical": hl.if_else(element.canonical == 1, "YES", ""),
+                "ensp": element.protein_id,
+                "gene": element.gene_id,
+                "symbol": element.gene_symbol,
+                "symbol_source": element.gene_symbol_source,
+                "cdna_position": hl.str(element.cdna_start)
+                + hl.if_else(
+                    element.cdna_start == element.cdna_end,
+                    "",
+                    "-" + hl.str(element.cdna_end),
+                ),
+                "cds_position": hl.str(element.cds_start)
+                + hl.if_else(
+                    element.cds_start == element.cds_end,
+                    "",
+                    "-" + hl.str(element.cds_end),
+                ),
+                "mirna": hl.delimit(element.mirna, "&") if "mirna" in element else None,
+                "protein_position": hl.str(element.protein_start)
+                + hl.if_else(
+                    element.protein_start == element.protein_end,
+                    "",
+                    "-" + hl.str(element.protein_end),
+                ),
+                "uniprot_isoform": (
+                    hl.delimit(element.uniprot_isoform, "&")
+                    if "uniprot_isoform" in element
+                    else None
+                ),
+            }
+            # Retain transcript dict updates only for fields that exist in the csq
+            # fields.
+            transcript_dict = {
+                k: v
+                for k, v in transcript_dict.items()
+                if k in [x.lower() for x in csq_fields.split("|")]
+            }
+            fields.update(transcript_dict)
+
             if has_polyphen_sift:
                 fields.update(
                     {
                         "sift": (
                             element.sift_prediction
                             + "("
                             + hl.format("%.3f", element.sift_score)
@@ -526,17 +604,18 @@
                     "domains": hl.delimit(
                         element.domains.map(lambda d: d.db + ":" + d.name), "&"
                     ),
                 }
             )
         elif feature_type == "MotifFeature":
             fields["motif_score_change"] = hl.format("%.3f", element.motif_score_change)
-            fields["transcription_factors"] = hl.delimit(
-                element.transcription_factors, "&"
-            )
+            if "transcription_factors" in element:
+                fields["transcription_factors"] = hl.delimit(
+                    element.transcription_factors, "&"
+                )
 
         return hl.delimit(
             [hl.or_else(hl.str(fields.get(f, "")), "") for f in _csq_fields], "|"
         )
 
     csq = hl.empty_array(hl.tstr)
     for feature_field, feature_type in [
@@ -638,47 +717,103 @@
     t: Union[hl.Table, hl.MatrixTable],
     vep_root: str = "vep",
     synonymous: bool = True,
     canonical: bool = True,
     mane_select: bool = False,
     filter_empty_csq: bool = True,
     ensembl_only: bool = True,
+    protein_coding: bool = False,
+    csqs: List[str] = None,
+    keep_csqs: bool = True,
+    genes: Optional[List[str]] = None,
+    keep_genes: bool = True,
+    match_by_gene_symbol: bool = False,
+    additional_filtering_criteria: Optional[List[Callable]] = None,
 ) -> Union[hl.Table, hl.MatrixTable]:
     """
     Filter VEP transcript consequences based on specified criteria, and optionally filter to variants where transcript consequences is not empty after filtering.
 
-    Transcript consequences can be filtered to those where 'most_severe_consequence' is 'synonymous_variant' and/or the transcript is the canonical transcript,
-    if the `synonymous` and `canonical` parameter are set to True, respectively.
-
-    If `filter_empty_csq` parameter is set to True, the Table/MatrixTable is filtered to variants where 'transcript_consequences' within the VEP annotation
-    is not empty after the specified filtering criteria is applied.
+    Transcript consequences can be filtered to those where 'most_severe_consequence' is
+    'synonymous_variant' and/or the transcript is the canonical transcript, if the
+    `synonymous` and `canonical` parameter are set to True, respectively.
+
+    If `filter_empty_csq` parameter is set to True, the Table/MatrixTable is filtered
+    to variants where 'transcript_consequences' within the VEP annotation is not empty
+    after the specified filtering criteria is applied.
 
     :param t: Input Table or MatrixTable.
     :param vep_root: Name used for VEP annotation. Default is 'vep'.
-    :param synonymous: Whether to filter to variants where the most severe consequence is 'synonymous_variant'. Default is True.
+    :param synonymous: Whether to filter to variants where the most severe consequence
+        is 'synonymous_variant'. Default is True.
     :param canonical: Whether to filter to only canonical transcripts. Default is True.
-    :param mane_select: Whether to filter to only MANE Select transcripts. Default is False.
-    :param filter_empty_csq: Whether to filter out rows where 'transcript_consequences' is empty, after filtering 'transcript_consequences' to the specified criteria. Default is True.
-    :param ensembl_only: Whether to filter to only Ensembl transcipts. This option is useful for deduplicating transcripts that are the same between RefSeq and Emsembl. Default is True.
+    :param mane_select: Whether to filter to only MANE Select transcripts. Default is
+        False.
+    :param filter_empty_csq: Whether to filter out rows where 'transcript_consequences'
+        is empty, after filtering 'transcript_consequences' to the specified criteria.
+        Default is True.
+    :param ensembl_only: Whether to filter to only Ensembl transcripts. This option is
+        useful for deduplicating transcripts that are the same between RefSeq and
+        Emsembl. Default is True.
+    :param protein_coding: Whether to filter to only protein-coding transcripts.
+        Default is False.
+    :param csqs: Optional list of consequence terms to filter to. Transcript
+        consequences are filtered to those where 'most_severe_consequence' is in the
+        list of consequence terms `csqs`. Default is None.
+    :param keep_csqs: Whether to keep transcript consequences that are in `csqs`. If
+        set to False, transcript consequences that are in `csqs` will be removed.
+        Default is True.
+    :param genes: Optional list of genes to filter VEP transcript consequences to.
+        Default is None.
+    :param keep_genes: Whether to keep transcript consequences that are in `genes`. If
+        set to False, transcript consequences that are in `genes` will be removed.
+        Default is True.
+    :param match_by_gene_symbol: Whether to match values in `genes` to VEP transcript
+        consequences by 'gene_symbol' instead of 'gene_id'. Default is False.
+    :param additional_filtering_criteria: Optional list of additional filtering
+        criteria to apply to the VEP transcript consequences.
     :return: Table or MatrixTable filtered to specified criteria.
     """
     if not synonymous and not (canonical or mane_select) and not filter_empty_csq:
         logger.warning("No changes have been made to input Table/MatrixTable!")
         return t
 
     transcript_csqs = t[vep_root].transcript_consequences
     criteria = [lambda csq: True]
     if synonymous:
-        criteria.append(lambda csq: csq.most_severe_consequence == "synonymous_variant")
+        logger.info("Filtering to most severe consequence of synonymous_variant...")
+        csqs = ["synonymous_variant"]
+    if csqs is not None:
+        csqs = hl.literal(csqs)
+        if keep_csqs:
+            criteria.append(lambda csq: csqs.contains(csq.most_severe_consequence))
+        else:
+            criteria.append(lambda csq: ~csqs.contains(csq.most_severe_consequence))
     if canonical:
+        logger.info("Filtering to canonical transcripts")
         criteria.append(lambda csq: csq.canonical == 1)
     if mane_select:
+        logger.info("Filtering to MANE Select transcripts...")
         criteria.append(lambda csq: hl.is_defined(csq.mane_select))
     if ensembl_only:
+        logger.info("Filtering to Ensembl transcripts...")
         criteria.append(lambda csq: csq.transcript_id.startswith("ENST"))
+    if protein_coding:
+        logger.info("Filtering to protein coding transcripts...")
+        criteria.append(lambda csq: csq.biotype == "protein_coding")
+    if genes is not None:
+        logger.info("Filtering to genes of interest...")
+        genes = hl.literal(genes)
+        gene_field = "gene_symbol" if match_by_gene_symbol else "gene_id"
+        if keep_genes:
+            criteria.append(lambda csq: genes.contains(csq[gene_field]))
+        else:
+            criteria.append(lambda csq: ~genes.contains(csq[gene_field]))
+    if additional_filtering_criteria is not None:
+        logger.info("Filtering to variants with additional criteria...")
+        criteria = criteria + additional_filtering_criteria
 
     transcript_csqs = transcript_csqs.filter(lambda x: combine_functions(criteria, x))
     is_mt = isinstance(t, hl.MatrixTable)
     vep_data = {vep_root: t[vep_root].annotate(transcript_consequences=transcript_csqs)}
     t = t.annotate_rows(**vep_data) if is_mt else t.annotate(**vep_data)
 
     if filter_empty_csq:
```

### Comparing `gnomad-0.7.1/gnomad/variant_qc/evaluation.py` & `gnomad-0.8.0/gnomad/variant_qc/evaluation.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/variant_qc/ld.py` & `gnomad-0.8.0/gnomad/variant_qc/ld.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/variant_qc/pipeline.py` & `gnomad-0.8.0/gnomad/variant_qc/pipeline.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/variant_qc/random_forest.py` & `gnomad-0.8.0/gnomad/variant_qc/random_forest.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad/variant_qc/training.py` & `gnomad-0.8.0/gnomad/variant_qc/training.py`

 * *Files identical despite different names*

### Comparing `gnomad-0.7.1/gnomad.egg-info/PKG-INFO` & `gnomad-0.8.0/gnomad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnomad
-Version: 0.7.1
+Version: 0.8.0
 Summary: Hail utilities for the Genome Aggregation Database
 Home-page: https://github.com/broadinstitute/gnomad_methods
 Author: The Genome Aggregation Database
 Author-email: gnomad@broadinstitute.org
 Project-URL: Documentation, https://broadinstitute.github.io/gnomad_methods/
 Project-URL: Source Code, https://github.com/broadinstitute/gnomad_methods
 Project-URL: Issues, https://github.com/broadinstitute/gnomad_methods/issues
```

### Comparing `gnomad-0.7.1/gnomad.egg-info/SOURCES.txt` & `gnomad-0.8.0/gnomad.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 gnomad/utils/intervals.py
 gnomad/utils/liftover.py
 gnomad/utils/plotting.py
 gnomad/utils/reference_genome.py
 gnomad/utils/release.py
 gnomad/utils/slack.py
 gnomad/utils/sparse_mt.py
+gnomad/utils/transcript_annotation.py
 gnomad/utils/vcf.py
 gnomad/utils/vep.py
 gnomad/variant_qc/__init__.py
 gnomad/variant_qc/evaluation.py
 gnomad/variant_qc/ld.py
 gnomad/variant_qc/pipeline.py
 gnomad/variant_qc/random_forest.py
```

### Comparing `gnomad-0.7.1/setup.py` & `gnomad-0.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     for req in (line.strip() for line in requirements_file):
         if req != "hail":
             install_requires.append(req)
 
 
 setuptools.setup(
     name="gnomad",
-    version="0.7.1",
+    version="0.8.0",
     author="The Genome Aggregation Database",
     author_email="gnomad@broadinstitute.org",
     description="Hail utilities for the Genome Aggregation Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/broadinstitute/gnomad_methods",
     packages=setuptools.find_namespace_packages(include=["gnomad.*"]),
```

