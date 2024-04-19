# Comparing `tmp/mirp-2.2.0.tar.gz` & `tmp/mirp-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirp-2.2.0.tar", last modified: Mon Mar 18 15:47:51 2024, max compression
+gzip compressed data, was "mirp-2.2.1.tar", last modified: Fri Apr 19 14:44:44 2024, max compression
```

## Comparing `mirp-2.2.0.tar` & `mirp-2.2.1.tar`

### file list

```diff
@@ -1,129 +1,125 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.701554 mirp-2.2.0/
--rw-rw-rw-   0        0        0     1205 2024-03-18 08:21:34.000000 mirp-2.2.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    14139 2020-10-01 17:38:34.000000 mirp-2.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       33 2023-10-27 15:27:23.000000 mirp-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11726 2024-03-18 15:33:26.000000 mirp-2.2.0/NEWS.md
--rw-rw-rw-   0        0        0    26031 2024-03-18 15:47:51.700520 mirp-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     8108 2024-03-18 08:21:34.000000 mirp-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.610354 mirp-2.2.0/mirp/
--rw-rw-rw-   0        0        0      927 2024-03-18 09:45:13.000000 mirp-2.2.0/mirp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.633110 mirp-2.2.0/mirp/_data_import/
--rw-rw-rw-   0        0        0        0 2023-10-27 15:27:08.000000 mirp-2.2.0/mirp/_data_import/__init__.py
--rw-rw-rw-   0        0        0    19497 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_data_import/dicom_file.py
--rw-rw-rw-   0        0        0     4595 2024-03-18 08:55:01.000000 mirp-2.2.0/mirp/_data_import/dicom_file_ct.py
--rw-rw-rw-   0        0        0     6577 2024-03-18 08:55:01.000000 mirp-2.2.0/mirp/_data_import/dicom_file_mr.py
--rw-rw-rw-   0        0        0    15758 2024-03-18 08:55:01.000000 mirp-2.2.0/mirp/_data_import/dicom_file_pet.py
--rw-rw-rw-   0        0        0     7070 2024-03-18 08:55:01.000000 mirp-2.2.0/mirp/_data_import/dicom_file_rtdose.py
--rw-rw-rw-   0        0        0    31369 2024-03-18 14:58:51.000000 mirp-2.2.0/mirp/_data_import/dicom_file_rtstruct.py
--rw-rw-rw-   0        0        0    21406 2024-03-18 09:37:21.000000 mirp-2.2.0/mirp/_data_import/dicom_file_seg.py
--rw-rw-rw-   0        0        0    10859 2024-03-18 13:08:45.000000 mirp-2.2.0/mirp/_data_import/dicom_file_stack.py
--rw-rw-rw-   0        0        0    22603 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_data_import/directory.py
--rw-rw-rw-   0        0        0    44469 2024-03-18 14:07:33.000000 mirp-2.2.0/mirp/_data_import/generic_file.py
--rw-rw-rw-   0        0        0    11043 2024-03-18 08:55:01.000000 mirp-2.2.0/mirp/_data_import/generic_file_stack.py
--rw-rw-rw-   0        0        0     6358 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_data_import/itk_file.py
--rw-rw-rw-   0        0        0     7141 2024-03-18 13:08:45.000000 mirp-2.2.0/mirp/_data_import/itk_file_stack.py
--rw-rw-rw-   0        0        0    13434 2024-03-18 08:55:01.000000 mirp-2.2.0/mirp/_data_import/mask_contour.py
--rw-rw-rw-   0        0        0     5699 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_data_import/numpy_file.py
--rw-rw-rw-   0        0        0     2944 2024-03-18 08:55:01.000000 mirp-2.2.0/mirp/_data_import/numpy_file_stack.py
--rw-rw-rw-   0        0        0     1228 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_data_import/read_data.py
--rw-rw-rw-   0        0        0    22414 2024-03-18 08:47:12.000000 mirp-2.2.0/mirp/_data_import/suv.py
--rw-rw-rw-   0        0        0    17570 2024-03-13 11:34:19.000000 mirp-2.2.0/mirp/_data_import/utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.644269 mirp-2.2.0/mirp/_featuresets/
--rw-rw-rw-   0        0        0        0 2020-10-01 17:38:34.000000 mirp-2.2.0/mirp/_featuresets/__init__.py
--rw-rw-rw-   0        0        0    21581 2024-03-18 10:28:31.000000 mirp-2.2.0/mirp/_featuresets/cm.py
--rw-rw-rw-   0        0        0    13820 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_featuresets/dzm.py
--rw-rw-rw-   0        0        0     6917 2024-03-18 14:19:01.000000 mirp-2.2.0/mirp/_featuresets/intensity_histogram.py
--rw-rw-rw-   0        0        0    10922 2024-03-18 14:19:01.000000 mirp-2.2.0/mirp/_featuresets/intensity_volume_histogram.py
--rw-rw-rw-   0        0        0     6275 2024-03-18 11:36:27.000000 mirp-2.2.0/mirp/_featuresets/local_intensity.py
--rw-rw-rw-   0        0        0    32584 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_featuresets/morphology_3d.py
--rw-rw-rw-   0        0        0    13752 2024-03-18 10:30:26.000000 mirp-2.2.0/mirp/_featuresets/ngldm.py
--rw-rw-rw-   0        0        0    12853 2024-03-18 14:19:01.000000 mirp-2.2.0/mirp/_featuresets/ngtdm.py
--rw-rw-rw-   0        0        0    18910 2024-03-18 10:29:26.000000 mirp-2.2.0/mirp/_featuresets/rlm.py
--rw-rw-rw-   0        0        0     4278 2024-03-18 09:37:21.000000 mirp-2.2.0/mirp/_featuresets/statistics.py
--rw-rw-rw-   0        0        0    13184 2024-03-18 10:30:26.000000 mirp-2.2.0/mirp/_featuresets/szm.py
--rw-rw-rw-   0        0        0     3185 2020-10-01 17:38:34.000000 mirp-2.2.0/mirp/_featuresets/utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.655429 mirp-2.2.0/mirp/_image_processing/
--rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.0/mirp/_image_processing/__init__.py
--rw-rw-rw-   0        0        0      987 2024-03-18 09:30:20.000000 mirp-2.2.0/mirp/_image_processing/add_noise.py
--rw-rw-rw-   0        0        0     2808 2024-03-18 09:37:21.000000 mirp-2.2.0/mirp/_image_processing/alter_mask.py
--rw-rw-rw-   0        0        0     1223 2023-10-27 15:27:23.000000 mirp-2.2.0/mirp/_image_processing/anti_aliasing.py
--rw-rw-rw-   0        0        0     4256 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_image_processing/cropping.py
--rw-rw-rw-   0        0        0     5128 2024-03-18 09:37:21.000000 mirp-2.2.0/mirp/_image_processing/discretise_image.py
--rw-rw-rw-   0        0        0      824 2024-03-18 09:30:20.000000 mirp-2.2.0/mirp/_image_processing/normalise_image.py
--rw-rw-rw-   0        0        0     2004 2024-03-18 13:08:45.000000 mirp-2.2.0/mirp/_image_processing/randomise_mask.py
--rw-rw-rw-   0        0        0      994 2024-03-18 09:37:21.000000 mirp-2.2.0/mirp/_image_processing/resegmentise_mask.py
--rw-rw-rw-   0        0        0      436 2024-03-18 09:30:20.000000 mirp-2.2.0/mirp/_image_processing/saturate_image.py
--rw-rw-rw-   0        0        0     1597 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_image_processing/split_mask.py
--rw-rw-rw-   0        0        0     2696 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_image_processing/tissue_mask.py
--rw-rw-rw-   0        0        0     2656 2024-03-18 09:37:21.000000 mirp-2.2.0/mirp/_image_processing/utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.667585 mirp-2.2.0/mirp/_imagefilters/
--rw-rw-rw-   0        0        0        0 2020-10-01 17:38:34.000000 mirp-2.2.0/mirp/_imagefilters/__init__.py
--rw-rw-rw-   0        0        0     1454 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/exponential_transform.py
--rw-rw-rw-   0        0        0     9339 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/gabor.py
--rw-rw-rw-   0        0        0     6439 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/gaussian.py
--rw-rw-rw-   0        0        0      562 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/generic.py
--rw-rw-rw-   0        0        0     7495 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/laplacian_of_gaussian.py
--rw-rw-rw-   0        0        0     7321 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_imagefilters/laws.py
--rw-rw-rw-   0        0        0     1496 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/log_transform.py
--rw-rw-rw-   0        0        0     2546 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/mean.py
--rw-rw-rw-   0        0        0     9798 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/nonseparable_wavelet.py
--rw-rw-rw-   0        0        0     7484 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/separable_wavelet.py
--rw-rw-rw-   0        0        0     1261 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/square_root_transform.py
--rw-rw-rw-   0        0        0     1230 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/_imagefilters/square_transform.py
--rw-rw-rw-   0        0        0    23965 2024-03-13 11:34:19.000000 mirp-2.2.0/mirp/_imagefilters/utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.676191 mirp-2.2.0/mirp/_images/
--rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.0/mirp/_images/__init__.py
--rw-rw-rw-   0        0        0     9141 2024-03-13 11:34:19.000000 mirp-2.2.0/mirp/_images/base_image.py
--rw-rw-rw-   0        0        0     2115 2024-03-18 09:30:20.000000 mirp-2.2.0/mirp/_images/ct_image.py
--rw-rw-rw-   0        0        0    51693 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_images/generic_image.py
--rw-rw-rw-   0        0        0    22180 2024-03-18 14:19:01.000000 mirp-2.2.0/mirp/_images/mask_image.py
--rw-rw-rw-   0        0        0     1911 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_images/mr_image.py
--rw-rw-rw-   0        0        0     2204 2024-03-18 09:30:20.000000 mirp-2.2.0/mirp/_images/pet_image.py
--rw-rw-rw-   0        0        0     1908 2024-03-18 09:30:20.000000 mirp-2.2.0/mirp/_images/rtdose_image.py
--rw-rw-rw-   0        0        0    26540 2024-03-18 09:30:20.000000 mirp-2.2.0/mirp/_images/transformed_image.py
--rw-rw-rw-   0        0        0     3473 2024-03-18 09:37:21.000000 mirp-2.2.0/mirp/_images/utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.678208 mirp-2.2.0/mirp/_masks/
--rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.0/mirp/_masks/__init__.py
--rw-rw-rw-   0        0        0    28803 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_masks/base_mask.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.680225 mirp-2.2.0/mirp/_workflows/
--rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.0/mirp/_workflows/__init__.py
--rw-rw-rw-   0        0        0      328 2024-03-18 08:55:01.000000 mirp-2.2.0/mirp/_workflows/baseWorkflow.py
--rw-rw-rw-   0        0        0    34886 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/_workflows/standardWorkflow.py
--rw-rw-rw-   0        0        0     3379 2023-10-27 15:27:23.000000 mirp-2.2.0/mirp/config_data.xml
--rw-rw-rw-   0        0        0    20912 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/config_settings.xml
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.683257 mirp-2.2.0/mirp/data_import/
--rw-rw-rw-   0        0        0        0 2024-03-18 14:58:21.000000 mirp-2.2.0/mirp/data_import/__init__.py
--rw-rw-rw-   0        0        0     8904 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/data_import/import_image.py
--rw-rw-rw-   0        0        0    15364 2024-03-18 14:58:51.000000 mirp-2.2.0/mirp/data_import/import_image_and_mask.py
--rw-rw-rw-   0        0        0     5049 2024-03-18 14:58:51.000000 mirp-2.2.0/mirp/data_import/import_mask.py
--rw-rw-rw-   0        0        0    17431 2024-03-18 14:58:51.000000 mirp-2.2.0/mirp/deep_learning_preprocessing.py
--rw-rw-rw-   0        0        0     1556 2023-10-27 15:27:23.000000 mirp-2.2.0/mirp/deprecated.py
--rw-rw-rw-   0        0        0    21532 2024-03-18 14:58:51.000000 mirp-2.2.0/mirp/extract_features_and_images.py
--rw-rw-rw-   0        0        0     4699 2024-03-18 14:58:51.000000 mirp-2.2.0/mirp/extract_image_parameters.py
--rw-rw-rw-   0        0        0     4635 2024-03-18 14:58:51.000000 mirp-2.2.0/mirp/extract_mask_labels.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.694471 mirp-2.2.0/mirp/settings/
--rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.0/mirp/settings/__init__.py
--rw-rw-rw-   0        0        0    34637 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/settings/feature_parameters.py
--rw-rw-rw-   0        0        0     3811 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/settings/general_parameters.py
--rw-rw-rw-   0        0        0     7936 2024-03-18 13:00:10.000000 mirp-2.2.0/mirp/settings/generic.py
--rw-rw-rw-   0        0        0    20044 2024-03-18 12:58:08.000000 mirp-2.2.0/mirp/settings/image_processing_parameters.py
--rw-rw-rw-   0        0        0     6596 2024-03-18 09:43:15.000000 mirp-2.2.0/mirp/settings/import_config_parameters.py
--rw-rw-rw-   0        0        0     5665 2024-03-13 11:34:19.000000 mirp-2.2.0/mirp/settings/import_data_parameters.py
--rw-rw-rw-   0        0        0     9775 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/settings/interpolation_parameters.py
--rw-rw-rw-   0        0        0    13717 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/settings/perturbation_parameters.py
--rw-rw-rw-   0        0        0     4149 2024-01-30 15:26:37.000000 mirp-2.2.0/mirp/settings/resegmentation_parameters.py
--rw-rw-rw-   0        0        0    65740 2024-03-18 13:11:27.000000 mirp-2.2.0/mirp/settings/transformation_parameters.py
--rw-rw-rw-   0        0        0     6872 2024-03-18 08:47:12.000000 mirp-2.2.0/mirp/settings/utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.698505 mirp-2.2.0/mirp/utilities/
--rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.0/mirp/utilities/__init__.py
--rw-rw-rw-   0        0        0     2495 2024-03-18 13:06:36.000000 mirp-2.2.0/mirp/utilities/config_utilities.py
--rw-rw-rw-   0        0        0     1248 2024-01-25 14:55:38.000000 mirp-2.2.0/mirp/utilities/parallel.py
--rw-rw-rw-   0        0        0      862 2024-01-25 14:55:38.000000 mirp-2.2.0/mirp/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:47:51.699521 mirp-2.2.0/mirp.egg-info/
--rw-rw-rw-   0        0        0    26031 2024-03-18 15:47:51.000000 mirp-2.2.0/mirp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3636 2024-03-18 15:47:51.000000 mirp-2.2.0/mirp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 15:47:51.000000 mirp-2.2.0/mirp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      252 2024-03-18 15:47:51.000000 mirp-2.2.0/mirp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-18 15:47:51.000000 mirp-2.2.0/mirp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1680 2024-03-18 15:47:34.000000 mirp-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-18 15:47:51.701554 mirp-2.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.538627 mirp-2.2.1/
+-rw-rw-rw-   0        0        0     1375 2024-04-04 14:37:05.000000 mirp-2.2.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    14139 2020-10-01 17:38:34.000000 mirp-2.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       33 2023-10-27 15:27:23.000000 mirp-2.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    12992 2024-04-19 14:41:38.000000 mirp-2.2.1/NEWS.md
+-rw-rw-rw-   0        0        0    26846 2024-04-19 14:44:44.537627 mirp-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8958 2024-04-09 11:53:59.000000 mirp-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.443542 mirp-2.2.1/mirp/
+-rw-rw-rw-   0        0        0      927 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.467563 mirp-2.2.1/mirp/_data_import/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/__init__.py
+-rw-rw-rw-   0        0        0    24825 2024-04-19 07:42:34.000000 mirp-2.2.1/mirp/_data_import/dicom_file.py
+-rw-rw-rw-   0        0        0     4595 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/dicom_file_ct.py
+-rw-rw-rw-   0        0        0     6577 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/dicom_file_mr.py
+-rw-rw-rw-   0        0        0    36854 2024-04-17 11:02:29.000000 mirp-2.2.1/mirp/_data_import/dicom_file_pet.py
+-rw-rw-rw-   0        0        0     7289 2024-04-18 15:42:31.000000 mirp-2.2.1/mirp/_data_import/dicom_file_rtdose.py
+-rw-rw-rw-   0        0        0    31324 2024-04-18 15:43:46.000000 mirp-2.2.1/mirp/_data_import/dicom_file_rtstruct.py
+-rw-rw-rw-   0        0        0    21406 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/dicom_file_seg.py
+-rw-rw-rw-   0        0        0    10873 2024-04-17 15:11:01.000000 mirp-2.2.1/mirp/_data_import/dicom_file_stack.py
+-rw-rw-rw-   0        0        0    22746 2024-04-18 15:11:10.000000 mirp-2.2.1/mirp/_data_import/directory.py
+-rw-rw-rw-   0        0        0    45837 2024-04-17 14:40:58.000000 mirp-2.2.1/mirp/_data_import/generic_file.py
+-rw-rw-rw-   0        0        0    11185 2024-04-17 14:40:58.000000 mirp-2.2.1/mirp/_data_import/generic_file_stack.py
+-rw-rw-rw-   0        0        0     6508 2024-04-18 14:55:20.000000 mirp-2.2.1/mirp/_data_import/itk_file.py
+-rw-rw-rw-   0        0        0     7141 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/itk_file_stack.py
+-rw-rw-rw-   0        0        0    13474 2024-04-10 14:03:09.000000 mirp-2.2.1/mirp/_data_import/mask_contour.py
+-rw-rw-rw-   0        0        0     5845 2024-04-18 14:55:20.000000 mirp-2.2.1/mirp/_data_import/numpy_file.py
+-rw-rw-rw-   0        0        0     2944 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/numpy_file_stack.py
+-rw-rw-rw-   0        0        0     1308 2024-04-19 06:51:53.000000 mirp-2.2.1/mirp/_data_import/read_data.py
+-rw-rw-rw-   0        0        0    22434 2024-04-12 11:31:49.000000 mirp-2.2.1/mirp/_data_import/suv.py
+-rw-rw-rw-   0        0        0    17570 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_data_import/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.479574 mirp-2.2.1/mirp/_featuresets/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/__init__.py
+-rw-rw-rw-   0        0        0    21581 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/cm.py
+-rw-rw-rw-   0        0        0    11525 2024-04-05 11:27:52.000000 mirp-2.2.1/mirp/_featuresets/dzm.py
+-rw-rw-rw-   0        0        0     6917 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/intensity_histogram.py
+-rw-rw-rw-   0        0        0    10922 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/intensity_volume_histogram.py
+-rw-rw-rw-   0        0        0     6275 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/local_intensity.py
+-rw-rw-rw-   0        0        0    32584 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/morphology_3d.py
+-rw-rw-rw-   0        0        0    13752 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/ngldm.py
+-rw-rw-rw-   0        0        0    12853 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/ngtdm.py
+-rw-rw-rw-   0        0        0    18910 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/rlm.py
+-rw-rw-rw-   0        0        0     4278 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/statistics.py
+-rw-rw-rw-   0        0        0    10900 2024-04-05 11:27:52.000000 mirp-2.2.1/mirp/_featuresets/szm.py
+-rw-rw-rw-   0        0        0     3185 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_featuresets/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.488582 mirp-2.2.1/mirp/_image_processing/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/__init__.py
+-rw-rw-rw-   0        0        0     2808 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/alter_mask.py
+-rw-rw-rw-   0        0        0     1223 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/anti_aliasing.py
+-rw-rw-rw-   0        0        0     4256 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/cropping.py
+-rw-rw-rw-   0        0        0     5128 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/discretise_image.py
+-rw-rw-rw-   0        0        0     2004 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/randomise_mask.py
+-rw-rw-rw-   0        0        0     1597 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/split_mask.py
+-rw-rw-rw-   0        0        0     2696 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/tissue_mask.py
+-rw-rw-rw-   0        0        0     2656 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_image_processing/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.501595 mirp-2.2.1/mirp/_imagefilters/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/__init__.py
+-rw-rw-rw-   0        0        0     1454 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/exponential_transform.py
+-rw-rw-rw-   0        0        0     9339 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/gabor.py
+-rw-rw-rw-   0        0        0     6436 2024-04-04 13:44:39.000000 mirp-2.2.1/mirp/_imagefilters/gaussian.py
+-rw-rw-rw-   0        0        0      562 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/generic.py
+-rw-rw-rw-   0        0        0     7495 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/laplacian_of_gaussian.py
+-rw-rw-rw-   0        0        0     7321 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/laws.py
+-rw-rw-rw-   0        0        0     1496 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/log_transform.py
+-rw-rw-rw-   0        0        0     2546 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/mean.py
+-rw-rw-rw-   0        0        0     9798 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/nonseparable_wavelet.py
+-rw-rw-rw-   0        0        0     7484 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/separable_wavelet.py
+-rw-rw-rw-   0        0        0     1261 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/square_root_transform.py
+-rw-rw-rw-   0        0        0     1230 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/square_transform.py
+-rw-rw-rw-   0        0        0    23965 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_imagefilters/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.511604 mirp-2.2.1/mirp/_images/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_images/__init__.py
+-rw-rw-rw-   0        0        0     9143 2024-04-05 10:37:51.000000 mirp-2.2.1/mirp/_images/base_image.py
+-rw-rw-rw-   0        0        0     2115 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_images/ct_image.py
+-rw-rw-rw-   0        0        0    51861 2024-04-10 15:17:41.000000 mirp-2.2.1/mirp/_images/generic_image.py
+-rw-rw-rw-   0        0        0    22184 2024-04-05 10:39:33.000000 mirp-2.2.1/mirp/_images/mask_image.py
+-rw-rw-rw-   0        0        0     1939 2024-04-09 08:50:40.000000 mirp-2.2.1/mirp/_images/mr_image.py
+-rw-rw-rw-   0        0        0     2204 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_images/pet_image.py
+-rw-rw-rw-   0        0        0     1908 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_images/rtdose_image.py
+-rw-rw-rw-   0        0        0    26540 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_images/transformed_image.py
+-rw-rw-rw-   0        0        0     4098 2024-04-09 05:58:15.000000 mirp-2.2.1/mirp/_images/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.513604 mirp-2.2.1/mirp/_masks/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_masks/__init__.py
+-rw-rw-rw-   0        0        0    28747 2024-04-10 11:46:45.000000 mirp-2.2.1/mirp/_masks/base_mask.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.515606 mirp-2.2.1/mirp/_workflows/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_workflows/__init__.py
+-rw-rw-rw-   0        0        0      328 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/_workflows/baseWorkflow.py
+-rw-rw-rw-   0        0        0    35003 2024-04-16 15:05:09.000000 mirp-2.2.1/mirp/_workflows/standardWorkflow.py
+-rw-rw-rw-   0        0        0     3379 2023-10-27 15:27:23.000000 mirp-2.2.1/mirp/config_data.xml
+-rw-rw-rw-   0        0        0    21251 2024-04-12 06:00:24.000000 mirp-2.2.1/mirp/config_settings.xml
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.519610 mirp-2.2.1/mirp/data_import/
+-rw-rw-rw-   0        0        0        0 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/data_import/__init__.py
+-rw-rw-rw-   0        0        0     8904 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/data_import/import_image.py
+-rw-rw-rw-   0        0        0    16692 2024-04-17 12:57:14.000000 mirp-2.2.1/mirp/data_import/import_image_and_mask.py
+-rw-rw-rw-   0        0        0     5072 2024-04-05 08:18:29.000000 mirp-2.2.1/mirp/data_import/import_mask.py
+-rw-rw-rw-   0        0        0    17516 2024-04-03 12:22:01.000000 mirp-2.2.1/mirp/deep_learning_preprocessing.py
+-rw-rw-rw-   0        0        0     1417 2024-04-03 12:34:47.000000 mirp-2.2.1/mirp/deprecated.py
+-rw-rw-rw-   0        0        0    21617 2024-04-09 05:58:15.000000 mirp-2.2.1/mirp/extract_features_and_images.py
+-rw-rw-rw-   0        0        0     4422 2024-04-05 14:31:39.000000 mirp-2.2.1/mirp/extract_image_parameters.py
+-rw-rw-rw-   0        0        0     4363 2024-04-05 14:31:39.000000 mirp-2.2.1/mirp/extract_mask_labels.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.530621 mirp-2.2.1/mirp/settings/
+-rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.1/mirp/settings/__init__.py
+-rw-rw-rw-   0        0        0    34723 2024-04-03 13:34:07.000000 mirp-2.2.1/mirp/settings/feature_parameters.py
+-rw-rw-rw-   0        0        0     3811 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/general_parameters.py
+-rw-rw-rw-   0        0        0     8382 2024-03-27 09:37:42.000000 mirp-2.2.1/mirp/settings/generic.py
+-rw-rw-rw-   0        0        0    22952 2024-04-16 14:53:14.000000 mirp-2.2.1/mirp/settings/image_processing_parameters.py
+-rw-rw-rw-   0        0        0     6596 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/import_config_parameters.py
+-rw-rw-rw-   0        0        0     5665 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/import_data_parameters.py
+-rw-rw-rw-   0        0        0    10008 2024-04-03 14:06:25.000000 mirp-2.2.1/mirp/settings/interpolation_parameters.py
+-rw-rw-rw-   0        0        0    13717 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/perturbation_parameters.py
+-rw-rw-rw-   0        0        0     4149 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/resegmentation_parameters.py
+-rw-rw-rw-   0        0        0    66066 2024-04-03 13:49:05.000000 mirp-2.2.1/mirp/settings/transformation_parameters.py
+-rw-rw-rw-   0        0        0     6872 2024-03-18 16:02:31.000000 mirp-2.2.1/mirp/settings/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.534623 mirp-2.2.1/mirp/utilities/
+-rw-rw-rw-   0        0        0        0 2023-10-27 15:27:23.000000 mirp-2.2.1/mirp/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2551 2024-04-04 15:10:05.000000 mirp-2.2.1/mirp/utilities/config_utilities.py
+-rw-rw-rw-   0        0        0     2533 2024-03-27 10:48:43.000000 mirp-2.2.1/mirp/utilities/parallel.py
+-rw-rw-rw-   0        0        0      862 2024-01-25 14:55:38.000000 mirp-2.2.1/mirp/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:44:44.535625 mirp-2.2.1/mirp.egg-info/
+-rw-rw-rw-   0        0        0    26846 2024-04-19 14:44:44.000000 mirp-2.2.1/mirp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3473 2024-04-19 14:44:44.000000 mirp-2.2.1/mirp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 14:44:44.000000 mirp-2.2.1/mirp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      291 2024-04-19 14:44:44.000000 mirp-2.2.1/mirp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-19 14:44:44.000000 mirp-2.2.1/mirp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1749 2024-04-09 10:25:45.000000 mirp-2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 14:44:44.538627 mirp-2.2.1/setup.cfg
```

### Comparing `mirp-2.2.0/CONTRIBUTING.md` & `mirp-2.2.1/CONTRIBUTING.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# How to contribute
+# Contributing
 
