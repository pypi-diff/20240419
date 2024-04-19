# Comparing `tmp/pyam_iamc-2.2.1.tar.gz` & `tmp/pyam_iamc-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyam_iamc-2.2.1.tar", max compression
+gzip compressed data, was "pyam_iamc-2.2.2.tar", max compression
```

## Comparing `pyam_iamc-2.2.1.tar` & `pyam_iamc-2.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1591 2024-04-17 10:12:28.770833 pyam_iamc-2.2.1/AUTHORS.rst
--rw-r--r--   0        0        0    10141 2024-04-17 10:12:28.770833 pyam_iamc-2.2.1/LICENSE
--rw-r--r--   0        0        0      605 2024-04-17 10:12:28.770833 pyam_iamc-2.2.1/NOTICE.md
--rw-r--r--   0        0        0     7626 2024-04-17 10:12:28.770833 pyam_iamc-2.2.1/README.md
--rw-r--r--   0        0        0      892 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/__init__.py
--rw-r--r--   0        0        0      622 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/_compare.py
--rw-r--r--   0        0        0      423 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/_debiasing.py
--rw-r--r--   0        0        0     6959 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/_ops.py
--rw-r--r--   0        0        0     3630 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/_style.py
--rw-r--r--   0        0        0     9863 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/aggregation.py
--rw-r--r--   0        0        0     9929 2024-04-17 10:12:28.790833 pyam_iamc-2.2.1/pyam/compute.py
--rwxr-xr-x   0        0        0   108859 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/core.py
--rwxr-xr-x   0        0        0     2572 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/figures.py
--rw-r--r--   0        0        0     3922 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/filter.py
--rw-r--r--   0        0        0    26714 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/iiasa.py
--rw-r--r--   0        0        0     4070 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/index.py
--rw-r--r--   0        0        0     4206 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/ixmp4.py
--rw-r--r--   0        0        0      466 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/logging.conf
--rw-r--r--   0        0        0     1391 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/logging.py
--rw-r--r--   0        0        0    40912 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/plotting.py
--rw-r--r--   0        0        0     4022 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/run_control.py
--rw-r--r--   0        0        0     2557 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/slice.py
--rw-r--r--   0        0        0    12102 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/statistics.py
--rw-r--r--   0        0        0     4448 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/str.py
--rw-r--r--   0        0        0     1050 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/testing.py
--rw-r--r--   0        0        0     2820 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/time.py
--rw-r--r--   0        0        0     5643 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/timeseries.py
--rw-r--r--   0        0        0     5261 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/unfccc.py
--rw-r--r--   0        0        0     4711 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/units.py
--rw-r--r--   0        0        0    21224 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/utils.py
--rw-r--r--   0        0        0     4592 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/validation.py
--rw-r--r--   0        0        0     2322 2024-04-17 10:12:28.794833 pyam_iamc-2.2.1/pyam/worldbank.py
--rw-r--r--   0        0        0     4426 2024-04-17 10:12:49.390940 pyam_iamc-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     9029 1970-01-01 00:00:00.000000 pyam_iamc-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1591 2024-04-19 12:03:49.267993 pyam_iamc-2.2.2/AUTHORS.rst
+-rw-r--r--   0        0        0    10141 2024-04-19 12:03:49.267993 pyam_iamc-2.2.2/LICENSE
+-rw-r--r--   0        0        0      605 2024-04-19 12:03:49.267993 pyam_iamc-2.2.2/NOTICE.md
+-rw-r--r--   0        0        0     7626 2024-04-19 12:03:49.267993 pyam_iamc-2.2.2/README.md
+-rw-r--r--   0        0        0      892 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/__init__.py
+-rw-r--r--   0        0        0      622 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/_compare.py
+-rw-r--r--   0        0        0      423 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/_debiasing.py
+-rw-r--r--   0        0        0     6951 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/_ops.py
+-rw-r--r--   0        0        0     3621 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/_style.py
+-rw-r--r--   0        0        0     9853 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/aggregation.py
+-rw-r--r--   0        0        0     9929 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/compute.py
+-rwxr-xr-x   0        0        0   108827 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/core.py
+-rwxr-xr-x   0        0        0     2538 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/figures.py
+-rw-r--r--   0        0        0     3922 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/filter.py
+-rw-r--r--   0        0        0    26677 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/iiasa.py
+-rw-r--r--   0        0        0     4070 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/index.py
+-rw-r--r--   0        0        0     4206 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/ixmp4.py
+-rw-r--r--   0        0        0      478 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/logging.json
+-rw-r--r--   0        0        0     1451 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/logging.py
+-rw-r--r--   0        0        0    40859 2024-04-19 12:03:49.287993 pyam_iamc-2.2.2/pyam/plotting.py
+-rw-r--r--   0        0        0     4014 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/run_control.py
+-rw-r--r--   0        0        0     2557 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/slice.py
+-rw-r--r--   0        0        0    11979 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/statistics.py
+-rw-r--r--   0        0        0     4364 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/str.py
+-rw-r--r--   0        0        0     1050 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/testing.py
+-rw-r--r--   0        0        0     2820 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/time.py
+-rw-r--r--   0        0        0     5638 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/timeseries.py
+-rw-r--r--   0        0        0     5255 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/unfccc.py
+-rw-r--r--   0        0        0     4711 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/units.py
+-rw-r--r--   0        0        0    21214 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/utils.py
+-rw-r--r--   0        0        0     4579 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/validation.py
+-rw-r--r--   0        0        0     2322 2024-04-19 12:03:49.291993 pyam_iamc-2.2.2/pyam/worldbank.py
+-rw-r--r--   0        0        0     4409 2024-04-19 12:04:05.368029 pyam_iamc-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8999 1970-01-01 00:00:00.000000 pyam_iamc-2.2.2/PKG-INFO
```

### Comparing `pyam_iamc-2.2.1/AUTHORS.rst` & `pyam_iamc-2.2.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/LICENSE` & `pyam_iamc-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/NOTICE.md` & `pyam_iamc-2.2.2/NOTICE.md`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/README.md` & `pyam_iamc-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyam/__init__.py` & `pyam_iamc-2.2.2/pyam/__init__.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyam/_compare.py` & `pyam_iamc-2.2.2/pyam/_compare.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyam/_ops.py` & `pyam_iamc-2.2.2/pyam/_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     if not isinstance(result, pd.Series):
         msg = f"Value returned by `{method.__name__}` cannot be cast to an IamDataFrame"
         raise ValueError(f"{msg}: {result}")
 
     # separate pint quantities into numerical value and unit (as index)
     if ignore_units is False:
         _value = pd.DataFrame(
-            [[i.magnitude, "{:~}".format(i.units)] for i in result.values],
+            [[i.magnitude, f"{i.units:~}"] for i in result.values],
             columns=["value", "unit"],
             index=result.index,
         ).set_index("unit", append=True)
         _value.index = replace_index_values(_value, "unit", {"dimensionless": ""})
 
     # otherwise, set unit (as index) to "unknown" or the value given by "ignore_units"
     else:
```

