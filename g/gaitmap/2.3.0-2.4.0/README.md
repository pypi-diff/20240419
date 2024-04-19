# Comparing `tmp/gaitmap-2.3.0.tar.gz` & `tmp/gaitmap-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap-2.3.0.tar", max compression
+gzip compressed data, was "gaitmap-2.4.0.tar", max compression
```

## Comparing `gaitmap-2.3.0.tar` & `gaitmap-2.4.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2032 2023-08-03 11:17:36.923938 gaitmap-2.3.0/LICENSE
--rw-r--r--   0        0        0    10679 2023-08-03 11:17:36.923938 gaitmap-2.3.0/README.md
--rw-r--r--   0        0        0       69 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/__init__.py
--rw-r--r--   0        0        0      164 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/_event_detection_common/__init__.py
--rw-r--r--   0        0        0     7510 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/_event_detection_common/_event_detection_mixin.py
--rw-r--r--   0        0        0    12216 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/base.py
--rw-r--r--   0        0        0     1316 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/data_transform/__init__.py
--rw-r--r--   0        0        0    15931 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/data_transform/_base.py
--rw-r--r--   0        0        0    12004 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/data_transform/_feature_transform.py
--rw-r--r--   0        0        0     3969 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/data_transform/_filter.py
--rw-r--r--   0        0        0    15524 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/data_transform/_scaler.py
--rw-r--r--   0        0        0      765 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/evaluation_utils/__init__.py
--rw-r--r--   0        0        0     6326 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/evaluation_utils/event_detection.py
--rw-r--r--   0        0        0    28925 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/evaluation_utils/parameter_errors.py
--rw-r--r--   0        0        0    11515 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/evaluation_utils/scores.py
--rw-r--r--   0        0        0    22255 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/evaluation_utils/stride_segmentation.py
--rw-r--r--   0        0        0      702 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/event_detection/__init__.py
--rw-r--r--   0        0        0    19385 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/event_detection/_herzer_event_detection.py
--rw-r--r--   0        0        0     7996 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/example_data.py
--rw-r--r--   0        0        0      542 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/gait_detection/__init__.py
--rw-r--r--   0        0        0      350 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/parameters/__init__.py
--rw-r--r--   0        0        0    21773 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/parameters/_spatial_parameters.py
--rw-r--r--   0        0        0     7836 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/parameters/_temporal_parameters.py
--rw-r--r--   0        0        0      287 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/preprocessing/__init__.py
--rw-r--r--   0        0        0      785 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0     5094 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
--rw-r--r--   0        0        0     3940 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
--rw-r--r--   0        0        0     6635 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
--rw-r--r--   0        0        0     1732 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/stride_segmentation/__init__.py
--rw-r--r--   0        0        0    14875 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py
--rw-r--r--   0        0        0     2713 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/stride_segmentation/_utils.py
--rw-r--r--   0        0        0     1181 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/stride_segmentation/hmm.py
--rw-r--r--   0        0        0     1029 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0    21419 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
--rw-r--r--   0        0        0     9438 2023-08-03 11:17:37.003943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
--rw-r--r--   0        0        0    10746 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
--rw-r--r--   0        0        0      317 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
--rw-r--r--   0        0        0     8096 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
--rw-r--r--   0        0        0     4858 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
--rw-r--r--   0        0        0      618 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0     7841 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
--rw-r--r--   0        0        0      243 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
--rw-r--r--   0        0        0    13664 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
--rw-r--r--   0        0        0    16637 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
--rw-r--r--   0        0        0       41 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/__init__.py
--rw-r--r--   0        0        0     1857 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/_algo_helper.py
--rw-r--r--   0        0        0     4695 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/_datatype_validation_helper.py
--rw-r--r--   0        0        0     1195 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/_gaitmap_mad.py
--rw-r--r--   0        0        0      381 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/_types.py
--rw-r--r--   0        0        0    17992 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/array_handling.py
--rw-r--r--   0        0        0     2555 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/consts.py
--rw-r--r--   0        0        0     6284 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/coordinate_conversion.py
--rw-r--r--   0        0        0    48845 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/datatype_helper.py
--rw-r--r--   0        0        0     1089 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/exceptions.py
--rw-r--r--   0        0        0     1865 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/fast_quaternion_math.py
--rw-r--r--   0        0        0    18908 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/rotations.py
--rw-r--r--   0        0        0     2372 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/signal_processing.py
--rw-r--r--   0        0        0    14377 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/static_moment_detection.py
--rw-r--r--   0        0        0     8512 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/stride_list_conversion.py
--rw-r--r--   0        0        0     4115 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/utils/vector_math.py
--rw-r--r--   0        0        0      670 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/zupt_detection/__init__.py
--rw-r--r--   0        0        0     1582 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/zupt_detection/_base.py
--rw-r--r--   0        0        0     3068 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/zupt_detection/_combo_zupt_detector.py
--rw-r--r--   0        0        0    21964 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py
--rw-r--r--   0        0        0     4897 2023-08-03 11:17:37.007943 gaitmap-2.3.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py
--rw-r--r--   0        0        0     5192 2023-08-03 11:17:37.011943 gaitmap-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    12050 1970-01-01 00:00:00.000000 gaitmap-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2032 2024-04-19 10:35:17.873916 gaitmap-2.4.0/LICENSE
+-rw-r--r--   0        0        0    11674 2024-04-19 10:35:17.873916 gaitmap-2.4.0/README.md
+-rw-r--r--   0        0        0       69 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/_event_detection_common/__init__.py
+-rw-r--r--   0        0        0     7495 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/_event_detection_common/_event_detection_mixin.py
+-rw-r--r--   0        0        0    12515 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/base.py
+-rw-r--r--   0        0        0     1317 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/data_transform/__init__.py
+-rw-r--r--   0        0        0    15973 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/data_transform/_base.py
+-rw-r--r--   0        0        0    12043 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/data_transform/_feature_transform.py
+-rw-r--r--   0        0        0     3943 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/data_transform/_filter.py
+-rw-r--r--   0        0        0    15601 2024-04-19 10:35:17.929916 gaitmap-2.4.0/gaitmap/data_transform/_scaler.py
+-rw-r--r--   0        0        0      765 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/evaluation_utils/__init__.py
+-rw-r--r--   0        0        0     6235 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/evaluation_utils/event_detection.py
+-rw-r--r--   0        0        0    28906 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/evaluation_utils/parameter_errors.py
+-rw-r--r--   0        0        0    11472 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/evaluation_utils/scores.py
+-rw-r--r--   0        0        0    22318 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/evaluation_utils/stride_segmentation.py
+-rw-r--r--   0        0        0      703 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/event_detection/__init__.py
+-rw-r--r--   0        0        0    19365 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/event_detection/_herzer_event_detection.py
+-rw-r--r--   0        0        0     8001 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/example_data.py
+-rw-r--r--   0        0        0      543 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/gait_detection/__init__.py
+-rw-r--r--   0        0        0      351 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/parameters/__init__.py
+-rw-r--r--   0        0        0    22578 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/parameters/_spatial_parameters.py
+-rw-r--r--   0        0        0     7833 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/parameters/_temporal_parameters.py
+-rw-r--r--   0        0        0      288 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/preprocessing/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0     5089 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
+-rw-r--r--   0        0        0     3940 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
+-rw-r--r--   0        0        0     6665 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
+-rw-r--r--   0        0        0     1732 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0    14886 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py
+-rw-r--r--   0        0        0     2707 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/stride_segmentation/_utils.py
+-rw-r--r--   0        0        0     1181 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/stride_segmentation/hmm.py
+-rw-r--r--   0        0        0     1355 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0    21027 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
+-rw-r--r--   0        0        0     9356 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
+-rw-r--r--   0        0        0    10514 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
+-rw-r--r--   0        0        0      317 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
+-rw-r--r--   0        0        0     8223 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
+-rw-r--r--   0        0        0     4957 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
+-rw-r--r--   0        0        0      618 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0     7849 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
+-rw-r--r--   0        0        0      243 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
+-rw-r--r--   0        0        0    13674 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
+-rw-r--r--   0        0        0    16858 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
+-rw-r--r--   0        0        0       41 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/__init__.py
+-rw-r--r--   0        0        0     1867 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/_algo_helper.py
+-rw-r--r--   0        0        0     4609 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/_datatype_validation_helper.py
+-rw-r--r--   0        0        0     1241 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/_gaitmap_mad.py
+-rw-r--r--   0        0        0      409 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/_types.py
+-rw-r--r--   0        0        0    18375 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/array_handling.py
+-rw-r--r--   0        0        0     2556 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/consts.py
+-rw-r--r--   0        0        0     6272 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/coordinate_conversion.py
+-rw-r--r--   0        0        0    48470 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/datatype_helper.py
+-rw-r--r--   0        0        0     1193 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/exceptions.py
+-rw-r--r--   0        0        0     1866 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/fast_quaternion_math.py
+-rw-r--r--   0        0        0    18902 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/rotations.py
+-rw-r--r--   0        0        0     2367 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/signal_processing.py
+-rw-r--r--   0        0        0    14394 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/static_moment_detection.py
+-rw-r--r--   0        0        0     8481 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/stride_list_conversion.py
+-rw-r--r--   0        0        0     4124 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/utils/vector_math.py
+-rw-r--r--   0        0        0      671 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/zupt_detection/__init__.py
+-rw-r--r--   0        0        0     1582 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/zupt_detection/_base.py
+-rw-r--r--   0        0        0     3063 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/zupt_detection/_combo_zupt_detector.py
+-rw-r--r--   0        0        0    21982 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py
+-rw-r--r--   0        0        0     4905 2024-04-19 10:35:17.933916 gaitmap-2.4.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py
+-rw-r--r--   0        0        0     3586 2024-04-19 10:35:17.941916 gaitmap-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13054 1970-01-01 00:00:00.000000 gaitmap-2.4.0/PKG-INFO
```

### Comparing `gaitmap-2.3.0/LICENSE` & `gaitmap-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap-2.3.0/README.md` & `gaitmap-2.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <img src="./docs/_static/logo/gaitmap_logo_with_text.png" height="200">
 
 [![PyPI](https://img.shields.io/pypi/v/gaitmap)](https://pypi.org/project/gaitmap/)
 [![pipeline status](https://github.com/mad-lab-fau/gaitmap/workflows/Test%20and%20Lint/badge.svg)](https://github.com/mad-lab-fau/gaitmap/actions/workflows/test-and-lint.yml)
 [![codecov](https://codecov.io/gh/mad-lab-fau/gaitmap/branch/master/graph/badge.svg?token=5NP5ZZ3KGX)](https://codecov.io/gh/mad-lab-fau/gaitmap)
-[![Documentation Status](https://readthedocs.org/projects/gaitmap/badge/?version=latest)](https://gaitmap.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/gaitmap/badge/?version=latest)](https://gaitmap.readthedocs.io/en/latest/README.html)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gaitmap)
 
 # gaitmap - The Gait and Movement Analysis Package
 
 *gaitmap* provides a set of algorithms to analyze your IMU movement data (with a focus on foot-worn IMUs) without 
 getting into your way.
 
 - 💻 [20+ Algorithms](https://gaitmap.readthedocs.io/en/latest/modules/index.html) from 17+ publications
 - 📚 Extensive [documentation](https://gaitmap.readthedocs.io/en/latest/)
 - 📝 Build to be [easily extendable](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)
 - ⚙️ Familiar API inspired by scikit-learn
 - 🤝 Interoperable with the other libraries from the gaitmap ecosystem ([gaitmap-dataset](https://github.com/mad-lab-fau/gaitmap-datasets), [tpcp](https://github.com/mad-lab-fau/tpcp), ...)
 
-**Documentation:** [gaitmap.readthedocs.io](https://gaitmap.readthedocs.io/en/latest/)<br>
-**Learn More about the gaitmap ecosystem:** Coming soon!
+**Documentation:** [gaitmap.readthedocs.io](https://gaitmap.readthedocs.io/en/latest/README.html)<br>
+**Learn more about the gaitmap ecosystem:** [the gaitmap ecosystem](https://gaitmap.readthedocs.io/en/latest/source/user_guide/gaitmap_ecosystem.html)
 
 ## Installation
 
 Gaitmap is split into two packages: `gaitmap` and `gaitmap_mad` ([Learn more](https://gaitmap.readthedocs.io/en/latest/source/user_guide/gaitmap_mad.html)).
 To get access to all available algorithms, you need to install both packages:
 
 ```bash
@@ -67,16 +67,16 @@
 Python 3.10.
 
 We are working on upgrading to a newer version of `pomegranate`, but this is not a priority at the moment.
 You can track the progress in the [pull request](https://github.com/mad-lab-fau/gaitmap/pull/20).
 
 ### Supported Python versions
 
-*gaitmap* is tested against Python 3.8 and 3.9 at the moment.
-We expect most features to work with all Python versions >= 3.8, but because of some known issues 
+*gaitmap* is tested against Python 3.9 at the moment.
+We expect most features to work with all Python versions >= 3.9, but because of some known issues 
 (see specific features above) we do not officially support them.
 
 ## Working with Algorithms
 
 *gaitmap* is designed to be a toolbox and not a single algorithm.
 This means, that you are expected to pick and use individual algorithms.
 
@@ -138,16 +138,31 @@
 For all these topics check out our [contributing guide](https://gaitmap.readthedocs.io/en/latest/source/user_guide/contributing.html) for more details.
 
 ## Citation
 
 If you use *gaitmap* in your research we would appreciate a citation.
 This helps us to justify the time we invest in the development and maintenance of the library.
 
-We currently prepare a paper to describe the *gaitmap* library in detail.
-Until then, please simply cite the repository.
+
+> A. Küderle et al., "Gaitmap—An Open Ecosystem for IMU-Based Human Gait Analysis and Algorithm Benchmarking," in IEEE Open Journal of Engineering in Medicine and Biology, vol. 5, pp. 163-172, 2024, doi: 10.1109/OJEMB.2024.3356791.
+
+
+```bibtex
+@ARTICLE{10411039,
+  author={Küderle, Arne and Ullrich, Martin and Roth, Nils and Ollenschläger, Malte and Ibrahim, Alzhraa A. and Moradi, Hamid and Richer, Robert and Seifer, Ann-Kristin and Zürl, Matthias and Sîmpetru, Raul C. and Herzer, Liv and Prossel, Dominik and Kluge, Felix and Eskofier, Bjoern M.},
+  journal={IEEE Open Journal of Engineering in Medicine and Biology}, 
+  title={Gaitmap—An Open Ecosystem for IMU-Based Human Gait Analysis and Algorithm Benchmarking}, 
+  year={2024},
+  volume={5},
+  number={},
+  pages={163-172},
+  keywords={Pipelines;Benchmark testing;Software algorithms;Ecosystems;Machine learning algorithms;Estimation;Trajectory;Accelerometer;walking;biomarker;biomechanics;movement analysis},
+  doi={10.1109/OJEMB.2024.3356791}}
+```
+
 
 If you use a specific algorithm please also make sure you cite the original paper of the algorithm!
 We recommend the following citation style:
 
 *We used the algorithm proposed by Author et al. [paper-citation], implemented by the Gaitmap package [gaitmap-citation].*
 
 ## License
```

### Comparing `gaitmap-2.3.0/gaitmap/_event_detection_common/_event_detection_mixin.py` & `gaitmap-2.4.0/gaitmap/_event_detection_common/_event_detection_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Mixin for event detection algorithms that work similar to Rampp et al."""
 
-from typing import Any, Callable, Dict, Optional, Tuple, Union
+from typing import Any, Callable, Optional, Union
 
 import numpy as np
 import pandas as pd
 from joblib import Memory
 from numpy.linalg import norm
 from typing_extensions import Self
 
@@ -26,29 +26,29 @@
     enforce_stride_list_consistency,
 )
 
 
 class _EventDetectionMixin:
     memory: Optional[Memory]
     enforce_consistency: bool
-    detect_only: Optional[Tuple[str, ...]]
+    detect_only: Optional[tuple[str, ...]]
 
-    min_vel_event_list_: Optional[Union[pd.DataFrame, Dict[str, pd.DataFrame]]]
-    segmented_event_list_: Optional[Union[pd.DataFrame, Dict[str, pd.DataFrame]]]
+    min_vel_event_list_: Optional[Union[pd.DataFrame, dict[str, pd.DataFrame]]]
+    segmented_event_list_: Optional[Union[pd.DataFrame, dict[str, pd.DataFrame]]]
 
     data: SensorData
     sampling_rate_hz: float
     stride_list: pd.DataFrame
 
     def __init__(
         self,
         memory: Optional[Memory] = None,
         enforce_consistency: bool = True,
-        detect_only: Optional[Tuple[str, ...]] = None,
-    ):
+        detect_only: Optional[tuple[str, ...]] = None,
+    ) -> None:
         self.memory = memory
         self.enforce_consistency = enforce_consistency
         self.detect_only = detect_only
 
     def detect(self, data: SensorData, stride_list: StrideList, *, sampling_rate_hz: float) -> Self:
         """Find gait events in data within strides provided by stride_list.
 
@@ -69,27 +69,27 @@
         """
         dataset_type = is_sensor_data(data, frame="body")
         stride_list_type = is_stride_list(stride_list, stride_type="any")
 
         if dataset_type != stride_list_type:
             raise ValidationError(
                 "An invalid combination of stride list and dataset was provided."
-                "The dataset is {} sensor and the stride list is {} sensor.".format(dataset_type, stride_list_type)
+                f"The dataset is {dataset_type} sensor and the stride list is {stride_list_type} sensor."
             )
 
         self.data = data
         self.sampling_rate_hz = sampling_rate_hz
         self.stride_list = stride_list
 
         detect_kwargs = self._get_detect_kwargs()
 
         if dataset_type == "single":
             results = self._detect_single_dataset(data, stride_list, detect_kwargs=detect_kwargs, memory=self.memory)
         else:
-            results_dict: Dict[_Hashable, Dict[str, pd.DataFrame]] = {}
+            results_dict: dict[_Hashable, dict[str, pd.DataFrame]] = {}
             for sensor in get_multi_sensor_names(data):
                 results_dict[sensor] = self._detect_single_dataset(
                     data[sensor],
                     stride_list[sensor],
                     detect_kwargs=detect_kwargs,
                     memory=self.memory,
                 )
@@ -100,17 +100,17 @@
         set_params_from_dict(self, results, result_formatting=True)
         return self
 
     def _detect_single_dataset(
         self,
         data: pd.DataFrame,
         stride_list: pd.DataFrame,
-        detect_kwargs: Dict[str, Any],
+        detect_kwargs: dict[str, Any],
         memory: Memory,
-    ) -> Dict[str, pd.DataFrame]:
+    ) -> dict[str, pd.DataFrame]:
         """Detect gait events for a single sensor data set and put into correct output stride list."""
         if memory is None:
             memory = Memory(None)
 
         acc = data[BF_ACC]
         gyr = data[BF_GYR]
 
@@ -164,15 +164,15 @@
     def _select_all_event_detection_method(self) -> Callable:
         """Select the function to calculate the all events.
 
         This is separate method to make it easy to overwrite by a subclass.
         """
         raise NotImplementedError()
 
-    def _get_detect_kwargs(self) -> Dict[str, Any]:
+    def _get_detect_kwargs(self) -> dict[str, Any]:
         """Return a dictionary of keyword arguments that should be passed to the detect method.
 
         This is a separate method to make it easy to overwrite by a subclass.
         """
         return {}
```

### Comparing `gaitmap-2.3.0/gaitmap/base.py` & `gaitmap-2.4.0/gaitmap/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Base class for all algorithms."""
 
 import json
 import warnings
-from typing import Any, Dict, Optional, Type, TypeVar, Union
+from typing import Any, Optional, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 import tpcp
 from joblib import Memory
 from scipy.spatial.transform import Rotation
 from typing_extensions import Self
@@ -18,14 +18,15 @@
     SensorData,
     SingleSensorData,
     SingleSensorOrientationList,
     SingleSensorStrideList,
     StrideList,
     VelocityList,
 )
+from gaitmap.utils.rotations import rotate_dataset_series
 
 BaseType = TypeVar("BaseType", bound="_BaseSerializable")  # pylint: disable=invalid-name
 
 
 def _hint_tuples(item):
     """Encode tuple values for json serialization.
 
@@ -40,15 +41,15 @@
     return item
 
 
 class _CustomEncoder(json.JSONEncoder):
     def encode(self, o: Any) -> str:
         return super().encode(_hint_tuples(o))
 
-    def default(self, o):  # noqa: C901
+    def default(self, o):  # noqa: C901, PLR0911
         if isinstance(o, _BaseSerializable):
             return o._to_json_dict()
         if isinstance(o, Rotation):
             return {"_obj_type": "Rotation", "quat": o.as_quat().tolist()}
         if isinstance(o, np.generic):
             return o.item()
         if isinstance(o, np.ndarray):
@@ -80,15 +81,15 @@
                 "This can be using `instance.set_params(memory=Memory(...))`"
             )
             return None
         # Let the base class default method raise the TypeError
         return super().default(o)
 
 
-def _custom_deserialize(json_obj):  # pylint: disable=too-many-return-statements
+def _custom_deserialize(json_obj):  # pylint: disable=too-many-return-statements  # noqa: PLR0911
     if "_gaitmap_obj" in json_obj:
         return _BaseSerializable._find_subclass(json_obj["_gaitmap_obj"])._from_json_dict(json_obj)
     if "_obj_type" in json_obj:
         if json_obj["_obj_type"] == "Rotation":
             return Rotation.from_quat(json_obj["quat"])
         if json_obj["_obj_type"] == "Array":
             return np.array(json_obj["array"])
@@ -110,35 +111,35 @@
         raise ValueError("Unknown object type found in serialization!")
 
     return json_obj
 
 
 class _BaseSerializable(tpcp.BaseTpcpObject):
     @classmethod
-    def _get_subclasses(cls: Type[Self]):
+    def _get_subclasses(cls: type[Self]):
         for subclass in cls.__subclasses__():
             yield from subclass._get_subclasses()
             yield subclass
 
     @classmethod
-    def _find_subclass(cls: Type[Self], name: str) -> Type[Self]:
+    def _find_subclass(cls: type[Self], name: str) -> type[Self]:
         for subclass in _BaseSerializable._get_subclasses():
             if subclass.__name__ == name:
                 return subclass
         raise ValueError(f"No algorithm class with name {name} exists")
 
     @classmethod
-    def _from_json_dict(cls: Type[Self], json_dict: Dict) -> Self:
+    def _from_json_dict(cls: type[Self], json_dict: dict) -> Self:
         params = json_dict["params"]
         input_data = {k: params[k] for k in tpcp.get_param_names(cls) if k in params}
         instance = cls(**input_data)
         return instance
 
-    def _to_json_dict(self) -> Dict[str, Any]:
-        json_dict: Dict[str, Union[str, Dict[str, Any]]] = {
+    def _to_json_dict(self) -> dict[str, Any]:
+        json_dict: dict[str, Union[str, dict[str, Any]]] = {
             "_gaitmap_obj": self.__class__.__name__,
             "params": self.get_params(deep=False),
         }
         return json_dict
 
     def to_json(self) -> str:
         """Export the current object parameters as json.
@@ -150,15 +151,15 @@
         .. warning:: This will only export the Parameters of the instance, but **not** any results!
 
         """
         final_dict = self._to_json_dict()
         return json.dumps(final_dict, indent=4, cls=_CustomEncoder)
 
     @classmethod
-    def from_json(cls: Type[Self], json_str: str) -> Self:
+    def from_json(cls: type[Self], json_str: str) -> Self:
         """Import an gaitmap object from its json representation.
 
         For details have a look at the this :ref:`example <algo_serialize>`.
 
         You can use the `to_json` method of a class to export it as a compatible json string.
 
         Parameters
@@ -225,21 +226,29 @@
 
 class BaseOrientationMethod(BaseAlgorithm):
     """Base class for the individual Orientation estimation methods that work on pd.DataFrame data."""
 
     _action_methods = ("estimate",)
     orientation_object_: Rotation
 
+    data: SingleSensorData
+    sampling_rate_hz: float
+
     @property
     def orientation_(self) -> SingleSensorOrientationList:
         """Orientations as pd.DataFrame."""
         df = pd.DataFrame(self.orientation_object_.as_quat(), columns=GF_ORI)
         df.index.name = "sample"
         return df
 
+    @property
+    def rotated_data_(self) -> SingleSensorData:
+        """Rotated data."""
+        return rotate_dataset_series(self.data, self.orientation_object_[:-1])
+
     def estimate(
         self,
         data: SingleSensorData,
         *,
         stride_event_list: Optional[SingleSensorStrideList] = None,
         sampling_rate_hz: float,
     ) -> Self:
```

### Comparing `gaitmap-2.3.0/gaitmap/data_transform/__init__.py` & `gaitmap-2.4.0/gaitmap/data_transform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Classes representing data transformations as preprocessing for different algorithms."""
+
 from gaitmap.data_transform._base import (
     BaseTransformer,
     ChainedTransformer,
     GroupedTransformer,
     IdentityTransformer,
     ParallelTransformer,
     TrainableTransformerMixin,
```

### Comparing `gaitmap-2.3.0/gaitmap/data_transform/_base.py` & `gaitmap-2.4.0/gaitmap/data_transform/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Basic transformers for higher level functionality."""
+
+from collections.abc import Sequence
 from copy import copy
 from functools import reduce
-from typing import List, Sequence, Set, Tuple, Union
+from typing import Union
 
 import pandas as pd
 from tpcp import OptimizableParameter, PureParameter
 from typing_extensions import Self
 
 from gaitmap.base import BaseAlgorithm
 from gaitmap.utils._types import _Hashable
@@ -85,24 +87,24 @@
     Other Parameters
     ----------------
     data
         The data passed to the transform method.
 
     """
 
-    transformer_mapping: OptimizableParameter[List[Tuple[Union[_Hashable, Tuple[_Hashable, ...]], BaseTransformer]]]
+    transformer_mapping: OptimizableParameter[list[tuple[Union[_Hashable, tuple[_Hashable, ...]], BaseTransformer]]]
     keep_all_cols: PureParameter[bool]
 
     data: SingleSensorData
 
     def __init__(
         self,
-        transformer_mapping: List[Tuple[Union[_Hashable, Tuple[_Hashable, ...]], BaseTransformer]],
+        transformer_mapping: list[tuple[Union[_Hashable, tuple[_Hashable, ...]], BaseTransformer]],
         keep_all_cols: bool = True,
-    ):
+    ) -> None:
         self.transformer_mapping = transformer_mapping
         self.keep_all_cols = keep_all_cols
 
     def self_optimize(self, data: Sequence[SingleSensorData], **kwargs) -> Self:
         """Train all trainable transformers based on the provided data.
 
         ... note :: All transformers will be trained on all columns they are applied to as group.
@@ -176,30 +178,30 @@
             # We clone here to make sure that we do not modify the "parameters" within the action method
             tmp = v.clone().transform(data[list(k)], **kwargs).transformed_data_
             for col in k:
                 results.append(tmp[[col]])
         self.transformed_data_ = pd.concat(results, axis=1)[sorted(mapped_cols, key=list(data.columns).index)]
         return self
 
-    def _validate_mapping(self) -> Set[_Hashable]:
+    def _validate_mapping(self) -> set[_Hashable]:
         # Check that each column is only mentioned once:
         unique_k = []
         for k, _ in self.transformer_mapping:
             if not isinstance(k, tuple):
                 k = (k,)
             for i in k:
                 if i in unique_k:
                     raise ValueError(
                         "Each column name must only be mentioned once in the keys of `scaler_mapping`."
                         "Applying multiple transformations to the same column is not supported."
                     )
                 unique_k.append(i)
         return set(unique_k)
 
-    def _validate(self, data: SingleSensorData, selected_cols: Set[_Hashable]):
+    def _validate(self, data: SingleSensorData, selected_cols: set[_Hashable]) -> None:
         if not set(data.columns).issuperset(selected_cols):
             raise ValueError("You specified transformations for columns that do not exist. This is not supported!")
 
 
 class ChainedTransformer(BaseTransformer, TrainableTransformerMixin):
     """Apply a series of transformations to the input.
 
@@ -232,17 +234,17 @@
     data
         The data passed to the transform method.
 
     """
 
     _composite_params = ("chain",)
 
-    chain: OptimizableParameter[List[Tuple[_Hashable, BaseTransformer]]]
+    chain: OptimizableParameter[list[tuple[_Hashable, BaseTransformer]]]
 
-    def __init__(self, chain: List[Tuple[_Hashable, BaseTransformer]]):
+    def __init__(self, chain: list[tuple[_Hashable, BaseTransformer]]) -> None:
         self.chain = chain
 
     def self_optimize(self, data: Sequence[SingleSensorData], **kwargs) -> Self:
         """Optimize the chained transformers.
 
         Parameters
         ----------
@@ -327,17 +329,17 @@
     data
         The data passed to the transform method.
 
     """
 
     _composite_params = ("transformers",)
 
-    transformers: OptimizableParameter[List[Tuple[_Hashable, BaseTransformer]]]
+    transformers: OptimizableParameter[list[tuple[_Hashable, BaseTransformer]]]
 
-    def __init__(self, transformers: List[Tuple[_Hashable, BaseTransformer]]):
+    def __init__(self, transformers: list[tuple[_Hashable, BaseTransformer]]) -> None:
         self.transformers = transformers
 
     def self_optimize(self, data: Sequence[SingleSensorData], **kwargs) -> Self:
         """Optimize all transformer.
 
         Each transformer's `self_optimize` method will be called individually with the data.
```

### Comparing `gaitmap-2.3.0/gaitmap/data_transform/_feature_transform.py` & `gaitmap-2.4.0/gaitmap/data_transform/_feature_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A set of transformers that can be used to calculate traditional features from a timeseries."""
+
 from copy import copy
-from typing import Optional
+from typing import NoReturn, Optional
 
 import numpy as np
 import pandas as pd
 from numpy import polyfit
 from pandas.core.window import Rolling
 from scipy import signal
 from typing_extensions import Self
@@ -51,15 +52,15 @@
     roi_list: SingleSensorRegionsOfInterestList
 
     transformed_roi_list_: SingleSensorRegionsOfInterestList
 
     def __init__(
         self,
         target_sampling_rate_hz: Optional[float] = None,
-    ):
+    ) -> None:
         self.target_sampling_rate_hz = target_sampling_rate_hz
 
     def transform(
         self,
         data: Optional[SingleSensorData] = None,
         *,
         roi_list: Optional[SingleSensorRegionsOfInterestList] = None,
@@ -125,15 +126,15 @@
 class BaseSlidingWindowFeatureTransform(BaseTransformer):
     """Baseclass for all Sliding window feature transforms."""
 
     window_size_s: Optional[float]
 
     sampling_rate_hz: float
 
-    def __init__(self, window_size_s: Optional[float] = None):
+    def __init__(self, window_size_s: Optional[float] = None) -> None:
         self.window_size_s = window_size_s
 
     @property
     def effective_window_size_samples_(self) -> int:
         """Get the real sample size of the window in samples after rounding effects."""
         win_size = int(np.round(self.sampling_rate_hz * self.window_size_s))
         if win_size % 2 == 0:
@@ -285,15 +286,15 @@
     else:
         raise ValueError("Only error of dim 1 or 2 can be turned into sliding windows with this method.")
 
     return sliding_window_view(array, window_size_samples, window_size_samples - 1).swapaxes(0, 1)
 
 
 class _CustomSlidingWindowTransform(BaseSlidingWindowFeatureTransform):
-    def _apply_to_window_view(self, windowed_view: np.ndarray, data: pd.DataFrame):
+    def _apply_to_window_view(self, windowed_view: np.ndarray, data: pd.DataFrame) -> NoReturn:
         raise NotImplementedError
 
     def _transform(self, data: SingleSensorData, sampling_rate_hz: float, **_) -> SingleSensorData:  # noqa: ARG002
         windowed_view = _get_centered_window_view(data.to_numpy(), self.effective_window_size_samples_, pad_value=0.0)
         # We pass the original data, so that the method can correctly create an output in form of a Dataframe
         return self._apply_to_window_view(windowed_view, data)
```

### Comparing `gaitmap-2.3.0/gaitmap/data_transform/_filter.py` & `gaitmap-2.4.0/gaitmap/data_transform/_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A set of filters that can be applied to data."""
-from typing import Literal, Optional, Tuple, Union
+
+from typing import Literal, Optional, Union
 
 import pandas as pd
 from scipy.signal import butter, sosfiltfilt
 from typing_extensions import Self
 
 from gaitmap.data_transform._base import BaseTransformer
 from gaitmap.utils.datatype_helper import SingleSensorData
@@ -18,17 +19,15 @@
     def filtered_data_(self) -> SingleSensorData:
         """Get filtered data.
 
         This is the same as `transformed_data_` and is just here, as it is easier to remember.
         """
         return self.transformed_data_
 
-    def filter(  # noqa: A003
-        self, data: SingleSensorData, *, sampling_rate_hz: Optional[float] = None, **kwargs
-    ) -> Self:
+    def filter(self, data: SingleSensorData, *, sampling_rate_hz: Optional[float] = None, **kwargs) -> Self:
         """Filter the data.
 
         This will apply the filter along the **first** axis (axis=0) (aka each column will be filtered).
 
         This is identical to the transform method, but is here for convenience, as it is more natural to type
         filter.filter() instead of filter.transform().
 
@@ -70,25 +69,25 @@
         The data passed to the filter/transform method
     sampling_rate_hz
         The sampling rate of the data
 
     """
 
     order: int
-    cutoff_freq_hz: Union[float, Tuple[float, float]]
+    cutoff_freq_hz: Union[float, tuple[float, float]]
     filter_type: Literal["lowpass", "highpass", "bandpass", "bandstop"]
 
     sampling_rate_hz: float
 
     def __init__(
         self,
         order: int,
-        cutoff_freq_hz: Union[float, Tuple[float, float]],
+        cutoff_freq_hz: Union[float, tuple[float, float]],
         filter_type: Literal["lowpass", "highpass", "bandpass", "bandstop"] = "lowpass",
-    ):
+    ) -> None:
         self.order = order
         self.cutoff_freq_hz = cutoff_freq_hz
         self.filter_type = filter_type
 
     def transform(self, data: SingleSensorData, *, sampling_rate_hz: Optional[float] = None, **_) -> Self:
         """Filter the data.
```

### Comparing `gaitmap-2.3.0/gaitmap/data_transform/_scaler.py` & `gaitmap-2.4.0/gaitmap/data_transform/_scaler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Transformers that scale data to certain data ranges."""
-from typing import Optional, Sequence, Tuple
+
+from collections.abc import Sequence
+from typing import Optional
 
 import numpy as np
 from tpcp import OptimizableParameter, Parameter
 from typing_extensions import Self
 
 from gaitmap.data_transform._base import BaseTransformer, TrainableTransformerMixin
 from gaitmap.utils.datatype_helper import SensorData, SingleSensorData, is_single_sensor_data
@@ -37,15 +39,15 @@
         The data passed to the transform method.
 
     """
 
     scale: Parameter[float]
     offset: Parameter[float]
 
-    def __init__(self, scale: float = 1, offset: float = 0):
+    def __init__(self, scale: float = 1, offset: float = 0) -> None:
         self.scale = scale
         self.offset = offset
 
     def transform(self, data: SingleSensorData, **_) -> Self:
         """Scale the data.
 
         Parameters
@@ -90,15 +92,15 @@
     data
         The data passed to the transform method.
 
     """
 
     ddof: Parameter[int] = 1
 
-    def __init__(self, ddof: int = 1):
+    def __init__(self, ddof: int = 1) -> None:
         self.ddof = ddof
 
     def transform(self, data: SingleSensorData, **_) -> Self:
         """Scale the data.
 
         Parameters
         ----------
@@ -146,15 +148,15 @@
         The data passed to the transform method.
 
     """
 
     mean: OptimizableParameter[Optional[float]]
     std: OptimizableParameter[Optional[float]]
 
-    def __init__(self, mean: Optional[float] = None, std: Optional[float] = None, ddof: int = 1):
+    def __init__(self, mean: Optional[float] = None, std: Optional[float] = None, ddof: int = 1) -> None:
         self.mean = mean
         self.std = std
         super().__init__(ddof=ddof)
 
     def self_optimize(self, data: Sequence[SingleSensorData], **_) -> Self:
         # Iteratively calculate the overall mean and std using a two-pass algorithm
         # First pass: Calculate the mean:
@@ -230,15 +232,15 @@
     data
         The data passed to the transform method.
 
     """
 
     out_max: Parameter[float]
 
-    def __init__(self, out_max: float = 1):
+    def __init__(self, out_max: float = 1) -> None:
         self.out_max = out_max
 
     def transform(self, data: SingleSensorData, **_) -> Self:
         """Scale the data.
 
         Parameters
         ----------
@@ -309,15 +311,15 @@
     data
         The data passed to the transform method.
 
     """
 
     data_max: OptimizableParameter[Optional[float]]
 
-    def __init__(self, out_max: float = 1, data_max: Optional[float] = None):
+    def __init__(self, out_max: float = 1, data_max: Optional[float] = None) -> None:
         self.data_max = data_max
         super().__init__(out_max=out_max)
 
     def self_optimize(self, data: Sequence[SingleSensorData], **_) -> Self:
         """Calculate scaling parameters based on a trainings sequence.
 
         Parameters
@@ -385,20 +387,20 @@
     Other Parameters
     ----------------
     data
         The data passed to the transform method.
 
     """
 
-    out_range: Parameter[Tuple[float, float]]
+    out_range: Parameter[tuple[float, float]]
 
     def __init__(
         self,
-        out_range: Tuple[float, float] = (0, 1.0),
-    ):
+        out_range: tuple[float, float] = (0, 1.0),
+    ) -> None:
         self.out_range = out_range
 
     def transform(self, data: SingleSensorData, **_) -> Self:
         """Scale the data.
 
         Parameters
         ----------
@@ -415,21 +417,21 @@
         # Test if out data range is valid
         if self.out_range[0] >= self.out_range[1]:
             raise ValueError("out_range[0] (new min) must be smaller than out_range[1] (new max)")
         data_range = self._calc_data_range(data)
         self.transformed_data_ = self._transform(data, data_range)
         return self
 
-    def _calc_data_range(self, data: SensorData) -> Tuple[float, float]:
+    def _calc_data_range(self, data: SensorData) -> tuple[float, float]:
         is_single_sensor_data(data, check_gyr=False, check_acc=False, raise_exception=True)
         # We calculate the global min and max over all rows and columns!
         data = data.to_numpy()
         return float(np.nanmin(data)), float(np.nanmax(data))
 
-    def _transform(self, data: SingleSensorData, data_range: Tuple[float, float]) -> SingleSensorData:
+    def _transform(self, data: SingleSensorData, data_range: tuple[float, float]) -> SingleSensorData:
         data = data.copy()
         feature_range = self.out_range
         data_min, data_max = data_range
         transform_range = (data_max - data_min) or 1.0
         transform_scale = (feature_range[1] - feature_range[0]) / transform_range
         transform_min = feature_range[0] - data_min * transform_scale
 
@@ -478,21 +480,21 @@
     Other Parameters
     ----------------
     data
         The data passed to the transform method.
 
     """
 
-    data_range: OptimizableParameter[Optional[Tuple[float, float]]]
+    data_range: OptimizableParameter[Optional[tuple[float, float]]]
 
     def __init__(
         self,
-        out_range: Tuple[float, float] = (0, 1.0),
-        data_range: Optional[Tuple[float, float]] = None,
-    ):
+        out_range: tuple[float, float] = (0, 1.0),
+        data_range: Optional[tuple[float, float]] = None,
+    ) -> None:
         self.data_range = data_range
         super().__init__(out_range=out_range)
 
     def self_optimize(self, data: Sequence[SingleSensorData], **_):
         """Calculate scaling parameters based on a trainings sequence.
 
         Parameters
```

### Comparing `gaitmap-2.3.0/gaitmap/evaluation_utils/__init__.py` & `gaitmap-2.4.0/gaitmap/evaluation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.3.0/gaitmap/evaluation_utils/event_detection.py` & `gaitmap-2.4.0/gaitmap/evaluation_utils/event_detection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A set of helper functions to evaluate the output of an event stride segmentation against ground truth."""
 
-from typing import Dict, Union
+from typing import Union
 
 from pandas import DataFrame
 from typing_extensions import Literal
 
 from gaitmap.evaluation_utils.stride_segmentation import _evaluate_stride_list
 from gaitmap.utils._types import _Hashable
 from gaitmap.utils.datatype_helper import StrideList
@@ -15,15 +15,15 @@
     ground_truth: StrideList,
     stride_event_list: StrideList,
     match_cols: Literal["pre_ic", "ic", "min_vel", "tc"],
     tolerance: Union[int, float] = 0,
     one_to_one: bool = True,
     stride_list_postfix: str = "",
     ground_truth_postfix: str = "_ground_truth",
-) -> Union[DataFrame, Dict[_Hashable, DataFrame]]:
+) -> Union[DataFrame, dict[_Hashable, DataFrame]]:
     """Find True Positives, False Positives and True Negatives by comparing an stride event list with ground truth.
 
     This compares a stride event list with a ground truth stride event list and returns True Positives,
     False Positives and True Negatives matches.
     The comparison is based on the chosen column ("pre_ic", "ic", "min_vel", or "tc").
     Two strides are considered a positive match, if the selected event differs by less than the
     threshold.
@@ -72,56 +72,45 @@
         All ground truth strides that do not have a counterpart are marked as "fn" (false negative).
         In case MultiSensorStrideLists were used as inputs, a dictionary of such dataframes is returned.
 
 
     Examples
     --------
     >>> stride_list_ground_truth = DataFrame(
-    ...     [[10,21, 10],[20,34, 30],[31,40, 20]],
-    ...     columns=["start", "end", "ic"]
-    ... ).rename_axis('s_id')
+    ...     [[10, 21, 10], [20, 34, 30], [31, 40, 20]], columns=["start", "end", "ic"]
+    ... ).rename_axis("s_id")
     >>> stride_list_seg = DataFrame(
-    ...     [[10,20, 10],[21,30, 30],[31,40, 22]],
-    ...     columns=["start", "end", "ic"]
-    ... ).rename_axis('s_id')
+    ...     [[10, 20, 10], [21, 30, 30], [31, 40, 22]], columns=["start", "end", "ic"]
+    ... ).rename_axis("s_id")
     >>> matches = evaluate_stride_event_list(
-    ...     ground_truth=stride_list_ground_truth,
-    ...     stride_event_list=stride_list_seg,
-    ...     match_cols="ic",
-    ...     tolerance=3
+    ...     ground_truth=stride_list_ground_truth, stride_event_list=stride_list_seg, match_cols="ic", tolerance=3
     ... )
     >>> matches
        s_id  s_id_ground_truth match_type
     0     0                  0         tp
     1     1                  1         tp
     2     2                  2         tp
 
     >>> stride_list_ground_truth_left = DataFrame(
-    ...     [[10,21,30],[20,34,20],[31,40,10], [10, 30 ,60]],
-    ...     columns=["start", "end", "ic"]
-    ... ).rename_axis('s_id')
+    ...     [[10, 21, 30], [20, 34, 20], [31, 40, 10], [10, 30, 60]], columns=["start", "end", "ic"]
+    ... ).rename_axis("s_id")
     >>> stride_list_ground_truth_right = DataFrame(
-    ...     [[10,21,1],[20,34,2],[31,40,3]],
-    ...     columns=["start", "end", "ic"]
-    ... ).rename_axis('s_id')
-    ...
+    ...     [[10, 21, 1], [20, 34, 2], [31, 40, 3]], columns=["start", "end", "ic"]
+    ... ).rename_axis("s_id")
     >>> stride_list_seg_left = DataFrame(
-    ...     [[10,20, 30],[21,30,20],[31,40,13]],
-    ...     columns=["start", "end", "ic"]
-    ... ).rename_axis('s_id')
+    ...     [[10, 20, 30], [21, 30, 20], [31, 40, 13]], columns=["start", "end", "ic"]
+    ... ).rename_axis("s_id")
     >>> stride_list_seg_right = DataFrame(
-    ...     [[10,21, 1],[20,34, 2],[31,40, 3]],
-    ...     columns=["start", "end", "ic"]
-    ... ).rename_axis('s_id')
-    ...
+    ...     [[10, 21, 1], [20, 34, 2], [31, 40, 3]], columns=["start", "end", "ic"]
+    ... ).rename_axis("s_id")
     >>> matches_multi = evaluate_stride_event_list(
     ...     ground_truth={"left_sensor": stride_list_ground_truth_left, "right_sensor": stride_list_ground_truth_right},
     ...     stride_event_list={"left_sensor": stride_list_seg_left, "right_sensor": stride_list_seg_right},
     ...     match_cols="ic",
-    ...     tolerance=2
+    ...     tolerance=2,
     ... )
     >>> matches_multi["left_sensor"]
       s_id s_id_ground_truth match_type
     0    0                 0         tp
     1    1                 1         tp
     2    2               NaN         fp
     3  NaN                 2         fn
```

### Comparing `gaitmap-2.3.0/gaitmap/evaluation_utils/parameter_errors.py` & `gaitmap-2.4.0/gaitmap/evaluation_utils/parameter_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """A helper function to evaluate the output of the temporal or spatial parameter calculation against a ground truth."""
+
 import warnings
-from typing import Dict, Literal, Tuple, Union
+from typing import Literal, Union
 
 import numpy as np
 import pandas as pd
 
 from gaitmap.utils._types import _Hashable
 from gaitmap.utils.datatype_helper import set_correct_index
 from gaitmap.utils.exceptions import ValidationError
 
 _ID_COL_NAME = "__id_col__"
 
 
 def calculate_parameter_errors(
     *,
-    reference_parameter: Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]],
-    predicted_parameter: Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]],
+    reference_parameter: Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]],
+    predicted_parameter: Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]],
     id_column: str = "s_id",
-) -> Tuple[Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]], Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]]]:
+) -> tuple[Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]], Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]]]:
     """Calculate the error per row between a parameter predicted and a given ground truth.
 
     We calculate four different groups of errors:
 
         - The error between the predicted and the reference value (`predicted - reference`)
         - The relative error between the predicted and the reference value (`(predicted - reference) / reference`)
         - The absolute error between the predicted and the reference value (`abs(predicted - reference)`)
@@ -91,16 +92,16 @@
         common_rows = common_rows["__dummy__"]
 
     return output, common_rows
 
 
 def calculate_aggregated_parameter_errors(
     *,
-    reference_parameter: Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]],
-    predicted_parameter: Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]],
+    reference_parameter: Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]],
+    predicted_parameter: Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]],
     calculate_per_sensor: bool = True,
     scoring_errors: Literal["ignore", "warn", "raise"] = "warn",
     id_column: str = "s_id",
 ) -> pd.DataFrame:
     """Calculate various error metrics between a parameter predicted and a given ground truth.
 
     This method can be applied to stride level parameters or aggregated parameters over a gait test/participant/... .
@@ -246,15 +247,14 @@
     icc_q95                   0.920000   0.940000
     n_common                  4.000000   4.000000
     n_additional_reference    0.000000   0.000000
     n_additional_predicted    0.000000   0.000000
 
     >>> pd.set_option("display.max_columns", None)
     >>> pd.set_option("display.width", 0)
-    ...
     >>> predicted_sensor_left = pd.DataFrame(columns=["para"], data=[23, 82, 42]).rename_axis("s_id")
     >>> reference_sensor_left = pd.DataFrame(columns=["para"], data=[21, 86, 65]).rename_axis("s_id")
     >>> predicted_sensor_right = pd.DataFrame(columns=["para"], data=[26, -58, -3]).rename_axis("s_id")
     >>> reference_sensor_right = pd.DataFrame(columns=["para"], data=[96, -78, 86]).rename_axis("s_id")
     >>> calculate_aggregated_parameter_errors(
     ...     predicted_parameter={"left_sensor": predicted_sensor_left, "right_sensor": predicted_sensor_right},
     ...     reference_parameter={"left_sensor": reference_sensor_left, "right_sensor": reference_sensor_right},
@@ -322,15 +322,15 @@
     n_additional_predicted     0.000000     0.000000
     n_additional_reference     0.000000     0.000000
     n_common                   3.000000     3.000000
 
     >>> calculate_aggregated_parameter_errors(
     ...     predicted_parameter={"left_sensor": predicted_sensor_left, "right_sensor": predicted_sensor_right},
     ...     reference_parameter={"left_sensor": reference_sensor_left, "right_sensor": reference_sensor_right},
-    ...     calculate_per_sensor=False
+    ...     calculate_per_sensor=False,
     ... )  # doctest: +NORMALIZE_WHITESPACE
                                    para
     predicted_mean            18.666667
     reference_mean            46.000000
     error_mean               -27.333333
     abs_error_mean            34.666667
     rel_error_mean            -0.387597
@@ -492,15 +492,15 @@
             raise ValidationError(err_msg_start + "common entries are found between predicted and reference!")
 
         aligned_dict[sensor] = aligned
 
     return aligned_dict, meta_error_dict
 
 
-def _calculate_error(aligned_parameters: Dict[_Hashable, pd.DataFrame]) -> Dict[_Hashable, pd.DataFrame]:
+def _calculate_error(aligned_parameters: dict[_Hashable, pd.DataFrame]) -> dict[_Hashable, pd.DataFrame]:
     """Calculate the error between a reference and a predicted parameter."""
     final_error_dict = {}
     for k, v in aligned_parameters.items():
         error_dict = {
             "predicted": v["predicted"],
             "reference": v["reference"],
             "error": v["predicted"] - v["reference"],
@@ -564,15 +564,15 @@
 
     assert set(data.columns.get_level_values("error_type")) == {"predicted", "reference"}
     # If it is not unique, the ICC calculation will fail.
     assert data.index.is_unique
 
     paras = data.columns.get_level_values("parameter").unique()
     data = data.stack("error_type").reset_index()
-    coefs: Dict[str, pd.Series] = {}
+    coefs: dict[str, pd.Series] = {}
     for para in paras:
         try:
             # If handle error is ignore, we also ignore all warnings here.
             with warnings.catch_warnings():
                 if scoring_errors == "ignore":
                     warnings.simplefilter("ignore")
                 icc, ci95 = pg.intraclass_corr(
```

### Comparing `gaitmap-2.3.0/gaitmap/evaluation_utils/scores.py` & `gaitmap-2.4.0/gaitmap/evaluation_utils/scores.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """A set of helper functions to score the output of the evaluation of a stride segmentation against ground truth."""
+
 import warnings
-from typing import Dict, Union, overload
+from typing import Union, overload
 
 import pandas as pd
 from typing_extensions import Literal, TypedDict
 
 from gaitmap.utils._types import _Hashable
 from gaitmap.utils.datatype_helper import get_multi_sensor_names
 
-_ScoresDict = TypedDict("_ScoresDict", {"precision": float, "recall": float, "f1_score": float})
+
+class _ScoresDict(TypedDict):
+    precision: float
+    recall: float
+    f1_score: float
 
 
 @overload
 def recall_score(
-    matches_df: Dict[_Hashable, pd.DataFrame], *, zero_division: Literal["warn", 0, 1] = "warn"
-) -> Dict[_Hashable, float]:
-    ...
+    matches_df: dict[_Hashable, pd.DataFrame], *, zero_division: Literal["warn", 0, 1] = "warn"
+) -> dict[_Hashable, float]: ...
 
 
 @overload
-def recall_score(matches_df: pd.DataFrame, *, zero_division: Literal["warn", 0, 1] = "warn") -> float:
-    ...
+def recall_score(matches_df: pd.DataFrame, *, zero_division: Literal["warn", 0, 1] = "warn") -> float: ...
 
 
 def recall_score(matches_df, *, zero_division: Literal["warn", 0, 1] = "warn"):
     """Compute the recall.
 
     The recall is the ratio tp / (tp + fn) where tp is the number of true positives and fn the number of false
     negatives. The recall is intuitively the ability of the classifier to find all the positive samples.
@@ -71,22 +74,20 @@
     if is_not_dict:
         return output["__dummy__"]
     return output
 
 
 @overload
 def precision_score(
-    matches_df: Dict[_Hashable, pd.DataFrame], *, zero_division: Literal["warn", 0, 1] = "warn"
-) -> Dict[_Hashable, float]:
-    ...
+    matches_df: dict[_Hashable, pd.DataFrame], *, zero_division: Literal["warn", 0, 1] = "warn"
+) -> dict[_Hashable, float]: ...
 
 
 @overload
