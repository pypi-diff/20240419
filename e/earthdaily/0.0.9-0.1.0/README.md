# Comparing `tmp/earthdaily-0.0.9.tar.gz` & `tmp/earthdaily-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthdaily-0.0.9.tar", last modified: Thu Feb 29 09:57:30 2024, max compression
+gzip compressed data, was "earthdaily-0.1.0.tar", last modified: Fri Apr 19 09:46:40 2024, max compression
```

## Comparing `earthdaily-0.0.9.tar` & `earthdaily-0.1.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-29 09:57:29.000000 earthdaily-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-02-29 09:57:30.363389 earthdaily-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-02-29 09:57:29.000000 earthdaily-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.359389 earthdaily-0.0.9/earthdaily/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/accessor/
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/accessor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/datasets/data/pivot.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/datasets/data/pivot_corumba.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/earthdatastore/
--rw-r--r--   0 runner    (1001) docker     (127)    37000 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/_scales_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/
--rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/_zonal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/custom_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/geometry_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/harmonizer/
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/earthdatastore/mask/
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/mask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 09:57:30.363389 earthdaily-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-29 09:57:29.000000 earthdaily-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.738356 earthdaily-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-19 09:46:40.000000 earthdaily-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-19 09:46:40.738356 earthdaily-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-19 09:46:40.000000 earthdaily-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/accessor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/accessor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/accessor/whittaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/accessor/whittaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/accessor/whittaker/_pywapor_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/datasets/data/pivot.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/datasets/data/pivot_corumba.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/earthdatastore/
+-rw-r--r--   0 runner    (1001) docker     (127)    37396 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/_scales_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/_zonal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.738356 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/custom_reducers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/geometry_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.738356 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/harmonizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.738356 earthdaily-0.1.0/earthdaily/earthdatastore/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily/earthdatastore/mask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:46:40.734356 earthdaily-0.1.0/earthdaily.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 09:46:40.000000 earthdaily-0.1.0/earthdaily.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:46:40.738356 earthdaily-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-19 09:46:40.000000 earthdaily-0.1.0/setup.py
```

### Comparing `earthdaily-0.0.9/LICENSE` & `earthdaily-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.9/PKG-INFO` & `earthdaily-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthdaily
-Version: 0.0.9
+Version: 0.1.0
 Summary: earthdaily: easy authentication, search and retrieval of Earth Data Store collections data
 Home-page: UNKNOWN
 Author: EarthDaily Agro
 License: MIT
 Keywords: Earth Data Store,earthdaily,earthdailyagro,stac
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zwz_02i7_/tmprdg0yxpr_TarContainer/0/2", line 25, column 36: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthdaily Version: 0.0.9 Summary: earthdaily: easy
+Metadata-Version: 2.1 Name: earthdaily Version: 0.1.0 Summary: earthdaily: easy
 authentication, search and retrieval of Earth Data Store collections data Home-
 page: UNKNOWN Author: EarthDaily Agro License: MIT Keywords: Earth Data
 Store,earthdaily,earthdailyagro,stac Platform: UNKNOWN Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 
 ************ EEaarrtthhDDaaiillyy PPyytthhoonn CClliieenntt ************
 Your gateway to the Earth Data Store STAC Catalog.
```

### Comparing `earthdaily-0.0.9/README.md` & `earthdaily-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.9/earthdaily/accessor/__init__.py` & `earthdaily-0.1.0/earthdaily/accessor/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,67 +3,20 @@
 import rioxarray as rxr
 import numpy as np
 import pandas as pd
 import geopandas as gpd
 from shapely.geometry import Point
 from dask import array as da
 import spyndex
-from dask_image import ndfilters as ndimage
-
+from dask_image import ndfilters as dask_ndimage
+from scipy import ndimage
 from xarray.core.extensions import AccessorRegistrationWarning
