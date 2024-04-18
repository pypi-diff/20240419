# Comparing `tmp/terrapyn-0.1.1.tar.gz` & `tmp/terrapyn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrapyn-0.1.1.tar", max compression
+gzip compressed data, was "terrapyn-0.1.2.tar", max compression
```

## Comparing `terrapyn-0.1.1.tar` & `terrapyn-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,30 @@
--rw-r--r--   0        0        0      126 2024-03-15 16:38:05.339691 terrapyn-0.1.1/AUTHORS.md
--rw-r--r--   0        0        0     1468 2024-03-15 16:38:05.339691 terrapyn-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     1958 2024-03-15 16:38:05.339691 terrapyn-0.1.1/README.md
--rw-r--r--   0        0        0     1140 2024-03-15 16:38:16.971670 terrapyn-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      266 2024-03-15 16:38:05.339691 terrapyn-0.1.1/terrapyn/__init__.py
--rw-r--r--   0        0        0    24009 2024-03-15 16:38:05.339691 terrapyn-0.1.1/terrapyn/conversion.py
--rw-r--r--   0        0        0     2842 2024-03-15 16:38:05.339691 terrapyn-0.1.1/terrapyn/dask_utils.py
--rw-r--r--   0        0        0       37 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/indices/__init__.py
--rw-r--r--   0        0        0    15286 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/indices/spi.py
--rw-r--r--   0        0        0       53 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/params/__init__.py
--rw-r--r--   0        0        0     9594 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/params/etp.py
--rw-r--r--   0        0        0    23658 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/params/solar.py
--rw-r--r--   0        0        0        0 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/py.typed
--rw-r--r--   0        0        0    26042 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/space.py
--rw-r--r--   0        0        0      217 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/stats/__init__.py
--rw-r--r--   0        0        0     4238 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/stats/_binning.py
--rw-r--r--   0        0        0     6146 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/stats/_ranking.py
--rw-r--r--   0        0        0     4887 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/stats/_stats.py
--rw-r--r--   0        0        0    43841 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/time.py
--rw-r--r--   0        0        0     6748 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/utils.py
--rw-r--r--   0        0        0     3387 2024-03-15 16:38:05.343691 terrapyn-0.1.1/terrapyn/validation.py
--rw-r--r--   0        0        0     3004 1970-01-01 00:00:00.000000 terrapyn-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      126 2024-04-18 23:47:03.828582 terrapyn-0.1.2/AUTHORS.md
+-rw-r--r--   0        0        0     1468 2024-04-18 23:47:03.828582 terrapyn-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     1958 2024-04-18 23:47:03.828582 terrapyn-0.1.2/README.md
+-rw-r--r--   0        0        0     1197 2024-04-18 23:47:16.000667 terrapyn-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      522 2024-04-18 23:47:03.828582 terrapyn-0.1.2/terrapyn/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-18 23:47:03.828582 terrapyn-0.1.2/terrapyn/bq/__init__.py
+-rw-r--r--   0        0        0    12530 2024-04-18 23:47:03.828582 terrapyn-0.1.2/terrapyn/bq/data.py
+-rw-r--r--   0        0        0    24009 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/conversion.py
+-rw-r--r--   0        0        0     2842 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/dask_utils.py
+-rw-r--r--   0        0        0       81 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/ee/__init__.py
+-rw-r--r--   0        0        0     8800 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/ee/data.py
+-rw-r--r--   0        0        0     1484 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/ee/io.py
+-rw-r--r--   0        0        0     8188 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/ee/stats.py
+-rw-r--r--   0        0        0     5230 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/ee/utils.py
+-rw-r--r--   0        0        0       99 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/indices/__init__.py
+-rw-r--r--   0        0        0     1066 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/indices/_agro.py
+-rw-r--r--   0        0        0    15286 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/indices/spi.py
+-rw-r--r--   0        0        0     3982 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/io.py
+-rw-r--r--   0        0        0      155 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/logger.py
+-rw-r--r--   0        0        0       67 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/params/__init__.py
+-rw-r--r--   0        0        0     9594 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/params/etp.py
+-rw-r--r--   0        0        0     3920 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/params/soil.py
+-rw-r--r--   0        0        0    23658 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/params/solar.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/py.typed
+-rw-r--r--   0        0        0    26042 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/space.py
+-rw-r--r--   0        0        0    22088 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/stats.py
+-rw-r--r--   0        0        0    47655 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/time.py
+-rw-r--r--   0        0        0     7736 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/utils.py
+-rw-r--r--   0        0        0     3387 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/validation.py
+-rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 terrapyn-0.1.2/PKG-INFO
```

### Comparing `terrapyn-0.1.1/LICENSE.md` & `terrapyn-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.1/README.md` & `terrapyn-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.1/pyproject.toml` & `terrapyn-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 [tool.poetry]
 name = "terrapyn"