-def precision_score(matches_df: pd.DataFrame, *, zero_division: Literal["warn", 0, 1] = "warn") -> float:
-    ...
+def precision_score(matches_df: pd.DataFrame, *, zero_division: Literal["warn", 0, 1] = "warn") -> float: ...
 
 
 def precision_score(matches_df, *, zero_division: Literal["warn", 0, 1] = "warn"):
     """Compute the precision.
 
     The precision is the ratio tp / (tp + fp) where tp is the number of true positives and fp the number of false
     positives. The precision is intuitively the ability of the classifier not to label as positive a sample that is
@@ -135,22 +136,20 @@
     if is_not_dict:
         return output["__dummy__"]
     return output
 
 
 @overload
 def f1_score(
-    matches_df: Dict[_Hashable, pd.DataFrame], *, zero_division: Literal["warn", 0, 1] = "warn"
-) -> Dict[_Hashable, float]:
-    ...
+    matches_df: dict[_Hashable, pd.DataFrame], *, zero_division: Literal["warn", 0, 1] = "warn"
+) -> dict[_Hashable, float]: ...
 
 
 @overload
-def f1_score(matches_df: pd.DataFrame, *, zero_division: Literal["warn", 0, 1] = "warn") -> float:
-    ...
+def f1_score(matches_df: pd.DataFrame, *, zero_division: Literal["warn", 0, 1] = "warn") -> float: ...
 
 
 def f1_score(matches_df, *, zero_division: Literal["warn", 0, 1] = "warn"):
     """Compute the F1 score, also known as balanced F-score or F-measure.
 
     The F1 score can be interpreted as the harmonic mean of precision and recall, where an F1 score reaches its
     best value at 1 and worst score at 0.