-
-warnings.filterwarnings("ignore", category=AccessorRegistrationWarning)
-
-
-class MisType(Warning):
-    pass
-
-
-_SUPPORTED_DTYPE = [int, float, list, bool, str]
-
-
-def _typer(raise_mistype=False):
-    def decorator(func):
-        def force(*args, **kwargs):
-            _args = list(args)
-            idx = 1
-            for key, val in func.__annotations__.items():
-                is_kwargs = key in kwargs.keys()
-                if not is_kwargs and idx >= len(args):
-                    continue
-                input_value = kwargs.get(key, None) if is_kwargs else args[idx]
-                if type(input_value) == val:
-                    continue
-                if raise_mistype and (
-                    val != type(kwargs.get(key))
-                    if is_kwargs
-                    else val != type(args[idx])
-                ):
-                    if is_kwargs:
-                        expected = f"{type(kwargs[key]).__name__} ({kwargs[key]})"
-                    else:
-                        expected = f"{type(args[idx]).__name__} ({args[idx]})"
-
-                        raise MisType(
-                            f"{key} expected a {val.__name__}, not a {expected}."
-                        )
-                if is_kwargs:
-                    kwargs[key] = val(kwargs[key]) if val != list else [kwargs[key]]
-                elif len(args) >= idx:
-                    _args[idx] = val(args[idx]) if val != list else [args[idx]]
-                idx += 1
-            args = tuple(_args)
-            return func(*args, **kwargs)
-
-        return force
-
-    return decorator
+from ..earthdatastore.cube_utils import GeometryManager
 
 
-@_typer()
 def xr_loop_func(
     dataset: xr.Dataset,
     func,
     to_numpy: bool = False,
     loop_dimension: str = "time",
     **kwargs,
 ):
@@ -86,28 +39,20 @@
             )
 
     return dataset.map(
         func=_xr_loop_func, metafunc=func, loop_dimension=loop_dimension, **kwargs
     )
 
 
-@_typer()
 def _lee_filter(img, window_size: int):
-    try:
-        from dask_image import ndfilters
-    except ImportError:
-        raise ImportError("Please install dask-image to run lee_filter")
-
     img_ = img.copy()
-    ndimage_type = ndfilters
-    if hasattr(img, "data"):
-        if isinstance(img.data, (memoryview, np.ndarray)):
-            ndimage_type = ndimage
-        img = img.data
-    # print(ndimage_type)
+    if isinstance(img, np.ndarray):
+        ndimage_type = ndimage
+    else:
+        ndimage_type = dask_ndimage
     binary_nan = ndimage_type.minimum_filter(
         xr.where(np.isnan(img), 0, 1), size=window_size
     )
     binary_nan = np.where(binary_nan == 0, np.nan, 1)
     img = xr.where(np.isnan(img), 0, img)
     window_size = da.from_array([window_size, window_size, 1])
 
@@ -120,97 +65,109 @@
     img_weights = img_variance / (np.add(img_variance, overall_variance))
 
     img_output = img_mean + img_weights * (np.subtract(img, img_mean))
     img_output = xr.where(np.isnan(binary_nan), img_, img_output)
     return img_output
 
 
+def _xr_rio_clip(datacube, geom):
+    geom = GeometryManager(geom).to_geopandas()
+    geom = geom.to_crs(datacube.rio.crs)
+    return datacube.rio.clip(geom.geometry)
+
+
 @xr.register_dataarray_accessor("ed")
 class EarthDailyAccessorDataArray:
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
 
-    def _max_time_wrap(self, wish=5):
-        return np.min((wish, self._obj["time"].size))
+    def clip(self, geom):
+        return _xr_rio_clip(self._obj, geom)
 
-    @_typer()
-    def plot_band(self, cmap="Greys", col="time", col_wrap=5, **kwargs):
-        return self._obj.plot.imshow(
-            cmap=cmap, col=col, col_wrap=self._max_time_wrap(col_wrap), **kwargs
-        )
+    def _max_time_wrap(self, wish=5, col="time"):
+        return np.min((wish, self._obj[col].size))
 
-    @_typer()
-    def plot_index(
-        self, cmap="RdYlGn", vmin=-1, vmax=1, col="time", col_wrap=5, **kwargs
-    ):
+    def plot_band(self, cmap="Greys", col="time", col_wrap=5, **kwargs):
         return self._obj.plot.imshow(
-            vmin=vmin,
-            vmax=vmax,
             cmap=cmap,
             col=col,
-            col_wrap=self._max_time_wrap(col_wrap),
+            col_wrap=self._max_time_wrap(col_wrap, col=col),
             **kwargs,
         )
 