-If you have ideas or code to contribute, please first open an [issue](https://github.com/oncoray/mirp/issues). We will then discuss your ideas and create an implementation roadmap.
+IRP is open-source software, hosted on [GitHub](https://github.com/oncoray/mirp). Contributions that enable
+new DICOM modalities are especially welcome! If you have ideas or code to contribute, please first open an
+`issue <https://github.com/oncoray/mirp/issues>`_ and describe your ideas.
 
-Please keep the following in mind when contributing:
+Technical documentation is forthcoming. For now, please keep the following in mind when contributing:
 
 - The main branch of `mirp` is protected. You can therefore make a pull request for your contribution to a 
   development branch of the intended future version.
-- If you introduce new functionality, this functionality should be tested as part of the tests in the `test`directory. 
+- If you introduce new functionality, this functionality should be tested as part of the tests in the `test` directory. 
   After implementation, please ensure that all tests complete without errors by running `pytest` from your IDE or 
   console using `python -m pytest test` from the mirp main directory.  
 - Code is styled according to [PEP8](https://peps.python.org/pep-0008/). Using a linter or IDE with automated linter 
   is recommended.
 - Function, class and method documentation is done using Numpy-flavoured [docstrings](https://numpydoc.readthedocs.io/en/latest/format.html).
   [Long-form documentation](https://oncoray.github.io/mirp/) is partially created from function, class and method 
-  documentation, embedded in restructured text files in `docs_source`.
+  documentation, embedded in restructured text files in the `docs_source` directory.
```

### Comparing `mirp-2.2.0/LICENSE.txt` & `mirp-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/NEWS.md` & `mirp-2.2.1/NEWS.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+# Version 2.2.1
+
+## Minor changes
+
+- If mask-related parameters are not provided for computing features or processing of images for deep learning, a 
+  mask is generated that covers the entire image.
+
+- Add fall-back methods for missing installation of the `ray` package for parallel processing. This can happen when 
+  a python version is not supported by the `ray` package. `ray` is now a conditional dependency, until that package 
+  is released for python `3.12`.
+
+- The default export format for `deep_learning_processing` and `deep_learning_processing_generator` is now `dict`, 
+  because the sample name is important for matching against observed outcomes.
+
+- `write_file` arguments of `extract_mask_labels` and `extract_image_parameters` were deprecated as these were 
+  redundant.
+
+## Fixes
+
+- Streamlined importing and reading DICOM files results in faster processing of DICOM-based imaging.
+
+- Fixed an indexing issue when attempting to split masks into bulk and rim sections in a slice-wise fashion.
+
+- Fixed an indexing issue in Rank's method for noise estimation.
+
+- Fixed incorrectly named image parameters file export. Instead of `mask_labels.csv`, image parameters are now 
+  correctly exported to `image_metadata.csv`.
+
 # Version 2.2.0
 
 ## Major changes
 
 - Added support for intensity scaling using the `intensity_scaling` parameter. Intensity scaling multiplies 
   intensities by a scalar value. Intensity scaling occurs after intensity normalisation (if any) and prior to adding 
   noise (if any). For example, intensity scaling can be used after intensity normalisation to scale intensities to a
```

### Comparing `mirp-2.2.0/PKG-INFO` & `mirp-2.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirp
-Version: 2.2.0
+Version: 2.2.1
 Summary: A package for standardised processing of medical imaging and computation of quantitative features.
 Author-email: Alex Zwanenburg <alexander.zwanenburg@nct-dresden.de>
 License: European Union Public Licence
         V. 1.2
         
         EUPL © the European Union 2007, 2016
         
@@ -280,91 +280,80 @@
         
 Project-URL: Repository, https://github.com/oncoray/mirp
 Project-URL: Documentation, https://oncoray.github.io/mirp/
 Project-URL: Changelog, https://github.com/oncoray/mirp/blob/master/NEWS.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: itk>=5.3.0
 Requires-Dist: matplotlib>=3.7.0
 Requires-Dist: numpy>=1.25
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: pydicom>=2.4.0
 Requires-Dist: pywavelets>=1.4.0
-Requires-Dist: ray>=2.7.0
 Requires-Dist: scikit-image>=0.20.0
 Requires-Dist: scipy>=1.11
 Requires-Dist: typing-extensions>=4.10; python_version < "3.11"
+Requires-Dist: ray>=2.10.0; python_version <= "3.11"
 Provides-Extra: test
 Requires-Dist: pytest>=7.4.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx>=5.0.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=2.0.0; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
 
 <img src="https://raw.githubusercontent.com/oncoray/mirp/master/icon/mirp.svg" align="right" width="120"/>
 
 # Medical Image Radiomics Processor
 
-Medical Image Radiomics Processor (MIRP) is an IBSI-compliant python package for medical image analysis.
-MIRP focuses on radiomics applications and supports computation of features for conventional radiomics
-and image processing for deep-learning applications.
+Medical Image Radiomics Processor (MIRP) is a python package for medical image analysis that is compliant with the 
+reference standards of the Image Biomarker Standardisation Initiative (IBSI). MIRP focuses on radiomics applications 
+and supports computation of features for conventional radiomics and image processing for deep-learning applications.
 
-## Documentation
+## Documentation and tutorials
 
-Documentation can be found here: https://oncoray.github.io/mirp/
+Documentation and tutorials can be found here: https://oncoray.github.io/mirp/
+
+## Supported Python and OS
+
+MIRP currently supports the following Python versions and operating systems: 
+
+| Python | Linux     | Win       | OSX       |
+|--------|-----------|-----------|-----------|
+| 3.10   | Supported | Supported | Supported |
+| 3.11   | Supported | Supported | Supported |
+
+## Supported imaging and mask modalities
+
+MIRP currently supports the following image modalities:
+
+| File format | File type | Supported modality |
+|-------------|-----------|--------------------|
+| DICOM       | image     | CT, MR, PT, RTDOSE |
+| DICOM       | mask      | RTSTRUCT, SEG      |
+| NIfTI       | any       | any                |
+| NRRD        | any       | any                |
+| numpy       | any       | any                |
+
+NIfTI, NRRD, and numpy files support any kind of (single-channel) image. MIRP cannot process RGB or 4D images.
 
 ## Installing MIRP
 MIRP is available from PyPI and can be installed using `pip`, or other installer tools:
 
 ```commandline
 pip install mirp
 ```
 
-## Transitioning to version 2
-
-Version 2 is a major refactoring of the previous code base. For users this brings the following noticeable changes:
-
-- MIRP was previously configured using two `xml` files: [`config_data.xml`](mirp/config_data.xml) for configuring
-  directories, data to be read, etc., and [`config_settings.xml`](mirp/config_settings.xml) for configuring experiments.
-  While these two files can still be used, MIRP can now be configured directly, without using these files.
-- The main functions of MIRP (`mainFunctions.py`) have all been re-implemented.
-  - `mainFunctions.extract_features` is now `extract_features` (functional form) or
-    `extract_features_generator` (generator). The replacements allow for both writing
-    feature values to a directory and returning them as function output. 
-  - `mainFunctions.extract_images_to_nifti` is now `extract_images` (functional form) or
-     `extract_images_generator` (generator). The replacements allow for both writing 
-     images to a directory (e.g., in NIfTI or numpy format) and returning them as function output.
-  - `mainFunctions.extract_images_for_deep_learning` has been replaced by 
-    `deep_learning_preprocessing` (functional form) and 
-    `deep_learning_preprocessing_generator` (generator).
-  - `mainFunctions.get_file_structure_parameters` and `mainFunctions.parse_file_structure` are deprecated, as the
-    the file import system used in version 2 no longer requires a rigid directory structure.
-  - `mainFunctions.get_roi_labels` is now `extract_mask_labels`.
-  - `mainFunctions.get_image_acquisition_parameters` is now `extract_image_parameters`.
-
-For advanced users and developers, the following changes are relevant:
-- MIRP previously relied on `ImageClass` and `RoiClass` objects. These have been completely replaced by `GenericImage`
-  (and its subclasses, e.g. `CTImage`) and `BaseMask` objects, respectively. New image modalities can be added as
-  subclass of `GenericImage` in the `mirp.images` submodule.
-- File import, e.g. from DICOM or NIfTI files, in version 1 was implemented in an ad-hoc manner, and required a rigid
-  directory structure. Since version 2, file import is implemented using an object-oriented approach, and directory
-  structures are more flexible. File import of new modalities can be implemented as a relevant subclass of `ImageFile`.
-- MIRP uses type hinting, and makes use of the `Self` type hint introduced in Python 3.11. MIRP 
-  therefore requires Python 3.11 or later.
-- MIRP now uses the `ray` package for parallel processing.
-
 ## Examples - Computing Radiomics Features
 
 MIRP can be used to compute quantitative features from regions of interest in images in an IBSI-compliant manner 
 using a standardized workflow This requires both images and masks. MIRP can process DICOM, NIfTI, NRRD and numpy 
 images. Masks are DICOM radiotherapy structure sets (RTSTRUCT), or volumetric data with integer labels (e.g. 1, 2, 
 etc.).
 
@@ -462,14 +451,45 @@
 from mirp import extract_mask_labels
 mask_labels = extract_mask_labels(
     mask="path to main mask directory",
     mask_sub_folder="mask subdirectory structure relative to main mask directory"
 )
 ```
 
+## Transitioning to version 2
+
+Version 2 is a major refactoring of the previous code base. For users this brings the following noticeable changes:
+
+- MIRP was previously configured using two `xml` files: [`config_data.xml`](mirp/config_data.xml) for configuring
+  directories, data to be read, etc., and [`config_settings.xml`](mirp/config_settings.xml) for configuring experiments.
+  While these two files can still be used, MIRP can now be configured directly, without using these files.
+- The main functions of MIRP (`mainFunctions.py`) have all been re-implemented.
+  - `mainFunctions.extract_features` is now `extract_features` (functional form) or
+    `extract_features_generator` (generator). The replacements allow for both writing
+    feature values to a directory and returning them as function output. 
+  - `mainFunctions.extract_images_to_nifti` is now `extract_images` (functional form) or
+     `extract_images_generator` (generator). The replacements allow for both writing 
+     images to a directory (e.g., in NIfTI or numpy format) and returning them as function output.
+  - `mainFunctions.extract_images_for_deep_learning` has been replaced by 
+    `deep_learning_preprocessing` (functional form) and 
+    `deep_learning_preprocessing_generator` (generator).
+  - `mainFunctions.get_file_structure_parameters` and `mainFunctions.parse_file_structure` are deprecated, as the
+    the file import system used in version 2 no longer requires a rigid directory structure.
+  - `mainFunctions.get_roi_labels` is now `extract_mask_labels`.
+  - `mainFunctions.get_image_acquisition_parameters` is now `extract_image_parameters`.
+
+For advanced users and developers, the following changes are relevant:
+- MIRP previously relied on `ImageClass` and `RoiClass` objects. These have been completely replaced by `GenericImage`
+  (and its subclasses, e.g. `CTImage`) and `BaseMask` objects, respectively. New image modalities can be added as
+  subclass of `GenericImage` in the `mirp.images` submodule.
+- File import, e.g. from DICOM or NIfTI files, in version 1 was implemented in an ad-hoc manner, and required a rigid
+  directory structure. Since version 2, file import is implemented using an object-oriented approach, and directory
+  structures are more flexible. File import of new modalities can be implemented as a relevant subclass of `ImageFile`.
+- MIRP now uses the `ray` package for parallel processing.
+
 # Citation info
 A publication for MIRP is forthcoming. For now, please cite the following work:
 ```Zwanenburg A, Leger S, Agolli L, Pilz K, Troost EG, Richter C, Löck S. Assessing robustness of radiomic features by image perturbation. Scientific reports. 2019 Jan 24;9(1):614.```
 
 # Contributing
 If you have ideas for improving MIRP, please read the short [contribution guide](./CONTRIBUTING.md).
```

### Comparing `mirp-2.2.0/README.md` & `mirp-2.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,49 @@
 <img src="https://raw.githubusercontent.com/oncoray/mirp/master/icon/mirp.svg" align="right" width="120"/>
 
 # Medical Image Radiomics Processor
 
-Medical Image Radiomics Processor (MIRP) is an IBSI-compliant python package for medical image analysis.
-MIRP focuses on radiomics applications and supports computation of features for conventional radiomics
-and image processing for deep-learning applications.
+Medical Image Radiomics Processor (MIRP) is a python package for medical image analysis that is compliant with the 
+reference standards of the Image Biomarker Standardisation Initiative (IBSI). MIRP focuses on radiomics applications 
+and supports computation of features for conventional radiomics and image processing for deep-learning applications.
 
-## Documentation
+## Documentation and tutorials
 
-Documentation can be found here: https://oncoray.github.io/mirp/
+Documentation and tutorials can be found here: https://oncoray.github.io/mirp/
+
+## Supported Python and OS
+
+MIRP currently supports the following Python versions and operating systems: 
+
+| Python | Linux     | Win       | OSX       |
+|--------|-----------|-----------|-----------|
+| 3.10   | Supported | Supported | Supported |
+| 3.11   | Supported | Supported | Supported |
+
+## Supported imaging and mask modalities
+
+MIRP currently supports the following image modalities:
+
+| File format | File type | Supported modality |
+|-------------|-----------|--------------------|
+| DICOM       | image     | CT, MR, PT, RTDOSE |
+| DICOM       | mask      | RTSTRUCT, SEG      |
+| NIfTI       | any       | any                |
+| NRRD        | any       | any                |
+| numpy       | any       | any                |
+
+NIfTI, NRRD, and numpy files support any kind of (single-channel) image. MIRP cannot process RGB or 4D images.
 
 ## Installing MIRP
 MIRP is available from PyPI and can be installed using `pip`, or other installer tools:
 
 ```commandline
 pip install mirp
 ```
 
-## Transitioning to version 2
-
-Version 2 is a major refactoring of the previous code base. For users this brings the following noticeable changes:
-
-- MIRP was previously configured using two `xml` files: [`config_data.xml`](mirp/config_data.xml) for configuring
-  directories, data to be read, etc., and [`config_settings.xml`](mirp/config_settings.xml) for configuring experiments.
-  While these two files can still be used, MIRP can now be configured directly, without using these files.
-- The main functions of MIRP (`mainFunctions.py`) have all been re-implemented.
-  - `mainFunctions.extract_features` is now `extract_features` (functional form) or
-    `extract_features_generator` (generator). The replacements allow for both writing
-    feature values to a directory and returning them as function output. 
-  - `mainFunctions.extract_images_to_nifti` is now `extract_images` (functional form) or
-     `extract_images_generator` (generator). The replacements allow for both writing 
-     images to a directory (e.g., in NIfTI or numpy format) and returning them as function output.
-  - `mainFunctions.extract_images_for_deep_learning` has been replaced by 
-    `deep_learning_preprocessing` (functional form) and 
-    `deep_learning_preprocessing_generator` (generator).
-  - `mainFunctions.get_file_structure_parameters` and `mainFunctions.parse_file_structure` are deprecated, as the
-    the file import system used in version 2 no longer requires a rigid directory structure.
-  - `mainFunctions.get_roi_labels` is now `extract_mask_labels`.
-  - `mainFunctions.get_image_acquisition_parameters` is now `extract_image_parameters`.
-
-For advanced users and developers, the following changes are relevant:
-- MIRP previously relied on `ImageClass` and `RoiClass` objects. These have been completely replaced by `GenericImage`
-  (and its subclasses, e.g. `CTImage`) and `BaseMask` objects, respectively. New image modalities can be added as
-  subclass of `GenericImage` in the `mirp.images` submodule.
-- File import, e.g. from DICOM or NIfTI files, in version 1 was implemented in an ad-hoc manner, and required a rigid
-  directory structure. Since version 2, file import is implemented using an object-oriented approach, and directory
-  structures are more flexible. File import of new modalities can be implemented as a relevant subclass of `ImageFile`.
-- MIRP uses type hinting, and makes use of the `Self` type hint introduced in Python 3.11. MIRP 
-  therefore requires Python 3.11 or later.
-- MIRP now uses the `ray` package for parallel processing.
-
 ## Examples - Computing Radiomics Features
 
 MIRP can be used to compute quantitative features from regions of interest in images in an IBSI-compliant manner 
 using a standardized workflow This requires both images and masks. MIRP can process DICOM, NIfTI, NRRD and numpy 
 images. Masks are DICOM radiotherapy structure sets (RTSTRUCT), or volumetric data with integer labels (e.g. 1, 2, 
 etc.).
 
@@ -151,14 +141,45 @@
 from mirp import extract_mask_labels
 mask_labels = extract_mask_labels(
     mask="path to main mask directory",
     mask_sub_folder="mask subdirectory structure relative to main mask directory"
 )
 ```
 
+## Transitioning to version 2
+
+Version 2 is a major refactoring of the previous code base. For users this brings the following noticeable changes:
+
+- MIRP was previously configured using two `xml` files: [`config_data.xml`](mirp/config_data.xml) for configuring
+  directories, data to be read, etc., and [`config_settings.xml`](mirp/config_settings.xml) for configuring experiments.
+  While these two files can still be used, MIRP can now be configured directly, without using these files.
+- The main functions of MIRP (`mainFunctions.py`) have all been re-implemented.
+  - `mainFunctions.extract_features` is now `extract_features` (functional form) or
+    `extract_features_generator` (generator). The replacements allow for both writing
+    feature values to a directory and returning them as function output. 
+  - `mainFunctions.extract_images_to_nifti` is now `extract_images` (functional form) or
+     `extract_images_generator` (generator). The replacements allow for both writing 
+     images to a directory (e.g., in NIfTI or numpy format) and returning them as function output.
+  - `mainFunctions.extract_images_for_deep_learning` has been replaced by 
+    `deep_learning_preprocessing` (functional form) and 
+    `deep_learning_preprocessing_generator` (generator).
+  - `mainFunctions.get_file_structure_parameters` and `mainFunctions.parse_file_structure` are deprecated, as the
+    the file import system used in version 2 no longer requires a rigid directory structure.
+  - `mainFunctions.get_roi_labels` is now `extract_mask_labels`.
+  - `mainFunctions.get_image_acquisition_parameters` is now `extract_image_parameters`.
+
+For advanced users and developers, the following changes are relevant:
+- MIRP previously relied on `ImageClass` and `RoiClass` objects. These have been completely replaced by `GenericImage`
+  (and its subclasses, e.g. `CTImage`) and `BaseMask` objects, respectively. New image modalities can be added as
+  subclass of `GenericImage` in the `mirp.images` submodule.
+- File import, e.g. from DICOM or NIfTI files, in version 1 was implemented in an ad-hoc manner, and required a rigid
+  directory structure. Since version 2, file import is implemented using an object-oriented approach, and directory
+  structures are more flexible. File import of new modalities can be implemented as a relevant subclass of `ImageFile`.
+- MIRP now uses the `ray` package for parallel processing.
+
 # Citation info
 A publication for MIRP is forthcoming. For now, please cite the following work:
 ```Zwanenburg A, Leger S, Agolli L, Pilz K, Troost EG, Richter C, Löck S. Assessing robustness of radiomic features by image perturbation. Scientific reports. 2019 Jan 24;9(1):614.```
 
 # Contributing
 If you have ideas for improving MIRP, please read the short [contribution guide](./CONTRIBUTING.md).
```

### Comparing `mirp-2.2.0/mirp/__init__.py` & `mirp-2.2.1/mirp/__init__.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_data_import/dicom_file.py` & `mirp-2.2.1/mirp/_data_import/dicom_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import datetime
 import os.path
 import hashlib
 import numpy as np
 
 from typing import Any
 
 from pydicom import dcmread
 from warnings import warn
 
 from mirp._data_import.generic_file import ImageFile, MaskFile
 from mirp._data_import.utilities import supported_image_modalities, stacking_dicom_image_modalities, \
-    supported_mask_modalities, get_pydicom_meta_tag
+    supported_mask_modalities, get_pydicom_meta_tag, convert_dicom_time
 
 
 class ImageDicomFile(ImageFile):
     def __init__(
             self,
             file_path: None | str = None,
             dir_path: None | str = None,
@@ -83,15 +84,15 @@
     def check(self, raise_error=False, remove_metadata=True) -> bool:
 
         # Metadata needs to be read from files, and should therefore be skipped if not available.
         if self.file_path is None:
             return True
 
         # Checks requires metadata.
-        self.load_metadata()
+        self.load_metadata(limited=True)
 
         # Perform general checks.
         if not super().check(raise_error=raise_error):
             if remove_metadata:
                 self.remove_metadata()
             return False
 
@@ -160,16 +161,15 @@
         # Import locally to prevent circular references.
         from mirp._data_import.dicom_file_ct import ImageDicomFileCT
         from mirp._data_import.dicom_file_mr import ImageDicomFileMR
         from mirp._data_import.dicom_file_pet import ImageDicomFilePT
         from mirp._data_import.dicom_file_rtdose import ImageDicomFileRTDose
 
         # Load metadata so that the modality tag can be read.
-        self.load_metadata()
-
+        self.load_metadata(limited=True)
         modality = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0060), tag_type="str").lower()
 
         if modality is None:
             raise TypeError(f"Modality attribute could not be obtained from DICOM file ({self.file_path})")
 
         if modality == "ct":
             file_class = ImageDicomFileCT
@@ -177,62 +177,77 @@
             file_class = ImageDicomFilePT
         elif modality == "mr":
             file_class = ImageDicomFileMR
         elif modality == "rtdose":
             file_class = ImageDicomFileRTDose
         else:
             # This will return a base class, which will fail to pass the modality check.
-            return self
+            return None
 
-        return file_class(
+        image = file_class(
             file_path=self.file_path,
             dir_path=self.dir_path,
             sample_name=self.sample_name,
             file_name=self.file_name,
             image_modality=self.modality,
             image_name=self.image_name,
             image_file_type=self.file_type,
             image_data=self.image_data,
             image_origin=self.image_origin,
             image_orientation=self.image_orientation,
             image_spacing=self.image_spacing,
-            image_dimensions=self.image_dimension
+            image_dimensions=self.image_dimension,
         )
 
+        # Set metadata of image.
+        image.image_metadata = self.image_metadata
+        image.is_limited_metadata = self.is_limited_metadata
+
+        return image
+
     def complete(self, remove_metadata=False, force=False):
 
         # complete loads metadata.
         super().complete(remove_metadata=False, force=force)
 
         # Set SOP instance UID.
-        self.sop_instance_uid = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0018), tag_type="str")
+        if self.sop_instance_uid is None:
+            self.load_metadata(limited=True)
+            self.sop_instance_uid = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0018), tag_type="str")
 
         # Set Frame of Reference UID (if any)
         self._complete_frame_of_reference_uid()
 
         # Set series UID
-        self.series_instance_uid = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0020, 0x000E), tag_type="str")
+        if self.series_instance_uid is None:
+            self.load_metadata(limited=True)
+            self.series_instance_uid = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0020, 0x000E), tag_type="str")
 
         if remove_metadata:
             self.remove_metadata()
 
     def _complete_modality(self):
         if self.modality is None:
+            self.load_metadata(limited=True)
             self.modality = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0060), tag_type="str")
 
         if self.modality is None:
             warn(f"Could not ascertain the modality from the DICOM file ({self.file_path}).", UserWarning)
 
             self.modality = "generic"
         else:
             self.modality = self.modality.lower()
 
     def _complete_sample_name(self):
         # Set sample name -- note that if sample_name is a (single) string, it is neither replaced nor updated.
         if self.sample_name is None or isinstance(self.sample_name, list):
+
+            # Load relevant metadata.
+            self.load_metadata(limited=True)
+
             # Consider the following DICOM elements:
             # patient id, study id, patient name, series description and study description.
             # These are explicitly ordered by relevance for setting the sample name.
             dicom_sample_name = [
                 get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0010, 0x0020), tag_type="str"),
                 get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0020, 0x0010), tag_type="str"),
                 get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0010, 0x0010), tag_type="str"),
@@ -259,23 +274,29 @@
 
     def _complete_image_origin(self, force=False):
         if self.image_origin is None:
             # Origin needs to be determined at the stack-level for slice-based dicom, not for each slice.
             if self.modality in stacking_dicom_image_modalities() and not force:
                 return
 
+            # Load relevant metadata.
+            self.load_metadata(limited=True)
+
             origin = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0020, 0x0032), tag_type="mult_float")[::-1]
             self.image_origin = tuple(origin)
 
     def _complete_image_orientation(self, force=False):
         if self.image_orientation is None:
             # Orientation needs to be determined at the stack-level for slice-based dicom, not for each slice.
             if self.modality in stacking_dicom_image_modalities() and not force:
                 return
 
+            # Load relevant metadata.
+            self.load_metadata(limited=True)
+
             orientation: list[float] = get_pydicom_meta_tag(
                 dcm_seq=self.image_metadata,
                 tag=(0x0020, 0x0037),
                 tag_type="mult_float"
             )
 
             # First compute z-orientation.
@@ -284,14 +305,17 @@
 
     def _complete_image_spacing(self, force=False):
         if self.image_spacing is None:
             # Image spacing needs to be determined at the stack-level for slice-based dicom, not for each slice.
             if self.modality in stacking_dicom_image_modalities() and not force:
                 return
 
+            # Load relevant metadata.
+            self.load_metadata(limited=True)
+
             # Get pixel-spacing.
             spacing = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x0030), tag_type="mult_float")
 
             # Get slice thickness.
             z_spacing = get_pydicom_meta_tag(
                 dcm_seq=self.image_metadata,
                 tag=(0x0018, 0x0050),
@@ -303,24 +327,28 @@
 
     def _complete_image_dimensions(self, force=False):
         if self.image_dimension is None:
             # Image dimension needs to be determined at the stack-level for slice-based dicom, not for each slice.
             if self.modality in stacking_dicom_image_modalities() and not force:
                 return
 
+            # Load relevant metadata.
+            self.load_metadata(limited=True)
+
             dimensions = tuple([
                 1,
-                get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x010), tag_type="int"),
-                get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x011), tag_type="int")
+                get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x0010), tag_type="int"),
+                get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x0011), tag_type="int")
             ])
 
             self.image_dimension = dimensions
 
     def _complete_frame_of_reference_uid(self):
         if self.frame_of_reference_uid is None:
+            self.load_metadata(limited=True)
             self.frame_of_reference_uid = get_pydicom_meta_tag(
                 dcm_seq=self.image_metadata,
                 tag=(0x0020, 0x0052),
                 tag_type="str"
             )
 
     def associate_with_mask(
@@ -339,28 +367,46 @@
 
             if len(matching_mask_list) > 0:
                 self.associated_masks = matching_mask_list
                 return
 
         return super().associate_with_mask(mask_list=mask_list, association_strategy=association_strategy)
 
-    def load_metadata(self):
-        if self.image_metadata is not None:
+    def load_metadata(self, limited=False, include_image=False):
+        if include_image:
+            limited = False
+
+        # Limited metadata exists and limited metadata is sufficient.
+        if self.image_metadata is not None and self.is_limited_metadata and limited:
+            return
+
+        # A full image metadata set exists.
+        if self.image_metadata is not None and not self.is_limited_metadata:
             return
 
         if self.file_path is None or not os.path.exists(self.file_path):
             raise FileNotFoundError(
                 f"The image file could not be found at the expected location: {self.file_path}")
 
-        dcm = dcmread(
-            self.file_path,
-            stop_before_pixels=True,
-            force=True)
+        if limited:
+            dcm = dcmread(
+                self.file_path,
+                stop_before_pixels=True,
+                force=True,
+                specific_tags=self._get_limited_metadata_tags()
+            )
+        else:
+            dcm = dcmread(
+                self.file_path,
+                stop_before_pixels=not include_image,
+                force=True
+            )
 
         self.image_metadata = dcm
+        self.is_limited_metadata = limited
 
     def load_data(self, **kwargs):
         raise NotImplementedError(
             "DEV: The load_data method should be specified for subclasses of ImageDicomFile. A generic method does not "
             "exist."
         )
 
@@ -377,27 +423,107 @@
                 f"The image file could not be found at the expected location: {self.file_path}"
             )
 
         if self.file_path is None:
             raise ValueError(f"A path to a file was expected, but not present.")
 
         # Load metadata.
-        self.load_metadata()
-
-        # Read
-        dcm = dcmread(self.file_path, stop_before_pixels=False, force=True)
-        image_data = dcm.pixel_array.astype(np.float32)
+        self.load_metadata(include_image=True)
+        image_data = self.image_metadata.pixel_array.astype(np.float32)
 
         # Update data with scale and intercept. These may change per slice.
-        rescale_intercept = get_pydicom_meta_tag(dcm_seq=dcm, tag=(0x0028, 0x1052), tag_type="float", default=0.0)
-        rescale_slope = get_pydicom_meta_tag(dcm_seq=dcm, tag=(0x0028, 0x1053), tag_type="float", default=1.0)
+        rescale_intercept = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x1052), tag_type="float", default=0.0)
+        rescale_slope = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x1053), tag_type="float", default=1.0)
         image_data = image_data * rescale_slope + rescale_intercept
 
         return image_data
 
+    @staticmethod
+    def _get_limited_metadata_tags():
+        # Limited tags are read to populate basic
+        return [
+            (0x0008, 0x0018),  # SOP instance UID
+            (0x0008, 0x0060),  # modality
+            (0x0008, 0x1030),  # series description
+            (0x0008, 0x103E),  # study description
+            (0x0010, 0x0010),  # patient name
+            (0x0010, 0x0020),  # patient id
+            (0x0018, 0x0050),  # slice thickness
+            (0x0020, 0x000E),  # series instance UID
+            (0x0020, 0x0010),  # study id
+            (0x0020, 0x0032),  # origin
+            (0x0020, 0x0037),  # orientation
+            (0x0020, 0x0052),  # frame of reference UID
+            (0x0028, 0x0008),  # number of frames
+            (0x0028, 0x0010),  # pixel rows
+            (0x0028, 0x0011),  # pixel columns
+            (0x0028, 0x0030),  # pixel spacing
+            (0x3004, 0x000C)  # grid frame offset vector
+        ]
+
+    def _get_acquisition_start_time(self) -> datetime.datetime:
+        self.load_metadata()
+
+        # Start of image acquisition. Prefer Acquisition Datetime (0x0008, 0x002A).
+        acquisition_ref_time = get_pydicom_meta_tag(
+            dcm_seq=self.image_metadata,
+            tag=(0x0008, 0x002A),
+            tag_type="str"
+        )
+        acquisition_ref_time = convert_dicom_time(datetime_str=acquisition_ref_time)
+
+        # Fall back to Acquisition Date (0x0008, 0x002A) and Acquisition Time (0x0008, 0x0032).
+        if acquisition_ref_time is None:
+            acquisition_start_date = get_pydicom_meta_tag(
+                dcm_seq=self.image_metadata,
+                tag=(0x0008, 0x0022),
+                tag_type="str"
+            )
+            acquisition_start_time = get_pydicom_meta_tag(
+                dcm_seq=self.image_metadata,
+                tag=(0x0008, 0x0032),
+                tag_type="str"
+            )
+            acquisition_ref_time = convert_dicom_time(
+                date_str=acquisition_start_date,
+                time_str=acquisition_start_time
+            )
+
+        # Fall back to Private GE Acquisition DateTime (0x0009, 0x100d).
+        if acquisition_ref_time is None:
+            acquisition_ref_time = get_pydicom_meta_tag(
+                dcm_seq=self.image_metadata,
+                tag=(0x0009, 0x100d),
+                tag_type="str"
+            )
+            acquisition_ref_time = convert_dicom_time(datetime_str=acquisition_ref_time)
+
+        # Fall back to Series Date and Series Time (
+        if acquisition_ref_time is None:
+            acquisition_start_date = get_pydicom_meta_tag(
+                dcm_seq=self.image_metadata,
+                tag=(0x0008, 0x0021),
+                tag_type="str"
+            )
+            acquisition_start_time = get_pydicom_meta_tag(
+                dcm_seq=self.image_metadata,
+                tag=(0x0008, 0x0031),
+                tag_type="str"
+            )
+            acquisition_ref_time = convert_dicom_time(
+                date_str=acquisition_start_date,
+                time_str=acquisition_start_time
+            )
+
+        # Final check.
+        if acquisition_ref_time is None:
+            raise ValueError(f"Acquisition start time cannot be determined from DICOM metadata in {self.file_path}.")
+
+        return acquisition_ref_time
+
 
 class MaskDicomFile(ImageDicomFile, MaskFile):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def _check_modality(self, raise_error: bool) -> bool:
         dicom_modality = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0060), tag_type="str")
@@ -426,37 +552,50 @@
         """
 
         # Import locally to prevent circular references.
         from mirp._data_import.dicom_file_rtstruct import MaskDicomFileRTSTRUCT
         from mirp._data_import.dicom_file_seg import MaskDicomFileSEG
 
         # Load metadata so that the modality tag can be read.
-        self.load_metadata()
+        self.load_metadata(limited=True)
 
         modality = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0008, 0x0060), tag_type="str").lower()
 
         if modality is None:
             raise TypeError(f"Modality attribute could not be obtained from DICOM file ({self.file_path})")
 
         if modality == "rtstruct":
             file_class = MaskDicomFileRTSTRUCT
         elif modality == "seg":
             file_class = MaskDicomFileSEG
         else:
-            # This will return a base class, which will fail to pass the modality check.
-            return self
+            return None
 
-        return file_class(
+        mask = file_class(
             file_path=self.file_path,
             dir_path=self.dir_path,
             sample_name=self.sample_name,
             file_name=self.file_name,
             image_modality=self.modality,
             image_name=self.image_name,
             image_file_type=self.file_type,
             image_data=self.image_data,
             image_origin=self.image_origin,
             image_orientation=self.image_orientation,
             image_spacing=self.image_spacing,
             image_dimensions=self.image_dimension,
             roi_name=self.roi_name
         )
+
+        # Set metadata of mask.
+        mask.image_metadata = self.image_metadata
+        mask.is_limited_metadata = self.is_limited_metadata
+
+        return mask
+
+    def _get_limited_metadata_tags(self):
+        tags = super()._get_limited_metadata_tags()
+
+        tags += [
+            (0x3006, 0x0020),  # Structure set roi sequence
+            (0x0028, 0x0008)  # number of frames
+        ]
```

### Comparing `mirp-2.2.0/mirp/_data_import/dicom_file_ct.py` & `mirp-2.2.1/mirp/_data_import/dicom_file_ct.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_data_import/dicom_file_mr.py` & `mirp-2.2.1/mirp/_data_import/dicom_file_mr.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_data_import/dicom_file_rtdose.py` & `mirp-2.2.1/mirp/_data_import/dicom_file_rtdose.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         return False
 
     def create(self):
         return self
 
     def _complete_image_orientation(self, force=False):
         if self.image_orientation is None:
+            # Load relevant metadata.
+            self.load_metadata(limited=True)
 
             # This is orientation for x and y directions.
             orientation: list[float] = get_pydicom_meta_tag(
                 dcm_seq=self.image_metadata,
                 tag=(0x0020, 0x0037),
                 tag_type="mult_float"
             )
@@ -62,14 +64,17 @@
             orientation += list(np.cross(orientation[0:3], orientation[3:6]))
 
             self.image_orientation = np.reshape(orientation[::-1], [3, 3], order="F")
 
     def _complete_image_spacing(self, force=False):
         if self.image_spacing is None:
 
+            # Load relevant metadata.
+            self.load_metadata(limited=True)
+
             # Get pixel-spacing.
             spacing = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x0030), tag_type="mult_float")
 
             # Get Grid Frame Offset Vector
             z_spacing = get_pydicom_meta_tag(
                 dcm_seq=self.image_metadata,
                 tag=(0x3004, 0x000C),
@@ -100,18 +105,22 @@
 
             spacing += [z_spacing]
 
             self.image_spacing = tuple(spacing[::-1])
 
     def _complete_image_dimensions(self, force=False):
         if self.image_dimension is None:
+
+            # Load relevant metadata.
+            self.load_metadata(limited=True)
+
             dimensions = tuple([
-                get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x008), tag_type="int"),
-                get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x010), tag_type="int"),
-                get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x011), tag_type="int")
+                get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x0008), tag_type="int"),
+                get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x0010), tag_type="int"),
+                get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0028, 0x0011), tag_type="int")
             ])
 
             self.image_dimension = dimensions
 
     def load_data(self, **kwargs):
         if self.image_data is not None:
             return self.image_data
@@ -121,22 +130,19 @@
                 f"The image file could not be found at the expected location: {self.file_path}"
             )
 
         if self.file_path is None:
             raise ValueError(f"A path to a file was expected, but not present.")
 
         # Load metadata.
-        self.load_metadata()
-
-        # Read
-        dcm = dcmread(self.file_path, stop_before_pixels=False, force=True)
-        image_data = dcm.pixel_array.astype(np.float32)
+        self.load_metadata(include_image=True)
+        image_data = self.image_metadata.pixel_array.astype(np.float32)
 
         # Update data with dose grid scaling
-        dose_grid_scaling = get_pydicom_meta_tag(dcm_seq=dcm, tag=(0x3004, 0x000E), tag_type="float", default=1.0)
+        dose_grid_scaling = get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x3004, 0x000E), tag_type="float", default=1.0)
         image_data = image_data * dose_grid_scaling
 
         self.image_data = image_data
 
     def export_metadata(self, self_only: bool = False, **kwargs) -> None | dict[str, Any]:
         if not self_only:
             metadata = super().export_metadata()
```

### Comparing `mirp-2.2.0/mirp/_data_import/dicom_file_rtstruct.py` & `mirp-2.2.1/mirp/_data_import/dicom_file_rtstruct.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         return
 
     def _complete_image_dimensions(self, force=False):
         return
 
     def _complete_frame_of_reference_uid(self):
         if self.frame_of_reference_uid is None:
+            self.load_metadata(limited=True)
+
             # Try to obtain a frame of reference UID
             if has_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0020, 0x0052)):
                 if get_pydicom_meta_tag(dcm_seq=self.image_metadata, tag=(0x0020, 0x0052), tag_type="str") is not None:
                     self.frame_of_reference_uid = get_pydicom_meta_tag(
                         dcm_seq=self.image_metadata,
                         tag=(0x0020, 0x0052),
                         tag_type="str")
@@ -188,21 +190,21 @@
             if image_data is None:
                 continue
 
             if not np.any(image_data):
                 continue
 
             # Complete a copy of the current object.
-            temp_mask_object = self.copy()
-            temp_mask_object.image_data = image_data
-            temp_mask_object.image_origin = image.image_origin
-            temp_mask_object.image_spacing = image.image_spacing
-            temp_mask_object.image_dimension = image.image_dimension
-            temp_mask_object.image_orientation = image.image_orientation
-            temp_mask_object.complete()
+            temp_mask_object = MaskDicomFile(
+                image_data=image_data,
+                image_origin=image.image_origin,
+                image_spacing=image.image_spacing,
+                image_dimensions=image.image_dimension,
+                image_orientation=image.image_orientation
+            )
             temp_mask_object.update_image_data()
 
             current_roi_name = [
                 x for ii, x in enumerate(roi_name_present) if roi_number_present[ii] == current_roi_number
             ][0]
 
             if isinstance(self.roi_name, dict):
```

### Comparing `mirp-2.2.0/mirp/_data_import/dicom_file_seg.py` & `mirp-2.2.1/mirp/_data_import/dicom_file_seg.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_data_import/dicom_file_stack.py` & `mirp-2.2.1/mirp/_data_import/dicom_file_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         by origin, and uses their relative positions to determine slice spacing and the orientation vector.
         :param remove_metadata: Whether metadata (DICOM headers) should be removed after completing information.
         :param force: Whether attributes are forced to update or not.
         :return: nothing, attributes are updated in place.
         """
 
         # Load metadata of every slice.