@@ -200,24 +199,22 @@
     if is_not_dict:
         return output["__dummy__"]
     return output
 
 
 @overload
 def precision_recall_f1_score(
-    matches_df: Dict[str, pd.DataFrame], *, zero_division: Literal["warn", 0, 1] = "warn"
-) -> Dict[str, _ScoresDict]:
-    ...
+    matches_df: dict[str, pd.DataFrame], *, zero_division: Literal["warn", 0, 1] = "warn"
+) -> dict[str, _ScoresDict]: ...
 
 
 @overload
 def precision_recall_f1_score(
     matches_df: pd.DataFrame, *, zero_division: Literal["warn", 0, 1] = "warn"
-) -> _ScoresDict:
-    ...
+) -> _ScoresDict: ...
 
 
 def precision_recall_f1_score(matches_df, *, zero_division: Literal["warn", 0, 1] = "warn"):
     """Compute precision, recall and F1-score.
 
     The precision is the ratio tp / (tp + fp) where tp is the number of true positives and fp the number of false
     positives. The precision is intuitively the ability of the classifier not to label as positive a sample that is
@@ -272,16 +269,16 @@
         "precision": precisions,
         "recall": recalls,
         "f1_score": f1_scores,
     }
 
 
 def _get_match_type_dfs(
-    match_results: Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]]
-) -> Union[Dict[_Hashable, Dict[str, pd.DataFrame]], Dict[str, pd.DataFrame]]:
+    match_results: Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]],
+) -> Union[dict[_Hashable, dict[str, pd.DataFrame]], dict[str, pd.DataFrame]]:
     is_not_dict = not isinstance(match_results, dict)
     if is_not_dict:
         match_results = {"__dummy__": match_results}
 
     for dataframe_name in get_multi_sensor_names(match_results):
         matches_types = match_results[dataframe_name].groupby("match_type")
         matches_types_dict = {}
```

### Comparing `gaitmap-2.3.0/gaitmap/evaluation_utils/stride_segmentation.py` & `gaitmap-2.4.0/gaitmap/evaluation_utils/stride_segmentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A set of helper functions to evaluate the output of a stride segmentation against ground truth."""
 
-from typing import Dict, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from scipy.spatial import KDTree, minkowski_distance
 
 from gaitmap.utils._types import _Hashable
 from gaitmap.utils.consts import SL_INDEX
@@ -22,15 +23,15 @@
     *,
     ground_truth: StrideList,
     segmented_stride_list: StrideList,
     tolerance: Union[int, float] = 0,
     one_to_one: bool = True,
     stride_list_postfix: str = "",
     ground_truth_postfix: str = "_ground_truth",
-) -> Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]]:
+) -> Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]]:
     """Find True Positives, False Positives and True Negatives by comparing a segmented stride list with ground truth.
 
     This compares a segmented stride list with a ground truth segmented stride list and returns True Positives,
     False Positives and True Negatives matches.
     The comparison is purely based on the start and end values of each stride in the lists.
     Two strides are considered a positive match, if both their start and their end values differ by less than the
     threshold.
@@ -78,48 +79,47 @@
         positives)
         All ground truth strides that do not have a segmented counterpart are marked as "fn" (false negative).
         In case MultiSensorStrideLists were used as inputs, a dictionary of such dataframes is returned.
 
 
     Examples
     --------
-    >>> stride_list_ground_truth = pd.DataFrame([[10,21],[20,34],[31,40]], columns=["start", "end"]).rename_axis('s_id')
-    >>> stride_list_seg = pd.DataFrame([[10,20],[21,30],[31,40],[50,60]], columns=["start", "end"]).rename_axis('s_id')
+    >>> stride_list_ground_truth = pd.DataFrame([[10, 21], [20, 34], [31, 40]], columns=["start", "end"]).rename_axis(
+    ...     "s_id"
+    ... )
+    >>> stride_list_seg = pd.DataFrame([[10, 20], [21, 30], [31, 40], [50, 60]], columns=["start", "end"]).rename_axis(
+    ...     "s_id"
+    ... )
     >>> matches = evaluate_segmented_stride_list(
-    ...     ground_truth=stride_list_ground_truth,
-    ...     segmented_stride_list=stride_list_seg,
-    ...     tolerance=2
+    ...     ground_truth=stride_list_ground_truth, segmented_stride_list=stride_list_seg, tolerance=2
     ... )
     >>> matches
       s_id s_id_ground_truth match_type
     0    0                 0         tp
     1    1               NaN         fp
     2    2                 2         tp
     3    3               NaN         fp
     4  NaN                 1         fn
 
     >>> stride_list_ground_truth_left = pd.DataFrame(
-    ...     [[10,21],[20,34],[31,40]],
-    ...     columns=["start", "end"]
-    ... ).rename_axis('s_id')
+    ...     [[10, 21], [20, 34], [31, 40]], columns=["start", "end"]
+    ... ).rename_axis("s_id")
     >>> stride_list_ground_truth_right = pd.DataFrame(
-    ...     [[10,21],[20,34],[31,40]],
-    ...     columns=["start", "end"]
-    ... ).rename_axis('s_id')
-    ...
+    ...     [[10, 21], [20, 34], [31, 40]], columns=["start", "end"]
+    ... ).rename_axis("s_id")
     >>> stride_list_seg_left = pd.DataFrame(
-    ...     [[10,20],[21,30],[31,40],[50,60]],
-    ...     columns=["start", "end"]
-    ... ).rename_axis('s_id')
-    >>> stride_list_seg_right = pd.DataFrame([[10,21],[20,34],[31,40]], columns=["start", "end"]).rename_axis('s_id')
-    ...
+    ...     [[10, 20], [21, 30], [31, 40], [50, 60]], columns=["start", "end"]
+    ... ).rename_axis("s_id")
+    >>> stride_list_seg_right = pd.DataFrame([[10, 21], [20, 34], [31, 40]], columns=["start", "end"]).rename_axis(
+    ...     "s_id"
+    ... )
     >>> matches = evaluate_segmented_stride_list(
     ...     ground_truth={"left_sensor": stride_list_ground_truth_left, "right_sensor": stride_list_ground_truth_right},
     ...     segmented_stride_list={"left_sensor": stride_list_seg_left, "right_sensor": stride_list_seg_right},
-    ...     tolerance=2
+    ...     tolerance=2,
     ... )
     >>> matches["left_sensor"]
       s_id s_id_ground_truth match_type
     0    0                 0         tp
     1    1               NaN         fp
     2    2                 2         tp
     3    3               NaN         fp
@@ -145,15 +145,15 @@
     ground_truth: StrideList,
     segmented_stride_list: StrideList,
     match_cols: Union[str, Sequence[str]] = ("start", "end"),
     tolerance: Union[int, float] = 0,
     one_to_one: bool = True,
     stride_list_postfix: str = "",
     ground_truth_postfix: str = "_ground_truth",
-) -> Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]]:
+) -> Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]]:
     segmented_stride_list_type = is_stride_list(segmented_stride_list)
     ground_truth_type = is_stride_list(ground_truth)
 
     if ground_truth_type != segmented_stride_list_type:
         raise ValidationError("The inputted lists are of not of same type")
 
     is_single = segmented_stride_list_type == "single"
@@ -192,15 +192,15 @@
     stride_list_a: StrideList,
     stride_list_b: StrideList,
     match_cols: Union[str, Sequence[str]] = ("start", "end"),
     tolerance: Union[int, float] = 0,
     one_to_one: bool = True,
     postfix_a: str = "_a",
     postfix_b: str = "_b",
-) -> Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]]:
+) -> Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]]:
     """Find matching strides in two stride lists with a certain tolerance.
 
     This function will find matching strides in two stride lists as long as all selected columns/event of a stride
     and its matching stride differ by less than the selected tolerance.
     This can be helpful to compare the result of a segmentation or event detection to a ground truth.
     In case both stride lists are multi-sensor stride lists, matching will be performed between all common sensors of
     the stride lists.
@@ -247,48 +247,50 @@
         The list is sorted by the index values of the left stride list.
         In case MultiSensorStrideLists were used as inputs, a dictionary of such values are returned.
 
     Examples
     --------
     Single Sensor:
 
-    >>> stride_list_left = pd.DataFrame([[10,20],[21,30],[31,40],[50,60]], columns=["start", "end"]).rename_axis('s_id')
-    >>> stride_list_right = pd.DataFrame([[10,21],[20,34],[31,40]], columns=["start", "end"]).rename_axis('s_id')
+    >>> stride_list_left = pd.DataFrame([[10, 20], [21, 30], [31, 40], [50, 60]], columns=["start", "end"]).rename_axis(
+    ...     "s_id"
+    ... )
+    >>> stride_list_right = pd.DataFrame([[10, 21], [20, 34], [31, 40]], columns=["start", "end"]).rename_axis("s_id")
     >>> match_stride_lists(
     ...     stride_list_a=stride_list_left,
     ...     stride_list_b=stride_list_right,
     ...     tolerance=2,
     ...     postfix_a="_left",
-    ...     postfix_b="_right"
+    ...     postfix_b="_right",
     ... )
       s_id_left s_id_right
     0         0          0
     1         1        NaN
     2         2          2
     3         3        NaN
     4       NaN          1
 
     Multi Sensor:
 
     >>> stride_list_left_11 = pd.DataFrame(
-    ...     [[10,20],[21,30],[31,40],[50,60]],
-    ...     columns=["start", "end"]
-    ... ).rename_axis('s_id')
-    >>> stride_list_right_12 = pd.DataFrame([[10,21],[20,34],[31,40]], columns=["start", "end"]).rename_axis('s_id')
-    ...
+    ...     [[10, 20], [21, 30], [31, 40], [50, 60]], columns=["start", "end"]
+    ... ).rename_axis("s_id")
+    >>> stride_list_right_12 = pd.DataFrame([[10, 21], [20, 34], [31, 40]], columns=["start", "end"]).rename_axis(
+    ...     "s_id"
+    ... )
     >>> stride_list_left_21 = pd.DataFrame(
-    ...     [[10,20],[31,41],[21,31],[50,60]],
-    ...     columns=["start", "end"]
-    ... ).rename_axis('s_id')
-    >>> stride_list_right_22 = pd.DataFrame([[10,22],[31, 41],[20, 36]], columns=["start", "end"]).rename_axis('s_id')
-    ...
+    ...     [[10, 20], [31, 41], [21, 31], [50, 60]], columns=["start", "end"]
+    ... ).rename_axis("s_id")
+    >>> stride_list_right_22 = pd.DataFrame([[10, 22], [31, 41], [20, 36]], columns=["start", "end"]).rename_axis(
+    ...     "s_id"
+    ... )
     >>> test_output = match_stride_lists(
     ...     stride_list_a={"left_sensor": stride_list_left_11, "right_sensor": stride_list_right_12},
     ...     stride_list_b={"left_sensor": stride_list_left_21, "right_sensor": stride_list_right_22},
-    ...     tolerance=1
+    ...     tolerance=1,
     ... )
     >>> test_output["left_sensor"]
        s_id_a  s_id_b
     0       0       0
     1       1       2
     2       2       1
     3       3       3
@@ -314,15 +316,15 @@
     stride_list_a: StrideList,
     stride_list_b: StrideList,
     match_cols: Union[str, Sequence[str]],
     tolerance: Union[int, float] = 0,
     one_to_one: bool = True,
     postfix_a: str = "_a",
     postfix_b: str = "_b",
-) -> Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]]:
+) -> Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]]:
     if postfix_a == postfix_b:
         raise ValueError("The postfix for the left and the right stride list must be different.")
 
     if tolerance < 0:
         raise ValueError("The tolerance must be larger 0.")
 
     match_cols = [match_cols] if isinstance(match_cols, str) else list(match_cols)
@@ -373,17 +375,15 @@
     tolerance: Union[int, float] = 0,
     one_to_one: bool = True,
     postfix_a: str = "_a",
     postfix_b: str = "_b",
 ) -> pd.DataFrame:
     if not (set(match_cols).issubset(stride_list_a.columns) and set(match_cols).issubset(stride_list_b.columns)):
         raise ValueError(
-            "One or more selected columns ({}) are missing in at least one of the provided stride lists".format(
-                match_cols
-            )
+            f"One or more selected columns ({match_cols}) are missing in at least one of the provided stride lists"
         )
     stride_list_a = set_correct_index(stride_list_a, SL_INDEX)
     stride_list_b = set_correct_index(stride_list_b, SL_INDEX)
 
     left_indices, right_indices = _match_label_lists(
         stride_list_a[match_cols].to_numpy(),
         stride_list_b[match_cols].to_numpy(),
@@ -417,15 +417,15 @@
     )
 
     return matches
 
 
 def _match_label_lists(
     list_left: np.ndarray, list_right: np.ndarray, tolerance: Union[int, float], one_to_one: bool
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Find matches in two lists based on the distance between their vectors.
 
     Parameters
     ----------
     list_left : array with shape (n, d)
         An n long array of d-dimensional vectors
     list_right : array with shape (m, d)
```

### Comparing `gaitmap-2.3.0/gaitmap/event_detection/__init__.py` & `gaitmap-2.4.0/gaitmap/event_detection/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The :py:mod:`gaitmap.event_detection` contains algorithms to detect temporal gait events in the sensor signal.
 
 Different algorithms for event detection are going to be collected here.
 """
+
 from gaitmap.event_detection._herzer_event_detection import HerzerEventDetection
 from gaitmap.utils._gaitmap_mad import patch_gaitmap_mad_import
 
 _gaitmap_mad_modules = {"RamppEventDetection", "FilteredRamppEventDetection"}
 
 if not (__getattr__ := patch_gaitmap_mad_import(_gaitmap_mad_modules, __name__)):
     del __getattr__
```

### Comparing `gaitmap-2.3.0/gaitmap/event_detection/_herzer_event_detection.py` & `gaitmap-2.4.0/gaitmap/event_detection/_herzer_event_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """An event detection algorithm optimized for stair ambulation developed by Liv Herzer in her Bachelor Thesis ."""
-from typing import Callable, Dict, Optional, Tuple, Union
+
+from typing import Callable, Optional, Union
 
 import numpy as np
 import pandas as pd
 from joblib import Memory
 from scipy import signal
 from tpcp import cf
 
@@ -178,37 +179,37 @@
        Real-Life Situations: Repeated Measures From Healthy Subjects," in IEEE Transactions on Neural Systems and
        Rehabilitation Engineering, vol. 26, no. 10, pp. 1945-1956, Oct. 2018, doi: 10.1109/TNSRE.2018.2868094.
     .. [3] https://www.mad.tf.fau.de/person/liv-herzer-2/
 
     """
 
     min_vel_search_win_size_ms: float
-    mid_swing_peak_prominence: Union[Tuple[float, float], float]
+    mid_swing_peak_prominence: Union[tuple[float, float], float]
     mid_swing_n_considered_peaks: int
     ic_lowpass_filter: BaseFilter
     memory: Optional[Memory]
     enforce_consistency: bool
 
     def __init__(
         self,
         min_vel_search_win_size_ms: float = 100,
-        mid_swing_peak_prominence: Union[Tuple[float, float], float] = 20,
+        mid_swing_peak_prominence: Union[tuple[float, float], float] = 20,
         mid_swing_n_considered_peaks: int = 3,
         ic_lowpass_filter: BaseFilter = cf(ButterworthFilter(order=1, cutoff_freq_hz=4)),
         memory: Optional[Memory] = None,
         enforce_consistency: bool = True,
-        detect_only: Optional[Tuple[str, ...]] = None,
-    ):
+        detect_only: Optional[tuple[str, ...]] = None,
+    ) -> None:
         self.min_vel_search_win_size_ms = min_vel_search_win_size_ms
         self.mid_swing_peak_prominence = mid_swing_peak_prominence
         self.mid_swing_n_considered_peaks = mid_swing_n_considered_peaks
         self.ic_lowpass_filter = ic_lowpass_filter
         super().__init__(memory=memory, enforce_consistency=enforce_consistency, detect_only=detect_only)
 
-    def _get_detect_kwargs(self) -> Dict[str, int]:
+    def _get_detect_kwargs(self) -> dict[str, int]:
         min_vel_search_win_size = int(self.min_vel_search_win_size_ms / 1000 * self.sampling_rate_hz)
         return {
             "min_vel_search_win_size": min_vel_search_win_size,
             "mid_swing_peak_prominence": self.mid_swing_peak_prominence,
             "mid_swing_n_considered_peaks": self.mid_swing_n_considered_peaks,
             "sampling_rate_hz": self.sampling_rate_hz,
             "ic_lowpass_filter": self.ic_lowpass_filter,
@@ -223,21 +224,21 @@
 
 
 def _find_all_events(
     gyr: pd.DataFrame,
     acc: pd.DataFrame,
     stride_list: pd.DataFrame,
     *,
-    events: Tuple[str, ...] = ("ic", "tc", "min_vel"),
+    events: tuple[str, ...] = ("ic", "tc", "min_vel"),
     min_vel_search_win_size: int,
-    mid_swing_peak_prominence: Union[Tuple[float, float], float],
+    mid_swing_peak_prominence: Union[tuple[float, float], float],
     mid_swing_n_considered_peaks: int,
     ic_lowpass_filter: BaseFilter,
     sampling_rate_hz: float,
-) -> Tuple[Optional[np.ndarray], Optional[np.ndarray], Optional[np.ndarray]]:
+) -> tuple[Optional[np.ndarray], Optional[np.ndarray], Optional[np.ndarray]]:
     """Find events in provided data by looping over single strides."""
     gyr_ml = gyr["gyr_ml"].to_numpy()
     gyr = gyr.to_numpy()
     # inverting acc, as this algorithm was developed assuming a flipped axis like the original Rampp algorithm
     acc_pa = -acc["acc_pa"].to_numpy()
     ic_events = []
     tc_events = []
@@ -275,15 +276,15 @@
     return (
         np.array(ic_events, dtype=float) if ic_events else None,
         np.array(tc_events, dtype=float) if tc_events else None,
         np.array(min_vel_events, dtype=float) if min_vel_events else None,
     )
 
 
-def _get_midswing_max(gyr_ml, peak_prominence_thresholds: Union[Tuple[float, float], float], n_considered_peaks: int):
+def _get_midswing_max(gyr_ml, peak_prominence_thresholds: Union[tuple[float, float], float], n_considered_peaks: int):
     """Return the first prominent maximum within the given stride.
 
     This maximum should correspond to the mid swing gait event.
     """
     peaks, properties = signal.find_peaks(gyr_ml, prominence=peak_prominence_thresholds, height=0)
     if len(peaks) == 0:
         return np.nan
