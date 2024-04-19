# Comparing `tmp/deeplake-3.9.0.tar.gz` & `tmp/deeplake-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.9.0.tar", last modified: Fri Apr  5 19:57:07 2024, max compression
+gzip compressed data, was "deeplake-3.9.1.tar", last modified: Fri Apr 19 21:53:04 2024, max compression
```

## Comparing `deeplake-3.9.0.tar` & `deeplake-3.9.1.tar`

### file list

```diff
@@ -1,423 +1,423 @@
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.203170 deeplake-3.9.0/
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15975 2024-04-05 17:56:26.000000 deeplake-3.9.0/LICENSE
--rw-r--r--   0 nvoxland   (501) wheel        (0)       36 2024-04-05 17:56:26.000000 deeplake-3.9.0/MANIFEST.in
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21928 2024-04-05 19:57:07.203281 deeplake-3.9.0/PKG-INFO
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21238 2024-04-05 17:56:26.000000 deeplake-3.9.0/README.md
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.132430 deeplake-3.9.0/deeplake/
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2812 2024-04-05 19:55:28.000000 deeplake-3.9.0/deeplake/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.135633 deeplake-3.9.0/deeplake/api/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   109206 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4693 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1203 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1698 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/link_tiled.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2908 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/read.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.143023 deeplake-3.9.0/deeplake/api/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4250 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1867 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    97680 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_api.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7076 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    11734 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2654 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2562 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2959 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1500 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6210 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1040 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_events.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5056 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      298 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6482 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6911 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7044 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_json.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26194 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3329 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1789 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_linking.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1024 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1204 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4109 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7900 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_none.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      970 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2108 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5680 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4249 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12455 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_pop.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1595 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    18930 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8958 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_reset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4596 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      526 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_tag.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3149 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_text.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26508 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8127 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7035 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tests/test_views.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1368 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/api/tiled.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.143207 deeplake-3.9.0/deeplake/auto/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.143566 deeplake-3.9.0/deeplake/auto/structured/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/structured/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      635 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/structured/base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7308 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.144663 deeplake-3.9.0/deeplake/auto/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7975 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13527 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5371 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5519 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.145384 deeplake-3.9.0/deeplake/auto/unstructured/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      537 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.146448 deeplake-3.9.0/deeplake/auto/unstructured/coco/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7093 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      669 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1709 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5237 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6701 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3533 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4514 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.147024 deeplake-3.9.0/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      278 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7394 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12933 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.148335 deeplake-3.9.0/deeplake/client/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.149050 deeplake-3.9.0/deeplake/client/auth/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      578 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/auth/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      886 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/auth/activeloop.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      933 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/auth/auth_context.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2407 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/auth/azure.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1603 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/auth/test_auth_context.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21451 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/client.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1436 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/config.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      690 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/log.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10650 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/test_client.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12996 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/client/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3876 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10287 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/constants.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.154179 deeplake-3.9.0/deeplake/core/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       23 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.156288 deeplake-3.9.0/deeplake/core/chunk/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/chunk/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    24544 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26270 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6748 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4944 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4512 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5464 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10139 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   137699 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    39184 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/compression.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.157668 deeplake-3.9.0/deeplake/core/compute/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/compute/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      911 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/compute/process.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2332 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/compute/provider.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      640 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/compute/ray.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      806 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/compute/serial.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      576 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/compute/thread.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.159681 deeplake-3.9.0/deeplake/core/dataset/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/dataset/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   196630 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/dataset/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16167 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12670 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/dataset/indra_dataset_view.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5999 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/dataset/indra_tensor_view.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      760 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4666 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/distance_type.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4348 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.160027 deeplake-3.9.0/deeplake/core/index/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      138 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/index/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    17988 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/index/index.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9539 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/index_maintenance.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    20531 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/io.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4121 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/ipc.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13074 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/link_creds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16646 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2277 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/linked_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2597 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9946 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/lock.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.160598 deeplake-3.9.0/deeplake/core/meta/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       97 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4043 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.162486 deeplake-3.9.0/deeplake/core/meta/encode/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    25591 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3915 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13848 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1551 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3972 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      941 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      683 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.163478 deeplake-3.9.0/deeplake/core/meta/encode/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      226 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2237 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1452 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2114 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3673 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2810 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7627 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      503 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    14862 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      906 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/partial_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      971 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/partial_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5269 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/polygon.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.164380 deeplake-3.9.0/deeplake/core/query/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       82 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/query/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12021 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/query/autocomplete.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15253 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/query/filter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8905 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/query/query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21165 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2506 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/seed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    23415 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.167155 deeplake-3.9.0/deeplake/core/storage/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      495 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15471 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/azure.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1053 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19256 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/gcs.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13455 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/google_drive.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3114 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/indra.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9604 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/local.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    20308 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3705 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/memory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7292 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/provider.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26754 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/storage/s3.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    65084 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tensor.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7571 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tensor_link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5185 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/test_serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.169416 deeplake-3.9.0/deeplake/core/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7674 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      729 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_compute.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2181 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16292 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_indra_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      913 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_io.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4811 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_locking.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1833 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      676 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      377 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_seed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1944 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_serialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10543 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tests/test_vdb_indexes.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.170745 deeplake-3.9.0/deeplake/core/tiling/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tiling/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4790 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1701 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4827 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2893 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tiling/serialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1968 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2367 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.171942 deeplake-3.9.0/deeplake/core/transform/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      111 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/transform/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    56175 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/transform/test_transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    30619 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/transform/transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    11143 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6049 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.172549 deeplake-3.9.0/deeplake/core/vectorstore/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      638 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.174075 deeplake-3.9.0/deeplake/core/vectorstore/dataset_handlers/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      100 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/dataset_handlers/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13355 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      450 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/dataset_handlers/dataset_handler.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6152 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.174586 deeplake-3.9.0/deeplake/core/vectorstore/deep_memory/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       73 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/deep_memory/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26733 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/deep_memory/deep_memory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    24999 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/deep_memory/test_deepmemory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    32155 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/deeplake_vectorstore.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.175038 deeplake-3.9.0/deeplake/core/vectorstore/embeddings/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/embeddings/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3777 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/embeddings/embedder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3131 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/embeddings/test_embedder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    90371 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.175619 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.176166 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      392 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    18849 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    14233 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.176754 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      286 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4396 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4223 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.177669 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5190 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7363 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3657 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.178178 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      275 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      956 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      221 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1406 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/vector_search.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.178860 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       93 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5839 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2047 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5205 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.179411 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1924 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2371 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1734 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21909 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3912 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.180489 deeplake-3.9.0/deeplake/core/version_control/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/version_control/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1954 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6337 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3127 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5006 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19869 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    91907 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.183829 deeplake-3.9.0/deeplake/enterprise/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      145 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/enterprise/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8422 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37913 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/enterprise/dataloader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5967 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6276 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    28963 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3432 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/enterprise/test_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    22675 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1819 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/enterprise/util.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1590 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/hooks.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8558 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/htype.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.184054 deeplake-3.9.0/deeplake/integrations/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       99 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.184392 deeplake-3.9.0/deeplake/integrations/huggingface/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       44 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5503 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.185440 deeplake-3.9.0/deeplake/integrations/mmdet/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    62719 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4740 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19652 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.186526 deeplake-3.9.0/deeplake/integrations/pytorch/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       40 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10179 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7317 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4367 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7282 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.187673 deeplake-3.9.0/deeplake/integrations/tf/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1270 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/tf/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2454 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5331 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.187942 deeplake-3.9.0/deeplake/integrations/wandb/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       21 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12089 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.188540 deeplake-3.9.0/deeplake/requirements/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      487 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/requirements/common.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)       71 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/requirements/docs.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/requirements/plugins.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)      416 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/requirements/tests.txt
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.189547 deeplake-3.9.0/deeplake/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1404 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2721 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/tests/client_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4218 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/tests/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4386 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    25709 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/tests/path_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2811 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.199298 deeplake-3.9.0/deeplake/util/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       86 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7370 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/access_method.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1130 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/agreement.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1567 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/array_list.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      619 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2961 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/auto.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5919 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/bugout_reporter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)       54 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/bugout_token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3623 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/cache_chain.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4612 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/casting.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      310 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/check_installation.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1213 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/check_latest_version.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3151 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4597 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/class_label.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      231 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1197 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/compute.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5706 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/connect_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1170 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      443 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/delete_entry.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15906 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5181 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/downsample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)       84 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/empty_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15642 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37198 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/exceptions.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2026 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/exif.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1803 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/from_tfds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/generate_id.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      306 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/hash.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2901 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/htype.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1517 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/image.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      873 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/invalid_view_op.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      135 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1001 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/iteration_warning.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      507 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/join_chunks.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6422 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/json.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7804 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/keys.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3071 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1646 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/logging.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37936 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/merge.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2426 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/modified.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/notebook.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.201080 deeplake-3.9.0/deeplake/util/object_3d/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3374 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1021 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      695 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1323 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6188 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1663 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3221 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10435 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7113 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1087 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4600 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/path.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3220 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/pretty_print.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2844 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/remove_cache.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4511 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/scheduling.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3140 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/shape_interval.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      351 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/shuffle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4784 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/spinner.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1153 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/split.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10033 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/storage.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1131 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tag.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1425 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tensor_db.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      951 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/testing.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.202687 deeplake-3.9.0/deeplake/util/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1476 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_auto.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1795 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1239 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      628 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_keys.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      892 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_read.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1071 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      429 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      698 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_split.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      974 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_tensor_db.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      299 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2452 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      559 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/tests/test_video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      276 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/threading.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    27435 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    41390 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/version_control.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1284 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      167 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/util/warnings.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.203057 deeplake-3.9.0/deeplake/visualizer/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       34 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/visualizer/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6466 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6764 2024-04-05 17:56:26.000000 deeplake-3.9.0/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-05 19:57:07.133533 deeplake-3.9.0/deeplake.egg-info/
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21928 2024-04-05 19:57:07.000000 deeplake-3.9.0/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13651 2024-04-05 19:57:07.000000 deeplake-3.9.0/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-04-05 19:57:07.000000 deeplake-3.9.0/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-04-05 17:57:23.000000 deeplake-3.9.0/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1109 2024-04-05 19:57:07.000000 deeplake-3.9.0/deeplake.egg-info/requires.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        9 2024-04-05 19:57:07.000000 deeplake-3.9.0/deeplake.egg-info/top_level.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)       63 2024-04-05 17:56:26.000000 deeplake-3.9.0/pyproject.toml
--rw-r--r--   0 nvoxland   (501) wheel        (0)      311 2024-04-05 19:57:07.203546 deeplake-3.9.0/setup.cfg
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3339 2024-04-05 17:56:26.000000 deeplake-3.9.0/setup.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.947813 deeplake-3.9.1/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15975 2024-04-19 21:51:56.000000 deeplake-3.9.1/LICENSE
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       36 2024-04-19 21:51:56.000000 deeplake-3.9.1/MANIFEST.in
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21937 2024-04-19 21:53:04.947975 deeplake-3.9.1/PKG-INFO
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21247 2024-04-19 21:51:56.000000 deeplake-3.9.1/README.md
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.866421 deeplake-3.9.1/deeplake/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2812 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.869160 deeplake-3.9.1/deeplake/api/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   109063 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4693 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1203 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1698 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/link_tiled.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2908 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/read.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.876496 deeplake-3.9.1/deeplake/api/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4250 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1867 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    97680 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_api.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7076 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    11734 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2654 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2562 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2959 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1500 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6210 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1040 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_events.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5056 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      298 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6482 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6911 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7044 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_json.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26194 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3329 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1789 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1024 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1204 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4109 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7900 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_none.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      970 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2108 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5680 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4249 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12455 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1595 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    18930 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8958 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4596 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      526 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_tag.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3149 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_text.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26508 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8127 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7035 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tests/test_views.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1368 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/api/tiled.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.876751 deeplake-3.9.1/deeplake/auto/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.877033 deeplake-3.9.1/deeplake/auto/structured/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      635 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/structured/base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7308 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.877952 deeplake-3.9.1/deeplake/auto/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7975 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13527 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5371 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5519 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.878845 deeplake-3.9.1/deeplake/auto/unstructured/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      537 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.879399 deeplake-3.9.1/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7093 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      669 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1709 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5237 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6701 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3533 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4514 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.879911 deeplake-3.9.1/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      278 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7394 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12933 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.881038 deeplake-3.9.1/deeplake/client/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.881819 deeplake-3.9.1/deeplake/client/auth/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      578 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/auth/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      886 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/auth/activeloop.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      933 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/auth/auth_context.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2407 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/auth/azure.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1603 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/auth/test_auth_context.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21451 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/client.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1436 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/config.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      690 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/log.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10650 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/test_client.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12996 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/client/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3876 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10287 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/constants.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.887734 deeplake-3.9.1/deeplake/core/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       23 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.892837 deeplake-3.9.1/deeplake/core/chunk/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    24544 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26270 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6748 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4944 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4512 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5464 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10139 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   137699 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    39184 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/compression.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.894211 deeplake-3.9.1/deeplake/core/compute/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/compute/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      911 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/compute/process.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2332 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/compute/provider.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      640 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/compute/ray.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      806 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/compute/serial.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      576 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/compute/thread.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.896035 deeplake-3.9.1/deeplake/core/dataset/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   196985 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16167 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12670 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/dataset/indra_dataset_view.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6249 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/dataset/indra_tensor_view.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      760 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4666 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/distance_type.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4348 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.896391 deeplake-3.9.1/deeplake/core/index/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      138 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/index/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    17988 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/index/index.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9539 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/index_maintenance.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    20531 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/io.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4121 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/ipc.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13074 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/link_creds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16646 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2277 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/linked_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2597 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9946 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/lock.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.897181 deeplake-3.9.1/deeplake/core/meta/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       97 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4043 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.899092 deeplake-3.9.1/deeplake/core/meta/encode/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    25591 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3915 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13848 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1551 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3972 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      941 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      683 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.900064 deeplake-3.9.1/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      226 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2237 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1452 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2114 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3673 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2810 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7627 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      503 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    14862 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      906 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/partial_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      971 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/partial_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5269 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/polygon.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.900684 deeplake-3.9.1/deeplake/core/query/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       82 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/query/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12021 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15253 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/query/filter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8905 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/query/query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21165 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2506 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/seed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    23415 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.902824 deeplake-3.9.1/deeplake/core/storage/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      495 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15471 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/azure.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1053 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19256 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/gcs.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13455 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3114 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/indra.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9604 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/local.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    20308 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3705 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/memory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7292 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/provider.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26754 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/storage/s3.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    65084 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tensor.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7571 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tensor_link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5185 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/test_serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.904706 deeplake-3.9.1/deeplake/core/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7674 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      729 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2181 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16372 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_indra_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      913 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_io.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4811 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1833 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      676 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      377 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_seed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1944 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_serialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10543 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tests/test_vdb_indexes.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.905737 deeplake-3.9.1/deeplake/core/tiling/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4790 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1701 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4827 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2893 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1968 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2367 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.906962 deeplake-3.9.1/deeplake/core/transform/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      111 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/transform/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    56175 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    30619 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/transform/transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    11143 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6049 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.907666 deeplake-3.9.1/deeplake/core/vectorstore/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      638 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.908795 deeplake-3.9.1/deeplake/core/vectorstore/dataset_handlers/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      100 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/dataset_handlers/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13355 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      450 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/dataset_handlers/dataset_handler.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6152 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.909275 deeplake-3.9.1/deeplake/core/vectorstore/deep_memory/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       73 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/deep_memory/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26733 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/deep_memory/deep_memory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    24999 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/deep_memory/test_deepmemory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    32155 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/deeplake_vectorstore.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.909902 deeplake-3.9.1/deeplake/core/vectorstore/embeddings/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/embeddings/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3777 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/embeddings/embedder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3131 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/embeddings/test_embedder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    90371 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.910436 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.911048 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      392 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    18849 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    14233 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.911527 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      286 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4396 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4223 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.913050 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5190 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7363 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3657 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.913684 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      275 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      956 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      221 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1406 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.914402 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       93 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5839 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2047 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5205 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.914912 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1924 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2371 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1734 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21909 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3912 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.916163 deeplake-3.9.1/deeplake/core/version_control/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1954 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6337 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3127 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5006 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19869 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    91907 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.919642 deeplake-3.9.1/deeplake/enterprise/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      145 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/enterprise/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8422 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37913 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5967 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6276 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    28963 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3432 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/enterprise/test_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    22675 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1819 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/enterprise/util.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1590 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/hooks.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8558 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/htype.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.919760 deeplake-3.9.1/deeplake/integrations/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       99 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.920024 deeplake-3.9.1/deeplake/integrations/huggingface/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       44 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5503 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.921349 deeplake-3.9.1/deeplake/integrations/mmdet/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    62719 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4740 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19652 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.922574 deeplake-3.9.1/deeplake/integrations/pytorch/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       40 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10179 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7317 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4367 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7282 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.923701 deeplake-3.9.1/deeplake/integrations/tf/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1270 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/tf/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2454 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5331 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.923971 deeplake-3.9.1/deeplake/integrations/wandb/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       21 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12089 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.924639 deeplake-3.9.1/deeplake/requirements/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      487 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/requirements/common.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       71 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/requirements/docs.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/requirements/plugins.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      416 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/requirements/tests.txt
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.925813 deeplake-3.9.1/deeplake/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1404 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2721 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4218 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/tests/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4386 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    25709 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2811 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.941118 deeplake-3.9.1/deeplake/util/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       86 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7370 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/access_method.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1130 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/agreement.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1567 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/array_list.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      619 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2961 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/auto.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5919 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       54 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/bugout_token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3623 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/cache_chain.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4612 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/casting.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      310 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/check_installation.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1213 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/check_latest_version.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3151 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4597 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/class_label.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      231 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1197 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/compute.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5706 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/connect_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1170 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      443 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/delete_entry.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15906 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5181 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/downsample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       84 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/empty_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15642 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37198 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/exceptions.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2026 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/exif.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1803 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/from_tfds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/generate_id.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      306 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/hash.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2901 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/htype.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1517 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/image.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      873 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      135 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1001 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/iteration_warning.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      507 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/join_chunks.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6422 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/json.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7804 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/keys.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3071 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1646 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/logging.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37936 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/merge.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2426 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/modified.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/notebook.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.945146 deeplake-3.9.1/deeplake/util/object_3d/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3374 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1021 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      695 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1323 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6188 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1663 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3221 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10435 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7113 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1087 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4600 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/path.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3220 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/pretty_print.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2844 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/remove_cache.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4511 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/scheduling.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3140 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/shape_interval.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      351 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/shuffle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4784 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/spinner.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1153 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/split.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10033 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/storage.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1131 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tag.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1425 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tensor_db.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      951 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/testing.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.947167 deeplake-3.9.1/deeplake/util/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1476 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1795 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1239 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      628 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_keys.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      892 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_read.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1071 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      429 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      698 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_split.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      974 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      299 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2452 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      559 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/tests/test_video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      276 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/threading.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    27435 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    41390 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/version_control.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1284 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      167 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/util/warnings.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.947627 deeplake-3.9.1/deeplake/visualizer/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       34 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/visualizer/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6466 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6764 2024-04-19 21:51:56.000000 deeplake-3.9.1/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-19 21:53:04.867288 deeplake-3.9.1/deeplake.egg-info/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21937 2024-04-19 21:53:04.000000 deeplake-3.9.1/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13651 2024-04-19 21:53:04.000000 deeplake-3.9.1/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-04-19 21:53:04.000000 deeplake-3.9.1/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-04-19 21:52:45.000000 deeplake-3.9.1/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1109 2024-04-19 21:53:04.000000 deeplake-3.9.1/deeplake.egg-info/requires.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        9 2024-04-19 21:53:04.000000 deeplake-3.9.1/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       63 2024-04-19 21:51:56.000000 deeplake-3.9.1/pyproject.toml
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      311 2024-04-19 21:53:04.948277 deeplake-3.9.1/setup.cfg
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3339 2024-04-19 21:51:56.000000 deeplake-3.9.1/setup.py
```

### Comparing `deeplake-3.9.0/LICENSE` & `deeplake-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/PKG-INFO` & `deeplake-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.9.0
+Version: 3.9.1
 Summary: Activeloop Deep Lake
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -57,15 +57,15 @@
 ## What is Deep Lake?
 
 Deep Lake is a Database for AI powered by a storage format optimized for deep-learning applications. Deep Lake can be used for:
 
 1. Storing data and vectors while building LLM applications
 2. Managing datasets while training deep learning models
    
