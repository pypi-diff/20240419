# Comparing `tmp/model_diagnostics-1.1.0.tar.gz` & `tmp/model_diagnostics-1.1.1.tar.gz`

## Comparing `model_diagnostics-1.1.0.tar` & `model_diagnostics-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/.codecov.yml
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/mkdocs.yml
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/dev_tools/print_package_versions.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/docs/development.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/docs/index.md
--rw-r--r--   0        0        0   254552 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/docs/examples/classification.ipynb
--rw-r--r--   0        0        0   317172 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/docs/examples/quantile_regression.ipynb
--rw-r--r--   0        0        0   553751 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/docs/examples/regression_on_workers_compensation.ipynb
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/__about__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/__init__.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/_utils/__init__.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/_utils/_array.py
--rw-r--r--   0        0        0    20825 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/_utils/isotonic.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/_utils/plot_helper.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/_utils/test_helper.py
--rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/_utils/tests/test_array.py
--rw-r--r--   0        0        0    15756 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/_utils/tests/test_isotonic.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/calibration/__init__.py
--rw-r--r--   0        0        0    23289 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/calibration/identification.py
--rw-r--r--   0        0        0    26093 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/calibration/plots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/calibration/tests/__init__.py
--rw-r--r--   0        0        0    19413 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/calibration/tests/test_identification.py
--rw-r--r--   0        0        0    15486 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/calibration/tests/test_plots.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/scoring/__init__.py
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/scoring/plots.py
--rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/scoring/scoring.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/scoring/tests/__init__.py
--rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/scoring/tests/test_plots.py
--rw-r--r--   0        0        0    41342 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/scoring/tests/test_scoring.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/src/model_diagnostics/tests/test_config.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/LICENSE
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/README.md
--rw-r--r--   0        0        0     6960 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 model_diagnostics-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/.codecov.yml
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/mkdocs.yml
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/dev_tools/print_package_versions.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/docs/development.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/docs/index.md
+-rw-r--r--   0        0        0   254552 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/docs/examples/classification.ipynb
+-rw-r--r--   0        0        0   317172 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/docs/examples/quantile_regression.ipynb
+-rw-r--r--   0        0        0   553751 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/docs/examples/regression_on_workers_compensation.ipynb
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/__about__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/__init__.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/_utils/__init__.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/_utils/_array.py
+-rw-r--r--   0        0        0    20825 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/_utils/isotonic.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/_utils/plot_helper.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/_utils/test_helper.py
+-rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/_utils/tests/test_array.py
+-rw-r--r--   0        0        0    15756 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/_utils/tests/test_isotonic.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/calibration/__init__.py
+-rw-r--r--   0        0        0    23746 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/calibration/identification.py
+-rw-r--r--   0        0        0    26055 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/calibration/plots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/calibration/tests/__init__.py
+-rw-r--r--   0        0        0    19413 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/calibration/tests/test_identification.py
+-rw-r--r--   0        0        0    15486 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/calibration/tests/test_plots.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/scoring/__init__.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/scoring/plots.py
+-rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/scoring/scoring.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/scoring/tests/__init__.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/scoring/tests/test_plots.py
+-rw-r--r--   0        0        0    41342 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/scoring/tests/test_scoring.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/src/model_diagnostics/tests/test_config.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/README.md
+-rw-r--r--   0        0        0     6960 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 model_diagnostics-1.1.1/PKG-INFO
```

### Comparing `model_diagnostics-1.1.0/mkdocs.yml` & `model_diagnostics-1.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/docs/development.md` & `model_diagnostics-1.1.1/docs/development.md`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/docs/gen_ref_pages.py` & `model_diagnostics-1.1.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/docs/index.md` & `model_diagnostics-1.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/docs/examples/classification.ipynb` & `model_diagnostics-1.1.1/docs/examples/classification.ipynb`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/docs/examples/quantile_regression.ipynb` & `model_diagnostics-1.1.1/docs/examples/quantile_regression.ipynb`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/docs/examples/regression_on_workers_compensation.ipynb` & `model_diagnostics-1.1.1/docs/examples/regression_on_workers_compensation.ipynb`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/__about__.py` & `model_diagnostics-1.1.1/src/model_diagnostics/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   X.Y.ZbN   # Beta release
 #   X.Y.ZrcN  # Release Candidate
 #   X.Y.Z     # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "1.1.0"