@@ -294,15 +295,15 @@
     return peak
 
 
 def _detect_ic(
     gyr_ml: np.ndarray,
     acc_pa_inv: np.ndarray,
     gyr_ml_grad: np.ndarray,
-    peak_prominence_thresholds: Union[Tuple[float, float], float],
+    peak_prominence_thresholds: Union[tuple[float, float], float],
     n_considered_peaks: int,
     lowpass_filter: BaseFilter,
     sampling_rate_hz: float,
 ) -> int:
     """Detect IC within the stride.
 
     Note, that this implementation expects the inverted signal of acc_pa compared to the normal bodyframe definition
@@ -324,17 +325,15 @@
         # The gyr argmax was not found in the first half of the step
         return np.nan
 
     # start with end as this max in the derivative is quite easily detectable within the search region
     # and the start acc_pa max has to be the max before that which is not necessarily
     # the global max within the search region
     refined_search_region_end = int(
-        search_region[0]
-        + np.argmax(gyr_ml_grad[slice(*search_region)])
-        + 1
+        search_region[0] + np.argmax(gyr_ml_grad[slice(*search_region)]) + 1
         # +1 because the min max distance is often very small
         # and in a search range the last value is normally not included but here it should be
     )
     refined_search_region_end = np.clip(refined_search_region_end, None, len(gyr_ml))
 
     # Low pass filter acc_pa to remove sharp peaks and get the overall shape of the signal.
     # The swing acceleration peak is now clearly distinguishable from the IC peak, because the latter is too high
```

### Comparing `gaitmap-2.3.0/gaitmap/example_data.py` & `gaitmap-2.4.0/gaitmap/example_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 import pandas as pd
 import pooch
 
 from gaitmap import __version__
 
 LOCAL_EXAMPLE_PATH = Path(__file__).parent.parent / "example_data/"
 PC_EXAMPLE_PATH = Path.home() / ".gaitmap_data/"
-GITHUB_FOLDER_PATH = "https://raw.githubusercontent.com/mad-lab-fau/gaitmap/v{version}/example_data/"
+GITHUB_FOLDER_PATH = "https://raw.githubusercontent.com/mad-lab-fau/gaitmap/{version}/example_data/"
 
 
 BRIAN = pooch.create(
     # Use the default cache folder for the operating system
     path=pooch.os_cache("gaitmap"),
     # The remote data is on Github
     base_url=GITHUB_FOLDER_PATH,
-    version=__version__,
+    version=f"v{__version__}",
     version_dev="master",
     registry={
         "imu_sample.csv": "sha256:fdb91f0a1e58b1ac518a324d38c9177de6c4388137c1b1683e4a72460873bfd7",
         "imu_sample_healthy_stair_down.csv": "935442b1ec74ad69211ff3364e1d949c2811f1e24afa7f2f5322ce167976980e",
         "imu_sample_healthy_stair_up.csv": "91c66d4370fa2c152ab280df3ac2c607c71bf788f3a4bff7e690030aa6f5d5fe",
         "imu_sample_ms_left.csv": "5308a0833629a6ea76f3cdba3dca4ac185eabfd93e00b85f9cdaaa2a7c599b62",
         "imu_sample_ms_right.csv": "5349aeed45fbdb491c16f633b1f10a0d1c42b1bb2f56b429ce5fa9b9cd484376",
```

### Comparing `gaitmap-2.3.0/gaitmap/gait_detection/__init__.py` & `gaitmap-2.4.0/gaitmap/gait_detection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The :py:mod:`gaitmap.gait_detection` contains algorithms to detect regions of gait in the sensor signal.
 
 Different algorithms for gait sequence detection are going to be collected here.
 """
+
 from gaitmap.utils._gaitmap_mad import patch_gaitmap_mad_import
 
 _gaitmap_mad_modules = {
     "UllrichGaitSequenceDetection",
 }
 
 if not (__getattr__ := patch_gaitmap_mad_import(_gaitmap_mad_modules, __name__)):
```

### Comparing `gaitmap-2.3.0/gaitmap/parameters/_spatial_parameters.py` & `gaitmap-2.4.0/gaitmap/parameters/_spatial_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Calculate spatial parameters algorithm by Kanzler et al. 2015 and Rampp et al. 2014."""
+
 import warnings
-from typing import Dict, Literal, Optional, Sequence, Union
+from collections.abc import Sequence
+from typing import Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 from numpy.linalg import norm
 from scipy.spatial.transform import Rotation
 from typing_extensions import Self
 
@@ -28,14 +30,15 @@
 )
 from gaitmap.utils.exceptions import ValidationError
 from gaitmap.utils.rotations import find_angle_between_orientations, find_unsigned_3d_angle
 
 ParamterNames = Literal[
     "stride_length",
     "gait_velocity",
+    "max_orientation_change",
     "ic_angle",
     "tc_angle",
     "turning_angle",
     "arc_length",
     "max_sensor_lift",
     "max_lateral_excursion",
 ]
@@ -89,14 +92,18 @@
         Note, that the stride time is calculated from `pre_ic` to `ic` if a `min_vel` type stride list is provided.
         The stride is estimated based on the position at the `start` and the `end` of a stride.
         This means these two measures are calculated from different time periods which might lead to errors in
         certain edge cases.
     Arc Length
         The overall arc length is directly calculated from the position of the sensor by adding the absolute changes in
         position at every time point.
+    Max. orientation change
+        The maximum change of sensor angle in the sagittal plane.
+        This is similar to the range of motion of the ankle, however, the measured parameter is effected by other joints
+        such as knee and hip as well.
     Turning Angle
         The turning angle is calculated as the difference in orientation of the forward direction between the first
         and the last sample of each stride.
         Only the rotation around the z-axis (upwards) is considered.
         A turn to the left results in a positive and a turn to the right in a negative turning angle independent of
         the foot.
     IC/TC Angle and angle course
@@ -132,64 +139,62 @@
     (orientation and position) as input.
 
     >>> stride_list = ...  # from event detection
     >>> positions = ...  # from position estimation
     >>> orientations = ...  # from orientation estimation
     >>> spatial_paras = SpatialParameterCalculation()
     >>> spatial_paras = spatial_paras.calculate(
-    ...                               stride_event_list=stride_list,
-    ...                               positions=positions,
-    ...                               orientations=orientations,
-    ...                               sampling_rate_hz=204.8
-    ...                  )
+    ...     stride_event_list=stride_list, positions=positions, orientations=orientations, sampling_rate_hz=204.8
+    ... )
     >>> spatial_paras.parameters_
     <Dataframe/dictionary with all the parameters>
     >>> spatial_paras.parameters_pretty_
     <Dataframe/dictionary with all the parameters with units included in column names>
 
     See Also
     --------
     gaitmap.parameters.TemporalParameterCalculation: Calculate temporal parameters
 
     """
 
     calculate_only: Optional[Sequence[ParamterNames]]
     expected_stride_type: Literal["min_vel", "ic"]
 
-    parameters_: Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]]
-    sole_angle_course_: Optional[Union[pd.Series, Dict[_Hashable, pd.Series]]]
+    parameters_: Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]]
+    sole_angle_course_: Optional[Union[pd.Series, dict[_Hashable, pd.Series]]]
 
     stride_event_list: StrideList
     positions: Optional[PositionList]
     orientations: Optional[OrientationList]
     sampling_rate_hz: float
 
     def __init__(
         self,
         calculate_only: Optional[Sequence[ParamterNames]] = None,
         expected_stride_type: Literal["min_vel", "ic"] = "min_vel",
-    ):
+    ) -> None:
         self.calculate_only = calculate_only
         self.expected_stride_type = expected_stride_type
 
     @property
-    def parameters_pretty_(self) -> Union[pd.DataFrame, Dict[_Hashable, pd.DataFrame]]:
+    def parameters_pretty_(self) -> Union[pd.DataFrame, dict[_Hashable, pd.DataFrame]]:
         """Return parameters with column names indicating units."""
         if isinstance(self.parameters_, dict):
             parameters_ = {}
             for sensor in self.parameters_:
                 parameters_[sensor] = self._rename_columns(self.parameters_[sensor])
             return parameters_
         return self._rename_columns(self.parameters_)
 
     @staticmethod
     def _rename_columns(parameters: pd.DataFrame) -> pd.DataFrame:
         pretty_columns = {
             "stride_length": "stride length [m]",
             "gait_velocity": "gait velocity [m/s]",
+            "max_orientation_change": "max. orientation change [deg]",
             "ic_angle": "ic angle [deg]",
             "tc_angle": "tc angle [deg]",
             "turning_angle": "turning angle [deg]",
             "arc_length": "arc length [m]",
             "max_sensor_lift": "max. sensor lift [m]",
             "max_lateral_excursion": "max. lateral excursion [m]",
         }
@@ -299,15 +304,15 @@
             The sampling rate of the data signal.
 
         Returns
         -------
         parameters_
             Data frame containing spatial parameters of single sensor
         sole_angle_course_
-            The sole angle in the sagttial plane for each stride
+            The sole angle in the sagittal plane for each stride
 
         """
         stride_event_list = set_correct_index(stride_event_list, SL_INDEX)
 
         stride_parameter_dict = {}
 
         if positions is not None:
@@ -372,14 +377,17 @@
 
         if self._should_calculate("tc_angle") and "tc" in stride_event_list.columns:
             tc_relative = (stride_event_list["tc"] - stride_event_list["start"]).astype("Int64")
             param_dict["tc_angle"] = _get_angle_at_index(angle_course, tc_relative)
         else:
             warnings.warn("TC angle could not be calculated as TC event is not available.")
 
+        if self._should_calculate("max_orientation_change"):
+            param_dict["max_orientation_change"] = _get_max_angle_change(sagittal_angles=angle_course + 90)
+
         if self._should_calculate("turning_angle"):
             param_dict["turning_angle"] = _calc_turning_angle(orientations)
 
         return param_dict
 
     def _should_calculate(self, parameter_name: ParamterNames) -> bool:
         if self.calculate_only is None:
@@ -396,14 +404,22 @@
 
 
 def _get_angle_at_index(angle_course: pd.Series, index_per_stride: pd.Series) -> pd.Series:
     indexer = pd.MultiIndex.from_frame(index_per_stride.reset_index())
     return angle_course[indexer].reset_index(level=1, drop=True)
 
 
+def _get_max_angle_change(sagittal_angles: pd.Series) -> pd.Series:
+    # get the maximum change in the orientation in sagittal plane. the sagittal angle is equal to the angle_course +90
+    # degrees. This parameter can have a value between 0 and 180.
+    max_angle = sagittal_angles.groupby(level="s_id").max()
+    min_angle = sagittal_angles.groupby(level="s_id").min()
+    return max_angle - min_angle
+
+
 def _calc_turning_angle(orientations: pd.DataFrame) -> pd.Series:
     # We need to handle the case of empty orientations df manually
     if orientations.empty:
         angles = pd.Series()
         angles.index.name = "s_id"
         return angles
```

### Comparing `gaitmap-2.3.0/gaitmap/parameters/_temporal_parameters.py` & `gaitmap-2.4.0/gaitmap/parameters/_temporal_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Calculate temporal parameters algorithm."""
-from typing import Dict, Literal, Tuple, TypeVar, Union
+
+from typing import Literal, TypeVar, Union
 
 import pandas as pd
 
 from gaitmap.base import BaseTemporalParameterCalculation
 from gaitmap.utils.consts import SL_INDEX
 from gaitmap.utils.datatype_helper import (
     SingleSensorStrideList,
@@ -66,15 +67,15 @@
        Engineering, vol. 62, no. 4, pp. 1089-1097, Apr. 2015. [Online].
        Available: http://ieeexplore.ieee.org/document/6949634/
 
     Examples
     --------
     This method requires the output of a event detection method as input.
 
-    >>> stride_list = ... #  from event detection
+    >>> stride_list = ...  #  from event detection
     >>> temporal_paras = TemporalParameterCalculation()
     >>> temporal_paras = temporal_paras.calculate(stride_event_list=stride_list, sampling_rate_hz=204.8)
     >>> temporal_paras.parameters_
     <Dataframe/dictionary with all the parameters>
     >>> temporal_paras.parameters_pretty_
     <Dataframe/dictionary with all the parameters with units included in column names>
 
@@ -82,24 +83,24 @@
     --------
     gaitmap.parameters.SpatialParameterCalculation: Calculate spatial parameters
 
     """
 
     expected_stride_type: Literal["min_vel", "ic"]
 
-    parameters_: Union[pd.DataFrame, Dict[str, pd.DataFrame]]
+    parameters_: Union[pd.DataFrame, dict[str, pd.DataFrame]]
 
     sampling_rate_hz: float
     stride_event_list: StrideList
 
-    def __init__(self, expected_stride_type: Literal["min_vel", "ic"] = "min_vel"):
+    def __init__(self, expected_stride_type: Literal["min_vel", "ic"] = "min_vel") -> None:
         self.expected_stride_type = expected_stride_type
 
     @property
-    def parameters_pretty_(self) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
+    def parameters_pretty_(self) -> Union[pd.DataFrame, dict[str, pd.DataFrame]]:
         """Return parameters with column names indicating units."""
         if isinstance(self.parameters_, dict):
             parameters_ = {}
             for sensor in self.parameters_:
                 parameters_[sensor] = self._rename_columns(self.parameters_[sensor])
             return parameters_
         return self._rename_columns(self.parameters_)
@@ -178,21 +179,21 @@
             "swing_time": swing_time,
             "stance_time": stance_time,
         }
         parameters_ = pd.DataFrame(stride_parameter_dict, index=stride_event_list.index)
         return parameters_
 
 
-def _get_stride_time_cols(stride_type: Literal["min_vel", "ic"]) -> Tuple[str, str]:
+def _get_stride_time_cols(stride_type: Literal["min_vel", "ic"]) -> tuple[str, str]:
     if stride_type == "min_vel":
         return "pre_ic", "ic"
     if stride_type == "ic":
         return "start", "end"
     raise ValueError("stride_type should be either 'min_vel' or 'ic'")
 
 
-def _get_swing_time_cols(stride_type: Literal["min_vel", "ic"]) -> Tuple[str, str]:
+def _get_swing_time_cols(stride_type: Literal["min_vel", "ic"]) -> tuple[str, str]:
     if stride_type == "min_vel":
         return "tc", "ic"
     if stride_type == "ic":
         return "tc", "end"
     raise ValueError("stride_type should be either 'min_vel' or 'ic'")
```

### Comparing `gaitmap-2.3.0/gaitmap/preprocessing/sensor_alignment/__init__.py` & `gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.3.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py` & `gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Helpers to rotate the sensor in the predefined gaitmap sensor frame."""
-from typing import Dict, Union
+
+from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from gaitmap.utils import rotations
 from gaitmap.utils._types import _Hashable
 from gaitmap.utils.consts import GRAV_VEC, SF_ACC, SF_GYR
@@ -78,15 +79,15 @@
     gaitmap.utils.static_moment_detection.find_static_sequences: Details on the used static moment detection function
         for this method.
 
     """
     dataset_type = is_sensor_data(dataset)
 
     window_length = int(round(window_length_s * sampling_rate_hz))
-    acc_vector: Union[np.ndarray, Dict[_Hashable, np.ndarray]]
+    acc_vector: Union[np.ndarray, dict[_Hashable, np.ndarray]]
     if dataset_type == "single":
         # get static acc vector
         acc_vector = _get_static_acc_vector(dataset, window_length, static_signal_th, metric)
         # get rotation to gravity
         rotation = rotations.get_gravity_rotation(acc_vector, gravity)
     else:
         # build dict with static acc vectors for each sensor in dataset
```

### Comparing `gaitmap-2.3.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py` & `gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.3.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py` & `gaitmap-2.4.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A implementation of a PCA based sensor alignment to perform coordinate system rotations."""
 
-from typing import Dict, Optional, Sequence, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import numpy as np
 from scipy.spatial.transform import Rotation
 from sklearn.decomposition import PCA
 from typing_extensions import Self
 
 from gaitmap.base import BaseSensorAlignment
@@ -101,17 +102,17 @@
 
 
     Examples
     --------
     Align dataset to medio-lateral plane, by aligning the y-axis with the dominant component in the
     gyro x-y-plane
 
-    >>> pca_alignment = PcaAlignment(target_axis="y", pca_plane_axis=("gyr_x","gyr_y"))
+    >>> pca_alignment = PcaAlignment(target_axis="y", pca_plane_axis=("gyr_x", "gyr_y"))
     >>> pca_alignment = pca_alignment.align(data, 204.8)
-    >>> pca_alignment.aligned_data_['left_sensor']
+    >>> pca_alignment.aligned_data_["left_sensor"]
     <copy of dataset with axis aligned to the medio-lateral plane>
     ...
 
     Notes
     -----
     The PCA is sign invariant this means only an alignment to the medio-lateral plane will be performend! An additional
     180deg flip of the coordinate system might be still necessary after the PCA alignment!
@@ -125,23 +126,23 @@
     --------
     sklearn.decomposition.PCA: Details on the used PCA implementation for this method.
     gaitmap.preprocessing.sensor_alignment.ForwardDirectionSignAlignment: Alignment of the forward direction after
                                                                           PCA Alignment
 
     """
 
-    rotation_: Union[Rotation, Dict[_Hashable, Rotation]]
-    pca_: Union[PCA, Dict[_Hashable, PCA]]
+    rotation_: Union[Rotation, dict[_Hashable, Rotation]]
+    pca_: Union[PCA, dict[_Hashable, PCA]]
 
     target_axis: str
     pca_plane_axis: Sequence[str]
 
     data: SensorData
 
-    def __init__(self, target_axis: str = "y", pca_plane_axis: Sequence[str] = ("gyr_x", "gyr_y")):
+    def __init__(self, target_axis: str = "y", pca_plane_axis: Sequence[str] = ("gyr_x", "gyr_y")) -> None:
         self.target_axis = target_axis
         self.pca_plane_axis = pca_plane_axis
 
     def align(self, data: SensorData, **_) -> Self:
         """Align sensor data."""
         self.data = data
         dataset_type = is_sensor_data(data, check_gyr=True, check_acc=True, frame="sensor")
```

### Comparing `gaitmap-2.3.0/gaitmap/stride_segmentation/__init__.py` & `gaitmap-2.4.0/gaitmap/stride_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.3.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py` & `gaitmap-2.4.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Wrapper class to apply a stride segmentation to multiple regions of interest in a dataset."""
+
 from copy import deepcopy
-from typing import Dict, Generic, Optional, TypeVar, Union
+from typing import Generic, Optional, TypeVar, Union
 
 import pandas as pd
 from tpcp import get_action_method
 from typing_extensions import Literal
 
 from gaitmap.base import BaseStrideSegmentation
 from gaitmap.utils._algo_helper import invert_result_dictionary, set_params_from_dict
@@ -122,15 +123,15 @@
     """
 
     segmentation_algorithm: Optional[StrideSegmentationAlgorithm]
     s_id_naming: Literal["replace", "prefix"]
     action_method: Optional[str]
 
     instances_per_roi_: Union[
-        Dict[_Hashable, StrideSegmentationAlgorithm], Dict[_Hashable, Dict[_Hashable, StrideSegmentationAlgorithm]]
+        dict[_Hashable, StrideSegmentationAlgorithm], dict[_Hashable, dict[_Hashable, StrideSegmentationAlgorithm]]
     ]
     stride_list_: StrideList
 
     data: SensorData
     sampling_rate_hz: float
     regions_of_interest: RegionsOfInterestList
 
@@ -138,15 +139,15 @@
     _multi_roi: bool
 
     def __init__(
         self,
         segmentation_algorithm: Optional[StrideSegmentationAlgorithm] = None,
         s_id_naming: Literal["replace", "prefix"] = "replace",
         action_method: Optional[str] = None,
-    ):
+    ) -> None:
         self.segmentation_algorithm = segmentation_algorithm
         self.s_id_naming = s_id_naming
         self.action_method = action_method
 
     def segment(
         self: Self,
         data: SensorData,
@@ -179,16 +180,16 @@
         self._validate_other_parameters()
         # For the type-checker
         assert self.regions_of_interest is not None
         assert self.segmentation_algorithm is not None
 
         if self._multi_roi:
             # Apply the segmentation to a single dataset in case a multi - sensor roi list is provided
-            results_dict: Dict[
-                _Hashable, Dict[str, Union[pd.DataFrame, Dict[_Hashable, StrideSegmentationAlgorithm]]]
+            results_dict: dict[
+                _Hashable, dict[str, Union[pd.DataFrame, dict[_Hashable, StrideSegmentationAlgorithm]]]
             ] = {}
             for sensor, roi in self.regions_of_interest.items():
                 sensor_data = self.data[sensor]
                 results_dict[sensor] = self._segment_single_sensor(
                     self.segmentation_algorithm, sensor_data, self.sampling_rate_hz, roi, sensor_name=sensor, **kwargs
                 )
             results = invert_result_dictionary(results_dict)
@@ -204,15 +205,15 @@
         self,
         segmentation_algorithm: StrideSegmentationAlgorithm,
         sensor_data: pd.DataFrame,
         sampling_rate_hz: float,
         rois: SingleSensorRegionsOfInterestList,
         sensor_name: Optional[_Hashable] = None,
         **kwargs,
-    ) -> Dict[str, Union[pd.DataFrame, Dict[_Hashable, StrideSegmentationAlgorithm]]]:
+    ) -> dict[str, Union[pd.DataFrame, dict[_Hashable, StrideSegmentationAlgorithm]]]:
         """Call the the segmentation algorithm for each region of interest and store the instance."""
         rois = rois.reset_index()
         index_col = ROI_ID_COLS[get_single_sensor_regions_of_interest_types(rois)]
 
         instances_per_roi = {}
         combined_stride_list = {}
         for _, (index, start, end) in rois[[index_col, "start", "end"]].iterrows():
@@ -241,15 +242,15 @@
                 combined_stride_list[index] = stride_list[sensor_name]
             else:
                 combined_stride_list[index] = stride_list
 
         combined_stride_list = self._merge_stride_lists(combined_stride_list, index_col)
         return {"stride_list": combined_stride_list, "instances_per_roi": instances_per_roi}
 
-    def _merge_stride_lists(self, stride_lists: Dict[_Hashable, StrideList], index_name: str) -> StrideList:
+    def _merge_stride_lists(self, stride_lists: dict[_Hashable, StrideList], index_name: str) -> StrideList:
         """Merge either single or multisensor stride lists.
 
         The roi id (the dict key in the input), will be a column in the final output dataframe.
         """
         # We assume all algorithms follow convention and return the correct format
         if self._multi_dataset and not self._multi_roi:
             inverted_stride_dict = invert_result_dictionary(stride_lists)
@@ -269,23 +270,23 @@
             concat_stride_list["s_id"] = list(range(len(concat_stride_list)))
         elif self.s_id_naming == "prefix":
             concat_stride_list["s_id"] = (
                 concat_stride_list[index_name].astype(str) + "_" + concat_stride_list["s_id"].astype(str)
             )
         return concat_stride_list.set_index("s_id")
 
-    def _validate_parameters(self):
+    def _validate_parameters(self) -> None:
         if self.segmentation_algorithm is None:
             raise ValueError(
                 "`segmentation_algorithm` must be a valid instance of a StrideSegmentation algorithm. Currently `None`"
             )
         if self.s_id_naming not in ["replace", "prefix"]:
             raise ValueError("Invalid value for `s_id_naming`")
 
-    def _validate_other_parameters(self):
+    def _validate_other_parameters(self) -> None:
         self._multi_dataset = is_sensor_data(self.data, check_acc=False, check_gyr=False) == "multi"
         self._multi_roi = is_regions_of_interest_list(self.regions_of_interest, region_type="any") == "multi"
         if self._multi_roi and not self._multi_dataset:
             raise ValidationError(
                 "You can not use a multi-sensor regions of interest list with a single sensor dataset."
             )
         if not self._multi_roi and self._multi_dataset and isinstance(self.data, dict):
@@ -293,10 +294,10 @@
                 "You can not use a single-sensor regions of interest list with an unsynchronised multi-sensor dataset."
             )
         if self._multi_roi and self._multi_dataset:
             sensor_names = get_multi_sensor_names(self.data)
             missing_sensors = [key for key in self.regions_of_interest if key not in sensor_names]
             if len(missing_sensors) > 0:
                 raise KeyError(
-                    "The regions of interest list contains information for a sensor ({}) that is not in the "
-                    "dataset.".format(missing_sensors)
+                    f"The regions of interest list contains information for a sensor ({missing_sensors}) that is not "
+                    "in the dataset."
                 )
```

### Comparing `gaitmap-2.3.0/gaitmap/stride_segmentation/_utils.py` & `gaitmap-2.4.0/gaitmap/stride_segmentation/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Some general utils for the stride segmentation algorithms."""
-from typing import Tuple, Union
+
+from typing import Union
 
 import numpy as np
 
 from gaitmap.utils.array_handling import find_extrema_in_radius
 
 
 def snap_to_min(
     data: np.ndarray,
     matches_start_end: np.ndarray,
-    snap_to_min_win_samples: Union[int, Tuple[int, int]],
+    snap_to_min_win_samples: Union[int, tuple[int, int]],
 ):
     """Post process a set of matches by "snapping" their start and end values to the closest minima of the data.
 
     Parameters
     ----------
     data
         The raw IMU data that should be used for snapping. Should be a 1D numpy array
```

### Comparing `gaitmap-2.3.0/gaitmap/stride_segmentation/hmm.py` & `gaitmap-2.4.0/gaitmap/stride_segmentation/hmm.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.3.0/gaitmap/trajectory_reconstruction/__init__.py` & `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 This module provides simple methods to estimate the orientation and position on custom IMU data and a set of wrappers
 to make applying these methods to the default gaitmap datasets easier.
 """
 
 from gaitmap.trajectory_reconstruction._region_level_trajectory import RegionLevelTrajectory
 from gaitmap.trajectory_reconstruction._stride_level_trajectory import StrideLevelTrajectory
 from gaitmap.trajectory_reconstruction.orientation_methods import MadgwickAHRS, SimpleGyroIntegration
-from gaitmap.trajectory_reconstruction.position_methods import (
-    ForwardBackwardIntegration,
-    PieceWiseLinearDedriftedIntegration,
-)
+from gaitmap.trajectory_reconstruction.position_methods._forward_backwards_integration import ForwardBackwardIntegration
 from gaitmap.trajectory_reconstruction.trajectory_methods import MadgwickRtsKalman, RtsKalman
+from gaitmap.utils._gaitmap_mad import patch_gaitmap_mad_import
+
+_gaitmap_mad_modules = {
+    "PieceWiseLinearDedriftedIntegration",
+}
+
+if not (__getattr__ := patch_gaitmap_mad_import(_gaitmap_mad_modules, __name__)):
+    del __getattr__
+    from gaitmap_mad.trajectory_reconstruction.position_methods import PieceWiseLinearDedriftedIntegration
 
 __all__ = [
     "MadgwickAHRS",
     "SimpleGyroIntegration",
     "ForwardBackwardIntegration",
     "RtsKalman",
     "MadgwickRtsKalman",
```

### Comparing `gaitmap-2.3.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py` & `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Wrapper to apply position and orientation estimation to multiple regions in a dataset."""
-from typing import Dict, List, Optional, Tuple, Union
+
+from typing import Optional, Union
 
 import pandas as pd
 from scipy.spatial.transform import Rotation
 from tpcp import CloneFactory, is_action_applied
 from typing_extensions import Literal, Self
 
 from gaitmap.base import (
@@ -135,17 +136,15 @@
     >>> # Create an instance of the wrapper
     >>> per_region_traj = RegionLevelTrajectory(trajectory_method=trajectory_method)
     >>> # Apply the method
     >>> data = ...
     >>> sampling_rate_hz = 204.8
     >>> roi_list = ...
     >>> per_region_traj = per_region_traj.estimate(
-    ...                                            data,
-    ...                                            regions_of_interest=roi_list,
-    ...                                            sampling_rate_hz=sampling_rate_hz
+    ...     data, regions_of_interest=roi_list, sampling_rate_hz=sampling_rate_hz
     ... )
     >>> per_region_traj.position_
     <Dataframe or dict with all the positions per region>
     >>> per_region_traj.orientation_
     <Dataframe or dict with all the orientations per region>
 
     If you want to have the trajectory per stride but still use integration methods that could benefit from
@@ -160,18 +159,15 @@
     >>> per_region_traj = RegionLevelTrajectory(trajectory_method=trajectory_method)
     >>> # Apply the method
     >>> data = ...
     >>> sampling_rate_hz = 204.8
     >>> roi_list = ...
     >>> stride_list = ...
     >>> per_region_traj = per_region_traj.estimate_intersect(
-    ...                                                      data,
-    ...                                                      regions_of_interest=roi_list,
-    ...                                                      stride_event_list=stride_list,
-    ...                                                      sampling_rate_hz=sampling_rate_hz
+    ...     data, regions_of_interest=roi_list, stride_event_list=stride_list, sampling_rate_hz=sampling_rate_hz
     ... )
     >>> per_region_traj.position_
     <Dataframe or dict with all the positions per stride>
     >>> per_region_traj.orientation_
     <Dataframe or dict with all the orientations per stride>
 
 
@@ -192,15 +188,15 @@
         self,
         *,
         ori_method: Optional[BaseOrientationMethod] = CloneFactory(SimpleGyroIntegration()),
         # TODO: Change default so simple forward integration once this is implemented
         pos_method: Optional[BasePositionMethod] = CloneFactory(ForwardBackwardIntegration()),
         trajectory_method: Optional[BaseTrajectoryMethod] = None,
         align_window_width: int = 8,
-    ):
+    ) -> None:
         # TODO: Make align window with a second value?
         self.align_window_width = align_window_width
         super().__init__(ori_method=ori_method, pos_method=pos_method, trajectory_method=trajectory_method)
 
     def estimate(
         self,
         data: SensorData,
@@ -326,20 +322,20 @@
             stride_event_list=stride_event_list, return_data=("orientation", "position", "velocity")
         )
         return self
 
     def intersect(
         self,
         stride_event_list: StrideList,
-        return_data: Tuple[Literal["orientation", "position", "velocity"], ...] = (
+        return_data: tuple[Literal["orientation", "position", "velocity"], ...] = (
             "orientation",
             "position",
             "velocity",
         ),
-    ) -> Tuple[Union[PositionList, OrientationList, VelocityList], ...]:
+    ) -> tuple[Union[PositionList, OrientationList, VelocityList], ...]:
         """Cut out the trajectory of individual strides from the region trajectories.
 
         This method can only be used after `estimate` was called.
         Calling `estimate_intersect` before, does **not** work!
 
         For more information about how the intersect works, see `estimate_intersect`.
 
@@ -393,16 +389,16 @@
                     raise ValidationError(
                         "The calculated trajectory is already on a per stride level. "
                         "Most likely, you called `estimate_intersect` before. "
                         "In this case there is no need to use intersect again."
                     ) from e
             if data_type != stride_list_type:
                 raise ValidationError(
-                    "You are trying to intersect the results from a {} sensor dataset with a {} "
-                    "sensor stride list".format(data_type, stride_list_type)
+                    f"You are trying to intersect the results from a {data_type} sensor dataset with a "
+                    f"{stride_list_type} sensor stride list"
                 )
             if data_type == "single":
                 data = self._intersect(data, self.regions_of_interest, stride_event_list)
             else:
                 data = {
                     k: self._intersect(data[k], self.regions_of_interest[k], stride_event_list[k])
                     for k in get_multi_sensor_names(data)
@@ -436,16 +432,16 @@
         output = pd.concat(output, names=["s_id", "sample"])
         return output
 
     def _estimate_single_sensor(
         self,
         data: SingleSensorData,
         integration_regions: SingleSensorRegionsOfInterestList,
-        stride_list_list: Optional[List[SingleSensorStrideList]],
-    ) -> Dict[str, pd.DataFrame]:
+        stride_list_list: Optional[list[SingleSensorStrideList]],
+    ) -> dict[str, pd.DataFrame]:
         # Set the class variable to determine the correct index values per dataset.
         self._expected_integration_region_index = [
             ROI_ID_COLS[get_single_sensor_regions_of_interest_types(integration_regions)]
         ]
         return super()._estimate_single_sensor(data, integration_regions, stride_list_list)
 
     def _calculate_initial_orientation(self, data: SingleSensorData, start: int) -> Rotation:
```

### Comparing `gaitmap-2.3.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py` & `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Wrapper to apply position and orientation estimation to each stride of a dataset."""
+
 from typing import Optional
 
 from scipy.spatial.transform import Rotation
 from tpcp import CloneFactory
 from typing_extensions import Self
 
 from gaitmap.base import (
@@ -108,17 +109,15 @@
     >>> # Create an instance of the wrapper
     >>> per_stride_traj = StrideLevelTrajectory(ori_method=ori_method, pos_method=pos_method)
     >>> # Apply the method
     >>> data = ...
     >>> sampling_rate_hz = 204.8
     >>> stride_list = ...
     >>> per_stride_traj = per_stride_traj.estimate(
-    ...                        data,
-    ...                        stride_event_list=stride_list,
-    ...                        sampling_rate_hz=sampling_rate_hz
+    ...     data, stride_event_list=stride_list, sampling_rate_hz=sampling_rate_hz
     ... )
     >>> per_stride_traj.position_
     <Dataframe or dict with all the positions per stride>
     >>> per_stride_traj.orientation_
     <Dataframe or dict with all the orientations per stride>
 
 
@@ -137,15 +136,15 @@
     def __init__(
         self,
         *,
         ori_method: Optional[BaseOrientationMethod] = CloneFactory(SimpleGyroIntegration()),
         pos_method: Optional[BasePositionMethod] = CloneFactory(ForwardBackwardIntegration()),
         trajectory_method: Optional[BaseTrajectoryMethod] = None,
         align_window_width: int = 8,
-    ):
+    ) -> None:
         # TODO: Make align window with a second value?
         self.align_window_width = align_window_width
         super().__init__(ori_method=ori_method, pos_method=pos_method, trajectory_method=trajectory_method)
 
     def estimate(self, data: SensorData, stride_event_list: StrideList, *, sampling_rate_hz: float) -> Self:
         """Use the initial rotation and the gyroscope signal to estimate the orientation to every time point .
 
@@ -169,15 +168,15 @@
 
         dataset_type = is_sensor_data(data, frame="sensor")
         stride_list_type = is_stride_list(stride_event_list, stride_type="min_vel", check_additional_cols=False)
 
         if dataset_type != stride_list_type:
             raise ValidationError(
                 "An invalid combination of stride list and dataset was provided. "
-                "The dataset is {} sensor and the stride list is {} sensor.".format(dataset_type, stride_list_type)
+                f"The dataset is {dataset_type} sensor and the stride list is {stride_list_type} sensor."
             )
 
         # For the per stride integration, we create a dummy stride list-list, containing only the single stride that is
         # in each integration region.
         if stride_list_type == "single":
             stride_event_list = set_correct_index(stride_event_list, SL_INDEX)
             stride_list_list = [
```

### Comparing `gaitmap-2.3.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py` & `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """A helper class for common utilities TrajectoryReconstructionWrapper classes."""
+
 import warnings
-from typing import Dict, List, Optional, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 from scipy.spatial.transform import Rotation
 from tpcp import cf
 from typing_extensions import Literal, Self
 
@@ -19,15 +21,15 @@
     SensorData,
     SingleSensorData,
     SingleSensorRegionsOfInterestList,
     SingleSensorStrideList,
     get_multi_sensor_names,
     set_correct_index,
 )
-from gaitmap.utils.rotations import get_gravity_rotation, rotate_dataset_series
+from gaitmap.utils.rotations import get_gravity_rotation
 
 
 class _TrajectoryReconstructionWrapperMixin:
     ori_method: Optional[BaseOrientationMethod]
     pos_method: Optional[BasePositionMethod]
     trajectory_method: Optional[BaseTrajectoryMethod]
 
@@ -40,20 +42,20 @@
 
     def __init__(
         self,
         *,
         ori_method: Optional[BaseOrientationMethod] = cf(SimpleGyroIntegration()),
         pos_method: Optional[BasePositionMethod] = cf(ForwardBackwardIntegration()),
         trajectory_method: Optional[BaseTrajectoryMethod] = None,
-    ):
+    ) -> None:
         self.ori_method = ori_method
         self.pos_method = pos_method
         self.trajectory_method = trajectory_method
 
-    def _validate_methods(self):
+    def _validate_methods(self) -> None:
         if self.trajectory_method:
             if self.ori_method or self.pos_method:
                 warnings.warn(
                     "You provided a trajectory method AND an ori or pos method. "
                     "The ori and pos method will be ignored.\n"
                     "If you see this warning, it could be that you simple left the ori and pos as their default "
                     "values. In this case you can ignore this warning. "
@@ -82,40 +84,40 @@
                 )
             self._combined_algo_mode = False
 
     def _estimate(
         self,
         data,
         integration_regions,
-        stride_list_list: Optional[Union[Dict[str, List[SingleSensorStrideList]], List[SingleSensorStrideList]]],
+        stride_list_list: Optional[Union[dict[str, list[SingleSensorStrideList]], list[SingleSensorStrideList]]],
         dataset_type: Literal["single", "multi"],
     ) -> Self:
         """Actual estimation method.
 
         This will call the correct estimation method depending on the dataset type and perform the integration per
         integration region.
         """
         if dataset_type == "single":
             results = self._estimate_single_sensor(data, integration_regions, stride_list_list)
         else:
-            results_dict: Dict[_Hashable, Dict[str, pd.DataFrame]] = {}
+            results_dict: dict[_Hashable, dict[str, pd.DataFrame]] = {}
             for sensor in get_multi_sensor_names(data):
                 results_dict[sensor] = self._estimate_single_sensor(
                     data[sensor], integration_regions[sensor], stride_list_list[sensor] if stride_list_list else None
                 )
             results = invert_result_dictionary(results_dict)
         set_params_from_dict(self, results, result_formatting=True)
         return self
 
     def _estimate_single_sensor(
         self,
         data: SingleSensorData,
         integration_regions: SingleSensorRegionsOfInterestList,
-        stride_list_list: Optional[List[SingleSensorStrideList]],
-    ) -> Dict[str, pd.DataFrame]:
+        stride_list_list: Optional[list[SingleSensorStrideList]],
+    ) -> dict[str, pd.DataFrame]:
         integration_regions = set_correct_index(integration_regions, self._expected_integration_region_index)
         full_index = (*self._expected_integration_region_index, "sample")
         orientation = {}
         velocity = {}
         position = {}
         if stride_list_list is not None:
             if len(stride_list_list) != len(integration_regions):