-Deep Lake simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage, and integrations with popular tools such as LangChain, LlamaIndex, Weights & Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in your own cloud and in one place. Deep Lake is used by Intel, Airbus, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. 
+Deep Lake simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage, and integrations with popular tools such as LangChain, LlamaIndex, Weights & Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in your own cloud and in one place. Deep Lake is used by Intel, Bayer Radiology, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. 
 
 ### Deep Lake includes the following features:
 
 <details>
   <summary><b>Multi-Cloud Support (S3, GCP, Azure)</b></summary>
 Use one API to upload, download, and stream datasets to/from S3, Azure, GCP, Activeloop cloud, local storage, or in-memory storage. Compatible with any S3-compatible storage such as MinIO. 
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.9.0 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.9.1 Summary: Activeloop Deep
 Lake Author: activeloop.ai Author-email: support@activeloop.ai License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/ Project-URL: Source,
 https://github.com/activeloopai/deeplake Classifier: License :: OSI Approved ::
 Mozilla Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown
 Provides-Extra: audio Provides-Extra: video Provides-Extra: av Provides-Extra:
 gcp Provides-Extra: azure Provides-Extra: dicom Provides-Extra: medical
 Provides-Extra: visualizer Provides-Extra: gdrive Provides-Extra: point_cloud
@@ -21,40 +21,40 @@
 deep learning models Deep Lake simplifies the deployment of enterprise-grade
 LLM-based products by offering storage for all data types (embeddings, audio,
 text, videos, images, pdfs, annotations, etc.), querying and vector search,
 data streaming while training models at scale, data versioning and lineage, and
 integrations with popular tools such as LangChain, LlamaIndex, Weights &
 Biases, and many more. Deep Lake works with data of any size, it is serverless,
 and it enables you to store all of your data in your own cloud and in one
