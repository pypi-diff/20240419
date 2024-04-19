# Comparing `tmp/polars_ts-0.0.6.tar.gz` & `tmp/polars_ts-0.0.7.tar.gz`

## Comparing `polars_ts-0.0.6.tar` & `polars_ts-0.0.7.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 polars_ts-0.0.6/Cargo.toml
--rw-r--r--   0     1001      127     3402 2024-04-18 14:22:51.000000 polars_ts-0.0.6/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127     3107 2024-04-18 14:22:51.000000 polars_ts-0.0.6/.gitignore
--rw-r--r--   0     1001      127        7 2024-04-18 14:22:51.000000 polars_ts-0.0.6/.python-version
--rw-r--r--   0     1001      127      147 2024-04-18 14:22:51.000000 polars_ts-0.0.6/.vscode/settings.json
--rw-r--r--   0     1001      127    11357 2024-04-18 14:22:51.000000 polars_ts-0.0.6/LICENSE
--rw-r--r--   0     1001      127      704 2024-04-18 14:22:51.000000 polars_ts-0.0.6/Makefile
--rw-r--r--   0     1001      127     1002 2024-04-18 14:22:51.000000 polars_ts-0.0.6/README.md
--rw-r--r--   0     1001      127      954 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/__init__.py
--rw-r--r--   0     1001      127     1637 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/calendar.py
--rw-r--r--   0     1001      127     2537 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/calendar_helper/__init__.py
--rw-r--r--   0     1001      127      673 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/display.py
--rw-r--r--   0     1001      127     2540 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/dummy.py
--rw-r--r--   0     1001      127     2851 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/dummy_helper/__init__.py
--rw-r--r--   0     1001      127     1178 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/dummymkt.py
--rw-r--r--   0     1001      127     1633 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/dummymkt_helper/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/expr/__init__.py
--rw-r--r--   0     1001      127     1580 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/expr/random.py
--rw-r--r--   0     1001      127     1213 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures.py
--rw-r--r--   0     1001      127     2307 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures_helper/__init__.py
--rw-r--r--   0     1001      127      850 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures_helper/bbg_symbols.py
--rw-r--r--   0     1001      127     1135 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures_helper/generic_symbols.py
--rw-r--r--   0     1001      127     7751 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures_helper/roll_calendar.py
--rw-r--r--   0     1001      127      890 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures_helper/util.py
--rw-r--r--   0     1001      127     5258 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/grouper.py
--rw-r--r--   0     1001      127      510 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/loader.py
--rw-r--r--   0     1001      127     1633 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/mathx.py
--rw-r--r--   0     1001      127     1876 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/mathx_helper/__init__.py
--rw-r--r--   0     1001      127     2437 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/resample.py
--rw-r--r--   0     1001      127     3118 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/resample_helper/__init__.py
--rw-r--r--   0     1001      127      770 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/sf.py
--rw-r--r--   0     1001      127     1495 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/sf_helper/__init__.py
--rw-r--r--   0     1001      127      684 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/time.py
--rw-r--r--   0     1001      127      937 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/time_helper/__init__.py
--rw-r--r--   0     1001      127      397 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/tsf.py
--rw-r--r--   0     1001      127      459 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/types.py
--rw-r--r--   0     1001      127     1289 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/utils.py
--rw-r--r--   0     1001      127       32 2024-04-18 14:22:51.000000 polars_ts-0.0.6/requirements.txt
--rw-r--r--   0     1001      127      445 2024-04-18 14:22:51.000000 polars_ts-0.0.6/ruff.toml
--rw-r--r--   0     1001      127      212 2024-04-18 14:22:51.000000 polars_ts-0.0.6/run.py
--rw-r--r--   0     1001      127     2617 2024-04-18 14:22:51.000000 polars_ts-0.0.6/src/expressions.rs
--rw-r--r--   0     1001      127      382 2024-04-18 14:22:51.000000 polars_ts-0.0.6/src/lib.rs
--rw-r--r--   0     1001      127     1839 2024-04-18 14:22:51.000000 polars_ts-0.0.6/src/math/mod.rs
--rw-r--r--   0     1001      127     2712 2024-04-18 14:22:51.000000 polars_ts-0.0.6/src/utils.rs
--rw-r--r--   0     1001      127      212 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/00_config/roll_config.csv
--rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/__init__.py
--rw-r--r--   0     1001      127      146 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/config.py
--rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/futures/__init__.py
--rw-r--r--   0     1001      127     2125 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/futures/test_continuous_contract.py
--rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/grouper/__init__.py
--rw-r--r--   0     1001      127     2737 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/grouper/test_grouper.py
--rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/mathx/__init__.py
--rw-r--r--   0     1001      127    11052 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/mathx/test_cum_sum.py
--rw-r--r--   0     1001      127    13921 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/mathx/test_diff.py
--rw-r--r--   0     1001      127     3234 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/mathx/test_ewm_mean.py
--rw-r--r--   0     1001      127    11395 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/mathx/test_shift.py
--rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/resample/__init__.py
--rw-r--r--   0     1001      127    10278 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/resample/test_resample.py
--rw-r--r--   0     1001      127     1248 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/sf/test_join.py
--rw-r--r--   0     1001      127      846 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/test_rust_templates.py
--rw-r--r--   0     1001      127    36490 2024-04-18 14:22:51.000000 polars_ts-0.0.6/Cargo.lock
--rw-r--r--   0     1001      127      478 2024-04-18 14:22:51.000000 polars_ts-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 polars_ts-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 polars_ts-0.0.7/Cargo.toml
+-rw-r--r--   0     1001      127     3402 2024-04-18 22:25:12.000000 polars_ts-0.0.7/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127     3107 2024-04-18 22:25:12.000000 polars_ts-0.0.7/.gitignore
+-rw-r--r--   0     1001      127        7 2024-04-18 22:25:12.000000 polars_ts-0.0.7/.python-version
+-rw-r--r--   0     1001      127      147 2024-04-18 22:25:12.000000 polars_ts-0.0.7/.vscode/settings.json
+-rw-r--r--   0     1001      127    11357 2024-04-18 22:25:12.000000 polars_ts-0.0.7/LICENSE
+-rw-r--r--   0     1001      127      704 2024-04-18 22:25:12.000000 polars_ts-0.0.7/Makefile
+-rw-r--r--   0     1001      127     1002 2024-04-18 22:25:12.000000 polars_ts-0.0.7/README.md
+-rw-r--r--   0     1001      127      950 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/__init__.py
+-rw-r--r--   0     1001      127     1637 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/calendar.py
+-rw-r--r--   0     1001      127     2537 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/calendar_helper/__init__.py
+-rw-r--r--   0     1001      127      673 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/display.py
+-rw-r--r--   0     1001      127     2567 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/dummy.py
+-rw-r--r--   0     1001      127     2851 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/dummy_helper/__init__.py
+-rw-r--r--   0     1001      127     1178 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/dummymkt.py
+-rw-r--r--   0     1001      127     1642 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/dummymkt_helper/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/expr/__init__.py
+-rw-r--r--   0     1001      127     1580 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/expr/random.py
+-rw-r--r--   0     1001      127     1213 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/futures.py
+-rw-r--r--   0     1001      127     2307 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/futures_helper/__init__.py
+-rw-r--r--   0     1001      127      850 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/futures_helper/bbg_symbols.py
+-rw-r--r--   0     1001      127     1135 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/futures_helper/generic_symbols.py
+-rw-r--r--   0     1001      127     7751 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/futures_helper/roll_calendar.py
+-rw-r--r--   0     1001      127      890 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/futures_helper/util.py
+-rw-r--r--   0     1001      127     5528 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/grouper.py
+-rw-r--r--   0     1001      127      507 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/io.py
+-rw-r--r--   0     1001      127     1084 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/io_helper/__init__.py
+-rw-r--r--   0     1001      127     1669 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/mathx.py
+-rw-r--r--   0     1001      127     1876 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/mathx_helper/__init__.py
+-rw-r--r--   0     1001      127     2446 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/resample.py
+-rw-r--r--   0     1001      127     2983 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/resample_helper/__init__.py
+-rw-r--r--   0     1001      127      947 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/sf.py
+-rw-r--r--   0     1001      127     1672 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/sf_helper/__init__.py
+-rw-r--r--   0     1001      127      684 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/time.py
+-rw-r--r--   0     1001      127      937 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/time_helper/__init__.py
+-rw-r--r--   0     1001      127      397 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/tsf.py
+-rw-r--r--   0     1001      127      459 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/types.py
+-rw-r--r--   0     1001      127     1289 2024-04-18 22:25:12.000000 polars_ts-0.0.7/polars_ts/utils.py
+-rw-r--r--   0     1001      127       32 2024-04-18 22:25:12.000000 polars_ts-0.0.7/requirements.txt
+-rw-r--r--   0     1001      127      445 2024-04-18 22:25:12.000000 polars_ts-0.0.7/ruff.toml
+-rw-r--r--   0     1001      127      212 2024-04-18 22:25:12.000000 polars_ts-0.0.7/run.py
+-rw-r--r--   0     1001      127     2617 2024-04-18 22:25:12.000000 polars_ts-0.0.7/src/expressions.rs
+-rw-r--r--   0     1001      127      382 2024-04-18 22:25:12.000000 polars_ts-0.0.7/src/lib.rs
+-rw-r--r--   0     1001      127     1839 2024-04-18 22:25:12.000000 polars_ts-0.0.7/src/math/mod.rs
+-rw-r--r--   0     1001      127     2712 2024-04-18 22:25:12.000000 polars_ts-0.0.7/src/utils.rs
+-rw-r--r--   0     1001      127      212 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/00_config/roll_config.csv
+-rw-r--r--   0     1001      127        0 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/__init__.py
+-rw-r--r--   0     1001      127      146 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/config.py
+-rw-r--r--   0     1001      127        0 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/futures/__init__.py
+-rw-r--r--   0     1001      127     2148 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/futures/test_continuous_contract.py
+-rw-r--r--   0     1001      127        0 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/grouper/__init__.py
+-rw-r--r--   0     1001      127     2771 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/grouper/test_grouper.py
+-rw-r--r--   0     1001      127        0 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/mathx/__init__.py
+-rw-r--r--   0     1001      127    11052 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/mathx/test_cum_sum.py
+-rw-r--r--   0     1001      127    13921 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/mathx/test_diff.py
+-rw-r--r--   0     1001      127     3234 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/mathx/test_ewm_mean.py
+-rw-r--r--   0     1001      127    11395 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/mathx/test_shift.py
+-rw-r--r--   0     1001      127        0 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/resample/__init__.py
+-rw-r--r--   0     1001      127    10725 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/resample/test_resample.py
+-rw-r--r--   0     1001      127     1248 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/sf/test_join.py
+-rw-r--r--   0     1001      127     1080 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/sf/test_sf.py
+-rw-r--r--   0     1001      127      846 2024-04-18 22:25:12.000000 polars_ts-0.0.7/tests/test_rust_templates.py
+-rw-r--r--   0     1001      127    36490 2024-04-18 22:25:12.000000 polars_ts-0.0.7/Cargo.lock
+-rw-r--r--   0     1001      127      478 2024-04-18 22:25:12.000000 polars_ts-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 polars_ts-0.0.7/PKG-INFO
```

### Comparing `polars_ts-0.0.6/Cargo.toml` & `polars_ts-0.0.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars-ts"
-version = "0.0.6"
+version = "0.0.7"
 edition = "2021"
 
 [lib]
 name = "polars_ts"
 crate-type= ["cdylib"]
 
 [dependencies]