@@ -131,57 +133,54 @@
             return {
                 "orientation": pd.DataFrame(columns=GF_ORI, index=index.copy()),
                 "velocity": pd.DataFrame(columns=GF_VEL, index=index.copy()),
                 "position": pd.DataFrame(columns=GF_POS, index=index.copy()),
             }
         for (r_id, i_region), stride_list in zip(integration_regions.iterrows(), stride_list_list):
             i_start, i_end = (int(i_region["start"]), int(i_region["end"]))
-            i_orientation, i_velocity, i_position = self._estimate_region(data, i_start, i_end, stride_list)
-            orientation[r_id] = pd.DataFrame(i_orientation.as_quat(), columns=GF_ORI)
-            velocity[r_id] = pd.DataFrame(i_velocity, columns=GF_VEL)
-            position[r_id] = pd.DataFrame(i_position, columns=GF_POS)
+            orientation[r_id], velocity[r_id], position[r_id] = self._estimate_region(data, i_start, i_end, stride_list)
         orientation_df = pd.concat(orientation)
         orientation_df.index = orientation_df.index.rename(full_index)
         velocity_df = pd.concat(velocity)
         velocity_df.index = velocity_df.index.rename(full_index)
         position_df = pd.concat(position)
         position_df.index = position_df.index.rename(full_index)
         return {"orientation": orientation_df, "velocity": velocity_df, "position": position_df}
 
     def _estimate_region(
         self, data: SingleSensorData, start: int, end: int, stride_event_list: SingleSensorStrideList
-    ) -> Tuple[Rotation, pd.DataFrame, pd.DataFrame]:
+    ) -> tuple[Rotation, pd.DataFrame, pd.DataFrame]:
         stride_data = data.iloc[start:end].copy()
         initial_orientation = self._calculate_initial_orientation(data, start)
 
         if self._combined_algo_mode is False:
             # For the type-checker
             assert self.ori_method is not None
             assert self.pos_method is not None
             # Apply the orientation method
             ori_method = self.ori_method.clone().set_params(initial_orientation=initial_orientation)
-            orientation = ori_method.estimate(
+            ori_method.estimate(
                 stride_data, sampling_rate_hz=self.sampling_rate_hz, stride_event_list=stride_event_list
-            ).orientation_object_
-
-            rotated_stride_data = rotate_dataset_series(stride_data, orientation[:-1])
+            )
+            orientation = ori_method.orientation_
+            rotated_stride_data = ori_method.rotated_data_
             # Apply the Position method
             pos_method = self.pos_method.clone().estimate(
                 rotated_stride_data, sampling_rate_hz=self.sampling_rate_hz, stride_event_list=stride_event_list
             )
             velocity = pos_method.velocity_
             position = pos_method.position_
         else:
             # For the type-checker
             assert self.trajectory_method is not None
             trajectory_method = self.trajectory_method.clone().set_params(initial_orientation=initial_orientation)
             trajectory_method = trajectory_method.estimate(
                 stride_data, sampling_rate_hz=self.sampling_rate_hz, stride_event_list=stride_event_list
             )
-            orientation = trajectory_method.orientation_object_
+            orientation = trajectory_method.orientation_
             velocity = trajectory_method.velocity_
             position = trajectory_method.position_
         return orientation, velocity, position
 
     def _calculate_initial_orientation(self, data: SingleSensorData, start: int) -> Rotation:
         raise NotImplementedError()
```

### Comparing `gaitmap-2.3.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py` & `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Implementation of the MadgwickAHRS."""
+
 from typing import Optional, Union
 
 import numpy as np
 from joblib import Memory
 from numba import njit
 from scipy.spatial.transform import Rotation
 from tpcp import cf
@@ -44,14 +45,17 @@
     Attributes
     ----------
     orientation_
         The rotations as a *SingleSensorOrientationList*, including the initial orientation.
         This means the there are len(data) + 1 orientations.
     orientation_object_
         The orientations as a single scipy Rotation object
+    rotated_data_
+        The rotated data after applying the estimated orientation to the data.
+        The first sample of the data remain unrotated (initial orientation).
 
     Other Parameters
     ----------------
     data
         The data passed to the estimate method
     sampling_rate_hz
         The sampling rate of this data
@@ -91,23 +95,20 @@
 
     """
 
     initial_orientation: Union[np.ndarray, Rotation]
     beta: float
     memory: Optional[Memory]
 
-    data: SingleSensorData
-    sampling_rate_hz: float
-
     def __init__(
         self,
         beta: float = 0.2,
         initial_orientation: Union[np.ndarray, Rotation] = cf(np.array([0, 0, 0, 1.0])),
         memory: Optional[Memory] = None,
-    ):
+    ) -> None:
         self.initial_orientation = initial_orientation
         self.beta = beta
         self.memory = memory
 
     def estimate(self, data: SingleSensorData, *, sampling_rate_hz: float, **_) -> Self:
         """Estimate the orientation of the sensor.
 
@@ -200,18 +201,18 @@
     return q
 
 
 @njit(cache=True)
 def _madgwick_update_series(gyro, acc, initial_orientation, sampling_rate_hz, beta):
     out = np.empty((len(gyro) + 1, 4))
     out[0] = initial_orientation
-    for i, (acc_val, gyro_val) in enumerate(zip(gyro, acc)):
+    for i, (gyro_val, acc_val) in enumerate(zip(gyro, acc)):
         initial_orientation = _madgwick_update(
-            gyro=acc_val,
-            acc=gyro_val,
+            gyro=gyro_val,
+            acc=acc_val,
             initial_orientation=initial_orientation,
             sampling_rate_hz=sampling_rate_hz,
             beta=beta,
         )
         out[i + 1] = initial_orientation
 
     return out
```

### Comparing `gaitmap-2.3.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py` & `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Naive Integration of Gyroscope to estimate the orientation."""
+
 from typing import Optional, Union
 
 import numpy as np
 from joblib import Memory
 from numba import njit
 from scipy.spatial.transform import Rotation
 from tpcp import cf
@@ -28,14 +29,17 @@
     Attributes
     ----------
     orientation_
         The rotations as a *SingleSensorOrientationList*, including the initial orientation.
         This means the there are len(data) + 1 orientations.
     orientation_object_
         The orientations as a single scipy Rotation object
+    rotated_data_
+        The rotated data after applying the estimated orientation to the data.
+        The first sample of the data remain unrotated (initial orientation).
 
     Other Parameters
     ----------------
     data
         The data passed to the estimate method
     sampling_rate_hz
         The sampling rate of this data
@@ -69,24 +73,19 @@
     gaitmap.trajectory_reconstruction.StrideLevelTrajectory: Apply the method for each stride of a stride list.
 
     """
 
     initial_orientation: Union[np.ndarray, Rotation]
     memory: Optional[Memory]
 
-    orientation_: Rotation
-
-    data: SingleSensorData
-    sampling_rate_hz: float
-
     def __init__(
         self,
         initial_orientation: Union[np.ndarray, Rotation] = cf(np.array([0, 0, 0, 1.0])),
         memory: Optional[Memory] = None,
-    ):
+    ) -> None:
         self.initial_orientation = initial_orientation
         self.memory = memory
 
     def estimate(self, data: SingleSensorData, *, sampling_rate_hz: float, **_) -> Self:
         """Estimate the orientation of the sensor by simple integration of the Gyro data.
 
         Parameters
```

### Comparing `gaitmap-2.3.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py` & `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.3.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py` & `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
     def __init__(
         self,
         turning_point: float = 0.5,
         steepness: float = 0.08,
         level_assumption: bool = True,
         gravity: Optional[np.ndarray] = cf(GRAV_VEC),
-    ):
+    ) -> None:
         self.turning_point = turning_point
         self.steepness = steepness
         self.level_assumption = level_assumption
         self.gravity = gravity
 
     def estimate(self, data: SingleSensorData, *, sampling_rate_hz: float, **_) -> Self:
         """Estimate the position of the sensor based on the provided global frame data.
```

### Comparing `gaitmap-2.3.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py` & `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Helper functions for the RTS Kalman filter."""
 
-from typing import Any, Callable, NamedTuple, Tuple
+from typing import Any, Callable, NamedTuple
 
 import numpy as np
 from numba import njit
 
 from gaitmap.trajectory_reconstruction.orientation_methods._madgwick import _madgwick_update
 from gaitmap.utils.consts import GRAV_VEC
 from gaitmap.utils.fast_quaternion_math import multiply, quat_from_rotvec, rotate_vector
@@ -17,26 +17,26 @@
 
 
 class ForwardPassDependencies(NamedTuple):
     """Required dependency functions for the forward pass."""
 
     motion_update_func: Callable
     # This needs to be a tuple and not a dict, as numba can not process dicts
