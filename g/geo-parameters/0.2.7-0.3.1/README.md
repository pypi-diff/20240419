# Comparing `tmp/geo_parameters-0.2.7.tar.gz` & `tmp/geo_parameters-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_parameters-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geo_parameters-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geo_parameters-0.2.7.tar` & `geo_parameters-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1776 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3140 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/.gitignore
--rw-r--r--   0        0        0     1079 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/LICENSE
--rw-r--r--   0        0        0     3386 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/README.md
--rw-r--r--   0        0        0       91 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/environment.yml
--rw-r--r--   0        0        0      162 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/geo_parameters/__init__.py
--rw-r--r--   0        0        0      830 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/geo_parameters/grid.py
--rw-r--r--   0        0        0     1967 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/geo_parameters/metaparameter.py
--rw-r--r--   0        0        0     1280 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/geo_parameters/ocean.py
--rw-r--r--   0        0        0     1124 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/geo_parameters/parameter_funcs.py
--rw-r--r--   0        0        0       68 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/geo_parameters/ureg.py
--rw-r--r--   0        0        0    18426 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/geo_parameters/wave.py
--rw-r--r--   0        0        0     1702 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/geo_parameters/wind.py
--rw-r--r--   0        0        0      450 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0     1810 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/tests/test_doc.py
--rw-r--r--   0        0        0     1020 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/tests/test_funcs.py
--rw-r--r--   0        0        0      808 2024-04-16 11:21:56.685194 geo_parameters-0.2.7/tests/test_names.py
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 geo_parameters-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1776 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3140 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1079 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3386 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/README.md
+-rw-r--r--   0        0        0       91 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/environment.yml
+-rw-r--r--   0        0        0      253 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/geo_parameters/__init__.py
+-rw-r--r--   0        0        0      830 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/geo_parameters/grid.py
+-rw-r--r--   0        0        0     1967 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/geo_parameters/metaparameter.py
+-rw-r--r--   0        0        0     1280 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/geo_parameters/ocean.py
+-rw-r--r--   0        0        0     2696 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/geo_parameters/parameter_funcs.py
+-rw-r--r--   0        0        0       68 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/geo_parameters/ureg.py
+-rw-r--r--   0        0        0    18426 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/geo_parameters/wave.py
+-rw-r--r--   0        0        0     1702 2024-04-19 14:03:50.484163 geo_parameters-0.3.1/geo_parameters/wind.py
+-rw-r--r--   0        0        0      450 2024-04-19 14:03:50.488163 geo_parameters-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 14:03:50.488163 geo_parameters-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      353 2024-04-19 14:03:50.488163 geo_parameters-0.3.1/tests/test_decode.py
+-rw-r--r--   0        0        0     2064 2024-04-19 14:03:50.488163 geo_parameters-0.3.1/tests/test_doc.py
+-rw-r--r--   0        0        0     1032 2024-04-19 14:03:50.488163 geo_parameters-0.3.1/tests/test_funcs.py
+-rw-r--r--   0        0        0      576 2024-04-19 14:03:50.488163 geo_parameters-0.3.1/tests/test_isgp.py
+-rw-r--r--   0        0        0      808 2024-04-19 14:03:50.488163 geo_parameters-0.3.1/tests/test_names.py
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 geo_parameters-0.3.1/PKG-INFO
```

### Comparing `geo_parameters-0.2.7/.github/workflows/tests.yml` & `geo_parameters-0.3.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.7/.gitignore` & `geo_parameters-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.7/LICENSE` & `geo_parameters-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.7/README.md` & `geo_parameters-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.7/geo_parameters/grid.py` & `geo_parameters-0.3.1/geo_parameters/grid.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.7/geo_parameters/metaparameter.py` & `geo_parameters-0.3.1/geo_parameters/metaparameter.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.7/geo_parameters/ocean.py` & `geo_parameters-0.3.1/geo_parameters/ocean.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.7/geo_parameters/wave.py` & `geo_parameters-0.3.1/geo_parameters/wave.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.7/geo_parameters/wind.py` & `geo_parameters-0.3.1/geo_parameters/wind.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.7/tests/test_doc.py` & `geo_parameters-0.3.1/tests/test_doc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,70 @@
-from geo_parameters.wave import Hs, Tp
-from geo_parameters import get as gpget
-from geo_parameters import dict_of_parameters
+import geo_parameters as gp
+
+# import xarray as xr
+import numpy as np
+import sys
 
 
 def test_names():