-version = "0.1.1"
+version = "0.1.2"
 description="Toolkit to manipulate Earth observations and models."
 authors = ["colinahill <colinalastairhill@gmail.com>"]
 readme = "README.md"
 license="BSD-3-Clause"
 packages = [{include = "terrapyn"}]
 
 [tool.poetry.dependencies]
-python = ">=3.11,<3.12"
+python = ">=3.10,<3.12"
 xarray = "^2024"
-pandas = "^2.0.0"
-geopandas = "^0.14"
-numpy = "^1.26.0"
-scipy = "^1.12.0"
+pandas = "^2"
+geopandas = "*"
+numpy = "*"
+scipy = "*"
 dask = "^2024"
-matplotlib = "^3.8.0"
-bottleneck = "^1.3.0"
-shapely = "^2.0.0"
-netcdf4 = "^1.6.0"
-ipykernel = "^6.29.0"
+matplotlib = "^3"
+bottleneck = "^1"
+shapely = "^2"
+netcdf4 = "*"
+ipykernel = "^6"
 pyarrow = "^15"
-fiona = "^1.9.0"
-tqdm = "^4.66.0"
+fiona = "*"
+tqdm = "*"
 jupyterlab = "^4.1"
-rioxarray = "^0.15"
+rioxarray = "*"
+earthengine-api = "^0.1"
+polygon-geohasher = "*"
+geemap = "*"
+google-cloud-bigquery = "^3.20.1"
+db-dtypes = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 pytest-cov = "^4.0"
-isort = "^5.12"
+isort = "^5"
 black = "^23.3"
 pre-commit = "^3.2"
 freezegun = "^1.2"
 nbstripout = "^0.6"
 coverage-badge = "^1.1"
 ruff = "^0.3"