-        self.load_metadata()
+        self.load_metadata(limited=True)
 
         self._complete_modality()
         self._complete_sample_name()
 
         # Set image orientation.
         # First read orientation (Xx, Xy, Xz, Yx, Yy, Yz) from metadata.
         image_orientation: list[float] = get_pydicom_meta_tag(
@@ -177,19 +177,19 @@
         # Determine how image objects should be sorted according to increasing layer positions.
         new_order = np.argsort(layer_positions)
         self.image_file_objects = [self.image_file_objects[ii] for ii in new_order]
 
         # Set image dimensions. First, find the number of rows (y) and columns (x) in the data set.
         n_x = get_pydicom_meta_tag(
             dcm_seq=self.image_file_objects[0].image_metadata,
-            tag=(0x0028, 0x011),
+            tag=(0x0028, 0x0011),
             tag_type="int")
         n_y = get_pydicom_meta_tag(
             dcm_seq=self.image_file_objects[0].image_metadata,
-            tag=(0x0028, 0x010),
+            tag=(0x0028, 0x0010),
             tag_type="int")
 
         if self.image_dimension is None:
             self.image_dimension = tuple([len(position_table), n_y, n_x])
 
         if self.sop_instance_uid is None:
             self.sop_instance_uid = [image.sop_instance_uid for image in self.image_file_objects]
```

### Comparing `mirp-2.2.0/mirp/_data_import/directory.py` & `mirp-2.2.1/mirp/_data_import/directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,17 @@
                 # Skip files that do not have the right extension.
                 if not current_item.lower().endswith(tuple(allowed_file_extensions)):
                     continue
 
                 if self.image_name is not None:
                     # Skip files that do not contain the image_name pattern.
                     if not match_file_name(
-                            current_item, pattern=self.image_name, file_extension=allowed_file_extensions
+                            current_item,
+                            pattern=self.image_name,
+                            file_extension=allowed_file_extensions
                     ):
                         continue
 
                 image_file_list.append(current_item)
 
             self.image_files = image_file_list
 
@@ -401,16 +403,18 @@
             return []
 
         image_file_list = []
         for image_file_name in self.image_files:
 
             # Create image file object.
             image_file = self._create_image_file(image_file_name=image_file_name)
+            if image_file is None:
+                continue
 
-            if not image_file.check(raise_error=False):
+            if not image_file.check(raise_error=False, remove_metadata=False):
                 continue
 
             image_file.complete()
 
             image_file_list.append(image_file)
 
         return image_file_list
```

### Comparing `mirp-2.2.0/mirp/_data_import/generic_file.py` & `mirp-2.2.1/mirp/_data_import/generic_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         self.update_image_data()
 
         # Check updated image data.
         _ = self._check_image_data()
 
         # Add metadata
         self.image_metadata = None
+        self.is_limited_metadata = False
 
         # Attempt to set the file name, if this is not externally provided.
         if isinstance(file_path, str) and file_name is None:
             file_name = os.path.basename(file_path)
 
         # Attempt to set the directory path, if this is not externally provided.
         if isinstance(file_path, str) and dir_path is None:
@@ -84,14 +85,17 @@
             f"DEV: There is (intentionally) no generic implementation of is_stackable. Please specify "
             f"implementation for subclasses."
         )
 
     def copy(self):
         return copy.deepcopy(self)
 
+    def on_file_system(self):
+        return self.file_path is None or self.dir_path is None
+
     def get_identifiers(self, as_hash=False) -> dict | bytes:
         """
         General identifiers for images. Note that image_origin is not included, as this should be different for every
         slice in a volume.
         :param as_hash: boolean flag. When true returns a SHA256 hash of the identifier data.
         :return: a dictionary with identifiers.
         """
@@ -415,34 +419,37 @@
                     return False
 
     def _check_sample_name(self, raise_error: bool) -> bool:
         # Check that image file contains a sample name, if multiple sample names are present. To assess the filename,
         # we first strip the extension. Optionally we split the filename on the image name pattern, reducing the
         # filename into parts that should contain the sample name.
         if isinstance(self.sample_name, list) and len(self.sample_name) > 1:
-            if self._get_sample_name_from_file() is None:
+            if self.get_sample_name_from_file() is None:
                 if raise_error:
                     raise ValueError(
                         f"The file name of the image file {os.path.basename(self.file_path)} does not contain "
                         f"any of the expected patterns: {', '.join(self.sample_name)}")
                 else:
                     return False
 
         return True
 
     def _check_modality(self, raise_error: bool) -> bool:
         return True
 
-    def _get_sample_name_from_file(self) -> None | str:
+    def get_sample_name_from_file(self, must_succeed=False) -> None | str:
         allowed_file_extensions = supported_file_types(self.file_type)
 
         # Do not obtain sample name from the file name if a file name has already been set.
         if isinstance(self.sample_name, str):
             return None
 
+        if self.file_name is None:
+            return None
+
         # Select the most appropriate sample name.
         if isinstance(self.sample_name, list) and len(self.sample_name) > 1:
             file_name = bare_file_name(x=self.file_name, file_extension=allowed_file_extensions)
             if self.image_name is not None:
                 image_id_name = self.image_name
                 if not isinstance(image_id_name, list):
                     image_id_name = [image_id_name]
@@ -496,14 +503,16 @@
                             matching_name = current_sample_name
 
                             if matching_frac == 1.0:
                                 return matching_name
 
             return matching_name
 
+        elif must_succeed:
+            return bare_file_name(x=self.file_name, file_extension=allowed_file_extensions)
         else:
             return None
 
     def _get_numeric_sequence_from_file(self) -> None | list[str]:
         allowed_file_extensions = supported_file_types(self.file_type)
         file_name = bare_file_name(x=self.file_name, file_extension=allowed_file_extensions)
 
@@ -584,17 +593,14 @@
         if len(file_name_parts) == 0:
             return None
 
         # Flatten list and return.
         return list(itertools.chain.from_iterable(file_name_parts))
 
     def complete(self, remove_metadata=False, force=False):
-        # Load metadata.
-        self.load_metadata()
-
         self._complete_modality()
         self._complete_sample_name()
         self._complete_image_dimensions(force=force)
         self._complete_image_origin(force=force)
         self._complete_image_orientation(force=force)
         self._complete_image_spacing(force=force)
 
@@ -609,15 +615,15 @@
         # Set modality.
         if self.modality is None:
             self.modality = "generic"
 
     def _complete_sample_name(self):
         # Set sample name.
         if isinstance(self.sample_name, list):
-            file_sample_name = self._get_sample_name_from_file()
+            file_sample_name = self.get_sample_name_from_file()
 
             if file_sample_name is None and len(self.sample_name) == 1:
                 self.sample_name = self.sample_name[0]
 
             elif file_sample_name is not None:
                 self.sample_name = file_sample_name
 
@@ -644,15 +650,15 @@
 
     def _complete_image_dimensions(self, force=False):
         raise NotImplementedError(
             f"DEV: There is (intentionally) no generic implementation of _complete_sample_dimensions. Please specify "
             f"implementation for subclasses."
         )
 
-    def load_metadata(self):
+    def load_metadata(self, limited=False, include_image=False):
         raise NotImplementedError(
             f"DEV: There is (intentionally) no generic implementation of load_metadata. Please specify "
             f"implementation for subclasses."
         )
 
     def remove_metadata(self):
         self.image_metadata = None
@@ -744,15 +750,15 @@
             if dims_to_add == 1:
                 image_spacing.insert(0, 1.0)
 
             self.image_spacing = tuple(image_spacing)
 
     def to_object(self, **kwargs) -> GenericImage:
 
-        self.load_data()
+        self.load_data(**kwargs)
         self.complete()
         self.stack_slices()
         self.update_image_data()
 
         return GenericImage(
             sample_name=self.sample_name,
             image_modality=self.modality,
@@ -830,15 +836,15 @@
 
     def _complete_image_dimensions(self, force=False):
         raise NotImplementedError(
             f"DEV: There is (intentionally) no generic implementation of _complete_image_dimensions. Please specify "
             f"implementation for subclasses."
         )
 
-    def load_metadata(self):
+    def load_metadata(self, **kwargs):
         raise NotImplementedError(
             f"DEV: There is (intentionally) no generic implementation of load_metadata. Please specify "
             f"implementation for subclasses."
         )
 
     def load_data(self, **kwargs):
         raise NotImplementedError(
@@ -1093,7 +1099,39 @@
 
         return {
             "sample_name": [self.sample_name] * n_labels,
             "dir_path": [self.dir_path] * n_labels,
             "file_path": [self.file_name] * n_labels,
             "roi_label": labels
         }
+
+
+class MaskFullImage(MaskFile):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.roi_name = "full_image_mask"
+
+    def to_object(
+            self,
+            image: None | ImageFile,
+            **kwargs
+    ) -> None | list[BaseMask]:
+        if image is None:
+            raise TypeError(
+                f"Creation of a full image mask requires that the corresponding image is set. "
+                f"No image was provided ({self.file_path})."
+            )
+        else:
+            image.complete()
+
+        self._complete_modality()
+
+        return [BaseMask(
+            roi_name=self.roi_name,
+            sample_name=image.sample_name,
+            image_modality=self.modality,
+            image_data=np.ones(image.image_dimension, dtype=bool),
+            image_spacing=image.image_spacing,
+            image_origin=image.image_origin,
+            image_orientation=image.image_orientation,
+            image_dimensions=image.image_dimension
+        )]
```

### Comparing `mirp-2.2.0/mirp/_data_import/generic_file_stack.py` & `mirp-2.2.1/mirp/_data_import/generic_file_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,25 +100,21 @@
         raise NotImplementedError(
             f"DEV: There is (intentionally) no generic implementation of complete. Please specify "
             f"implementation for subclasses."
         )
 
     def _complete_sample_name(self):
         if self.sample_name is None:
-            image_object = copy.deepcopy(self.image_file_objects[0])
-            image_object._complete_sample_name()
-
-            self.sample_name = image_object.sample_name
+            self.image_file_objects[0]._complete_sample_name()
+            self.sample_name = self.image_file_objects[0].sample_name
 
     def _complete_modality(self):
         if self.modality is None:
-            image_object = copy.deepcopy(self.image_file_objects[0])
-            image_object._complete_modality()
-
-            self.modality = image_object.modality
+            self.image_file_objects[0]._complete_modality()
+            self.modality = self.image_file_objects[0].modality
 
     def _complete_image_origin(self, force=False):
         # Image origin and other image-related aspects are set using the complete method of subclasses.
         pass
 
     def _complete_image_orientation(self, force=False):
         pass
@@ -178,23 +174,27 @@
 
         # Sort image file objects.
         self.image_file_objects = [
             self.image_file_objects[position_table.original_object_order[ii]]
             for ii in range(len(position_table))
         ]
 
-    def load_metadata(self):
+    def load_metadata(self, limited=False, include_image=False):
         # Load metadata for underlying files in the order indicated by self.image_file_objects.
         for image_file_object in self.image_file_objects:
-            image_file_object.load_metadata()
+            image_file_object.load_metadata(limited=limited, include_image=include_image)
+
+    def remove_metadata(self):
+        for image_file_object in self.image_file_objects:
+            image_file_object.remove_metadata()
 
     def load_data(self, **kwargs):
         # Load data for underlying files in the order indicated by self.image_file_objects.
         for image_file_object in self.image_file_objects:
-            image_file_object.load_data()
+            image_file_object.load_data(**kwargs)
 
     def stack_slices(self):
         if self.image_data is not None:
             return
 
         image = np.zeros(self.image_dimension, dtype=np.float32)
         for ii, image_file in enumerate(self.image_file_objects):
```

### Comparing `mirp-2.2.0/mirp/_data_import/itk_file.py` & `mirp-2.2.1/mirp/_data_import/itk_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,51 +66,59 @@
         else:
             raise ValueError(
                 f"The stack_images argument is expected to be one of yes, auto, or no. Found: {stack_images}."
             )
 
     def _complete_image_origin(self, force=False):
         if self.image_origin is None:
+            self.load_metadata()
+
             # Get dimensions, as this determines what can be meaningfully read.
             n_dimensions = self.image_metadata.GetNumberOfDimensions()
 
             # Get origin.
             origin = [0.0] * n_dimensions
             for ii in range(n_dimensions):
                 origin[n_dimensions - (ii + 1)] = self.image_metadata.GetOrigin(ii)
 
             # Set origin.
             self.image_origin = tuple(origin)
 
     def _complete_image_orientation(self, force=False):
         if self.image_orientation is None:
+            self.load_metadata()
+
             # Get dimensions, as this determines what can be meaningfully read.
             n_dimensions = self.image_metadata.GetNumberOfDimensions()
 
             # Get orientation.
             orientation = []
             for ii in range(n_dimensions):
                 orientation.append(self.image_metadata.GetDirection(ii))
 
             self.image_orientation = np.reshape(np.ravel(np.array(orientation))[::-1], [n_dimensions, n_dimensions])
 
     def _complete_image_spacing(self, force=False):
         if self.image_spacing is None:
+            self.load_metadata()
+
             # Get dimensions, as this determines what can be meaningfully read.
             n_dimensions = self.image_metadata.GetNumberOfDimensions()
 
             # Get spacing.
             spacing = [0.0] * n_dimensions
             for ii in range(n_dimensions):
                 spacing[n_dimensions - (ii + 1)] = self.image_metadata.GetSpacing(ii)
 
             # Set spacing.
             self.image_spacing = tuple(spacing)
 
     def _complete_image_dimensions(self, force=False):
+        self.load_metadata()
+
         if self.image_dimension is None:
             # Get dimensions, as this determines what can be meaningfully read.
             n_dimensions = self.image_metadata.GetNumberOfDimensions()
 
             # Get size of dimensions
             dimensions = [0] * n_dimensions
             for ii in range(n_dimensions):
@@ -118,15 +126,15 @@
 
             # Set size of dimensions
             self.image_dimension = tuple(dimensions)
 
     def create(self):
         return self
 
-    def load_metadata(self):
+    def load_metadata(self, **kwargs):
         if self.image_metadata is not None:
             return
 
         if self.file_path is None or not os.path.exists(self.file_path):
             raise FileNotFoundError(
                 f"The image file could not be found at the expected location: {self.file_path}")
```

### Comparing `mirp-2.2.0/mirp/_data_import/itk_file_stack.py` & `mirp-2.2.1/mirp/_data_import/itk_file_stack.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_data_import/mask_contour.py` & `mirp-2.2.1/mirp/_data_import/mask_contour.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                 origin=np.array([0.0, 0.0]),
                 shape=np.array([image.image_dimension[1], image.image_dimension[2]])
             ))
 
         return slice_list, mask_list
 
 
-def mesh2grid(verts, faces, spacing, origin=None):
+def mesh2grid(verts, faces, spacing, origin=None):  # pragma: no cover
 
     # Remove superfluous dimensions
     verts = np.squeeze(np.asarray(verts))
 
     # Determine triangle vertices
     vert_1 = verts[faces[:, 0], :]
     vert_2 = verts[faces[:, 1], :]
@@ -279,15 +279,15 @@
 
         # Voxels in the roi cross an uneven number of meshes from the origin
         vox_grid[:, x_ind] += np.logical_and(vox_col_frwd % 2, vox_col_bkwd % 2)
 
     return vox_grid.astype(dtype=bool)
 
 
-def ray_triangle_intersect(ray_orig, ray_dir, vert_1, vert_2, vert_3):
+def ray_triangle_intersect(ray_orig, ray_dir, vert_1, vert_2, vert_3):  # pragma: no cover
     # Implementation of the Moeller-Trumbore intersection algorithm to determine intersection point
     # between ray and triangle
     # This point satisfies ray_orig + t * ray_dir = (1 - u -v) * vert_1 + u * vert_2 + v * vert_3
     # See DOI: 10.1145/1198555.1198746
     # Back facing triangles are allowed
 
     epsilon = 0.000001
```

### Comparing `mirp-2.2.0/mirp/_data_import/numpy_file.py` & `mirp-2.2.1/mirp/_data_import/numpy_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,35 +91,39 @@
 
             return False
 
         return True
 
     def _complete_image_origin(self, force=False):
         if self.image_origin is None:
+            self.load_metadata()
             n_dim = len(self.image_metadata.shape)
             self.image_origin = tuple([0.0] * n_dim)
 
     def _complete_image_orientation(self, force=False):
         if self.image_orientation is None:
+            self.load_metadata()
             n_dim = len(self.image_metadata.shape)
             self.image_orientation = np.identity(n_dim, dtype=float)
 
     def _complete_image_spacing(self, force=False):
         if self.image_spacing is None:
+            self.load_metadata()
             n_dim = len(self.image_metadata.shape)
             self.image_spacing = tuple([1.0] * n_dim)
 
     def _complete_image_dimensions(self, force=False):
         if self.image_dimension is None:
+            self.load_metadata()
             self.image_dimension = tuple(self.image_metadata.shape)
 
     def create(self):
         return self
 
-    def load_metadata(self):
+    def load_metadata(self, **kwargs):
         if self.image_metadata is not None:
             return
 
         if self.file_path is None or not os.path.exists(self.file_path):
             raise FileNotFoundError(
                 f"The image file could not be found at the expected location: {self.file_path}")
```

### Comparing `mirp-2.2.0/mirp/_data_import/numpy_file_stack.py` & `mirp-2.2.1/mirp/_data_import/numpy_file_stack.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_data_import/read_data.py` & `mirp-2.2.1/mirp/_data_import/read_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,41 +4,43 @@
 from mirp._data_import.utilities import flatten_list
 from mirp._images.generic_image import GenericImage
 from mirp._masks.base_mask import BaseMask
 
 
 def read_image(
         image: ImageFile,
-        to_numpy=False
+        to_numpy=False,
+        **kwargs
 ) -> np.ndarray | GenericImage:
-    image = image.to_object().promote()
+    image = image.to_object(**kwargs).promote()
 
     if to_numpy:
         image = image.get_voxel_grid()
 
     return image
 
 
 def read_image_and_masks(
         image: ImageFile,
-        to_numpy=False
+        to_numpy=False,
+        **kwargs
 ) -> tuple[np.ndarray | GenericImage, list[np.ndarray] | list[BaseMask]]:
+    # Read image from file.
+    image_out = image.to_object(**kwargs).promote()
+
     mask_list = []
     if image.associated_masks is not None:
         mask_list = image.associated_masks
 
     # Read masks from file.
     if mask_list is not None:
-        mask_list = [mask.to_object(image=image) for mask in mask_list]
+        mask_list = [mask.to_object(image=image, **kwargs) for mask in mask_list]
         mask_list = flatten_list(mask_list)
 
     # Remove None entries.
     mask_list = [mask for mask in mask_list if mask is not None]
 
-    # Read image from file.
-    image = image.to_object().promote()
-
     if to_numpy:
-        image = image.get_voxel_grid()
+        image_out = image_out.get_voxel_grid()
         mask_list = [mask.roi.get_voxel_grid() for mask in mask_list]
 
-    return image, mask_list
+    return image_out, mask_list
```

### Comparing `mirp-2.2.0/mirp/_data_import/suv.py` & `mirp-2.2.1/mirp/_data_import/suv.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from copy import deepcopy
 
 import numpy as np
 
 from mirp._data_import.utilities import convert_dicom_time, get_pydicom_meta_tag, set_pydicom_meta_tag
 
 
-class SUVscalingObj:
+class SUVscalingObj:  # pragma: no cover
 
     def __init__(self, dcm):
 
         # Start of image acquisition for the current position
         acquisition_start_date = get_pydicom_meta_tag(dcm_seq=dcm, tag=(0x0008, 0x0022), tag_type="str")
         acquisition_start_time = get_pydicom_meta_tag(dcm_seq=dcm, tag=(0x0008, 0x0032), tag_type="str")
         self.acquisition_ref_time = convert_dicom_time(date_str=acquisition_start_date, time_str=acquisition_start_time)
```

### Comparing `mirp-2.2.0/mirp/_data_import/utilities.py` & `mirp-2.2.1/mirp/_data_import/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_featuresets/cm.py` & `mirp-2.2.1/mirp/_featuresets/cm.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_featuresets/dzm.py` & `mirp-2.2.1/mirp/_featuresets/dzm.py`

 * *Files 10% similar despite different names*

```diff
@@ -217,73 +217,14 @@
 
         # Rename columns
         df_dzm.columns = ["i", "d", "n"]
 
         # Add matrix to object
         self.matrix = df_dzm
 
-    def calculate_matrix_deprecated(self, img_obj, roi_obj, df_img):
-
-        # Check if the input image and roi exist
-        if img_obj.is_missing or roi_obj.roi_intensity is None or df_img is None:
-            self.set_empty()
-            return
-
-        # Check if the roi contains any masked voxels. If this is not the case, don't construct the GLDZM.
-        if not np.any(roi_obj.roi_intensity.get_voxel_grid()):
-            self.set_empty()
-            return
-
-        from skimage.measure import label
-
-        # Define neighbour directions
-        if self.spatial_method == "3d":
-            connectivity = 3
-            img_vol = copy.deepcopy(img_obj.get_voxel_grid())
-            roi_vol = copy.deepcopy(roi_obj.roi_intensity.get_voxel_grid())
-            df_dzm = copy.deepcopy(df_img)
-
-        elif self.spatial_method in ["2d", "2.5d"]:
-            connectivity = 2
-            img_vol = img_obj.get_voxel_grid()[self.slice, :, :]
-            roi_vol = roi_obj.roi_intensity.get_voxel_grid()[self.slice, :, :]
-            df_dzm = copy.deepcopy(df_img[df_img.z == self.slice])
-
-        else:
-            raise ValueError("The spatial method for grey level distance zone matrices should be one of \"2d\", \"2.5d\" or \"3d\".")
-
-        # Check dimensionality and update connectivity if necessary.
-        connectivity = min([connectivity, real_ndim(img_vol)])
-
-        # Set voxels outside the roi to 0.0
-        img_vol[~roi_vol] = 0.0
-
-        # Count the number of voxels within the roi
-        self.n_v = np.sum(roi_vol)
-
-        # Label all connected voxels with the same grey level
-        img_label = label(img_vol, background=0, connectivity=connectivity)
-
-        # Add group labels
-        df_dzm["vol_id"] = np.ravel(img_label)
-
-        # Select minimum group distance for unique groups
-        df_dzm = df_dzm[df_dzm.roi_int_mask].groupby(by=["g", "vol_id"])["border_distance"].min().reset_index(
-
-        ).rename(columns={"border_distance": "d"})
-
-        # Count occurrence of grey level and distance
-        df_dzm = df_dzm.groupby(by=["g", "d"]).size().reset_index(name="n")
-
-        # Rename columns
-        df_dzm.columns = ["i", "d", "n"]
-
-        # Add matrix to object
-        self.matrix = df_dzm
-
     def compute_features(self):
 
         # Create feature table
         feat_names = ["dzm_sde", "dzm_lde", "dzm_lgze", "dzm_hgze", "dzm_sdlge", "dzm_sdhge", "dzm_ldlge", "dzm_ldhge",
                       "dzm_glnu", "dzm_glnu_norm", "dzm_zdnu", "dzm_zdnu_norm", "dzm_z_perc",
                       "dzm_gl_var", "dzm_zd_var", "dzm_zd_entr"]
         df_feat = pd.DataFrame(np.full(shape=(1, len(feat_names)), fill_value=np.nan))
