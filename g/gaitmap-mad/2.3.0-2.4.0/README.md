# Comparing `tmp/gaitmap_mad-2.3.0.tar.gz` & `tmp/gaitmap_mad-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap_mad-2.3.0.tar", max compression
+gzip compressed data, was "gaitmap_mad-2.4.0.tar", max compression
```

## Comparing `gaitmap_mad-2.3.0.tar` & `gaitmap_mad-2.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      734 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/LICENSE
--rw-r--r--   0        0        0      597 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/README.md
--rw-r--r--   0        0        0      481 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/__init__.py
--rw-r--r--   0        0        0      441 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/event_detection/__init__.py
--rw-r--r--   0        0        0     6013 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py
--rw-r--r--   0        0        0    14317 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/event_detection/_rampp_event_detection.py
--rw-r--r--   0        0        0      340 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/gait_detection/__init__.py
--rw-r--r--   0        0        0    24779 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py
--rw-r--r--   0        0        0      117 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/preprocessing/__init__.py
--rw-r--r--   0        0        0      234 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0    12666 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py
--rw-r--r--   0        0        0     1114 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/__init__.py
--rw-r--r--   0        0        0      813 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/__init__.py
--rw-r--r--   0        0        0    15216 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py
--rw-r--r--   0        0        0    36773 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py
--rw-r--r--   0        0        0     8809 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py
--rw-r--r--   0        0        0      436 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/__init__.py
--rw-r--r--   0        0        0     7513 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv
--rw-r--r--   0        0        0    15956 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py
--rw-r--r--   0        0        0     3589 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py
--rw-r--r--   0        0        0     1184 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/__init__.py
--rw-r--r--   0        0        0    10922 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py
--rw-r--r--   0        0        0    12589 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py
--rw-r--r--   0        0        0        0 2023-08-03 11:17:31.005154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/__init__.py
--rw-r--r--   0        0        0   397824 2023-08-03 11:17:31.009154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json
--rw-r--r--   0        0        0    27245 2023-08-03 11:17:31.009154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py
--rw-r--r--   0        0        0    19087 2023-08-03 11:17:31.009154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py
--rw-r--r--   0        0        0    26902 2023-08-03 11:17:31.009154 gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_utils.py
--rw-r--r--   0        0        0      265 2023-08-03 11:17:31.009154 gaitmap_mad-2.3.0/gaitmap_mad/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0      263 2023-08-03 11:17:31.009154 gaitmap_mad-2.3.0/gaitmap_mad/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0    10862 2023-08-03 11:17:31.009154 gaitmap_mad-2.3.0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py
--rw-r--r--   0        0        0      589 2023-08-03 11:17:31.009154 gaitmap_mad-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 gaitmap_mad-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0      734 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/LICENSE
+-rw-r--r--   0        0        0      597 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/README.md
+-rw-r--r--   0        0        0      482 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/event_detection/__init__.py
+-rw-r--r--   0        0        0     6009 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py
+-rw-r--r--   0        0        0    14305 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/event_detection/_rampp_event_detection.py
+-rw-r--r--   0        0        0      340 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/gait_detection/__init__.py
+-rw-r--r--   0        0        0    24803 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py
+-rw-r--r--   0        0        0      117 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/preprocessing/__init__.py
+-rw-r--r--   0        0        0      234 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0    12668 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py
+-rw-r--r--   0        0        0     1115 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0      814 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/__init__.py
+-rw-r--r--   0        0        0    15231 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py
+-rw-r--r--   0        0        0    36710 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py
+-rw-r--r--   0        0        0     8812 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py
+-rw-r--r--   0        0        0      436 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/__init__.py
+-rw-r--r--   0        0        0     7513 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv
+-rw-r--r--   0        0        0    16016 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py
+-rw-r--r--   0        0        0     3563 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py
+-rw-r--r--   0        0        0     1185 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/__init__.py
+-rw-r--r--   0        0        0    11514 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py
+-rw-r--r--   0        0        0    12637 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:35:18.327953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/__init__.py
+-rw-r--r--   0        0        0   397824 2024-04-19 10:35:18.331953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json
+-rw-r--r--   0        0        0    27238 2024-04-19 10:35:18.331953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py
+-rw-r--r--   0        0        0    19115 2024-04-19 10:35:18.331953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py
+-rw-r--r--   0        0        0    26896 2024-04-19 10:35:18.331953 gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_utils.py
+-rw-r--r--   0        0        0      265 2024-04-19 10:35:18.331953 gaitmap_mad-2.4.0/gaitmap_mad/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-19 10:35:18.331953 gaitmap_mad-2.4.0/gaitmap_mad/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0    10706 2024-04-19 10:35:18.331953 gaitmap_mad-2.4.0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py
+-rw-r--r--   0        0        0      589 2024-04-19 10:35:18.331953 gaitmap_mad-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 gaitmap_mad-2.4.0/PKG-INFO
```

### Comparing `gaitmap_mad-2.3.0/LICENSE` & `gaitmap_mad-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.3.0/README.md` & `gaitmap_mad-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py` & `gaitmap_mad-2.4.0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """The event detection algorithm by Rampp et al. 2014."""
-from typing import Dict, Optional, Tuple
+
+from typing import Optional
 
 from joblib import Memory
 from tpcp import cf
 
 from gaitmap.data_transform import BaseFilter, ButterworthFilter
 from gaitmap_mad.event_detection._rampp_event_detection import RamppEventDetection
 
@@ -86,26 +87,26 @@
 
     """
 
     ic_lowpass_filter: BaseFilter
 
     def __init__(
         self,
-        ic_search_region_ms: Tuple[float, float] = (80, 50),
+        ic_search_region_ms: tuple[float, float] = (80, 50),
         min_vel_search_win_size_ms: float = 100,
         ic_lowpass_filter: BaseFilter = cf(ButterworthFilter(order=2, cutoff_freq_hz=15)),
         memory: Optional[Memory] = None,
         enforce_consistency: bool = True,
-        detect_only: Optional[Tuple[str, ...]] = None,
-    ):
+        detect_only: Optional[tuple[str, ...]] = None,
+    ) -> None:
         self.ic_lowpass_filter = ic_lowpass_filter
         super().__init__(
             memory=memory,
             enforce_consistency=enforce_consistency,
             ic_search_region_ms=ic_search_region_ms,
             min_vel_search_win_size_ms=min_vel_search_win_size_ms,
             detect_only=detect_only,
         )
 
-    def _get_detect_kwargs(self) -> Dict:
+    def _get_detect_kwargs(self) -> dict:
         parent_kwargs = super()._get_detect_kwargs()
         return {**parent_kwargs, "gyr_ic_lowpass_filter": self.ic_lowpass_filter}
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/event_detection/_rampp_event_detection.py` & `gaitmap_mad-2.4.0/gaitmap_mad/event_detection/_rampp_event_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """The event detection algorithm by Rampp et al. 2014."""
-from typing import Callable, Dict, Optional, Tuple, Union, cast
+
+from typing import Callable, Optional, Union, cast
 
 import numpy as np
 import pandas as pd
 from joblib import Memory
 
 from gaitmap._event_detection_common._event_detection_mixin import _detect_min_vel_gyr_energy, _EventDetectionMixin
 from gaitmap.base import BaseEventDetection
@@ -147,63 +148,63 @@
 
     .. [1] Rampp, A., Barth, J., Schülein, S., Gaßmann, K. G., Klucken, J., & Eskofier, B. M. (2014). Inertial
        sensor-based stride parameter calculation from gait sequences in geriatric patients. IEEE transactions on
        biomedical engineering, 62(4), 1089-1097.. https://doi.org/10.1109/TBME.2014.2368211
 
     """
 
-    ic_search_region_ms: Tuple[float, float]
+    ic_search_region_ms: tuple[float, float]
     min_vel_search_win_size_ms: float
 
     def __init__(
         self,
-        ic_search_region_ms: Tuple[float, float] = (80, 50),
+        ic_search_region_ms: tuple[float, float] = (80, 50),
         min_vel_search_win_size_ms: float = 100,
         memory: Optional[Memory] = None,
         enforce_consistency: bool = True,
-        detect_only: Optional[Tuple[str, ...]] = None,
-    ):
+        detect_only: Optional[tuple[str, ...]] = None,
+    ) -> None:
         self.ic_search_region_ms = ic_search_region_ms
         self.min_vel_search_win_size_ms = min_vel_search_win_size_ms
         super().__init__(memory=memory, enforce_consistency=enforce_consistency, detect_only=detect_only)
 
     def _select_all_event_detection_method(self) -> Callable:
         """Select the function to calculate the all events.
 
         This is separate method to make it easy to overwrite by a subclass.
         """
         return _find_all_events
 
