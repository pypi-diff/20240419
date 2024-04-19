# Comparing `tmp/dvcx-0.74.0.tar.gz` & `tmp/dvcx-0.75.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.74.0.tar", last modified: Tue Apr 16 08:37:58 2024, max compression
+gzip compressed data, was "dvcx-0.75.0.tar", last modified: Fri Apr 19 09:47:08 2024, max compression
```

## Comparing `dvcx-0.74.0.tar` & `dvcx-0.75.0.tar`

### file list

```diff
@@ -1,228 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.024024 dvcx-0.74.0/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-16 08:37:52.000000 dvcx-0.74.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 08:37:52.000000 dvcx-0.74.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.980024 dvcx-0.74.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.980024 dvcx-0.74.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.980024 dvcx-0.74.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 08:37:52.000000 dvcx-0.74.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-16 08:37:52.000000 dvcx-0.74.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-16 08:37:52.000000 dvcx-0.74.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.980024 dvcx-0.74.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 08:37:52.000000 dvcx-0.74.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 08:37:52.000000 dvcx-0.74.0/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-16 08:37:52.000000 dvcx-0.74.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-16 08:37:52.000000 dvcx-0.74.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-16 08:37:52.000000 dvcx-0.74.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.984024 dvcx-0.74.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-16 08:37:52.000000 dvcx-0.74.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-16 08:37:52.000000 dvcx-0.74.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-16 08:37:52.000000 dvcx-0.74.0/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-16 08:37:58.024024 dvcx-0.74.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-16 08:37:52.000000 dvcx-0.74.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.984024 dvcx-0.74.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-16 08:37:52.000000 dvcx-0.74.0/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.984024 dvcx-0.74.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.988024 dvcx-0.74.0/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.988024 dvcx-0.74.0/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.988024 dvcx-0.74.0/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 08:37:52.000000 dvcx-0.74.0/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-16 08:37:52.000000 dvcx-0.74.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-16 08:37:52.000000 dvcx-0.74.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:37:58.024024 dvcx-0.74.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.976024 dvcx-0.74.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.992024 dvcx-0.74.0/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.996024 dvcx-0.74.0/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72831 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    30133 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:57.996024 dvcx-0.74.0/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.000024 dvcx-0.74.0/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    44816 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30556 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    33008 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    15559 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.000024 dvcx-0.74.0/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/param.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.004024 dvcx-0.74.0/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    57791 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.004024 dvcx-0.74.0/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.004024 dvcx-0.74.0/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.004024 dvcx-0.74.0/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.004024 dvcx-0.74.0/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.008024 dvcx-0.74.0/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-16 08:37:52.000000 dvcx-0.74.0/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.016024 dvcx-0.74.0/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 08:37:57.000000 dvcx-0.74.0/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.008024 dvcx-0.74.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.008024 dvcx-0.74.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.008024 dvcx-0.74.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35621 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   114379 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/func/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/test_cli_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.016024 dvcx-0.74.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.016024 dvcx-0.74.0/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.016024 dvcx-0.74.0/tests/unit/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:37:58.016024 dvcx-0.74.0/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-16 08:37:52.000000 dvcx-0.74.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.154194 dvcx-0.75.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-19 09:47:03.000000 dvcx-0.75.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 09:47:03.000000 dvcx-0.75.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.110194 dvcx-0.75.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.110194 dvcx-0.75.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-19 09:47:03.000000 dvcx-0.75.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-19 09:47:03.000000 dvcx-0.75.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-19 09:47:03.000000 dvcx-0.75.0/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 09:47:03.000000 dvcx-0.75.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-19 09:47:03.000000 dvcx-0.75.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.110194 dvcx-0.75.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-19 09:47:03.000000 dvcx-0.75.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 09:47:03.000000 dvcx-0.75.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-19 09:47:03.000000 dvcx-0.75.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-19 09:47:03.000000 dvcx-0.75.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-19 09:47:03.000000 dvcx-0.75.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-19 09:47:03.000000 dvcx-0.75.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.110194 dvcx-0.75.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 09:47:03.000000 dvcx-0.75.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-19 09:47:03.000000 dvcx-0.75.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-19 09:47:03.000000 dvcx-0.75.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-19 09:47:03.000000 dvcx-0.75.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-19 09:47:03.000000 dvcx-0.75.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.114194 dvcx-0.75.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-19 09:47:03.000000 dvcx-0.75.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-19 09:47:03.000000 dvcx-0.75.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-19 09:47:03.000000 dvcx-0.75.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-19 09:47:08.154194 dvcx-0.75.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-19 09:47:03.000000 dvcx-0.75.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.114194 dvcx-0.75.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-19 09:47:03.000000 dvcx-0.75.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.114194 dvcx-0.75.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.118194 dvcx-0.75.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.118194 dvcx-0.75.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.118194 dvcx-0.75.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 09:47:03.000000 dvcx-0.75.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-19 09:47:03.000000 dvcx-0.75.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-19 09:47:03.000000 dvcx-0.75.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:47:08.154194 dvcx-0.75.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.106194 dvcx-0.75.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.122194 dvcx-0.75.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-19 09:47:07.000000 dvcx-0.75.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.126194 dvcx-0.75.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71363 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/catalog/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30133 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.126194 dvcx-0.75.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.126194 dvcx-0.75.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44816 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30556 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33020 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.130194 dvcx-0.75.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.134194 dvcx-0.75.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57821 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.134194 dvcx-0.75.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.134194 dvcx-0.75.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.134194 dvcx-0.75.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.138194 dvcx-0.75.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.138194 dvcx-0.75.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-19 09:47:03.000000 dvcx-0.75.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.150194 dvcx-0.75.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-19 09:47:08.000000 dvcx-0.75.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-19 09:47:08.000000 dvcx-0.75.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:47:08.000000 dvcx-0.75.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 09:47:08.000000 dvcx-0.75.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-19 09:47:08.000000 dvcx-0.75.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 09:47:08.000000 dvcx-0.75.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.138194 dvcx-0.75.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.138194 dvcx-0.75.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.142194 dvcx-0.75.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34442 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112414 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/func/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/test_cli_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.146194 dvcx-0.75.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.146194 dvcx-0.75.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.146194 dvcx-0.75.0/tests/unit/sql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:47:08.146194 dvcx-0.75.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_catalog_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-19 09:47:03.000000 dvcx-0.75.0/tests/utils.py
```

### Comparing `dvcx-0.74.0/.cruft.json` & `dvcx-0.75.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.75.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.75.0/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/.github/workflows/benchmarks.yml` & `dvcx-0.75.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/.github/workflows/release.yml` & `dvcx-0.75.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/.github/workflows/tests.yml` & `dvcx-0.75.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/.gitignore` & `dvcx-0.75.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/.pre-commit-config.yaml` & `dvcx-0.75.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/CODE_OF_CONDUCT.rst` & `dvcx-0.75.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/CONTRIBUTING.rst` & `dvcx-0.75.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/LICENSE` & `dvcx-0.75.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/LICENSES/Apache-2.0.txt` & `dvcx-0.75.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/LICENSES/BSD-3-Clause.txt` & `dvcx-0.75.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/LICENSES/Python-2.0.txt` & `dvcx-0.75.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/PKG-INFO` & `dvcx-0.75.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.74.0
+Version: 0.75.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.74.0/README.rst` & `dvcx-0.75.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/docs/udfs.md` & `dvcx-0.75.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/blip2_image_desc_lib.py` & `dvcx-0.75.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/clip.py` & `dvcx-0.75.0/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/common_sql_functions.py` & `dvcx-0.75.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/dir_expansion.py` & `dvcx-0.75.0/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/hf_pipeline.py` & `dvcx-0.75.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/llava2_image_desc_lib.py` & `dvcx-0.75.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/loader.py` & `dvcx-0.75.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/neurips/README` & `dvcx-0.75.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/neurips/distance_to_query.py` & `dvcx-0.75.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/neurips/llm_chat.py` & `dvcx-0.75.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/neurips/single_query.py` & `dvcx-0.75.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/neurips/text_loaders.py` & `dvcx-0.75.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/openai_image_desc_lib.py` & `dvcx-0.75.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/openimage-detect.py` & `dvcx-0.75.0/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/pose_detection.py` & `dvcx-0.75.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/torch-loader.py` & `dvcx-0.75.0/examples/torch-loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 if __name__ == "__main__":
     q = DatasetQuery(STORAGE).filter(C.name.glob("*.jpg")).add_signals(extract_label)
 
     train_loader = DataLoader(
         q.to_pytorch(Image(), Label("label", CLASSES), cache=True, transform=transform),
         batch_size=16,
+        num_workers=2,
     )
 
     model = CNN()
     criterion = nn.CrossEntropyLoss()
     optimizer = optim.Adam(model.parameters(), lr=0.001)
 
     # Train the model
