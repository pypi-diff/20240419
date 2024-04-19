# Comparing `tmp/ship_model_lib-1.0.0.tar.gz` & `tmp/ship_model_lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ship_model_lib-1.0.0.tar", last modified: Wed Apr 17 06:38:50 2024, max compression
+gzip compressed data, was "ship_model_lib-1.0.1.tar", last modified: Fri Apr 19 11:40:26 2024, max compression
```

## Comparing `ship_model_lib-1.0.0.tar` & `ship_model_lib-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.358578 ship_model_lib-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-17 06:38:50.358578 ship_model_lib-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.350578 ship_model_lib-1.0.0/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/dependencies/B_series_coefficients.npy
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/dependencies/Re_correction.npy
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:38:50.358578 ship_model_lib-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.354578 ship_model_lib-1.0.0/ship_model_lib/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63365 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)    45217 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/added_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)    30021 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/calm_water_resistance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.354578 ship_model_lib-1.0.0/ship_model_lib/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/data/create_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/data/drag_coefficient.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/machinery.py
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/operation_profile_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    24580 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/propulsor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/ship_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19887 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/ship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/ship_model_lib/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.358578 ship_model_lib-1.0.0/ship_model_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 06:38:50.000000 ship_model_lib-1.0.0/ship_model_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:38:50.358578 ship_model_lib-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    33659 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/tests/test_added_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/tests/test_machinery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/tests/test_propulsor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-04-17 06:38:43.000000 ship_model_lib-1.0.0/tests/test_ship_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:40:26.202502 ship_model_lib-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-19 11:40:26.202502 ship_model_lib-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:40:26.198502 ship_model_lib-1.0.1/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/dependencies/B_series_coefficients.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/dependencies/Re_correction.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:40:26.202502 ship_model_lib-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:40:26.198502 ship_model_lib-1.0.1/ship_model_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63365 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45217 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/added_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30021 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/calm_water_resistance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:40:26.202502 ship_model_lib-1.0.1/ship_model_lib/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/data/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/data/drag_coefficient.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/machinery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/operation_profile_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24580 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/propulsor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/ship_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23867 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/ship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/ship_model_lib/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:40:26.202502 ship_model_lib-1.0.1/ship_model_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-19 11:40:26.000000 ship_model_lib-1.0.1/ship_model_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-19 11:40:26.000000 ship_model_lib-1.0.1/ship_model_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:40:26.000000 ship_model_lib-1.0.1/ship_model_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 11:40:26.000000 ship_model_lib-1.0.1/ship_model_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:40:26.000000 ship_model_lib-1.0.1/ship_model_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-19 11:40:26.000000 ship_model_lib-1.0.1/ship_model_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 11:40:26.000000 ship_model_lib-1.0.1/ship_model_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:40:26.202502 ship_model_lib-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    33659 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/tests/test_added_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/tests/test_machinery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/tests/test_propulsor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-04-19 11:40:22.000000 ship_model_lib-1.0.1/tests/test_ship_model.py
```

### Comparing `ship_model_lib-1.0.0/LICENSE` & `ship_model_lib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/PKG-INFO` & `ship_model_lib-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ship_model_lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Model library for the hydrodynamics, energy system and fuel calculation
 Home-page: https://github.com/developer/https://github.com/SINTEF/shipdesignlab/
 Author: SINTEF Ocean
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: Ship Energy Model
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ship_model_lib-1.0.0/dependencies/B_series_coefficients.npy` & `ship_model_lib-1.0.1/dependencies/B_series_coefficients.npy`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/settings.ini` & `ship_model_lib-1.0.1/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # All sections below are required unless otherwise specified
 # see https://github.com/fastai/nbdev/blob/master/settings.ini for examples
 
 ### Python Library ###
 lib_name = ship_model_lib
 min_python = 3.10
 # x-release-please-start-version
-version = 1.0.0
+version = 1.0.1
 # x-release-please-end
 
 ### OPTIONAL ###
 
 requirements = pandas>=2.0.0 pandas<3 scipy>=1.11.0 scipy<2 operation_profile_lib~=0.1.11 matplotlib~=3.8.2 plotly~=5.13.0
 # dev_requirements =
 # console_scripts =
```