-    def _get_detect_kwargs(self) -> Dict[str, Union[Tuple[int, int], int]]:
+    def _get_detect_kwargs(self) -> dict[str, Union[tuple[int, int], int]]:
         ic_search_region = cast(
-            Tuple[int, int], tuple(int(v / 1000 * self.sampling_rate_hz) for v in self.ic_search_region_ms)
+            tuple[int, int], tuple(int(v / 1000 * self.sampling_rate_hz) for v in self.ic_search_region_ms)
         )
         if all(v == 0 for v in ic_search_region):
             raise ValueError(
-                "The chosen values are smaller than the sample time ({} ms)".format((1 / self.sampling_rate_hz) * 1000)
+                f"The chosen values are smaller than the sample time ({(1 / self.sampling_rate_hz) * 1000} ms)"
             )
         min_vel_search_win_size = int(self.min_vel_search_win_size_ms / 1000 * self.sampling_rate_hz)
         return {
             "ic_search_region": ic_search_region,
             "min_vel_search_win_size": min_vel_search_win_size,
             "sampling_rate_hz": self.sampling_rate_hz,
             "gyr_ic_lowpass_filter": None,
         }
 
 
 def _find_all_events(
     gyr: pd.DataFrame,
     acc: pd.DataFrame,
     stride_list: pd.DataFrame,
-    events: Tuple[str, ...],
-    ic_search_region: Tuple[float, float],
+    events: tuple[str, ...],
+    ic_search_region: tuple[float, float],
     min_vel_search_win_size: int,
     sampling_rate_hz: float,
     gyr_ic_lowpass_filter: Optional[BaseFilter],
-) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Find events in provided data by looping over single strides."""
     gyr_ml = gyr["gyr_ml"]
 
     if "ic" in events:
         if gyr_ic_lowpass_filter is not None:
             gyr_ml_filtered = gyr_ic_lowpass_filter.filter(
                 gyr_ml, sampling_rate_hz=sampling_rate_hz
@@ -235,15 +236,15 @@
         np.array(ic_events, dtype=float) if ic_events else None,
         np.array(tc_events, dtype=float) if tc_events else None,
         np.array(min_vel_events, dtype=float) if min_vel_events else None,
     )
 
 
 def _detect_ic(
-    gyr_ml: np.ndarray, acc_pa_inv: np.ndarray, gyr_ml_grad: np.ndarray, ic_search_region: Tuple[float, float]
+    gyr_ml: np.ndarray, acc_pa_inv: np.ndarray, gyr_ml_grad: np.ndarray, ic_search_region: tuple[float, float]
 ) -> float:
     """Find the ic.
 
     Note, that this implementation expects the inverted signal of acc_pa compared to the normal bodyframe definition
     in gaitmap.
     This is because the algorithm was originally developed considering a different coordinate system.
     To keep the logic identical to the original paper, we pass in the inverted signal axis (see parent function)
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py` & `gaitmap_mad-2.4.0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The gait sequence detection algorithm by Ullrich et al. 2020."""
+
 import copy
 import itertools
-from typing import Dict, Tuple, TypeVar, Union
+from typing import Optional, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 from numpy.linalg import norm
 from scipy.fft import rfft
 from scipy.signal import peak_prominences
 
@@ -142,20 +143,20 @@
     sampling_rate_hz: float
 
     def __init__(
         self,
         sensor_channel_config: str = "gyr_ml",
         peak_prominence: float = 17.0,
         window_size_s: float = 10,
-        active_signal_threshold: float = None,
-        locomotion_band: Tuple[float, float] = (0.5, 3),
+        active_signal_threshold: Optional[float] = None,
+        locomotion_band: tuple[float, float] = (0.5, 3),
         harmonic_tolerance_hz: float = 0.3,
         merge_gait_sequences_from_sensors: bool = False,
-        additional_margin_s: float = None,
-    ):
+        additional_margin_s: Optional[float] = None,
+    ) -> None:
         self.sensor_channel_config = sensor_channel_config
         self.peak_prominence = peak_prominence
         self.window_size_s = window_size_s
         self.active_signal_threshold = active_signal_threshold
         self.locomotion_band = locomotion_band
         self.harmonic_tolerance_hz = harmonic_tolerance_hz
         self.merge_gait_sequences_from_sensors = merge_gait_sequences_from_sensors
@@ -184,40 +185,40 @@
 
         window_size = int(self.window_size_s * self.sampling_rate_hz)
 
         dataset_type = is_sensor_data(self.data)
         if dataset_type == "single":
             results = self._detect_single_dataset(data, window_size)
         else:  # Multisensor
-            results_dict: Dict[_Hashable, Dict[str, pd.DataFrame]] = {}
+            results_dict: dict[_Hashable, dict[str, pd.DataFrame]] = {}
             for sensor in get_multi_sensor_names(data):
                 results_dict[sensor] = self._detect_single_dataset(data[sensor], window_size)
             results = invert_result_dictionary(results_dict)
 
             if self.merge_gait_sequences_from_sensors:
                 results["gait_sequences"] = self._merge_gait_sequences_multi_sensor_data(results["gait_sequences"])
 
         set_params_from_dict(self, results, result_formatting=True)
         return self
 
     @property
-    def start_(self) -> Union[np.ndarray, Dict[_Hashable, np.ndarray]]:
+    def start_(self) -> Union[np.ndarray, dict[_Hashable, np.ndarray]]:
         """Just the start values of all gait sequences."""
         if isinstance(self.gait_sequences_, dict):
             return {k: np.array(v["start"]) for k, v in self.gait_sequences_.items()}
         return np.array(self.gait_sequences_["start"])
 
     @property
-    def end_(self) -> Union[np.ndarray, Dict[_Hashable, np.ndarray]]:
+    def end_(self) -> Union[np.ndarray, dict[_Hashable, np.ndarray]]:
         """Just the end values of all gait sequences."""
         if isinstance(self.gait_sequences_, dict):
             return {k: np.array(v["end"]) for k, v in self.gait_sequences_.items()}
         return np.array(self.gait_sequences_["end"])
 
-    def _detect_single_dataset(self, data: pd.DataFrame, window_size: int) -> Dict[str, pd.DataFrame]:
+    def _detect_single_dataset(self, data: pd.DataFrame, window_size: int) -> dict[str, pd.DataFrame]:
         """Detect gait sequences for a single sensor data set."""
         s_3d, s_1d, active_signal_th, fft_factor = self._signal_extraction(data)
 
         # sig_length is required later for the concatenation of gait sequences
         sig_length = len(s_1d)
 
         # lowpass filter the signal: this is now happening before the windowing and thus before the active signal
@@ -396,15 +397,15 @@
         # find valid windows with n_harmonics > threshold
         n_harmonics_threshold = 2  # 2 as defined in the paper
 
         valid_windows = n_harmonics >= n_harmonics_threshold
 
         return valid_windows
 
-    def _assert_input_data(self, data):
+    def _assert_input_data(self, data) -> None:
         if self.merge_gait_sequences_from_sensors and is_multi_sensor_data(data) and not isinstance(data, pd.DataFrame):
             raise ValueError("Merging of data set is only possible for synchronized data sets.")
 
         # check for correct input value for sensor_channel_config
         if isinstance(self.sensor_channel_config, str) and self.sensor_channel_config not in list(
             itertools.chain(BF_ACC, BF_GYR, ["gyr", "acc"])
         ):
@@ -425,24 +426,24 @@
         if self.locomotion_band[0] <= 0:
             raise ValueError("The first entry of the locomotion band must be larger than 0.")
 
         # check if 5 * upper freq range limit is close to nyquist freq (allow for a difference > 5 Hz). This would
         # cause edge cases for the flattened fft peak detection later on.
         if (self.sampling_rate_hz / 2) - (5 * self.locomotion_band[1]) < 5:
             raise ValueError(
-                "The upper limit of the locomotion band ({} Hz) is too close to the Nyquist frequency ({} Hz) of the "
-                "signal, given the sampling rate of {} Hz. The difference between upper limit of locomotion band and "
-                "Nyquist frequency should be smaller than 5 Hz.".format(
-                    self.locomotion_band[1], self.sampling_rate_hz / 2, self.sampling_rate_hz
-                )
+                f"The upper limit of the locomotion band ({self.locomotion_band[1]} Hz) is too close to the Nyquist "
+                f"frequency ({self.sampling_rate_hz / 2} Hz) of the signal, given the sampling rate of "
+                f"{self.sampling_rate_hz} Hz. "
+                "The difference between upper limit of locomotion band and Nyquist frequency should be smaller than "
+                "5 Hz."
             )
 
     def _merge_gait_sequences_multi_sensor_data(
-        self, gait_sequences: Dict[_Hashable, pd.DataFrame]
-    ) -> Dict[_Hashable, pd.DataFrame]:
+        self, gait_sequences: dict[_Hashable, pd.DataFrame]
+    ) -> dict[_Hashable, pd.DataFrame]:
         """Merge gait sequences from different sensor positions for synced data.
 
         Gait sequences from individual sensors are merged using gaitmap.utils.array_handling.merge_intervals.
         The gait sequences are returned as a dictionary of pd.Dataframes with start and end samples of the merged gait
         sequences.
         """
         # In case all dataframes are empty, so no gait sequences were detected just return an empty dataframe.
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py` & `gaitmap_mad-2.4.0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Correct for 180 degree misalignments between sensor and foot coordinate frame based on forward direction."""
 
-from typing import Dict, Union
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from scipy.spatial.transform import Rotation
 from tpcp import cf
 from typing_extensions import Self
 
@@ -82,15 +82,15 @@
     Examples
     --------
     Estimate the sign of the forward direction velocity and apply a 0deg or 180deg flip on the data accordingly. This
     step is usually a subsequent step of a previous sign invariant alignment step like the PCA alignment.
 
     >>> fdsa = ForwardDirectionSignAlignment(forward_direction="x", rotation_axis="z", baseline_velocity_threshold=0.2)
     >>> fdsa = fdsa.align(data, 204.8)
-    >>> fdsa.aligned_data_['left_sensor']
+    >>> fdsa.aligned_data_["left_sensor"]
     <copy of dataset with axis aligned to the medio-lateral plane>
     ...
     >>> fdsa.is_flipped_  # True when the data was rotated by 180 deg, False afterwise
     True
 
     Notes
     -----
@@ -107,18 +107,18 @@
     ori_method: BaseOrientationMethod
     zupt_detector_orientation_init: BaseZuptDetector
     pos_method: BasePositionMethod
 
     data: SensorData
     sampling_rate_hz: float
 