### Comparing `pyam_iamc-2.2.1/pyam/_style.py` & `pyam_iamc-2.2.2/pyam/_style.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     import matplotlib.pyplot as plt
 
     if color is None and colormap is not None:
         if isinstance(colormap, str):
             cmap = colormap
             colormap = cm.get_cmap(colormap)
             if colormap is None:
-                raise ValueError("Colormap {0} is not recognized".format(cmap))
+                raise ValueError(f"Colormap {cmap} is not recognized")
         colors = [colormap(num) for num in np.linspace(0, 1, num=num_colors)]
     elif color is not None:
         if colormap is not None:
             warnings.warn(
                 "'color' and 'colormap' cannot be used "
                 + "simultaneously. Using 'color'"
             )
```

### Comparing `pyam_iamc-2.2.1/pyam/aggregation.py` & `pyam_iamc-2.2.2/pyam/aggregation.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     # keep variable at highest level if it exists
     _df = df.filter(variable=[variable, f"{variable}|*"])
     data_list = []
 
     # iterate over variables (bottom-up) and aggregate all components up to `variable`
     for d in reversed(range(find_depth(variable), max(find_depth(_df.variable)))):
         components = compress(_df.variable, find_depth(_df.variable, level=d + 1))
-        var_list = set([reduce_hierarchy(v, -1) for v in components])
+        var_list = {reduce_hierarchy(v, -1) for v in components}
 
         # a temporary dataframe allows to distinguish between full data and new data
         _data_agg = _aggregate(_df, variable=var_list)
 
         # check if data for intermediate variables already exists
         with adjust_log_level("pyam.core"):
             _data_self = _df.filter(variable=var_list)._data
@@ -171,15 +171,15 @@
     return _data.dropna()
 
 
 def _aggregate_time(df, variable, column, value, components, method="sum"):
     """Internal implementation for aggregating data over subannual time"""
     # default `components` to all entries in `column` other than `value`
     if components is None:
-        components = list(set(df.data.subannual.unique()) - set([value]))
+        components = list(set(df.data.subannual.unique()) - {value})
 
     # compute aggregate over time
     filter_args = dict(variable=variable)
     filter_args[column] = components
     index = [d for d in df.dimensions if d != column]
 
     _data = pd.concat(
```

### Comparing `pyam_iamc-2.2.1/pyam/compute.py` & `pyam_iamc-2.2.2/pyam/compute.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyam/core.py` & `pyam_iamc-2.2.2/pyam/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     write_sheet,
 )
 from pyam.validation import _exclude_on_fail, _validate
 
 logger = logging.getLogger(__name__)
 
 
