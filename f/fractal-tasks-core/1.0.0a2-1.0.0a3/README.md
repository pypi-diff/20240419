# Comparing `tmp/fractal_tasks_core-1.0.0a2.tar.gz` & `tmp/fractal_tasks_core-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_tasks_core-1.0.0a2.tar", max compression
+gzip compressed data, was "fractal_tasks_core-1.0.0a3.tar", max compression
```

## Comparing `fractal_tasks_core-1.0.0a2.tar` & `fractal_tasks_core-1.0.0a3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0     1584 2024-04-17 14:03:40.647913 fractal_tasks_core-1.0.0a2/LICENSE
--rw-r--r--   0        0        0     3743 2024-04-17 14:03:40.647913 fractal_tasks_core-1.0.0a2/README.md
--rw-r--r--   0        0        0       32 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/.gitignore
--rw-r--r--   0        0        0    64035 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/__FRACTAL_MANIFEST__.json
--rw-r--r--   0        0        0      200 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/__init__.py
--rw-r--r--   0        0        0       87 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/cellvoyager/__init__.py
--rw-r--r--   0        0        0     4552 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/cellvoyager/filenames.py
--rw-r--r--   0        0        0    12515 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/cellvoyager/metadata.py
--rw-r--r--   0        0        0    16707 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/channels.py
--rw-r--r--   0        0        0      108 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/README.md
--rw-r--r--   0        0        0       98 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/__init__.py
--rw-r--r--   0        0        0     4607 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/check_manifest.py
--rw-r--r--   0        0        0     5368 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/create_manifest.py
--rw-r--r--   0        0        0     8166 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_args_schemas.py
--rw-r--r--   0        0        0     6406 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_descriptions.py
--rw-r--r--   0        0        0     3260 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_signature_constraints.py
--rw-r--r--   0        0        0     2827 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_task_docs.py
--rw-r--r--   0        0        0     2273 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_titles.py
--rw-r--r--   0        0        0     3624 2024-04-17 14:03:40.651913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/task_list.py
--rw-r--r--   0        0        0     2660 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/task_models.py
--rw-r--r--   0        0        0     5189 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/labels.py
--rw-r--r--   0        0        0     9005 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/masked_loading.py
--rw-r--r--   0        0        0      508 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/ngff/__init__.py
--rw-r--r--   0        0        0    13113 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/ngff/specs.py
--rw-r--r--   0        0        0     3974 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/ngff/zarr_utils.py
--rw-r--r--   0        0        0     3788 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/pyramids.py
--rw-r--r--   0        0        0      185 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/__init__.py
--rw-r--r--   0        0        0     4501 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/_overlaps_common.py
--rw-r--r--   0        0        0     1327 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/load_region.py
--rw-r--r--   0        0        0    18609 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1.py
--rw-r--r--   0        0        0     4910 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1_checks.py
--rw-r--r--   0        0        0    13273 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1_overlaps.py
--rw-r--r--   0        0        0     3394 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tables/__init__.py
--rw-r--r--   0        0        0    11579 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tables/v1.py
--rw-r--r--   0        0        0       72 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/__init__.py
--rw-r--r--   0        0        0     8392 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/_registration_utils.py
--rw-r--r--   0        0        0     2407 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/_utils.py
--rw-r--r--   0        0        0    13827 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/apply_registration_to_image.py
--rw-r--r--   0        0        0     9363 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/calculate_registration_image_based.py
--rw-r--r--   0        0        0    27516 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellpose_segmentation.py
--rw-r--r--   0        0        0     8458 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellpose_transforms.py
--rw-r--r--   0        0        0     7779 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py
--rw-r--r--   0        0        0    18431 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py
--rw-r--r--   0        0        0    21103 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py
--rw-r--r--   0        0        0    11258 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py
--rw-r--r--   0        0        0     6403 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/find_registration_consensus.py
--rw-r--r--   0        0        0    10319 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/illumination_correction.py
--rw-r--r--   0        0        0     3596 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/image_based_registration_hcs_init.py
--rw-r--r--   0        0        0    11764 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/import_ome_zarr.py
--rw-r--r--   0        0        0     2998 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py
--rw-r--r--   0        0        0     4903 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/io_models.py
--rw-r--r--   0        0        0     6239 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/maximum_intensity_projection.py
--rw-r--r--   0        0        0    24816 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/napari_workflows_wrapper.py
--rw-r--r--   0        0        0     7136 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/upscale_array.py
--rw-r--r--   0        0        0     6101 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/utils.py
--rw-r--r--   0        0        0     3890 2024-04-17 14:03:40.655913 fractal_tasks_core-1.0.0a2/fractal_tasks_core/zarr_utils.py
--rw-r--r--   0        0        0     3387 2024-04-17 14:03:40.659913 fractal_tasks_core-1.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 fractal_tasks_core-1.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1584 2024-04-19 12:17:10.268485 fractal_tasks_core-1.0.0a3/LICENSE
+-rw-r--r--   0        0        0     3743 2024-04-19 12:17:10.268485 fractal_tasks_core-1.0.0a3/README.md
+-rw-r--r--   0        0        0       32 2024-04-19 12:17:10.272485 fractal_tasks_core-1.0.0a3/fractal_tasks_core/.gitignore
+-rw-r--r--   0        0        0    64035 2024-04-19 12:17:10.272485 fractal_tasks_core-1.0.0a3/fractal_tasks_core/__FRACTAL_MANIFEST__.json
+-rw-r--r--   0        0        0      200 2024-04-19 12:17:10.272485 fractal_tasks_core-1.0.0a3/fractal_tasks_core/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-19 12:17:10.272485 fractal_tasks_core-1.0.0a3/fractal_tasks_core/cellvoyager/__init__.py
+-rw-r--r--   0        0        0     4552 2024-04-19 12:17:10.272485 fractal_tasks_core-1.0.0a3/fractal_tasks_core/cellvoyager/filenames.py
+-rw-r--r--   0        0        0    12515 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/cellvoyager/metadata.py
+-rw-r--r--   0        0        0    16707 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/channels.py
+-rw-r--r--   0        0        0      108 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/README.md
+-rw-r--r--   0        0        0       98 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/__init__.py
+-rw-r--r--   0        0        0     4607 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/check_manifest.py
+-rw-r--r--   0        0        0     5368 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/create_manifest.py
+-rw-r--r--   0        0        0     8166 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_args_schemas.py
+-rw-r--r--   0        0        0     6406 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_descriptions.py
+-rw-r--r--   0        0        0     3260 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_signature_constraints.py
+-rw-r--r--   0        0        0     2827 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_task_docs.py
+-rw-r--r--   0        0        0     2273 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_titles.py
+-rw-r--r--   0        0        0     3624 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/task_list.py
+-rw-r--r--   0        0        0     2660 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/task_models.py
+-rw-r--r--   0        0        0     5189 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/labels.py
+-rw-r--r--   0        0        0     9005 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/masked_loading.py
+-rw-r--r--   0        0        0      508 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/ngff/__init__.py
+-rw-r--r--   0        0        0    13113 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/ngff/specs.py
+-rw-r--r--   0        0        0     3974 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/ngff/zarr_utils.py
+-rw-r--r--   0        0        0     3788 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/pyramids.py
+-rw-r--r--   0        0        0      185 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/__init__.py
+-rw-r--r--   0        0        0     4501 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/_overlaps_common.py
+-rw-r--r--   0        0        0     1327 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/load_region.py
+-rw-r--r--   0        0        0    18609 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1.py
+-rw-r--r--   0        0        0     4910 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1_checks.py
+-rw-r--r--   0        0        0    13273 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1_overlaps.py
+-rw-r--r--   0        0        0     3394 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tables/__init__.py
+-rw-r--r--   0        0        0    11579 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tables/v1.py
+-rw-r--r--   0        0        0       72 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/__init__.py
+-rw-r--r--   0        0        0     8166 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/_registration_utils.py
+-rw-r--r--   0        0        0     2407 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/_utils.py
+-rw-r--r--   0        0        0     3839 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/_zarr_utils.py
+-rw-r--r--   0        0        0    13819 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/apply_registration_to_image.py
+-rw-r--r--   0        0        0     9363 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/calculate_registration_image_based.py
+-rw-r--r--   0        0        0    27516 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellpose_segmentation.py
+-rw-r--r--   0        0        0     8458 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellpose_transforms.py
+-rw-r--r--   0        0        0     7779 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py
+-rw-r--r--   0        0        0    18431 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py
+-rw-r--r--   0        0        0    21103 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py
+-rw-r--r--   0        0        0    11258 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py
+-rw-r--r--   0        0        0     6403 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/find_registration_consensus.py
+-rw-r--r--   0        0        0    10480 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/illumination_correction.py
+-rw-r--r--   0        0        0     3596 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/image_based_registration_hcs_init.py
+-rw-r--r--   0        0        0    11764 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/import_ome_zarr.py
+-rw-r--r--   0        0        0     2998 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py
+-rw-r--r--   0        0        0     4903 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/io_models.py
+-rw-r--r--   0        0        0     6239 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/maximum_intensity_projection.py
+-rw-r--r--   0        0        0    24816 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/napari_workflows_wrapper.py
+-rw-r--r--   0        0        0     7136 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/upscale_array.py
+-rw-r--r--   0        0        0     6101 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/utils.py
+-rw-r--r--   0        0        0     3890 2024-04-19 12:17:10.276486 fractal_tasks_core-1.0.0a3/fractal_tasks_core/zarr_utils.py
+-rw-r--r--   0        0        0     3387 2024-04-19 12:17:10.280485 fractal_tasks_core-1.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 fractal_tasks_core-1.0.0a3/PKG-INFO
```

### Comparing `fractal_tasks_core-1.0.0a2/LICENSE` & `fractal_tasks_core-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/README.md` & `fractal_tasks_core-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/__FRACTAL_MANIFEST__.json` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/__FRACTAL_MANIFEST__.json`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/cellvoyager/filenames.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/cellvoyager/filenames.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/cellvoyager/metadata.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/cellvoyager/metadata.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/channels.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/channels.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/check_manifest.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/check_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/create_manifest.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/create_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_args_schemas.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_args_schemas.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_descriptions.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_descriptions.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_signature_constraints.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_signature_constraints.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_task_docs.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_task_docs.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/lib_titles.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/lib_titles.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/task_list.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/task_list.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/dev/task_models.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/dev/task_models.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/labels.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/labels.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/masked_loading.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/masked_loading.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/ngff/specs.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/ngff/specs.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/ngff/zarr_utils.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/ngff/zarr_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/pyramids.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/pyramids.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/_overlaps_common.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/_overlaps_common.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/load_region.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/load_region.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1_checks.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1_checks.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/roi/v1_overlaps.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/roi/v1_overlaps.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tables/__init__.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tables/v1.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tables/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/_registration_utils.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/_registration_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,15 @@
 import copy
 
 import anndata as ad
 import numpy as np
 import pandas as pd
 
 from fractal_tasks_core.ngff.zarr_utils import load_NgffWellMeta