-    rotation_: Union[Rotation, Dict[_Hashable, Rotation]]
-    is_flipped_: Union[bool, Dict[_Hashable, bool]]
-    pos_method_: Union[BasePositionMethod, Dict[_Hashable, BasePositionMethod]]
-    ori_method_: Union[BaseOrientationMethod, Dict[_Hashable, BaseOrientationMethod]]
+    rotation_: Union[Rotation, dict[_Hashable, Rotation]]
+    is_flipped_: Union[bool, dict[_Hashable, bool]]
+    pos_method_: Union[BasePositionMethod, dict[_Hashable, BasePositionMethod]]
+    ori_method_: Union[BaseOrientationMethod, dict[_Hashable, BaseOrientationMethod]]
 
     def __init__(
         self,
         forward_direction: str = "x",
         rotation_axis: str = "z",
         baseline_velocity_threshold: float = 0.2,
         ori_method: BaseOrientationMethod = cf(MadgwickAHRS(beta=0.1)),
@@ -128,15 +128,15 @@
         pos_method: BasePositionMethod = cf(
             PieceWiseLinearDedriftedIntegration(
                 NormZuptDetector(sensor="gyr", window_length_s=0.15, inactive_signal_threshold=15.0, metric="mean"),
                 level_assumption=False,
                 gravity=GRAV_VEC,
             )
         ),
-    ):
+    ) -> None:
         self.forward_direction = forward_direction
         self.rotation_axis = rotation_axis
         self.baseline_velocity_threshold = baseline_velocity_threshold
         self.ori_method = ori_method
         self.zupt_detector_orientation_init = zupt_detector_orientation_init
         self.pos_method = pos_method
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/__init__.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 The stride segmentation module includes all algorithms that are able to find stride candidates in a continuous sensor
 signal.
 Some are able to directly detect individual biomechanical events.
 Other algorithm are only able to detect stride candidates and need to be paired by an explicit event detection
 algorithm, as implemented in :py:mod:`gaitmap.event_detection`, to be able to provide information about biomechanical
 events.
 """
+
 from gaitmap_mad.stride_segmentation.dtw import (
     BarthDtw,
     BarthOriginalTemplate,
     BaseDtw,
     BaseDtwTemplate,
     ConstrainedBarthDtw,
     DtwTemplate,
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/__init__.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Dtw based Stride Segmentation."""
+
 from gaitmap_mad.stride_segmentation.dtw._barth_dtw import BarthDtw
 from gaitmap_mad.stride_segmentation.dtw._base_dtw import (
     BaseDtw,
     find_matches_find_peaks,
     find_matches_min_under_threshold,
 )
 from gaitmap_mad.stride_segmentation.dtw._constrained_barth_dtw import ConstrainedBarthDtw
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """The msDTW based stride segmentation algorithm by Barth et al 2013."""
+
 import warnings
-from typing import Dict, List, Optional, Tuple, Union
+from typing import NoReturn, Optional, Union
 
 import numpy as np
 import pandas as pd
 from joblib import Memory
 from tpcp import CloneFactory
 from typing_extensions import Literal
 
@@ -165,29 +166,29 @@
 
     snap_to_min_win_ms: Optional[float]
     snap_to_min_axis: Optional[str]
     conflict_resolution: bool
 
     def __init__(
         self,
-        template: Optional[Union[BaseDtwTemplate, Dict[_Hashable, BaseDtwTemplate]]] = CloneFactory(
+        template: Optional[Union[BaseDtwTemplate, dict[_Hashable, BaseDtwTemplate]]] = CloneFactory(
             BarthOriginalTemplate()
         ),
         resample_template: bool = True,
         find_matches_method: Literal["min_under_thres", "find_peaks"] = "find_peaks",
         max_cost: Optional[float] = 4.0,
         min_match_length_s: Optional[float] = 0.6,
         max_match_length_s: Optional[float] = 3.0,
         max_template_stretch_ms: Optional[float] = None,
         max_signal_stretch_ms: Optional[float] = None,
         snap_to_min_win_ms: Optional[float] = 300,
         snap_to_min_axis: Optional[str] = "gyr_ml",
         conflict_resolution: bool = True,
         memory: Optional[Memory] = None,
-    ):
+    ) -> None:
         self.snap_to_min_win_ms = snap_to_min_win_ms
         self.snap_to_min_axis = snap_to_min_axis
         self.conflict_resolution = conflict_resolution
         super().__init__(
             template=template,
             max_cost=max_cost,
             min_match_length_s=min_match_length_s,
@@ -204,15 +205,15 @@
         """Return start and end of each match as pd.DataFrame."""
         start_ends = self.matches_start_end_
         if isinstance(start_ends, dict):
             return {k: self._format_stride_list(v) for k, v in start_ends.items()}
         return self._format_stride_list(start_ends)
 
     @stride_list_.setter
-    def stride_list_(self, arg: StrideList):  # noqa: no-self-use
+    def stride_list_(self, arg: StrideList) -> NoReturn:  # noqa: ARG002
         """Fake setter for the stride list.
 
         This is required to be type compatible with the base class.
         """
         raise ValueError("The argument `stride_list_` is readonly.")
 
     @staticmethod
@@ -224,21 +225,21 @@
         # Add the s_id
         as_df.index.name = "s_id"
         return as_df
 
     def _postprocess_matches(
         self,
         data,
-        paths: List,
+        paths: list,
         cost: np.ndarray,
         matches_start_end: np.ndarray,
         acc_cost_mat: np.ndarray,
         to_keep: np.ndarray,
         memory: Memory,
-    ) -> Tuple[np.ndarray, np.ndarray]:
+    ) -> tuple[np.ndarray, np.ndarray]:
         # Apply snap to minimum
         if self.snap_to_min_win_ms:
             # Late import to avoid circular import
             from gaitmap.stride_segmentation._utils import snap_to_min  # pylint: disable=import-outside-toplevel
 
             matches_start_end = snap_to_min(
                 data[self.snap_to_min_axis].to_numpy(),
@@ -282,14 +283,14 @@
                 keep = np.argmin(cost_per_valid_stride[indices])
                 # Remove all strides except the one with the lowest cost.
                 to_keep[valid_indices[indices]] = False
                 to_keep[valid_indices[indices[keep]]] = True
 
         return matches_start_end, to_keep
 
-    def _post_postprocess_check(self, matches_start_end):
+    def _post_postprocess_check(self, matches_start_end) -> None:
         super()._post_postprocess_check(matches_start_end)
         # Check if there are still overlapping strides
         if np.any(np.diff(matches_start_end.flatten()) < 0):
             warnings.warn(
                 "There are still overlapping strides left after postprocessing. Please manually review the results."
             )
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A implementation of a sDTW that can be used independent of the context of Stride Segmentation."""
+
 import warnings
-from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, ClassVar, Optional, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 from joblib import Memory
 from numba import njit
 from scipy.interpolate import interp1d
 from typing_extensions import Literal
@@ -235,33 +236,36 @@
     array([[2, 4],
            [6, 8]])
 
     """
 
     _action_methods = ("segment",)
 
-    template: Optional[Union[BaseDtwTemplate, Dict[_Hashable, BaseDtwTemplate]]]
+    template: Optional[Union[BaseDtwTemplate, dict[_Hashable, BaseDtwTemplate]]]
     max_cost: Optional[float]
     resample_template: bool
     min_match_length_s: Optional[float]
     max_match_length_s: Optional[float]
     max_template_stretch_ms: Optional[float]
     max_signal_stretch_ms: Optional[float]
     find_matches_method: Literal["min_under_thres", "find_peaks"]
     memory: Optional[Memory]
 
-    matches_start_end_: Union[np.ndarray, Dict[_Hashable, np.ndarray]]
-    acc_cost_mat_: Union[np.ndarray, Dict[_Hashable, np.ndarray]]
-    paths_: Union[List[np.ndarray], Dict[_Hashable, List[np.ndarray]]]
-    costs_: Union[np.ndarray, Dict[_Hashable, np.ndarray]]
+    matches_start_end_: Union[np.ndarray, dict[_Hashable, np.ndarray]]
+    acc_cost_mat_: Union[np.ndarray, dict[_Hashable, np.ndarray]]
+    paths_: Union[list[np.ndarray], dict[_Hashable, list[np.ndarray]]]
+    costs_: Union[np.ndarray, dict[_Hashable, np.ndarray]]
 
     data: Union[np.ndarray, SensorData]
     sampling_rate_hz: float
 
-    _allowed_methods_map = {"min_under_thres": find_matches_min_under_threshold, "find_peaks": find_matches_find_peaks}
+    _allowed_methods_map: ClassVar = {
+        "min_under_thres": find_matches_min_under_threshold,
+        "find_peaks": find_matches_find_peaks,
+    }
     _min_sequence_length: Optional[float]
     _max_sequence_length: Optional[float]
     _max_template_stretch: Optional[int]
     _max_signal_stretch: Optional[int]
 
     @property
     def cost_function_(self):
@@ -269,36 +273,36 @@
         if isinstance(self.acc_cost_mat_, dict):
             return {s: np.sqrt(cost_mat[-1, :]) for s, cost_mat in self.acc_cost_mat_.items()}
         return np.sqrt(self.acc_cost_mat_[-1, :])
 
     @property
     def matches_start_end_original_(
         self,
-    ) -> Union[np.ndarray, Dict[_Hashable, np.ndarray]]:
+    ) -> Union[np.ndarray, dict[_Hashable, np.ndarray]]:
         """Return the starts and end directly from the paths.
 
         This will not be effected by potential changes of the postprocessing.
         """
         if isinstance(self.paths_, dict):
             # We add +1 here to adhere to the convention that the end index of a region/stride is exclusive.
             return {s: np.array([[p[0][-1], p[-1][-1] + 1] for p in path]) for s, path in self.paths_.items()}
         return np.array([[p[0][-1], p[-1][-1] + 1] for p in self.paths_])
 
     def __init__(
         self,
-        template: Optional[Union[BaseDtwTemplate, Dict[_Hashable, BaseDtwTemplate]]] = None,
+        template: Optional[Union[BaseDtwTemplate, dict[_Hashable, BaseDtwTemplate]]] = None,
         resample_template: bool = True,
         find_matches_method: Literal["min_under_thres", "find_peaks"] = "find_peaks",
         max_cost: Optional[float] = None,
         min_match_length_s: Optional[float] = None,
         max_match_length_s: Optional[float] = None,
         max_template_stretch_ms: Optional[float] = None,
         max_signal_stretch_ms: Optional[float] = None,
         memory: Optional[Memory] = None,
-    ):
+    ) -> None:
         self.template = template
         self.max_cost = max_cost
         self.min_match_length_s = min_match_length_s
         self.max_match_length_s = max_match_length_s
         self.max_template_stretch_ms = max_template_stretch_ms
         self.max_signal_stretch_ms = max_signal_stretch_ms
         self.resample_template = resample_template