```

### Comparing `mirp-2.2.0/mirp/_featuresets/intensity_histogram.py` & `mirp-2.2.1/mirp/_featuresets/intensity_histogram.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_featuresets/intensity_volume_histogram.py` & `mirp-2.2.1/mirp/_featuresets/intensity_volume_histogram.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_featuresets/local_intensity.py` & `mirp-2.2.1/mirp/_featuresets/local_intensity.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_featuresets/morphology_3d.py` & `mirp-2.2.1/mirp/_featuresets/morphology_3d.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_featuresets/ngldm.py` & `mirp-2.2.1/mirp/_featuresets/ngldm.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_featuresets/ngtdm.py` & `mirp-2.2.1/mirp/_featuresets/ngtdm.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_featuresets/rlm.py` & `mirp-2.2.1/mirp/_featuresets/rlm.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_featuresets/statistics.py` & `mirp-2.2.1/mirp/_featuresets/statistics.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_featuresets/szm.py` & `mirp-2.2.1/mirp/_featuresets/szm.py`

 * *Files 18% similar despite different names*

```diff
@@ -203,69 +203,14 @@
 
         # Rename columns
         df_szm.columns = ["i", "s", "n"]
 
         # Add matrix to object
         self.matrix = df_szm
 
-    def calculate_matrix_deprecated(self, img_obj, roi_obj):
-
-        # Check if the input image and roi exist
-        if img_obj.is_missing or roi_obj.roi_intensity is None:
-            self.set_empty()
-            return
-
-        # Check if the roi contains any masked voxels. If this is not the case, don't construct the GLSZM.
-        if not np.any(roi_obj.roi_intensity.get_voxel_grid()):
-            self.set_empty()
-            return
-
-        from skimage.measure import label
-
-        # Define neighbour directions
-        if self.spatial_method == "3d":
-            connectivity = 3
-            img_vol = copy.deepcopy(img_obj.get_voxel_grid())
-            roi_vol = copy.deepcopy(roi_obj.roi_intensity.get_voxel_grid())
-        elif self.spatial_method in ["2d", "2.5d"]:
-            connectivity = 2
-            img_vol = img_obj.get_voxel_grid()[self.slice, :, :]
-            roi_vol = roi_obj.roi_intensity.get_voxel_grid()[self.slice, :, :]
-        else:
-            raise ValueError("The spatial method for grey level size zone matrices should be one of \"2d\", \"2.5d\" or \"3d\".")
-
-        # Check dimensionality and update connectivity if necessary.
-        connectivity = min([connectivity, real_ndim(img_vol)])
-
-        # Set voxels outside roi to 0.0
-        img_vol[~roi_vol] = 0.0
-
-        # Count the number of voxels within the roi
-        self.n_v = np.sum(roi_vol)
-
-        # Label all connected voxels with the same label.
-        img_label = label(img_vol, background=0, connectivity=connectivity)
-
-        # Generate data frame
-        df_szm = pd.DataFrame({"g":      np.ravel(img_vol),
-                               "vol_id": np.ravel(img_label),
-                               "in_roi": np.ravel(roi_vol)})
-
-        # Remove all non-roi entries and count occurrence of combinations of volume id and grey level
-        df_szm = df_szm[df_szm.in_roi].groupby(by=["g", "vol_id"]).size().reset_index(name="zone_size")
-
-        # Count the number of co-occurring sizes and grey values
-        df_szm = df_szm.groupby(by=["g", "zone_size"]).size().reset_index(name="n")
-
-        # Rename columns
-        df_szm.columns = ["i", "s", "n"]
-
-        # Add matrix to object
-        self.matrix = df_szm
-
     def compute_features(self):
 
         # Create feature table
         feat_names = [
             "szm_sze", "szm_lze", "szm_lgze", "szm_hgze", "szm_szlge", "szm_szhge", "szm_lzlge", "szm_lzhge",
             "szm_glnu", "szm_glnu_norm", "szm_zsnu", "szm_zsnu_norm", "szm_z_perc",
             "szm_gl_var", "szm_zs_var", "szm_zs_entr"
```

### Comparing `mirp-2.2.0/mirp/_featuresets/utilities.py` & `mirp-2.2.1/mirp/_featuresets/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_image_processing/alter_mask.py` & `mirp-2.2.1/mirp/_image_processing/alter_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_image_processing/anti_aliasing.py` & `mirp-2.2.1/mirp/_image_processing/anti_aliasing.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_image_processing/cropping.py` & `mirp-2.2.1/mirp/_image_processing/cropping.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_image_processing/discretise_image.py` & `mirp-2.2.1/mirp/_image_processing/discretise_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_image_processing/randomise_mask.py` & `mirp-2.2.1/mirp/_image_processing/randomise_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_image_processing/split_mask.py` & `mirp-2.2.1/mirp/_image_processing/split_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_image_processing/tissue_mask.py` & `mirp-2.2.1/mirp/_image_processing/tissue_mask.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_image_processing/utilities.py` & `mirp-2.2.1/mirp/_image_processing/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/exponential_transform.py` & `mirp-2.2.1/mirp/_imagefilters/exponential_transform.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/gabor.py` & `mirp-2.2.1/mirp/_imagefilters/gabor.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/gaussian.py` & `mirp-2.2.1/mirp/_imagefilters/gaussian.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         return response_map
 
     def transform_grid(self,
                        voxel_grid: np.array,
                        sigma: np.array):
         # Determine the size of the filter
         filter_size = 1 + 2 * np.floor(self.sigma_cutoff * sigma + 0.5)
-        filter_size.astype(np.int)
+        filter_size.astype(int)
 
         if self.by_slice:
             # Set the number of dimensions.
             d = 2.0
 
             # Create the grid coordinates, with [0, 0, 0] in the center.
             y, x = np.mgrid[:filter_size[1], :filter_size[2]]
```

### Comparing `mirp-2.2.0/mirp/_imagefilters/generic.py` & `mirp-2.2.1/mirp/_imagefilters/generic.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/laplacian_of_gaussian.py` & `mirp-2.2.1/mirp/_imagefilters/laplacian_of_gaussian.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/laws.py` & `mirp-2.2.1/mirp/_imagefilters/laws.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/log_transform.py` & `mirp-2.2.1/mirp/_imagefilters/log_transform.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/mean.py` & `mirp-2.2.1/mirp/_imagefilters/mean.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/nonseparable_wavelet.py` & `mirp-2.2.1/mirp/_imagefilters/nonseparable_wavelet.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/separable_wavelet.py` & `mirp-2.2.1/mirp/_imagefilters/separable_wavelet.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/square_root_transform.py` & `mirp-2.2.1/mirp/_imagefilters/square_root_transform.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/square_transform.py` & `mirp-2.2.1/mirp/_imagefilters/square_transform.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_imagefilters/utilities.py` & `mirp-2.2.1/mirp/_imagefilters/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_images/base_image.py` & `mirp-2.2.1/mirp/_images/base_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.image_dimension = copy.deepcopy(image_dimensions)
 
         # Set sample name.
         self.sample_name = sample_name
 
     def is_isotropic(self, by_slice: bool) -> bool:
         if by_slice:
-            spacing = np.array(self.image_spacing)[1, 2]
+            spacing = np.array(self.image_spacing)[[1, 2]]
         else:
             spacing = np.array(self.image_spacing)
 
         return np.all(spacing == spacing[0])
 
     def world_coordinates(self):
```

### Comparing `mirp-2.2.0/mirp/_images/ct_image.py` & `mirp-2.2.1/mirp/_images/ct_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_images/generic_image.py` & `mirp-2.2.1/mirp/_images/generic_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
 import hashlib
 import sys
 import numpy as np
 import pandas as pd
 
 from typing import Any
+from pathlib import Path
+
 from mirp._images.base_image import BaseImage
 from mirp.settings.generic import SettingsClass
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
@@ -167,15 +169,15 @@
 
     def get_voxel_grid(self) -> None | np.ndarray:
         return self.image_data
 
     def update_image_data(self):
         pass
 
-    def show(self, mask=None):
+    def show(self, mask=None, slice_id=None):  # pragma: no cover
         import matplotlib.pyplot as plt
         from mirp._images.utilities import InteractivePlot
 
         if self.is_empty():
             return
 
         if mask is not None:
@@ -184,24 +186,21 @@
             mask.register(
                 image=self,
                 spline_order=1,
                 anti_aliasing=False,
                 anti_aliasing_smoothing_beta=0.98
             )
 
-        figure, axes = plt.subplots()
-
         # Create an index tracked object
         tracker = InteractivePlot(
-            axes=axes,
             image=self,
-            mask=mask
+            mask=mask,
+            slice_id=slice_id
         )
 
-        figure.canvas.mpl_connect('scroll_event', tracker.onscroll)
         plt.show()
 
     @staticmethod
     def get_colour_map():
         return "gist_gray"
 
     @staticmethod
@@ -634,23 +633,22 @@
 
             # Step 3: calculate median noise - this differs from the original
             # Set local variances below 0 (due to floating point rounding) to 0.
             local_variance = np.ravel(local_variance)
             local_variance[local_variance < 0.0] = 0.0
 
             # Select robust range (within IQR)
-            local_variance = local_variance[
-                np.percentile(local_variance, 25) <= local_variance <= np.percentile(local_variance, 75)
-            ]
+            local_variance = local_variance[np.logical_and(
+                local_variance >= np.percentile(local_variance, 25),
+                local_variance <= np.percentile(local_variance, 75)
+            )]
 
             # Calculate Gaussian noise
             estimated_noise = np.sqrt(np.mean(local_variance))
 
-            del local_variance
-
         elif method == "ikeda":
             """ Estimate image noise level using a method by Ikeda, Makino, Imai et al., A method for estimating noise
              variance of CT image, Comp Med Imaging Graph (2010) 34:642-650"""
 
             # Step 1: filter with a cascading difference filter to suppress original image volume
             diff_filter = np.array([-1.0 / np.sqrt(2.0), 1.0 / np.sqrt(2.0)])
 
@@ -1153,15 +1151,15 @@
 
     def bias_field_correction(self, in_place=True, **kwargs):
         if not in_place:
             return self.copy()
 
     def write(
             self,
-            dir_path: str,
+            dir_path: str | Path,
             file_name: None | str = None,
             file_format: str = "nifti"
     ):
         """ Writes the image to a file """
         import os
         import itk
 
@@ -1204,14 +1202,19 @@
 
             itk.imwrite(image_data, file_path)
 
         elif file_format == "numpy":
             image_data = self.get_voxel_grid()
             np.save(file_path, image_data)
 
+        else:
+            raise ValueError(
+                f"file format was not recognised: {file_format}. MIRP currently supports nifti and numpy are supported."
+            )
+
     def get_file_name_descriptor(self) -> list[str]:
         descriptors = []
 
         # Sample name
         if self.sample_name is not None:
             descriptors += [self.sample_name]
```

### Comparing `mirp-2.2.0/mirp/_images/mask_image.py` & `mirp-2.2.1/mirp/_images/mask_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         if not self.is_isotropic(by_slice=by_slice):
             warnings.warn(
                 "Non-uniform voxel spacing was detected. Mask dilation requires uniform voxel spacing.", UserWarning
             )
 
         # Set spacing
         if by_slice:
-            spacing = np.array(self.image_spacing)[1, 2]
+            spacing = np.array(self.image_spacing)[[1, 2]]
         else:
             spacing = np.array(self.image_spacing)
 
         # Derive filter extension and distance
         if distance is not None:
             base_ext: int = np.max([np.floor(distance / np.max(spacing)).astype(int), 0])
         else:
@@ -287,15 +287,15 @@
         if not self.is_isotropic(by_slice=by_slice):
             warnings.warn(
                 "Non-uniform voxel spacing was detected. Mask erosion requires uniform voxel spacing.", UserWarning
             )
 
         # Set spacing.
         if by_slice:
-            spacing = np.array(self.image_spacing)[1, 2]
+            spacing = np.array(self.image_spacing)[[1, 2]]
         else:
             spacing = np.array(self.image_spacing)
 
         # Set geometrical structure. For 2D, the structures in different slices are set to 0.
         geom_struct = ndi.generate_binary_structure(3, 1)
         if by_slice:
             geom_struct[(0, 2), :, :] = False
```

### Comparing `mirp-2.2.0/mirp/_images/mr_image.py` & `mirp-2.2.1/mirp/_images/mr_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         threader.SetGlobalDefaultNumberOfThreads(1)
 
         # Start N4 bias correction
         corrector = itk.N4BiasFieldCorrectionImageFilter.New(input_image, input_mask)
         corrector.SetNumberOfFittingLevels(n_fitting_levels)
         corrector.SetMaximumNumberOfIterations(n_max_iterations)
         corrector.SetConvergenceThreshold(convergence_threshold)
+        corrector.Update()
         output_image = corrector.GetOutput()
 
         # Save bias-corrected image.
         if not in_place:
             image = self.copy(drop_image=True)
             image.set_voxel_grid(voxel_grid=itk.GetArrayFromImage(output_image).astype(float))
             return image
```

### Comparing `mirp-2.2.0/mirp/_images/pet_image.py` & `mirp-2.2.1/mirp/_images/pet_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_images/rtdose_image.py` & `mirp-2.2.1/mirp/_images/rtdose_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_images/transformed_image.py` & `mirp-2.2.1/mirp/_images/transformed_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/_images/utilities.py` & `mirp-2.2.1/mirp/_images/utilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,40 +3,51 @@
 from matplotlib.colors import LinearSegmentedColormap
 
 from mirp._images.generic_image import GenericImage
 from mirp._images.mask_image import MaskImage
 from mirp._masks.base_mask import BaseMask
 
 
-class InteractivePlot:
+class InteractivePlot:  # pragma: no cover
 
     def __init__(
             self,
-            axes: plt.Axes,
             image: GenericImage,
-            mask: MaskImage | BaseMask | None = None
+            mask: MaskImage | BaseMask | None = None,
+            slice_id: int | None = None
     ):
 
         # Determine if a mask should be shown.
         show_mask = mask is not None and not mask.is_empty()
 
         if show_mask and isinstance(mask, BaseMask):
             mask = mask.roi
         if show_mask:
             show_mask = not mask.is_empty_mask()
 
+        # Generate figure
+        figure, axes = plt.subplots()
         self.axes = axes
+        self.figure = figure
+
+        # Attach connections
+        self.scroll_cid = self.figure.canvas.mpl_connect("scroll_event", self.onscroll)
+        self.close_cid = self.figure.canvas.mpl_connect("close_event", self.disconnect)
+
         self.image_data = image.get_voxel_grid()
 
         self.mask_data = None
         if show_mask:
             self.mask_data = mask.get_voxel_grid()
 
         self.n_slices, _, _ = image.image_dimension
-        self.slice_index = int(np.floor(self.n_slices / 2.0))
+        if slice_id is None or slice_id < 1 or slice_id > self.n_slices:
+            self.slice_index = int(np.floor(self.n_slices / 2.0))
+        else:
+            self.slice_index = slice_id - 1
 
         # Set plotting options
         colour_map = image.get_colour_map()
         min_intensity = image.get_default_lowest_intensity() if image.get_default_lowest_intensity() is not None else (
             np.min(self.image_data))
         max_intensity = image.get_default_upper_intensity() if image.get_default_upper_intensity() is not None else (
             np.max(self.image_data))
@@ -95,7 +106,11 @@
         self.axes.set_title(f"slice {self.slice_index + 1}")
         self.image_layer.set_data(self.image_data[self.slice_index, :, :])
         self.image_layer.axes.figure.canvas.draw()
 
         if self.mask_layer is not None:
             self.mask_layer.set_data(self.mask_data[self.slice_index, :, :])
             self.mask_layer.axes.figure.canvas.draw()
+
+    def disconnect(self):
+        self.figure.canvas.mpl_disconnect(self.scroll_cid)
+        self.figure.canvas.mpl_disconnect(self.close_cid)
```

### Comparing `mirp-2.2.0/mirp/_masks/base_mask.py` & `mirp-2.2.1/mirp/_masks/base_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 import copy
 import sys
 from typing import Any
+from pathlib import Path
 
 from mirp._images.generic_image import GenericImage
 from mirp._images.mask_image import MaskImage
 from mirp.settings.generic import SettingsClass
 
 if sys.version_info >= (3, 11):
     from typing import Self
@@ -52,16 +53,21 @@
             slice_number = [slice_number]
 
         for current_slice_id in slice_number:
             slice_mask = self.copy(drop_image=True)
             slice_mask.roi = self.roi.get_slices(slice_number=current_slice_id)
             if slice_mask.roi_intensity is not None and not primary_mask_only:
                 slice_mask.roi_intensity = self.roi_intensity.get_slices(slice_number=current_slice_id)
+            else:
+                slice_mask.roi_intensity = None
+
             if slice_mask.roi_morphology is not None and not primary_mask_only:
-                slice_mask.roi_intensity = self.roi_morphology.get_slices(slice_number=slice_number)
+                slice_mask.roi_morphology = self.roi_morphology.get_slices(slice_number=current_slice_id)
+            else:
+                slice_mask.roi_morphology = None
 
             if slice_mask.is_empty():
                 continue
 
             mask_list += [slice_mask]
 
         if len(mask_list) == 0:
@@ -91,25 +97,14 @@
             return True
 
         return self.roi.is_empty()
 
     def is_empty_mask(self):
         return self.roi.is_empty_mask()
 
-    def append_name(self, x):
-        if isinstance(self.roi_name, str):
-            self.roi_name = [self.roi_name]
-
-        if isinstance(x, str):
-            self.roi_name += [x]
-        elif isinstance(x, list):
-            self.roi_name += x
-        else:
-            raise TypeError("The x attribute is expected to be a string or list of strings.")
-
     def interpolate(
             self,
             image: None | GenericImage,
             settings: SettingsClass
     ):
         # Skip if image and/or mask is missing
         if self.is_empty():
@@ -576,15 +571,15 @@
     def get_bounding_box(self):
         return self.roi.get_bounding_box()
 
     def compute_diagnostic_features(
             self,
             image: GenericImage,
             settings: SettingsClass,
-            append_str: str = ""
+            append_str: str | None = None
     ) -> pd.DataFrame:
         """ Creates diagnostic features for the ROI """
 
         # Set feature names
         feature_names = [
             "int_map_dim_x", "int_map_dim_y", "int_map_dim_z", "int_bb_dim_x", "int_bb_dim_y", "int_bb_dim_z",
             "int_vox_dim_x", "int_vox_dim_y", "int_vox_dim_z", "int_vox_count", "int_mean_int", "int_min_int",
@@ -616,19 +611,19 @@
         img_voxel_grid = image.get_voxel_grid()
         int_voxel_grid = mask_copy.roi_intensity.get_voxel_grid()
         mrp_voxel_grid = mask_copy.roi_morphology.get_voxel_grid()
 
         # Compute bounding boxes
         int_bounding_box_dim = mask_copy.roi_intensity.get_bounding_box()
         mrp_bounding_box_dim = mask_copy.roi_morphology.get_bounding_box()
-        if any(x is None for x in int_bounding_box_dim) or (y is None for y in mrp_bounding_box_dim):
+        if any(x is None for x in int_bounding_box_dim) or any(y is None for y in mrp_bounding_box_dim):
             return df
 
-        int_bounding_box_dim = np.squeeze(np.diff(int_bounding_box_dim, axis=0) + 1)
-        mrp_bounding_box_dim = np.squeeze(np.diff(mrp_bounding_box_dim, axis=0) + 1)
+        int_bounding_box_dim = np.squeeze(np.diff(int_bounding_box_dim, axis=1) + 1)
+        mrp_bounding_box_dim = np.squeeze(np.diff(mrp_bounding_box_dim, axis=1) + 1)
 
         # Set intensity mask features
         df["int_map_dim_x"] = mask_copy.roi_intensity.image_dimension[2]
         df["int_map_dim_y"] = mask_copy.roi_intensity.image_dimension[1]
         df["int_map_dim_z"] = mask_copy.roi_intensity.image_dimension[0]
         df["int_bb_dim_x"] = int_bounding_box_dim[2]
         df["int_bb_dim_y"] = int_bounding_box_dim[1]
@@ -653,15 +648,18 @@
         df["mrp_vox_dim_z"] = mask_copy.roi_morphology.image_spacing[0]
         df["mrp_vox_count"] = np.sum(mrp_voxel_grid)
         df["mrp_mean_int"] = np.mean(img_voxel_grid[mrp_voxel_grid])
         df["mrp_min_int"] = np.min(img_voxel_grid[mrp_voxel_grid])
         df["mrp_max_int"] = np.max(img_voxel_grid[mrp_voxel_grid])
 
         # Update column names
-        df.columns = ["_".join(["diag", feature, append_str]).strip("_") for feature in df.columns]
+        if append_str is None:
+            df.columns = ["_".join(["diag", feature]) for feature in df.columns]
+        else:
+            df.columns = ["_".join(["diag", feature, append_str]) for feature in df.columns]
 
         del mask_copy
 
         return df
 
     def get_center_position(self) -> list[Any]:
         """Identify location of the geometric center of the roi."""
@@ -685,15 +683,15 @@
         z_ind, y_ind, x_ind = np.where(self.roi.get_voxel_grid())
         z_center = (np.max(z_ind) + np.min(z_ind)) // 2
 
         return z_center
 
     def write(
             self,
-            dir_path: str,
+            dir_path: str | Path,
             write_all: bool = False,
             file_format: str = "nifti"
     ):
         """
         Write masks to file
         :param dir_path: Path to directory where the image should be written.
         :param write_all: If true, creates NIfTI files from both intensity and morphology (original) masks.
```

### Comparing `mirp-2.2.0/mirp/_workflows/standardWorkflow.py` & `mirp-2.2.1/mirp/_workflows/standardWorkflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,19 @@
             format="%(levelname)s\t: %(processName)s \t %(asctime)s \t %(message)s",
             level=logging.INFO, stream=sys.stdout)
 
         # Notify
         logging.info(self._message_start())
 
         # Read image and masks.
-        image, masks = read_image_and_masks(self.image_file, to_numpy=False)
+        image, masks = read_image_and_masks(
+            self.image_file,
+            to_numpy=False,
+            pet_suv_conversion=self.settings.post_process.suv_conversion_type
+        )
 
         if masks is None or len(masks) == 0:
             warnings.warn("No segmentation masks were read.")
             return
 
         if any(not isinstance(mask, BaseMask) for mask in masks):
             object_types = list(set([str(type(mask)) for mask in masks if not isinstance(mask, BaseMask)]))
```

### Comparing `mirp-2.2.0/mirp/config_data.xml` & `mirp-2.2.1/mirp/config_data.xml`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/config_settings.xml` & `mirp-2.2.1/mirp/config_settings.xml`

 * *Files 1% similar despite different names*

#### Comparing `mirp-2.2.0/mirp/config_settings.xml` & `mirp-2.2.1/mirp/config_settings.xml`

```diff
@@ -58,14 +58,18 @@
       <!-- Number of fitting levels for N4 bias field correction. Default: 1 -->
       <n_fitting_levels/>
       <!-- Max number of iterations for each of the fitting levels for N4 bias field correction, e.g. 100, 100
             if two fitting levels are used. Default: 50 -->
       <n_max_iterations/>
       <!-- Convergence threshold for N4 bias field correction. Default: 0.001 -->
       <convergence_threshold/>
+      <!-- Intensities in PET imaging are often stored as detected radiotracer activity. To make detected activity more
+            comparable between patients, these are converted to standardised uptake values. The following are possible:
+            body_weight, none. -->
+      <pet_suv_conversion/>
       <!-- Algorithm used to normalise intensities in the image. Will use only intensities in voxels masked by
             the  tissue mask. Can be none (default), range (maps to an intensity range), relative_range (maps to a
             range  of relative intensities), quantile_range (maps to a range of relative intensities based on
             intensity percentiles), standardisation (performs z-normalisation). -->
       <intensity_normalisation/>
       <!-- Intensity range for range, relative_range and quantile_range normalisation. -->
       <intensity_normalisation_range/>
```

### Comparing `mirp-2.2.0/mirp/data_import/import_image.py` & `mirp-2.2.1/mirp/data_import/import_image.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/data_import/import_image_and_mask.py` & `mirp-2.2.1/mirp/data_import/import_image_and_mask.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from mirp.data_import.import_image import import_image
 from mirp.data_import.import_mask import import_mask
-from mirp._data_import.generic_file import ImageFile, MaskFile
+from mirp._data_import.generic_file import ImageFile, MaskFile, MaskFullImage
 from mirp._data_import.dicom_file import ImageDicomFile, MaskDicomFile
 from mirp._data_import.dicom_file_stack import ImageDicomFileStack
 from mirp.utilities.utilities import random_string
 
 
 def import_image_and_mask(
         image,
@@ -14,15 +14,15 @@
         image_file_type: None | str = None,
         image_modality: None | str | list[str] = None,
         image_sub_folder: None | str = None,
         mask_name: None | str | list[str] = None,
         mask_file_type: None | str = None,
         mask_modality: None | str | list[str] = None,
         mask_sub_folder: None | str = None,
-        roi_name: None | str | list[str] | dict[str | str] = None,
+        roi_name: None | str | list[str] | dict[str, str] = None,
         association_strategy: None | str | list[str] = None,
         stack_images: str = "auto",
         stack_masks: str = "auto"
 ) -> list[ImageFile]:
     """
     Creates and curates references to image and mask files. This function is usually called internally by other
     functions such as :func:`~mirp.extractFeaturesAndImages.extract_features`.
@@ -77,15 +77,15 @@
         Note that only DICOM files contain metadata concerning modality. Masks from non-DICOM files are considered to
         be "generic_mask".
 
     mask_sub_folder: str, optional, default: None
         Fixed directory substructure where mask files are located. If None, the directory substructure is not used for
         filtering files.
 
-    roi_name: str, optional, default: None
+    roi_name: str or list of str or dict, optional, default: None
         Name of the regions of interest that should be assessed.
 
     association_strategy: {"frame_of_reference", "sample_name", "file_distance", "file_name_similarity",  "list_order", "position", "single_image"}
         The preferred strategy for associating images and masks. File association is preferably done using frame of
         reference UIDs (DICOM), or sample name (NIfTI, numpy). Other options are relatively frail, except for
         `list_order` which may be applicable when a list with images and a list with masks is provided and both lists
         are of equal length.
@@ -105,101 +105,125 @@
         because their stacking can be determined from metadata.
 
     Returns
     -------
     list[ImageFile]
         The functions returns a list of ImageFile objects, if any were found with the specified filters.
     """
-    if mask is None:
+
+    # If mask = None, this can mean several things. Here we check that mask should not be interpreted as having the
+    # same meaning as image.
+    if mask is None and (
+            mask_name is not None or mask_sub_folder is not None or mask_modality is not None or
+            mask_file_type is not None or roi_name is not None
+    ):
+        mask = image
+
+    elif mask is None and isinstance(image, str) and image.endswith(".xml"):
         mask = image
 
     # Generate list of images.
     image_list = import_image(
         image,
         sample_name=sample_name,
         image_name=image_name,
         image_file_type=image_file_type,
         image_modality=image_modality,
         image_sub_folder=image_sub_folder,
         stack_images=stack_images
     )
 
-    # Generate list of images.
-    mask_list = import_mask(
-        mask,
-        sample_name=sample_name,
-        mask_name=mask_name,
-        mask_file_type=mask_file_type,
-        mask_modality=mask_modality,
-        mask_sub_folder=mask_sub_folder,
-        stack_masks=stack_masks,
-        roi_name=roi_name
-    )
-
     if len(image_list) == 0:
         raise ValueError(f"No images were found. Possible reasons are lack of images with the preferred modality.")
-    if len(mask_list) == 0:
-        raise ValueError(f"No masks were found. Possible reasons are lack of masks with the preferred modality.")
-
-    # Determine association strategy, if this is unset.
-    possible_association_strategy = set_association_strategy(
-        image_list=image_list,
-        mask_list=mask_list
-    )
 
-    if association_strategy is None:
-        association_strategy = possible_association_strategy
-    elif isinstance(association_strategy, str):
-        association_strategy = [association_strategy]
-
-    if not isinstance(association_strategy, set):
-        association_strategy = set(association_strategy)
-
-    # Test association strategy.
-    unavailable_strategy = association_strategy - possible_association_strategy
-    if len(unavailable_strategy) > 0:
-        raise ValueError(
-            f"One or more strategies for associating images and masks are not available for the provided image and "
-            f"mask set: {', '.join(list(unavailable_strategy))}. Only the following strategies are available: "
-            f"{'. '.join(list(possible_association_strategy))}"
+    # Remove metadata (if any) - anything relevant can be loaded later.
+    for image in image_list:
+        image.remove_metadata()
+
+    if mask is not None:
+        # Generate list of masks from mask.
+        mask_list = import_mask(
+            mask,
+            sample_name=sample_name,
+            mask_name=mask_name,
+            mask_file_type=mask_file_type,
+            mask_modality=mask_modality,
+            mask_sub_folder=mask_sub_folder,
+            stack_masks=stack_masks,
+            roi_name=roi_name
         )
 
-    if len(possible_association_strategy) == 0:
-        raise ValueError(
-            f"No strategies for associating images and masks are available, indicating that there is no clear way to "
-            f"establish an association."
-        )
+        if len(mask_list) == 0:
+            raise ValueError(f"No masks were found. Possible reasons are lack of masks with the preferred modality.")
 
-    # Start association.
-    if association_strategy == {"list_order"}:
-        # If only the list_order strategy is available, use this.
-        for ii, image in enumerate(image_list):
-            image.associated_masks = [mask_list[ii]]
+        # Remove metadata (if any) - anything relevant can be loaded later.
+        for mask in mask_list:
+            mask.remove_metadata()
+
+        # Determine association strategy, if this is unset.
+        possible_association_strategy = set_association_strategy(
+            image_list=image_list,
+            mask_list=mask_list
+        )
 
-    elif association_strategy == {"single_image"}:
-        # If single_image is the only strategy, use this.
-        image_list[0].associated_masks = mask_list
+        if association_strategy is None:
+            association_strategy = possible_association_strategy
+        elif isinstance(association_strategy, str):
+            association_strategy = [association_strategy]
+
+        if not isinstance(association_strategy, set):
+            association_strategy = set(association_strategy)
+
+        # Test association strategy.
+        unavailable_strategy = association_strategy - possible_association_strategy
+        if len(unavailable_strategy) > 0:
+            raise ValueError(
+                f"One or more strategies for associating images and masks are not available for the provided image and "
+                f"mask set: {', '.join(list(unavailable_strategy))}. Only the following strategies are available: "
+                f"{'. '.join(list(possible_association_strategy))}"
+            )
 
-    else:
-        for ii, image in enumerate(image_list):
-            image.associate_with_mask(
-                mask_list=mask_list,
-                association_strategy=association_strategy
+        if len(possible_association_strategy) == 0:
+            raise ValueError(
+                f"No strategies for associating images and masks are available, indicating that there is no clear way to "
+                f"establish an association."
             )
 
-        if all(image.associated_masks is None for image in image_list):
-            if "single_image" in association_strategy:
-                image_list[0].associated_masks = mask_list
-            elif "list_order" in association_strategy:
-                for ii, image in enumerate(image_list):
-                    image.associated_masks = [mask_list[ii]]
-
-    # Ensure that we are working with deep copies from this point - we don't want to propagate changes to masks,
-    # images by reference.
-    image_list = [image.copy() for image in image_list]
+        # Start association.
+        if association_strategy == {"list_order"}:
+            # If only the list_order strategy is available, use this.
+            for ii, image in enumerate(image_list):
+                image.associated_masks = [mask_list[ii]]
+
+        elif association_strategy == {"single_image"}:
+            # If single_image is the only strategy, use this.
+            image_list[0].associated_masks = mask_list
+
+        else:
+            for ii, image in enumerate(image_list):
+                image.associate_with_mask(
+                    mask_list=mask_list,
+                    association_strategy=association_strategy
+                )
+
+            if all(image.associated_masks is None for image in image_list):
+                if "single_image" in association_strategy:
+                    image_list[0].associated_masks = mask_list
+                elif "list_order" in association_strategy:
+                    for ii, image in enumerate(image_list):
+                        image.associated_masks = [mask_list[ii]]
+
+    else:
+        # Generate full masks.
+        for image in image_list:
+            image.associated_masks = [MaskFullImage()]
+
+    # In case we are not working with file-based images, ensure that we are working with deep copies from this point -
+    # we don't want to propagate changes to masks and images by reference.
+    image_list = [image if image.on_file_system() else image.copy() for image in image_list]
 
     # Set sample names. First we check if all sample names are missing.
     if all(image.sample_name is None for image in image_list):
         if isinstance(sample_name, str):
             sample_name = [sample_name]
 
         if isinstance(sample_name, list) and len(sample_name) == len(image_list):
@@ -207,19 +231,20 @@
                 image.set_sample_name(sample_name=sample_name[ii])
                 if image.associated_masks is not None:
                     for mask in image.associated_masks:
                         mask.set_sample_name(sample_name=sample_name[ii])
 
         elif all(image.file_name is not None for image in image_list):
             for image in image_list:
-                image.set_sample_name(sample_name=image.file_name)
+                file_sample_name = image.get_sample_name_from_file(must_succeed=True)
+                image.set_sample_name(sample_name=file_sample_name)
 
                 if image.associated_masks is not None:
                     for mask in image.associated_masks:
-                        mask.set_sample_name(sample_name=image.file_name)
+                        mask.set_sample_name(sample_name=file_sample_name)
 
     # Then set any sample names for images that still miss them.
     if any(image.sample_name is None for image in image_list):
         for ii, image in enumerate(image_list):
             if image.sample_name is None:
                 generated_sample_name = str(ii + 1) + "_" + random_string(16)
                 image.set_sample_name(sample_name=generated_sample_name)
```

### Comparing `mirp-2.2.0/mirp/data_import/import_mask.py` & `mirp-2.2.1/mirp/data_import/import_mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         Note that only DICOM files contain metadata concerning modality. Masks from non-DICOM files are considered to
         be "generic_mask".
 
     mask_sub_folder: str, optional, default: None
         Fixed directory substructure where mask files are located. If None, the directory substructure is not used for
         filtering files.
 
-    roi_name: str, optional, default: None
+    roi_name: str or list of str or dict, optional, default: None
         Name of the regions of interest that should be assessed.
 
     stack_masks: {"auto", "yes", "no"}, optional, default: "str"
         If mask files in the same directory cannot be assigned to different samples, and are 2D (slices) of the same
         size, they might belong to the same 3D mask stack. "auto" will stack 2D numpy arrays, but not other file
         types. "yes" will stack all files that contain 2D images, that have the same dimensions, orientation and
         spacing, except for DICOM files. "no" will not stack any files. DICOM files ignore this argument,
```

### Comparing `mirp-2.2.0/mirp/deep_learning_preprocessing.py` & `mirp-2.2.1/mirp/deep_learning_preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Generator, Iterable, Any
 import copy
-import ray
 
 from mirp._data_import.generic_file import ImageFile
 from mirp.settings.generic import SettingsClass
+from mirp.utilities.parallel import ray_remote, ray_init, ray_is_initialized, ray_get, ray_shutdown
 from mirp._workflows.standardWorkflow import StandardWorkflow
 
 
 def deep_learning_preprocessing(
         output_slices: bool = False,
         crop_size: None | list[float] | list[int] = None,
-        image_export_format: str = "numpy",
+        image_export_format: str = "dict",
         write_file_format: str = "numpy",
         export_images: None | bool = None,
         write_images: None | bool = None,
         write_dir: None | str = None,
         num_cpus: None | int = None,
         **kwargs
 ) -> None | list[Any]:
@@ -30,15 +30,15 @@
         Size to which the images and masks should be cropped. Images and masks are cropped around the center of the
         mask(s).
 
         .. note::
             MIRP follows the numpy convention for indexing (*z*, *y*, *x*). The final element always corresponds to the
             *x* dimension.
 
-    image_export_format: {"dict", "native", "numpy"}, default: "numpy"
+    image_export_format: {"dict", "native", "numpy"}, default: "dict"
         Return format for processed images and masks. ``"dict"`` returns dictionaries of images and masks as numpy
         arrays and associated characteristics. ``"native"`` returns images and masks in their internal format.
         ``"numpy"`` returns images and masks in numpy format. This argument is only used if ``export_images=True``.
 
     write_file_format: {"nifti", "numpy"}, default: "numpy"
         File format for processed images and masks. ``"nifti"`` writes images and masks in the NIfTI file format,
         and ``"numpy"`` writes images and masks as numpy files. This argument is only used if ``write_images=True``.
@@ -80,19 +80,19 @@
     * image interpolation / resampling (:class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass` and
       :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`)
     * mask resegmentation (:class:`~mirp.settings.resegmentation_parameters.ResegmentationSettingsClass`)
 
     """
 
     # Conditionally start a ray cluster.
-    external_ray = ray.is_initialized()
+    external_ray = ray_is_initialized()
     if not external_ray and num_cpus is not None and num_cpus > 1:
-        ray.init(num_cpus=num_cpus)
+        ray_init(num_cpus=num_cpus)
 
-    if ray.is_initialized():
+    if ray_is_initialized():
         # Parallel processing.
         results = [
             _ray_extractor.remote(
                 workflow=workflow,
                 output_slices=output_slices,
                 crop_size=crop_size,
                 image_export_format=image_export_format,
@@ -102,17 +102,17 @@
                 export_images=export_images,
                 write_images=write_images,
                 write_dir=write_dir,
                 **kwargs
             )
         ]
 
-        results = ray.get(results)
+        results = ray_get(results)
         if not external_ray:
-            ray.shutdown()
+            ray_shutdown()
     else:
         workflows = list(_base_deep_learning_preprocessing(
             export_images=export_images,
             write_images=write_images,
             write_dir=write_dir,
             **kwargs)
         )
@@ -126,15 +126,15 @@
             )
             for workflow in workflows
         ]
 
     return results
 
 