```

### Comparing `dvcx-0.74.0/examples/udfs/batching.py` & `dvcx-0.75.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/udfs/image_transformation.py` & `dvcx-0.75.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/udfs/parallel.py` & `dvcx-0.75.0/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/udfs/simple.py` & `dvcx-0.75.0/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/udfs/stateful.py` & `dvcx-0.75.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/udfs/stateful_similarity.py` & `dvcx-0.75.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/unstructured-text.py` & `dvcx-0.75.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/wds.py` & `dvcx-0.75.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/wds_filtered.py` & `dvcx-0.75.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/wds_meta.py` & `dvcx-0.75.0/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/zalando/zalando_clip.py` & `dvcx-0.75.0/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.75.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/noxfile.py` & `dvcx-0.75.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/pyproject.toml` & `dvcx-0.75.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/asyn.py` & `dvcx-0.75.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/cache.py` & `dvcx-0.75.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/catalog/catalog.py` & `dvcx-0.75.0/src/dvcx/catalog/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,15 @@
 
 from dvcx.cache import DVCXCache
 from dvcx.client import Client
 from dvcx.config import get_remote_config, read_config
 from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
 from dvcx.dataset import (
     DATASET_PREFIX,
-    QUERY_DATASET_NAME_PREFIX,
-    TEMP_DATASET_NAME_PREFIX,
+    QUERY_DATASET_PREFIX,
     DatasetDependency,
     DatasetRecord,
     DatasetRow,
     DatasetStats,
     create_dataset_uri,
     parse_dataset_uri,
 )
@@ -604,31 +603,15 @@
             result.id_generator = None
             result.metastore = None
             result.warehouse = None
         return result
 
     @classmethod
     def generate_query_dataset_name(cls) -> str:
-        return f"{QUERY_DATASET_NAME_PREFIX}_{uuid4().hex}"
-
-    @classmethod
-    def generate_temp_dataset_name(cls, query_session_uuid: str) -> str:
-        """
-        Temp or ephemeral datasets are the ones created without specified name
-        with DatasetQuery, e.g ds = DatasetQuery(path="s3://ldb-public").save().
-        They are useful for optimization purposes and should be removed when
-        query ends.
-        Temp dataset has specific name that starts with ds_temp keyword and then
-        follows by unique query uuid. Finally it ends with unique uuid to make
-        sure it's generally unique. Examples:
-        ds_temp_afcc3350-8dee-4342-9a84-1556fc0fae45_03c071eb-6728-4192-b7dd-624b4148e8b4
-        ds_temp_2801235b-63c7-4c5a-9555-4b962d2a5dff
-        """
-
-        return f"{TEMP_DATASET_NAME_PREFIX}{query_session_uuid}_{uuid4().hex}"
+        return f"{QUERY_DATASET_PREFIX}_{uuid4().hex}"
 
     def compile_query_script(self, script: str, save=False) -> str:
         wrapper_function = "query_wrapper_print"
         if save:
             wrapper_function = "query_wrapper_save"
 
         code_ast = ast.parse(script)