@@ -333,15 +337,15 @@
         return self
 
     def _segment(
         self,
         data: Union[np.ndarray, SensorData],
         sampling_rate_hz: float,
         memory: Optional[Memory] = None,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         if not memory:
             memory = Memory(None)
 
         self._validate_basic_inputs()
 
         self._min_sequence_length = self.min_match_length_s
         if self._min_sequence_length is not None:
@@ -350,27 +354,27 @@
         if self._max_sequence_length is not None:
             self._max_sequence_length *= sampling_rate_hz
 
         # For the typechecker
         assert self.template is not None
 
         results: Union[
-            Dict[str, Union[np.ndarray, List[np.ndarray]]],
-            Dict[str, Dict[Union[_Hashable, str], Union[np.ndarray, List[np.ndarray]]]],
+            dict[str, Union[np.ndarray, list[np.ndarray]]],
+            dict[str, dict[Union[_Hashable, str], Union[np.ndarray, list[np.ndarray]]]],
         ]
         if isinstance(data, np.ndarray):
             dataset_type = "array"
         else:
             dataset_type = is_sensor_data(data, check_gyr=False, check_acc=False)
         template = self.template
         if dataset_type in ("single", "array"):
             # Single template single sensor: easy
             results = self._segment_single_dataset(data, template, memory=memory)
         else:  # Multisensor
-            result_dict: Dict[_Hashable, Dict[str, Union[np.ndarray, List[np.ndarray]]]] = {}
+            result_dict: dict[_Hashable, dict[str, Union[np.ndarray, list[np.ndarray]]]] = {}
             if isinstance(template, dict):
                 # multiple templates, multiple sensors: Apply the correct template to the correct sensor.
                 # Ignore the rest
                 for sensor, single_template in template.items():
                     result_dict[sensor] = self._segment_single_dataset(data[sensor], single_template, memory=memory)
             elif is_single_sensor_data(template.get_data(), check_gyr=False, check_acc=False):
                 # single template, multiple sensors: Apply template to all sensors
@@ -382,31 +386,31 @@
                     "`Dict[str, DtwTemplate]` or the template array must have the shape of a single-sensor dataframe."
                 )
             results = invert_result_dictionary(result_dict)
 
         return results
 
     def _segment_single_dataset(
-        self, dataset, template: Union[BaseDtwTemplate, Dict[_Hashable, BaseDtwTemplate]], memory: Memory
-    ) -> Dict[str, Union[np.ndarray, List[np.ndarray]]]:
+        self, dataset, template: Union[BaseDtwTemplate, dict[_Hashable, BaseDtwTemplate]], memory: Memory
+    ) -> dict[str, Union[np.ndarray, list[np.ndarray]]]:
         template_sampling_rate = getattr(template, "sampling_rate_hz", None)
         if self.resample_template and not template_sampling_rate:
             raise ValueError(
                 "To resample the template (`resample_template=True`), a `sampling_rate_hz` must be specified for the "
                 "template."
             )
         if (
             template_sampling_rate
             and self.sampling_rate_hz != template_sampling_rate
             and self.resample_template is False
         ):
             warnings.warn(
-                "The data and template sampling rate are different ({} Hz vs. {} Hz), "
-                "but `resample_template` is False. "
-                "This might lead to unexpected results".format(template_sampling_rate, self.sampling_rate_hz)
+                f"The data and template sampling rate are different ({template_sampling_rate} Hz vs. "
+                f"{self.sampling_rate_hz} Hz), but `resample_template` is False. "
+                "This might lead to unexpected results"
             )
 
         # Extract the parts of the data that is relevant for matching and apply potential data transforms defined in
         # the template.
         template_array, matching_data = self._extract_relevant_data_and_template(
             template, dataset, self.sampling_rate_hz
         )
@@ -469,15 +473,15 @@
             "paths": paths_,
             "costs": costs_,
             "matches_start_end": matches_start_end_,
         }
 
     def _select_cost_matrix_method(
         self, max_template_stretch: float, max_signal_stretch: float
-    ) -> Tuple[Callable, Dict[str, Any]]:
+    ) -> tuple[Callable, dict[str, Any]]:
         """Select the correct function to calculate the cost matrix.
 
         This is separate method to make it easy to overwrite by a subclass.
         """
         # In case we don't have local constrains, we can use the simple dtw implementation
         if max_template_stretch == np.inf and max_signal_stretch == np.inf:
             return subsequence_cost_matrix, {}
@@ -501,21 +505,21 @@
             max_cost=max_cost,
             min_distance=min_sequence_length,
         )
 
     def _postprocess_matches(
         self,
         data,  # noqa: ARG002
-        paths: List,  # noqa: ARG002
+        paths: list,  # noqa: ARG002
         cost: np.ndarray,  # noqa: ARG002
         matches_start_end: np.ndarray,
         acc_cost_mat: np.ndarray,  # noqa: ARG002
         to_keep: np.ndarray,
         memory: Memory,  # noqa: ARG002
-    ) -> Tuple[np.ndarray, np.ndarray]:
+    ) -> tuple[np.ndarray, np.ndarray]:
         """Apply postprocessing.
 
         This can be overwritten by subclasses to filter and modify the matches further.
         Note, that no values from matches_start_stop or paths should be deleted (only modified).
         If a stride needs to be deleted, its index from the **original** matches_start_end list should be added to
         the `to_remove` boolmap should be updated.
 
@@ -566,15 +570,15 @@
             matches_start_end_valid = matches_start_end[indices]
             invalid_strides = (
                 np.abs(matches_start_end_valid[:, 1] - matches_start_end_valid[:, 0]) >= max_sequence_length
             )
             to_keep[indices[invalid_strides]] = False
         return matches_start_end, to_keep
 
-    def _post_postprocess_check(self, matches_start_end):
+    def _post_postprocess_check(self, matches_start_end) -> None:
         """Check that is invoked after all processing is done.
 
         Parameters
         ----------
         matches_start_end
             The start and end of all matches remaining after the postprocessing
 
@@ -598,29 +602,28 @@
         return template
 
     @staticmethod
     def _extract_relevant_data_and_template(
         template: BaseDtwTemplate,
         data: Union[np.ndarray, pd.DataFrame],
         sampling_rate_hz: float,
-    ) -> Tuple[np.ndarray, np.ndarray]:
+    ) -> tuple[np.ndarray, np.ndarray]:
         """Get the relevant parts of the data based on the provided template and return template and data as array."""
         template_array = template.get_data()
         data_is_numpy = isinstance(data, np.ndarray)
         template_is_numpy = isinstance(template_array, np.ndarray)
         if data_is_numpy and template_is_numpy:
             data = np.squeeze(data)
             template_array = np.squeeze(template_array)
             if template_array.ndim == 1 and data.ndim == 1:
                 return template_array, data
             if template_array.shape[1] > data.shape[1]:
                 raise ValueError(
-                    "The provided data has less columns than the used template. ({} < {})".format(
-                        data.shape[1], template_array.shape[1]
-                    )
+                    "The provided data has less columns than the used template. "
+                    f"({data.shape[1]} < {template_array.shape[1]})"
                 )
             return (
                 template_array,
                 data[:, : template_array.shape[1]],
             )
         data_is_df = isinstance(data, pd.DataFrame)
         template_is_df = isinstance(template_array, pd.DataFrame)
@@ -631,49 +634,47 @@
                 # We transform the data here based on the scaling/preprocessing defined in the template
                 data = template.transform_data(data, sampling_rate_hz)
             except KeyError as e:
                 raise KeyError(
                     "Some columns of the template are not available in the data! This might happen because you "
                     "provided the data in the wrong coordinate frame (Sensor vs. Body)."
                     "Review the general documentation for more information."
-                    "\n\nMissing columns: {}".format(list(set(template_array.columns) - set(data.columns)))
+                    f"\n\nMissing columns: {list(set(template_array.columns) - set(data.columns))}"
                 ) from e
             return template_array.to_numpy(), data.to_numpy()
         # TODO: Better error message
         raise ValueError("Invalid combination of data and template")
 
     @staticmethod
-    def _find_multiple_paths(acc_cost_mat: np.ndarray, start_points: np.ndarray) -> List[np.ndarray]:
+    def _find_multiple_paths(acc_cost_mat: np.ndarray, start_points: np.ndarray) -> list[np.ndarray]:
         paths = []
         for start in start_points:
             path = subsequence_path(acc_cost_mat, start)
             path_array = np.array(path)
             paths.append(path_array)
         return paths
 