-    assert Hs.standard_name() == "sea_surface_wave_significant_height"
-    assert Hs.name == "hs"
-    hsig = Hs()
+    assert gp.wave.Hs.standard_name() == "sea_surface_wave_significant_height"
+    assert gp.wave.Hs.name == "hs"
+    hsig = gp.wave.Hs()
     assert hsig.name == "hs"
 
-    hsig = Hs(name="hsig")
+    hsig = gp.wave.Hs(name="hsig")
     assert hsig.name == "hsig"
 
     assert hsig.standard_name() == "sea_surface_wave_significant_height"
     assert hsig.long_name() == "significant_wave_height"
 
     assert (
         hsig.standard_name(alias=True) == "significant_height_of_wind_and_swell_waves"
     )
 
     assert (
-        Tp.standard_name(alias=True)
+        gp.wave.Tp.standard_name(alias=True)
         == "sea_surface_wave_period_at_variance_spectral_density_maximum"
     )
 
     assert (
-        Tp.standard_name()
+        gp.wave.Tp.standard_name()
         == "sea_surface_wave_period_at_variance_spectral_density_maximum"
     )
 
 
 def test_get():
-    assert gpget("sea_surface_wave_significant_height") == Hs
+    assert gp.get("sea_surface_wave_significant_height") == gp.wave.Hs
+    assert gp.get("significant_height_of_wind_and_swell_waves") == gp.wave.Hs
+    assert gp.get("hs") is None
+    assert gp.shortget("hs") == gp.wave.Hs
+
     # <class 'geo_parameters.geo_parameters.wave.Hs'>
 
 
 def test_dicts():
-    dict_of_parameters()
-    dict_of_parameters(short=True)
-    dict_of_parameters(alias=True)
-
-
-# def test_ds_find_me():
-#     ds = xr.Dataset(
-#         data_vars=dict(
-#             interesting_hs_name=(["lat", "lon"], np.zeros((11, 6))),
-#             peak_period=(["lat", "lon"], np.ones((11, 6))),
-#         ),
-#         coords=dict(
-#             lon=(["lon"], np.linspace(5, 10, 6)),
-#             lat=(["lat"], np.linspace(50, 60, 11)),
-#         ),
-#     )
-#     ds.interesting_hs_name.attrs = {
-#         "standard_name": "sea_surface_wave_significant_height"
-#     }
-
-#     ds.peak_period.attrs = {
-#         "standard_name": "sea_surface_wave_period_at_variance_spectral_density_maximum"
-#     }
-#     assert Hs.find_me_in_ds(ds) == "interesting_hs_name"
-#     assert Tp.find_me_in_ds(ds) == "peak_period"
+    gp.dict_of_parameters()
+    gp.dict_of_parameters(short=True)
+    gp.dict_of_parameters(alias=True)
+
+
+def test_ds_find_me():
+    if "xr" in sys.modules:
+        ds = xr.Dataset(
+            data_vars=dict(
+                interesting_hs_name=(["lat", "lon"], np.zeros((11, 6))),
+                peak_period=(["lat", "lon"], np.ones((11, 6))),
+            ),
+            coords=dict(
+                lon=(["lon"], np.linspace(5, 10, 6)),
+                lat=(["lat"], np.linspace(50, 60, 11)),
+            ),
+        )
+        ds.interesting_hs_name.attrs = {
+            "standard_name": "sea_surface_wave_significant_height"
+        }
+
+        ds.peak_period.attrs = {
+            "standard_name": "sea_surface_wave_period_at_variance_spectral_density_maximum"
+        }
+        assert gp.wave.Hs.find_me_in_ds(ds) == "interesting_hs_name"
+        assert gp.wave.Tp.find_me_in_ds(ds) == "peak_period"
```

### Comparing `geo_parameters-0.2.7/tests/test_names.py` & `geo_parameters-0.3.1/tests/test_names.py`

 * *Files identical despite different names*