@@ -1149,25 +1132,14 @@
         ensure that they are cleaned up as soon as they are no longer
         needed. When running the same `DatasetQuery` multiple times we
         may use the same temporary table names.
         """
         self.warehouse.cleanup_temp_tables(names)
         self.id_generator.delete_uris(names)
 
-    def cleanup_temp_datasets(self, query_session_uuid: Optional[str] = None) -> None:
-        """
-        This method removes temporary datasets for specific query session uuid
-        or in general
-        """
-        prefix = TEMP_DATASET_NAME_PREFIX
-        if query_session_uuid:
-            prefix = f"{prefix}{query_session_uuid}"
-        for dataset in self.metastore.list_datasets_by_prefix(prefix):
-            self.remove_dataset(dataset.name, force=True)
-
     def create_dataset_from_sources(
         self,
         name: str,
         sources: list[str],
         client_config=None,
         recursive=False,
     ) -> DatasetRecord:
@@ -1818,25 +1790,23 @@
             startupinfo.lpAttributeList["handle_list"].append(handle)
             kwargs: dict[str, Any] = {"startupinfo": startupinfo}
         else:
             handle = w
             kwargs = {"pass_fds": [w]}
 
         envs = dict(envs or os.environ)
-        query_session_uuid = uuid4().hex
         envs.update(
             {
                 "DVCX_QUERY_PREVIEW_ARGS": json.dumps(
                     {
                         "limit": preview_limit,
                         "offset": preview_offset,
                         "columns": preview_columns,
                     }
                 ),
-                "DVCX_QUERY_SESSION_UUID": query_session_uuid,
                 "PYTHONUNBUFFERED": "1",
                 "DVCX_OUTPUT_FD": str(handle),
             },
         )
 
         python_executable = python_executable or sys.executable
         with subprocess.Popen(
@@ -1866,15 +1836,14 @@
         except ValueError:
             response = {}
         records = response.get("preview", None)
         dataset_name, dataset_version = response.get("dataset", (None, None))
 
         script_output = "".join(lines)
 
-        self.cleanup_temp_datasets(query_session_uuid)
         if proc.returncode:
             if proc.returncode == QUERY_SCRIPT_CANCELED_EXIT_CODE:
                 raise QueryScriptCancelError(
                     "Query script was canceled by user",
                     return_code=proc.returncode,
                     output=script_output,
                 )
```

### Comparing `dvcx-0.74.0/src/dvcx/catalog/datasource.py` & `dvcx-0.75.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/catalog/formats.py` & `dvcx-0.75.0/src/dvcx/catalog/formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/catalog/loader.py` & `dvcx-0.75.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/cli.py` & `dvcx-0.75.0/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/cli_utils.py` & `dvcx-0.75.0/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/client/azure.py` & `dvcx-0.75.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/client/fileslice.py` & `dvcx-0.75.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/client/fsspec.py` & `dvcx-0.75.0/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/client/gcs.py` & `dvcx-0.75.0/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/client/local.py` & `dvcx-0.75.0/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/client/s3.py` & `dvcx-0.75.0/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/config.py` & `dvcx-0.75.0/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/data_storage/db_engine.py` & `dvcx-0.75.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/data_storage/id_generator.py` & `dvcx-0.75.0/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/data_storage/metastore.py` & `dvcx-0.75.0/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/data_storage/schema.py` & `dvcx-0.75.0/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/data_storage/serializer.py` & `dvcx-0.75.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/data_storage/sqlite.py` & `dvcx-0.75.0/src/dvcx/data_storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/data_storage/warehouse.py` & `dvcx-0.75.0/src/dvcx/data_storage/warehouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
         # reset query order by and apply new order by id
         paginated_query = query.order_by(None).order_by(*ordering).limit(page_size)
 
         offset = 0
         num_yielded = 0
         while True:
-            if limit:
+            if limit is not None:
                 limit -= num_yielded
                 if limit == 0:
                     break
                 if limit < page_size:
                     paginated_query = paginated_query.limit(None).limit(limit)
 
             results = self.db.execute(paginated_query.offset(offset))
```

### Comparing `dvcx-0.74.0/src/dvcx/dataset.py` & `dvcx-0.75.0/src/dvcx/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,15 @@
     from dvcx.storage import StorageURI
 
 T = TypeVar("T", bound="DatasetRecord")
 V = TypeVar("V", bound="DatasetVersion")
 DD = TypeVar("DD", bound="DatasetDependency")
 
 DATASET_PREFIX = "ds://"
-QUERY_DATASET_NAME_PREFIX = "ds_query_"
-TEMP_DATASET_NAME_PREFIX = "ds_temp_"
+QUERY_DATASET_PREFIX = "query_"
 
 
 def parse_dataset_uri(uri: str) -> tuple[str, Optional[int]]:
     """
     Parse dataser uri to extract name and version out of it (if version is defined)
     Example:
         Input: ds://zalando@v3
```

### Comparing `dvcx-0.74.0/src/dvcx/error.py` & `dvcx-0.75.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/cached_stream.py` & `dvcx-0.75.0/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/dataset.py` & `dvcx-0.75.0/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/feature.py` & `dvcx-0.75.0/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/feature_udf.py` & `dvcx-0.75.0/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/file.py` & `dvcx-0.75.0/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.75.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.75.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.75.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/image_transform.py` & `dvcx-0.75.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.75.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/param.py` & `dvcx-0.75.0/src/dvcx/lib/param.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,58 @@
-from typing import TYPE_CHECKING, Any
+from collections.abc import Iterable
+from typing import TYPE_CHECKING, Callable, Optional
 
 import attrs
 
 from dvcx.query.schema import Object, UDFParameter
 
 if TYPE_CHECKING:
     from dvcx.catalog import Catalog
     from dvcx.dataset import DatasetRow as Row
 
 
-def Image(formats=None, mode="RGB", size=None, transform=None):  # noqa: N802
-    try:
-        import PIL.Image
-    except ImportError as exc:
-        raise ImportError(
-            "Missing dependency Pillow for computer vision:\n"
-            "To install run:\n\n"
-            "  pip install 'dvcx[cv]'\n"
-        ) from exc
-
-    def load_img(raw):
-        img = PIL.Image.open(raw, formats=formats).convert(mode)
-        if size:
-            img = img.resize(size)
-        if transform:
-            img = transform(img)
-        return img
+class Image(Object):
+    def __init__(
+        self,
+        formats: Optional[Iterable[str]] = None,
+        mode: str = "RGB",
+        size: Optional[tuple[int, int]] = None,
+        transform: Optional[Callable] = None,
+    ):
+        """
+        Return image from file object, optionally resized/transformed.
+
+        Args:
+            formats (Iterable[str]): PIL.Image formats.
+            mode (str): PIL.Image mode.
+            size (tuple[int, int]): Size in (width, height) pixels for resizing.
+            transform (Callable): Torchvision v1 or other transform to apply.
+        """
+        self.formats = formats
+        self.mode = mode
+        self.size = size
+        self.transform = transform
+        super().__init__(reader=self.load_img)
 
-    return Object(load_img)
+    def load_img(self, raw):
+        try:
+            import PIL.Image
+        except ImportError as exc:
+            raise ImportError(
+                "Missing dependency Pillow for computer vision:\n"
+                "To install run:\n\n"
+                "  pip install 'dvcx[cv]'\n"
+            ) from exc
+
+        img = PIL.Image.open(raw, formats=self.formats).convert(self.mode)
+        if self.size:
+            img = img.resize(self.size)
+        if self.transform:
+            img = self.transform(img)
+        return img
 
 
 @attrs.define(slots=False)
 class Label(UDFParameter):
     """
     Encode column value as an index into the provided list of labels.
     """
@@ -41,24 +62,23 @@
 
     def get_value(self, catalog: "Catalog", row: "Row", **kwargs) -> int:
         label = row[self.column]
         return self.classes.index(label)
 
 
 class Text(UDFParameter):