```

### Comparing `terrapyn-0.1.1/terrapyn/conversion.py` & `terrapyn-0.1.2/terrapyn/conversion.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.1/terrapyn/dask_utils.py` & `terrapyn-0.1.2/terrapyn/dask_utils.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.1/terrapyn/indices/spi.py` & `terrapyn-0.1.2/terrapyn/indices/spi.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.1/terrapyn/params/etp.py` & `terrapyn-0.1.2/terrapyn/params/etp.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.1/terrapyn/params/solar.py` & `terrapyn-0.1.2/terrapyn/params/solar.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.1/terrapyn/space.py` & `terrapyn-0.1.2/terrapyn/space.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.1/terrapyn/time.py` & `terrapyn-0.1.2/terrapyn/time.py`

 * *Files 9% similar despite different names*

```diff
@@ -834,15 +834,15 @@
     time_dim: str = "time",
     freq: str = "D",
     closed: str = "left",
     day_start_hour: int = 0,
     other_grouping_columns: list = None,
 ):
     """
-    Resample data in time.
+    Group data by time.
 
     Args:
         data: Data to resample in time
         time_dim: Name of the time dimension/index/column in `data` that will be used to determine the grouping.
         freq: Resample frequency. Follows Pandas notation here
         https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#dateoffset-objects
         day_start_hour: The hour that is used as the start of the day (so 1 complete day is from
@@ -988,14 +988,102 @@
         rolling_data = data.rolling({time_dim: n_periods}, min_periods=n_periods)
     else:
         raise TypeError("data must be of type pd.Series or xr.DataArray")
 
     return tp.utils._call_resample_method(rolling_data, method, dim=time_dim)
 
 
+def disaggregate_to_daily(
+    data: pd.DataFrame = None,
+    time_dim: str = "time",
+    n_days_in_period: int = 8,
+    agg_type: str = "sum",
+    normalize_year_end: bool = True,
+) -> pd.DataFrame:
+    """
+    Dissaggregate data with multi-day period (e.g. 8-day, 16-day) to daily values.
+
+    If `agg_type=='sum'` then the values are divided by the number of days in each period, to give
+    the mean daily value. If `agg_type=='mean'` then the values are duplicated for each day in the period.
+
+    Optionally takes care of incomplete periods at the end of a calendar year and normalizes data using
+    however many days are in that incomplete period. e.g. for 8-day periods where the 'date' is the start
+    of the 8 day period, the last period of each year covers 5 or 6 days. For daily values, the data are
+    normalized by 8 days apart from the last periods in the year which are normalized by 5 or 6 days.
+
+    Args:
+        data: Input data
+        n_days_in_period: Number of days in period
+        agg_type: Type of aggregation used in creating the input data. Options are 'sum', 'mean'.
+        This determines how the values are normalized (divided or duplicated).
+        normalize_year_end: If True, normalize the last period of each year by the number of days in the period
+
+    Returns:
+        pd.DataFrame with index of 'date' and values resampled to daily values
+    """
+    # Extract/Convert the `time_dim` to a pandas.DatetimeIndex
+    times = get_time_from_data(data, time_dim=time_dim)
+
+    # Daily date range from period start date to period end date + n_days_in_period
+    # unless end date is in last period of year, then end of year
+    start = times[0]
+    end = times[-1]
+    if (end.month == 12) & (31 - end.day < n_days_in_period):
+        end = pd.Timestamp(year=end.year, month=12, day=31)
+        fill_until_year_end = True
+    else:
+        end = end + pd.Timedelta(n_days_in_period - 1, unit="D")
+        fill_until_year_end = False
+
+    daily = pd.date_range(start, end, freq="D")
+
+    orig_daily = data.reindex(index=daily, method="ffill").copy()
+
+    if agg_type == "sum":
+        if normalize_year_end:
+            # Divide all values by n_days_in_period apart from last period in year
+            # unless fill_until_year_end == False, then just divide last day by n_days_in_period
+            factor = pd.Series(data=n_days_in_period, index=times)
+
+            if fill_until_year_end:
+                # how many days until end of year for each of these dates
+                end_of_year_dates = factor.index[
+                    (factor.index.month == 12) & (31 - factor.index.day < n_days_in_period)
+                ]
+                end_of_year_factors = [
+                    (366 - date.day_of_year + 1) if date.is_leap_year else (365 - date.day_of_year + 1)
+                    for date in end_of_year_dates
+                ]
+                factor[end_of_year_dates] = end_of_year_factors
+
+            factor_daily = factor.reindex(index=daily, method="ffill")
+            orig_daily = orig_daily.div(factor_daily, axis=0)
+        else:
+            # divide all by n_days_in_period
+            orig_daily = orig_daily.div(n_days_in_period)
+
+    return orig_daily
+
+
+def test_disaggregate_to_daily():
+    """
+    Test disaggregate_to_daily
+    """
+    # Create a dataframe with 8-day period data
+    dates = pd.date_range("2022-01-01", freq="8D", periods=2, name="time")
+    data = pd.DataFrame({"data": np.full(len(dates), 8)}, index=dates)
+
+    disaggregated = disaggregate_to_daily(data, n_days_in_period=8, agg_type="sum", normalize_year_end=True)
+
+    daily_dates = pd.date_range("2022-01-01", freq="D", periods=16, name="time")
+    expected = pd.Series(index=daily_dates, data=np.full(len(daily_dates), 1.0))
+
+    assert disaggregated["data"].equals(expected)
+
+
 ################################################
 
 # Dictionary to define the relative order of pandas time frequencies, where a lower value is higher frequency.
 # FREQUENCY_DICT = {
 #     "N": 0,
 #     "U": 1,
 #     "us": 1,
```

### Comparing `terrapyn-0.1.1/terrapyn/utils.py` & `terrapyn-0.1.2/terrapyn/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,22 @@
     Example:
         >>> split_into_chunks(np.arange(10), 3)
         [array([0, 1, 2]), array([3, 4, 5]), array([6, 7, 8]), array([9])]
     """
     return np.split(a, range(n, len(a), n), axis=axis)
 
 