-class IamDataFrame(object):
+class IamDataFrame:
     """Scenario timeseries data and meta indicators
 
     The class provides a number of diagnostic features (including validation of
     data, completeness of variables provided), processing tools (e.g.,
     unit conversion), as well as visualization and plotting tools.
 
     Parameters
@@ -302,16 +302,16 @@
 
         if len(self.meta.columns):
             info += "\nMeta indicators:\n"
             info += "\n".join(
                 [
                     print_meta_row(m, t, self.meta[m].unique())
                     for m, t in zip(
-                    self.meta.columns[0:meta_rows], self.meta.dtypes[0:meta_rows]
-                )
+                        self.meta.columns[0:meta_rows], self.meta.dtypes[0:meta_rows]
+                    )
                 ]
             )
             # print `...` if more than `meta_rows` columns
             if len(self.meta.columns) > meta_rows:
                 info += "\n   ..."
 
         # add info on size (optional)
@@ -1777,15 +1777,15 @@
     def _variable_components(self, variable, level=0):
         """Get all components (sub-categories) of a variable for a given level
 
         If `level=0`, for `variable='foo'`, return `['foo|bar']`, but don't
         include `'foo|bar|baz'`, which is a sub-sub-category. If `level=None`,
         all variables below `variable` in the hierarchy are returned."""
         var_list = pd.Series(self.variable)
-        return var_list[pattern_match(var_list, "{}|*".format(variable), level=level)]
+        return var_list[pattern_match(var_list, f"{variable}|*", level=level)]
 
     def _get_cols(self, cols):
         """Return a list of columns of `self.data`"""
         return META_IDX + cols + self.extra_cols
 
     def check_internal_consistency(self, components=False, **kwargs):
         """Check whether a scenario ensemble is internally consistent.
@@ -2441,15 +2441,15 @@
             excel_writer = pd.ExcelWriter(excel_writer, **kwargs)
 
         # write data table
         write_sheet(excel_writer, sheet_name, self._to_file_format(iamc_index))
 
         # write meta table unless `include_meta=False`
         if include_meta and len(self.meta.columns):
-            meta_rename = dict([(i, i.capitalize()) for i in self.index.names])
+            meta_rename = {i: i.capitalize() for i in self.index.names}
             write_sheet(
                 excel_writer,
                 "meta" if include_meta is True else include_meta,
                 self.meta.reset_index().rename(columns=meta_rename),
             )
 
         # close the file if `excel_writer` arg was a file name
@@ -2497,15 +2497,15 @@
         with TemporaryDirectory(dir=".") as tmp:
             # save data and meta tables to a temporary folder
             self.data.to_csv(Path(tmp) / "data.csv", index=False)
             self.meta.to_csv(Path(tmp) / "meta.csv")
 
             # cast tables to datapackage
             package = Package()
-            package.infer("{}/*.csv".format(tmp))
+            package.infer(f"{tmp}/*.csv")
             if not package.valid:
                 logger.warning("The exported datapackage is not valid")
             package.save(path)
 
         # return the package (needs to reloaded because `tmp` was deleted)
         return Package(path)
 
@@ -2526,15 +2526,15 @@
         """
 
         # load from file
         path = path if isinstance(path, pd.ExcelFile) else Path(path)
         meta = read_pandas(path, sheet_name=sheet_name, **kwargs)
 
         # cast index-column headers to lower-case, check that required index exists
-        meta = meta.rename(columns=dict([(i.capitalize(), i) for i in META_IDX]))
+        meta = meta.rename(columns={i.capitalize(): i for i in META_IDX})
         if missing_cols := [c for c in self.index.names if c not in meta.columns]:
             raise ValueError(
                 f"Missing index columns for meta indicators: {missing_cols}"
             )
 
         # skip import of meta indicators if no rows in meta
         if not len(meta.index):
```

### Comparing `pyam_iamc-2.2.1/pyam/figures.py` & `pyam_iamc-2.2.2/pyam/figures.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,20 +47,18 @@
         if len(levels) > 1:
             raise ValueError(f"Non-unique values in column {col}: {levels}")
 
     # Concatenate the data with source and target columns
     _df = pd.DataFrame.from_dict(
         mapping, orient="index", columns=["source", "target"]
     ).merge(df._data, how="left", left_index=True, right_on="variable")
-    label_mapping = dict(
-        [
-            (label, i)
-            for i, label in enumerate(set(pd.concat([_df["source"], _df["target"]])))
-        ]
-    )
+    label_mapping = {
+        label: i
+        for i, label in enumerate(set(pd.concat([_df["source"], _df["target"]])))
+    }
     _df.replace(label_mapping, inplace=True)
     region = get_index_levels(_df, "region")[0]
     unit = get_index_levels(_df, "unit")[0]
     year = get_index_levels(_df, "year")[0]
     fig = go.Figure(
         data=[
             go.Sankey(
```

### Comparing `pyam_iamc-2.2.1/pyam/filter.py` & `pyam_iamc-2.2.2/pyam/filter.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyam/iiasa.py` & `pyam_iamc-2.2.2/pyam/iiasa.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 def set_config(*args, **kwargs):
     raise DeprecationWarning(f"This method is deprecated. {IXMP4_LOGIN}.")
 
 
 def _read_config(file):
     """Read username and password for IIASA API connection from file"""
-    with open(file, "r") as stream:
+    with open(file) as stream:
         creds = yaml.safe_load(stream)
 
     return ManagerAuth(**creds, url=str(settings.manager_url))
 
 
 def _check_response(r, msg="Error connecting to IIASA database", error=RuntimeError):
     if not r.ok:
@@ -135,15 +135,15 @@
             else:
                 self.auth.refresh_or_reobtain_jwt()
                 self.access_token = self.auth.access_token
 
         return {"Authorization": "Bearer " + self.access_token}
 
 
-class Connection(object):
+class Connection:
     """A class to facilitate querying an IIASA Scenario Explorer database API
 
     Parameters
     ----------
     name : str, optional
         The name of a database API.
         Use :attr:`valid_connections <pyam.iiasa.Connection.valid_connections>`