-@ray.remote
+@ray_remote
 def _ray_extractor(
         workflow: StandardWorkflow,
         output_slices: bool = False,
         crop_size: None | list[float] | list[int] = None,
         image_export_format: str = "numpy",
         write_file_format: str = "numpy"
 ):
@@ -149,15 +149,15 @@
         write_file_format=write_file_format
     )
 
 
 def deep_learning_preprocessing_generator(
         output_slices: bool = False,
         crop_size: None | list[float] | list[int] = None,
-        image_export_format: str = "numpy",
+        image_export_format: str = "dict",
         write_file_format: str = "numpy",
         export_images: None | bool = None,
         write_images: None | bool = None,
         write_dir: None | str = None,
         **kwargs
 ) -> Generator[Any, None, None]:
     """
@@ -172,15 +172,15 @@
         Size to which the images and masks should be cropped. Images and masks are cropped around the center of the
         mask(s).
 
         .. note::
             MIRP follows the numpy convention for indexing (*z*, *y*, *x*). The final element always corresponds to the
             *x* dimension.
 
-    image_export_format: {"dict", "native", "numpy"}, default: "numpy"
+    image_export_format: {"dict", "native", "numpy"}, default: "dict"
         Return format for processed images and masks. ``"dict"`` returns dictionaries of images and masks as numpy
         arrays and associated characteristics. ``"native"`` returns images and masks in their internal format.
         ``"numpy"`` returns images and masks in numpy format. This argument is only used if ``export_images=True``.
 
     write_file_format: {"nifti", "numpy"}, default: "numpy"
         File format for processed images and masks. ``"nifti"`` writes images and masks in the NIfTI file format,
         and ``"numpy"`` writes images and masks as numpy files. This argument is only used if ``write_images=True``.
```

### Comparing `mirp-2.2.0/mirp/deprecated.py` & `mirp-2.2.1/mirp/deprecated.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 def get_roi_labels(**kwargs):
     raise RuntimeError(
         f"The get_roi_labels function has been replaced by "
-        f"mirp.extractMaskLabels.extract_mask_labels."
+        f"mirp.extract_mask_labels."
     )
 
 
 def get_image_acquisition_parameters(**kwargs):
     raise RuntimeError(
         f"The get_image_acquisition_parameters function has been replaced by "
-        f"mirp.extractImageParameters.extract_image_parameters."
+        f"mirp.extract_image_parameters."
     )
 
 
 def get_file_structure_parameters(**kwargs):
     raise RuntimeError(
         f"The get_file_structure_parameters function has been fully deprecated, without replacement."
     )
@@ -23,27 +23,27 @@
         f"The parse_file_structure function has been fully deprecated, without replacement."
     )
 
 
 def extract_images_for_deep_learning(**kwargs):
     raise RuntimeError(
         f"The extract_images_for_deep_learning function has been replaced by "
-        f"mirp.deepLearningPreprocessing.deep_learning_preprocessing."
+        f"mirp.deep_learning_preprocessing."
     )
 
 
 def extract_features(**kwargs):
     raise RuntimeError(
-        f"The extract_features function has been replaced by mirp.extractFeaturesAndImage.extract_features."
+        f"The extract_features function has been replaced by mirp.extract_features."
     )
 
 
 def extract_images_to_nifti(**kwargs):
     raise RuntimeError(
-        f"The extract_images_to_nifti function has been replaced by mirp.extractFeaturesAndImage.extract_images."
+        f"The extract_images_to_nifti function has been replaced by mirp.extract_images."
     )
 
 
 def process_images(**kwargs):
     raise RuntimeError(
-        "The process_images function has been replaced by mirp.extractFeaturesAndImage.extract_features_and_images."
+        "The process_images function has been replaced by mirp.extract_features_and_images."
     )
```

### Comparing `mirp-2.2.0/mirp/extract_features_and_images.py` & `mirp-2.2.1/mirp/extract_features_and_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Generator, Iterable, Any
 import copy
 
-import ray
-
 from mirp._data_import.generic_file import ImageFile
 from mirp.settings.generic import SettingsClass
+from mirp.utilities.parallel import ray_remote, ray_init, ray_is_initialized, ray_get, ray_shutdown
 from mirp._workflows.standardWorkflow import StandardWorkflow
 
 
 def extract_features(
         write_features: None | bool = None,
         export_features: None | bool = None,
         write_dir: None | str = None,
@@ -91,16 +90,16 @@
         write_images=False,
         export_images=False,
         **kwargs
     )
 
 
 def extract_images(
-        write_images: None | bool = True,
-        export_images: None | bool = False,
+        write_images: None | bool = None,
+        export_images: None | bool = None,
         write_dir: None | str = None,
         **kwargs
 ):
     """
     Process images and masks. This function is a wrapper around
     :func:`~mirp.extractFeaturesAndImages.extract_features_and_images`.
 
@@ -186,15 +185,15 @@
         **kwargs
 ):
     """
     Processes images and computes features from regions of interest.
 
     Parameters
     ----------
-    image_export_format: {"dict", "native", "numpy"}, default: "numpy"
+    image_export_format: {"dict", "native", "numpy"}, default: "dict"
         Return format for processed images and masks. ``"dict"`` returns dictionaries of images and masks as numpy
         arrays and associated characteristics. ``"native"`` returns images and masks in their internal format.
         ``"numpy"`` returns images and masks in numpy format. This argument is only used if ``export_images=True``.
 
     num_cpus: int, optional, default: None
         Number of CPU nodes that should be used for parallel processing. Image processing and feature computation can be
         parallelized using the ``ray`` package. If a ray cluster is defined by the user, this cluster will be used
@@ -233,28 +232,28 @@
     * mask resegmentation (:class:`~mirp.settings.resegmentation_parameters.ResegmentationSettingsClass`)
     * image transformation (:class:`~mirp.settings.transformation_parameters.ImageTransformationSettingsClass`)
     * feature computation / extraction (:class:`~mirp.settings.feature_parameters.FeatureExtractionSettingsClass`)
 
     """
 
     # Conditionally start a ray cluster.