+__version__ = "1.1.1"
```

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/_config.py` & `model_diagnostics-1.1.1/src/model_diagnostics/_config.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/_utils/_array.py` & `model_diagnostics-1.1.1/src/model_diagnostics/_utils/_array.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/_utils/isotonic.py` & `model_diagnostics-1.1.1/src/model_diagnostics/_utils/isotonic.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/_utils/plot_helper.py` & `model_diagnostics-1.1.1/src/model_diagnostics/_utils/plot_helper.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/_utils/test_helper.py` & `model_diagnostics-1.1.1/src/model_diagnostics/_utils/test_helper.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/_utils/tests/test_array.py` & `model_diagnostics-1.1.1/src/model_diagnostics/_utils/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/_utils/tests/test_isotonic.py` & `model_diagnostics-1.1.1/src/model_diagnostics/_utils/tests/test_isotonic.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/calibration/identification.py` & `model_diagnostics-1.1.1/src/model_diagnostics/calibration/identification.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,16 +462,23 @@
                         pl.when(pl.col(feature_name).is_null())
                         .then(pl.max("bias_count") + 1)
                         .otherwise(pl.col("bias_count"))
                         .alias("__priority")
                     )
                     .sort("__priority", descending=True)
                     .head(n_bins)
-                    .sort(feature_name, descending=False)
                 )
+                # FIXME: When n_bins=0, the resut should be an empty dataframe
+                # (0 rows and some columns). For some unknown reason as of
+                # polars 0.20.20, the following sort neglects the head(0) statement.
+                # Therefore, we place an explicit collect here. This should not be
+                # needed!
+                if n_bins == 0 or feature.null_count() >= 1:
+                    df = df.collect().lazy()
+                df = df.sort(feature_name, descending=False)
 
                 df = df.select(
                     [
                         pl.col(feature_name),
                         pl.col("bias_mean"),
                         pl.col("bias_count"),
                         pl.col("bias_weights"),
```

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/calibration/plots.py` & `model_diagnostics-1.1.1/src/model_diagnostics/calibration/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,14 @@
     weights: Optional[npt.ArrayLike] = None,
     *,
     functional: str = "mean",
     level: float = 0.5,
     n_bins: int = 10,
     confidence_level: float = 0.9,
     ax: Optional[mpl.axes.Axes] = None,
-    plot_backend: str = "matplotlib",
 ):
     r"""Plot model bias conditional on a feature.
 
     This plots the generalised bias (residuals), i.e. the values of the canonical
     identification function, versus a feature. This is a good way to assess whether
     a model is conditionally calibrated or not. Well calibrated models have bias terms
     around zero.
```

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/calibration/tests/test_identification.py` & `model_diagnostics-1.1.1/src/model_diagnostics/calibration/tests/test_identification.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/calibration/tests/test_plots.py` & `model_diagnostics-1.1.1/src/model_diagnostics/calibration/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/scoring/plots.py` & `model_diagnostics-1.1.1/src/model_diagnostics/scoring/plots.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/scoring/scoring.py` & `model_diagnostics-1.1.1/src/model_diagnostics/scoring/scoring.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/scoring/tests/test_plots.py` & `model_diagnostics-1.1.1/src/model_diagnostics/scoring/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/scoring/tests/test_scoring.py` & `model_diagnostics-1.1.1/src/model_diagnostics/scoring/tests/test_scoring.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/src/model_diagnostics/tests/test_config.py` & `model_diagnostics-1.1.1/src/model_diagnostics/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/.gitignore` & `model_diagnostics-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/LICENSE` & `model_diagnostics-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/README.md` & `model_diagnostics-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/pyproject.toml` & `model_diagnostics-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `model_diagnostics-1.1.0/PKG-INFO` & `model_diagnostics-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-diagnostics
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for diagnostics and assessment of (machine learning) models
 Project-URL: Homepage, https://lorentzenchr.github.io/model-diagnostics/
 Project-URL: Source, https://github.com/lorentzenchr/model-diagnostics
 Project-URL: Tracker, https://github.com/lorentzenchr/model-diagnostics/issues
 Author-email: Christian Lorentzen <lorentzen.ch@gmail.com>
 License: MIT License
```