-    motion_update_func_parameters: Tuple
+    motion_update_func_parameters: tuple
 
 
 def rts_kalman_update_series(
     acc,
     gyro,
     initial_orientation,
     sampling_rate_hz,
     meas_noise,
     process_noise,
     zupts,
-    parameters: Tuple[Any, ...],
+    parameters: tuple[Any, ...],
     forward_pass_func: Callable,
     forward_pass_dependencies: ForwardPassDependencies,
 ):
     """Perform a forward and backwards kalman pass with smoothing over the entire series."""
     return _rts_kalman_update_series(
         acc,
         gyro,
@@ -79,15 +79,15 @@
     rotated_acc = rotate_vector(new_orientation, acc)
     new_position = position + velocity / sampling_rate_hz + 0.5 * (rotated_acc - GRAV_VEC) / sampling_rate_hz**2
     new_velocity = velocity + (rotated_acc - GRAV_VEC) / sampling_rate_hz
     return new_position, new_velocity, new_orientation
 
 
 @njit()
-def default_rts_kalman_forward_pass(  # pylint: disable=too-many-statements
+def default_rts_kalman_forward_pass(  # pylint: disable=too-many-statements  # noqa: PLR0915
     accel,
     gyro,
     initial_orientation,
     sampling_rate_hz,
     meas_noise,
     process_noise,
     zupts,
@@ -288,15 +288,15 @@
     acc,
     gyro,
     initial_orientation,
     sampling_rate_hz,
     meas_noise,
     process_noise,
     zupts,
-    parameters: Tuple[Any, ...],
+    parameters: tuple[Any, ...],
     forward_pass_func: Callable,
     forward_pass_dependencies: ForwardPassDependencies,
 ):
     forward_eskf_results, forward_nominal_states = forward_pass_func(
         acc,
         gyro,
         initial_orientation,
```

### Comparing `gaitmap-2.3.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py` & `gaitmap-2.4.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """An error state kalman filter with Rauch-Tung-Striebel smoothing fo estimating trajectories."""
+
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 from scipy.spatial.transform import Rotation
 from tpcp import cf
 from typing_extensions import Self
@@ -77,14 +78,17 @@
     velocity_
         The calculated velocities
     covariance_
         The covariance matrices of the kalman filter after smoothing.
         They can be used as a measure of how good the filter worked and how accurate the results are.
     zupts_
         2D array indicating the start and the end samples of the detected ZUPTs for debug porpuses.
+    rotated_data_
+        The rotated data after applying the estimated orientation to the data.
+        The first sample of the data remain unrotated (initial orientation).
 
     Other Parameters
     ----------------
     data
         The data passed to the estimate method
     sampling_rate_hz
         The sampling rate of this data
@@ -111,22 +115,21 @@
 
     >>> import pandas as pd
     >>> from gaitmap.utils.consts import SF_COLS
     >>> from gaitmap.trajectory_reconstruction import RtsKalman
     >>> data = pd.DataFrame(..., columns=SF_COLS)
     >>> sampling_rate_hz = 100
     >>> # Create an algorithm instance
-    >>> kalman = RtsKalman(initial_orientation=np.array([0, 0, 0, 1.0]),
-    ...                    zupt_variance=10e-8,
-    ...                    velocity_error_variance=10e5,
-    ...                    orientation_error_variance=10e-2,
-    ...                    zupt_detector=NormZuptDetector(semsor="gyr",
-    ...                                                   window_length_s=0.05
-    ...                    )
-    ...             )
+    >>> kalman = RtsKalman(
+    ...     initial_orientation=np.array([0, 0, 0, 1.0]),
+    ...     zupt_variance=10e-8,
+    ...     velocity_error_variance=10e5,
+    ...     orientation_error_variance=10e-2,
+    ...     zupt_detector=NormZuptDetector(semsor="gyr", window_length_s=0.05),
+    ... )
     >>> # Apply the algorithm
     >>> kalman = kalman.estimate(data, sampling_rate_hz=sampling_rate_hz)
     >>> # Inspect the results
     >>> kalman.orientation_
     <pd.Dataframe with resulting quaternions>
     >>> kalman.orientation_object_
     <scipy.Rotation object>
@@ -173,15 +176,15 @@
         level_walking: bool = True,
         level_walking_variance: float = 10e-8,
         zupt_detector=cf(
             NormZuptDetector(
                 sensor="gyr", window_length_s=0.05, window_overlap=0.5, metric="maximum", inactive_signal_threshold=34.0
             )
         ),
-    ):
+    ) -> None:
         self.initial_orientation = initial_orientation
         self.zupt_variance = zupt_variance
         self.velocity_error_variance = velocity_error_variance
         self.orientation_error_variance = orientation_error_variance
         self.level_walking = level_walking
         self.level_walking_variance = level_walking_variance
         self.zupt_detector = zupt_detector
@@ -338,14 +341,17 @@
     velocity_
         The calculated velocities
     covariance_
         The covariance matrices of the kalman filter after smoothing.
         They can be used as a measure of how good the filter worked and how accurate the results are.
     zupts_
         2D array indicating the start and the end samples of the detected ZUPTs for debug purposes.
+    rotated_data_
+        The rotated data after applying the estimated orientation to the data.
+        The first sample of the data remain unrotated (initial orientation).
 
     Other Parameters
     ----------------
     data
         The data passed to the estimate method
     sampling_rate_hz
         The sampling rate of this data
@@ -370,15 +376,15 @@
         level_walking_variance: float = 10e-8,
         zupt_detector=cf(
             NormZuptDetector(
                 sensor="gyr", window_length_s=0.05, window_overlap=0.5, metric="maximum", inactive_signal_threshold=34.0
             )
         ),
         madgwick_beta: float = 0.2,
-    ):
+    ) -> None:
         self.madgwick_beta = madgwick_beta
         super().__init__(
             initial_orientation=initial_orientation,
             zupt_variance=zupt_variance,
             velocity_error_variance=velocity_error_variance,
             orientation_error_variance=orientation_error_variance,
             level_walking=level_walking,
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/_algo_helper.py` & `gaitmap-2.4.0/gaitmap/utils/_algo_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """A set of helper functions to make developing algorithms easier."""
+
 from __future__ import annotations
 
 from typing import Any
 
 from gaitmap.utils._types import _Hashable, _HashableVar
 
 
 def invert_result_dictionary(
-    nested_dict: dict[_Hashable, dict[_HashableVar, Any]]
+    nested_dict: dict[_Hashable, dict[_HashableVar, Any]],
 ) -> dict[_HashableVar, dict[_Hashable, Any]]:
     """Invert result dictionaries that are obtained from multi sensor results.
 
     This method expects a two level dictionary and flips the levels.
     This means that if a value can be accessed as `nested_dict[k1][k2] = v` in the input, it can be accessed as
     `output_dict[k2][k1] = v`.
 
@@ -29,15 +30,15 @@
     for ok, ov in nested_dict.items():
         for k, v in ov.items():
             nested = out.setdefault(k, {})
             nested[ok] = v
     return out
 
 
-def set_params_from_dict(obj: Any, param_dict: dict[str, Any], result_formatting: bool = False):
+def set_params_from_dict(obj: Any, param_dict: dict[str, Any], result_formatting: bool = False) -> None:
     """Update object attributes from dictionary.
 
     The object will be updated inplace.
 
     Parameters
     ----------
     obj
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/_datatype_validation_helper.py` & `gaitmap-2.4.0/gaitmap/utils/_datatype_validation_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Internal helpers for dataset validation."""
-from typing import Dict, Iterable, List, Sequence, Tuple, Union
+
+from collections.abc import Iterable, Sequence
+from typing import Union
 
 import pandas as pd
 from typing_extensions import Literal
 
 from gaitmap.utils._types import _Hashable
 from gaitmap.utils.consts import BF_ACC, BF_GYR, SF_ACC, SF_GYR
 from gaitmap.utils.exceptions import ValidationError
@@ -12,15 +14,15 @@
 _ALLOWED_FRAMES_TYPE = Literal["any", "body", "sensor"]  # pylint: disable=invalid-name
 _ALLOWED_STRIDE_TYPE = Literal["any", "segmented", "min_vel", "ic"]  # pylint: disable=invalid-name
 _ALLOWED_TRAJ_LIST_TYPES = Literal["stride", "roi", "gs", "any_roi"]  # pylint: disable=invalid-name
 
 
 def _get_expected_dataset_cols(
     frame: Literal["sensor", "body"], check_acc: bool = True, check_gyr: bool = True
-) -> List:
+) -> list:
     expected_cols = []
     if frame == "sensor":
         acc = SF_ACC
         gyr = SF_GYR
     elif frame == "body":
         acc = BF_ACC
         gyr = BF_GYR
@@ -29,21 +31,21 @@
     if check_acc is True:
         expected_cols.extend(acc)
     if check_gyr is True:
         expected_cols.extend(gyr)
     return expected_cols
 
 
-def _assert_is_dtype(obj, dtype: Union[type, Tuple[type, ...]]):
+def _assert_is_dtype(obj, dtype: Union[type, tuple[type, ...]]) -> None:
     """Check if an object has a specific dtype."""
     if not isinstance(obj, dtype):
         raise ValidationError(f"The dataobject is expected to be one of ({dtype},). But it is a {type(obj)}")
 
 
-def _assert_has_multindex_cols(df: pd.DataFrame, nlevels: int = 2, expected: bool = True):
+def _assert_has_multindex_cols(df: pd.DataFrame, nlevels: int = 2, expected: bool = True) -> None:
     """Check if a pd.DataFrame has a multiindex as columns.
 
     Parameters
     ----------
     df
         The dataframe to check
     nlevels
@@ -53,28 +55,28 @@
 
     """
     has_multiindex = isinstance(df.columns, pd.MultiIndex)
     if has_multiindex is not expected:
         if expected is False:
             raise ValidationError(
                 "The dataframe is expected to have a single level of columns. "
-                "But it has a MultiIndex with {} levels.".format(df.columns.nlevels)
+                f"But it has a MultiIndex with {df.columns.nlevels} levels."
             )
         raise ValidationError(
-            "The dataframe is expected to have a MultiIndex with {} levels as columns. "
-            "It has just a single normal column level.".format(nlevels)
+            f"The dataframe is expected to have a MultiIndex with {nlevels} levels as columns. "
+            "It has just a single normal column level."
         )
     if has_multiindex is True and not df.columns.nlevels == nlevels:
         raise ValidationError(
-            "The dataframe is expected to have a MultiIndex with {} levels as columns. "
-            "It has a MultiIndex with {} levels.".format(nlevels, df.columns.nlevels)
+            f"The dataframe is expected to have a MultiIndex with {nlevels} levels as columns. "
+            f"It has a MultiIndex with {df.columns.nlevels} levels."
         )
 
 
-def _assert_has_columns(df: pd.DataFrame, columns_sets: Sequence[Union[List[_Hashable], List[str]]]):
+def _assert_has_columns(df: pd.DataFrame, columns_sets: Sequence[Union[list[_Hashable], list[str]]]) -> None:
     """Check if the dataframe has at least all columns sets.
 
     Examples
     --------
     >>> df = pd.DataFrame()
     >>> df.columns = ["col1", "col2"]
     >>> _assert_has_columns(df, [["other_col1", "other_col2"], ["col1", "col2"]])
@@ -89,38 +91,31 @@
 
     if result is False:
         if len(columns_sets) == 1:
             helper_str = f"columns: {columns_sets[0]}"
         else:
             helper_str = f"one of the following sets of columns: {columns_sets}"
         raise ValidationError(
-            "The dataframe is expected to have {}. Instead it has the following columns: {}".format(
-                helper_str, list(df.columns)
-            )
+            f"The dataframe is expected to have {helper_str}. Instead it has the following columns: {list(df.columns)}"
         )
 
 
-def _assert_has_index_columns(df: pd.DataFrame, index_cols: Iterable[_Hashable]):
+def _assert_has_index_columns(df: pd.DataFrame, index_cols: Iterable[_Hashable]) -> None:
     ex_index_cols = list(index_cols)
     ac_index_cols = list(df.index.names)
     if ex_index_cols != ac_index_cols:
         raise ValidationError(
-            "The dataframe is expected to have exactly the following index columns ({}), "
-            "but it has {}".format(index_cols, df.index.name)
+            f"The dataframe is expected to have exactly the following index columns ({index_cols}), "
+            f"but it has {df.index.name}"
         )
 
 
 # This function exists to avoid cyclic imports in this module
 def _get_multi_sensor_data_names(dataset: Union[dict, pd.DataFrame]) -> Sequence[str]:
-    if isinstance(dataset, pd.DataFrame):
-        keys = dataset.columns.unique(level=0)
-    else:
-        # In case it is a dict
-        keys = dataset.keys()
-
+    keys = dataset.columns.unique(level=0) if isinstance(dataset, pd.DataFrame) else dataset.keys()
     return keys
 
 
-def _assert_multisensor_is_not_empty(obj: Union[pd.DataFrame, Dict]):
+def _assert_multisensor_is_not_empty(obj: Union[pd.DataFrame, dict]) -> None:
     sensors = _get_multi_sensor_data_names(obj)
     if len(sensors) == 0:
         raise ValidationError("The provided multi-sensor object does not contain any data/contains no sensors.")
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/_gaitmap_mad.py` & `gaitmap-2.4.0/gaitmap/utils/_gaitmap_mad.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Helper functions to handle the gaitmap/gaitmap_mad split."""
+
 from importlib.util import find_spec
 
 import gaitmap
 
 
 def patch_gaitmap_mad_import(_gaitmap_mad_modules, current_module_name):
     """Check if the gaitmap_mad module is available and return a patched getattr method if not."""
     if find_spec("gaitmap_mad"):
         import gaitmap_mad  # pylint: disable=import-outside-toplevel
 
-        assert (gm_version := gaitmap_mad.__version__) == (g_version := gaitmap.__version__), (
-            "We only support using the exact same version of `gaitmap` and `gaitmap_mad`. "
-            f"Currently you have the versions `gaitmap`: v{g_version} and `gaitmap_mad`: v{gm_version}. "
-            "Update the `gaitmap` and `gaitmap_mad` packages to the same version (likely you just forgot to update "
-            "`gaitmap_mad` when you updated `gaitmap`)."
-        )
+        if (gm_version := gaitmap_mad.__version__) != (g_version := gaitmap.__version__):
+            raise ImportError(
+                "We only support using the exact same version of `gaitmap` and `gaitmap_mad`. "
+                f"Currently you have the versions `gaitmap`: v{g_version} and `gaitmap_mad`: v{gm_version}. "
+                "Update the `gaitmap` and `gaitmap_mad` packages to the same version (likely you just forgot to update "
+                "`gaitmap_mad` when you updated `gaitmap`)."
+            )
         return None
     from gaitmap.utils.exceptions import GaitmapMadImportError  # pylint: disable=import-outside-toplevel
 
     def new_getattr(name: str):
         if name in _gaitmap_mad_modules:
             raise GaitmapMadImportError(name, current_module_name)
         return globals()[name]
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/array_handling.py` & `gaitmap-2.4.0/gaitmap/utils/array_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """A set of util functions that help to manipulate arrays in any imaginable way."""
-from typing import Iterable, Iterator, List, Optional, Tuple, Union
+
+from collections.abc import Iterable, Iterator
+from typing import Optional, Union
 
 import numba.typed
 import numpy as np
 from numba import njit
 from scipy.interpolate import interp1d
 from scipy.signal import find_peaks
 from typing_extensions import Literal
@@ -48,16 +50,16 @@
     Returns
     -------
     windowed view (or copy for nan_padding) of input array as specified, last window might be nan padded if necessary to
     match window size
 
     Examples
     --------
-    >>> data = np.arange(0,10)
-    >>> windowed_view = sliding_window_view(arr = data, window_length = 5, overlap = 3, nan_padding = True)
+    >>> data = np.arange(0, 10)
+    >>> windowed_view = sliding_window_view(arr=data, window_length=5, overlap=3, nan_padding=True)
     >>> windowed_view
     array([[ 0.,  1.,  2.,  3.,  4.],
            [ 2.,  3.,  4.,  5.,  6.],
            [ 4.,  5.,  6.,  7.,  8.],
            [ 6.,  7.,  8.,  9., nan]])
 
     """
@@ -96,48 +98,53 @@
 
     return view
 
 
 def bool_array_to_start_end_array(bool_array: np.ndarray) -> np.ndarray:
     """Find regions in bool array and convert those to start-end indices.
 
-    The end index is inclusiv!
+    The end index is the first element after the True-region,
+    so you can use it for upper-bound exclusive slicing etc.
 
     Parameters
     ----------
     bool_array : array with shape (n,)
         boolean array with either 0/1, 0.0/1.0 or True/False elements
 
     Returns
     -------
     array of [start, end] indices with shape (n,2)
 
     Examples
     --------
-    >>> example_array = np.array([0,0,1,1,0,0,1,1,1])
+    >>> example_array = np.array([0, 0, 1, 1, 0, 0, 1, 1, 1])
     >>> start_end_list = bool_array_to_start_end_array(example_array)
     >>> start_end_list
     array([[2, 4],
            [6, 9]])
-    >>> example_array[start_end_list[0, 0]: start_end_list[0, 1]]
+    >>> example_array[start_end_list[0, 0] : start_end_list[0, 1]]
     array([1, 1])
 
     """
+    # check if input is a numpy array. E.g. for a Series, start and end will just be the first and last index.
+    if not isinstance(bool_array, np.ndarray):
+        raise TypeError("Input must be a numpy array!")
+
     # check if input is actually a boolean array
     if not np.array_equal(bool_array, bool_array.astype(bool)):
         raise ValueError("Input must be boolean array!")
 
     if len(bool_array) == 0:
         return np.array([])
 
     slices = np.ma.flatnotmasked_contiguous(np.ma.masked_equal(bool_array, 0))
     return np.array([[s.start, s.stop] for s in slices])
 
 
-def start_end_array_to_bool_array(start_end_array: np.ndarray, pad_to_length: int = None) -> np.ndarray:
+def start_end_array_to_bool_array(start_end_array: np.ndarray, pad_to_length: Optional[int] = None) -> np.ndarray:
     """Convert a start-end list to a bool array.
 
     Parameters
     ----------
     start_end_array : array with shape (n,2)
         2d-array indicating start and end values e.g. [[10,20],[20,40],[70,80]]
 
@@ -153,19 +160,19 @@
     -------
     array with shape (n,)
         boolean array with True/False elements
 
     Examples
     --------
     >>> import numpy as np
-    >>> example_array = np.array([[3,5],[7,8]])
+    >>> example_array = np.array([[3, 5], [7, 8]])
     >>> start_end_array_to_bool_array(example_array, pad_to_length=12)
     array([False, False, False,  True,  True,  True, False,  True,  True,
            False, False, False])
-    >>> example_array = np.array([[3,5],[7,8]])
+    >>> example_array = np.array([[3, 5], [7, 8]])
     >>> start_end_array_to_bool_array(example_array, pad_to_length=None)
     array([False, False, False,  True,  True,  True, False,  True,  True])
 
     """
     start_end_array = np.atleast_2d(start_end_array)
 
     if pad_to_length is None:
@@ -177,15 +184,15 @@
 
     bool_array = np.zeros(n_elements)
     for start, end in start_end_array:
         bool_array[start:end] = 1
     return bool_array.astype(bool)
 
 
-def split_array_at_nan(a: np.ndarray) -> List[Tuple[int, np.ndarray]]:
+def split_array_at_nan(a: np.ndarray) -> list[tuple[int, np.ndarray]]:
     """Split an array into sections at nan values.
 
     Examples
     --------
     >>> a = np.array([1, np.nan, 2, 3])
     >>> split_array_at_nan(a)
     [(0, array([1.])), (2, array([2., 3.]))]
@@ -232,15 +239,15 @@
         threshold *= -1
     return find_peaks(-data, height=threshold, **kwargs)[0]
 
 
 def find_extrema_in_radius(
     data: np.ndarray,
     indices: np.ndarray,
-    radius: Union[int, Tuple[int, int]],
+    radius: Union[int, tuple[int, int]],
     extrema_type: Literal["min", "max"] = "min",
 ):
     """Return the index of the global extrema of data in the given radius around each index in indices.
 
     Parameters
     ----------
     data : 1D array
@@ -264,15 +271,15 @@
         Array of the position of each identified extremum
 
     """
     extrema_funcs = {"min": np.nanargmin, "max": np.nanargmax}
     if extrema_type not in extrema_funcs:
         raise ValueError(f"`extrema_type` must be one of {list(extrema_funcs.keys())}, not {extrema_type}")
     extrema_func = extrema_funcs[extrema_type]
-    if radius == 0 or radius == (0, 0):
+    if radius in (0, (0, 0)):
         # In case the search radius is 0 samples, we can just return the input.
         return indices
     if isinstance(radius, int):
         before, after = radius, radius
     elif isinstance(radius, tuple):
         before, after = radius
     else:
@@ -308,15 +315,15 @@
         val = bool_values[i]
         index = index[~np.isnan(index)]
         # perform logical or operation to combine all overlapping window results
         array[index] = np.logical_or(array[index], val)
     return array
 
 
-def multi_array_interpolation(arrays: List[np.ndarray], n_samples, kind: str = "linear") -> np.ndarray:
+def multi_array_interpolation(arrays: list[np.ndarray], n_samples, kind: str = "linear") -> np.ndarray:
     """Interpolate multiple 2D-arrays to the same length along axis 0.
 
     Parameters
     ----------
     arrays
         List of 2D arrays.
         Note that `arr.shape[1]` must be identical for all arrays.
@@ -344,15 +351,14 @@
         x_new = np.linspace(0, len(s), n_samples)
         final_array[i] = interp1d(x_orig, s.T, kind=kind)(x_new)
     return final_array
 
 
 @numba.njit()
 def _fast_linear_interpolation(arrays: numba.typed.List, n_samples) -> np.ndarray:
-
     final_array = np.empty((len(arrays), arrays[0].shape[1], n_samples))
     for i, s in enumerate(arrays):
         s_len = len(s)
         x_orig = np.linspace(0, s_len, s_len)
         x_new = np.linspace(0, s_len, n_samples)
         for j, col in enumerate(s.T):
             final_array[i, j] = np.interp(x_new, x_orig, col)
@@ -388,14 +394,17 @@
            [18, 20]])
 
     >>> merge_intervals(test, 2)
     array([[ 1, 15],
            [18, 20]])
 
     """
+    if input_array.shape[0] == 0:
+        return input_array
+
     return np.array(_solve_overlap(np.sort(input_array, axis=0, kind="stable"), gap_size))
 
 
 @njit
 def _solve_overlap(input_array: np.ndarray, gap_size: int) -> numba.typed.List:
     """Merge intervals that are overlapping and that are a distance less or equal to gap_size from each other."""
     stack = numba.typed.List()
@@ -409,15 +418,15 @@
 
     return stack
 
 
 def iterate_region_data(
     signal_sequence: Iterable[SingleSensorData],
     label_sequences: Iterable[Union[SingleSensorStrideList, SingleSensorRegionsOfInterestList]],
-    expected_col_order: Optional[List[str]] = None,
+    expected_col_order: Optional[list[str]] = None,
 ) -> Iterator[SingleSensorData]:
     """Iterate over individual strides/ROIs in multiple sensor data sequences.
 
     This can be helpful if you want to apply operations to each of these strides or ROIs and there is no other way
     besides iterating over the data.
 
     Parameters
@@ -447,18 +456,18 @@
             try:
                 is_single_sensor_regions_of_interest_list(labels, raise_exception=True)
             except ValidationError as e_roi:
                 raise ValidationError(
                     "The label sequences must be either SingleSensorStrideList or SingleSensorRegionsOfInterestList. "
                     "\n"
                     "The validations failed with the following errors: \n\n"
-                    f"Stride List: \n\n{str(e_stride_list)}\n\n"
-                    f"Regions of Interest List: \n\n{str(e_roi)}"
+                    f"Stride List: \n\n{e_stride_list!s}\n\n"
+                    f"Regions of Interest List: \n\n{e_roi!s}"
                 ) from e_roi
         if expected_col_order is None:
             # In the first iteration we pull the column order.
             # We don't do that beforehand, because otherwise we could not take a generator as input and force the
             # user to put all the data in RAM first.
             expected_col_order = df.columns
         df = df.reindex(columns=expected_col_order)
-        for (_, s, e) in labels[["start", "end"]].itertuples():
+        for _, s, e in labels[["start", "end"]].itertuples():
             yield df.iloc[s:e]
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/consts.py` & `gaitmap-2.4.0/gaitmap/utils/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common constants used in the library."""
+
 import numpy as np
 
 #: The default names of the Gyroscope columns in the sensor frame
 SF_GYR = ["gyr_x", "gyr_y", "gyr_z"]
 #: The default names of the Accelerometer columns in the sensor frame
 SF_ACC = ["acc_x", "acc_y", "acc_z"]
 #: The default names of all columns in the sensor frame
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/coordinate_conversion.py` & `gaitmap-2.4.0/gaitmap/utils/coordinate_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """A set of helper functions for the conversion of accelerometer and gyroscope data from the sensor to the body frame.
 
 Definitions can be found in the :ref:`coordinate_systems` guide.
 """
+
 import warnings
-from typing import List, Optional
+from typing import Optional
 
 import pandas as pd
 
 from gaitmap.utils.consts import BF_COLS, FSF_FBF_CONVERSION_LEFT, FSF_FBF_CONVERSION_RIGHT, SF_COLS
 from gaitmap.utils.datatype_helper import (
     MultiSensorData,
     SingleSensorData,
@@ -77,18 +78,18 @@
         result[FSF_FBF_CONVERSION_RIGHT[sf_col_name][1]] = FSF_FBF_CONVERSION_RIGHT[sf_col_name][0] * data[sf_col_name]
 
     return result
 
 
 def convert_to_fbf(
     data: MultiSensorData,
-    left: Optional[List[str]] = None,
-    right: Optional[List[str]] = None,
-    right_like: str = None,
-    left_like: str = None,
+    left: Optional[list[str]] = None,
+    right: Optional[list[str]] = None,
+    right_like: Optional[str] = None,
+    left_like: Optional[str] = None,
 ):
     """Convert the axes from the sensor frame to the body frame for one MultiSensorDataset.
 
     This function assumes that your dataset is already aligned to the gaitmap FSF.
     Sensors that should not be transformed are kept untouched.
     Note, that the column names of all transformed dataset is changed to the respective body frame names.
 
@@ -116,15 +117,15 @@
     -------
     converted MultiSensorDataset
 
     Examples
     --------
     These examples assume that your dataset has two sensors called `left_sensor` and `right_sensor`.
 
-    >>> dataset = ... # Sensordata in FSF
+    >>> dataset = ...  # Sensordata in FSF
     >>> fbf_dataset = convert_to_fbf(dataset, left_like="left_", right_like="right_")
 
     Alternatively, you can specify the full sensor names.
 
     >>> fbf_dataset = convert_to_fbf(dataset, left=["left_sensor"], right_sensor=["right_sensor"])
 
     See Also