### Comparing `ship_model_lib-1.0.0/setup.py` & `ship_model_lib-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib/_modidx.py` & `ship_model_lib-1.0.1/ship_model_lib/_modidx.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib/added_resistance.py` & `ship_model_lib-1.0.1/ship_model_lib/added_resistance.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib/calm_water_resistance.py` & `ship_model_lib-1.0.1/ship_model_lib/calm_water_resistance.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib/data/create_table.py` & `ship_model_lib-1.0.1/ship_model_lib/data/create_table.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib/data/drag_coefficient.csv` & `ship_model_lib-1.0.1/ship_model_lib/data/drag_coefficient.csv`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib/machinery.py` & `ship_model_lib-1.0.1/ship_model_lib/machinery.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib/operation_profile_structure.py` & `ship_model_lib-1.0.1/ship_model_lib/operation_profile_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,19 +213,19 @@
     heading_deg: Numeric = None
     auxiliary_power: Numeric = None
     weather: Weather = None
     location: Location = None
 
     def __init__(
         self,
+        speed_kn: Numeric,
         timestamp_seconds: Numeric = None,
-        speed_kn: Numeric = None,
-        power_limit_kw: Numeric = None,
+        power_limit_kw: Numeric = 1e6,
         heading_deg: Numeric = None,
-        auxiliary_power: Numeric = None,
+        auxiliary_power: Numeric = 0,
         weather: Weather = None,
         location: Location = None,
     ):
         self.timestamp_seconds = (
             np.array([timestamp_seconds])
             if isinstance(timestamp_seconds, (float, int))
             else timestamp_seconds
```

### Comparing `ship_model_lib-1.0.0/ship_model_lib/propulsor.py` & `ship_model_lib-1.0.1/ship_model_lib/propulsor.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib/ship_dimensions.py` & `ship_model_lib-1.0.1/ship_model_lib/ship_dimensions.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib/ship_model.py` & `ship_model_lib-1.0.1/ship_model_lib/ship_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from ship_model_lib.added_resistance import (
     WaveSpectrumType,
     AddedResistanceByStaWave2,
     AddedResistanceBySeaMarginCurve,
     AddedResistanceBySNNM,
     AddedResistanceWindITTC,
 )
-from .operation_profile_structure import Weather, OperationPoint
+from .operation_profile_structure import Weather, OperationPoint, Location
 from .utility import kn_to_m_per_s, m_per_s_to_kn, Interpolated1DValue
 from ship_model_lib.machinery import (
     Point,
     Curve,
     EmissionType,
     EmissionFactor,
     FuelByMassFraction,
@@ -456,48 +456,126 @@
         self, operation_point: OperationPoint
     ) -> ShipPerformanceData:
         """Calculates the ship performance data from the operating point.
 
         :param operation_point: The operating point
         :return: The ship performance data
         """
-        performance_data_from_speed = self.get_ship_performance_data_from_speed(
+        performance_data = self.get_ship_performance_data_from_speed(
             vessel_speed_kn=operation_point.speed_kn,
             weather=operation_point.weather,
             heading_deg=operation_point.heading_deg,
             auxiliary_power_kw=operation_point.auxiliary_power,
         )
         # Determine what power source data is available
         if self.machinery_system is not None:
             if self.machinery_system.propulsion_type is PropulsionType.MECHANICAL:
                 power_on_source_kw = (
-                    performance_data_from_speed.power_source_data.mechanical_system.power_on_source_kw
+                    performance_data.power_source_data.mechanical_system.power_on_source_kw
                 )
             elif self.machinery_system.propulsion_type is PropulsionType.ELECTRIC:
                 power_on_source_kw = (
-                    performance_data_from_speed.power_source_data.electric_system.power_on_source_kw
+                    performance_data.power_source_data.electric_system.power_on_source_kw
                 )
             else:
                 raise NotImplementedError(
                     "The power source data is not implemented for the propulsion type: {self.machinery_system.propulsion_type}"
                 )
         elif self.machinery_system is None and self.propulsor is not None:
-            power_on_source_kw = (
-                performance_data_from_speed.propeller_data.shaft_power_kw
-            )
+            power_on_source_kw = performance_data.propeller_data.shaft_power_kw
         elif self.machinery_system is None and self.propulsor is None:
-            power_on_source_kw = (
-                performance_data_from_speed.hull_data.total_towing_power_kw
-            )
+            power_on_source_kw = performance_data.hull_data.total_towing_power_kw
         else:
-            power_on_source_kw = 0
+            power_on_source_kw = np.zeros([len(operation_point.speed_kn)])
 
-        if power_on_source_kw > operation_point.power_limit_kw:
-            performance_data_from_power = self.get_ship_performance_data_from_power(
-                power_out_source_kw=operation_point.power_limit_kw,
+        greater_than_power_limit = np.greater(
+            power_on_source_kw, operation_point.power_limit_kw
+        )
+        if np.any(greater_than_power_limit):
+            for index, greater_than_power_limit_each in enumerate(
+                greater_than_power_limit
+            ):
+                if greater_than_power_limit_each:
+                    if operation_point.weather.significant_wave_height_m:
+                        significant_wave_height_m = (
+                            operation_point.weather.significant_wave_height_m[index]
+                        )
+                    else:
+                        significant_wave_height_m = None
+                    if operation_point.weather.mean_wave_period_s:
+                        mean_wave_period_s = operation_point.weather.mean_wave_period_s[
+                            index
+                        ]
+                    else:
+                        mean_wave_period_s = (None,)
+                    if operation_point.weather.wave_direction_deg:
+                        wave_direction_deg = operation_point.weather.wave_direction_deg[
+                            index
+                        ]
+                    else:
+                        wave_direction_deg = None
+                    if operation_point.weather.wind_speed_m_per_s:
+                        wind_speed_m_per_s = operation_point.weather.wind_speed_m_per_s[
+                            index
+                        ]
+                    else:
+                        wind_speed_m_per_s = None
+                    if operation_point.weather.wind_direction_deg:
+                        wind_direction_deg = operation_point.weather.wind_direction_deg[
+                            index
+                        ]
+                    else:
+                        wind_direction_deg = None
+                    if operation_point.weather.ocean_current_speed_m_per_s:
+                        ocean_current_speed_m_per_s = (
+                            operation_point.weather.ocean_current_speed_m_per_s[index]
+                        )
+                    else:
+                        ocean_current_speed_m_per_s = None
+                    if operation_point.weather.ocean_current_direction_deg:
+                        ocean_current_direction_deg = (
+                            operation_point.weather.ocean_current_direction_deg[index]
+                        )
+                    else:
+                        ocean_current_direction_deg = None
+                    weather = Weather(
+                        significant_wave_height_m=significant_wave_height_m,
+                        mean_wave_period_s=mean_wave_period_s,
+                        wave_direction_deg=wave_direction_deg,
+                        wind_speed_m_per_s=wind_speed_m_per_s,
+                        wind_direction_deg=wind_direction_deg,
+                        ocean_current_speed_m_per_s=ocean_current_speed_m_per_s,
+                        ocean_current_direction_deg=ocean_current_direction_deg,
+                    )
+                    if operation_point.power_limit_kw:
+                        power_limit_kw = operation_point.power_limit_kw[index]
+                    else:
+                        power_limit_kw = 1e6
+                    if operation_point.heading_deg:
+                        heading_deg = operation_point.heading_deg[index]
+                    else:
+                        heading_deg = None
+                    if operation_point.auxiliary_power:
+                        auxiliary_power_kw = operation_point.auxiliary_power[index]
+                    else:
+                        auxiliary_power_kw = 0
+                    performance_data_from_power = (
+                        self.get_ship_performance_data_from_power(
+                            power_out_source_kw=power_limit_kw,
+                            weather=weather,
+                            heading_deg=heading_deg,
+                            auxiliary_power_kw=auxiliary_power_kw,
+                        )
+                    )
+
+                    operation_point.speed_kn[index] = (
+                        performance_data_from_power.hull_data.vessel_speed_kn
+                    )
+
+            performance_data = self.get_ship_performance_data_from_speed(
+                vessel_speed_kn=operation_point.speed_kn,
                 weather=operation_point.weather,
                 heading_deg=operation_point.heading_deg,
                 auxiliary_power_kw=operation_point.auxiliary_power,
             )
-            return performance_data_from_power
-        else:
-            return performance_data_from_speed
+
+        return performance_data
```

### Comparing `ship_model_lib-1.0.0/ship_model_lib/types.py` & `ship_model_lib-1.0.1/ship_model_lib/types.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib/utility.py` & `ship_model_lib-1.0.1/ship_model_lib/utility.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/ship_model_lib.egg-info/PKG-INFO` & `ship_model_lib-1.0.1/ship_model_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ship_model_lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Model library for the hydrodynamics, energy system and fuel calculation
 Home-page: https://github.com/developer/https://github.com/SINTEF/shipdesignlab/
 Author: SINTEF Ocean
 Author-email: kevinkoosup.yum@sintef.no
 License: Apache Software License 2.0
 Keywords: Ship Energy Model
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ship_model_lib-1.0.0/ship_model_lib.egg-info/SOURCES.txt` & `ship_model_lib-1.0.1/ship_model_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/tests/test_added_resistance.py` & `ship_model_lib-1.0.1/tests/test_added_resistance.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/tests/test_machinery.py` & `ship_model_lib-1.0.1/tests/test_machinery.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/tests/test_propulsor.py` & `ship_model_lib-1.0.1/tests/test_propulsor.py`

 * *Files identical despite different names*

### Comparing `ship_model_lib-1.0.0/tests/test_ship_model.py` & `ship_model_lib-1.0.1/tests/test_ship_model.py`

 * *Files identical despite different names*