-    external_ray = ray.is_initialized()
+    external_ray = ray_is_initialized()
     if not external_ray and num_cpus is not None and num_cpus > 1:
-        ray.init(num_cpus=num_cpus)
+        ray_init(num_cpus=num_cpus)
 
-    if ray.is_initialized():
+    if ray_is_initialized():
         # Parallel processing.
         results = [
             _ray_extractor.remote(workflow=workflow, image_export_format=image_export_format)
             for workflow in _base_extract_features_and_images(**kwargs)
         ]
 
-        results = ray.get(results)
+        results = ray_get(results)
         if not external_ray:
-            ray.shutdown()
+            ray_shutdown()
 
     else:
         # Sequential processing.
         workflows = list(_base_extract_features_and_images(**kwargs))
         results = [workflow.standard_extraction(image_export_format=image_export_format) for workflow in workflows]
 
     return results
@@ -311,15 +310,15 @@
     """
 
     workflows = list(_base_extract_features_and_images(**kwargs))
     for workflow in workflows:
         yield workflow.standard_extraction(image_export_format=image_export_format)
 
 
-@ray.remote
+@ray_remote
 def _ray_extractor(workflow: StandardWorkflow, image_export_format="dict"):
     # Limit internal threading by third-party libraries.
     from mirp.utilities.parallel import limit_inner_threads
     limit_inner_threads()
 
     return workflow.standard_extraction(image_export_format=image_export_format)
```

### Comparing `mirp-2.2.0/mirp/extract_image_parameters.py` & `mirp-2.2.1/mirp/extract_image_parameters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import pandas as pd
+from pathlib import Path
 
 from mirp._data_import.generic_file import ImageFile
 
 
 def extract_image_parameters(
         image,
         sample_name: None | str | list[str] = None,
         image_name: None | str | list[str] = None,
         image_file_type: None | str = None,
         image_modality: None | str | list[str] = None,
         image_sub_folder: None | str = None,
         stack_images: str = "auto",
-        write_file: bool = False,
-        write_dir: None | str = None
+        write_dir: None | str | Path = None
 ) -> pd.DataFrame | None:
     """
     Extract parameters related to image acquisition and reconstruction from images. Not all metadata may
     be available.
 
     Parameters
     ----------
@@ -52,54 +52,46 @@
     stack_images: {"auto", "yes", "no"}, optional, default: "str"
         If image files in the same directory cannot be assigned to different samples, and are 2D (slices) of the same
         size, they might belong to the same 3D image stack. "auto" will stack 2D numpy arrays, but not other file types.
         "yes" will stack all files that contain 2D images, that have the same dimensions, orientation and spacing,
         except for DICOM files. "no" will not stack any files. DICOM files ignore this argument, because their stacking
         can be determined from metadata.
 
-    write_file: bool, optional, default: False
-        Determines whether image acquisition and reconstruction metadata should be written to a table.
-
-    write_dir: str, optional, default: None
-        Folder to which the table with image acquisition and reconstruction metadata is written.
+    write_dir: str or Path, optional, default: None
+        Directory to which the table with image acquisition and reconstruction metadata is written. Image metadata are
+        written to ``image_metadata.csv`` in this directory.
 
     Returns
     -------
     pd.DataFrame | None
-        The functions returns a table with metadata (`write_file == False`) or nothing (`write_file == True`)
+        The functions returns a table with metadata (``write_dir = None``) or nothing.
     """
 
     from mirp.data_import.import_image import import_image
 
-    if not write_file:
-        write_dir = None
-
-    if write_file and write_dir is None:
-        raise ValueError("write_dir argument should be provided for writing a table with image metadata.")
-
     image_list = import_image(
         image=image,
         sample_name=sample_name,
         image_name=image_name,
         image_file_type=image_file_type,
         image_modality=image_modality,
         image_sub_folder=image_sub_folder,
         stack_images=stack_images
     )
 
     metadata = [_extract_image_parameters(ii, image) for ii, image in enumerate(image_list)]
     metadata = pd.DataFrame(metadata)
 
-    if write_file:
+    if write_dir is not None:
         write_dir = os.path.normpath(write_dir)
         if not os.path.exists(write_dir):
             os.makedirs(write_dir)
 
         metadata.to_csv(
-            path_or_buf=os.path.join(write_dir, "mask_labels.csv")
+            path_or_buf=os.path.join(write_dir, "image_metadata.csv")
         )
     else:
         return metadata
 
 
 def _extract_image_parameters(index: int, image: ImageFile) -> dict[str, str]:
```

### Comparing `mirp-2.2.0/mirp/extract_mask_labels.py` & `mirp-2.2.1/mirp/extract_mask_labels.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any
+from pathlib import Path
 
 import os
 import pandas as pd
 
 from mirp._data_import.generic_file import MaskFile
 
 
@@ -10,16 +11,15 @@
         mask=None,
         sample_name: None | str | list[str] = None,
         mask_name: None | str | list[str] = None,
         mask_file_type: None | str = None,
         mask_modality: None | str | list[str] = None,
         mask_sub_folder: None | str = None,
         stack_masks: str = "auto",
-        write_file: bool = False,
-        write_dir: None | str = None
+        write_dir: None | str | Path = None
 ) -> pd.DataFrame | None:
     """
     Extract labels of regions of interest present in one or more mask files.
 
     Parameters
     ----------
     mask: Any
@@ -53,49 +53,40 @@
     stack_masks: {"auto", "yes", "no"}, optional, default: "str"
         If mask files in the same directory cannot be assigned to different samples, and are 2D (slices) of the same
         size, they might belong to the same 3D mask stack. "auto" will stack 2D numpy arrays, but not other file
         types. "yes" will stack all files that contain 2D images, that have the same dimensions, orientation and
         spacing, except for DICOM files. "no" will not stack any files. DICOM files ignore this argument,
         because their stacking can be determined from metadata.
 
-    write_file: bool, optional, default: False
-        Determines whether the labels should be written to a table.
-
     write_dir: str, optional, default: None
-        Folder to which a table with mask labels should be written.
+        Directory to which a table with mask labels should be written, if any. Masks labels are exported to
+        ``mask_labels.csv``.
 
     Returns
     -------
     pd.DataFrame | None
-        The functions returns a table with labels extracted from mask files (`write_file == False`),
-        or None `(write_file == True)`.
+        The functions returns a table with labels extracted from mask files (``write_dir = None``) or nothing.
 
     """
     from mirp.data_import.import_mask import import_mask
 
-    if not write_file:
-        write_dir = None
-
-    if write_file and write_dir is None:
-        raise ValueError("write_dir argument should be provided for writing a table with mask labels.")
-
     mask_list = import_mask(
         mask=mask,
         sample_name=sample_name,
         mask_name=mask_name,
         mask_file_type=mask_file_type,
         mask_modality=mask_modality,
         mask_sub_folder=mask_sub_folder,
         stack_masks=stack_masks
     )
 
     labels = [pd.DataFrame(_extract_mask_labels(ii, mask)) for ii, mask in enumerate(mask_list)]
     labels = pd.concat(labels)
 
-    if write_file:
+    if write_dir is not None:
         write_dir = os.path.normpath(write_dir)
         if not os.path.exists(write_dir):
             os.makedirs(write_dir)
 
         labels.to_csv(
             path_or_buf=os.path.join(write_dir, "mask_labels.csv")
         )
```

### Comparing `mirp-2.2.0/mirp/settings/feature_parameters.py` & `mirp-2.2.1/mirp/settings/feature_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from mirp.settings.utilities import setting_def
 
 
 @dataclass
 class FeatureExtractionSettingsClass:
     """
     Parameters related to feature computation. Many are conditional on the type of features that will be computed (
-    ``base_feature_families``).
+    ``base_feature_families``). Features and their parameters are defined `here <https://arxiv.org/abs/1612.07003>`_.
 
     Parameters
     ----------
     by_slice: str or bool, optional, default: False
         Defines whether calculations should be performed in 2D (True) or 3D (False), or alternatively only in the
         largest slice ("largest"). See :class:`~mirp.settings.general_parameters.GeneralSettingsClass`.
```

### Comparing `mirp-2.2.0/mirp/settings/general_parameters.py` & `mirp-2.2.1/mirp/settings/general_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/settings/generic.py` & `mirp-2.2.1/mirp/settings/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 import copy
+import sys
+if sys.version_info >= (3, 11):
+    from typing import Unpack
+else:
+    from typing_extensions import Unpack
 
 from mirp.settings.feature_parameters import FeatureExtractionSettingsClass
 from mirp.settings.general_parameters import GeneralSettingsClass
 from mirp.settings.image_processing_parameters import ImagePostProcessingClass
 from mirp.settings.transformation_parameters import ImageTransformationSettingsClass
 from mirp.settings.interpolation_parameters import ImageInterpolationSettingsClass, MaskInterpolationSettingsClass
 from mirp.settings.resegmentation_parameters import ResegmentationSettingsClass
@@ -48,15 +53,15 @@
         Configuration object for parameters related to feature computation. See
         :class:`~mirp.settings.feature_parameters.FeatureExtractionSettingsClass`.
 
     img_transform_settings: ImageTransformationSettingsClass, optional
         Configuration object for parameters related to image transformation. See
         :class:`~mirp.settings.transformation_parameters.ImageTransformationSettingsClass`.
 
-    **kwargs: dict, optional
+    **kwargs: Any, optional
         Keyword arguments for initialising configuration objects stored in this container object.
 
     See Also
     --------
 
     * general settings (:class:`~mirp.settings.general_parameters.GeneralSettingsClass`)
     * image post-processing (:class:`~mirp.settings.image_processing_parameters.ImagePostProcessingClass`)
@@ -75,15 +80,19 @@
             post_process_settings: None | ImagePostProcessingClass = None,
             perturbation_settings: None | ImagePerturbationSettingsClass = None,
             img_interpolate_settings: None | ImageInterpolationSettingsClass = None,
             roi_interpolate_settings: None | MaskInterpolationSettingsClass = None,
             roi_resegment_settings: None | ResegmentationSettingsClass = None,
             feature_extr_settings: None | FeatureExtractionSettingsClass = None,
             img_transform_settings: None | ImageTransformationSettingsClass = None,
-            **kwargs
+            **kwargs: Unpack[
+                None | GeneralSettingsClass | ImagePostProcessingClass | ImagePostProcessingClass |
+                ImageInterpolationSettingsClass | MaskInterpolationSettingsClass | ResegmentationSettingsClass |
+                FeatureExtractionSettingsClass | ImageTransformationSettingsClass
+            ]
     ):
         kwargs = copy.deepcopy(kwargs)
 
         # General settings.
         if general_settings is None:
             general_settings = GeneralSettingsClass(**kwargs)
         self.general = general_settings
```

### Comparing `mirp-2.2.0/mirp/settings/image_processing_parameters.py` & `mirp-2.2.1/mirp/settings/image_processing_parameters.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,27 +12,54 @@
     resampling are set separately, see :class:`~mirp.settings.perturbation_parameters.ImagePerturbationSettingsClass` and
     :class:`~mirp.settings.interpolation_parameters.ImageInterpolationSettingsClass`.
 
     Parameters
     ----------
     bias_field_correction: bool, optional, default: False
         Determines whether N4 bias field correction should be performed. When a tissue mask is present, bias field
-        correction is conducted using the information contained within the mask. Bias-field correction can only be
-        applied to MR imaging.
+        correction is conducted using the information contained within the mask.
+
+        .. note::
+            Bias-field correction can only be applied to MR imaging.
 
     bias_field_correction_n_fitting_levels: int, optional, default: 1
         The number of fitting levels for the N4 bias field correction algorithm.
 
     bias_field_correction_n_max_iterations: int or list of int, optional, default: 50
         The number of fitting iterations for the N4 bias field algorithm. A single integer, or a list of integers
         with a length equal to the number of fitting levels is expected.
 
     bias_field_convergence_threshold: float, optional, default: 0.001
         Convergence threshold for N4 bias field correction algorithm.
 
+    pet_suv_conversion: {"body_weight", "none"}, default: "body_weight"
+        Intensities in PET imaging are often stored as detected radiotracer activity. To make detected activity more
+        comparable between patients, these are converted to standardised uptake values. The following are possible:
+
+        * "body_weight": activity is normalised by body weight.
+        * "body_surface_area": activity is normalised by body surface area according to DuBois (A formula to estimate
+          the approximate surface area if height and weight be known. Arch intern med. 1916;17:863-71).
+        * "lean_body_mass": activity is normalised by lean body mass according to James et al. (DHSS/MRC Group on
+          Obesity Research, James WP, Waterlow JC. Research on Obesity: A Report of the DHSS/MRC Group; Compiled by
+          WPT James. HM Stationery Office; 1976).
+        * "lean_body_mass_bmi": activity is normalised by lean body mass according to Janmahasatian et al.
+          (Quantification of lean bodyweight. Clinical pharmacokinetics. 2005 Oct;44:1051-65).
+        * "ideal_body_weight": activity is normalised by ideal body weight according to Zasadny and Wahl (
+          Standardized uptake values of normal tissues at PET with 2-[fluorine-18]-fluoro-2-deoxy-D-glucose:
+          variations with body weight and a method for correction. Radiology. 1993 Dec;189(3):847-50).
+        * "none": activity is not normalised.
+
+        .. note::
+            Conversion of activity to standardised uptake values can only be performed for PET data.
+
+        .. warning::
+            Conversion of activity to standardised uptake values requires metadata related to image acquisition and to
+            the patient. These metadata are only present in DICOM files. MIRP cannot convert activity to standardised
+            uptake values for images in different formats, and this parameter will have no effect.
+
     intensity_normalisation: {"none", "range", "relative_range", "quantile_range", "standardisation"}, default: "none"
         Specifies the algorithm used to normalise intensities in the image. Will use only intensities in voxels
         masked by the tissue mask (of present). The following are possible:
 
         * "none": no normalisation
         * "range": normalises intensities based on a fixed mapping against the ``intensity_normalisation_range``
           parameter, which is interpreted to represent an intensity range.
@@ -40,15 +67,16 @@
           parameter, which is interpreted to represent a relative intensity range.
         * "quantile_range": normalises intensities based on a fixed mapping against the
           ``intensity_normalisation_range`` parameter, which is interpreted to represent a quantile range.
         * "standardisation": normalises intensities by subtraction of the mean intensity and division by the standard
           deviation of intensities.
 
         .. note::
-            intensity normalisation may remove any physical meaning of intensity units.
+            Intensity normalisation may remove any physical meaning of intensity units. For example, intensity
+            normalisation of CT images yield intensities that no longer represent Hounsfield Units.
 
     intensity_normalisation_range: list of float, optional
         Required for "range", "relative_range", and "quantile_range" intensity normalisation methods, and defines the
         intensities that are mapped to the [0.0, 1.0] range during normalisation. The default range depends on the
         type of normalisation method:
 
         * "range": [np.nan, np.nan]: the minimum and maximum intensity value present in the image are used to set the
@@ -89,14 +117,15 @@
 
     def __init__(
             self,
             bias_field_correction: bool = False,
             bias_field_correction_n_fitting_levels: int = 1,
             bias_field_correction_n_max_iterations: int | list[int] | None = None,
             bias_field_convergence_threshold: float = 0.001,
+            pet_suv_conversion: str = "body_weight",
             intensity_normalisation: str = "none",
             intensity_normalisation_range: list[float] | None = None,
             intensity_normalisation_saturation: list[float] | None = None,
             intensity_scaling: float | None = None,
             tissue_mask_type: str = "relative_range",
             tissue_mask_range: list[float] | None = None,
             **kwargs
@@ -179,14 +208,27 @@
 
         else:
             bias_field_convergence_threshold = None
 
         # Set convergence_threshold attribute.
         self.convergence_threshold: None | float = bias_field_convergence_threshold
 
+        # Check that pet_suv_conversion has the correct values.
+        if pet_suv_conversion not in [
+            "body_weight", "body_surface_area", "lean_body_mass", "lean_body_mass_bmi", "ideal_body_weight", "none"
+        ]:
+            raise ValueError(
+                f"The pet_suv_conversion parameter is expected to have one of the following values: ",
+                f"'body_weight', `body_surface_area`, `lean_body_mass`, `lean_body_mass_bmi`, `ideal_body_weight` or "
+                f"'none'. Found: {pet_suv_conversion}"
+            )
+
+        # Set suv_conversion_type parameter.
+        self.suv_conversion_type = pet_suv_conversion
+
         # Check that intensity_normalisation has the correct values.
         if intensity_normalisation not in ["none", "range", "relative_range", "quantile_range", "standardisation"]:
             raise ValueError(
                 f"The intensity_normalisation parameter is expected to have one of the following values: "
                 f"'none', 'range', 'relative_range', 'quantile_range', 'standardisation'. Found: "
                 f"{intensity_normalisation}.")
 
@@ -351,14 +393,15 @@
             "bias_field_correction_n_max_iterations", "int", xml_key="n_max_iterations",
             class_key="n_max_iterations", to_list=True, test=[1000, 1000]
         ),
         setting_def(
             "bias_field_convergence_threshold", "float", xml_key="convergence_threshold",
             class_key="convergence_threshold", test=0.1
         ),
+        setting_def("pet_suv_conversion", "str", class_key="suv_conversion_type", test="none"),
         setting_def("intensity_normalisation", "str", test="relative_range"),
         setting_def("intensity_normalisation_range", "float", to_list=True, test=[0.10, 0.90]),
         setting_def("intensity_normalisation_saturation", "float", to_list=True, test=[0.00, 10.00]),
         setting_def("intensity_scaling", "float", test=3.0),
         setting_def("tissue_mask_type", "str", test="range"),
         setting_def("tissue_mask_range", "float", to_list=True, test=[0.00, 10.00])
     ]