+    def whittaker(
+        self,
+        lmbd: float,
+        weights: np.ndarray = None,
+        a: float = 0.5,
+        min_value: float = -np.inf,
+        max_value: float = np.inf,
+        max_iter: int = 10,
+        time="time",
+    ):
+        from . import whittaker
+
+        return whittaker.xr_wt(
+            self._obj.to_dataset(name="index"),
+            lmbd,
+            time=time,
+            weights=weights,
+            a=a,
+            min_value=min_value,
+            max_value=max_value,
+            max_iter=max_iter,
+        )["index"]
+
 
 @xr.register_dataset_accessor("ed")
 class EarthDailyAccessorDataset:
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
 
-    def _max_time_wrap(self, wish=5):
-        return np.min((wish, self._obj["time"].size))
+    def clip(self, geom):
+        return _xr_rio_clip(self._obj, geom)
+
+    def _max_time_wrap(self, wish=5, col="time"):
+        return np.min((wish, self._obj[col].size))
 
-    @_typer()
     def plot_rgb(
         self,
         red: str = "red",
         green: str = "green",
         blue: str = "blue",
         col="time",
         col_wrap=5,
         **kwargs,
     ):
         return (
             self._obj[[red, green, blue]]
             .to_array(dim="bands")
-            .plot.imshow(col=col, col_wrap=self._max_time_wrap(col_wrap), **kwargs)
+            .plot.imshow(
+                col=col, col_wrap=self._max_time_wrap(col_wrap, col=col), **kwargs
+            )
         )
 
-    @_typer()
     def plot_band(self, band, cmap="Greys", col="time", col_wrap=5, **kwargs):
         return self._obj[band].plot.imshow(
-            cmap=cmap, col=col, col_wrap=self._max_time_wrap(col_wrap), **kwargs
-        )
-
-    @_typer()
-    def plot_index(
-        self, index, cmap="RdYlGn", vmin=-1, vmax=1, col="time", col_wrap=5, **kwargs
-    ):
-        return self._obj[index].plot.imshow(
-            vmin=vmin,
-            vmax=vmax,
             cmap=cmap,
             col=col,
-            col_wrap=self._max_time_wrap(col_wrap),
+            col_wrap=self._max_time_wrap(col_wrap, col=col),
             **kwargs,
         )
 
-    @_typer()
-    def lee_filter(self, window_size: int = 7):
+    def lee_filter(self, window_size: int):
         return xr.apply_ufunc(
             _lee_filter,
             self._obj,
             input_core_dims=[["time"]],
             dask="allowed",
             output_core_dims=[["time"]],
             kwargs=dict(window_size=window_size),
         )
 
-    @_typer()
     def centroid(self, to_wkt: str = False, to_4326: bool = True):
         """Return the geographic center point in 4326/WKT of this dataset."""
         # we can use a cache on our accessor objects, because accessors
         # themselves are cached on instances that access them.
         lon = float(self._obj.x[int(self._obj.x.size / 2)])
         lat = float(self._obj.y[int(self._obj.y.size / 2)])
         point = gpd.GeoSeries([Point(lon, lat)], crs=self._obj.rio.crs)
@@ -265,59 +222,97 @@
                 if needed_band not in mapper:
                     missing_bands = True
                     break
             if missing_bands is False:
                 available_indices.append(spyndex.indices[k] if details else k)
         return available_indices
 
-    @_typer()
-    def add_indices(self, index: list, **kwargs):
+    def add_indices(self, indices: list, **kwargs):
         """
         Uses spyndex to compute and add index.
 
         For list of indices, see https://github.com/awesome-spectral-indices/awesome-spectral-indices.
 
 
         Parameters
         ----------
-        index : list
+        indices : list
             ['NDVI'].
         Returns
         -------
         xr.Dataset
             The input xr.Dataset with new data_vars of indices.
 
         """
 
         params = {}
         params = self._auto_mapper()
         params.update(**kwargs)
-        idx = spyndex.computeIndex(index=index, params=params, **kwargs)
+        idx = spyndex.computeIndex(index=indices, params=params, **kwargs)
 