@@ -173,15 +173,15 @@
 
         if self.auth.user is not None:
             logger.info(f"You are connected as user `{self.auth.user}`")
         else:
             logger.info("You are connected as an anonymous user")
 
     @property
-    @lru_cache()
+    @lru_cache
     def _connection_map(self):
         # TODO: application-list will be reimplemented in conjunction with ixmp-server
         r = self.auth.client.get("legacy/applications", headers=self.auth())
         if r.status_code >= 400:
             raise ValueError("Unknown API error: " + r.text)
 
         aliases = set()
@@ -190,27 +190,27 @@
             if "config" in x:
                 env = next(
                     (r["value"] for r in x["config"] if r["path"] == "env"), None
                 )
                 name = x["name"]
                 if env is not None:
                     if env in aliases:
-                        logger.warning("Duplicate instance alias {}".format(env))
+                        logger.warning(f"Duplicate instance alias {env}")
                         conn_map[name] = name
                         first_duplicate = conn_map.pop(env)
                         conn_map[first_duplicate] = first_duplicate
                     else:
                         conn_map[env] = name
                     aliases.add(env)
                 else:
                     conn_map[name] = name
         return conn_map
 
     @property
-    @lru_cache()
+    @lru_cache
     def valid_connections(self):
         """Return available resources (database API connections)"""
         logger.warning(
             "IIASA is migrating to a database infrastructure using the ixmp4 package."
             "Use `pyam.iiasa.platforms()` to list available ixmp4 databases."
         )
         return list(self._connection_map.keys())
@@ -354,36 +354,36 @@
             default_only = _new_default_api(kwargs)
 
         audit_cols = ["cre_user", "cre_date", "upd_user", "upd_date"]
         other_cols = ["version"] if default_only else ["version", "is_default"]
         cols = audit_cols + other_cols
 
         _df = self._query_index(default_only, meta=True, cols=cols, **kwargs)
-        audit_mapping = dict([(i, i.replace("_", "ate_")) for i in audit_cols])
+        audit_mapping = {i: i.replace("_", "ate_") for i in audit_cols}
 
         return _df.set_index(META_IDX).rename(columns=audit_mapping)
 
     def models(self):
         """List all models in the connected resource"""
         return pd.Series(self._query_index()["model"].unique(), name="model")
 
     def scenarios(self):
         """List all scenarios in the connected resource"""
         return pd.Series(self._query_index()["scenario"].unique(), name="scenario")
 
-    @lru_cache()
+    @lru_cache
     def variables(self):
         """List all variables in the connected resource"""
         url = "/".join([self._base_url, "ts"])
         r = requests.get(url, headers=self.auth())
         _check_response(r)
         df = pd.read_json(StringIO(r.text), orient="records")
         return pd.Series(df["variable"].unique(), name="variable")
 
-    @lru_cache()
+    @lru_cache
     def regions(self, include_synonyms=False):
         """List all regions in the connected resource
 
         Parameters
         ----------
         include_synonyms : bool
             whether to include synonyms
```

### Comparing `pyam_iamc-2.2.1/pyam/index.py` & `pyam_iamc-2.2.2/pyam/index.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyam/ixmp4.py` & `pyam_iamc-2.2.2/pyam/ixmp4.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyam/logging.py` & `pyam_iamc-2.2.2/pyam/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import json
 import warnings
 from contextlib import contextmanager
 from logging import config, getLogger
 from pathlib import Path
 
 import pandas as pd
 
 here = Path(__file__).parent
 logger = getLogger(__name__)
 
 
 def configure_logging():
     """Configure logging"""
-    config.fileConfig(here / "logging.conf", disable_existing_loggers=False)
+    logging_config = here / "logging.json"
+    with open(logging_config) as file:
+        config.dictConfig(json.load(file))
 
 
 @contextmanager
 def adjust_log_level(logger="pyam", level="ERROR"):
     """Context manager to change log level"""
     if isinstance(logger, str):
         logger = getLogger(logger)
```

### Comparing `pyam_iamc-2.2.1/pyam/plotting.py` & `pyam_iamc-2.2.2/pyam/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
     """
 
     # cast to DataFrame if necessary
     # TODO: select only relevant meta columns
     if not isinstance(df, pd.DataFrame):
         df = df.as_pandas()
 