@@ -160,17 +161,16 @@
 
 def _handle_foot(foot, foot_like, data, rot_func):
     result = {}
     if foot_like:
         foot = [sensor for sensor in get_multi_sensor_names(data) if foot_like in sensor]
         if not foot:
             warnings.warn(
-                "The substring {} is not contained in any sensor name. Available sensor names are: {}".format(
-                    foot_like, get_multi_sensor_names(data)
-                )
+                f"The substring {foot_like} is not contained in any sensor name. Available sensor names are: "
+                f"{get_multi_sensor_names(data)}"
             )
     foot = foot or []
     for s in foot:
         if s not in data:
             raise KeyError("Sensordata contains no sensor with name " + s)
         result[s] = rot_func(data[s])
     return result
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/datatype_helper.py` & `gaitmap-2.4.0/gaitmap/utils/datatype_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """A couple of helper functions that easy the use of the typical gaitmap data formats."""
-from typing import Callable, Dict, Iterable, List, Optional, Sequence, Tuple, Union, cast
+
+from collections.abc import Iterable, Sequence
+from typing import Callable, Optional, Union, cast
 
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
 from gaitmap.utils._datatype_validation_helper import (
     _ALLOWED_FRAMES,
@@ -35,34 +37,34 @@
 SingleSensorData = _DataFrame
 SingleSensorStrideList = _DataFrame
 SingleSensorRegionsOfInterestList = _DataFrame
 SingleSensorPositionList = _DataFrame
 SingleSensorVelocityList = _DataFrame
 SingleSensorOrientationList = _DataFrame
 
-MultiSensorData = Union[pd.DataFrame, Dict[_Hashable, SingleSensorData]]
+MultiSensorData = Union[pd.DataFrame, dict[_Hashable, SingleSensorData]]
 SensorData = Union[SingleSensorData, MultiSensorData]
 
-MultiSensorStrideList = Dict[_Hashable, pd.DataFrame]
+MultiSensorStrideList = dict[_Hashable, pd.DataFrame]
 StrideList = Union[SingleSensorStrideList, MultiSensorStrideList]
 
-MultiSensorRegionsOfInterestList = Dict[_Hashable, pd.DataFrame]
+MultiSensorRegionsOfInterestList = dict[_Hashable, pd.DataFrame]
 RegionsOfInterestList = Union[SingleSensorRegionsOfInterestList, MultiSensorRegionsOfInterestList]
 
-MultiSensorPositionList = Dict[_Hashable, pd.DataFrame]
+MultiSensorPositionList = dict[_Hashable, pd.DataFrame]
 PositionList = Union[SingleSensorPositionList, MultiSensorPositionList]
 
-MultiSensorVelocityList = Dict[_Hashable, pd.DataFrame]
+MultiSensorVelocityList = dict[_Hashable, pd.DataFrame]
 VelocityList = Union[SingleSensorVelocityList, MultiSensorVelocityList]
 
-MultiSensorOrientationList = Dict[_Hashable, pd.DataFrame]
+MultiSensorOrientationList = dict[_Hashable, pd.DataFrame]
 OrientationList = Union[SingleSensorOrientationList, MultiSensorOrientationList]
 
 
-def to_dict_multi_sensor_data(sensordata: MultiSensorData) -> Dict[_Hashable, SingleSensorData]:
+def to_dict_multi_sensor_data(sensordata: MultiSensorData) -> dict[_Hashable, SingleSensorData]:
     """Convert a multi-sensor data to a dictionary of single sensor datas.
 
     If it is already in this format, the function will not do anything.
     """
     is_multi_sensor_data(sensordata, check_acc=False, check_gyr=False, raise_exception=True)
     if isinstance(sensordata, dict):
         return sensordata
@@ -131,15 +133,15 @@
         else:
             _assert_has_columns(data, [_get_expected_dataset_cols(frame, check_acc=check_acc, check_gyr=check_gyr)])
 
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object does not seem to be SingleSensorData. "
-                "The validation failed with the following error:\n\n{}".format(str(e))
+                f"The validation failed with the following error:\n\n{e!s}"
             ) from e
         return False
     return True
 
 
 def is_multi_sensor_data(
     data: MultiSensorData,
@@ -190,28 +192,26 @@
         if isinstance(data, pd.DataFrame):
             _assert_has_multindex_cols(data, expected=True, nlevels=2)
         _assert_multisensor_is_not_empty(data)
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object does not seem to be MultiSensorData. "
-                "The validation failed with the following error:\n\n{}".format(str(e))
+                f"The validation failed with the following error:\n\n{e!s}"
             ) from e
         return False
 
     try:
         for k in get_multi_sensor_names(data):
             is_single_sensor_data(data[k], check_acc=check_acc, check_gyr=check_gyr, frame=frame, raise_exception=True)
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object appears to be MultiSensorData, "
-                'but for the sensor with the name "{}", the following validation error was raised:\n\n{}'.format(
-                    k, str(e)
-                )
+                f'but for the sensor with the name "{k}", the following validation error was raised:\n\n{e!s}'
             ) from e
         return False
     return True
 
 
 def is_sensor_data(
     data: SensorData, check_acc: bool = True, check_gyr: bool = True, frame: _ALLOWED_FRAMES_TYPE = "any"
@@ -265,25 +265,25 @@
         return "multi"
 
     raise ValidationError(
         "The passed object appears to be neither single- or multi-sensor data. "
         "Below you can find the errors raised for both checks:\n\n"
         "Single-Sensor\n"
         "=============\n"
-        f"{str(single_error)}\n\n"
+        f"{single_error!s}\n\n"
         "Multi-Sensor\n"
         "=============\n"
-        f"{str(multi_error)}"
+        f"{multi_error!s}"
     )
 
 
 def is_single_sensor_stride_list(
     stride_list: SingleSensorStrideList,
     stride_type: _ALLOWED_STRIDE_TYPE = "any",
-    check_additional_cols: Union[bool, Tuple[str, ...]] = True,
+    check_additional_cols: Union[bool, tuple[str, ...]] = True,
     raise_exception: bool = False,
 ) -> bool:
     """Check if an input is a single-sensor stride list.
 
     A valid stride list:
 
     - is a pandas Dataframe with at least the following columns: `["s_id", "start", "end"]`.
@@ -361,35 +361,35 @@
         # Check that the start time corresponds to the correct event
         if (
             start_event.get(stride_type, False)
             and len(stride_list) > 0
             and not np.array_equal(stride_list["start"].to_numpy(), stride_list[start_event[stride_type]].to_numpy())
         ):
             raise ValidationError(
-                "For a {} stride list, the start column is expected to be identical to the {} column, "
-                "but they are different.".format(stride_type, start_event[stride_type])
+                f"For a {stride_type} stride list, the start column is expected to be identical to the "
+                f"{start_event[stride_type]} column, but they are different."
             )
         # Check that the stride ids are unique
         if not stride_list.index.nunique() == stride_list.index.size:
             raise ValidationError("The stride id of the stride list is expected to be unique.")
 
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object does not seem to be a SingleSensorStrideList. "
-                "The validation failed with the following error:\n\n{}".format(str(e))
+                f"The validation failed with the following error:\n\n{e!s}"
             ) from e
         return False
     return True
 
 
 def is_multi_sensor_stride_list(
     stride_list: MultiSensorStrideList,
     stride_type: _ALLOWED_STRIDE_TYPE = "any",
-    check_additional_cols: Union[bool, Tuple[str, ...]] = True,
+    check_additional_cols: Union[bool, tuple[str, ...]] = True,
     raise_exception: bool = False,
 ) -> bool:
     """Check if an input is a multi-sensor stride list.
 
     A valid multi-sensor stride list is dictionary of single-sensor stride lists.
 
     This function :func:`~gaitmap.utils.dataset_helper.is_single_sensor_stride_list` for each of the contained stride
@@ -420,15 +420,15 @@
     try:
         _assert_is_dtype(stride_list, dict)
         _assert_multisensor_is_not_empty(stride_list)
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object does not seem to be a MultiSensorStrideList. "
-                "The validation failed with the following error:\n\n{}".format(str(e))
+                f"The validation failed with the following error:\n\n{e!s}"
             ) from e
         return False
 
     try:
         for k in stride_list:
             is_single_sensor_stride_list(
                 stride_list[k],
@@ -436,26 +436,24 @@
                 check_additional_cols=check_additional_cols,
                 raise_exception=True,
             )
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object appears to be a MultiSensorStrideList, "
-                'but for the sensor with the name "{}", the following validation error was raised:\n\n{}'.format(
-                    k, str(e)
-                )
+                f'but for the sensor with the name "{k}", the following validation error was raised:\n\n{e!s}'
             ) from e
         return False
     return True
 
 
 def is_stride_list(
     stride_list: StrideList,
     stride_type: _ALLOWED_STRIDE_TYPE = "any",
-    check_additional_cols: Union[bool, Tuple[str, ...]] = True,
+    check_additional_cols: Union[bool, tuple[str, ...]] = True,
 ) -> Literal["single", "multi"]:
     """Check if an object is a valid multi-sensor or single-sensor stride list.
 
     This function will try to check the input using
     :func:`~gaitmap.utils.dataset_helper.is_single_sensor_stride_list` and
     :func:`~gaitmap.utils.dataset_helper.is_multi_sensor_stride_list`.
     In case one of the two checks is successful, a string is returned, which type of dataset the input is.
@@ -504,30 +502,30 @@
         return "multi"
 
     raise ValidationError(
         "The passed object appears to be neither a single- or a multi-sensor stride list. "
         "Below you can find the errors raised for both checks:\n\n"
         "Single-Sensor\n"
         "=============\n"
-        f"{str(single_error)}\n\n"
+        f"{single_error!s}\n\n"
         "Multi-Sensor\n"
         "=============\n"
-        f"{str(multi_error)}"
+        f"{multi_error!s}"
     )
 
 
 def get_single_sensor_regions_of_interest_types(roi_list: SingleSensorRegionsOfInterestList) -> Literal["roi", "gs"]:
     """Identify which type of region of interest list is passed by checking the existing columns."""
     roi_list_columns = roi_list.reset_index().columns
     valid_index_dict = ROI_ID_COLS
     matched_index_col = [col for col in roi_list_columns if col in valid_index_dict.values()]
     if not matched_index_col:
         raise ValidationError(
-            "The region of interest list is expected to have one of {} either as a column or in the "
-            "index".format(list(valid_index_dict.values()))
+            f"The region of interest list is expected to have one of {list(valid_index_dict.values())} either as a "
+            "column or in the index"
         )
     region_type = cast(
         Literal["roi", "gs"], list(valid_index_dict.keys())[list(valid_index_dict.values()).index(matched_index_col[0])]
     )
     return region_type
 
 
@@ -570,31 +568,30 @@
     try:
         _assert_is_dtype(roi_list, pd.DataFrame)
         _assert_has_multindex_cols(roi_list, expected=False)
 
         actual_region_type = get_single_sensor_regions_of_interest_types(roi_list)
         if region_type not in ("any", actual_region_type):
             raise ValidationError(
-                "A ROI list of type {} is expected to have a either an index or a column named {}. "
-                "The provided ROI list appears to be of the type {} instead.".format(
-                    region_type, ROI_ID_COLS[region_type], actual_region_type
-                )
+                f"A ROI list of type {region_type} is expected to have a either an index or a column named "
+                f"{ROI_ID_COLS[region_type]}."
+                "The provided ROI list appears to be of the type {actual_region_type} instead."
             )
 
         roi_list = set_correct_index(roi_list, [ROI_ID_COLS[actual_region_type]])
         _assert_has_columns(roi_list, [["start", "end"]])
 
         # Check that the roi ids are unique
         if not roi_list.index.nunique() == roi_list.index.size:
             raise ValidationError("The roi/gs id of the stride list is expected to be unique.")
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object does not seem to be a SingleSensorRegionsOfInterestList. "
-                "The validation failed with the following error:\n\n{}".format(str(e))
+                f"The validation failed with the following error:\n\n{e!s}"
             ) from e
         return False
 
     return True
 
 
 def is_multi_sensor_regions_of_interest_list(
@@ -628,28 +625,26 @@
     try:
         _assert_is_dtype(roi_list, dict)
         _assert_multisensor_is_not_empty(roi_list)
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object does not seem to be a MultiSensorRegionsOfInterestList. "
-                "The validation failed with the following error:\n\n{}".format(str(e))
+                f"The validation failed with the following error:\n\n{e!s}"
             ) from e
         return False
 
     try:
         for k in roi_list:
             is_single_sensor_regions_of_interest_list(roi_list[k], region_type=region_type, raise_exception=True)
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
                 "The passed object appears to be a MultiSensorRegionsOfInterestList, "
-                'but for the sensor with the name "{}", the following validation error was raised:\n\n{}'.format(
-                    k, str(e)
-                )
+                f'but for the sensor with the name "{k}", the following validation error was raised:\n\n{e!s}'
             ) from e
         return False
     return True
 
 
 def is_regions_of_interest_list(
     roi_list: RegionsOfInterestList, region_type: Literal["any", "roi", "gs"] = "any"
@@ -699,18 +694,18 @@
         return "multi"
 
     raise ValidationError(
         "The passed object appears to be neither a single- or a multi-sensor regions of interest list. "
         "Below you can find the errors raised for both checks:\n\n"
         "Single-Sensor\n"
         "=============\n"
-        f"{str(single_error)}\n\n"
+        f"{single_error!s}\n\n"
         "Multi-Sensor\n"
         "=============\n"
-        f"{str(multi_error)}"
+        f"{multi_error!s}"
     )
 
 
 def get_multi_sensor_names(dataset: MultiSensorData) -> Sequence[_Hashable]:
     """Get the list of sensor names from a multi-sensor dataset.
 
     .. warning:
@@ -721,36 +716,36 @@
     The keys are not guaranteed to be ordered.
 
     """
     return _get_multi_sensor_data_names(dataset=dataset)
 
 
 def get_single_sensor_trajectory_list_types(
-    traj_list: Union[SingleSensorPositionList, SingleSensorOrientationList, SingleSensorVelocityList]
+    traj_list: Union[SingleSensorPositionList, SingleSensorOrientationList, SingleSensorVelocityList],
 ) -> Literal["roi", "gs", "stride"]:
     """Identify which type of trajectory list is passed by checking the existing columns."""
     traj_list_columns = traj_list.reset_index().columns
     valid_index_dict = TRAJ_TYPE_COLS
     matched_index_col = [col for col in traj_list_columns if col in valid_index_dict.values()]
     if not matched_index_col:
         raise ValidationError(
-            "The trajectory (orientation, position, velocity) list is expected to have one of {} either as a column or "
-            "in the index".format(list(valid_index_dict.values()))
+            "The trajectory (orientation, position, velocity) list is expected to have one of "
+            f"{list(valid_index_dict.values())} either as a column or in the index"
         )
     list_type = cast(
         Literal["roi", "gs", "stride"],
         list(valid_index_dict.keys())[list(valid_index_dict.values()).index(matched_index_col[0])],
     )
     return list_type
 
 
 def _is_single_sensor_trajectory_list(
     input_prefix: str,
     input_datatype: str,
-    expected_cols: List[str],
+    expected_cols: list[str],
     traj_list: Union[SingleSensorOrientationList, SingleSensorVelocityList, SingleSensorOrientationList],
     traj_list_type: Optional[_ALLOWED_TRAJ_LIST_TYPES] = None,
     raise_exception: bool = False,
 ) -> bool:
     if traj_list_type and traj_list_type != "any_roi" and traj_list_type not in TRAJ_TYPE_COLS:
         raise ValueError(
             "The argument `{}_type` must be None, or one of {} and not {}.".format(
@@ -767,16 +762,16 @@
             nested_expected_cols = [[*expected_cols, TRAJ_TYPE_COLS[traj_list_type]]]
         else:
             nested_expected_cols = [expected_cols]
         _assert_has_columns(traj_list, nested_expected_cols)
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
-                "The passed object does not seem to be a {}. "
-                "The validation failed with the following error:\n\n{}".format(input_datatype, str(e))
+                f"The passed object does not seem to be a {input_datatype}. "
+                f"The validation failed with the following error:\n\n{e!s}"
             ) from e
         return False
     return True
 
 
 def _is_multi_sensor_trajectory_list(
     input_datatype: str,
@@ -787,29 +782,27 @@
 ) -> bool:
     try:
         _assert_is_dtype(traj_list, dict)
         _assert_multisensor_is_not_empty(traj_list)
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
-                "The passed object does not seem to be a {}. "
-                "The validation failed with the following error:\n\n{}".format(input_datatype, str(e))
+                f"The passed object does not seem to be a {input_datatype}. "
+                f"The validation failed with the following error:\n\n{e!s}"
             ) from e
         return False
 
     try:
         for k in traj_list:
             single_func(traj_list[k], **kwargs, raise_exception=True)
     except ValidationError as e:
         if raise_exception is True:
             raise ValidationError(
-                "The passed object appears to be a {}, "
-                'but for the sensor with the name "{}", the following validation error was raised:\n\n{}'.format(
-                    input_datatype, k, str(e)
-                )
+                f"The passed object appears to be a {input_datatype}, "
+                f'but for the sensor with the name "{k}", the following validation error was raised:\n\n{e!s}'
             ) from e
         return False
     return True
 
 
 def _is_trajectory_list(
     input_datatype: str,
@@ -833,18 +826,18 @@
         return "multi"
 
     raise ValidationError(
         f"The passed object appears to be neither a single- or a multi-sensor {input_datatype}. "
         "Below you can find the errors raised for both checks:\n\n"
         "Single-Sensor\n"
         "=============\n"
-        f"{str(single_error)}\n\n"
+        f"{single_error!s}\n\n"
         "Multi-Sensor\n"
         "=============\n"
-        f"{str(multi_error)}"
+        f"{multi_error!s}"
     )
 
 
 def is_single_sensor_position_list(
     position_list: SingleSensorPositionList,
     position_list_type: Optional[_ALLOWED_TRAJ_LIST_TYPES] = None,
     raise_exception: bool = False,
@@ -1250,12 +1243,12 @@
         # In case correct index cols are remaining make them to regular columns
         df_just_right_index = df_just_right_index.reset_index()
 
     try:
         _assert_has_columns(df_just_right_index, [index_cols])
     except ValidationError as e:
         raise ValidationError(
-            "The dataframe is expected to have the following columns either in the index or as columns ({}), "
-            "but it has {}".format(index_cols, df.columns)
+            "The dataframe is expected to have the following columns either in the index or as columns "
+            f"({index_cols}), but it has {df.columns}"
         ) from e
 
     return df_just_right_index.set_index(index_cols)
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/exceptions.py` & `gaitmap-2.4.0/gaitmap/utils/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 class ValidationError(Exception):
     """An error indicating that data-object does not comply with the guidelines."""
 
 
 class GaitmapMadImportError(ImportError):
     """An error indicating that the algorithm is implemented in gaitmap-mad and not gaitmap."""
 
-    def __init__(self, object_name: str, module_name: str):
+    def __init__(self, object_name: str, module_name: str) -> None:
         self.object_name = object_name
         self.module_name = module_name
         super().__init__()
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Return a string representation of the error."""
         return (
             f"You are trying to import {self.object_name} from {self.module_name}."
             "\n\n"
             "This class/function is only available via the `gaitmap_mad` package that needs to be installed "
             "separately.\n"
-            "Install it using TODO: Update instructions.\n\n"
+            "Install it using `pip install gaitmap_mad`."
+            "Make sure you use the exact same version that you use for gaitmap as well.\n\n"
             "Warning: `gaitmap_mad` has a different license (AGPL3) than gaitmap. "
             "Make sure you understand what this means, before you proceed! "
             "See the README of gaitmap for more info."
         )
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/fast_quaternion_math.py` & `gaitmap-2.4.0/gaitmap/utils/fast_quaternion_math.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """A set of numba accelerated quaternion functions.
 
 Note that we follow the same order as :class:`~scipy.spatial.transform.Rotation` (x, y, z, w).
 """
+
 import numpy as np
 from numba import njit
 
 
 @njit()
 def rate_of_change_from_gyro(gyro: np.ndarray, current_orientation: np.ndarray) -> np.ndarray:
     """Rate of change of quaternion from gyroscope."""
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/rotations.py` & `gaitmap-2.4.0/gaitmap/utils/rotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """A set of util functions that ease handling rotations.
 
 All util functions use :class:`scipy.spatial.transform.Rotation` to represent rotations.
 """
-from typing import Callable, Dict, List, Optional, Union
+
+from typing import Callable, Optional, Union
 
 import numpy as np
 import pandas as pd
 from numpy.linalg import norm
 from scipy.spatial.transform import Rotation
 
 from gaitmap.utils.consts import GRAV_VEC, SF_ACC, SF_GYR
@@ -37,27 +38,27 @@
     Examples
     --------
     Single rotation: 180 deg rotation around the x-axis
 
     >>> rot = rotation_from_angle(np.array([1, 0, 0]), np.deg2rad(180))
     >>> rot.as_quat().round(decimals=3)
     array([1., 0., 0., 0.])
-    >>> rot.apply(np.array([[0, 0, 1.], [0, 1, 0.]])).round()
+    >>> rot.apply(np.array([[0, 0, 1.0], [0, 1, 0.0]])).round()
     array([[ 0., -0., -1.],
            [ 0., -1.,  0.]])
 
     Multiple rotations: 90 and 180 deg rotation around the x-axis
 
     >>> rot = rotation_from_angle(np.array([1, 0, 0]), np.deg2rad([90, 180]))
     >>> rot.as_quat().round(decimals=3)
     array([[0.707, 0.   , 0.   , 0.707],
            [1.   , 0.   , 0.   , 0.   ]])
     >>> # In case of multiple rotations, the first rotation is applied to the first vector
     >>> # and the second to the second
-    >>> rot.apply(np.array([[0, 0, 1.], [0, 1, 0.]])).round()
+    >>> rot.apply(np.array([[0, 0, 1.0], [0, 1, 0.0]])).round()
     array([[ 0., -1.,  0.],
            [ 0., -1.,  0.]])
 
     """
     angle = np.atleast_2d(angle)
     axis = np.atleast_2d(axis)
     return Rotation.from_rotvec(np.squeeze(axis * angle.T))
@@ -113,15 +114,15 @@
         return data
     data[SF_GYR] = rotation.apply(data[SF_GYR].to_numpy())
     data[SF_ACC] = rotation.apply(data[SF_ACC].to_numpy())
     return data
 
 
 def _rotate_or_flip_dataset(
-    dataset: SensorData, rotation: Union[Rotation, Dict[str, Rotation]], single_rot_method: Callable
+    dataset: SensorData, rotation: Union[Rotation, dict[str, Rotation]], single_rot_method: Callable
 ):
     dataset_type = is_sensor_data(dataset, frame="sensor")
     if dataset_type == "single":
         if isinstance(rotation, dict):
             raise ValueError(
                 "A Dictionary for the `rotation` parameter is only supported if a MultiIndex dataset (named sensors) is"
                 " passed."
@@ -143,15 +144,15 @@
 
     if isinstance(dataset, pd.DataFrame):
         # Restore original order
         rotated_dataset = rotated_dataset[original_cols]
     return rotated_dataset
 
 
-def flip_dataset(dataset: SensorData, rotation: Union[Rotation, Dict[str, Rotation]]) -> SensorData:
+def flip_dataset(dataset: SensorData, rotation: Union[Rotation, dict[str, Rotation]]) -> SensorData:
     """Flip datasets around axis data of a dataset.
 
     This is equivalent to rotating the data, but only 90/180 deg rotations are allowed.
     With this restriction, we don't need to actually rotate the data, but can just swap and flip the columns.
 
     This method should be used, when roughly aligning the data to a reference frame, where you usually would only
     apply 90 deg rotations based on the known rough orientation of the sensor.
@@ -178,15 +179,15 @@
     --------
     gaitmap.utils.rotations.rotate_dataset: Freely rotate a dataset
 
     """
     return _rotate_or_flip_dataset(dataset, rotation, _flip_sensor)
 
 
-def rotate_dataset(dataset: SensorData, rotation: Union[Rotation, Dict[str, Rotation]]) -> SensorData:
+def rotate_dataset(dataset: SensorData, rotation: Union[Rotation, dict[str, Rotation]]) -> SensorData:
     """Apply a rotation to acc and gyro data of a dataset.
 
     Parameters
     ----------
     dataset
         dataframe representing a single or multiple sensors.
         In case of multiple sensors a df with MultiIndex columns is expected where the first level is the sensor name
@@ -315,15 +316,15 @@
 
     """
     gravity_vector = normalize(gravity_vector)
     expected_gravity = normalize(expected_gravity)
     return find_shortest_rotation(gravity_vector, expected_gravity)
 
 
-def find_rotation_around_axis(rot: Rotation, rotation_axis: Union[np.ndarray, List]) -> Rotation:
+def find_rotation_around_axis(rot: Rotation, rotation_axis: Union[np.ndarray, list]) -> Rotation:
     """Calculate the rotation component of rot around the given rotation axis.
 
     This performs a swing-twist decomposition of the rotation quaternion [1]_.
     The returned rotation is the twist component of this decomposition.
     This is equivalent to the rotation around the rotation axis.
 
     Parameters
@@ -336,15 +337,15 @@
         axis for all rotations.
         In case n axis are provided for n rotations, the angle for each rotation is extracted around the respective
         axis.
 
     Examples
     --------
     >>> # Create composite rotation around y and z axis
-    >>> rot = Rotation.from_rotvec([0, 0, np.pi / 2]) * Rotation.from_rotvec([0, np.pi / 4, 0 ])
+    >>> rot = Rotation.from_rotvec([0, 0, np.pi / 2]) * Rotation.from_rotvec([0, np.pi / 4, 0])
     >>> find_rotation_around_axis(rot, [0, 0, 1]).as_rotvec()  # Extract part around z
     array([0.        , 0.        , 1.57079633])
     >>> find_rotation_around_axis(rot, [0, 1, 0]).as_rotvec()  # Extract part around y
     array([0.        , 0.78539816, 0.        ])
 
     Notes
     -----
@@ -440,15 +441,15 @@
     two vectors: 1D
 
     >>> find_unsigned_3d_angle(np.array([-1, 0, 0]), np.array([-1, 0, 0]))
     0
 
     two vectors: 2D
 