-        if len(index) == 1:
-            idx = idx.expand_dims(index=index)
+        if len(indices) == 1:
+            idx = idx.expand_dims(index=indices)
         idx = idx.to_dataset(dim="index")
 
         return xr.merge((self._obj, idx))
 
-    @_typer()
     def sel_nearest_dates(
         self,
-        target,
+        target: (xr.Dataset, xr.DataArray),
         max_delta: int = 0,
         method: str = "nearest",
         return_target: bool = False,
     ):
         src_time = self._obj.sel(time=target.time.dt.date, method=method).time.dt.date
         target_time = target.time.dt.date
         pos = np.abs(src_time.data - target_time.data)
         pos = [
             src_time.isel(time=i).time.values
             for i, j in enumerate(pos)
             if j.days <= max_delta
         ]
+        pos = np.unique(pos)
         if return_target:
             method_convert = {"bfill": "ffill", "ffill": "bfill", "nearest": "nearest"}
             return self._obj.sel(time=pos), target.sel(
                 time=pos, method=method_convert[method]
             )
         return self._obj.sel(time=pos)
+
+    def whittaker(
+        self,
+        lmbd: float,
+        weights: np.ndarray = None,
+        a: float = 0.5,
+        min_value: float = -np.inf,
+        max_value: float = np.inf,
+        max_iter: int = 10,
+        time="time",
+    ):
+        from . import whittaker
+
+        return whittaker.xr_wt(
+            self._obj,
+            lmbd,
+            time=time,
+            weights=weights,
+            a=a,
+            min_value=min_value,
+            max_value=max_value,
+            max_iter=max_iter,
+        )
+
+    def zonal_stats(
+        self,
+        geometry,
+        operations: list = ["mean"],
+        raise_missing_geometry: bool = False,
+    ):
+        from ..earthdatastore.cube_utils import zonal_stats, GeometryManager
+
+        geometry = GeometryManager(geometry).to_geopandas()
+        return zonal_stats(
+            self._obj,
+            geometry,
+            operations=operations,
+            raise_missing_geometry=raise_missing_geometry,
+        )
```

### Comparing `earthdaily-0.0.9/earthdaily/datasets/__init__.py` & `earthdaily-0.1.0/earthdaily/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.9/earthdaily/datasets/data/pivot.geojson` & `earthdaily-0.1.0/earthdaily/datasets/data/pivot.geojson`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.9/earthdaily/datasets/data/pivot_corumba.geojson` & `earthdaily-0.1.0/earthdaily/datasets/data/pivot_corumba.geojson`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/__init__.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -646,14 +646,15 @@
             else:
                 mask_with = mask._native_mask_def_mapping.get(collections[0], None)
                 if isinstance(assets, list):
                     assets.append(mask_with)
 
         if intersects is not None:
             intersects = cube_utils.GeometryManager(intersects).to_geopandas()
+            self.intersects = intersects
         items = self.search(
             collections=collections,
             bbox=bbox,
             intersects=intersects,
             datetime=datetime,
             prefer_alternate=prefer_alternate,
             add_default_scale_factor=add_default_scale_factor,
@@ -741,15 +742,14 @@
                 )
 
             Mask = mask.Mask(xr_datacube, intersects=intersects, bbox=bbox)
             xr_datacube = getattr(Mask, mask_with)(**mask_kwargs)
 
             if clear_cover:
                 xr_datacube = mask.filter_clear_cover(xr_datacube, clear_cover)