-    for col in set(SORT_IDX) - set([category]):
+    for col in set(SORT_IDX) - {category}:
         if len(df[col].unique()) > 1:
             msg = (
                 "Can not plot multiple {}s in a pie plot with value={} and category={}"
             )
             raise ValueError(msg.format(col, value, category))
 
     if ax is None:
@@ -432,15 +432,15 @@
     x = x or time_col_or_year(df)
 
     # cast to DataFrame if necessary
     # TODO: select only relevant meta columns
     if not isinstance(df, pd.DataFrame):
         df = df.as_pandas()
 
-    for col in set(SORT_IDX) - set([x, stack]):
+    for col in set(SORT_IDX) - {x, stack}:
         if len(df[col].unique()) > 1:
             msg = "Can not plot multiple {}s in stack_plot with x={}, stack={}"
             raise ValueError(msg.format(col, x, stack))
 
     if ax is None:
         fig, ax = plt.subplots()
 
@@ -535,15 +535,15 @@
         ax.set_ylabel(units[0])
 
     # build a default title if possible
     _title = []
     for var in ["model", "scenario", "region", "variable"]:
         values = df[var].unique()
         if len(values) == 1:
-            _title.append("{}: {}".format(var, values[0]))
+            _title.append(f"{var}: {values[0]}")
     if title and _title:
         title = " ".join(_title) if title is True else title
         ax.set_title(title)
 
     return ax
 
 
@@ -601,15 +601,15 @@
     x = x or time_col_or_year(df)
 
     # cast to DataFrame if necessary
     # TODO: select only relevant meta columns
     if not isinstance(df, pd.DataFrame):
         df = df.as_pandas()
 
-    for col in set(SORT_IDX) - set([x, bars]):
+    for col in set(SORT_IDX) - {x, bars}:
         if len(df[col].unique()) > 1:
             msg = "Can not plot multiple {}s in bar plot with x={}, bars={}"
             raise ValueError(msg.format(col, x, bars))
 
     if ax is None:
         fig, ax = plt.subplots()
 
@@ -654,15 +654,15 @@
             ax.set_xlabel(units[0])
 
     # build a default title if possible
     _title = []
     for var in ["model", "scenario", "region", "variable"]:
         values = df[var].unique()
         if len(values) == 1:
-            _title.append("{}: {}".format(var, values[0]))
+            _title.append(f"{var}: {values[0]}")
     if title and _title:
         title = " ".join(_title) if title is True else title
         ax.set_title(title)
 
     return ax
 
 
@@ -1004,17 +1004,17 @@
     if not isinstance(df, pd.DataFrame):
         meta_col_args = dict(color=color, marker=marker, linestyle=linestyle)
         df = df.as_pandas(meta_cols=mpl_args_to_meta_cols(df, **meta_col_args))
 
     # pivot data if asked for explicit variable name
     variables = df["variable"].unique()
     if x in variables or y in variables:
-        keep_vars = set([x, y]) & set(variables)
+        keep_vars = {x, y} & set(variables)
         df = df[df["variable"].isin(keep_vars)]