```

### Comparing `mirp-2.2.0/mirp/settings/import_config_parameters.py` & `mirp-2.2.1/mirp/settings/import_config_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/settings/import_data_parameters.py` & `mirp-2.2.1/mirp/settings/import_data_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/settings/interpolation_parameters.py` & `mirp-2.2.1/mirp/settings/interpolation_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from mirp.settings.utilities import setting_def
 
 
 @dataclass
 class ImageInterpolationSettingsClass:
     """
     Parameters related to image interpolating / resampling. Images in a dataset are typically resampled to uniform
-    voxel spacing to ensure that their spatial representation does not vary between samples. Note that when the
-    voxel spacing in the original image is smaller than that in the resampled image (e.g., 0.5 mm sampled to 1.0 mm),
-    antialiasing may be recommended.
+    voxel spacing to ensure that their spatial representation does not vary between samples.
 
     For parameters related to mask interpolation / resampling, see
     :class:`~mirp.settings.interpolation_parameters.MaskInterpolationSettingsClass`.
 
     Parameters
     ----------
     by_slice: str or bool, optional, default: False
@@ -34,17 +32,23 @@
         <https://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.map_coordinates.html#scipy.ndimage
         .map_coordinates>`_ internally. Spline orders 0, 1, and 3 refer to nearest neighbour, linear interpolation
         and cubic interpolation, respectively.
 
     anti_aliasing: bool, optional, default: true
         Determines whether to perform antialiasing, which is done to mitigate aliasing artifacts when downsampling.
 
+        .. note::
+            When voxel spacing in the original image is smaller than that in the resampled image (e.g., 0.5 mm sampled
+            to 1.0 mm), antialiasing is recommended `[Mackin et al.] <http://dx.doi.org/10.1371/journal.pone.0178524>`_.
+
     smoothing_beta: float, optional, default: 0.98
         Determines the smoothness of the Gaussian filter used for anti-aliasing. A value of 1.00 equates to no
         antialiasing, with lower values producing increasingly smooth imaging. Values above 0.90 are recommended.
+        The effect of this parameter is shown in the supplement of `Zwanenburg et al.
+        <http://dx.doi.org/10.1038/s41598-018-36938-4>`_.
 
     **kwargs: dict, optional
         Unused keyword arguments.
     """
 
     def __init__(
             self,
```

### Comparing `mirp-2.2.0/mirp/settings/perturbation_parameters.py` & `mirp-2.2.1/mirp/settings/perturbation_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/settings/resegmentation_parameters.py` & `mirp-2.2.1/mirp/settings/resegmentation_parameters.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/settings/transformation_parameters.py` & `mirp-2.2.1/mirp/settings/transformation_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from mirp.settings.utilities import setting_def
 
 
 @dataclass
 class ImageTransformationSettingsClass:
     """
     Parameters related to image transformation using filters. Many parameters are conditional on the selected image
-    filter (``filter_kernels``). By default, only statistical features are computed from filtered images.
+    filter (``filter_kernels``). Filters and their parameters are defined `here <https://arxiv.org/abs/2006.05470>`_
+    By default, only statistical features are computed from filtered images.
 
     .. note::
         Many feature extraction parameters are copied from
         :class:`~mirp.settings.feature_parameters.FeatureExtractionSettingsClass`, except
         ``response_map_feature_families``, ``response_map_discretisation_method`` and
         ``response_map_discretisation_n_bins``. If other parameters need to be changed from their default settings,
         first create an object of the current class (
@@ -56,15 +57,15 @@
 
         In addition, the following tags can be used:
 
         * "none": no features are computed.
         * "all": all features are computed.
 
         A list of tags may be provided to select multiple feature families. Morphological features are not computed
-        from response maps, because these are mask-based and are invariant to filtering.
+        from response maps (filtered images), because these are mask-based and are invariant to filtering.
 
     response_map_discretisation_method: {"fixed_bin_number", "fixed_bin_size", "fixed_bin_size_pyradiomics", "none"}, optional, default: "fixed_bin_number"
         Method used for discretising intensities. Used to compute intensity histogram as well as texture features.
         The setting is ignored if none of these feature families are being computed. The following options are
         available:
 
         * "fixed_bin_number": The intensity range within the mask is divided into a fixed number of bins,
@@ -120,15 +121,15 @@
         .. note::
             There is no IBSI reference standard for Gaussian filters. However, the filter implementation is relatively
             straightforward, and most likely reproducible.
 
         .. warning::
             Riesz transformation and steerable riesz transformations are experimental. The implementation of these
             filter transformations is complex. Since there is no corresponding IBSI reference standard, any feature
-            derived from response maps of Riesz transformations is unlikely to be reproducible.
+            derived from response maps (filtered images) of Riesz transformations is unlikely to be reproducible.
 
         .. warning::
             Function transformations (square, square root, logarithm, exponential) do not have an IBSI reference
             standard. These transformations follow the definition in pyradiomics, and have been implemented for
             validation purposes.
 
     boundary_condition: {"reflect", "constant", "nearest", "mirror", "wrap"}, optional, default: "mirror"
@@ -150,25 +151,25 @@
 
     separable_wavelet_stationary: bool, optional, default: True
         Determines if wavelets are stationary or not. Stationary wavelets maintain the image dimensions after
         decomposition.
 
     separable_wavelet_decomposition_level: int or list of int, optional, default: 1
         Sets the wavelet decomposition level. For the first decomposition level, the base image is used as input to
-        generate a  response map. For decomposition levels greater than 1, the low-pass image from the previous level
-        is used as input. More than 1 value may be specified in a list.
+        generate a  response map (filtered image). For decomposition levels greater than 1, the low-pass image from the
+        previous level is used as input. More than 1 value may be specified in a list.
 
     separable_wavelet_rotation_invariance: bool, optional, default: True
         Determines whether separable filters are applied in a pseudo-rotational invariant manner. This generates
-        permutations of the filter and, as a consequence, additional response maps. These maps are then merged using
-        the pooling method (``separable_wavelet_pooling_method``).
+        permutations of the filter and, as a consequence, additional response maps (filtered images). These maps are
+        then merged using the pooling method (``separable_wavelet_pooling_method``).
 
     separable_wavelet_pooling_method: {"max", "min", "mean", "sum"}, optional, default: "max"
-        Response maps are pooled to create a rotationally invariant response map. This sets the method for
-        pooling.
+        Response maps are pooled to create a rotationally invariant response map (filtered image). This sets the
+        method for pooling.
 
         * "max": Each voxel of the pooled response map represents the maximum value for that voxel in the underlying
           response maps.
         * "min": Each voxel of the pooled response map represents the minimum value for that voxel in the underlying
           response maps.
         * "mean": Each voxel of the pooled response map represents the mean value for that voxel in the underlying
           response maps. For band-pass and high-pass filters, this will likely result in values close to 0.0,
@@ -186,17 +187,17 @@
 
     nonseparable_wavelet_decomposition_level: int or list of int, optional, default: 1
         Sets the wavelet decomposition level. Unlike the decomposition level in separable wavelets, decomposition of
         non-separable wavelets is purely a filter-based operation.
 
     nonseparable_wavelet_response: {"modulus", "abs", "magnitude", "angle", "phase", "argument", "real", "imaginary"}, optional, default: "real"
         Nonseparable wavelets produce response maps with complex numbers. The complex-valued response map is
-        converted to a real-valued response map using the specified method. "modulus", "abs", "magnitude" are
-        synonymous, as are "angle", "phase", and "argument". "real" selects the real component of the complex values,
-        and "imaginary" selects the imaginary component.
+        converted to a real-valued response map (filtered image) using the specified method. "modulus", "abs",
+        "magnitude" are synonymous, as are "angle", "phase", and "argument". "real" selects the real component of the
+        complex values, and "imaginary" selects the imaginary component.
 
     nonseparable_wavelet_boundary_condition: str, optional, default: "mirror"
         Sets the boundary condition for non-separable wavelets. This supersedes any value set by the general
         ``boundary_condition`` parameter. See the ``boundary_condition`` parameter above for all valid options.
 
     gaussian_sigma: float or list of float, optional
          Width of the Gaussian filter in physical dimensions (e.g. mm). Multiple values can be specified.
@@ -211,16 +212,16 @@
     laplacian_of_gaussian_sigma: float or list of float, optional
         Width of the Gaussian filter in physical dimensions (e.g. mm). Multiple values can be specified.
 
     laplacian_of_gaussian_kernel_truncate: float, optional, default: 4.0
         Width, in sigma, at which the filter is truncated.
 
     laplacian_of_gaussian_pooling_method: {"max", "min", "mean", "sum", "none"}, optional, default: "none"
-        Determines whether and how response maps for filters with different widths (``laplacian_of_gaussian_sigma``)
-        are pooled.
+        Determines whether and how response maps (filtered images) for filters with different widths (
+        ``laplacian_of_gaussian_sigma``) are pooled.
 
         * "max": Each voxel of the pooled response map represents the maximum value for that voxel in the underlying
           response maps.
         * "min": Each voxel of the pooled response map represents the minimum value for that voxel in the underlying
           response maps.
         * "mean": Each voxel of the pooled response map represents the mean value for that voxel in the underlying
           response maps. For band-pass and high-pass filters, this will likely result in values close to 0.0,
@@ -236,27 +237,27 @@
     laws_kernel: str or list of str, optional
         Compute specific Laws kernels these typically are specific combinations of kernels such as L5S5E5,
         E5E5E5. The following kernels are available: 'l5', 'e5', 's5', 'w5', 'r5', 'l3', 'e3', 's3'. A combination of
         two kernels is expected for 2D (``by_slice=True``), whereas a kernel triplet is expected for 3D filters (
         ``by_slice=False``).
 
     laws_compute_energy: bool, optional, default: True
-        Determine whether an energy image should be computed, or just the response map.
+        Determine whether an energy image should be computed, or just the response map (filtered) image.
 
     laws_delta: int or list of int, optional, default: 7
         Delta for chebyshev distance between center voxel and neighbourhood boundary used to calculate energy maps.
 
     laws_rotation_invariance: bool, optional, default: True
         Determines whether separable filters are applied in a pseudo-rotational invariant manner. This generates
-        permutations of the filter and, as a consequence, additional response maps. These maps are then merged using
-        the pooling method (``laws_pooling_method``).
+        permutations of the filter and, as a consequence, additional response maps (filtered images). These maps are
+        then merged using the pooling method (``laws_pooling_method``).
 
     laws_pooling_method:  {"max", "min", "mean", "sum"}, optional, default: "max"
-        Response maps are pooled to create a rotationally invariant response map. This sets the method for
-        pooling.
+        Response maps are pooled to create a rotationally invariant response map (filtered image). This sets the
+        method for pooling.
 
         * "max": Each voxel of the pooled response map represents the maximum value for that voxel in the underlying
           response maps.
         * "min": Each voxel of the pooled response map represents the minimum value for that voxel in the underlying
           response maps.
         * "mean": Each voxel of the pooled response map represents the mean value for that voxel in the underlying
           response maps. For band-pass and high-pass filters, this will likely result in values close to 0.0,
@@ -282,25 +283,25 @@
         Initial angle of the Gabor filter in degrees (not radians). Multiple angles can be provided.
 
     gabor_theta_step: float, optional, default: None
         Angle step size in degrees for in-plane rotational invariance. A value of 0.0 or None (default) disables
         stepping.
 
     gabor_response: {"modulus", "abs", "magnitude", "angle", "phase", "argument", "real", "imaginary"}, optional, default: "modulus"
-        Type of response map created by Gabor filters. Gabor kernels consist of complex numbers, and the response map
-        will be complex as well. The complex-valued response map is converted to a real-valued response map using the
-        specified method.
+        Type of response map (filtered image) created by Gabor filters. Gabor kernels consist of complex numbers,
+        and the response map will be complex as well. The complex-valued response map is converted to a real-valued
+        response map using the specified method.
 
     gabor_rotation_invariance: bool, optional, default: False
         Determines whether (2D) Gabor filters are applied in a pseudo-rotational invariant manner. If True,
         Gabor filters are applied in each of the orthogonal planes.
 
     gabor_pooling_method: {"max", "min", "mean", "sum"}, optional, default: "max"
-        Response maps are pooled to create a rotationally invariant response map. This sets the method for
-        pooling.
+        Response maps are pooled to create a rotationally invariant response map (filtered image). This sets the
+        method for pooling.
 
         * "max": Each voxel of the pooled response map represents the maximum value for that voxel in the underlying
           response maps.
         * "min": Each voxel of the pooled response map represents the minimum value for that voxel in the underlying
           response maps.
         * "mean": Each voxel of the pooled response map represents the mean value for that voxel in the underlying
           response maps. For band-pass and high-pass filters, this will likely result in values close to 0.0,
@@ -309,15 +310,16 @@
           response maps. Similar to the "mean" pooling method, but without the normalisation.
 
     gabor_boundary_condition: str, optional, default: "mirror"
         Sets the boundary condition for Gabor filters. This supersedes any value set by the general
         ``boundary_condition`` parameter. See the ``boundary_condition`` parameter above for all valid options.
 
     mean_filter_kernel_size: int or list of int, optional
-        Length of the kernel in pixels. Multiple values can be specified to create multiple response maps.
+        Length of the kernel in pixels. Multiple values can be specified to create multiple response maps (filtered
+        images).
 
     mean_filter_boundary_condition: str, optional, default: "mirror"
         Sets the boundary condition for mean filters. This supersedes any value set by the general
         ``boundary_condition`` parameter. See the ``boundary_condition`` parameter above for all valid options.
 
     riesz_filter_order: float, list of float or list of list of float, optional
         Riesz-transformation order. If required, should be a 2 (2D filter), or 3-element (3D filter) integer
```

### Comparing `mirp-2.2.0/mirp/settings/utilities.py` & `mirp-2.2.1/mirp/settings/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp/utilities/config_utilities.py` & `mirp-2.2.1/mirp/utilities/config_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os.path
 import shutil
 import sys
 import warnings
+from pathlib import Path
 
 
-def get_settings_xml(target_dir: str):
+def get_settings_xml(target_dir: str | Path):
     """
     Creates a local copy of the settings ``xml`` file. This file can be used to configure the image processing and
     feature extraction workflow.
 
     Parameters
     ----------
-    target_dir: str
+    target_dir: str or Path
         Path where the settings ``xml`` file should be copied to.
 
     Returns
     -------
     None
         No return values. The settings ``xml`` is copied to the intended directory.
     """
@@ -38,21 +39,21 @@
     source_file_path = os.path.join(mirp_dir, "config_settings.xml")
 
     shutil.copy(source_file_path, destination_file_path)
 
     print(f"A copy of the settings xml file was created at {destination_file_path}.")
 
 
-def get_data_xml(target_dir: str):
+def get_data_xml(target_dir: str | Path):
     """
     Creates a local copy of the data ``xml`` file. This file can be used to configure import of images and masks.
 
     Parameters
     ----------
-    target_dir: str
+    target_dir: str or Path
         Path where the data ``xml`` file should be copied to.
 
     Returns
     -------
     None
         No return values. The data ``xml`` is copied to the intended directory.
     """
```

### Comparing `mirp-2.2.0/mirp/utilities/utilities.py` & `mirp-2.2.1/mirp/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `mirp-2.2.0/mirp.egg-info/PKG-INFO` & `mirp-2.2.1/mirp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirp
-Version: 2.2.0
+Version: 2.2.1
 Summary: A package for standardised processing of medical imaging and computation of quantitative features.
 Author-email: Alex Zwanenburg <alexander.zwanenburg@nct-dresden.de>
 License: European Union Public Licence
         V. 1.2
         
         EUPL © the European Union 2007, 2016
         
@@ -280,91 +280,80 @@
         
 Project-URL: Repository, https://github.com/oncoray/mirp
 Project-URL: Documentation, https://oncoray.github.io/mirp/
 Project-URL: Changelog, https://github.com/oncoray/mirp/blob/master/NEWS.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: itk>=5.3.0
 Requires-Dist: matplotlib>=3.7.0
 Requires-Dist: numpy>=1.25
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: pydicom>=2.4.0
 Requires-Dist: pywavelets>=1.4.0
-Requires-Dist: ray>=2.7.0
 Requires-Dist: scikit-image>=0.20.0
 Requires-Dist: scipy>=1.11
 Requires-Dist: typing-extensions>=4.10; python_version < "3.11"
+Requires-Dist: ray>=2.10.0; python_version <= "3.11"
 Provides-Extra: test
 Requires-Dist: pytest>=7.4.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx>=5.0.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=2.0.0; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
 
 <img src="https://raw.githubusercontent.com/oncoray/mirp/master/icon/mirp.svg" align="right" width="120"/>
 
 # Medical Image Radiomics Processor
 
-Medical Image Radiomics Processor (MIRP) is an IBSI-compliant python package for medical image analysis.
-MIRP focuses on radiomics applications and supports computation of features for conventional radiomics
-and image processing for deep-learning applications.
+Medical Image Radiomics Processor (MIRP) is a python package for medical image analysis that is compliant with the 
+reference standards of the Image Biomarker Standardisation Initiative (IBSI). MIRP focuses on radiomics applications 
+and supports computation of features for conventional radiomics and image processing for deep-learning applications.
 
-## Documentation
+## Documentation and tutorials
 
-Documentation can be found here: https://oncoray.github.io/mirp/
+Documentation and tutorials can be found here: https://oncoray.github.io/mirp/
+
+## Supported Python and OS
+
+MIRP currently supports the following Python versions and operating systems: 
+
+| Python | Linux     | Win       | OSX       |
+|--------|-----------|-----------|-----------|
+| 3.10   | Supported | Supported | Supported |
+| 3.11   | Supported | Supported | Supported |
+
+## Supported imaging and mask modalities
+
+MIRP currently supports the following image modalities:
+
+| File format | File type | Supported modality |
+|-------------|-----------|--------------------|
+| DICOM       | image     | CT, MR, PT, RTDOSE |
+| DICOM       | mask      | RTSTRUCT, SEG      |
+| NIfTI       | any       | any                |
+| NRRD        | any       | any                |
+| numpy       | any       | any                |
+
+NIfTI, NRRD, and numpy files support any kind of (single-channel) image. MIRP cannot process RGB or 4D images.
 
 ## Installing MIRP
 MIRP is available from PyPI and can be installed using `pip`, or other installer tools:
 
 ```commandline
 pip install mirp
 ```
 
-## Transitioning to version 2
-
-Version 2 is a major refactoring of the previous code base. For users this brings the following noticeable changes:
-
-- MIRP was previously configured using two `xml` files: [`config_data.xml`](mirp/config_data.xml) for configuring
-  directories, data to be read, etc., and [`config_settings.xml`](mirp/config_settings.xml) for configuring experiments.
-  While these two files can still be used, MIRP can now be configured directly, without using these files.
-- The main functions of MIRP (`mainFunctions.py`) have all been re-implemented.
-  - `mainFunctions.extract_features` is now `extract_features` (functional form) or
-    `extract_features_generator` (generator). The replacements allow for both writing
-    feature values to a directory and returning them as function output. 
-  - `mainFunctions.extract_images_to_nifti` is now `extract_images` (functional form) or
-     `extract_images_generator` (generator). The replacements allow for both writing 
-     images to a directory (e.g., in NIfTI or numpy format) and returning them as function output.
-  - `mainFunctions.extract_images_for_deep_learning` has been replaced by 
-    `deep_learning_preprocessing` (functional form) and 
-    `deep_learning_preprocessing_generator` (generator).
-  - `mainFunctions.get_file_structure_parameters` and `mainFunctions.parse_file_structure` are deprecated, as the
-    the file import system used in version 2 no longer requires a rigid directory structure.
-  - `mainFunctions.get_roi_labels` is now `extract_mask_labels`.
-  - `mainFunctions.get_image_acquisition_parameters` is now `extract_image_parameters`.
-
-For advanced users and developers, the following changes are relevant:
-- MIRP previously relied on `ImageClass` and `RoiClass` objects. These have been completely replaced by `GenericImage`
-  (and its subclasses, e.g. `CTImage`) and `BaseMask` objects, respectively. New image modalities can be added as
-  subclass of `GenericImage` in the `mirp.images` submodule.
-- File import, e.g. from DICOM or NIfTI files, in version 1 was implemented in an ad-hoc manner, and required a rigid
-  directory structure. Since version 2, file import is implemented using an object-oriented approach, and directory
-  structures are more flexible. File import of new modalities can be implemented as a relevant subclass of `ImageFile`.
-- MIRP uses type hinting, and makes use of the `Self` type hint introduced in Python 3.11. MIRP 
-  therefore requires Python 3.11 or later.
-- MIRP now uses the `ray` package for parallel processing.
-
 ## Examples - Computing Radiomics Features
 
 MIRP can be used to compute quantitative features from regions of interest in images in an IBSI-compliant manner 
 using a standardized workflow This requires both images and masks. MIRP can process DICOM, NIfTI, NRRD and numpy 
 images. Masks are DICOM radiotherapy structure sets (RTSTRUCT), or volumetric data with integer labels (e.g. 1, 2, 
 etc.).
 
@@ -462,14 +451,45 @@
 from mirp import extract_mask_labels
 mask_labels = extract_mask_labels(
     mask="path to main mask directory",
     mask_sub_folder="mask subdirectory structure relative to main mask directory"
 )
 ```
 
+## Transitioning to version 2
+
+Version 2 is a major refactoring of the previous code base. For users this brings the following noticeable changes:
+
+- MIRP was previously configured using two `xml` files: [`config_data.xml`](mirp/config_data.xml) for configuring
+  directories, data to be read, etc., and [`config_settings.xml`](mirp/config_settings.xml) for configuring experiments.
+  While these two files can still be used, MIRP can now be configured directly, without using these files.
+- The main functions of MIRP (`mainFunctions.py`) have all been re-implemented.
+  - `mainFunctions.extract_features` is now `extract_features` (functional form) or
+    `extract_features_generator` (generator). The replacements allow for both writing
+    feature values to a directory and returning them as function output. 
+  - `mainFunctions.extract_images_to_nifti` is now `extract_images` (functional form) or
+     `extract_images_generator` (generator). The replacements allow for both writing 
+     images to a directory (e.g., in NIfTI or numpy format) and returning them as function output.
+  - `mainFunctions.extract_images_for_deep_learning` has been replaced by 
+    `deep_learning_preprocessing` (functional form) and 
+    `deep_learning_preprocessing_generator` (generator).
+  - `mainFunctions.get_file_structure_parameters` and `mainFunctions.parse_file_structure` are deprecated, as the
+    the file import system used in version 2 no longer requires a rigid directory structure.
+  - `mainFunctions.get_roi_labels` is now `extract_mask_labels`.
+  - `mainFunctions.get_image_acquisition_parameters` is now `extract_image_parameters`.
+
+For advanced users and developers, the following changes are relevant:
+- MIRP previously relied on `ImageClass` and `RoiClass` objects. These have been completely replaced by `GenericImage`
+  (and its subclasses, e.g. `CTImage`) and `BaseMask` objects, respectively. New image modalities can be added as
+  subclass of `GenericImage` in the `mirp.images` submodule.
+- File import, e.g. from DICOM or NIfTI files, in version 1 was implemented in an ad-hoc manner, and required a rigid
+  directory structure. Since version 2, file import is implemented using an object-oriented approach, and directory
+  structures are more flexible. File import of new modalities can be implemented as a relevant subclass of `ImageFile`.
+- MIRP now uses the `ray` package for parallel processing.
+
 # Citation info
 A publication for MIRP is forthcoming. For now, please cite the following work:
 ```Zwanenburg A, Leger S, Agolli L, Pilz K, Troost EG, Richter C, Löck S. Assessing robustness of radiomic features by image perturbation. Scientific reports. 2019 Jan 24;9(1):614.```
 
 # Contributing
 If you have ideas for improving MIRP, please read the short [contribution guide](./CONTRIBUTING.md).
```

### Comparing `mirp-2.2.0/mirp.egg-info/SOURCES.txt` & `mirp-2.2.1/mirp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -47,23 +47,19 @@
 mirp/_featuresets/ngldm.py
 mirp/_featuresets/ngtdm.py
 mirp/_featuresets/rlm.py
 mirp/_featuresets/statistics.py
 mirp/_featuresets/szm.py
 mirp/_featuresets/utilities.py
 mirp/_image_processing/__init__.py
-mirp/_image_processing/add_noise.py
 mirp/_image_processing/alter_mask.py
 mirp/_image_processing/anti_aliasing.py
 mirp/_image_processing/cropping.py
 mirp/_image_processing/discretise_image.py
-mirp/_image_processing/normalise_image.py
 mirp/_image_processing/randomise_mask.py
-mirp/_image_processing/resegmentise_mask.py
-mirp/_image_processing/saturate_image.py
 mirp/_image_processing/split_mask.py
 mirp/_image_processing/tissue_mask.py
 mirp/_image_processing/utilities.py
 mirp/_imagefilters/__init__.py
 mirp/_imagefilters/exponential_transform.py
 mirp/_imagefilters/gabor.py
 mirp/_imagefilters/gaussian.py
```

### Comparing `mirp-2.2.0/pyproject.toml` & `mirp-2.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mirp"
-version = "2.2.0"
+version = "2.2.1"
 description = "A package for standardised processing of medical imaging and computation of quantitative features."
 authors = [
     {name = "Alex Zwanenburg", email = "alexander.zwanenburg@nct-dresden.de"}
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "Programming Language :: Python :: 3.13",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Scientific/Engineering :: Medical Science Apps."
 ]
 requires-python = ">=3.10"
 dependencies = [
     "itk>=5.3.0",
     "matplotlib>=3.7.0",
     "numpy>=1.25",
     "pandas>=2.0.0",
     "pydicom>=2.4.0",
     "pywavelets>=1.4.0",
-    "ray>=2.7.0",
     "scikit-image>=0.20.0",
     "scipy>=1.11",
-    "typing-extensions>=4.10;  python_version<'3.11'"
+    "typing-extensions>=4.10; python_version<'3.11'",
+    "ray>=2.10.0; python_version<='3.11'"
 ]
 
 [project.urls]
 Repository = "https://github.com/oncoray/mirp"
 Documentation = "https://oncoray.github.io/mirp/"
 Changelog = "https://github.com/oncoray/mirp/blob/master/NEWS.md"
 
 [project.optional-dependencies]
 test = ["pytest>=7.4.0"]
-docs = ["sphinx>=5.0.0", "sphinx_rtd_theme>=2.0.0"]
+docs = ["sphinx>=5.0.0", "sphinx_rtd_theme>=2.0.0", "nbsphinx"]
+
+[tool.pytest.ini_options]
+addopts = ["--strict-markers"]
+markers = [
+    "ci: marks tests for continuous integration"
+]
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["mirp*"]
 exclude = ["docs*"]
 
 [tool.setuptools.package-data]
```