```

### Comparing `polars_ts-0.0.6/.github/workflows/publish_to_pypi.yml` & `polars_ts-0.0.7/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/.gitignore` & `polars_ts-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/LICENSE` & `polars_ts-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/Makefile` & `polars_ts-0.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/README.md` & `polars_ts-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/__init__.py` & `polars_ts-0.0.7/polars_ts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING
 
 import polars as pl
 
 from .display import *
 from .sf import *
 from .tsf import *
-from .loader import *
+from .io import *
 from .time import *
 from .dummy import *
 from .mathx import *
 from .resample import *
 
 from .calendar import *
 from .futures import *
```

### Comparing `polars_ts-0.0.6/polars_ts/calendar.py` & `polars_ts-0.0.7/polars_ts/calendar.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/calendar_helper/__init__.py` & `polars_ts-0.0.7/polars_ts/calendar_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/display.py` & `polars_ts-0.0.7/polars_ts/display.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/dummy.py` & `polars_ts-0.0.7/polars_ts/dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def random_category_subgroups(
         self,
         prefix: IntoExpr,
         sizes: List[int],
         *,
         max_num_subgroups: Optional[int] = None,
         seed: int = 42,
-        partition: Grouper = Grouper(),
+        partition: Grouper = Grouper().by_all(),
         out: str = "subgroup",
     ) -> FrameType:
         prefix = parse_into_expr(prefix)
 
         if max_num_subgroups is None:
             size_estimate = self._df.select(1 + (pl.len() // max(sizes)))
             if isinstance(size_estimate, pl.LazyFrame):
@@ -51,27 +51,27 @@
         return prepare_result(df)
 
     def random_uniform(
         self,
         lower: Union[pl.Expr, float] = 0.0,
         upper: Union[pl.Expr, float] = 1.0,
         *,
-        partition: Grouper = Grouper(),
+        partition: Grouper = Grouper().by_all(),
         out: str = "value",
     ) -> FrameType:
         df = impl_random_uniform(self._df, lower, upper, partition, out)
 
         return prepare_result(df)
 
     def random_normal(
         self,
         mu: Union[pl.Expr, float] = 0.0,
         sigma: Union[pl.Expr, float] = 1.0,
         *,
-        partition: Grouper = Grouper(),
+        partition: Grouper = Grouper().by_all(),
         out: str = "value",
     ) -> FrameType:
         df = impl_random_normal(self._df, partition, out, mu, sigma)
 
         return prepare_result(df)
 
     def enum(
```

### Comparing `polars_ts-0.0.6/polars_ts/dummy_helper/__init__.py` & `polars_ts-0.0.7/polars_ts/dummy_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/dummymkt.py` & `polars_ts-0.0.7/polars_ts/dummymkt.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/dummymkt_helper/__init__.py` & `polars_ts-0.0.7/polars_ts/dummymkt_helper/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             time=pl.date_ranges(start_dt, end_dt),
             asset=pl.col("asset"),
             instrument_id=pl.col("instrument_id"),
         )
         .explode(pl.col("time"))
         .pipe(
             lambda df: impl_random_normal(
-                df, partition=Grouper(), out="value", mu=0.0, sigma=1.0
+                df, partition=Grouper().by_all(), out="value", mu=0.0, sigma=1.0
             )
         )
         .filter(pl.col("time").dt.weekday().is_in(hols).not_())
         .with_columns(pl.col("value").cum_sum().over("asset", "instrument_id"))
     )
 
     return result
```

### Comparing `polars_ts-0.0.6/polars_ts/expr/random.py` & `polars_ts-0.0.7/polars_ts/expr/random.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/futures.py` & `polars_ts-0.0.7/polars_ts/futures.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/futures_helper/__init__.py` & `polars_ts-0.0.7/polars_ts/futures_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/futures_helper/bbg_symbols.py` & `polars_ts-0.0.7/polars_ts/futures_helper/bbg_symbols.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/futures_helper/generic_symbols.py` & `polars_ts-0.0.7/polars_ts/futures_helper/generic_symbols.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/futures_helper/roll_calendar.py` & `polars_ts-0.0.7/polars_ts/futures_helper/roll_calendar.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/futures_helper/util.py` & `polars_ts-0.0.7/polars_ts/futures_helper/util.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/grouper.py` & `polars_ts-0.0.7/polars_ts/grouper.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,19 +113,22 @@
 
     @staticmethod
     def numerics(df: FrameType) -> List[str]:
         cols = df.select(pl.col(pl.NUMERIC_DTYPES)).columns
         return sorted(cols)
 
     def apply(self, *dfs: FrameType) -> List[str]:
+        if not self._has_defined_spec:
+            raise ValueError("A Grouper spec has not been defined.")
+
         if self._common and len(dfs) < 2:
             raise ValueError("Require at least 2 dataframes when 'common' flag is set.")
 
         if not self._common and len(dfs) != 1:
-            raise ValueError("Too many arguments passed to apply.")
+            raise ValueError(f"Too many arguments passed to {str(self)}.apply(...)")
 
         if self._common:
             df = dfs[0]
             df_other = dfs[1]
             df_has_time = ("time" in df) and ("time" in df_other)
             cols = set(Grouper.common_categories(df, df_other))
         else:
@@ -164,8 +167,12 @@
             time_clause = "TimeAnd" if self._result_includes_time else ""
             return f"By{time_clause}({','.join(sorted(self._by))})"
 
         if self._all:
             time_clause = "TimeAnd" if self._result_includes_time else ""
             return f"By{time_clause}All"
 
+        if self._common:
+            time_clause = "TimeAnd" if self._result_includes_time else ""
+            return f"By{time_clause}Common"
+
         return "ByNone"
```

### Comparing `polars_ts-0.0.6/polars_ts/mathx.py` & `polars_ts-0.0.7/polars_ts/mathx.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,38 +19,38 @@
     def __init__(self, df: FrameType):
         super().__init__(df)
 
     def diff(
         self,
         k: int = 1,
         method: Literal["arithmetic", "fractional", "geometric"] = "arithmetic",
-        partition: Grouper = Grouper(),
+        partition: Grouper = Grouper().by_all(),
         null_strategy: NullStrategyType = "drop",
         null_sentinel_numeric: SentinelNumeric = 0.0,
     ) -> FrameType:
         df = impl_diff(
             self._df, k, method, partition, null_strategy, null_sentinel_numeric
         )
         return prepare_result(df)
 
-    def cum_sum(self, partition: Grouper = Grouper()) -> FrameType:
+    def cum_sum(self, partition: Grouper = Grouper().by_all()) -> FrameType:
         df = impl_cum_sum(self._df, partition)
 
         return prepare_result(df)
 
     def shift(
         self,
         k: int = 1,
         null_strategy: NullStrategyType = "ignore",
         null_sentinel_numeric: SentinelNumeric = 0.0,
-        partition: Grouper = Grouper(),
+        partition: Grouper = Grouper().by_all(),
     ) -> FrameType:
         df = impl_shift(self._df, k, null_strategy, null_sentinel_numeric, partition)
         return prepare_result(df)
 
     def ewm_mean(
         self,
         half_life: float,
-        partition: Grouper = Grouper(),
+        partition: Grouper = Grouper().by_all(),
     ) -> FrameType:
         df = impl_ewm_mean(self._df, half_life, partition)
         return prepare_result(df)
```

### Comparing `polars_ts-0.0.6/polars_ts/mathx_helper/__init__.py` & `polars_ts-0.0.7/polars_ts/mathx_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/resample.py` & `polars_ts-0.0.7/polars_ts/resample.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def __init__(self, df: FrameType):
         super().__init__(df)
 
     def to_ohlc(
         self,
         period: str,
         *,
-        partition: Grouper = Grouper(),
+        partition: Grouper = Grouper().by_all(),
         value_col: str = "value",
     ) -> FrameType:
         grouper_cols = partition.apply(self._df)
 
         df = (
             self._df.sort("time")
             .group_by_dynamic("time", every=period, group_by=grouper_cols)
@@ -47,39 +47,39 @@
         )
 
         return prepare_result(df)
 
     def align_to_time(
         self,
         time_axis: pl.Series,
-        partition: Grouper = Grouper(),
+        partition: Grouper = Grouper().by_all(),
         closed: IntervalType = "left",
         null_strategy: NullStrategyType = "forward",
         null_sentinel_numeric: Union[float, int] = 0.0,
     ) -> FrameType:
         df = impl_align_to_time(
             self._df, time_axis, partition, closed, null_strategy, null_sentinel_numeric
         )
 
         return prepare_result(df)
 
     def resample_categories(
         self,
         time_axis: pl.Series,
-        partition: Grouper = Grouper(),
+        partition: Grouper = Grouper().by_all(),
         closed: IntervalType = "left",
     ) -> FrameType:
         df = impl_resample_categories(self._df, time_axis, partition, closed)
 
         return prepare_result(df)
 
     def align_values(
         self,
         rhs: FrameType,
-        partition: Grouper = Grouper().by_common_including_time(),
+        partition: Grouper = Grouper().by_all(),
         retain_values: Literal["lhs", "rhs", "both"] = "lhs",
         null_strategy: NullStrategyType = "forward",
         null_sentinel_numeric: Union[float, int] = 0.0,
     ) -> FrameType:
         df = impl_align_values(
             self._df,
             rhs,
```

### Comparing `polars_ts-0.0.6/polars_ts/resample_helper/__init__.py` & `polars_ts-0.0.7/polars_ts/resample_helper/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, List
+from typing import Union
 
 import polars as pl
 
 from ..sf_helper import impl_apply_null_strategy
 from ..grouper import Grouper
 
 from ..types import (
@@ -86,24 +86,19 @@
         rhs = rhs_grid
 
     if retain_values == "rhs":
         # strip away lhs values
         lhs_cat_cols = Grouper.categories(lhs, include_time=True)
         lhs = lhs.select(lhs_cat_cols)
 
-    assert isinstance(lhs, type(rhs)) and (
-        isinstance(lhs, pl.LazyFrame) or isinstance(lhs, pl.DataFrame)
-    )
-
-    grouper_cols: List[str] = partition.apply(lhs, rhs)
-
+    common_cols = Grouper().by_common_including_time().apply(lhs, rhs)
     result = (
-        lhs.join(rhs, on=["time", *grouper_cols], how="outer_coalesce")
+        lhs.join(rhs, on=common_cols, how="outer_coalesce")
         .filter(pl.col("time").is_not_null())
-        .sort("time", *grouper_cols)
+        .sort(*common_cols)
         .unique(keep="first", maintain_order=True)
     )
 
     result = impl_apply_null_strategy(
         result, null_strategy, null_sentinel_numeric, partition
     )
```

### Comparing `polars_ts-0.0.6/polars_ts/sf.py` & `polars_ts-0.0.7/polars_ts/sf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from typing import Generic
 
 import polars as pl
 from polars.type_aliases import JoinStrategy
 
 from .grouper import Grouper
-from .sf_helper import RESERVED_ALL_GRP, impl_join, prepare_result
+from .sf_helper import RESERVED_ALL_GRP, impl_join, prepare_result, impl_unique
 from .types import FrameType
 
 __NAMESPACE = "sf"
 
 
 @pl.api.register_lazyframe_namespace(__NAMESPACE)
 class SeriesFrame(Generic[FrameType]):
     def __init__(self, df: FrameType):
         self._df: FrameType = df.with_columns(
-            pl.lit(0, pl.Boolean).cast(pl.Categorical).alias(RESERVED_ALL_GRP)
+            pl.lit("_placeholder_").cast(pl.Categorical).alias(RESERVED_ALL_GRP)
         )
 
     def join(
         self,
         other: FrameType,
         grouper: Grouper = Grouper().by_common_including_time(),
         how: JoinStrategy = "inner",
     ) -> FrameType:
         df = impl_join(self._df, other, grouper, how)
         return prepare_result(df)
+
+    def unique(self, grouper: Grouper = Grouper().by_time_and_all()) -> FrameType:
+        df = impl_unique(self._df, grouper)
+        return prepare_result(df)
```

### Comparing `polars_ts-0.0.6/polars_ts/sf_helper/__init__.py` & `polars_ts-0.0.7/polars_ts/sf_helper/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,7 +47,13 @@
 def impl_join(
     lhs: FrameType, rhs: FrameType, grouper: Grouper, how: JoinStrategy
 ) -> FrameType:
     grouper_cols = grouper.apply(lhs, rhs)
     df = lhs.join(rhs, on=grouper_cols, how=how)
 
     return df
+
+
+def impl_unique(df: FrameType, grouper: Grouper) -> FrameType:
+    grouper_cols = grouper.apply(df)
+    df = df.unique(subset=grouper_cols, maintain_order=True)
+    return df
```

### Comparing `polars_ts-0.0.6/polars_ts/time.py` & `polars_ts-0.0.7/polars_ts/time.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/time_helper/__init__.py` & `polars_ts-0.0.7/polars_ts/time_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/polars_ts/utils.py` & `polars_ts-0.0.7/polars_ts/utils.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/src/expressions.rs` & `polars_ts-0.0.7/src/expressions.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/src/math/mod.rs` & `polars_ts-0.0.7/src/math/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/src/utils.rs` & `polars_ts-0.0.7/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/tests/futures/test_continuous_contract.py` & `polars_ts-0.0.7/tests/futures/test_continuous_contract.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def test_continuous_contract():
     market_start_date = datetime(1990, 1, 1, 23, 0, tzinfo=UTC)
     market_end_date = datetime(2000, 1, 1, 23, 0, tzinfo=UTC)
 
     roll_config_filename = get_config_filename("roll_config.csv")
-    roll_config = pl.LazyFrame().loader.csv(roll_config_filename)
+    roll_config = pl.LazyFrame().io.read_csv(roll_config_filename)
 
     generic_symbols = generic_symbol_universe(
         roll_config, market_start_date, market_end_date
     )
     security_meta = guess_security_meta(generic_symbols, roll_config)
 
     security_dates = (
@@ -58,11 +58,13 @@
         ),
         ("unadjusted", pl.Float64),
         ("panama_backwards", pl.Float64),
     ]
 
     assert adjusted_prices_schema == expected_schema
 
-    assert adjusted_prices.shape == (10030, 5)
+    result = adjusted_prices.collect()
+
+    assert result.shape == (10030, 5)
 
     # replace that with a stable hash
-    assert adjusted_prices.hash_rows().sum() == 4148443207706655575
+    assert result.hash_rows().sum() == 4148443207706655575
```

### Comparing `polars_ts-0.0.6/tests/grouper/test_grouper.py` & `polars_ts-0.0.7/tests/grouper/test_grouper.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,16 @@
     assert Grouper.by_common_including_time().apply(df, df) == [
         "time",
         "catsa",
         "catsb",
     ]
 
     with pytest.raises(ValueError, match="Empty Grouper Specification"):
-        assert Grouper.omitting_time_and("catsa", "catsb").apply(df) == []
+        Grouper.omitting_time_and("catsa", "catsb").apply(df) == []
 
     with pytest.raises(ValueError, match="Empty Grouper Specification"):
-        assert Grouper.omitting("time", "catsa", "catsb").apply(df) == []
+        Grouper.omitting("time", "catsa", "catsb").apply(df) == []
 
 
 def test_default(df):
-    assert Grouper().apply(df) == Grouper.by_all().apply(df)
+    with pytest.raises(ValueError, match="A Grouper spec has not been defined"):
+        Grouper().apply(df)
```

### Comparing `polars_ts-0.0.6/tests/mathx/test_cum_sum.py` & `polars_ts-0.0.7/tests/mathx/test_cum_sum.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/tests/mathx/test_diff.py` & `polars_ts-0.0.7/tests/mathx/test_diff.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/tests/mathx/test_ewm_mean.py` & `polars_ts-0.0.7/tests/mathx/test_ewm_mean.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/tests/mathx/test_shift.py` & `polars_ts-0.0.7/tests/mathx/test_shift.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/tests/resample/test_resample.py` & `polars_ts-0.0.7/tests/resample/test_resample.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime, timedelta
 import polars as pl
+import polars_ts  # noqa
 import pytest
 
 
 @pytest.fixture
 def df() -> pl.LazyFrame:
     t = datetime(2024, 1, 1, 0)
     nrows = 3
@@ -328,7 +329,23 @@
         ]
     )
 
     assert align_none.equals(expected_df)
     assert align_left.equals(expected_df)
     assert align_right.equals(expected_df)
     assert align_both.equals(expected_df)