-place. Deep Lake is used by Intel, Airbus, Matterport, ZERO Systems, Red Cross,
-Yale, & Oxford. ### Deep Lake includes the following features: MMuullttii--CClloouudd
-SSuuppppoorrtt ((SS33,, GGCCPP,, AAzzuurree)) Use one API to upload, download, and stream datasets
-to/from S3, Azure, GCP, Activeloop cloud, local storage, or in-memory storage.
-Compatible with any S3-compatible storage such as MinIO. NNaattiivvee CCoommpprreessssiioonn
-wwiitthh LLaazzyy NNuummPPyy--lliikkee IInnddeexxiinngg Store images, audio, and videos in their native
-compression. Slice, index, iterate, and interact with your data like a
-collection of NumPy arrays in your system's memory. Deep Lake lazily loads data
-only when needed, e.g., when training a model or running queries. DDaattaasseett
-VVeerrssiioonn CCoonnttrrooll Commits, branches, checkout - Concepts you are already familiar
-with in your code repositories can now be applied to your datasets as well!
-DDaattaallooaaddeerrss ffoorr PPooppuullaarr DDeeeepp LLeeaarrnniinngg FFrraammeewwoorrkkss Deep Lake comes with built-in
-dataloaders for Pytorch and TensorFlow. Train your model with a few lines of
-code - we even take care of dataset shuffling. :) IInntteeggrraattiioonnss wwiitthh PPoowweerrffuull
-TToooollss Deep Lake has integrations with _L_a_n_g_c_h_a_i_n and _L_L_a_m_a_I_n_d_e_x as a vector
-store for LLM apps, _W_e_i_g_h_t_s_ _&_ _B_i_a_s_e_s for data lineage during model training,
-and _M_M_D_e_t_e_c_t_i_o_n for training object detection models. 110000++ mmoosstt--ppooppuullaarr iimmaaggee,,
-vviiddeeoo,, aanndd aauuddiioo ddaattaasseettss aavvaaiillaabbllee iinn sseeccoonnddss Deep Lake community has uploaded
-_1_0_0_+_ _i_m_a_g_e_,_ _v_i_d_e_o_ _a_n_d_ _a_u_d_i_o_ _d_a_t_a_s_e_t_s like _M_N_I_S_T, _C_O_C_O, _I_m_a_g_e_N_e_t, _C_I_F_A_R, _G_T_Z_A_N
-and others. IInnssttaanntt VViissuuaalliizzaattiioonn SSuuppppoorrtt iinn tthhee _DD_ee_ee_pp_ _LL_aa_kk_ee_ _AA_pp_pp Deep Lake
-datasets are instantly visualized with bounding boxes, masks, annotations, etc.
-in _D_e_e_p_ _L_a_k_e_ _V_i_s_u_a_l_i_z_e_r (see below). [![Visualizer](https://
-www.linkpicture.com/q/ReadMe.gif "Visualizer")](https://www.youtube.com/
-watch?v=SxsofpSIw3k) ## ð Performance Deep Lake's performant dataloader
-built in C++ speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et
-al. 2022, Hambardzumyan et al. 2023)
+place. Deep Lake is used by Intel, Bayer Radiology, Matterport, ZERO Systems,
+Red Cross, Yale, & Oxford. ### Deep Lake includes the following features:
+MMuullttii--CClloouudd SSuuppppoorrtt ((SS33,, GGCCPP,, AAzzuurree)) Use one API to upload, download, and
+stream datasets to/from S3, Azure, GCP, Activeloop cloud, local storage, or in-
+memory storage. Compatible with any S3-compatible storage such as MinIO. NNaattiivvee
+CCoommpprreessssiioonn wwiitthh LLaazzyy NNuummPPyy--lliikkee IInnddeexxiinngg Store images, audio, and videos in
+their native compression. Slice, index, iterate, and interact with your data
+like a collection of NumPy arrays in your system's memory. Deep Lake lazily
+loads data only when needed, e.g., when training a model or running queries.
+DDaattaasseett VVeerrssiioonn CCoonnttrrooll Commits, branches, checkout - Concepts you are already
+familiar with in your code repositories can now be applied to your datasets as
+well! DDaattaallooaaddeerrss ffoorr PPooppuullaarr DDeeeepp LLeeaarrnniinngg FFrraammeewwoorrkkss Deep Lake comes with
+built-in dataloaders for Pytorch and TensorFlow. Train your model with a few
+lines of code - we even take care of dataset shuffling. :) IInntteeggrraattiioonnss wwiitthh
+PPoowweerrffuull TToooollss Deep Lake has integrations with _L_a_n_g_c_h_a_i_n and _L_L_a_m_a_I_n_d_e_x as a
+vector store for LLM apps, _W_e_i_g_h_t_s_ _&_ _B_i_a_s_e_s for data lineage during model
+training, and _M_M_D_e_t_e_c_t_i_o_n for training object detection models. 110000++ mmoosstt--
+ppooppuullaarr iimmaaggee,, vviiddeeoo,, aanndd aauuddiioo ddaattaasseettss aavvaaiillaabbllee iinn sseeccoonnddss Deep Lake
+community has uploaded _1_0_0_+_ _i_m_a_g_e_,_ _v_i_d_e_o_ _a_n_d_ _a_u_d_i_o_ _d_a_t_a_s_e_t_s like _M_N_I_S_T, _C_O_C_O,
+_I_m_a_g_e_N_e_t, _C_I_F_A_R, _G_T_Z_A_N and others. IInnssttaanntt VViissuuaalliizzaattiioonn SSuuppppoorrtt iinn tthhee _DD_ee_ee_pp
+_LL_aa_kk_ee_ _AA_pp_pp Deep Lake datasets are instantly visualized with bounding boxes,
+masks, annotations, etc. in _D_e_e_p_ _L_a_k_e_ _V_i_s_u_a_l_i_z_e_r (see below). [![Visualizer]
+(https://www.linkpicture.com/q/ReadMe.gif "Visualizer")](https://
+www.youtube.com/watch?v=SxsofpSIw3k) ## ð Performance Deep Lake's performant
+dataloader built in C++ speeds up data streaming by >2x compared to Hub 2.x
+(Ofeidis et al. 2022, Hambardzumyan et al. 2023)
                    _[_d_o_c_s_/_s_o_u_r_c_e_/___s_t_a_t_i_c_/_i_m_g_/_b_e_n_c_h_m_a_r_k_s_._p_n_g_]
 ## ð How to install Deep Lake Deep Lake can be installed using pip: ```sh
 pip3 install deeplake ``` **By default, Deep Lake does not install dependencies
 for audio, video, google-cloud, and other features. Details on all installation
 options are [available here](https://docs.deeplake.ai/en/latest/
 Installation.html).** ### To access all of Deep Lake's features, please
 register in the [Deep Lake App](https://app.activeloop.ai/register/). ## ð§
```

### Comparing `deeplake-3.9.0/README.md` & `deeplake-3.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ## What is Deep Lake?
 
 Deep Lake is a Database for AI powered by a storage format optimized for deep-learning applications. Deep Lake can be used for:
 
 1. Storing data and vectors while building LLM applications
 2. Managing datasets while training deep learning models
    
-Deep Lake simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage, and integrations with popular tools such as LangChain, LlamaIndex, Weights & Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in your own cloud and in one place. Deep Lake is used by Intel, Airbus, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. 
+Deep Lake simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage, and integrations with popular tools such as LangChain, LlamaIndex, Weights & Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in your own cloud and in one place. Deep Lake is used by Intel, Bayer Radiology, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. 
 
 ### Deep Lake includes the following features:
 
 <details>
   <summary><b>Multi-Cloud Support (S3, GCP, Azure)</b></summary>
 Use one API to upload, download, and stream datasets to/from S3, Azure, GCP, Activeloop cloud, local storage, or in-memory storage. Compatible with any S3-compatible storage such as MinIO. 
 </details>
```

#### html2text {}

```diff
@@ -12,40 +12,40 @@
 deep learning models Deep Lake simplifies the deployment of enterprise-grade
 LLM-based products by offering storage for all data types (embeddings, audio,
 text, videos, images, pdfs, annotations, etc.), querying and vector search,
 data streaming while training models at scale, data versioning and lineage, and
 integrations with popular tools such as LangChain, LlamaIndex, Weights &
 Biases, and many more. Deep Lake works with data of any size, it is serverless,
 and it enables you to store all of your data in your own cloud and in one
-place. Deep Lake is used by Intel, Airbus, Matterport, ZERO Systems, Red Cross,
-Yale, & Oxford. ### Deep Lake includes the following features: MMuullttii--CClloouudd
-SSuuppppoorrtt ((SS33,, GGCCPP,, AAzzuurree)) Use one API to upload, download, and stream datasets
-to/from S3, Azure, GCP, Activeloop cloud, local storage, or in-memory storage.
-Compatible with any S3-compatible storage such as MinIO. NNaattiivvee CCoommpprreessssiioonn
-wwiitthh LLaazzyy NNuummPPyy--lliikkee IInnddeexxiinngg Store images, audio, and videos in their native
-compression. Slice, index, iterate, and interact with your data like a
-collection of NumPy arrays in your system's memory. Deep Lake lazily loads data
-only when needed, e.g., when training a model or running queries. DDaattaasseett
-VVeerrssiioonn CCoonnttrrooll Commits, branches, checkout - Concepts you are already familiar
-with in your code repositories can now be applied to your datasets as well!
-DDaattaallooaaddeerrss ffoorr PPooppuullaarr DDeeeepp LLeeaarrnniinngg FFrraammeewwoorrkkss Deep Lake comes with built-in
-dataloaders for Pytorch and TensorFlow. Train your model with a few lines of
-code - we even take care of dataset shuffling. :) IInntteeggrraattiioonnss wwiitthh PPoowweerrffuull
-TToooollss Deep Lake has integrations with _L_a_n_g_c_h_a_i_n and _L_L_a_m_a_I_n_d_e_x as a vector
-store for LLM apps, _W_e_i_g_h_t_s_ _&_ _B_i_a_s_e_s for data lineage during model training,
-and _M_M_D_e_t_e_c_t_i_o_n for training object detection models. 110000++ mmoosstt--ppooppuullaarr iimmaaggee,,
-vviiddeeoo,, aanndd aauuddiioo ddaattaasseettss aavvaaiillaabbllee iinn sseeccoonnddss Deep Lake community has uploaded
-_1_0_0_+_ _i_m_a_g_e_,_ _v_i_d_e_o_ _a_n_d_ _a_u_d_i_o_ _d_a_t_a_s_e_t_s like _M_N_I_S_T, _C_O_C_O, _I_m_a_g_e_N_e_t, _C_I_F_A_R, _G_T_Z_A_N
-and others. IInnssttaanntt VViissuuaalliizzaattiioonn SSuuppppoorrtt iinn tthhee _DD_ee_ee_pp_ _LL_aa_kk_ee_ _AA_pp_pp Deep Lake
-datasets are instantly visualized with bounding boxes, masks, annotations, etc.
-in _D_e_e_p_ _L_a_k_e_ _V_i_s_u_a_l_i_z_e_r (see below). [![Visualizer](https://
-www.linkpicture.com/q/ReadMe.gif "Visualizer")](https://www.youtube.com/
-watch?v=SxsofpSIw3k) ## ð Performance Deep Lake's performant dataloader
-built in C++ speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et
-al. 2022, Hambardzumyan et al. 2023)
+place. Deep Lake is used by Intel, Bayer Radiology, Matterport, ZERO Systems,
+Red Cross, Yale, & Oxford. ### Deep Lake includes the following features:
+MMuullttii--CClloouudd SSuuppppoorrtt ((SS33,, GGCCPP,, AAzzuurree)) Use one API to upload, download, and
+stream datasets to/from S3, Azure, GCP, Activeloop cloud, local storage, or in-
+memory storage. Compatible with any S3-compatible storage such as MinIO. NNaattiivvee
+CCoommpprreessssiioonn wwiitthh LLaazzyy NNuummPPyy--lliikkee IInnddeexxiinngg Store images, audio, and videos in
+their native compression. Slice, index, iterate, and interact with your data
+like a collection of NumPy arrays in your system's memory. Deep Lake lazily
+loads data only when needed, e.g., when training a model or running queries.
+DDaattaasseett VVeerrssiioonn CCoonnttrrooll Commits, branches, checkout - Concepts you are already
+familiar with in your code repositories can now be applied to your datasets as
+well! DDaattaallooaaddeerrss ffoorr PPooppuullaarr DDeeeepp LLeeaarrnniinngg FFrraammeewwoorrkkss Deep Lake comes with
+built-in dataloaders for Pytorch and TensorFlow. Train your model with a few
+lines of code - we even take care of dataset shuffling. :) IInntteeggrraattiioonnss wwiitthh
+PPoowweerrffuull TToooollss Deep Lake has integrations with _L_a_n_g_c_h_a_i_n and _L_L_a_m_a_I_n_d_e_x as a
+vector store for LLM apps, _W_e_i_g_h_t_s_ _&_ _B_i_a_s_e_s for data lineage during model
+training, and _M_M_D_e_t_e_c_t_i_o_n for training object detection models. 110000++ mmoosstt--
+ppooppuullaarr iimmaaggee,, vviiddeeoo,, aanndd aauuddiioo ddaattaasseettss aavvaaiillaabbllee iinn sseeccoonnddss Deep Lake
+community has uploaded _1_0_0_+_ _i_m_a_g_e_,_ _v_i_d_e_o_ _a_n_d_ _a_u_d_i_o_ _d_a_t_a_s_e_t_s like _M_N_I_S_T, _C_O_C_O,
+_I_m_a_g_e_N_e_t, _C_I_F_A_R, _G_T_Z_A_N and others. IInnssttaanntt VViissuuaalliizzaattiioonn SSuuppppoorrtt iinn tthhee _DD_ee_ee_pp
+_LL_aa_kk_ee_ _AA_pp_pp Deep Lake datasets are instantly visualized with bounding boxes,
+masks, annotations, etc. in _D_e_e_p_ _L_a_k_e_ _V_i_s_u_a_l_i_z_e_r (see below). [![Visualizer]
+(https://www.linkpicture.com/q/ReadMe.gif "Visualizer")](https://
+www.youtube.com/watch?v=SxsofpSIw3k) ## ð Performance Deep Lake's performant
+dataloader built in C++ speeds up data streaming by >2x compared to Hub 2.x
+(Ofeidis et al. 2022, Hambardzumyan et al. 2023)
                    _[_d_o_c_s_/_s_o_u_r_c_e_/___s_t_a_t_i_c_/_i_m_g_/_b_e_n_c_h_m_a_r_k_s_._p_n_g_]
 ## ð How to install Deep Lake Deep Lake can be installed using pip: ```sh
 pip3 install deeplake ``` **By default, Deep Lake does not install dependencies
 for audio, video, google-cloud, and other features. Details on all installation
 options are [available here](https://docs.deeplake.ai/en/latest/
 Installation.html).** ### To access all of Deep Lake's features, please
 register in the [Deep Lake App](https://app.activeloop.ai/register/). ## ð§
```

### Comparing `deeplake-3.9.0/deeplake/__init__.py` & `deeplake-3.9.1/deeplake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     "copy",
     "query",
     "rename",
     "random",
 ]
 
 