-    >>> find_unsigned_3d_angle(np.array([[-1, 0, 0],[-1, 0, 0]]), np.array([[-1, 0, 0],[-1, 0, 0]]))
+    >>> find_unsigned_3d_angle(np.array([[-1, 0, 0], [-1, 0, 0]]), np.array([[-1, 0, 0], [-1, 0, 0]]))
     array([0,0])
 
     """
     v1_, v2_ = np.atleast_2d(v1, v2)
     v1_ = normalize(v1_)
     v2_ = normalize(v2_)
     out = np.arccos(row_wise_dot(v1_, v2_) / (norm(v1_, axis=-1) * norm(v2_, axis=-1)))
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/signal_processing.py` & `gaitmap-2.4.0/gaitmap/utils/signal_processing.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
     Returns
     -------
     the filtered signal
 
     Examples
     --------
-    >>> data = np.arange(0,100)
-    >>> data_filtered = butter_lowpass_filter_1d(data = data, sampling_rate_hz = 10, cutoff_freq_hz = 1, order = 4)
+    >>> data = np.arange(0, 100)
+    >>> data_filtered = butter_lowpass_filter_1d(data=data, sampling_rate_hz=10, cutoff_freq_hz=1, order=4)
     >>> data_filtered
     array([0.00000000e+00, 4.82434336e-03, 4.03774045e-02, 1.66525148e-01,...])
 
     """
     b, a = butter(order, cutoff_freq_hz, btype="low", analog=False, fs=sampling_rate_hz)
     return lfilter(b, a, data)
 
@@ -49,15 +49,15 @@
 
     Returns
     -------
     A 2d array that holds the autocorrelation function for each row in the input array
 
     Examples
     --------
-    >>> t = np.arange(0,1,0.1)
+    >>> t = np.arange(0, 1, 0.1)
     >>> sin_wave = np.sin(t)
     >>> array = np.array([sin_wave, sin_wave])
     >>> out = row_wise_autocorrelation(array, 5)
     >>> out
     np.array([[2.38030226, 2.03883723, 1.68696752, 1.33807603, 1.00531772, 0.70139157],
        [2.38030226, 2.03883723, 1.68696752, 1.33807603, 1.00531772, 0.70139157]])
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/static_moment_detection.py` & `gaitmap-2.4.0/gaitmap/utils/static_moment_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """A set of util functions to detect static regions in a IMU signal given certain constrains."""
+
+from collections.abc import Sequence
 from functools import partial
-from typing import Callable, Optional, Sequence, Tuple, get_args
+from typing import Callable, Optional, get_args
 
 import numpy as np
 from numpy.linalg import norm
 from typing_extensions import Literal
 
 from gaitmap.utils import array_handling
 from gaitmap.utils.array_handling import _bool_fill
@@ -13,15 +15,15 @@
 # supported metric functions
 _METRIC_FUNCTIONS = {"maximum": np.nanmax, "variance": np.nanvar, "mean": np.nanmean, "median": np.nanmedian}
 METRIC_FUNCTION_NAMES = Literal["maximum", "variance", "mean", "median", "squared_mean"]  # pylint: disable=invalid-name
 
 
 def _window_apply_threshold(
     data, window_length: int, overlap: int, func: Callable[[np.ndarray], np.ndarray], threshold: float
-) -> Tuple[np.ndarray, int, float]:
+) -> tuple[np.ndarray, int, float]:
     # allocate output array
     inactive_signal_bool_array = np.zeros(len(data))
 
     windowed_norm = np.atleast_2d(array_handling.sliding_window_view(data, window_length, overlap, nan_padding=False))
     values = func(windowed_norm)
     is_static = np.broadcast_to(values <= threshold, windowed_norm.shape[::-1]).T
 
@@ -40,15 +42,15 @@
 
 def find_static_samples(
     signal: np.ndarray,
     window_length: int,
     inactive_signal_th: float,
     metric: METRIC_FUNCTION_NAMES = "mean",
     overlap: Optional[int] = None,
-) -> Tuple[np.ndarray, int, float]:
+) -> tuple[np.ndarray, int, float]:
     """Search for static samples within given input signal, based on windowed L2-norm thresholding.
 
     .. warning::
         Due to edge cases at the end of the input data where window size and overlap might not fit your data, the last
         window might be discarded for analysis and will therefore always be considered as non-static!
 
     Parameters
@@ -92,15 +94,15 @@
         Value of the given metric at the sample with the lowest value of the given metric or rather the window with the
         lowest value.
         Note, that this value can be larger than the threshold, if no ZUPTs were detected.
 
     Examples
     --------
     >>> test_data = load_gyro_data(path)
-    >>> get_static_moments(gyro_data, window_length=128, overlap=64, inactive_signal_th = 5, metric = 'mean')
+    >>> get_static_moments(gyro_data, window_length=128, overlap=64, inactive_signal_th=5, metric="mean")
 
     References
     ----------
     .. [1] I. Skog, J.-O. Nilsson, P. Händel, and J. Rantakokko, “Zero-velocity detection—An algorithm evaluation,”
        IEEE Trans. Biomed. Eng., vol. 57, no. 11, pp. 2657-2666, Nov. 2010.
 
     See Also
@@ -115,15 +117,15 @@
     if metric not in get_args(METRIC_FUNCTION_NAMES):
         raise ValueError(f"Invalid metric passed! {metric} as metric is not supported.")
 
     # check if minimum signal length matches window length
     if window_length > len(signal):
         raise ValueError(
             "Invalid window length, window must be smaller or equal than given signal length. Given signal length: "
-            "{} with given window_length: {}.".format(len(signal), window_length)
+            f"{len(signal)} with given window_length: {window_length}."
         )
 
     # add default overlap value
     if overlap is None:
         overlap = window_length - 1
 
     # calculate norm of input signal (do this outside of loop to boost performance at cost of memory!)
@@ -142,15 +144,15 @@
     acc: np.ndarray,
     gyr: np.ndarray,
     acc_noise_var: float,
     gyr_noise_var: float,
     window_length: int,
     inactive_signal_th: float,
     overlap: Optional[int] = None,
-) -> Tuple[np.ndarray, int, float]:
+) -> tuple[np.ndarray, int, float]:
     """Use the SHOE algorithm for static moment detection.
 
     This is based on the papers [1]_ and [2]_ and uses as weighted sum of the gravity corrected acc and the gyro norm to
     detect the static moments.
 
     Parameters
     ----------
@@ -217,15 +219,15 @@
 
 
 def find_static_sequences(
     signal: np.ndarray,
     window_length: int,
     inactive_signal_th: float,
     metric: METRIC_FUNCTION_NAMES = "mean",
-    overlap: int = None,
+    overlap: Optional[int] = None,
 ) -> np.ndarray:
     """Search for static sequences within given input signal, based on windowed L2-norm thresholding.
 
     .. warning::
         Due to edge cases at the end of the input data where window size and overlap might not fit your data, the last
         window might be discarded for analysis and will therefore always be considered as non-static!
 
@@ -278,15 +280,15 @@
         overlap=overlap,
     )
     return array_handling.bool_array_to_start_end_array(static_moment_bool_array)
 
 
 def find_first_static_window_multi_sensor(
     signals: Sequence[np.ndarray], window_length: int, inactive_signal_th: float, metric: METRIC_FUNCTION_NAMES
-) -> Tuple[int, int]:
+) -> tuple[int, int]:
     """Find the first time window in the signal where all provided sensors are static.
 
     Parameters
     ----------
     signals : Sequence of n arrays with shape (k, m) or a 3D-array with shape (k, n, m)
         The signals of n senors with m axis and k samples.
     window_length
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/stride_list_conversion.py` & `gaitmap-2.4.0/gaitmap/utils/stride_list_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """A couple of utils to convert stride lists into different formats."""
-from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
 from gaitmap.utils.consts import SL_EVENT_ORDER, SL_INDEX
 from gaitmap.utils.datatype_helper import (
@@ -43,15 +42,15 @@
         k: _segmented_stride_list_to_min_vel_single_sensor(v, target_stride_type=target_stride_type)[0]
         for k, v in stride_list.items()
     }
 
 
 def _segmented_stride_list_to_min_vel_single_sensor(
     stride_list: SingleSensorStrideList, target_stride_type: Literal["min_vel", "ic"]
-) -> Tuple[SingleSensorStrideList, SingleSensorStrideList]:
+) -> tuple[SingleSensorStrideList, SingleSensorStrideList]:
     """Convert a segmented stride list with detected events into other types of stride lists.
 
     During the conversion some strides might be removed.
     For more information about the different types of stride lists see the :ref:`stride list guide <stride_list_guide>`.
 
     Note, this function does not check if the input is a proper stride list.
 
@@ -110,15 +109,15 @@
     return converted_stride_list, stride_list[~stride_list.index.isin(converted_stride_list.index)]
 
 
 def enforce_stride_list_consistency(
     stride_list: SingleSensorStrideList,
     stride_type=Literal["segmented", "min_vel", "ic"],
     check_stride_list: bool = True,
-) -> Tuple[SingleSensorStrideList, SingleSensorStrideList]:
+) -> tuple[SingleSensorStrideList, SingleSensorStrideList]:
     """Exclude those strides where the gait events do not match the expected order or contain NaN.
 
     Correct order in depends on the stride type:
 
     - segmented: ["tc", "ic", "min_vel"]
     - min_vel: ["pre_ic", "min_vel", "tc", "ic"]
     - ic: ["ic", "min_vel", "tc"]
@@ -164,15 +163,15 @@
 
     return stride_list[bool_map], stride_list[~bool_map]
 
 
 def intersect_stride_list(
     stride_event_list: SingleSensorStrideList,
     regions_of_interest: SingleSensorRegionsOfInterestList,
-) -> List[SingleSensorStrideList]:
+) -> list[SingleSensorStrideList]:
     """Split the stride list into multiple stride lists based on the regions of interest.
 
     All events in the returned stride lists are made relative to the start of the region of interest.
 
     In all cases, only strides that are fully contained within a region of interest are included in the output stride
     lists.
```

### Comparing `gaitmap-2.3.0/gaitmap/utils/vector_math.py` & `gaitmap-2.4.0/gaitmap/utils/vector_math.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """A set of helper functions to handle common vector operations.
 
 Wherever possible, these functions are designed to handle multiple vectors at the same time to perform efficient
 computations.
 """
+
 from typing import Union
 
 import numpy as np
 from numpy.linalg import norm
 
 
 def row_wise_dot(v1, v2, squeeze=False):
@@ -45,15 +46,15 @@
     >>> is_almost_parallel_or_antiparallel(np.array([0, 0, 1]), np.array([0, 0, 1]))
     True
     >>> is_almost_parallel_or_antiparallel(np.array([0, 0, 1]), np.array([0, 1, 0]))
     False
 
     array of vectors
 
-    >>> is_almost_parallel_or_antiparallel(np.array([[0, 0, 1],[0,1,0]]), np.array([[0, 0, 2],[1,0,0]]))
+    >>> is_almost_parallel_or_antiparallel(np.array([[0, 0, 1], [0, 1, 0]]), np.array([[0, 0, 2], [1, 0, 0]]))
     array([True,False])
 
     """
     return np.isclose(np.abs(row_wise_dot(normalize(v1), normalize(v2))), 1, rtol=rtol, atol=atol)
 
 
 def normalize(v: np.ndarray) -> np.ndarray:
@@ -76,15 +77,15 @@
     1D array
 
     >>> normalize(np.array([0, 0, 2]))
     array([0., 0., 1.])
 
     2D array
 
-    >>> normalize(np.array([[2, 0, 0],[2, 0, 0]]))
+    >>> normalize(np.array([[2, 0, 0], [2, 0, 0]]))
     array([[1., 0., 0.],
            [1., 0., 0.]])
 
     0 Array:
 
     >>> normalize(np.array([0, 0, 0]))
     array([nan, nan, nan])
@@ -139,15 +140,15 @@
         Returns the cross product of the two if they are not equal.
 
         Returns a random vector in the perpendicular plane if they are either parallel or antiparallel.
         (see :func:`find_random_orthogonal`
 
     Examples
     --------
-    >>> find_orthogonal(np.array([1, 0, 0]),np.array([-1, 0, 0]))
+    >>> find_orthogonal(np.array([1, 0, 0]), np.array([-1, 0, 0]))
     array([0, 0, -1])
 
     """
     if v1.ndim > 1 or v2.ndim > 1:
         raise ValueError(f"v1 and v2 need to be at max 1D (currently {v1.ndim}D and {v2.ndim}D")
     if is_almost_parallel_or_antiparallel(v1, v2):
         return find_random_orthogonal(v1)
```

### Comparing `gaitmap-2.3.0/gaitmap/zupt_detection/__init__.py` & `gaitmap-2.4.0/gaitmap/zupt_detection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A set of methods to detect static regions/zero-velocity regions (ZUPTS) in a signal."""
+
 from gaitmap.zupt_detection._base import PerSampleZuptDetectorMixin, RegionZuptDetectorMixin
 from gaitmap.zupt_detection._combo_zupt_detector import ComboZuptDetector
 from gaitmap.zupt_detection._moving_window_zupt_detector import AredZuptDetector, NormZuptDetector, ShoeZuptDetector
 from gaitmap.zupt_detection._stride_event_zupt_detector import StrideEventZuptDetector
 
 __all__ = [
     "NormZuptDetector",
```

### Comparing `gaitmap-2.3.0/gaitmap/zupt_detection/_base.py` & `gaitmap-2.4.0/gaitmap/zupt_detection/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.3.0/gaitmap/zupt_detection/_combo_zupt_detector.py` & `gaitmap-2.4.0/gaitmap/zupt_detection/_combo_zupt_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Literal, Optional, Tuple
+from typing import Literal, Optional
 
 import numpy as np
 from typing_extensions import Self
 
 from gaitmap.base import BaseZuptDetector
 from gaitmap.utils.datatype_helper import SingleSensorData
 from gaitmap.zupt_detection._base import PerSampleZuptDetectorMixin
@@ -38,20 +38,20 @@
     min_vel_index_
         Always None. Only implemented for API compatibility.
 
     """
 
     _composite_params = ("detectors",)
 
-    detectors: Optional[List[Tuple[str, BaseZuptDetector]]]
+    detectors: Optional[list[tuple[str, BaseZuptDetector]]]
     operation: Literal["and", "or"]
 
     def __init__(
-        self, detectors: Optional[List[Tuple[str, BaseZuptDetector]]] = None, operation: Literal["and", "or"] = "or"
-    ):
+        self, detectors: Optional[list[tuple[str, BaseZuptDetector]]] = None, operation: Literal["and", "or"] = "or"
+    ) -> None:
         self.detectors = detectors
         self.operation = operation
 
     def detect(
         self,
         data: SingleSensorData,
         *,
```

### Comparing `gaitmap-2.3.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py` & `gaitmap-2.4.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A Basic ZUPT detector based on moving windows on the norm."""
-from typing import Optional, Tuple
+
+from typing import Optional
 
 import numpy as np
 from typing_extensions import Literal, Self
 
 from gaitmap.base import BaseZuptDetector
 from gaitmap.utils.datatype_helper import SingleSensorData, is_single_sensor_data
 from gaitmap.utils.exceptions import ValidationError
@@ -14,15 +15,15 @@
 
 
 def _validate_window(
     window_length_s: float,
     window_overlap: Optional[float],
     window_overlap_samples: Optional[int],
     sampling_rate_hz: float,
-) -> Tuple[int, Optional[int]]:
+) -> tuple[int, Optional[int]]:
     """Validate window_length and overlap."""
     window_length = round(sampling_rate_hz * window_length_s)
     if window_length < 3:
         raise ValidationError(
             f"The effective window size is smaller than 3 samples (`sampling_rate_hz`={sampling_rate_hz}, "
             f"`window_length_s={window_length_s}`). "
             "Specify a larger window length."
@@ -180,15 +181,15 @@
         *,
         sensor: SENSOR_NAMES = "gyr",
         window_length_s: float = 0.15,
         window_overlap: Optional[float] = 0.5,
         window_overlap_samples: Optional[int] = None,
         metric: METRIC_FUNCTION_NAMES = "mean",
         inactive_signal_threshold: float = 15,
-    ):
+    ) -> None:
         self.sensor = sensor
         self.window_length_s = window_length_s
         self.window_overlap = window_overlap
         self.window_overlap_samples = window_overlap_samples
         self.metric = metric
         self.inactive_signal_threshold = inactive_signal_threshold
 
@@ -329,15 +330,15 @@
         *,
         sensor: SENSOR_NAMES = "gyr",
         window_length_s: float = 0.15,
         window_overlap: Optional[float] = None,
         window_overlap_samples: Optional[int] = -1,
         metric: METRIC_FUNCTION_NAMES = "squared_mean",
         inactive_signal_threshold: float = 180,
-    ):
+    ) -> None:
         super().__init__(
             sensor=sensor,
             window_length_s=window_length_s,
             window_overlap=window_overlap,
             window_overlap_samples=window_overlap_samples,
             metric=metric,
             inactive_signal_threshold=inactive_signal_threshold,
@@ -455,15 +456,15 @@
         *,
         acc_noise_variance: float = 3.5e-9,
         gyr_noise_variance: float = 1.3e-7,
         window_length_s: float = 0.15,
         window_overlap: Optional[float] = 0.5,
         window_overlap_samples: Optional[int] = None,
         inactive_signal_threshold: float = 2310129700,
-    ):
+    ) -> None:
         self.acc_noise_variance = acc_noise_variance
         self.gyr_noise_variance = gyr_noise_variance
         self.window_length_s = window_length_s
         self.window_overlap = window_overlap
         self.window_overlap_samples = window_overlap_samples
         self.inactive_signal_threshold = inactive_signal_threshold
```

### Comparing `gaitmap-2.3.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py` & `gaitmap-2.4.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         Always None. Only implemented for API compatibility.
 
     """
 
     half_region_size_s: float
     half_region_size_samples_: int
 
-    def __init__(self, half_region_size_s: float = 0.05):
+    def __init__(self, half_region_size_s: float = 0.05) -> None:
         self.half_region_size_s = half_region_size_s
 
     def detect(
         self,
         data: SingleSensorData,
         *,
         stride_event_list: Optional[SingleSensorStrideList] = None,
```

### Comparing `gaitmap-2.3.0/PKG-INFO` & `gaitmap-2.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: gaitmap
-Version: 2.3.0
+Version: 2.4.0
 Summary: The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis.
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: MIT
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
-Requires-Python: >=3.8.0,<4.0
+Requires-Python: >=3.9.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: hmm
 Provides-Extra: stats
 Requires-Dist: joblib (>=1.2.0)
 Requires-Dist: numba (>=0.55)
 Requires-Dist: numba (>=0.55.2) ; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: pandas (>=2)
 Requires-Dist: pingouin (>=0.5.3,<0.6.0) ; extra == "stats" or extra == "all"
 Requires-Dist: pomegranate (>=0.14.2,<=0.14.6) ; (python_version < "3.10") and (extra == "hmm" or extra == "all")
 Requires-Dist: pooch (>=1.7.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.1)
 Requires-Dist: scipy (>=1.6.1)
-Requires-Dist: tpcp (>=0.15.0)
+Requires-Dist: tpcp (>=0.32.0,<0.33.0)
 Requires-Dist: typing_extensions (>=4.1.1)
 Project-URL: Repository, https://github.com/mad-lab-fau/gaitmap
 Description-Content-Type: text/markdown
 
 <img src="./docs/_static/logo/gaitmap_logo_with_text.png" height="200">
 
 [![PyPI](https://img.shields.io/pypi/v/gaitmap)](https://pypi.org/project/gaitmap/)
 [![pipeline status](https://github.com/mad-lab-fau/gaitmap/workflows/Test%20and%20Lint/badge.svg)](https://github.com/mad-lab-fau/gaitmap/actions/workflows/test-and-lint.yml)
 [![codecov](https://codecov.io/gh/mad-lab-fau/gaitmap/branch/master/graph/badge.svg?token=5NP5ZZ3KGX)](https://codecov.io/gh/mad-lab-fau/gaitmap)
-[![Documentation Status](https://readthedocs.org/projects/gaitmap/badge/?version=latest)](https://gaitmap.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/gaitmap/badge/?version=latest)](https://gaitmap.readthedocs.io/en/latest/README.html)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gaitmap)
 
 # gaitmap - The Gait and Movement Analysis Package
 
 *gaitmap* provides a set of algorithms to analyze your IMU movement data (with a focus on foot-worn IMUs) without 
 getting into your way.
 
 - 💻 [20+ Algorithms](https://gaitmap.readthedocs.io/en/latest/modules/index.html) from 17+ publications
 - 📚 Extensive [documentation](https://gaitmap.readthedocs.io/en/latest/)
 - 📝 Build to be [easily extendable](https://gaitmap.readthedocs.io/en/latest/source/user_guide/create_own_algorithm.html)
 - ⚙️ Familiar API inspired by scikit-learn
 - 🤝 Interoperable with the other libraries from the gaitmap ecosystem ([gaitmap-dataset](https://github.com/mad-lab-fau/gaitmap-datasets), [tpcp](https://github.com/mad-lab-fau/tpcp), ...)
 
-**Documentation:** [gaitmap.readthedocs.io](https://gaitmap.readthedocs.io/en/latest/)<br>
-**Learn More about the gaitmap ecosystem:** Coming soon!
+**Documentation:** [gaitmap.readthedocs.io](https://gaitmap.readthedocs.io/en/latest/README.html)<br>
+**Learn more about the gaitmap ecosystem:** [the gaitmap ecosystem](https://gaitmap.readthedocs.io/en/latest/source/user_guide/gaitmap_ecosystem.html)
 
 ## Installation
 
 Gaitmap is split into two packages: `gaitmap` and `gaitmap_mad` ([Learn more](https://gaitmap.readthedocs.io/en/latest/source/user_guide/gaitmap_mad.html)).
 To get access to all available algorithms, you need to install both packages:
 
 ```bash
@@ -100,16 +100,16 @@
 Python 3.10.
 
 We are working on upgrading to a newer version of `pomegranate`, but this is not a priority at the moment.
 You can track the progress in the [pull request](https://github.com/mad-lab-fau/gaitmap/pull/20).
 
 ### Supported Python versions
 
-*gaitmap* is tested against Python 3.8 and 3.9 at the moment.
-We expect most features to work with all Python versions >= 3.8, but because of some known issues 
+*gaitmap* is tested against Python 3.9 at the moment.
+We expect most features to work with all Python versions >= 3.9, but because of some known issues 
 (see specific features above) we do not officially support them.
 
 ## Working with Algorithms
 
 *gaitmap* is designed to be a toolbox and not a single algorithm.
 This means, that you are expected to pick and use individual algorithms.
 
@@ -171,16 +171,31 @@
 For all these topics check out our [contributing guide](https://gaitmap.readthedocs.io/en/latest/source/user_guide/contributing.html) for more details.
 
 ## Citation
 
 If you use *gaitmap* in your research we would appreciate a citation.
 This helps us to justify the time we invest in the development and maintenance of the library.
 
-We currently prepare a paper to describe the *gaitmap* library in detail.
-Until then, please simply cite the repository.
+
+> A. Küderle et al., "Gaitmap—An Open Ecosystem for IMU-Based Human Gait Analysis and Algorithm Benchmarking," in IEEE Open Journal of Engineering in Medicine and Biology, vol. 5, pp. 163-172, 2024, doi: 10.1109/OJEMB.2024.3356791.
+
+
+```bibtex
+@ARTICLE{10411039,
+  author={Küderle, Arne and Ullrich, Martin and Roth, Nils and Ollenschläger, Malte and Ibrahim, Alzhraa A. and Moradi, Hamid and Richer, Robert and Seifer, Ann-Kristin and Zürl, Matthias and Sîmpetru, Raul C. and Herzer, Liv and Prossel, Dominik and Kluge, Felix and Eskofier, Bjoern M.},
+  journal={IEEE Open Journal of Engineering in Medicine and Biology}, 
+  title={Gaitmap—An Open Ecosystem for IMU-Based Human Gait Analysis and Algorithm Benchmarking}, 
+  year={2024},
+  volume={5},
+  number={},
+  pages={163-172},
+  keywords={Pipelines;Benchmark testing;Software algorithms;Ecosystems;Machine learning algorithms;Estimation;Trajectory;Accelerometer;walking;biomarker;biomechanics;movement analysis},
+  doi={10.1109/OJEMB.2024.3356791}}
+```
+
 
 If you use a specific algorithm please also make sure you cite the original paper of the algorithm!
 We recommend the following citation style:
 
 *We used the algorithm proposed by Author et al. [paper-citation], implemented by the Gaitmap package [gaitmap-citation].*
 
 ## License
```