-
         return xr_datacube
 
     def _update_search_for_assets(self, assets):
         fields = {
             "include": [
                 "id",
                 "type",
@@ -937,16 +937,26 @@
                 )
             return products
 
         items_id = ag_cloud_mask_from_items(items_collection)
         if len(items_id) == 0:
             raise ValueError("Sorry, no ag_cloud_mask available.")
         collections = list(items_id.keys())
-        ids = [x for n in (items_id.values()) for x in n]
-        return self.search(collections=collections, ids=ids)
+        ids_ = [x for n in (items_id.values()) for x in n]
+        items_list = []
+        step = 100
+        for items_start_idx in range(0, len(ids_), step):
+            items = self.search(
+                collections=collections,
+                # intersects=self.intersects,
+                ids=ids_[items_start_idx : items_start_idx + step],
+                limit=step,
+            )
+            items_list.extend(list(items))
+        return ItemCollection(items_list)
 
 
 def item_property_to_df(
     item,
     asset="data",
     property_name="raster:bands",
     sub_property_name="classification:classes",
```

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/_scales_collections.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/_scales_collections.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/__init__.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-import logging
-from datetime import datetime
 from collections import defaultdict
+import logging
 import pandas as pd
 import geopandas as gpd
 import numpy as np
-import pytz
 import xarray as xr
 from rasterio.enums import Resampling
 from shapely.geometry import box
 from .geometry_manager import GeometryManager
 from ._zonal import zonal_stats, zonal_stats_numpy
 from .harmonizer import Harmonizer
 from .asset_mapper import AssetMapper
 import rioxarray
 from functools import wraps
+import json
 
 __all__ = ["GeometryManager", "rioxarray", "zonal_stats", "zonal_stats_numpy"]
 
 
 def _datacubes(method):
     @wraps(method)
     def _impl(self, *args, **kwargs):
@@ -38,15 +37,15 @@
             datacube = method(self, *args, **kwargs)
         return datacube
 
     return _impl
 
 
 def _match_xy_dims(src, dst, resampling=Resampling.nearest):
-    if src.sizes != dst.sizes:
+    if (src.sizes["x"], src.sizes["y"]) != (dst.sizes["x"], dst.sizes["y"]):
         src = src.rio.reproject_match(dst, resampling=resampling)
     return src
 
 
 def _bbox_to_intersects(bbox):
     if isinstance(bbox, str):
         bbox = [float(i) for i in bbox.split(",")]
@@ -114,14 +113,16 @@
                     metadata[k].append(v)
         # to avoid mismatch if some properties are not available on all items
         df = pd.DataFrame.from_dict(metadata, orient="index").T
         # convert to xarray needs
         metadata = {k: ("time", v.tolist()) for k, v in df.items()}
         # assign metadata as coords
         ds = ds.assign_coords(**metadata)
+    ds = ds.chunk(kwargs["chunks"])
+
     return ds
 
 
 def _cube_stackstac(items_collection, assets=None, times=None, **kwargs):
     from stackstac import stack
 
     if "epsg" in kwargs:
@@ -245,14 +246,24 @@
         if ds.time.size != np.unique(ds.time.dt.strftime("%Y%m%d")).size:
             ds = ds.groupby("time.date")
             ds = getattr(ds, groupby_date)().rename(dict(date="time"))
     ds["time"] = ds.time.astype("<M8[ns]")
 
     if isinstance(assets, dict):
         ds = ds.rename(assets)
+
+    for coord in ds.coords:
+        if ds.coords[coord].values.shape == ():
+            continue
+        if isinstance(ds.coords[coord].values[0], (list, dict)):
+            ds.coords[coord].values = [
+                json.dumps(ds.coords[coord].values[idx])
+                for idx in range(ds.coords[coord].size)
+            ]
+
     return ds
 
 
 def rescale_assets_with_items(
     items_collection,
     ds,
     assets=None,
@@ -354,22 +365,17 @@
                 scales[ds_asset][scale][offset].append(time)
     if len(scales) > 0:
         ds_scaled = {}
         for asset in scales.keys():
             ds_scaled[asset] = []
             for scale in scales[asset].keys():
                 for offset in scales[asset][scale].keys():
-                    times = list(set(scales[asset][scale][offset]))
-                    if len(times) != len(scales[asset][scale][offset]):
-                        for time in times:
-                            d = ds[[asset]].loc[dict(time=time)] * scale + offset
-                            ds_scaled[asset].append(d)
-                    else:
-                        d = ds[[asset]].loc[dict(time=times)] * scale + offset
-                        ds_scaled[asset].append(d)
+                    times = np.in1d(ds.time, list(set(scales[asset][scale][offset])))
+                    asset_scaled = ds[[asset]].isel(time=times) * scale + offset
+                    ds_scaled[asset].append(asset_scaled)
         ds_ = []
         for k, v in ds_scaled.items():
             ds_k = []
             for d in v:
                 ds_k.append(d)
             ds_.append(xr.concat(ds_k, dim="time"))
         attrs = ds.attrs
```

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/_zonal.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/_zonal.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 @author: nkk
 """
 
 from rasterio import features
 import numpy as np
 import xarray as xr
 import tqdm
-from . import custom_operations
+
+from . import custom_reducers
 from .preprocessing import rasterize
 from scipy.sparse import csr_matrix
 
 
 def _compute_M(data):
     cols = np.arange(data.size)
     return csr_matrix((cols, (data.ravel(), cols)), shape=(data.max() + 1, data.size))
@@ -101,19 +102,87 @@
     tqdm_bar.close()
     return xr.merge(ds).transpose("feature", "time", "stats")
 
 
 def zonal_stats(
     dataset,
     gdf,
-    operations=["mean"],
+    operations: list = ["mean"],
     all_touched=False,
-    method="optimized",
+    method="geocube",
     verbose=False,
+    raise_missing_geometry=False,
 ):
+    """
+
+
+    Parameters
+    ----------
+    dataset : xr.Dataset
+        DESCRIPTION.
+    gdf : gpd.GeoDataFrame
+        DESCRIPTION.
+    operations : TYPE, list.
+        DESCRIPTION. The default is ["mean"].
+    all_touched : TYPE, optional
+        DESCRIPTION. The default is False.
+    method : TYPE, optional
+        DESCRIPTION. The default is "geocube".
+    verbose : TYPE, optional
+        DESCRIPTION. The default is False.
+    raise_missing_geometry : TYPE, optional
+        DESCRIPTION. The default is False.
+
+    Raises
+    ------
+    ValueError
+        DESCRIPTION.
+    NotImplementedError
+        DESCRIPTION.
+
+    Returns
+    -------
+    TYPE
+        DESCRIPTION.
+
+    """
+    if method == "geocube":
+        from geocube.api.core import make_geocube
+        from geocube.rasterize import rasterize_image
+
+        def custom_rasterize_image(all_touched=all_touched, **kwargs):
+            return rasterize_image(all_touched=all_touched, **kwargs)
+
+        gdf["tmp_index"] = np.arange(gdf.shape[0])
+        out_grid = make_geocube(
+            gdf,
+            measurements=["tmp_index"],
+            like=dataset,  # ensure the data are on the same grid
+            rasterize_function=custom_rasterize_image,
+        )
+        cube = dataset.groupby(out_grid.tmp_index)
+        zonal_stats = xr.concat(
+            [getattr(cube, operation)() for operation in operations], dim="stats"
+        )
+        zonal_stats["stats"] = operations
+
+        if zonal_stats["tmp_index"].size != gdf.shape[0]:
+            index_list = [
+                gdf.index[i] for i in zonal_stats["tmp_index"].values.astype(np.int16)
+            ]
+            if raise_missing_geometry:
+                diff = gdf.shape[0] - len(index_list)
+                raise ValueError(
+                    f'{diff} geometr{"y is" if diff==1 else "ies are"} missing in the zonal stats. This can be due to too small geometries, duplicated...'
+                )
+        else:
+            index_list = list(gdf.index)
+        zonal_stats["tmp_index"] = index_list
+        return zonal_stats.rename(dict(tmp_index="feature"))
+
     tqdm_bar = tqdm.tqdm(total=gdf.shape[0])
 
     if dataset.rio.crs != gdf.crs:
         Warning(
             f"Different projections. Reproject vector to EPSG:{dataset.rio.crs.to_epsg()}."
         )
         gdf = gdf.to_crs(dataset.rio.crs)
```

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 import json
 
 eds = earthdaily.earthdatastore.Auth()
 asset_mapper_path = (
     earthdaily.earthdatastore.cube_utils.asset_mapper.__asset_mapper_config_path
 )
 asset_mapper_config = (
-    earthdaily.earthdatastore.cube_utils.asset_mapper.__asset_mapper_config
+    earthdaily.earthdatastore.cube_utils.asset_mapper._asset_mapper_config
 )
 
 for collection in eds.explore():
     try:
         assets_name = list(eds.explore(collection).item.assets.keys())
     except AttributeError:
         print(f"collection {collection} has no items")
         continue
     for asset_name in assets_name:
+        print(asset_name)
         if asset_mapper_config.get(collection) is None:
             asset_mapper_config[collection] = [{}]
         if asset_name not in asset_mapper_config[collection][0].values():
             asset_mapper_config[collection][0][asset_name] = asset_name
 
 with open(asset_mapper_path, "w", encoding="utf-8") as f:
     json.dump(asset_mapper_config, f, ensure_ascii=False, indent=4)
```

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json` & `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/custom_operations.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/custom_reducers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import xarray as xr
 from xarray.core import groupby
 import numpy as np
 
 
-class CustomOperations:
+class CustomReducers:
     @staticmethod
     def _np_mode(arr, **kwargs):
         if isinstance(arr, list):
             arr = np.asarray(arr)
         if isinstance(arr, xr.Dataset | xr.DataArray):
             if arr.chunks is not None:
                 arr = arr.compute()
@@ -18,21 +18,21 @@
         values, counts = values[~rm], counts[~rm]
         return values[np.argmax(counts)]
 
     @staticmethod
     def mode(data_array_grouped, optional_arg=None):
         # Apply _xrmode to DataArrayGroupBy object
         result = data_array_grouped.reduce(
-            CustomOperations._np_mode,
+            CustomReducers._np_mode,
             list(dim for dim in data_array_grouped.dims if dim != "time"),
         )
         return result
 
     @staticmethod
-    def register_custom_operations():
+    def register_custom_reducers():
         # register custom methods fo DataArrayGroupBy
-        xr.core.groupby.DataArrayGroupBy.mode = CustomOperations.mode
-        xr.core.groupby.DatasetGroupBy.mode = CustomOperations.mode
-        np.mode = CustomOperations._np_mode
+        xr.core.groupby.DataArrayGroupBy.mode = CustomReducers.mode
+        xr.core.groupby.DatasetGroupBy.mode = CustomReducers.mode
+        np.mode = CustomReducers._np_mode
 
 
-CustomOperations.register_custom_operations()
+CustomReducers.register_custom_reducers()
```

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/geometry_manager.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/geometry_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 
 class GeometryManager:
     def __init__(self, geometry):
         self.geometry = geometry
         self._obj = self.to_geopandas()
 
+    def __call__(self):
+        return self._obj
+
     def to_intersects(self, crs="EPSG:4326"):
         return json.loads(self._obj.to_crs(crs).dissolve().to_json(drop_id=True))[
             "features"
         ][0]["geometry"]
 
     def to_wkt(self, crs="EPSG:4326"):
         wkts = list(self._obj.to_crs(crs=crs).to_wkt()["geometry"])
@@ -39,23 +42,36 @@
                 self.input_type = "wkt"
                 return gpd.GeoDataFrame(
                     geometry=[shapely.wkt.loads(geometry)], crs="EPSG:4326"
                 )
             except:
                 pass
         if isinstance(geometry, (dict, str)):
-            if isinstance(geometry, str):
-                geometry = json.loads(geometry)
-            self.input_type = "geojson"
+            self.input_type = "GeoJson"
             try:
-                return gpd.GeoDataFrame.from_features(geometry, crs="EPSG:4326")
+                return gpd.read_file(geometry, driver="GeoJson", crs="EPSG:4326")
             except:
-                if "type" in geometry:
-                    geom = shapely.__dict__[geometry["type"]](
-                        geometry["coordinates"][0]
-                    )
-                    return gpd.GeoDataFrame(geometry=[geom])
+                try:
+                    return gpd.GeoDataFrame.from_features(geometry, crs="EPSG:4326")
+                except:
+                    if "type" in geometry:
+                        geom = shapely.__dict__[geometry["type"]](
+                            [geometry["coordinates"][0]]
+                        )
+                        return gpd.GeoDataFrame(geometry=[geom], crs="EPSG:4326")
         elif isinstance(geometry, gpd.GeoSeries):
             self.input_type = "GeoSeries"
-            return gpd.GeoDataFrame(geometry=geometry, crs="EPSG:4326")
+
+            return gpd.GeoDataFrame(
+                geometry=geometry,
+                crs="EPSG:4326" if geometry.crs is None else geometry.crs,
+            )
         else:
             raise NotImplementedError("Couldn't guess your geometry type")
+
+    def buffer_in_meter(self, distance: int, crs_meters: str = "EPSG:3857", **kwargs):
+        return (
+            self._obj.to_crs(crs=crs_meters)
+            .buffer(distance=distance, **kwargs)
+            .to_crs(crs=self._obj.crs)
+            .geometry
+        )
```

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/preprocessing.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/cube_utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.9/earthdaily/earthdatastore/mask/__init__.py` & `earthdaily-0.1.0/earthdaily/earthdatastore/mask/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
                     np.multiply(
                         n_pixels_as_labels / self._obj.attrs["usable_pixels"],
                         100,
                     ).astype(np.int8),
                 )
             }
         )
+        # self._obj = self._obj.reset_coords(names=['clear_pixels','clear_percent'])
 
         return self._obj
 
     def compute_available_pixels(self):
         if self.intersects is None:
             raise ValueError(
                 "bbox or intersects must be defined for now to compute cloud statistics."
```

### Comparing `earthdaily-0.0.9/earthdaily.egg-info/PKG-INFO` & `earthdaily-0.1.0/earthdaily.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthdaily
-Version: 0.0.9
+Version: 0.1.0
 Summary: earthdaily: easy authentication, search and retrieval of Earth Data Store collections data
 Home-page: UNKNOWN
 Author: EarthDaily Agro
 License: MIT
 Keywords: Earth Data Store,earthdaily,earthdailyagro,stac
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zwz_02i7_/tmprdg0yxpr_TarContainer/0/32", line 25, column 36: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthdaily Version: 0.0.9 Summary: earthdaily: easy
+Metadata-Version: 2.1 Name: earthdaily Version: 0.1.0 Summary: earthdaily: easy
 authentication, search and retrieval of Earth Data Store collections data Home-
 page: UNKNOWN Author: EarthDaily Agro License: MIT Keywords: Earth Data
 Store,earthdaily,earthdailyagro,stac Platform: UNKNOWN Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 
 ************ EEaarrtthhDDaaiillyy PPyytthhoonn CClliieenntt ************
 Your gateway to the Earth Data Store STAC Catalog.
```

### Comparing `earthdaily-0.0.9/earthdaily.egg-info/SOURCES.txt` & `earthdaily-0.1.0/earthdaily.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 earthdaily.egg-info/PKG-INFO
 earthdaily.egg-info/SOURCES.txt
 earthdaily.egg-info/dependency_links.txt
 earthdaily.egg-info/not-zip-safe
 earthdaily.egg-info/requires.txt
 earthdaily.egg-info/top_level.txt
 earthdaily/accessor/__init__.py
+earthdaily/accessor/whittaker/__init__.py
+earthdaily/accessor/whittaker/_pywapor_core.py
 earthdaily/datasets/__init__.py
 earthdaily/datasets/data/__init__.py
 earthdaily/datasets/data/pivot.geojson
 earthdaily/datasets/data/pivot_corumba.geojson
 earthdaily/earthdatastore/__init__.py
 earthdaily/earthdatastore/_scales_collections.py
 earthdaily/earthdatastore/cube_utils/__init__.py
 earthdaily/earthdatastore/cube_utils/_zonal.py
-earthdaily/earthdatastore/cube_utils/custom_operations.py
+earthdaily/earthdatastore/cube_utils/custom_reducers.py
 earthdaily/earthdatastore/cube_utils/geometry_manager.py
 earthdaily/earthdatastore/cube_utils/preprocessing.py
 earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
 earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
 earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
 earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
 earthdaily/earthdatastore/mask/__init__.py
```

### Comparing `earthdaily-0.0.9/setup.py` & `earthdaily-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,17 @@
         "rasterio",
         "rioxarray",
         "tqdm",
         "python-dotenv",
         "rich",
         "dask",
         "spyndex",
-        "dask-image"
+        "dask-image",
+        "numba",
+        "geocube"
     ],
     include_package_data=True,
     package_data={"":['*.geojson','*.json']},
     license="MIT",
     zip_safe=False,
     keywords=["Earth Data Store", "earthdaily", "earthdailyagro", "stac"],
 )
```