-__version__ = "3.9.0"
+__version__ = "3.9.1"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
```

### Comparing `deeplake-3.9.0/deeplake/api/dataset.py` & `deeplake-3.9.1/deeplake/api/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,24 @@
 )
 from deeplake.util.compute import get_compute_provider
 from deeplake.util.remove_cache import get_base_storage
 from deeplake.util.cache_chain import generate_chain
 from deeplake.core.storage.deeplake_memory_object import DeepLakeMemoryObject
 
 
+def _check_indra_and_read_only_flags(indra: bool, read_only: Optional[bool]):
+    if indra == False:
+        return
+    if read_only == True:
+        return
+    raise ValueError(
+        "'indra = True' is only available for read_only datasets. Please also specify 'read_only = True'."
+    )
+
+
 class dataset:
     @staticmethod
     @spinner
     def init(
         path: Union[str, pathlib.Path],
         runtime: Optional[Dict] = None,
         read_only: Optional[bool] = None,
@@ -202,14 +212,15 @@
 
         Warning:
             Setting ``access_method`` to download will overwrite the local copy of the dataset if it was previously downloaded.
 
         Note:
             Any changes made to the dataset in download / local mode will only be made to the local copy and will not be reflected in the original dataset.
         """
+        _check_indra_and_read_only_flags(indra, read_only)
         access_method, num_workers, scheduler = parse_access_method(access_method)
         check_access_method(access_method, overwrite, unlink)
 
         path, address = process_dataset_path(path)
         verify_dataset_name(path)
 
         if org_id is not None and get_path_type(path) != "local":
@@ -379,15 +390,14 @@
         creds: Optional[Union[Dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         lock_enabled: Optional[bool] = True,
         lock_timeout: Optional[int] = 0,
         verbose: bool = True,
         index_params: Optional[Dict[str, Union[int, str]]] = None,
-        indra: bool = USE_INDRA,
     ) -> Dataset:
         """Creates an empty dataset
 
         Args:
             path (str, pathlib.Path): - The full path to the dataset. It can be:
                 - a Deep Lake cloud path of the form ``hub://org_id/dataset_name``. Requires registration with Deep Lake.
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
@@ -404,15 +414,14 @@
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling high-performance features. Only applicable for local datasets.
             verbose (bool): If True, logs will be printed. Defaults to True.
             lock_timeout (int): Number of seconds to wait before throwing a LockException. If None, wait indefinitely
             lock_enabled (bool): If true, the dataset manages a write lock. NOTE: Only set to False if you are managing concurrent access externally.
             index_params: Optional[Dict[str, Union[int, str]]]: Index parameters used while creating vector store, passed down to dataset.
-            indra (bool): Flag indicating whether indra api should be used to create the dataset. Defaults to false
 
         Returns:
             Dataset: Dataset created using the arguments provided.
 
         Raises:
             DatasetHandlerError: If a Dataset already exists at the given path and overwrite is False.
             UserNotLoggedInException: When user is not authenticated
@@ -444,15 +453,14 @@
                 path=path,
                 db_engine=db_engine,
                 read_only=False,
                 creds=creds,
                 token=token,
                 memory_cache_size=memory_cache_size,
                 local_cache_size=local_cache_size,
-                indra=indra,
             )
 
             feature_report_path(
                 path,
                 "empty",
                 {
                     "runtime": runtime,
@@ -611,14 +619,15 @@
 
         Warning:
             Setting ``access_method`` to download will overwrite the local copy of the dataset if it was previously downloaded.
 
         Note:
             Any changes made to the dataset in download / local mode will only be made to the local copy and will not be reflected in the original dataset.
         """
+        _check_indra_and_read_only_flags(indra, read_only)
         access_method, num_workers, scheduler = parse_access_method(access_method)
         check_access_method(access_method, overwrite=False, unlink=unlink)
 
         path, address = process_dataset_path(path)
 
         if creds is None:
             creds = {}
@@ -1504,15 +1513,14 @@
         dest_creds: Optional[Union[str, Dict]] = None,
         inspect_limit: int = 1000000,
         progressbar: bool = True,
         shuffle: bool = False,
         num_workers: int = 0,
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
-        indra: bool = USE_INDRA,
         **dataset_kwargs,
     ) -> Dataset:
         """Ingest images and annotations in COCO format to a Deep Lake Dataset. The source data can be stored locally or in the cloud.
 
         Examples:
             >>> # Ingest local data in COCO format to a Deep Lake dataset stored in Deep Lake storage.
             >>> ds = deeplake.ingest_coco(
@@ -1558,15 +1566,14 @@
             dest_creds (Optional[Union[str, Dict]]): The string ``ENV`` or a dictionary containing credentials used to access the destination path of the dataset.
             inspect_limit (int): The maximum number of samples to inspect in the annotations json, in order to generate the set of COCO annotation keys. Set to ``1000000`` by default.
             progressbar (bool): Enables or disables ingestion progress bar. Set to ``True`` by default.
             shuffle (bool): Shuffles the input data prior to ingestion. Set to ``False`` by default.
             num_workers (int): The number of workers to use for ingestion. Set to ``0`` by default.
             token (Optional[str]): The token to use for accessing the dataset and/or connecting it to Deep Lake.
             connect_kwargs (Optional[Dict]): If specified, the dataset will be connected to Deep Lake, and connect_kwargs will be passed to :meth:`Dataset.connect <deeplake.core.dataset.Dataset.connect>`.
-            indra (bool): Flag indicating whether indra api should be used to create the dataset. Defaults to false
             **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function. See :func:`deeplake.empty`.
 
         Returns:
             Dataset: The Dataset created from images and COCO annotations.
 
         Raises:
             IngestionError: If either ``key_to_tensor_mapping`` or ``file_to_group_mapping`` are not one-to-one.
@@ -1601,15 +1608,14 @@
         structure = unstructured.prepare_structure(inspect_limit)
 
         ds = deeplake.empty(
             dest,
             creds=dest_creds,
             verbose=False,
             token=token,
-            indra=indra,
             **dataset_kwargs,
         )
         if connect_kwargs is not None:
             connect_kwargs["token"] = token or connect_kwargs.get("token")
             ds.connect(**connect_kwargs)
 
         structure.create_missing(ds)
@@ -1633,15 +1639,14 @@
         image_creds_key: Optional[str] = None,
         inspect_limit: int = 1000,
         progressbar: bool = True,
         shuffle: bool = False,
         num_workers: int = 0,
         token: Optional[str] = None,
         connect_kwargs: Optional[Dict] = None,
-        indra: bool = USE_INDRA,
         **dataset_kwargs,
     ) -> Dataset:
         """Ingest images and annotations (bounding boxes or polygons) in YOLO format to a Deep Lake Dataset. The source data can be stored locally or in the cloud.
 
         Examples:
             >>> # Ingest local data in YOLO format to a Deep Lake dataset stored in Deep Lake storage.
             >>> ds = deeplake.ingest_yolo(
@@ -1682,15 +1687,14 @@
             image_creds_key (Optional[str]): creds_key for linked tensors, applicable if the htype for the images tensor is specified as 'link[image]' in the 'image_params' input.
             inspect_limit (int): The maximum number of annotations to inspect, in order to infer whether they are bounding boxes of polygons. This in put is ignored if the htype is specfied in the 'coordinates_params'.
             progressbar (bool): Enables or disables ingestion progress bar. Set to ``True`` by default.
             shuffle (bool): Shuffles the input data prior to ingestion. Set to ``False`` by default.
             num_workers (int): The number of workers to use for ingestion. Set to ``0`` by default.
             token (Optional[str]): The token to use for accessing the dataset and/or connecting it to Deep Lake.
             connect_kwargs (Optional[Dict]): If specified, the dataset will be connected to Deep Lake, and connect_kwargs will be passed to :meth:`Dataset.connect <deeplake.core.dataset.Dataset.connect>`.
-            indra (bool): Flag indicating whether indra api should be used to create the dataset. Defaults to false
             **dataset_kwargs: Any arguments passed here will be forwarded to the dataset creator function. See :func:`deeplake.empty`.
 
         Returns:
             Dataset: The Dataset created from the images and YOLO annotations.
 
         Raises:
             IngestionError: If annotations are not found for all the images and 'allow_no_annotation' is False
@@ -1734,15 +1738,14 @@
         structure = unstructured.prepare_structure()
 
         ds = deeplake.empty(
             dest,
             creds=dest_creds,
             verbose=False,
             token=token,
-            indra=indra,
             **dataset_kwargs,
         )
         if connect_kwargs is not None:
             connect_kwargs["token"] = token or connect_kwargs.get("token")
             ds.connect(**connect_kwargs)
 
         structure.create_missing(ds)
@@ -1895,15 +1898,14 @@
             unstructured = ImageClassification(source=src)
 
             ds = deeplake.empty(
                 dest,
                 creds=dest_creds,
                 token=token,
                 verbose=False,
-                indra=indra,
                 **dataset_kwargs,
             )
             if connect_kwargs is not None:
                 connect_kwargs["token"] = token or connect_kwargs.get("token")
                 ds.connect(**connect_kwargs)
 
             # TODO: auto detect compression
```

### Comparing `deeplake-3.9.0/deeplake/api/info.py` & `deeplake-3.9.1/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/link.py` & `deeplake-3.9.1/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/link_tiled.py` & `deeplake-3.9.1/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/read.py` & `deeplake-3.9.1/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_access_method.py` & `deeplake-3.9.1/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_agreement.py` & `deeplake-3.9.1/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_api.py` & `deeplake-3.9.1/deeplake/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.9.1/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.9.1/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.9.1/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.9.1/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_dataset.py` & `deeplake-3.9.1/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_dicom.py` & `deeplake-3.9.1/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_downsample.py` & `deeplake-3.9.1/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_events.py` & `deeplake-3.9.1/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_grayscale.py` & `deeplake-3.9.1/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_info.py` & `deeplake-3.9.1/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.9.1/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_json.py` & `deeplake-3.9.1/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_link.py` & `deeplake-3.9.1/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.9.1/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_linking.py` & `deeplake-3.9.1/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_mesh.py` & `deeplake-3.9.1/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_meta.py` & `deeplake-3.9.1/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_nifti.py` & `deeplake-3.9.1/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_none.py` & `deeplake-3.9.1/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.9.1/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_pickle.py` & `deeplake-3.9.1/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.9.1/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_polygons.py` & `deeplake-3.9.1/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_pop.py` & `deeplake-3.9.1/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_readonly.py` & `deeplake-3.9.1/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_rechunk.py` & `deeplake-3.9.1/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_reset.py` & `deeplake-3.9.1/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_sample_info.py` & `deeplake-3.9.1/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_tag.py` & `deeplake-3.9.1/deeplake/api/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_text.py` & `deeplake-3.9.1/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_update_samples.py` & `deeplake-3.9.1/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_video.py` & `deeplake-3.9.1/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tests/test_views.py` & `deeplake-3.9.1/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/api/tiled.py` & `deeplake-3.9.1/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/structured/base.py` & `deeplake-3.9.1/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/structured/dataframe.py` & `deeplake-3.9.1/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.9.1/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.9.1/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.9.1/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.9.1/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/unstructured/base.py` & `deeplake-3.9.1/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.9.1/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.9.1/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.9.1/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.9.1/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.9.1/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.9.1/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/unstructured/util.py` & `deeplake-3.9.1/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.9.1/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.9.1/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/client/auth/__init__.py` & `deeplake-3.9.1/deeplake/client/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/client/auth/activeloop.py` & `deeplake-3.9.1/deeplake/client/auth/activeloop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/client/auth/auth_context.py` & `deeplake-3.9.1/deeplake/client/auth/auth_context.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/client/auth/azure.py` & `deeplake-3.9.1/deeplake/client/auth/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/client/auth/test_auth_context.py` & `deeplake-3.9.1/deeplake/client/auth/test_auth_context.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/client/client.py` & `deeplake-3.9.1/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/client/config.py` & `deeplake-3.9.1/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/client/log.py` & `deeplake-3.9.1/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/client/test_client.py` & `deeplake-3.9.1/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/client/utils.py` & `deeplake-3.9.1/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/compression.py` & `deeplake-3.9.1/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/constants.py` & `deeplake-3.9.1/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/chunk/base_chunk.py` & `deeplake-3.9.1/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.9.1/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.9.1/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.9.1/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.9.1/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.9.1/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.9.1/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/chunk_engine.py` & `deeplake-3.9.1/deeplake/core/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/compression.py` & `deeplake-3.9.1/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/compute/process.py` & `deeplake-3.9.1/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/compute/provider.py` & `deeplake-3.9.1/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/compute/ray.py` & `deeplake-3.9.1/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/compute/serial.py` & `deeplake-3.9.1/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/compute/thread.py` & `deeplake-3.9.1/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/dataset/__init__.py` & `deeplake-3.9.1/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/dataset/dataset.py` & `deeplake-3.9.1/deeplake/core/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -2104,22 +2104,23 @@
             shuffle (bool): If ``True``, the data loader will shuffle the data indices. Default value is False. Details about how Deep Lake shuffles data can be found at `Shuffling in ds.pytorch() <https://docs.activeloop.ai/how-it-works/shuffling-in-ds.pytorch>`_
             buffer_size (int): The size of the buffer used to shuffle the data in MBs. Defaults to 2048 MB. Increasing the buffer_size will increase the extent of shuffling.
             use_local_cache (bool): If ``True``, the data loader will use a local cache to store data. The default cache location is ~/.activeloop/cache, but it can be changed by setting the ``LOCAL_CACHE_PREFIX`` environment variable. This is useful when the dataset can fit on the machine and we don't want to fetch the data multiple times for each iteration. Default value is ``False``
             progressbar (bool): If ``True``, tqdm will be wrapped around the returned dataloader. Default value is True.
             return_index (bool): If ``True``, the returned dataloader will have a key "index" that contains the index of the sample(s) in the original dataset. Default value is True.
             pad_tensors (bool): If ``True``, shorter tensors will be padded to the length of the longest tensor. Default value is False.
             transform_kwargs (optional, Dict[str, Any]): Additional kwargs to be passed to ``transform``.
-            decode_method (Dict[str, str], Optional): A dictionary of decode methods for each tensor. Defaults to ``None``.
+            decode_method (Dict[str, str], Optional): The method for decoding the Deep Lake tensor data, the result of which is passed to the transform. Decoding occurs outside of the transform so that it can be performed in parallel and as rapidly as possible as per Deep Lake optimizations.
 
                 - Supported decode methods are:
-
-                    :'numpy': Default behaviour. Returns samples as numpy arrays.
-                    :'tobytes': Returns raw bytes of the samples.
+                    :'numpy': Default behaviour. Returns samples as numpy arrays, the same as ds.tensor[i].numpy()
+                    :'tobytes': Returns raw bytes of the samples the same as ds.tensor[i].tobytes()
+                    :'data': Returns a dictionary with keys,values depending on htype, the same as ds.tensor[i].data()
                     :'pil': Returns samples as PIL images. Especially useful when transformation use torchvision transforms, that
                             require PIL images as input. Only supported for tensors with ``sample_compression='jpeg'`` or ``'png'``.
+
             cache_size (int): The size of the cache per tensor in MBs. Defaults to max(maximum chunk size of tensor, 32 MB).
 
         ..
             # noqa: DAR101
 
         Returns:
             A torch.utils.data.DataLoader object.
```

### Comparing `deeplake-3.9.0/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.9.1/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/dataset/indra_dataset_view.py` & `deeplake-3.9.1/deeplake/core/dataset/indra_dataset_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/dataset/indra_tensor_view.py` & `deeplake-3.9.1/deeplake/core/dataset/indra_tensor_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import deeplake.util.shape_interval as shape_interval
 from deeplake.core import tensor
-from typing import List, Union, Optional
+from typing import Dict, List, Union, Optional
 from deeplake.core.index import Index
 from deeplake.core.tensor import Any
 import numpy as np
 from deeplake.core.index import replace_ellipsis_with_slices
 from deeplake.core.meta.tensor_meta import TensorMeta
 from deeplake.util.exceptions import InvalidKeyTypeError, DynamicTensorNumpyError
 from deeplake.util.pretty_print import summary_tensor
@@ -148,14 +148,24 @@
     def index(self):
         try:
             return Index(self.indra_tensor.indexes)
         except:
             return Index(slice(0, len(self)))
 
     @property
+    def sample_info(self):
+        try:
+            r = self.indra_tensor.sample_info
+            if not self.index.values[0].subscriptable():
+                r = r[0]
+            return r
+        except:
+            return None
+
+    @property
     def shape_interval(self):
         return shape_interval.ShapeInterval(
             (len(self),) + self.min_shape, (len(self),) + self.max_shape
         )
 
     @property
     def ndim(self):
```

### Comparing `deeplake-3.9.0/deeplake/core/dataset/invalid_view.py` & `deeplake-3.9.1/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/dataset/view_entry.py` & `deeplake-3.9.1/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/fast_forwarding.py` & `deeplake-3.9.1/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/index/index.py` & `deeplake-3.9.1/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/index_maintenance.py` & `deeplake-3.9.1/deeplake/core/index_maintenance.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/io.py` & `deeplake-3.9.1/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/ipc.py` & `deeplake-3.9.1/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/link_creds.py` & `deeplake-3.9.1/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/linked_chunk_engine.py` & `deeplake-3.9.1/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/linked_sample.py` & `deeplake-3.9.1/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/linked_tiled_sample.py` & `deeplake-3.9.1/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/lock.py` & `deeplake-3.9.1/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/dataset_meta.py` & `deeplake-3.9.1/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.9.1/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.9.1/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.9.1/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/creds.py` & `deeplake-3.9.1/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/pad.py` & `deeplake-3.9.1/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/sequence.py` & `deeplake-3.9.1/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/shape.py` & `deeplake-3.9.1/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.9.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.9.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.9.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.9.1/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.9.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/encode/tile.py` & `deeplake-3.9.1/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/meta/tensor_meta.py` & `deeplake-3.9.1/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/partial_reader.py` & `deeplake-3.9.1/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/partial_sample.py` & `deeplake-3.9.1/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/polygon.py` & `deeplake-3.9.1/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/query/autocomplete.py` & `deeplake-3.9.1/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/query/filter.py` & `deeplake-3.9.1/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/query/query.py` & `deeplake-3.9.1/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/sample.py` & `deeplake-3.9.1/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/seed.py` & `deeplake-3.9.1/deeplake/core/seed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/serialize.py` & `deeplake-3.9.1/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/storage/azure.py` & `deeplake-3.9.1/deeplake/core/storage/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.9.1/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/storage/gcs.py` & `deeplake-3.9.1/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/storage/google_drive.py` & `deeplake-3.9.1/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/storage/indra.py` & `deeplake-3.9.1/deeplake/core/storage/indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/storage/local.py` & `deeplake-3.9.1/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/storage/lru_cache.py` & `deeplake-3.9.1/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/storage/memory.py` & `deeplake-3.9.1/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/storage/provider.py` & `deeplake-3.9.1/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/storage/s3.py` & `deeplake-3.9.1/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tensor.py` & `deeplake-3.9.1/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tensor_link.py` & `deeplake-3.9.1/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/test_serialize.py` & `deeplake-3.9.1/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tests/test_compression.py` & `deeplake-3.9.1/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tests/test_compute.py` & `deeplake-3.9.1/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tests/test_dataset.py` & `deeplake-3.9.1/deeplake/core/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tests/test_indra_dataset.py` & `deeplake-3.9.1/deeplake/core/tests/test_indra_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
         )
         for i in range(100):
             deeplake_ds.label.append(int(i / 10))
             deeplake_ds.image.append(np.random.randint(0, 255, (100, 200, 3), np.uint8))
 
     indra_ds = dataset_to_libdeeplake(deeplake_ds)
     deeplake_indra_ds = IndraDatasetView(indra_ds=indra_ds)
+    assert deeplake_indra_ds.image.sample_info == deeplake_ds.image.sample_info
 
     view = deeplake_indra_ds.query("SELECT * GROUP BY label")
     assert len(view) == 10
     assert view.label.shape == view.tensors["label"].shape
     for i in range(len(view)):
         arr = view.label[i].numpy()
         assert len(arr) == 10
```

### Comparing `deeplake-3.9.0/deeplake/core/tests/test_io.py` & `deeplake-3.9.1/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tests/test_locking.py` & `deeplake-3.9.1/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tests/test_query.py` & `deeplake-3.9.1/deeplake/core/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tests/test_readonly.py` & `deeplake-3.9.1/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tests/test_serialize.py` & `deeplake-3.9.1/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tests/test_vdb_indexes.py` & `deeplake-3.9.1/deeplake/core/tests/test_vdb_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tiling/deserialize.py` & `deeplake-3.9.1/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tiling/optimizer.py` & `deeplake-3.9.1/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.9.1/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tiling/serialize.py` & `deeplake-3.9.1/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.9.1/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/tiling/test_serialize.py` & `deeplake-3.9.1/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/transform/test_transform.py` & `deeplake-3.9.1/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/transform/transform.py` & `deeplake-3.9.1/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/transform/transform_dataset.py` & `deeplake-3.9.1/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/transform/transform_tensor.py` & `deeplake-3.9.1/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/__init__.py` & `deeplake-3.9.1/deeplake/core/vectorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py` & `deeplake-3.9.1/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py` & `deeplake-3.9.1/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/deep_memory/deep_memory.py` & `deeplake-3.9.1/deeplake/core/vectorstore/deep_memory/deep_memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/deep_memory/test_deepmemory.py` & `deeplake-3.9.1/deeplake/core/vectorstore/deep_memory/test_deepmemory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.9.1/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/embeddings/embedder.py` & `deeplake-3.9.1/deeplake/core/vectorstore/embeddings/embedder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/embeddings/test_embedder.py` & `deeplake-3.9.1/deeplake/core/vectorstore/embeddings/test_embedder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.9.1/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/indra/vector_search.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/indra/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/python/search_algorithm.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/python/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/python/test_vector_search.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/python/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.9.1/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.9.1/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/version_control/commit_diff.py` & `deeplake-3.9.1/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/version_control/commit_node.py` & `deeplake-3.9.1/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.9.1/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/version_control/test_merge.py` & `deeplake-3.9.1/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/core/version_control/test_version_control.py` & `deeplake-3.9.1/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.9.1/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/enterprise/dataloader.py` & `deeplake-3.9.1/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.9.1/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.9.1/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/enterprise/test_pytorch.py` & `deeplake-3.9.1/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/enterprise/test_query.py` & `deeplake-3.9.1/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.9.1/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/enterprise/util.py` & `deeplake-3.9.1/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/hooks.py` & `deeplake-3.9.1/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/htype.py` & `deeplake-3.9.1/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.9.1/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.9.1/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.9.1/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.9.1/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/pytorch/common.py` & `deeplake-3.9.1/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.9.1/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.9.1/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.9.1/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/tf/common.py` & `deeplake-3.9.1/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.9.1/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.9.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/integrations/wandb/wandb.py` & `deeplake-3.9.1/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/tests/cache_fixtures.py` & `deeplake-3.9.1/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/tests/client_fixtures.py` & `deeplake-3.9.1/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/tests/common.py` & `deeplake-3.9.1/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/tests/dataset_fixtures.py` & `deeplake-3.9.1/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/tests/path_fixtures.py` & `deeplake-3.9.1/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/tests/storage_fixtures.py` & `deeplake-3.9.1/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/access_method.py` & `deeplake-3.9.1/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/agreement.py` & `deeplake-3.9.1/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/array_list.py` & `deeplake-3.9.1/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/assert_byte_indexes.py` & `deeplake-3.9.1/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/auto.py` & `deeplake-3.9.1/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/bugout_reporter.py` & `deeplake-3.9.1/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/cache_chain.py` & `deeplake-3.9.1/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/casting.py` & `deeplake-3.9.1/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/check_latest_version.py` & `deeplake-3.9.1/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/chunk_engine.py` & `deeplake-3.9.1/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/class_label.py` & `deeplake-3.9.1/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/compute.py` & `deeplake-3.9.1/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/connect_dataset.py` & `deeplake-3.9.1/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/dataset.py` & `deeplake-3.9.1/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/diff.py` & `deeplake-3.9.1/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/downsample.py` & `deeplake-3.9.1/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/encoder.py` & `deeplake-3.9.1/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/exceptions.py` & `deeplake-3.9.1/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/exif.py` & `deeplake-3.9.1/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/from_tfds.py` & `deeplake-3.9.1/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/htype.py` & `deeplake-3.9.1/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/image.py` & `deeplake-3.9.1/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/invalid_view_op.py` & `deeplake-3.9.1/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/iteration_warning.py` & `deeplake-3.9.1/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/json.py` & `deeplake-3.9.1/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/keys.py` & `deeplake-3.9.1/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/link.py` & `deeplake-3.9.1/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/logging.py` & `deeplake-3.9.1/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/merge.py` & `deeplake-3.9.1/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/modified.py` & `deeplake-3.9.1/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/notebook.py` & `deeplake-3.9.1/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/object_3d/mesh.py` & `deeplake-3.9.1/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.9.1/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.9.1/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.9.1/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.9.1/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.9.1/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.9.1/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.9.1/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.9.1/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.9.1/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/path.py` & `deeplake-3.9.1/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/pretty_print.py` & `deeplake-3.9.1/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/remove_cache.py` & `deeplake-3.9.1/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/scheduling.py` & `deeplake-3.9.1/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/shape_interval.py` & `deeplake-3.9.1/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/spinner.py` & `deeplake-3.9.1/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/split.py` & `deeplake-3.9.1/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/storage.py` & `deeplake-3.9.1/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tag.py` & `deeplake-3.9.1/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tensor_db.py` & `deeplake-3.9.1/deeplake/util/tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/testing.py` & `deeplake-3.9.1/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tests/test_auto.py` & `deeplake-3.9.1/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.9.1/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.9.1/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tests/test_keys.py` & `deeplake-3.9.1/deeplake/util/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tests/test_read.py` & `deeplake-3.9.1/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.9.1/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tests/test_split.py` & `deeplake-3.9.1/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tests/test_tensor_db.py` & `deeplake-3.9.1/deeplake/util/tests/test_tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tests/test_version_control.py` & `deeplake-3.9.1/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/tests/test_video.py` & `deeplake-3.9.1/deeplake/util/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/transform.py` & `deeplake-3.9.1/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/version_control.py` & `deeplake-3.9.1/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/util/video.py` & `deeplake-3.9.1/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/visualizer/video_streaming.py` & `deeplake-3.9.1/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake/visualizer/visualizer.py` & `deeplake-3.9.1/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake.egg-info/PKG-INFO` & `deeplake-3.9.1/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.9.0
+Version: 3.9.1
 Summary: Activeloop Deep Lake
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -57,15 +57,15 @@
 ## What is Deep Lake?
 
 Deep Lake is a Database for AI powered by a storage format optimized for deep-learning applications. Deep Lake can be used for:
 
 1. Storing data and vectors while building LLM applications
 2. Managing datasets while training deep learning models
    
-Deep Lake simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage, and integrations with popular tools such as LangChain, LlamaIndex, Weights & Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in your own cloud and in one place. Deep Lake is used by Intel, Airbus, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. 
+Deep Lake simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage, and integrations with popular tools such as LangChain, LlamaIndex, Weights & Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in your own cloud and in one place. Deep Lake is used by Intel, Bayer Radiology, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. 
 
 ### Deep Lake includes the following features:
 
 <details>
   <summary><b>Multi-Cloud Support (S3, GCP, Azure)</b></summary>
 Use one API to upload, download, and stream datasets to/from S3, Azure, GCP, Activeloop cloud, local storage, or in-memory storage. Compatible with any S3-compatible storage such as MinIO. 
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.9.0 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.9.1 Summary: Activeloop Deep
 Lake Author: activeloop.ai Author-email: support@activeloop.ai License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/ Project-URL: Source,
 https://github.com/activeloopai/deeplake Classifier: License :: OSI Approved ::
 Mozilla Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown
 Provides-Extra: audio Provides-Extra: video Provides-Extra: av Provides-Extra:
 gcp Provides-Extra: azure Provides-Extra: dicom Provides-Extra: medical
 Provides-Extra: visualizer Provides-Extra: gdrive Provides-Extra: point_cloud
@@ -21,40 +21,40 @@
 deep learning models Deep Lake simplifies the deployment of enterprise-grade
 LLM-based products by offering storage for all data types (embeddings, audio,
 text, videos, images, pdfs, annotations, etc.), querying and vector search,
 data streaming while training models at scale, data versioning and lineage, and
 integrations with popular tools such as LangChain, LlamaIndex, Weights &
 Biases, and many more. Deep Lake works with data of any size, it is serverless,
 and it enables you to store all of your data in your own cloud and in one
-place. Deep Lake is used by Intel, Airbus, Matterport, ZERO Systems, Red Cross,
-Yale, & Oxford. ### Deep Lake includes the following features: MMuullttii--CClloouudd
-SSuuppppoorrtt ((SS33,, GGCCPP,, AAzzuurree)) Use one API to upload, download, and stream datasets
-to/from S3, Azure, GCP, Activeloop cloud, local storage, or in-memory storage.
-Compatible with any S3-compatible storage such as MinIO. NNaattiivvee CCoommpprreessssiioonn
-wwiitthh LLaazzyy NNuummPPyy--lliikkee IInnddeexxiinngg Store images, audio, and videos in their native
-compression. Slice, index, iterate, and interact with your data like a
-collection of NumPy arrays in your system's memory. Deep Lake lazily loads data
-only when needed, e.g., when training a model or running queries. DDaattaasseett
-VVeerrssiioonn CCoonnttrrooll Commits, branches, checkout - Concepts you are already familiar
-with in your code repositories can now be applied to your datasets as well!
-DDaattaallooaaddeerrss ffoorr PPooppuullaarr DDeeeepp LLeeaarrnniinngg FFrraammeewwoorrkkss Deep Lake comes with built-in
-dataloaders for Pytorch and TensorFlow. Train your model with a few lines of
-code - we even take care of dataset shuffling. :) IInntteeggrraattiioonnss wwiitthh PPoowweerrffuull
-TToooollss Deep Lake has integrations with _L_a_n_g_c_h_a_i_n and _L_L_a_m_a_I_n_d_e_x as a vector
-store for LLM apps, _W_e_i_g_h_t_s_ _&_ _B_i_a_s_e_s for data lineage during model training,
-and _M_M_D_e_t_e_c_t_i_o_n for training object detection models. 110000++ mmoosstt--ppooppuullaarr iimmaaggee,,
-vviiddeeoo,, aanndd aauuddiioo ddaattaasseettss aavvaaiillaabbllee iinn sseeccoonnddss Deep Lake community has uploaded
-_1_0_0_+_ _i_m_a_g_e_,_ _v_i_d_e_o_ _a_n_d_ _a_u_d_i_o_ _d_a_t_a_s_e_t_s like _M_N_I_S_T, _C_O_C_O, _I_m_a_g_e_N_e_t, _C_I_F_A_R, _G_T_Z_A_N
-and others. IInnssttaanntt VViissuuaalliizzaattiioonn SSuuppppoorrtt iinn tthhee _DD_ee_ee_pp_ _LL_aa_kk_ee_ _AA_pp_pp Deep Lake
-datasets are instantly visualized with bounding boxes, masks, annotations, etc.
-in _D_e_e_p_ _L_a_k_e_ _V_i_s_u_a_l_i_z_e_r (see below). [![Visualizer](https://
-www.linkpicture.com/q/ReadMe.gif "Visualizer")](https://www.youtube.com/
-watch?v=SxsofpSIw3k) ## ð Performance Deep Lake's performant dataloader
-built in C++ speeds up data streaming by >2x compared to Hub 2.x (Ofeidis et
-al. 2022, Hambardzumyan et al. 2023)
+place. Deep Lake is used by Intel, Bayer Radiology, Matterport, ZERO Systems,
+Red Cross, Yale, & Oxford. ### Deep Lake includes the following features:
+MMuullttii--CClloouudd SSuuppppoorrtt ((SS33,, GGCCPP,, AAzzuurree)) Use one API to upload, download, and
+stream datasets to/from S3, Azure, GCP, Activeloop cloud, local storage, or in-
+memory storage. Compatible with any S3-compatible storage such as MinIO. NNaattiivvee
+CCoommpprreessssiioonn wwiitthh LLaazzyy NNuummPPyy--lliikkee IInnddeexxiinngg Store images, audio, and videos in
+their native compression. Slice, index, iterate, and interact with your data
+like a collection of NumPy arrays in your system's memory. Deep Lake lazily
+loads data only when needed, e.g., when training a model or running queries.
+DDaattaasseett VVeerrssiioonn CCoonnttrrooll Commits, branches, checkout - Concepts you are already
+familiar with in your code repositories can now be applied to your datasets as
+well! DDaattaallooaaddeerrss ffoorr PPooppuullaarr DDeeeepp LLeeaarrnniinngg FFrraammeewwoorrkkss Deep Lake comes with
+built-in dataloaders for Pytorch and TensorFlow. Train your model with a few
+lines of code - we even take care of dataset shuffling. :) IInntteeggrraattiioonnss wwiitthh
+PPoowweerrffuull TToooollss Deep Lake has integrations with _L_a_n_g_c_h_a_i_n and _L_L_a_m_a_I_n_d_e_x as a
+vector store for LLM apps, _W_e_i_g_h_t_s_ _&_ _B_i_a_s_e_s for data lineage during model
+training, and _M_M_D_e_t_e_c_t_i_o_n for training object detection models. 110000++ mmoosstt--
+ppooppuullaarr iimmaaggee,, vviiddeeoo,, aanndd aauuddiioo ddaattaasseettss aavvaaiillaabbllee iinn sseeccoonnddss Deep Lake
+community has uploaded _1_0_0_+_ _i_m_a_g_e_,_ _v_i_d_e_o_ _a_n_d_ _a_u_d_i_o_ _d_a_t_a_s_e_t_s like _M_N_I_S_T, _C_O_C_O,
+_I_m_a_g_e_N_e_t, _C_I_F_A_R, _G_T_Z_A_N and others. IInnssttaanntt VViissuuaalliizzaattiioonn SSuuppppoorrtt iinn tthhee _DD_ee_ee_pp
+_LL_aa_kk_ee_ _AA_pp_pp Deep Lake datasets are instantly visualized with bounding boxes,
+masks, annotations, etc. in _D_e_e_p_ _L_a_k_e_ _V_i_s_u_a_l_i_z_e_r (see below). [![Visualizer]
+(https://www.linkpicture.com/q/ReadMe.gif "Visualizer")](https://
+www.youtube.com/watch?v=SxsofpSIw3k) ## ð Performance Deep Lake's performant
+dataloader built in C++ speeds up data streaming by >2x compared to Hub 2.x
+(Ofeidis et al. 2022, Hambardzumyan et al. 2023)
                    _[_d_o_c_s_/_s_o_u_r_c_e_/___s_t_a_t_i_c_/_i_m_g_/_b_e_n_c_h_m_a_r_k_s_._p_n_g_]
 ## ð How to install Deep Lake Deep Lake can be installed using pip: ```sh
 pip3 install deeplake ``` **By default, Deep Lake does not install dependencies
 for audio, video, google-cloud, and other features. Details on all installation
 options are [available here](https://docs.deeplake.ai/en/latest/
 Installation.html).** ### To access all of Deep Lake's features, please
 register in the [Deep Lake App](https://app.activeloop.ai/register/). ## ð§
```

### Comparing `deeplake-3.9.0/deeplake.egg-info/SOURCES.txt` & `deeplake-3.9.1/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.0/deeplake.egg-info/requires.txt` & `deeplake-3.9.1/deeplake.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 click
 pathos
 humbug>=0.3.1
 tqdm
 lz4
 pyjwt
 pydantic
-libdeeplake==0.0.118
+libdeeplake==0.0.119
 
 [:python_version >= "3.7" and sys_platform != "win32"]
 aioboto3>=10.4.0
 nest_asyncio
 
 [all]
-pydicom
-azure-cli
-google-auth-oauthlib~=0.4.5
-azure-storage-blob
-google-api-python-client~=2.31.0
+google-auth~=2.0.1
 laspy
-IPython
-azure-identity
+google-api-python-client~=2.31.0
+azure-storage-blob
+oauth2client~=4.1.3
 nibabel
-google-auth~=2.0.1
+IPython
+azure-cli
 google-cloud-storage~=1.42.0
-oauth2client~=4.1.3
+google-auth-oauthlib~=0.4.5
+pydicom
 flask
-libdeeplake==0.0.118
+azure-identity
+libdeeplake==0.0.119
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
 [audio]
 
 [audio:python_version >= "3.7" or sys_platform != "win32"]
@@ -49,15 +49,15 @@
 azure-storage-blob
 
 [dicom]
 pydicom
 nibabel
 
 [enterprise]
-libdeeplake==0.0.118
+libdeeplake==0.0.119
 pyjwt
 
 [gcp]
 google-cloud-storage~=1.42.0
 google-auth~=2.0.1
 google-auth-oauthlib~=0.4.5
```

### Comparing `deeplake-3.9.0/setup.py` & `deeplake-3.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 all_extras = {r for v in extras.values() for r in v}
 install_requires = [req_map[r] for r in req_map if r not in all_extras]
 extras_require = {k: [req_map[r] for r in v] for k, v in extras.items()}
 
 extras_require["all"] = [req_map[r] for r in all_extras]
 
 if libdeeplake_available():
-    libdeeplake = "libdeeplake==0.0.118"
+    libdeeplake = "libdeeplake==0.0.119"
     extras_require["enterprise"] = [libdeeplake, "pyjwt"]
     extras_require["all"].append(libdeeplake)
     install_requires.append(libdeeplake)
 
 init_file = os.path.join(project_name, "__init__.py")
```