+
+
+def test_align_to_time(df):
+    time_axis = pl.datetime_ranges(
+        df.collect()["time"].min(), df.collect()["time"].max(), eager=True
+    ).explode()
+
+    result = df.rs.align_to_time(
+        time_axis, closed="none", null_strategy="sentinel_numeric"
+    )
+    assert not result.collect().is_empty()
+
+
+def test_align_values(df):
+    result = df.rs.align_values(df).collect()
+    assert df.collect().equals(result)
```

### Comparing `polars_ts-0.0.6/tests/sf/test_join.py` & `polars_ts-0.0.7/tests/sf/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/tests/test_rust_templates.py` & `polars_ts-0.0.7/tests/test_rust_templates.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.6/Cargo.lock` & `polars_ts-0.0.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -671,15 +671,15 @@
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-ts"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "jemallocator",
  "polars",
  "pyo3",
  "pyo3-polars",
  "rand",
  "rand_distr",
```

### Comparing `polars_ts-0.0.6/PKG-INFO` & `polars_ts-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-ts
-Version: 0.0.6
+Version: 0.0.7
 Requires-Dist: polars >=0.20.21
 Requires-Dist: polars-xdt
 Requires-Dist: hvplot
 Requires-Dist: pyarrow
 Requires-Dist: hvplot ; extra == 'dev'
 Requires-Dist: pyarrow ; extra == 'dev'
 Provides-Extra: dev
```