-    def _validate_basic_inputs(self):
+    def _validate_basic_inputs(self) -> None:
         if self.template is None:
             raise ValueError("A `template` must be specified.")
 
         if self.find_matches_method not in self._allowed_methods_map:
             raise ValueError(
-                "Invalid value for `find_matches_method`. Must be one of {}".format(
-                    list(self._allowed_methods_map.keys())
-                )
+                f"Invalid value for `find_matches_method`. Must be one of {list(self._allowed_methods_map.keys())}"
             )
 
         if self.max_template_stretch_ms is not None and self.max_template_stretch_ms <= 0:
             raise ValueError(
                 "Invalid value for `max_template_stretch_ms`."
-                "The value must be a number larger than 0 and not {}".format(self.max_template_stretch_ms)
+                f"The value must be a number larger than 0 and not {self.max_template_stretch_ms}"
             )
         if self.max_signal_stretch_ms is not None and self.max_signal_stretch_ms <= 0:
             raise ValueError(
                 "Invalid value for `max_signal_stretch_ms`."
-                "The value must be a number larger than 0 and not {}".format(self.max_signal_stretch_ms)
+                f"The value must be a number larger than 0 and not {self.max_signal_stretch_ms}"
             )
 
     def _calculate_constrains(self, template: BaseDtwTemplate):
         _max_template_stretch = self.max_template_stretch_ms
         _max_signal_stretch = self.max_signal_stretch_ms
         template_sampling_rate = getattr(template, "sampling_rate_hz", None)
         if _max_signal_stretch and template_sampling_rate is None:
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A version of BarthDTW that used local warping constrains by default."""
-from typing import Dict, Optional, Union
+
+from typing import Optional, Union
 
 from joblib import Memory
 from tpcp import CloneFactory
 from typing_extensions import Literal
 
 from gaitmap.utils._types import _Hashable
 from gaitmap_mad.stride_segmentation.dtw._barth_dtw import BarthDtw
@@ -130,29 +131,29 @@
     --------
     gaitmap.stride_segmentation.BarthDtw: For all details on the method
 
     """
 
     def __init__(
         self,
-        template: Optional[Union[BaseDtwTemplate, Dict[_Hashable, BaseDtwTemplate]]] = CloneFactory(
+        template: Optional[Union[BaseDtwTemplate, dict[_Hashable, BaseDtwTemplate]]] = CloneFactory(
             BarthOriginalTemplate()
         ),
         resample_template: bool = True,
         find_matches_method: Literal["min_under_thres", "find_peaks"] = "find_peaks",
         max_cost: Optional[float] = 4,
         min_match_length_s: Optional[float] = 0.6,
         max_match_length_s: Optional[float] = 3.0,
         max_template_stretch_ms: Optional[float] = 120,
         max_signal_stretch_ms: Optional[float] = 120,
         snap_to_min_win_ms: Optional[float] = 300,
         snap_to_min_axis: Optional[str] = "gyr_ml",
         conflict_resolution: bool = True,
         memory: Optional[Memory] = None,
-    ):
+    ) -> None:
         super().__init__(
             template=template,
             max_cost=max_cost,
             min_match_length_s=min_match_length_s,
             max_match_length_s=max_match_length_s,
             max_template_stretch_ms=max_template_stretch_ms,
             max_signal_stretch_ms=max_signal_stretch_ms,
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Dtw template base classes and helper."""
+
+from collections.abc import Iterable, Sequence
 from importlib.resources import open_text
-from typing import Iterable, List, Optional, Sequence, Tuple, Union, cast
+from typing import Optional, Union, cast
 
 import numpy as np
 import pandas as pd
 from tpcp import HyperParameter, OptimizableParameter, cf
 from typing_extensions import Self
 
 from gaitmap.base import BaseAlgorithm
@@ -20,15 +22,15 @@
     use_cols: Optional[Sequence[Union[str, int]]]
 
     def __init__(
         self,
         *,
         scaling: Optional[BaseTransformer] = None,
         use_cols: Optional[Sequence[Union[str, int]]] = None,
-    ):
+    ) -> None:
         self.scaling = scaling
         self.use_cols = use_cols
 
     def get_data(self) -> Union[np.ndarray, pd.DataFrame]:
         """Return the template data."""
         raise NotImplementedError
 
@@ -100,15 +102,17 @@
     gaitmap.stride_segmentation.BarthDtw: How to apply templates for stride segmentation
 
     """
 
     template_file_name = "barth_original_template.csv"
     sampling_rate_hz = 204.8
 
-    def __init__(self, *, scaling=cf(FixedScaler(scale=500.0)), use_cols: Optional[Sequence[Union[str, int]]] = None):
+    def __init__(
+        self, *, scaling=cf(FixedScaler(scale=500.0)), use_cols: Optional[Sequence[Union[str, int]]] = None
+    ) -> None:
         super().__init__(scaling=scaling, use_cols=use_cols)
 
     def get_data(self) -> Union[np.ndarray, pd.DataFrame]:
         """Return the template data.
 
         This will only return the columns of data that are listed in `use_cols` and will apply the scaling.
         """
@@ -127,15 +131,15 @@
     """Mixin for templates that can be optimized/trained/generated from data."""
 
     def self_optimize(
         self,
         data_sequences: Iterable[SingleSensorData],
         sampling_rate_hz: Optional[float] = None,
         *,
-        columns: Optional[List[_Hashable]] = None,
+        columns: Optional[list[_Hashable]] = None,
         **_,
     ) -> Self:
         """Optimize or recreate the template from data sequences."""
         raise NotImplementedError
 
 
 class DtwTemplate(BaseDtwTemplate):
@@ -182,16 +186,15 @@
     def __init__(
         self,
         *,
         data: Optional[Union[np.ndarray, pd.DataFrame]] = None,
         sampling_rate_hz: Optional[float] = None,
         scaling: Optional[BaseTransformer] = None,
         use_cols: Optional[Sequence[Union[str, int]]] = None,
-    ):
-
+    ) -> None:
         self.data = data
         self.sampling_rate_hz = sampling_rate_hz
         super().__init__(scaling=scaling, use_cols=use_cols)
 
     def get_data(self) -> Union[np.ndarray, pd.DataFrame]:
         """Return the template data.
 
@@ -275,30 +278,30 @@
         *,
         data: Optional[Union[np.ndarray, pd.DataFrame]] = None,
         sampling_rate_hz: Optional[float] = None,
         scaling: Optional[BaseTransformer] = None,
         interpolation_method: str = "linear",
         n_samples: Optional[int] = None,
         use_cols: Optional[Sequence[Union[str, int]]] = None,
-    ):
+    ) -> None:
         self.interpolation_method = interpolation_method
         self.n_samples = n_samples
         super().__init__(
             data=data,
             sampling_rate_hz=sampling_rate_hz,
             scaling=scaling,
             use_cols=use_cols,
         )
 
     def self_optimize(
         self,
         data_sequences: Iterable[SingleSensorData],
         sampling_rate_hz: Optional[float] = None,
         *,
-        columns: Optional[List[_Hashable]] = None,
+        columns: Optional[list[_Hashable]] = None,
         **_,
     ):
         """Create a template from multiple data sequences.
 
         All data sequences will be interpolated to match `self.n_samples` and then averaged.
         If `self.scaling` is `optimizable`, the scaler will be optimized as well based on the final template data.
         Note, that the scaler is not trained or applied to the data, before the template is generated,
@@ -341,16 +344,16 @@
 
 
 def _create_interpolated_dtw_template(
     signal_sequences: Iterable[SingleSensorData],
     sampling_rate_hz: float,
     kind: str = "linear",
     n_samples: Optional[int] = None,
-    columns: Optional[List[_Hashable]] = None,
-) -> Tuple[pd.DataFrame, float]:
+    columns: Optional[list[_Hashable]] = None,
+) -> tuple[pd.DataFrame, float]:
     expected_col_order = columns
     arrays = []
     for df in signal_sequences:
         is_single_sensor_data(df, check_acc=False, check_gyr=False, frame="any", raise_exception=True)
         if expected_col_order is None:
             expected_col_order = df.columns
         arrays.append(df[expected_col_order].to_numpy())
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,16 +96,15 @@
         Matching path represented as a list of index pairs. In each pair, the
         first index corresponds to `subseq` and the second one corresponds to
         `longseq`. The startpoint of the Path is :math:`P_0 = (0, ?)` and it
         ends at :math:`P_L = (len(subseq)-1, idx\_path\_end)`
 
     Examples
     --------
-    >>> acc_cost_mat = numpy.array([[1., 0., 0., 1., 4.],
-    ...                             [5., 1., 1., 0., 1.]])
+    >>> acc_cost_mat = numpy.array([[1.0, 0.0, 0.0, 1.0, 4.0], [5.0, 1.0, 1.0, 0.0, 1.0]])
     >>> # calculate the globally optimal path
     >>> optimal_end_point = numpy.argmin(acc_cost_mat[-1, :])
     >>> path = subsequence_path(acc_cost_mat, optimal_end_point)
     >>> path
     [(0, 2), (1, 3)]
 
     """
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/__init__.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Roth et al. HMM based stride segmentation model."""
+
 import multiprocessing
 import warnings
 
 from gaitmap_mad.stride_segmentation.hmm._hmm_feature_transform import (
     BaseHmmFeatureTransformer,
     RothHmmFeatureTransformer,
 )
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Feature transformation class for HMM."""
-from typing import List, Optional
+
+from typing import NoReturn, Optional
 
 import numpy as np
 import pandas as pd
+from scipy.interpolate import interp1d
 from sklearn import preprocessing
 from tpcp import cf
 
 from gaitmap.data_transform import (
     BaseFilter,
     BaseTransformer,
     ButterworthFilter,
@@ -49,34 +51,34 @@
     def transform(
         self,
         data: Optional[SingleSensorData] = None,
         *,
         roi_list: Optional[SingleSensorRegionsOfInterestList] = None,
         sampling_rate_hz: Optional[float] = None,
         **kwargs,
-    ):
+    ) -> NoReturn:
         """Transform the data and the roi/stride list into to the feature space.
 
         Transforming the roi/stride list is only required, if the sampling rate of the features space is different from
         the data space.
         If now down-sampling is required, set `self.transformed_roi_list_` to `roi_list`.
 
         """
         raise NotImplementedError()
 
-    def inverse_transform_state_sequence(self, state_sequence: np.ndarray, *, sampling_rate_hz: float) -> np.ndarray:
+    def inverse_transform_state_sequence(self, state_sequence: np.ndarray, *, data: np.array) -> np.ndarray:
         """Inverse transform a state sequence to the original sampling rate.
 
         Parameters
         ----------
         state_sequence
             The state sequence to be transformed back to the original sampling rate.
             This is done by repeating each state for the number of samples it was downsampled to.