+def split_number_into_parts(a: int = None, b: int = None):
+    """
+    Split an integer `a` into a list of `b` integer parts, where
+    the values are as equal as possible while remaining whole numbers.
+    """
+    return [a // b + 1] * (a % b) + [a // b] * (b - a % b)
+
+
 def set_dim_values_in_data(
     data: T.Union[
         xr.Dataset,
         xr.DataArray,
         pd.DataFrame,
         pd.Series,
     ] = None,
@@ -162,16 +170,20 @@
             return dim in index.names
     else:
         if index.name is not None:
             return dim in index.name
 
 
 def ensure_list(a: T.Any = None) -> T.List[T.Any]:
-    """Ensure data `a` is a list and cast if required"""
-    if isinstance(a, list):
+    """
+    Ensure data `a` is a list if not None
+    """
+    if a is None:
+        return None
+    elif isinstance(a, list):
         return a
     elif isinstance(a, (str, int, float)):
         return [a]
     else:
         return list(a)
 
 
@@ -196,7 +208,27 @@
         # convert all single values to a list
         remove_list = ensure_list(remove_list)
 
         return [e for e in input_list if e not in set(remove_list)]
 
     else:
         raise ValueError("both `input_list` and `remove_list` must be provided")
+
+
+def get_key_for_value_in_dict(dictionary: dict, value):
+    """Get the key for a value in a dictionary"""
+    return list(dictionary.keys())[list(dictionary.values()).index(value)]
+
+
+def get_first_dictionary_value(dictionary: dict):
+    """Get the first value in a dictionary"""
+    return next(iter(dictionary.values()))
+
+
+def get_indexes_of_items_in_list(input_list: T.List = None, items: T.List = None) -> T.List[int]:
+    """Get the (first) index of each item in `items` in the list `input_list`"""
+    return [input_list.index(item) for item in items]
+
+
+def utf8_len(s: str) -> int:
+    """Calculate the size of a string in bytes."""
+    return len(s.encode("utf-8"))
```

### Comparing `terrapyn-0.1.1/terrapyn/validation.py` & `terrapyn-0.1.2/terrapyn/validation.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.1/PKG-INFO` & `terrapyn-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: terrapyn
-Version: 0.1.1
+Version: 0.1.2
 Summary: Toolkit to manipulate Earth observations and models.
 License: BSD-3-Clause
 Author: colinahill
 Author-email: colinalastairhill@gmail.com
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bottleneck (>=1.3.0,<2.0.0)
+Requires-Dist: bottleneck (>=1,<2)
 Requires-Dist: dask (>=2024,<2025)
-Requires-Dist: fiona (>=1.9.0,<2.0.0)
-Requires-Dist: geopandas (>=0.14,<0.15)
-Requires-Dist: ipykernel (>=6.29.0,<7.0.0)
+Requires-Dist: db-dtypes (>=1.2.0,<2.0.0)
+Requires-Dist: earthengine-api (>=0.1,<0.2)
+Requires-Dist: fiona
+Requires-Dist: geemap
+Requires-Dist: geopandas
+Requires-Dist: google-cloud-bigquery (>=3.20.1,<4.0.0)
+Requires-Dist: ipykernel (>=6,<7)
 Requires-Dist: jupyterlab (>=4.1,<5.0)
-Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
-Requires-Dist: netcdf4 (>=1.6.0,<2.0.0)
-Requires-Dist: numpy (>=1.26.0,<2.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: matplotlib (>=3,<4)
+Requires-Dist: netcdf4
+Requires-Dist: numpy
+Requires-Dist: pandas (>=2,<3)
+Requires-Dist: polygon-geohasher
 Requires-Dist: pyarrow (>=15,<16)
-Requires-Dist: rioxarray (>=0.15,<0.16)
-Requires-Dist: scipy (>=1.12.0,<2.0.0)
-Requires-Dist: shapely (>=2.0.0,<3.0.0)
-Requires-Dist: tqdm (>=4.66.0,<5.0.0)
+Requires-Dist: rioxarray
+Requires-Dist: scipy
+Requires-Dist: shapely (>=2,<3)
+Requires-Dist: tqdm
 Requires-Dist: xarray (>=2024,<2025)
 Description-Content-Type: text/markdown
 
 # terrapyn
 
 ![Code Coverage](https://img.shields.io/badge/Coverage-83%25-yellowgreen.svg)
 [![PyPI version](https://badge.fury.io/py/terrapyn.svg)](https://badge.fury.io/py/terrapyn)
```