-    """
-    Tokenize and otherwise transform text column.
-
-    Args:
-        column (str): Name of column containing text.
-        tokenizer (Any): Tokenizer to use to tokenize objects.
-        kwargs (dict): Additional kwargs to pass when calling tokenizer.
-    """
-
-    def __init__(self, column: str, tokenizer: Any, **kwargs):
+    def __init__(self, column: str, tokenizer: Callable, **kwargs):
+        """
+        Tokenize and otherwise transform text column.
+
+        Args:
+            column (str): Name of column containing text.
+            tokenizer (Callable): Tokenizer to use to tokenize objects.
+            kwargs (dict): Additional kwargs to pass when calling tokenizer.
+        """
         self.column = column
         self.tokenizer = tokenizer
         self.kwargs = kwargs
 
         self.hf = False
         try:
             from transformers.tokenization_utils_base import PreTrainedTokenizerBase
```

### Comparing `dvcx-0.74.0/src/dvcx/lib/pytorch.py` & `dvcx-0.75.0/src/dvcx/lib/pytorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,36 +30,41 @@
 
 class PytorchDataset(IterableDataset):
     def __init__(
         self,
         params: Sequence["UDFParamSpec"],
         name: str,
         version: Optional[int] = None,
+        catalog: Optional["Catalog"] = None,
         transform: Optional["Transform"] = DEFAULT_TRANSFORM,
         workers: int = ASYNC_WORKERS,
         cache: bool = False,
-        catalog: Optional["Catalog"] = None,
+        num_samples: int = 0,
     ):
         """
         Pytorch IterableDataset that streams DVCx datasets.
 
         Args:
             params (UDFParamSpec): Fields from DVCx dataset to stream.
             name (str): Name of DVCx dataset to stream.
             version (int): Version of DVCx dataset to stream.
+            catalog (Catalog): DVCx catalog to which dataset belongs.
             transform (Transform): Torchvision v2 transforms to apply to the dataset.
             workers (int): Number of async workers per process.
             cache (bool): Whether to download and cache objects locally.
+            num_samples (int): Number of random samples to draw for each epoch.
+                This argument is ignored if `num_samples=0` (the default).
         """
         self.params = params
         self.name = name
         self.version = version
         self.transform = transform
         self.workers = workers
         self.cache = cache
+        self.num_samples = num_samples
         if catalog is None:
             catalog = get_catalog()
         self._init_catalog(catalog)
 
     def _init_catalog(self, catalog: "Catalog"):
         # For compatibility with multiprocessing,
         # we can only store params in __init__(), as Catalog isn't picklable
@@ -79,17 +84,18 @@
         wh = wh_cls(*wh_args, **wh_kwargs)
         return Catalog(idgen, ms, wh, **self._catalog_params)
 
     def __iter__(self) -> Iterator[Any]:
         if self.catalog is None:
             self.catalog = self._get_catalog()
         total_rank, total_workers = self.get_rank_and_workers()
-        q = DatasetQuery(
-            name=self.name, version=self.version, catalog=self.catalog
-        ).chunk(total_rank, total_workers)
+        q = DatasetQuery(name=self.name, version=self.version, catalog=self.catalog)
+        if self.num_samples > 0:
+            q = q.sample(self.num_samples)
+        q = q.chunk(total_rank, total_workers)
         stream = q.extract(*self.params, workers=self.workers, cache=self.cache)
         for row in stream:
             # Apply transforms
             if self.transform:
                 try:
                     row = self.transform(row)
                 except ValueError:
@@ -99,15 +105,15 @@
 
     @staticmethod
     def get_rank_and_workers() -> tuple[int, int]:
         """Get combined rank and number of workers across all nodes."""
         try:
             world_rank = get_rank()
             world_size = get_world_size()
-        except ValueError:
+        except (RuntimeError, ValueError):
             world_rank = 0
             world_size = 1
         worker_info = get_worker_info()
         if worker_info:
             worker_rank = worker_info.id
             num_workers = worker_info.num_workers
         else:
```

### Comparing `dvcx-0.74.0/src/dvcx/lib/udf.py` & `dvcx-0.75.0/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/unstructured.py` & `dvcx-0.75.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/utils.py` & `dvcx-0.75.0/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/webdataset.py` & `dvcx-0.75.0/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.75.0/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.75.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/listing.py` & `dvcx-0.75.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/node.py` & `dvcx-0.75.0/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/nodes_fetcher.py` & `dvcx-0.75.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/nodes_thread_pool.py` & `dvcx-0.75.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/progress.py` & `dvcx-0.75.0/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/query/batch.py` & `dvcx-0.75.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/query/builtins.py` & `dvcx-0.75.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/query/dataset.py` & `dvcx-0.75.0/src/dvcx/query/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     Any,
     Callable,
     Optional,
     Protocol,
     TypeVar,
     Union,
 )
-from uuid import uuid4
 
 import attrs
 import sqlalchemy
 from attrs import frozen
 from dill import dumps
 from sqlalchemy.sql import func as f
 from sqlalchemy.sql.elements import ColumnClause, ColumnElement
@@ -45,19 +44,21 @@
     PARTITION_COLUMN_ID,
     partition_col_names,
     partition_columns,
 )
 from dvcx.dataset import DatasetRow
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetNotFoundError, QueryScriptCancelError
+from dvcx.sql.functions import rand
 from dvcx.sql.types import SQLType
 from dvcx.storage import StorageURI
 from dvcx.utils import chunk, determine_processes
 
 from .schema import C, UDFParamSpec, normalize_param
+from .session import Session
 from .udf import UDFBase, UDFClassWrapper, UDFFactory, UDFType
 
 if TYPE_CHECKING:
     from sqlalchemy.sql.elements import ClauseElement
     from sqlalchemy.sql.schema import Table
     from sqlalchemy.sql.selectable import GenerativeSelect
     from typing_extensions import Concatenate, ParamSpec, Self
@@ -981,27 +982,27 @@
         self,
         path: str = "",
         name: str = "",
         version: Optional[int] = None,
         catalog: Optional["Catalog"] = None,
         client_config=None,
         recursive: Optional[bool] = True,
+        session: Optional[Session] = None,
     ):
         self.steps: list["Step"] = []
         self.catalog = catalog or get_catalog(client_config=client_config)
         self._chunk_index: Optional[int] = None
         self._chunk_total: Optional[int] = None
         self.temp_table_names: list[str] = []
         self.dependencies: set[DatasetDependencyType] = set()
         self.table = self.get_table()
         self.starting_step: StartingStep
         self.name: Optional[str] = None
         self.version: Optional[int] = None
-        # if run with Catalog.query(...) it will have this env variable defined
-        self.query_session_uuid = os.getenv("DVCX_QUERY_SESSION_UUID", None)
+        self.session = Session.get(session, catalog=catalog)
 
         if path:
             self.starting_step = IndexingStep(
                 path, self.catalog, {"client_config": client_config}, recursive
             )
         elif name:
             version = version or self.catalog.get_dataset(name).latest_version