-        sampling_rate_hz
-            The sampling rate of the original data in Hz
+        data
+            The original data used for the transformation
 
         Returns
         -------
         The state sequence in the original sampling rate
 
         """
         raise NotImplementedError()
@@ -153,28 +155,28 @@
            https://doi.org/10.1186/s12984-021-00883-7
 
     """
 
     # TODO: Find a way to expose the internal objects instead of exposing just parameters.
     sampling_rate_feature_space_hz: float
     low_pass_filter: Optional[BaseFilter]
-    axes: List[str]
-    features: List[str]
+    axes: list[str]
+    features: list[str]
     window_size_s: float
     standardization: bool
 
     def __init__(
         self,
         sampling_rate_feature_space_hz: float = 51.2,
         low_pass_filter: Optional[BaseFilter] = cf(ButterworthFilter(cutoff_freq_hz=10.0, order=4)),
-        axes: List[str] = cf(["gyr_ml"]),
-        features: List[str] = cf(["raw", "gradient"]),
+        axes: list[str] = cf(["gyr_ml"]),
+        features: list[str] = cf(["raw", "gradient"]),
         window_size_s: float = 0.2,
         standardization: bool = True,
-    ):
+    ) -> None:
         self.sampling_rate_feature_space_hz = sampling_rate_feature_space_hz
         self.low_pass_filter = low_pass_filter
         self.axes = axes
         self.features = features
         self.window_size_s = window_size_s
         self.standardization = standardization
 
@@ -205,14 +207,20 @@
         sampling_rate_hz
             The sampling rate of the data in Hz
 
         """
         self.sampling_rate_hz = sampling_rate_hz
         if sampling_rate_hz is None:
             raise ValueError(f"{type(self).__name__}.transform requires a `sampling_rate_hz` to be passed.")
+        if sampling_rate_hz < self.sampling_rate_feature_space_hz:
+            raise ValueError(
+                f"Invalid value for `sampling_rate_hz`={sampling_rate_hz}. \n"
+                f"Sampling rate of data can not be lower than the  feature space sampling rate of the "
+                f"used model {type(self).__name__}: {self.sampling_rate_feature_space_hz}Hz."
+            )
         if data is not None:
             self.data = data
 
             if self.low_pass_filter is not None and not isinstance(self.low_pass_filter, BaseFilter):
                 raise TypeError(f"{type(self).__name__}.low_pass_filter must be a subclass of BaseFilter.")
 
             preprocessor = ChainedTransformer(
@@ -254,24 +262,27 @@
                 Resample(self.sampling_rate_feature_space_hz)
                 .transform(roi_list=roi_list, sampling_rate_hz=sampling_rate_hz)
                 .transformed_roi_list_
             )
 
         return self
 
-    def inverse_transform_state_sequence(self, state_sequence: np.ndarray, *, sampling_rate_hz: float) -> np.ndarray:
+    def inverse_transform_state_sequence(self, state_sequence: np.ndarray, *, data: np.array) -> np.ndarray:
         """Inverse transform a state sequence to the original sampling rate.
 
         Parameters
         ----------
         state_sequence
             The state sequence to be transformed back to the original sampling rate.
             This is done by repeating each state for the number of samples it was downsampled to.
-        sampling_rate_hz
-            The sampling rate of the original data in Hz
+        data
+            The original data used for the transformation
 
         Returns
         -------
         The state sequence in the original sampling rate
 
         """
-        return np.repeat(state_sequence, sampling_rate_hz / self.sampling_rate_feature_space_hz)
+        downsampled_x = np.arange(0, len(data) - 1, len(data) / len(state_sequence))
+        new_x = np.arange(0, len(data))
+        interpolated = interp1d(downsampled_x, state_sequence, kind="nearest", fill_value="extrapolate")(new_x)
+        return interpolated.astype(int)
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """HMM based stride segmentation by Roth et al. 2021."""
+
 from contextlib import suppress
 from importlib.resources import open_text
 from pathlib import Path
-from typing import Dict, Generic, Optional, TypeVar, Union
+from typing import Generic, Optional, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 from tpcp import cf, make_action_safe
 from typing_extensions import Self
 
 from gaitmap.base import BaseStrideSegmentation
@@ -37,17 +38,20 @@
            free-living gait data in Parkinson`s disease patients. J NeuroEngineering Rehabil 18, 93 (2021).
            https://doi.org/10.1186/s12984-021-00883-7
 
     """
 
     def __new__(cls):
         # try to load models
-        with open_text(
-            "gaitmap_mad.stride_segmentation.hmm._pre_trained_models", "fallriskpd_at_lab_model.json"
-        ) as test_data, Path(test_data.name).open(encoding="utf8") as f:
+        with (
+            open_text(
+                "gaitmap_mad.stride_segmentation.hmm._pre_trained_models", "fallriskpd_at_lab_model.json"
+            ) as test_data,
+            Path(test_data.name).open(encoding="utf8") as f,
+        ):
             model_json = f.read()
         return RothSegmentationHmm.from_json(model_json)
 
 
 BaseSegmentationHmmT = TypeVar("BaseSegmentationHmmT", bound=BaseSegmentationHmm)
 
 
@@ -121,39 +125,39 @@
     snap_to_min_win_ms: Optional[float]
     snap_to_min_axis: str
     model: BaseSegmentationHmmT
 
     data: Union[np.ndarray, SensorData]
     sampling_rate_hz: float
 
-    matches_start_end_: Union[np.ndarray, Dict[str, np.ndarray]]
-    hidden_state_sequence_: Union[np.ndarray, Dict[str, np.ndarray]]
-    result_model_: Union[BaseSegmentationHmmT, Dict[str, BaseSegmentationHmmT]]
+    matches_start_end_: Union[np.ndarray, dict[str, np.ndarray]]
+    hidden_state_sequence_: Union[np.ndarray, dict[str, np.ndarray]]
+    result_model_: Union[BaseSegmentationHmmT, dict[str, BaseSegmentationHmmT]]
 
     def __init__(
         self,
         model: BaseSegmentationHmmT = cf(PreTrainedRothSegmentationModel()),
         *,
         snap_to_min_win_ms: Optional[float] = 100,
         snap_to_min_axis: str = "gyr_ml",
-    ):
+    ) -> None:
         self.snap_to_min_win_ms = snap_to_min_win_ms
         self.snap_to_min_axis = snap_to_min_axis
         self.model = model
 
     @property
-    def stride_list_(self) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
+    def stride_list_(self) -> Union[pd.DataFrame, dict[str, pd.DataFrame]]:
         """Return start and end of each match as pd.DataFrame."""
         start_ends = self.matches_start_end_
         if isinstance(start_ends, dict):
             return {k: self._format_stride_list(v) for k, v in start_ends.items()}
         return self._format_stride_list(start_ends)
 
     @property
-    def matches_start_end_original_(self) -> Union[np.ndarray, Dict[_Hashable, np.ndarray]]:
+    def matches_start_end_original_(self) -> Union[np.ndarray, dict[_Hashable, np.ndarray]]:
         """Return the starts and end directly from the hidden state sequence.
 
         This will not be effected by potential changes of the postprocessing.
         """
         stride_start_state = self.model.stride_states[0]
         stride_end_state = self.model.stride_states[-1]
         if isinstance(self.hidden_state_sequence_, dict):
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Segmentation _model base classes and helper."""
+
 import copy
-from typing import Any, Dict, List, Literal, Optional, Sequence, Tuple
+from collections.abc import Sequence
+from typing import Any, Literal, Optional
 
 import numpy as np
 import pandas as pd
 import pomegranate as pg
 from pomegranate import HiddenMarkovModel as pgHMM
 from pomegranate.hmm import History
 from tpcp import OptiPara, cf, make_optimize_safe
@@ -97,15 +99,15 @@
 
     hidden_state_sequence_: np.ndarray
 
     data: pd.DataFrame
     sampling_rate_hz: float
 
     @property
-    def stride_states(self) -> List[int]:
+    def stride_states(self) -> list[int]:
         """Get the indexes of the states in the hidden state sequence corresponding to strides."""
         raise NotImplementedError
 
     def predict(self, data: SingleSensorData, sampling_rate_hz: float) -> Self:
         """Perform prediction based on given data and given model.
 
         Parameters
@@ -150,15 +152,15 @@
         raise NotImplementedError
 
     def self_optimize_with_info(
         self,
         data_sequence: Sequence[SingleSensorData],
         stride_list_sequence: Sequence[SingleSensorStrideList],
         sampling_rate_hz: float,
-    ) -> Tuple[Self, Any]:
+    ) -> tuple[Self, Any]:
         """Create and train the HMM model based on the given data and labels.
 
         This is identical to `self_optimize`, but can return additional information about the training process.
 
         Parameters
         ----------
         data_sequence
@@ -292,15 +294,15 @@
     stop_threshold: float
     max_iterations: int
     initialization: Literal["labels", "fully-connected"]
     verbose: bool
     n_jobs: int
     name: Optional[str]
     model: OptiPara[Optional[pgHMM]]
-    data_columns: OptiPara[Optional[Tuple[str, ...]]]
+    data_columns: OptiPara[Optional[tuple[str, ...]]]
 
     feature_space_data_: pd.DataFrame
     hidden_state_sequence_feature_space_: np.ndarray
 
     def __init__(
         self,
         stride_model: SimpleHmm = cf(
@@ -332,16 +334,16 @@
         stop_threshold: float = 1e-9,
         max_iterations: int = 1,
         initialization: Literal["labels", "fully-connected"] = "labels",
         verbose: bool = True,
         n_jobs: int = 1,
         name: str = "segmentation_model",
         model: Optional[pgHMM] = None,
-        data_columns: Optional[Tuple[str, ...]] = None,
-    ):
+        data_columns: Optional[tuple[str, ...]] = None,
+    ) -> None:
         self.stride_model = stride_model
         self.transition_model = transition_model
         self.feature_transform = feature_transform
         self.algo_predict = algo_predict
         self.algo_train = algo_train
         self.stop_threshold = stop_threshold
         self.max_iterations = max_iterations
@@ -354,20 +356,20 @@
 
     @property
     def n_states(self) -> int:
         """Return the number of states of the final model."""
         return self.transition_model.n_states + self.stride_model.n_states
 
     @property
-    def stride_states(self) -> List[int]:
+    def stride_states(self) -> list[int]:
         """Return the ids of the stride states."""
         return (np.arange(self.stride_model.n_states) + self.transition_model.n_states).tolist()
 
     @property
-    def transition_states(self) -> List[int]:
+    def transition_states(self) -> list[int]:
         """Return the ids of the transition states."""
         return np.arange(self.transition_model.n_states).tolist()
 
     def predict(self, data: SingleSensorData, sampling_rate_hz: float) -> Self:
         """Perform prediction based on given data and given model.
 
         This generates the hidden state sequence and stores it in the `hidden_state_sequence_` attribute.