-
-
-def _split_well_path_image_path(zarr_url: str) -> tuple[str, str]:
-    """
-    Returns path to well folder for HCS OME-Zarr `zarr_url`.
-    """
-    zarr_url = zarr_url.rstrip("/")
-    well_path = "/".join(zarr_url.split("/")[:-1])
-    img_path = zarr_url.split("/")[-1]
-    return well_path, img_path
+from fractal_tasks_core.tasks._zarr_utils import _split_well_path_image_path
 
 
 def create_well_acquisition_dict(
     zarr_urls: list[str],
 ) -> dict[str, dict[int, str]]:
     """
     Parses zarr_urls & groups them by HCS wells & acquisition
```

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/_utils.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/apply_registration_to_image.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/apply_registration_to_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 )
 from fractal_tasks_core.roi import (
     convert_ROI_table_to_indices,
 )
 from fractal_tasks_core.roi import is_standard_roi_table
 from fractal_tasks_core.roi import load_region
 from fractal_tasks_core.tables import write_table
-from fractal_tasks_core.tasks._registration_utils import (
+from fractal_tasks_core.tasks._zarr_utils import (
     _split_well_path_image_path,
 )
 from fractal_tasks_core.utils import _get_table_path_dict
 
 logger = logging.getLogger(__name__)
```

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/calculate_registration_image_based.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/calculate_registration_image_based.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellpose_segmentation.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellpose_segmentation.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellpose_transforms.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellpose_transforms.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/find_registration_consensus.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/find_registration_consensus.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/illumination_correction.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/illumination_correction.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from fractal_tasks_core.channels import OmeroChannel
 from fractal_tasks_core.ngff import load_NgffImageMeta
 from fractal_tasks_core.pyramids import build_pyramid
 from fractal_tasks_core.roi import check_valid_ROI_indices
 from fractal_tasks_core.roi import (
     convert_ROI_table_to_indices,
 )
+from fractal_tasks_core.tasks._zarr_utils import _copy_hcs_ome_zarr_metadata
 
 logger = logging.getLogger(__name__)
 
 
 def correct(
     img_stack: np.ndarray,
     corr_img: np.ndarray,
@@ -138,17 +139,17 @@
             illumination corrected data is saved there.
         suffix: What suffix to append to the illumination corrected images.
             Only relevant if `overwrite_input=False`.
     """
 
     # Defione old/new zarrurls
     if overwrite_input:
-        zarr_url_new = zarr_url
+        zarr_url_new = zarr_url.rstrip("/")
     else:
-        zarr_url_new = zarr_url + suffix
+        zarr_url_new = zarr_url.rstrip("/") + suffix
 
     t_start = time.perf_counter()
     logger.info("Start illumination_correction")
     logger.info(f"  {overwrite_input=}")
     logger.info(f"  {zarr_url=}")
     logger.info(f"  {zarr_url_new=}")
 
@@ -222,14 +223,15 @@
             shape=data_czyx.shape,
             chunks=data_czyx.chunksize,
             dtype=data_czyx.dtype,
             store=zarr.storage.FSStore(f"{zarr_url_new}/0"),
             overwrite=False,
             dimension_separator="/",
         )
+        _copy_hcs_ome_zarr_metadata(zarr_url, zarr_url_new)
 
     # Iterate over FOV ROIs
     num_ROIs = len(list_indices)
     for i_c, channel in enumerate(channels):
         for i_ROI, indices in enumerate(list_indices):
             # Define region
             s_z, e_z, s_y, e_y, s_x, e_x = indices[:]
```

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/image_based_registration_hcs_init.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/image_based_registration_hcs_init.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/import_ome_zarr.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/import_ome_zarr.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/io_models.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/io_models.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/maximum_intensity_projection.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/maximum_intensity_projection.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/tasks/napari_workflows_wrapper.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/tasks/napari_workflows_wrapper.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/upscale_array.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/upscale_array.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/utils.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/fractal_tasks_core/zarr_utils.py` & `fractal_tasks_core-1.0.0a3/fractal_tasks_core/zarr_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.0a2/pyproject.toml` & `fractal_tasks_core-1.0.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-tasks-core"
-version = "1.0.0a2"
+version = "1.0.0a3"
 description = "Core bioimage-analysis library and tasks of the Fractal analytics platform"
 authors = [
     "Joel Lüthi  <joel.luethi@fmi.ch>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
@@ -85,15 +85,15 @@
 branch = true
 parallel = true
 relative_files = true
 source = ["fractal_tasks_core"]
 omit = ["tests/*", "examples/*", "fractal_tasks_core/dev/*"]
 
 [tool.bumpver]
-current_version = "1.0.0a2"
+current_version = "1.0.0a3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_tasks_core-1.0.0a2/PKG-INFO` & `fractal_tasks_core-1.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-tasks-core
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Core bioimage-analysis library and tasks of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-tasks-core
 License: BSD-3-Clause
 Author: Joel Lüthi 
 Author-email: joel.luethi@fmi.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