@@ -1065,14 +1066,17 @@
 
         if index is not None and total is not None:
             index, total = int(index), int(total)  # os.getenv returns str
 
             if not (0 <= index < total):
                 raise ValueError("chunk index must be between 0 and total")
 
+            # Respect limit in chunks
+            query.steps = self._chunk_limit(query.steps, index, total)
+
             # Prepend the chunk filter to the step chain.
             query = query.filter(C.random % total == index)
             query.steps = query.steps[-1:] + query.steps[:-1]
 
         result = query.starting_step.apply()
         group_by = None
         self.temp_table_names.extend(result.temp_table_names)
@@ -1094,14 +1098,34 @@
         if group_by:
             result = group_by.apply(result.query_generator)
             self.temp_table_names.extend(result.temp_table_names)
             self.dependencies.update(result.dependencies)
 
         return result.query_generator
 
+    @staticmethod
+    def _chunk_limit(steps: list["Step"], index: int, total: int) -> list["Step"]:
+        no_limit_steps = []
+        limit = None
+        for step in steps:
+            # Remember last limit
+            if isinstance(step, SQLLimit):
+                limit = step.n
+            # Only keep non-limit steps
+            else:
+                no_limit_steps.append(step)
+        # Chunk the limit
+        if limit:
+            limit_modulo = limit % total
+            limit = limit // total
+            if index < limit_modulo:
+                limit += 1
+            return no_limit_steps + [SQLLimit(limit)]
+        return steps
+
     def cleanup(self) -> None:
         self.catalog.warehouse.clone().cleanup_temp_tables(self.temp_table_names)
         self.catalog.metastore.clone().cleanup_temp_tables(self.temp_table_names)
         self.temp_table_names = []
 
     def results(self, row_factory=None, **kwargs):
         with self.as_iterable(**kwargs) as result:
@@ -1178,17 +1202,15 @@
 
         records = self.to_records()
         return pd.DataFrame.from_records(records)
 
     def to_pytorch(
         self,
         *params: UDFParamSpec,
-        transform=None,
-        workers: int = ASYNC_WORKERS,
-        cache: bool = False,
+        **kwargs,
     ) -> "PytorchDataset":
         try:
             import torch  # noqa: F401
         except ImportError as exc:
             raise ImportError(
                 "Missing required dependency 'torch' for DatasetQuery.to_pytorch()"
             ) from exc
@@ -1200,24 +1222,36 @@
             ds_name = self.catalog.generate_query_dataset_name()
             ds = self.save(ds_name)
         assert ds.name is not None  # for mypy
         return PytorchDataset(
             params,
             ds.name,
             ds.version,
-            transform=transform,
-            workers=workers,
-            cache=cache,
             catalog=self.catalog,
+            **kwargs,
         )
 
     def shuffle(self) -> "DatasetQuery":
         # ToDo: implement shaffle based on seed and/or generating random column
         return self.order_by(C.random)
 
+    def sample(self, n) -> "DatasetQuery":
+        """
+        Return a random sample from the dataset.
+
+        Args:
+            n (int): Number of samples to draw.
+
+        NOTE: Sampled are not deterministic, and streamed/paginated queries or
+        multiple workers will draw samples with replacement.
+        """
+        sampled = self.order_by(rand())
+
+        return sampled.limit(n)
+
     def show(self, limit=20) -> None:
         df = self.limit(limit).to_pandas()
         no_footer = re.sub(r"\n\[\d+ rows x \d+ columns\]$", "", str(df))
         print(no_footer.rstrip(" \n"))
         if len(df) == limit:
             print(f"[limited by {limit} objects]")
 
@@ -1529,18 +1563,15 @@
                 raise RuntimeError(f"Dataset {name} already has version {version}")
         except DatasetNotFoundError:
             pass
         if not name and version:
             raise RuntimeError("Cannot set version for temporary datasets")
 
         if not name:
-            # missing name means this is temp dataset
-            if not self.query_session_uuid:
-                raise RuntimeError("Temporary dataset must be created using session")
-            name = self.catalog.generate_temp_dataset_name(self.query_session_uuid)
+            name = self.session.generate_temp_dataset_name()
 
         try:
             query = self.apply_steps()
 
             missing_default_columns = [
                 c_name
                 for c_name in DATASET_CORE_COLUMN_NAMES
@@ -1677,35 +1708,7 @@
 
 
 def _random_string(length: int) -> str:
     return "".join(
         random.choice(string.ascii_letters + string.digits)  # noqa: S311
         for i in range(length)
     )
-
-
-class Session:
-    """
-    Object that injects it's unique uuid to DatasetQuery instances created
-    through it. This is needed for things like temp datasets.
-    """
-
-    def __init__(self, catalog: Optional["Catalog"] = None):
-        self.uuid = uuid4().hex
-        self.catalog = catalog or get_catalog()
-
-    def DatasetQuery(self, *args, **kwargs) -> DatasetQuery:  # noqa: N802
-        ds = DatasetQuery(*args, **kwargs)
-        ds.query_session_uuid = self.uuid
-        return ds
-
-    def cleanup(self) -> None:
-        self.catalog.cleanup_temp_datasets(self.uuid)
-
-
-@contextlib.contextmanager
-def session(catalog: Optional["Catalog"] = None):
-    session = Session(catalog=catalog)
-    try:
-        yield session
-    finally:
-        session.cleanup()
```

### Comparing `dvcx-0.74.0/src/dvcx/query/dispatch.py` & `dvcx-0.75.0/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/query/schema.py` & `dvcx-0.75.0/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/query/udf.py` & `dvcx-0.75.0/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/remote/studio.py` & `dvcx-0.75.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/sql/default/base.py` & `dvcx-0.75.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/sql/functions/array.py` & `dvcx-0.75.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/sql/functions/path.py` & `dvcx-0.75.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/sql/selectable.py` & `dvcx-0.75.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/sql/sqlite/base.py` & `dvcx-0.75.0/src/dvcx/sql/sqlite/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import ujson
 from sqlalchemy.dialects import sqlite
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.sql.elements import literal
 from sqlalchemy.sql.expression import case
 from sqlalchemy.sql.functions import func
 
-from dvcx.sql.functions import array, conditional, string
+from dvcx.sql.functions import array, conditional, random, string
 from dvcx.sql.functions import path as sql_path
 from dvcx.sql.selectable import Values, base_values_compiler
 from dvcx.sql.sqlite.types import (
     SQLiteTypeConverter,
     SQLiteTypeReadConverter,
     register_type_converters,
 )
@@ -74,14 +74,15 @@
     compiles(array.euclidean_distance, "sqlite")(compile_euclidean_distance)
     compiles(array.length, "sqlite")(compile_array_length)
     compiles(string.length, "sqlite")(compile_string_length)
     compiles(string.split, "sqlite")(compile_string_split)
     compiles(conditional.greatest, "sqlite")(compile_greatest)
     compiles(conditional.least, "sqlite")(compile_least)
     compiles(Values, "sqlite")(compile_values)
+    compiles(random.rand, "sqlite")(compile_rand)
 
     register_user_defined_sql_functions()
     setup_is_complete = True
 
 
 def run_compiler_hook(name):
     try:
@@ -320,7 +321,11 @@
     else:
         expr = func.min(*args)
     return compiler.process(expr, **kwargs)
 
 
 def compile_values(element, compiler, **kwargs):
     return base_values_compiler(lambda i: f"column{i}", element, compiler, **kwargs)
+
+
+def compile_rand(element, compiler, **kwargs):
+    return compiler.process(func.random(), **kwargs)
```

### Comparing `dvcx-0.74.0/src/dvcx/sql/sqlite/types.py` & `dvcx-0.75.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/sql/types.py` & `dvcx-0.75.0/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/sql/utils.py` & `dvcx-0.75.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/storage.py` & `dvcx-0.75.0/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx/utils.py` & `dvcx-0.75.0/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.75.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.74.0
+Version: 0.75.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.74.0/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.75.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -120,27 +120,29 @@
 src/dvcx/lib/webdataset_meta.py
 src/dvcx/query/__init__.py
 src/dvcx/query/batch.py
 src/dvcx/query/builtins.py
 src/dvcx/query/dataset.py
 src/dvcx/query/dispatch.py
 src/dvcx/query/schema.py
+src/dvcx/query/session.py
 src/dvcx/query/udf.py
 src/dvcx/remote/__init__.py
 src/dvcx/remote/studio.py
 src/dvcx/sql/__init__.py
 src/dvcx/sql/selectable.py
 src/dvcx/sql/types.py
 src/dvcx/sql/utils.py
 src/dvcx/sql/default/__init__.py
 src/dvcx/sql/default/base.py
 src/dvcx/sql/functions/__init__.py
 src/dvcx/sql/functions/array.py
 src/dvcx/sql/functions/conditional.py
 src/dvcx/sql/functions/path.py
+src/dvcx/sql/functions/random.py
 src/dvcx/sql/functions/string.py
 src/dvcx/sql/sqlite/__init__.py
 src/dvcx/sql/sqlite/base.py
 src/dvcx/sql/sqlite/types.py
 src/dvcx/sql/sqlite/vector.py
 tests/__init__.py
 tests/conftest.py
@@ -173,23 +175,25 @@
 tests/unit/test_database_engine.py
 tests/unit/test_dataset.py
 tests/unit/test_fileslice.py
 tests/unit/test_id_generator.py
 tests/unit/test_listing.py
 tests/unit/test_metastore.py
 tests/unit/test_serializer.py
+tests/unit/test_session.py
 tests/unit/test_storage.py
 tests/unit/test_udf.py
 tests/unit/test_utils.py
 tests/unit/test_warehouse.py
 tests/unit/lib/test_cached_stream.py
 tests/unit/lib/test_feature.py
 tests/unit/lib/test_feature_udf.py
 tests/unit/lib/test_file.py
 tests/unit/lib/test_webdataset.py
 tests/unit/lib/test_webdataset_meta.py
 tests/unit/sql/test_array.py
 tests/unit/sql/test_conditional.py
 tests/unit/sql/test_path.py
+tests/unit/sql/test_random.py
 tests/unit/sql/test_selectable.py
 tests/unit/sql/test_string.py
 tests/unit/sql/sqlite/test_utils.py
```

### Comparing `dvcx-0.74.0/src/dvcx.egg-info/requires.txt` & `dvcx-0.75.0/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/benchmarks/conftest.py` & `dvcx-0.75.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/conftest.py` & `dvcx-0.75.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/data.py` & `dvcx-0.75.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/func/test_catalog.py` & `dvcx-0.75.0/tests/func/test_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import io
 import json
 import os
 from contextlib import suppress
 from pathlib import Path
 from textwrap import dedent
 from urllib.parse import urlparse
-from uuid import uuid4
 
 import pytest
 import yaml
 from fsspec.implementations.local import LocalFileSystem
 
 from dvcx.catalog import indexer_formats, parse_edvcx_file
-from dvcx.dataset import TEMP_DATASET_NAME_PREFIX
 from dvcx.error import (
-    DatasetNotFoundError,
     QueryScriptCompileError,
     QueryScriptDatasetNotFound,
     QueryScriptRunError,
     StorageNotFoundError,
 )
 
 from ..data import ENTRIES
@@ -929,44 +926,14 @@
 def test_index_error(cloud_test_catalog):
     protocol = cloud_test_catalog.src_uri.split("://", 1)[0]
     # XXX: different clients raise inconsistent exceptions
     with pytest.raises(Exception):  # noqa: B017
         cloud_test_catalog.catalog.index([f"{protocol}://does_not_exist"])
 
 
-def test_generate_temp_dataset_name_with_query_session_uuid(cloud_test_catalog):
-    catalog = cloud_test_catalog.catalog
-    query_session_uuid = uuid4().hex
-    name = catalog.generate_temp_dataset_name(query_session_uuid)
-    assert name.startswith(f"{TEMP_DATASET_NAME_PREFIX}{query_session_uuid}")
-
-
-def test_clean_temp_dataset(cloud_test_catalog):
-    # if temp dataset is created by using dvcx as a lib in client's code, it
-    # needs to be created using sessions which will inject it's unique query
-    # session uuid
-    catalog = cloud_test_catalog.catalog
-    query_session_uuid = uuid4().hex
-
-    ds_name = catalog.generate_temp_dataset_name(query_session_uuid)
-    dataset = catalog.create_dataset_from_sources(
-        ds_name,
-        [f"{cloud_test_catalog.src_uri}/dogs/*"],
-        recursive=True,
-    )
-    assert dataset.name == ds_name
-
-    catalog.cleanup_temp_datasets("wrong_uuid")
-    catalog.get_dataset(ds_name)
-
-    catalog.cleanup_temp_datasets(query_session_uuid)
-    with pytest.raises(DatasetNotFoundError):
-        catalog.get_dataset(ds_name)
-
-
 def test_query(cloud_test_catalog, mock_popen_dataset_created):
     catalog = cloud_test_catalog.catalog
     src_uri = cloud_test_catalog.src_uri
 
     query_script = f"""\
     from dvcx.query import C, DatasetQuery
     DatasetQuery({src_uri!r})
```

### Comparing `dvcx-0.74.0/tests/func/test_client.py` & `dvcx-0.75.0/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/func/test_dataset_query.py` & `dvcx-0.75.0/tests/func/test_dataset_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 import sqlalchemy
 from dateutil.parser import isoparse
 from sqlalchemy import tuple_
 
 from dvcx.catalog import indexer_formats
 from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
 from dvcx.data_storage.warehouse import RANDOM_BITS
-from dvcx.dataset import TEMP_DATASET_NAME_PREFIX, DatasetDependencyType
+from dvcx.dataset import DatasetDependencyType
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetInvalidVersionError, DatasetNotFoundError
 from dvcx.lib.param import Label, Text
 from dvcx.node import Node
 from dvcx.query import (
     C,
     DatasetQuery,
     DatasetRow,
     LocalFilename,
     Object,
     Stream,
-    session,
     udf,
 )
 from dvcx.query.builtins import checksum, index_tar
 from dvcx.query.dataset import QueryStep
 from dvcx.sql import functions
 from dvcx.sql.functions.array import cosine_distance, euclidean_distance
 from dvcx.sql.types import (
@@ -245,34 +244,14 @@
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
-def test_saving_temp_dataset(cloud_test_catalog, dogs_cats_dataset):
-    catalog = cloud_test_catalog.catalog
-    ds = DatasetQuery(name=dogs_cats_dataset.name, version=1, catalog=catalog)
-    ds.query_session_uuid = uuid.uuid4().hex
-
-    ds2 = ds.save()
-    assert ds2.name.startswith(TEMP_DATASET_NAME_PREFIX)
-    assert isinstance(ds2, DatasetQuery)
-    assert (
-        {row.name for row in catalog.ls_dataset_rows(dogs_cats_dataset.name, 1)}
-        == {row.name for row in catalog.ls_dataset_rows(ds2.name, ds2.version)}
-        == {"cat1", "cat2", "dog1", "dog2", "dog3", "dog4"}
-    )
-
-
-@pytest.mark.parametrize(
-    "cloud_type,version_aware",
-    [("s3", True)],
-    indirect=True,
-)
 def test_query_specific_dataset_set_proper_dataset_name_version(
     cloud_test_catalog, dogs_cats_dataset
 ):
     catalog = cloud_test_catalog.catalog
     ds = DatasetQuery(name=dogs_cats_dataset.name, version=1, catalog=catalog)
     assert ds.name == dogs_cats_dataset.name
     assert ds.version == 1
@@ -1233,14 +1212,30 @@
         ("woof", "dog1"),
         ("arf", "dog2"),
         ("bark", "dog3"),
         ("ruff", "dog4"),
     }
 
 
+def test_extract_chunked_limit(cloud_test_catalog, dogs_dataset):
+    ctc = cloud_test_catalog
+    chunks = 5
+    limit = 1
+    all_data = []
+    q = DatasetQuery(name=dogs_dataset.name, version=1, catalog=ctc.catalog)
+    # Add sufficient rows to ensure each chunk has rows
+    for _ in range(5):
+        q = q.union(q)
+    for i in range(chunks):
+        data = q.limit(limit).chunk(i, chunks).extract(Object(to_str), "name")
+        all_data.extend(data)
+
+    assert len(all_data) == limit
+
+
 @pytest.mark.parametrize(
     "cloud_type, version_aware",
     [("file", False)],
     indirect=True,
 )
 def test_extract_limit(cloud_test_catalog, dogs_dataset):
     catalog = cloud_test_catalog.catalog
@@ -3619,64 +3614,7 @@
         DatasetQuery(path=path, catalog=catalog).select(C.name).save("cats", version=1)
 
     assert str(exc_info.value) == (
         "Missing default columns from final query: id, vtype, dir_type, parent_id, "
         "parent, checksum, etag, version, is_latest, last_modified, size, "
         "owner_name, owner_id, anno, random, location, source"
     )
-
-
-@pytest.mark.parametrize(
-    "cloud_type,version_aware",
-    [("s3", True)],
-    indirect=True,
-)
-def test_temp_dataset_used_and_removed(cloud_test_catalog, dogs_cats_dataset):
-    catalog = cloud_test_catalog.catalog
-
-    with session(catalog=catalog) as query_session:
-        temp = query_session.DatasetQuery(
-            name=dogs_cats_dataset.name, catalog=catalog
-        ).save()
-        (
-            query_session.DatasetQuery(name=temp.name, catalog=catalog)
-            .filter(C.name.glob("dog*"))
-            .save("dogs")
-        )
-        (
-            query_session.DatasetQuery(name=temp.name, catalog=catalog)
-            .filter(C.name.glob("cat*"))
-            .save("cats")
-        )
-
-    assert {r.name for r in catalog.ls_dataset_rows("dogs", 1)} == {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
-    assert {r.name for r in catalog.ls_dataset_rows("cats", 1)} == {
-        "cat1",
-        "cat2",
-    }
-
-    # make sure temp is removed
-    assert (
-        list(catalog.metastore.list_datasets_by_prefix(TEMP_DATASET_NAME_PREFIX)) == []
-    )
-    # check one more time 2 datasets created out of temp are present: dogs and cats
-    assert "cats" in [d.name for d in catalog.ls_datasets()]
-    assert "dogs" in [d.name for d in catalog.ls_datasets()]
-
-
-@pytest.mark.parametrize(
-    "cloud_type,version_aware",
-    [("s3", True)],
-    indirect=True,
-)
-def test_temp_dataset_used_outside_session(cloud_test_catalog, dogs_dataset):
-    catalog = cloud_test_catalog.catalog
-
-    with pytest.raises(RuntimeError) as exc_info:
-        DatasetQuery(name=dogs_dataset.name, catalog=catalog).save()
-
-    assert str(exc_info.value) == "Temporary dataset must be created using session"
```

### Comparing `dvcx-0.74.0/tests/func/test_datasets.py` & `dvcx-0.75.0/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/func/test_ls.py` & `dvcx-0.75.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/func/test_pull.py` & `dvcx-0.75.0/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/func/test_pytorch.py` & `dvcx-0.75.0/tests/func/test_pytorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,7 +42,19 @@
         version=fake_dataset.version,
         transform=transform,
     )
     for img, label in pt_dataset:
         assert isinstance(img, Tensor)
         assert isinstance(label, int)
         assert img.size() == Size([3, 64, 64])
+
+
+def test_pytorch_dataset_sample(tmp_path, fake_dataset):
+    transform = v2.Compose([v2.ToTensor(), v2.Resize((64, 64))])
+    pt_dataset = PytorchDataset(
+        params=[Image(), "label"],
+        name=fake_dataset.name,
+        version=fake_dataset.version,
+        transform=transform,
+        num_samples=700,
+    )
+    assert len(list(pt_dataset)) == 700
```

### Comparing `dvcx-0.74.0/tests/func/test_query.py` & `dvcx-0.75.0/tests/func/test_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from textwrap import dedent
 
 import dill
 import pytest
 
-from dvcx.catalog import QUERY_DATASET_NAME_PREFIX, TEMP_DATASET_NAME_PREFIX
+from dvcx.catalog import QUERY_DATASET_PREFIX
 from dvcx.cli import query
 
 
 @pytest.fixture
 def catalog_info_filepath(cloud_test_catalog_tmpfile, tmp_path):
     catalog = cloud_test_catalog_tmpfile.catalog
 
@@ -93,15 +93,15 @@
     from dvcx.query import C, DatasetQuery
 
     DatasetQuery({src_uri!r}, catalog=catalog)
     """
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
     dataset, version, output, _ = catalog.query(query_script, save=True)
-    assert dataset.name.startswith(QUERY_DATASET_NAME_PREFIX)
+    assert dataset.name.startswith(QUERY_DATASET_PREFIX)
     assert dataset.query_script == query_script
     assert version == 1
     assert dataset.versions_values == [1]
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
         "cat1",
         "cat2",
         "description",
@@ -126,15 +126,15 @@
     from dvcx.query import C, DatasetQuery
 
     DatasetQuery({src_uri!r}, catalog=catalog).filter(C.name.glob("dog*")).save("dogs")
     """
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
     dataset, version, output, _ = catalog.query(query_script, save=True)
-    assert not dataset.name.startswith(QUERY_DATASET_NAME_PREFIX)
+    assert not dataset.name.startswith(QUERY_DATASET_PREFIX)
     assert dataset.query_script == query_script
     assert version == 1
     assert dataset.versions_values == [1]
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
         "dog1",
         "dog2",
         "dog3",
@@ -202,92 +202,7 @@
     assert dataset.versions_values == [1]
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, version)} == {
         "dog1",
         "dog2",
         "dog3",
         "dog4",
     }
-
-
-def test_query_with_temp_dataset(
-    cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath
-):
-    catalog = cloud_test_catalog_tmpfile.catalog
-    src_uri = cloud_test_catalog_tmpfile.src_uri
-
-    query_script = f"""\
-    from dvcx.query import C, DatasetQuery
-
-    # creating temp dataset for optimization
-    temp = DatasetQuery({src_uri!r}, catalog=catalog).save()
-    DatasetQuery(
-        name=temp.name, catalog=catalog
-    ).filter(C.name.glob("cat*")).save("cats")
-    DatasetQuery(
-        name=temp.name, catalog=catalog
-    ).filter(C.name.glob("dog*")).save("dogs")
-    """
-    query_script = setup_catalog(query_script, catalog_info_filepath)
-
-    catalog.query(query_script, save=True)
-
-    assert {r.name for r in catalog.ls_dataset_rows("dogs", 1)} == {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
-    assert {r.name for r in catalog.ls_dataset_rows("cats", 1)} == {
-        "cat1",
-        "cat2",
-    }
-
-    # make sure temp is removed
-    assert (
-        list(catalog.metastore.list_datasets_by_prefix(TEMP_DATASET_NAME_PREFIX)) == []
-    )
-    # check one more time only 2 datasets are present: dogs and cats
-    assert sorted([d.name for d in catalog.ls_datasets()]) == ["cats", "dogs"]
-
-
-def test_query_with_temp_dataset_using_session(
-    cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath
-):
-    catalog = cloud_test_catalog_tmpfile.catalog
-    src_uri = cloud_test_catalog_tmpfile.src_uri
-
-    query_script = f"""\
-    from dvcx.query import C, DatasetQuery, session
-
-    with session(catalog=catalog) as session:
-        # creating temp dataset for optimization
-        temp = DatasetQuery({src_uri!r}, catalog=catalog).save()
-        DatasetQuery(name=temp.name, catalog=catalog).filter(
-            C.name.glob("cat*")
-        ).save("cats")
-        DatasetQuery(name=temp.name, catalog=catalog).filter(
-            C.name.glob("dog*")
-        ).save("dogs")
-
-    DatasetQuery(name="dogs", catalog=catalog)
-    """
-    query_script = setup_catalog(query_script, catalog_info_filepath)
-
-    catalog.query(query_script, save=True)
-
-    assert {r.name for r in catalog.ls_dataset_rows("dogs", 1)} == {
-        "dog1",
-        "dog2",
-        "dog3",
-        "dog4",
-    }
-    assert {r.name for r in catalog.ls_dataset_rows("cats", 1)} == {
-        "cat1",
-        "cat2",
-    }
-
-    # make sure temp is removed
-    assert (
-        list(catalog.metastore.list_datasets_by_prefix(TEMP_DATASET_NAME_PREFIX)) == []
-    )
-    # check one more time only 2 datasets are present: dogs and cats
-    assert sorted([d.name for d in catalog.ls_datasets()]) == ["cats", "dogs"]
```

### Comparing `dvcx-0.74.0/tests/test_cli_e2e.py` & `dvcx-0.75.0/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/lib/test_cached_stream.py` & `dvcx-0.75.0/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/lib/test_feature.py` & `dvcx-0.75.0/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/lib/test_feature_udf.py` & `dvcx-0.75.0/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/lib/test_file.py` & `dvcx-0.75.0/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/lib/test_webdataset.py` & `dvcx-0.75.0/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.75.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/sql/test_array.py` & `dvcx-0.75.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/sql/test_conditional.py` & `dvcx-0.75.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/sql/test_path.py` & `dvcx-0.75.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/sql/test_selectable.py` & `dvcx-0.75.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/sql/test_string.py` & `dvcx-0.75.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_asyn.py` & `dvcx-0.75.0/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_cache.py` & `dvcx-0.75.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_catalog.py` & `dvcx-0.75.0/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_catalog_formats.py` & `dvcx-0.75.0/tests/unit/test_catalog_formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_catalog_loader.py` & `dvcx-0.75.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_cli_parsing.py` & `dvcx-0.75.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_client.py` & `dvcx-0.75.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_client_s3.py` & `dvcx-0.75.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_data_storage.py` & `dvcx-0.75.0/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_database_engine.py` & `dvcx-0.75.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_dataset.py` & `dvcx-0.75.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_fileslice.py` & `dvcx-0.75.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_id_generator.py` & `dvcx-0.75.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_listing.py` & `dvcx-0.75.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_metastore.py` & `dvcx-0.75.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_serializer.py` & `dvcx-0.75.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_storage.py` & `dvcx-0.75.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_udf.py` & `dvcx-0.75.0/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_utils.py` & `dvcx-0.75.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/unit/test_warehouse.py` & `dvcx-0.75.0/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.74.0/tests/utils.py` & `dvcx-0.75.0/tests/utils.py`

 * *Files identical despite different names*