@@ -405,15 +407,15 @@
         self.feature_space_data_ = feature_data
 
         # pomegranate always adds a label for the start- and end-state, which can be ignored here!
         self.hidden_state_sequence_feature_space_ = predict(
             self.model, feature_data, expected_columns=self.data_columns, algorithm=self.algo_predict
         )
         self.hidden_state_sequence_ = self.feature_transform.inverse_transform_state_sequence(
-            self.hidden_state_sequence_feature_space_, sampling_rate_hz=sampling_rate_hz
+            self.hidden_state_sequence_feature_space_, data=data
         )
         return self
 
     def _transform(
         self,
         data_sequence: Sequence[pd.DataFrame],
         stride_list_sequence: Optional[Sequence[pd.DataFrame]],
@@ -472,15 +474,15 @@
 
     @make_optimize_safe
     def self_optimize_with_info(
         self,
         data_sequence: Sequence[SingleSensorData],
         stride_list_sequence: Sequence[SingleSensorStrideList],
         sampling_rate_hz: float,
-    ) -> Tuple[Self, Dict[Literal["self", "transition_model", "stride_model"], History]]:
+    ) -> tuple[Self, dict[Literal["self", "transition_model", "stride_model"], History]]:
         """Create and train the HMM model based on the given data and labels.
 
         This is identical to `self_optimize`, but returns additional information about the training process.
         The dictionary returned as second parameter contains the training history for each of the three models (
         stride-model, transition-model, and the combined final model "self").
 
         Parameters
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Simple model base classes and helper."""
 
 import copy
 import warnings
-from typing import Literal, Optional, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 import pomegranate as pg
 from pomegranate import HiddenMarkovModel as pgHMM
 from pomegranate.hmm import History
 from tpcp import OptiPara, make_optimize_safe
@@ -252,31 +253,31 @@
     algo_train: Literal["viterbi", "baum-welch"]
     stop_threshold: float
     max_iterations: int
     verbose: bool
     n_jobs: int
     name: Optional[str]
     model: OptiPara[Optional[pgHMM]]
-    data_columns: OptiPara[Optional[Tuple[str, ...]]]
+    data_columns: OptiPara[Optional[tuple[str, ...]]]
 
     def __init__(
         self,
         n_states: int,
         n_gmm_components: int,
         *,
         architecture: Literal["left-right-strict", "left-right-loose", "fully-connected"] = "left-right-strict",
         algo_train: Literal["viterbi", "baum-welch", "labeled"] = "viterbi",
         stop_threshold: float = 1e-9,
         max_iterations: int = 1e8,
         verbose: bool = True,
         n_jobs: int = 1,
         name: str = "my_model",
         model: Optional[pgHMM] = None,
-        data_columns: Optional[Tuple[str, ...]] = None,
-    ):
+        data_columns: Optional[tuple[str, ...]] = None,
+    ) -> None:
         self.n_states = n_states
         self.n_gmm_components = n_gmm_components
         self.algo_train = algo_train
         self.stop_threshold = stop_threshold
         self.max_iterations = max_iterations
         self.architecture = architecture
         self.verbose = verbose
@@ -342,15 +343,15 @@
         """
         return self.self_optimize_with_info(data_sequence, labels_sequence)[0]
 
     def self_optimize_with_info(
         self,
         data_sequence: Sequence[SingleSensorData],
         labels_sequence: Sequence[Union[np.ndarray, pd.Series, pd.DataFrame]],
-    ) -> Tuple[Self, History]:
+    ) -> tuple[Self, History]:
         """Create and train the HMM model based on the given data and labels.
 
         This is identical to `self_optimize`, but returns additional information about the training process.
 
         Parameters
         ----------
         data_sequence
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/stride_segmentation/hmm/_utils.py` & `gaitmap_mad-2.4.0/gaitmap_mad/stride_segmentation/hmm/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Utils and helper functions for HMM classes."""
+
 import json
 import warnings
-from typing import Any, List, Literal, Optional, Set, Tuple
+from typing import Any, Literal, Optional
 
 import numpy as np
 import pandas as pd
 import pomegranate as pg
 from pomegranate.hmm import History
 from tpcp import BaseTpcpObject, CloneFactory
 from tpcp._hash import custom_hash
 
 from gaitmap.utils.datatype_helper import SingleSensorData, SingleSensorRegionsOfInterestList, SingleSensorStrideList
 
 
-def _add_transition(model, a, b, probability, pseudocount, group):
+def _add_transition(model, a, b, probability, pseudocount, group) -> None:
     """Hacky way to add a transition when cloning a model in the "wrong" way."""
     pseudocount = pseudocount or probability
     model.graph.add_edge(a, b, probability=probability, pseudocount=pseudocount, group=group)
 
 
 def _clone_model(orig_model: pg.HiddenMarkovModel, assert_correct: bool = True) -> pg.HiddenMarkovModel:
     """Clone a HMM without changing its values using a hacky way.
@@ -87,15 +88,15 @@
     # Indicate appropriate start and end states
     model.start = states[d["start_index"]]
     model.end = states[d["end_index"]]
 
     new_state_order = [state.name for state in states]
 
     # Add all the edges to the model