-        idx = list(set(df.columns) - set(["value"]))
+        idx = list(set(df.columns) - {"value"})
         df = (
             df.reset_index()
             .set_index(idx)
             .value.unstack(level="variable")  # df -> series  # keep_vars are columns
             .rename_axis(None, axis=1)  # rm column index name
             .reset_index()
             .set_index(META_IDX)
@@ -1034,15 +1034,15 @@
         raise ValueError("Must use `color` kwarg if using `fill_between`")
     if final_ranges and "color" not in props:
         raise ValueError("Must use `color` kwarg if using `final_ranges`")
 
     # prepare a dict for ordering, reshape data for use in line_plot
     idx_cols = list(df.columns.drop(y))
     if not isinstance(order, dict):
-        order = dict([(i, None) for i in order or idx_cols])
+        order = {i: None for i in order or idx_cols}
     df = reshape_mpl(df, x, y, idx_cols, **order)
 
     # determine the columns that should go into the legend
     idx_cols.remove(x)
     title_cols = []
     y_label = None
     for col in idx_cols:
@@ -1154,15 +1154,15 @@
         # line
         ax.set_xlim(xmin, xpos + first - xmin)
         ax.set_xticks(xticks)
         ax.set_xticklabels(xlabels)
 
     # build unique legend handles and labels
     if legend is not False:
-        handles, labels = [np.array(i) for i in ax.get_legend_handles_labels()]
+        handles, labels = (np.array(i) for i in ax.get_legend_handles_labels())
         if label is not None:  # label given explicitly via kwarg
             _add_legend(ax, handles, labels, legend)
         else:
             _, idx = np.unique(labels, return_index=True)
             idx.sort()
             _add_legend(ax, handles[idx], labels[idx], legend)
```

### Comparing `pyam_iamc-2.2.1/pyam/run_control.py` & `pyam_iamc-2.2.2/pyam/run_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,22 +109,22 @@
             return fname
 
         _fname = os.path.join(os.path.dirname(fyaml), fname)
         if not os.path.exists(_fname):
             msg = (
                 "YAML key '{}' in {}: {} is not a valid relative " + "or absolute path"
             )
-            raise IOError(msg.format(key, fyaml, fname))
+            raise OSError(msg.format(key, fyaml, fname))
         return _fname
 
     def _load_yaml(self, obj):
         if hasattr(obj, "read"):  # it's a file
             obj = obj.read()
         if is_str(obj) and not os.path.exists(obj):
-            raise IOError("File {} does not exist".format(obj))
+            raise OSError(f"File {obj} does not exist")
         if is_str(obj) and os.path.exists(obj):
             fname = obj
             with open(fname) as f:
                 obj = f.read()
         if not isinstance(obj, dict):
             obj = yaml.load(obj, Loader=yaml.FullLoader)
         return obj
```

### Comparing `pyam_iamc-2.2.1/pyam/slice.py` & `pyam_iamc-2.2.2/pyam/slice.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyam/statistics.py` & `pyam_iamc-2.2.2/pyam/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pandas as pd
 
 from pyam import filter_by_meta
 from pyam.str import is_str
 from pyam.utils import META_IDX, is_list_like
 
 
-class Statistics(object):
+class Statistics:
     """This class generates descriptive statistics of timeseries data
 
     Parameters
     ----------
     df : IamDataFrame
         an IamDataFrame from which to retrieve meta indicators for grouping
         or filtering
@@ -42,17 +42,17 @@
             self.col = groupby
             self.groupby = {groupby: None}
         elif isinstance(groupby, dict) and len(groupby) == 1:
             self.col = list(groupby.keys())[0]
             self.groupby = groupby
             self.idx_depth = 2
         elif groupby is not None:
-            raise ValueError("arg `{}` not valid `groupby`".format(groupby))
+            raise ValueError(f"arg `{groupby}` not valid `groupby`")
         if self.col is not None and self.col not in df.meta.columns:
-            raise ValueError("column `{}` not in `df.meta`".format(self.col))
+            raise ValueError(f"column `{self.col}` not in `df.meta`")
 
         # if neither groupby nor filters is given, use filters to describe all
         # and assume that rows are used
         if groupby is None and filters is None:
             self.filters = [("", {})]
             rows = True
         else:
@@ -75,51 +75,49 @@
             else:
                 if not (
                     isinstance(idx, tuple)
                     and len(idx) == 2
                     and is_str(idx[0])
                     or not is_str(idx[1])
                 ):
-                    raise ValueError("`{}` is not a valid index".format(idx))
+                    raise ValueError(f"`{idx}` is not a valid index")
                 self._add_to_index(idx[0], idx[1])
             # check that filters in tuple are valid
             if not isinstance(_filter, dict):
-                raise ValueError("`{}` is not a valid filter".format(_filter))
+                raise ValueError(f"`{_filter}` is not a valid filter")
             elif not (set(_filter) - set(META_IDX)).issubset(df.meta):
                 raise ValueError(
                     "column `{}` not in `df.meta`".format(
                         set(_filter) - set(META_IDX) - set(df.meta)
                     )
                 )
 
         self.stats = None
         self.rows = [] if rows else None
 
         # percentiles for passing to `pandas.describe()`
         self.percentiles = list(percentiles)
         self._describe_cols = (
             ["count", "mean", "std", "min"]
-            + ["{:.0%}".format(i) for i in self.percentiles]
+            + [f"{i:.0%}" for i in self.percentiles]
             + ["max"]
         )
 
     def _add_to_index(self, idx, sub_idx=None):
         # assign index depth if not set
         if self.idx_depth is None:
             self.idx_depth = 1 if sub_idx is None else 2
         # check that index matches depth
         if self.groupby is not None and sub_idx is None:
             msg = "if `groupby` is used, index `{}` must have format `{}`"
             raise ValueError(msg.format(idx, "(idx0, idx1)"))
         if self.idx_depth == 1 and sub_idx is not None:
-            raise ValueError(
-                "index depth set to 1, found `({}, {})`".format(idx, sub_idx)
-            )
+            raise ValueError(f"index depth set to 1, found `({idx}, {sub_idx})`")
         if self.idx_depth == 2 and sub_idx is None:
-            raise ValueError("index depth set to 2, found `({})`".format(idx))
+            raise ValueError(f"index depth set to 2, found `({idx})`")
 
         # append to lists for sorting index
         if idx not in self._idx:
             self._idx.append(idx)
         if self.idx_depth == 2 and sub_idx not in self._sub_idx:
             self._sub_idx.append(sub_idx)
 
@@ -288,15 +286,15 @@
     row = row.sort_index()
     center = "50%" if center == "median" else center
 
     # get maximum of `count` and write to first entry of return series
     count = max(
         [i for i in row.loc[(slice(None), slice(None), "count")] if not np.isnan(i)]
     )
-    ret.loc[("count", "")] = ("{:.0f}".format(count)) if count > 1 else ""
+    ret.loc[("count", "")] = (f"{count:.0f}") if count > 1 else ""
 
     # set upper and lower for the range
     upper, lower = ("max", "min") if fullrange is True else ("75%", "25%")
 
     # format `describe()` columns to string output
     for i in row_index:
         x = row.loc[i]
@@ -304,14 +302,14 @@
         if np.isnan(_count) or _count == 0:
             s = ""
         elif _count > 1:
             s = "{f} ({f}, {f})".format(f=custom_format).format(
                 x[center], x[upper], x[lower]
             )
         elif _count == 1:
-            s = "{f}".format(f=custom_format).format(x["50%"])
+            s = f"{custom_format}".format(x["50%"])
         # add count of this section as `[]` if different from count_max
         if 0 < _count < count:
-            s += " [{:.0f}]".format(_count)
+            s += f" [{_count:.0f}]"
         ret.loc[i] = s
 
     return ret
```

### Comparing `pyam_iamc-2.2.1/pyam/str.py` & `pyam_iamc-2.2.2/pyam/str.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 
 import numpy as np
 import pandas as pd
-import six
 from pandas.api.types import is_list_like
 
+REGEXP_CHARACTERS = r".^$+?()[]{}|"
+
 
 def concat_with_pipe(x, *args, cols=None):
     """Concatenate a list or pandas.Series using ``|``, drop None or numpy.nan"""
     if args:
         # Guard against legacy-errors when adding `*args` (#778)
         # TODO: deprecated, remove for release >= 3.0
         for i in args:
@@ -77,15 +78,15 @@
         level = int(level[:-1])
 
         # test = lambda x: level <= x if x is not None else False
         def test(x):
             return level <= x if x is not None else False
 
     else:
-        raise ValueError("Unknown level type: `{}`".format(level))
+        raise ValueError(f"Unknown level type: `{level}`")
 
     return list(map(test, n_pipes))
 
 
 def get_variable_components(x, level, join=False):
     """Return components for requested level in a list or join these in a str.
 
@@ -120,27 +121,23 @@
         Uses ``|`` to separate the components of the variable.
     depth : int or list of int
         Position of the components.
 
     """
     _x = x.split("|")
     depth = len(_x) + depth - 1 if depth < 0 else depth
-    return "|".join(_x[0 : (depth + 1)])
+    return "|".join(_x[0: (depth + 1)])
 
 
 def escape_regexp(s):
     """Escape characters with specific regexp use"""
-    return (
-        str(s)
-        .replace("|", "\\|")
-        .replace(".", r"\.")  # `.` has to be replaced before `*`
-        .replace("*", ".*")
-        .replace("+", r"\+")
-        .replace("(", r"\(")
-        .replace(")", r"\)")
-        .replace("$", "\\$")
-    )
+    s = str(s)
+    for c in REGEXP_CHARACTERS:
+        s = s.replace(c, "\\" + c)
+    # pyam uses `*` as wildcard, replace with `.*` for regex
+    s = s.replace("*", ".*")
+    return s
 
 
 def is_str(x):
     """Returns True if x is a string"""
-    return isinstance(x, six.string_types)
+    return isinstance(x, str)
```

### Comparing `pyam_iamc-2.2.1/pyam/testing.py` & `pyam_iamc-2.2.2/pyam/testing.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyam/time.py` & `pyam_iamc-2.2.2/pyam/time.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyam/timeseries.py` & `pyam_iamc-2.2.2/pyam/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     direction : str, optional
         Whether to return all years where the threshold is crossed
         or only where threshold is crossed in a specific direction
     return_type : type, optional
         Whether to cast the returned values to integer (years)
     """
     direction = [direction] if is_str(direction) else list(direction)
-    if not set(direction).issubset(set(["from above", "from below"])):
+    if not set(direction).issubset({"from above", "from below"}):
         raise ValueError(f"Invalid direction: {direction}")
 
     # get the values and time-domain index
     x = x.dropna()
     values, index = x.values - threshold, x.index.to_numpy()
     positive, negative = (values >= 0), (values < 0)
```

### Comparing `pyam_iamc-2.2.1/pyam/unfccc.py` & `pyam_iamc-2.2.2/pyam/unfccc.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     return IamDataFrame(data, model=model, scenario=scenario, region="party")
 
 
 def _compile_variable(i, variable):
     """Translate UNFCCC columns into an IAMC-style variable"""
     if i["variable"]:
         raise ValueError("Conflict in variable mapping.")
-    return variable.format(**dict((c, i[c]) for c in NAME_COLS))
+    return variable.format(**{c: i[c] for c in NAME_COLS})
 
 
 def _compile_unit(i):
     """Append gas to unit and update CO2e for pint/iam-unit compatibility"""
     if " equivalent" in i["unit"]:
         return i["unit"].replace("CO2 equivalent", "CO2e")
     if i["unit"] in ["kt", "t"]:
```

### Comparing `pyam_iamc-2.2.1/pyam/units.py` & `pyam_iamc-2.2.2/pyam/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         ret._data.index = replace_index_values(*index_args)
         return None if inplace else ret
 
     # Convert using a pint.UnitRegistry; default the one from iam_units
     registry = registry or iam_units.registry
 
     # Make versions without -equiv
-    _current, _to = [i.replace("-equiv", "") for i in [current, to]]
+    _current, _to = (i.replace("-equiv", "") for i in [current, to])
     # Pair of (magnitude, unit)
     qty = [ret._data.loc[where].values, _current]
 
     try:
         # Create a vector pint.Quantity and convert it ordinarily
         result = registry.Quantity(*qty).to(
             _to, context if context is not None else pint.Context()
```

### Comparing `pyam_iamc-2.2.1/pyam/utils.py` & `pyam_iamc-2.2.2/pyam/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 # dictionary to translate column count to Excel column names
 NUMERIC_TO_STR = dict(
     zip(
         range(0, 702),
         [i for i in string.ascii_uppercase]
         + [
-            "{}{}".format(i, j)
+            f"{i}{j}"
             for i, j in itertools.product(
                 string.ascii_uppercase, string.ascii_uppercase
             )
         ],
     )
 )
```

### Comparing `pyam_iamc-2.2.1/pyam/validation.py` & `pyam_iamc-2.2.2/pyam/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     in_range : bool, optional
         check if values are inside or outside of provided range
     return_test : str, optional
         possible values:
             - 'any': default, return scenarios where check passes for any entry
             - 'all': test if all values match checks, if not, return empty set
     """
-    valid_checks = set(["up", "lo", "year"])
+    valid_checks = {"up", "lo", "year"}
     if not set(check.keys()).issubset(valid_checks):
         msg = "Unknown checking type: {}"
         raise ValueError(msg.format(check.keys() - valid_checks))
     if "year" not in check:
         where_idx = set(rows.index)
     else:
         if "time" in rows.index.names:
@@ -95,15 +95,15 @@
             check_idx.append(set(rows.index[op(check[bd])]))
 
     if return_test == "any":
         ret = where_idx & set.union(*check_idx)
     elif return_test == "all":
         ret = where_idx if where_idx == set.intersection(*check_idx) else set()
     else:
-        raise ValueError("Unknown return test: {}".format(return_test))
+        raise ValueError(f"Unknown return test: {return_test}")
     return ret
 
 
 def _apply_criteria(df, criteria, **kwargs):
     """Apply criteria individually to every model/scenario instance"""
     idxs = []
     for var, check in criteria.items():
```

### Comparing `pyam_iamc-2.2.1/pyam/worldbank.py` & `pyam_iamc-2.2.2/pyam/worldbank.py`

 * *Files identical despite different names*

### Comparing `pyam_iamc-2.2.1/pyproject.toml` & `pyam_iamc-2.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyam-iamc"
-version = "2.2.1"
+version = "2.2.2"
 description = "Analysis & visualization of integrated-assessment scenarios"
 authors = [
     "Matthew Gidden <gidden@iiasa.ac.at>",
     "Daniel Huppmann <huppmann@iiasa.ac.at>",
     "Zebedee Nicholls <znicholls@unknown.com>",
     "Nikolay Kushin <zikolach@unknown.com>",
     "Robin Lamboll <Rlamboll@unknown.com>",
@@ -49,15 +49,14 @@
 numpy = ">=1.26.0"
 openpyxl = ">=3.1.2"
 pandas = ">=2.1.2"
 Pint = ">=0.13"
 PyYAML = ">=6.0.1"
 scipy = ">=1.10.0"
 seaborn = ">=0.11"
-six = ">=1.16.0"
 requests = ">2.27.1"
 wquantiles = ">=0.6"
 XlsxWriter = ">=3.0.3"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `pyam_iamc-2.2.1/PKG-INFO` & `pyam_iamc-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyam-iamc
-Version: 2.2.1
+Version: 2.2.2
 Summary: Analysis & visualization of integrated-assessment scenarios
 Home-page: https://github.com/IAMconsortium/pyam
 License: Apache-2.0
 Author: Matthew Gidden
 Author-email: gidden@iiasa.ac.at
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,14 @@
 Requires-Dist: matplotlib (>=3.6.0)
 Requires-Dist: numpy (>=1.26.0)
 Requires-Dist: openpyxl (>=3.1.2)
 Requires-Dist: pandas (>=2.1.2)
 Requires-Dist: requests (>2.27.1)
 Requires-Dist: scipy (>=1.10.0)
 Requires-Dist: seaborn (>=0.11)
-Requires-Dist: six (>=1.16.0)
 Requires-Dist: wquantiles (>=0.6)
 Project-URL: Documentation, https://pyam-iamc.readthedocs.io
 Project-URL: Repository, https://github.com/IAMconsortium/pyam
 Description-Content-Type: text/markdown
 
 pyam: analysis & visualization <br /> of integrated-assessment and macro-energy scenarios
 =========================================================================================
```