-    for (start, end, data) in list(orig_model.graph.edges(data=True)):
+    for start, end, data in list(orig_model.graph.edges(data=True)):
         _add_transition(
             model,
             states[new_state_order.index(start.name)],
             states[new_state_order.index(end.name)],
             data["probability"],
             data["pseudocount"],
             data["group"],
@@ -148,26 +149,26 @@
             if isinstance(value, pg.HiddenMarkovModel):
                 return f"{name}=HiddenMarkovModel[name={value.name}](...)"
             if isinstance(value, CloneFactory) and isinstance(value.default_value, pg.HiddenMarkovModel):
                 return f"{name}=cf(HiddenMarkovModel[name={value.get_value().name}](...))"
         return super().__repr_parameter__(name, value)
 
 
-def create_transition_matrix_fully_connected(n_states: int) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+def create_transition_matrix_fully_connected(n_states: int) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Create nxn transition matrix with only 1 entries."""
     transition_matrix = np.ones((n_states, n_states)) / n_states
     start_probs = np.ones(n_states)
     end_probs = np.ones(n_states)
 
     return transition_matrix, start_probs, end_probs
 
 
 def create_transition_matrix_left_right(
     n_states: int, self_transition: bool = True
-) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Create nxn transition for left to right model."""
     transition_matrix = np.zeros((n_states, n_states))
     transition_matrix[range(n_states - 1), range(1, n_states)] = 1
     transition_matrix[range(n_states), range(n_states)] = 1
     if self_transition:
         transition_matrix[-1][0] = 1
 
@@ -177,25 +178,25 @@
     # and force end with last state
     end_probs = np.zeros(n_states)
     end_probs[-1] = 1
 
     return transition_matrix, start_probs, end_probs
 
 
-def print_transition_matrix(model: pg.HiddenMarkovModel, precision: int = 3):
+def print_transition_matrix(model: pg.HiddenMarkovModel, precision: int = 3) -> None:
     """Print model transition matrix in user-friendly format."""
     np.set_printoptions(suppress=True)
     np.set_printoptions(precision)
     if isinstance(model, pg.HiddenMarkovModel):
         print(model.dense_transition_matrix()[0:-2, 0:-2])
     if isinstance(model, np.ndarray):
         print(model)
 
 
-def cluster_data_by_labels(data_list: List[np.ndarray], label_list: List[np.ndarray]):
+def cluster_data_by_labels(data_list: list[np.ndarray], label_list: list[np.ndarray]):
     """Cluster data by labels."""
     assert isinstance(label_list, list), "label_list must be list!"
     assert isinstance(data_list, list), "data_list must be list!"
 
     label_list = [np.asarray(label).tolist() for label in label_list]
     data_list = [np.asarray(data).tolist() for data in data_list]
 
@@ -322,15 +323,15 @@
                     if not np.all(np.isfinite(param)):
                         return False
             if hasattr(dist, "weights") and not np.all(np.isfinite(dist.weights)):
                 return False
     return True
 
 
-def check_history_for_training_failure(history: History):
+def check_history_for_training_failure(history: History) -> None:
     """Check if training history contains any NaNs."""
     if not np.all(np.isfinite(history.improvements)) or np.any(np.array(history.improvements) < 0):
         warnings.warn(
             "During training the improvement per epoch became NaN/infinite or negative! "
             "Run `self_optimize_with_info` and inspect the history element for more information. "
             "With a high likelihood, the final model is not usable and will result in errors during prediction. "
             "This usually happens when there is not enough data for a large number of distributions and "
@@ -344,37 +345,37 @@
     """Get state object from model by name."""
     for state in model.states:
         if state.name == state_name:
             return state
     raise ValueError(f"State {state_name} not found within given _model!")
 
 
-def add_transition(model: pg.HiddenMarkovModel, transition: Tuple[str, str], transition_probability: float):
+def add_transition(model: pg.HiddenMarkovModel, transition: tuple[str, str], transition_probability: float) -> None:
     """Add a transition to an existing model by state-names.
 
     add_transition(model, transition = ("s0","s1"), transition_probability = 0.5)
     to add an edge from state s0 to state s1 with a transition probability of 0.5.
     """
     model.add_transition(
         get_state_by_name(model, transition[0]),
         get_state_by_name(model, transition[1]),
         transition_probability,
     )
 
 
-def get_model_distributions(model: pg.HiddenMarkovModel) -> List[pg.Distribution]:
+def get_model_distributions(model: pg.HiddenMarkovModel) -> list[pg.Distribution]:
     """Return all not None distributions as list from given model."""
     distributions = []
     for state in model.states:
         if state.distribution is not None:
             distributions.append(state.distribution)
     return distributions
 
 
-def labels_to_strings(labelsequence: List[Optional[np.ndarray]]) -> List[Optional[List[str]]]:
+def labels_to_strings(labelsequence: list[Optional[np.ndarray]]) -> list[Optional[list[str]]]:
     """Convert label sequence of ints to strings.
 
     Pomegranated messes up sorting of states: it will sort like this: s0, s1, s10, s2.... which can lead to unexpected
     behaviour.
     """
     assert isinstance(labelsequence, list), "labelsequence must be list!"
 
@@ -384,16 +385,16 @@
             labelsequence_str.append(sequence)
             continue
         labelsequence_str.append([f"s{i:02}" for i in sequence])
     return labelsequence_str
 
 
 def extract_transitions_starts_stops_from_hidden_state_sequence(
-    hidden_state_sequence: List[np.ndarray],
-) -> Tuple[Set[Tuple[str, str]], np.ndarray, np.ndarray]:
+    hidden_state_sequence: list[np.ndarray],
+) -> tuple[set[tuple[str, str]], np.ndarray, np.ndarray]:
     """Extract transitions from hidden state sequence.
 
     This function will return a list of transitions as well as start and stop labels that can be found within the
     input sequences.
 
     input = [[1,1,1,1,1,3,3,3,3,2,2,2,2,4,4,4,4,5,5],
              [0,0,1,1,1,3,3,3,3,2,2,2,6]]
@@ -443,19 +444,19 @@
     n_labels : int
         Number of labels to create.
     n_states : int
         Number of unique states in the output sequence.
 
     Example
     -------
-    >>> create_equidistant_label_sequence(n_labels = 10, n_states = 5)
+    >>> create_equidistant_label_sequence(n_labels=10, n_states=5)
     array([0, 0, 1, 1, 2, 2, 3, 3, 4, 4])
-    >>> create_equidistant_label_sequence(n_labels = 10, n_states = 4)
+    >>> create_equidistant_label_sequence(n_labels=10, n_states=4)
     array([0, 0, 0, 1, 1, 2, 2, 3, 3, 3])
-    >>> create_equidistant_label_sequence(n_labels = 10, n_states = 3)
+    >>> create_equidistant_label_sequence(n_labels=10, n_states=3)
     array([0, 0, 0, 1, 1, 1, 2, 2, 2, 2])
 
     """
     if n_labels < n_states:
         raise ValueError("n_labels must be larger than n_states!")
 
     # calculate the samples per state (must be integer!)
@@ -495,29 +496,28 @@
 
     return pd.DataFrame(
         [(s, e) for s, e in zip(transition_starts, transition_ends) if e - s > 0], columns=["start", "end"]
     )
 
 
 def get_train_data_sequences_transitions(
-    data_train_sequence: List[SingleSensorData], stride_list_sequence: List[SingleSensorStrideList], n_states: int
-) -> Tuple[List[np.ndarray], List[np.ndarray]]:
+    data_train_sequence: list[SingleSensorData], stride_list_sequence: list[SingleSensorStrideList], n_states: int
+) -> tuple[list[np.ndarray], list[np.ndarray]]:
     """Extract Transition Training set.
 
     - data_train_sequence: list of datasets in feature space
     - stride_list_sequence: list of gaitmap stride-lists
     - n_states: number of labels.
     """
     trans_data_train_sequence = []
     trans_labels_train_sequence = []
 
     n_too_short_transitions = 0
 
     for data, stride_list in zip(data_train_sequence, stride_list_sequence):
-
         # for each transition, get data and create some naive labels for initialization
         for start, end in convert_stride_list_to_transition_list(stride_list, data.shape[0])[
             ["start", "end"]
         ].to_numpy():
             # append extracted sequences and corresponding label set to results list
             try:
                 labels = create_equidistant_label_sequence(end - start, n_states).astype("int64")
@@ -536,16 +536,16 @@
             "enough to train a model."
         )
 
     return trans_data_train_sequence, trans_labels_train_sequence
 
 
 def get_train_data_sequences_strides(
-    data_train_sequence: List[SingleSensorData], stride_list_sequence: List[SingleSensorStrideList], n_states: int
-) -> Tuple[List[np.ndarray], List[np.ndarray]]:
+    data_train_sequence: list[SingleSensorData], stride_list_sequence: list[SingleSensorStrideList], n_states: int
+) -> tuple[list[np.ndarray], list[np.ndarray]]:
     """Extract Transition Training set.
 
     - data_train_sequence: list of datasets in feature space
     - stride_list_sequence: list of gaitmap stride-lists
     - n_states: number of labels.
     """
     stride_data_train_sequence = []
@@ -579,15 +579,15 @@
     pass
 
 
 def predict(
     model: Optional[pg.HiddenMarkovModel],
     data: pd.DataFrame,
     *,
-    expected_columns: Tuple[str, ...],
+    expected_columns: tuple[str, ...],
     algorithm: Literal["viterbi", "map"],
 ) -> np.ndarray:
     """Predict the hidden state sequence for the given data.
 
     Parameters
     ----------
     model
@@ -628,15 +628,15 @@
             f"of the model ({len(model.states) - 2}). "
             f"But it only has {len(data)} samples."
         )
 
     data = np.ascontiguousarray(data.to_numpy())
     try:
         labels_predicted = np.asarray(model.predict(data.copy(), algorithm=algorithm))
-    except Exception as e:  # noqa: broad-except
+    except Exception as e:  # noqa: BLE001
         if not model_params_are_finite(model):
             raise ValueError(
                 "Prediction failed! (See error above.). "
                 "However, the provided pomegranate model has non-finite/NaN parameters. "
                 "This might be the source of the observed error and indicates problems during training. "
                 "Check the training history and the model parameters to confirm invalid training behaviour. "
                 "Unfortunately, there is no way to automatically fix these issues. "
```

### Comparing `gaitmap_mad-2.3.0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py` & `gaitmap_mad-2.4.0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,19 +77,17 @@
 
     >>> import pandas as pd
     >>> from gaitmap.utils.consts import SF_COLS
     >>> from gaitmap.zupt_detection import NormZuptDetector
     >>> data = pd.DataFrame(..., columns=SF_COLS)
     >>> sampling_rate_hz = 100
     >>> # Create an algorithm instance
-    >>> pwli = PieceWiseLinearDedriftedIntegration(NormZuptDetector(window_length_s=0.15,
-    ...                                                             inactive_signal_threshold=15.
-    ...                                            ),
-    ...                                            gravity=np.array([0, 0, 9.81])
-    ...        )
+    >>> pwli = PieceWiseLinearDedriftedIntegration(
+    ...     NormZuptDetector(window_length_s=0.15, inactive_signal_threshold=15.0), gravity=np.array([0, 0, 9.81])
+    ... )
     >>> # Apply the algorithm
     >>> pwli = pwli.estimate(data, sampling_rate_hz=sampling_rate_hz)
     >>> # Inspect the results
     >>> pwli.position_
     <pd.Dataframe with resulting positions>
     >>> pwli.velocity_
     <pd.Dataframe with resulting velocities>
@@ -140,15 +138,15 @@
         zupt_detector=cf(
             NormZuptDetector(
                 sensor="gyr", window_length_s=0.15, window_overlap=0.5, metric="mean", inactive_signal_threshold=15.0
             )
         ),
         level_assumption: bool = True,
         gravity: Optional[np.ndarray] = cf(GRAV_VEC),
-    ):
+    ) -> None:
         self.zupt_detector = zupt_detector
         self.level_assumption = level_assumption
         self.gravity = gravity
 
     def estimate(self, data: SingleSensorData, *, sampling_rate_hz: float, **_) -> Self:
         """Estimate the position of the sensor based on the provided global frame data.
```

### Comparing `gaitmap_mad-2.3.0/pyproject.toml` & `gaitmap_mad-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaitmap_mad"
-version = "2.3.0"
+version = "2.4.0"
 description = "Specific algorithm implementaions by the mad_lab"
 license = "AGPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/gaitmap"
 repository = "https://github.com/mad-lab-fau/gaitmap"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
```

### Comparing `gaitmap_mad-2.3.0/PKG-INFO` & `gaitmap_mad-2.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
-Name: gaitmap-mad
-Version: 2.3.0
+Name: gaitmap_mad
+Version: 2.4.0
 Summary: Specific algorithm implementaions by the mad_lab
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: AGPL-3.0
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/mad-lab-fau/gaitmap
 Description-Content-Type: text/markdown
 
 # Gaitmap-MAD
 
 This is a companion package to the `gaitmap` library.
 It contains algorithms developed by the [MaD Lab](https://www.mad.tf.fau.de/) in collaboration with industry partners.
```

