# Comparing `tmp/polars_ts-0.0.5.tar.gz` & `tmp/polars_ts-0.0.6.tar.gz`

## Comparing `polars_ts-0.0.5.tar` & `polars_ts-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,63 @@
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 polars_ts-0.0.5/Cargo.toml
--rw-r--r--   0     1001      127     3402 2024-04-17 22:55:56.000000 polars_ts-0.0.5/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127     3107 2024-04-17 22:55:56.000000 polars_ts-0.0.5/.gitignore
--rw-r--r--   0     1001      127        7 2024-04-17 22:55:56.000000 polars_ts-0.0.5/.python-version
--rw-r--r--   0     1001      127      147 2024-04-17 22:55:56.000000 polars_ts-0.0.5/.vscode/settings.json
--rw-r--r--   0     1001      127    11357 2024-04-17 22:55:56.000000 polars_ts-0.0.5/LICENSE
--rw-r--r--   0     1001      127      704 2024-04-17 22:55:56.000000 polars_ts-0.0.5/Makefile
--rw-r--r--   0     1001      127     1002 2024-04-17 22:55:56.000000 polars_ts-0.0.5/README.md
--rw-r--r--   0     1001      127      933 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/__init__.py
--rw-r--r--   0     1001      127     1637 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/calendar.py
--rw-r--r--   0     1001      127     2537 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/calendar_helper/__init__.py
--rw-r--r--   0     1001      127      673 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/display.py
--rw-r--r--   0     1001      127     2540 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/dummy.py
--rw-r--r--   0     1001      127     2851 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/dummy_helper/__init__.py
--rw-r--r--   0     1001      127     1178 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/dummymkt.py
--rw-r--r--   0     1001      127     1633 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/dummymkt_helper/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/expr/__init__.py
--rw-r--r--   0     1001      127     1580 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/expr/random.py
--rw-r--r--   0     1001      127     1213 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures.py
--rw-r--r--   0     1001      127     2307 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures_helper/__init__.py
--rw-r--r--   0     1001      127      850 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures_helper/bbg_symbols.py
--rw-r--r--   0     1001      127     1135 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures_helper/generic_symbols.py
--rw-r--r--   0     1001      127     7751 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures_helper/roll_calendar.py
--rw-r--r--   0     1001      127      890 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/futures_helper/util.py
--rw-r--r--   0     1001      127     4810 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/grouper.py
--rw-r--r--   0     1001      127      510 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/loader.py
--rw-r--r--   0     1001      127     2317 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/resample.py
--rw-r--r--   0     1001      127     3475 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/resample_helper/__init__.py
--rw-r--r--   0     1001      127      876 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/sf.py
--rw-r--r--   0     1001      127      539 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/sf_helper/__init__.py
--rw-r--r--   0     1001      127      684 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/time.py
--rw-r--r--   0     1001      127      937 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/time_helper/__init__.py
--rw-r--r--   0     1001      127      397 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/tsf.py
--rw-r--r--   0     1001      127      397 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/types.py
--rw-r--r--   0     1001      127     1289 2024-04-17 22:55:56.000000 polars_ts-0.0.5/polars_ts/utils.py
--rw-r--r--   0     1001      127       32 2024-04-17 22:55:56.000000 polars_ts-0.0.5/requirements.txt
--rw-r--r--   0     1001      127      445 2024-04-17 22:55:56.000000 polars_ts-0.0.5/ruff.toml
--rw-r--r--   0     1001      127      212 2024-04-17 22:55:56.000000 polars_ts-0.0.5/run.py
--rw-r--r--   0     1001      127     2617 2024-04-17 22:55:56.000000 polars_ts-0.0.5/src/expressions.rs
--rw-r--r--   0     1001      127      382 2024-04-17 22:55:56.000000 polars_ts-0.0.5/src/lib.rs
--rw-r--r--   0     1001      127     1839 2024-04-17 22:55:56.000000 polars_ts-0.0.5/src/math/mod.rs
--rw-r--r--   0     1001      127     2712 2024-04-17 22:55:56.000000 polars_ts-0.0.5/src/utils.rs
--rw-r--r--   0     1001      127        0 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/grouper/__init__.py
--rw-r--r--   0     1001      127     2685 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/grouper/test_grouper.py
--rw-r--r--   0     1001      127        0 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/resample/__init__.py
--rw-r--r--   0     1001      127    10278 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/resample/test_resample.py
--rw-r--r--   0     1001      127       27 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/sf/test_sf.py
--rw-r--r--   0     1001      127      846 2024-04-17 22:55:56.000000 polars_ts-0.0.5/tests/test_rust_templates.py
--rw-r--r--   0     1001      127    36490 2024-04-17 22:55:56.000000 polars_ts-0.0.5/Cargo.lock
--rw-r--r--   0     1001      127      478 2024-04-17 22:55:56.000000 polars_ts-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 polars_ts-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 polars_ts-0.0.6/Cargo.toml
+-rw-r--r--   0     1001      127     3402 2024-04-18 14:22:51.000000 polars_ts-0.0.6/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127     3107 2024-04-18 14:22:51.000000 polars_ts-0.0.6/.gitignore
+-rw-r--r--   0     1001      127        7 2024-04-18 14:22:51.000000 polars_ts-0.0.6/.python-version
+-rw-r--r--   0     1001      127      147 2024-04-18 14:22:51.000000 polars_ts-0.0.6/.vscode/settings.json
+-rw-r--r--   0     1001      127    11357 2024-04-18 14:22:51.000000 polars_ts-0.0.6/LICENSE
+-rw-r--r--   0     1001      127      704 2024-04-18 14:22:51.000000 polars_ts-0.0.6/Makefile
+-rw-r--r--   0     1001      127     1002 2024-04-18 14:22:51.000000 polars_ts-0.0.6/README.md
+-rw-r--r--   0     1001      127      954 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/__init__.py
+-rw-r--r--   0     1001      127     1637 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/calendar.py
+-rw-r--r--   0     1001      127     2537 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/calendar_helper/__init__.py
+-rw-r--r--   0     1001      127      673 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/display.py
+-rw-r--r--   0     1001      127     2540 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/dummy.py
+-rw-r--r--   0     1001      127     2851 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/dummy_helper/__init__.py
+-rw-r--r--   0     1001      127     1178 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/dummymkt.py
+-rw-r--r--   0     1001      127     1633 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/dummymkt_helper/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/expr/__init__.py
+-rw-r--r--   0     1001      127     1580 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/expr/random.py
+-rw-r--r--   0     1001      127     1213 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures.py
+-rw-r--r--   0     1001      127     2307 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures_helper/__init__.py
+-rw-r--r--   0     1001      127      850 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures_helper/bbg_symbols.py
+-rw-r--r--   0     1001      127     1135 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures_helper/generic_symbols.py
+-rw-r--r--   0     1001      127     7751 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures_helper/roll_calendar.py
+-rw-r--r--   0     1001      127      890 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/futures_helper/util.py
+-rw-r--r--   0     1001      127     5258 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/grouper.py
+-rw-r--r--   0     1001      127      510 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/loader.py
+-rw-r--r--   0     1001      127     1633 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/mathx.py
+-rw-r--r--   0     1001      127     1876 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/mathx_helper/__init__.py
+-rw-r--r--   0     1001      127     2437 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/resample.py
+-rw-r--r--   0     1001      127     3118 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/resample_helper/__init__.py
+-rw-r--r--   0     1001      127      770 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/sf.py
+-rw-r--r--   0     1001      127     1495 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/sf_helper/__init__.py
+-rw-r--r--   0     1001      127      684 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/time.py
+-rw-r--r--   0     1001      127      937 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/time_helper/__init__.py
+-rw-r--r--   0     1001      127      397 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/tsf.py
+-rw-r--r--   0     1001      127      459 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/types.py
+-rw-r--r--   0     1001      127     1289 2024-04-18 14:22:51.000000 polars_ts-0.0.6/polars_ts/utils.py
+-rw-r--r--   0     1001      127       32 2024-04-18 14:22:51.000000 polars_ts-0.0.6/requirements.txt
+-rw-r--r--   0     1001      127      445 2024-04-18 14:22:51.000000 polars_ts-0.0.6/ruff.toml
+-rw-r--r--   0     1001      127      212 2024-04-18 14:22:51.000000 polars_ts-0.0.6/run.py
+-rw-r--r--   0     1001      127     2617 2024-04-18 14:22:51.000000 polars_ts-0.0.6/src/expressions.rs
+-rw-r--r--   0     1001      127      382 2024-04-18 14:22:51.000000 polars_ts-0.0.6/src/lib.rs
+-rw-r--r--   0     1001      127     1839 2024-04-18 14:22:51.000000 polars_ts-0.0.6/src/math/mod.rs
+-rw-r--r--   0     1001      127     2712 2024-04-18 14:22:51.000000 polars_ts-0.0.6/src/utils.rs
+-rw-r--r--   0     1001      127      212 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/00_config/roll_config.csv
+-rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/__init__.py
+-rw-r--r--   0     1001      127      146 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/config.py
+-rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/futures/__init__.py
+-rw-r--r--   0     1001      127     2125 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/futures/test_continuous_contract.py
+-rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/grouper/__init__.py
+-rw-r--r--   0     1001      127     2737 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/grouper/test_grouper.py
+-rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/mathx/__init__.py
+-rw-r--r--   0     1001      127    11052 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/mathx/test_cum_sum.py
+-rw-r--r--   0     1001      127    13921 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/mathx/test_diff.py
+-rw-r--r--   0     1001      127     3234 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/mathx/test_ewm_mean.py
+-rw-r--r--   0     1001      127    11395 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/mathx/test_shift.py
+-rw-r--r--   0     1001      127        0 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/resample/__init__.py
+-rw-r--r--   0     1001      127    10278 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/resample/test_resample.py
+-rw-r--r--   0     1001      127     1248 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/sf/test_join.py
+-rw-r--r--   0     1001      127      846 2024-04-18 14:22:51.000000 polars_ts-0.0.6/tests/test_rust_templates.py
+-rw-r--r--   0     1001      127    36490 2024-04-18 14:22:51.000000 polars_ts-0.0.6/Cargo.lock
+-rw-r--r--   0     1001      127      478 2024-04-18 14:22:51.000000 polars_ts-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 polars_ts-0.0.6/PKG-INFO
```

### Comparing `polars_ts-0.0.5/Cargo.toml` & `polars_ts-0.0.6/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "polars-ts"
-version = "0.0.5"
+version = "0.0.6"
 edition = "2021"
 
 [lib]
 name = "polars_ts"
 crate-type= ["cdylib"]
 
 [dependencies]
```

### Comparing `polars_ts-0.0.5/.github/workflows/publish_to_pypi.yml` & `polars_ts-0.0.6/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/.gitignore` & `polars_ts-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/LICENSE` & `polars_ts-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/Makefile` & `polars_ts-0.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/README.md` & `polars_ts-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/__init__.py` & `polars_ts-0.0.6/polars_ts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from .display import *
 from .sf import *
 from .tsf import *
 from .loader import *
 from .time import *
 from .dummy import *
+from .mathx import *
 from .resample import *
 
 from .calendar import *
 from .futures import *
 from .dummymkt import *
 
 pl.enable_string_cache()
```

### Comparing `polars_ts-0.0.5/polars_ts/calendar.py` & `polars_ts-0.0.6/polars_ts/calendar.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/calendar_helper/__init__.py` & `polars_ts-0.0.6/polars_ts/calendar_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/display.py` & `polars_ts-0.0.6/polars_ts/display.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/dummy.py` & `polars_ts-0.0.6/polars_ts/dummy.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/dummy_helper/__init__.py` & `polars_ts-0.0.6/polars_ts/dummy_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/dummymkt.py` & `polars_ts-0.0.6/polars_ts/dummymkt.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/dummymkt_helper/__init__.py` & `polars_ts-0.0.6/polars_ts/dummymkt_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/expr/random.py` & `polars_ts-0.0.6/polars_ts/expr/random.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/futures.py` & `polars_ts-0.0.6/polars_ts/futures.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/futures_helper/__init__.py` & `polars_ts-0.0.6/polars_ts/futures_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/futures_helper/bbg_symbols.py` & `polars_ts-0.0.6/polars_ts/futures_helper/bbg_symbols.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/futures_helper/generic_symbols.py` & `polars_ts-0.0.6/polars_ts/futures_helper/generic_symbols.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/futures_helper/roll_calendar.py` & `polars_ts-0.0.6/polars_ts/futures_helper/roll_calendar.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/futures_helper/util.py` & `polars_ts-0.0.6/polars_ts/futures_helper/util.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/grouper.py` & `polars_ts-0.0.6/polars_ts/grouper.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,61 +69,76 @@
         g = Grouper()
         g._all = True
         g._result_includes_time = True
         g._has_defined_spec = True
         return g
 
     @staticmethod
-    def by_common() -> "Grouper":
+    def by_common_excluding_time() -> "Grouper":
         g = Grouper()
         g._common = True
         g._has_defined_spec = True
         return g
 
     @staticmethod
-    def by_time_and_common() -> "Grouper":
+    def by_common_including_time() -> "Grouper":
         g = Grouper()
         g._common = True
         g._result_includes_time = True
         g._has_defined_spec = True
         return g
 
     @staticmethod
-    def _get_common_categories_without_time(
-        lhs: FrameType, rhs: FrameType
+    def common_categories(
+        lhs: FrameType, rhs: FrameType, include_time: bool = False
     ) -> List[str]:
-        cat_lhs = Grouper._get_categories_without_time(lhs)
-        cat_rhs = Grouper._get_categories_without_time(rhs)
-        common = set(cat_lhs).intersection(cat_rhs)
+        cat_lhs = Grouper.categories(lhs, include_time)
+        cat_rhs = Grouper.categories(rhs, include_time)
+        cols = set(cat_lhs).intersection(cat_rhs)
 
-        return sorted(common)
+        return sorted(cols)
 
     @staticmethod
-    def _get_categories_without_time(df: FrameType) -> List[str]:
-        return df.select(pl.col(pl.Categorical, pl.Enum)).columns
+    def categories(df: FrameType, include_time: bool) -> List[str]:
+        cols = df.select(pl.col(pl.Categorical, pl.Enum)).columns
+        if include_time:
+            cols = ["time"] + sorted(cols)
+
+        return cols
+
+    @staticmethod
+    def values(df: FrameType) -> List[str]:
+        cats = set(Grouper.categories(df, include_time=True))
+        cols = set(df.columns).difference(cats)
+        return sorted(cols)
+
+    @staticmethod
+    def numerics(df: FrameType) -> List[str]:
+        cols = df.select(pl.col(pl.NUMERIC_DTYPES)).columns
+        return sorted(cols)
 
     def apply(self, *dfs: FrameType) -> List[str]:
         if self._common and len(dfs) < 2:
             raise ValueError("Require at least 2 dataframes when 'common' flag is set.")
 
         if not self._common and len(dfs) != 1:
             raise ValueError("Too many arguments passed to apply.")
 
         if self._common:
             df = dfs[0]
             df_other = dfs[1]
             df_has_time = ("time" in df) and ("time" in df_other)
-            cols = set(Grouper._get_common_categories_without_time(df, df_other))
+            cols = set(Grouper.common_categories(df, df_other))
         else:
             if not self._has_defined_spec:
                 self._all = True
 
             df = dfs[0]
             df_has_time = "time" in df
-            cols = set(Grouper._get_categories_without_time(df))
+            cols = set(Grouper.categories(df, include_time=False))
 
             if len(self._by) > 0:
                 cols = cols.intersection(self._by)
             elif len(self._omitting) > 0:
                 cols = cols.difference(self._omitting)
             elif self._all:
                 pass
```

### Comparing `polars_ts-0.0.5/polars_ts/resample.py` & `polars_ts-0.0.6/polars_ts/resample.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     impl_resample_categories,
 )
 
 from .grouper import Grouper
 from .tsf import TimeSeriesFrame
 from .types import (
     IntervalType,
-    FillStrategyType,
+    NullStrategyType,
     FrameType,
 )
 
 __NAMESPACE = "rs"
 
 
 @pl.api.register_lazyframe_namespace(__NAMESPACE)
@@ -49,19 +49,19 @@
         return prepare_result(df)
 
     def align_to_time(
         self,
         time_axis: pl.Series,
         partition: Grouper = Grouper(),
         closed: IntervalType = "left",
-        fill_strategy: FillStrategyType = "forward",
-        fill_sentinel: Union[float, int] = 0.0,
+        null_strategy: NullStrategyType = "forward",
+        null_sentinel_numeric: Union[float, int] = 0.0,
     ) -> FrameType:
         df = impl_align_to_time(
-            self._df, time_axis, partition, closed, fill_strategy, fill_sentinel
+            self._df, time_axis, partition, closed, null_strategy, null_sentinel_numeric
         )
 
         return prepare_result(df)
 
     def resample_categories(
         self,
         time_axis: pl.Series,
@@ -71,17 +71,22 @@
         df = impl_resample_categories(self._df, time_axis, partition, closed)
 
         return prepare_result(df)
 
     def align_values(
         self,
         rhs: FrameType,
-        partition: Grouper = Grouper(),
+        partition: Grouper = Grouper().by_common_including_time(),
         retain_values: Literal["lhs", "rhs", "both"] = "lhs",
-        fill_strategy: FillStrategyType = "forward",
-        fill_sentinel: Union[float, int] = 0.0,
+        null_strategy: NullStrategyType = "forward",
+        null_sentinel_numeric: Union[float, int] = 0.0,
     ) -> FrameType:
         df = impl_align_values(
-            self._df, rhs, partition, retain_values, fill_strategy, fill_sentinel
+            self._df,
+            rhs,
+            partition,
+            retain_values,
+            null_strategy,
+            null_sentinel_numeric,
         )
 
         return prepare_result(df)
```

### Comparing `polars_ts-0.0.5/polars_ts/resample_helper/__init__.py` & `polars_ts-0.0.6/polars_ts/resample_helper/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from typing import Union, List
 
 import polars as pl
 
-from ..sf_helper import impl_categories
+from ..sf_helper import impl_apply_null_strategy
 from ..grouper import Grouper
 
 from ..types import (
     IntervalType,
-    FillStrategyType,
+    NullStrategyType,
     RetainValuesType,
     FrameType,
 )
 
 
 def impl_align_to_time(
     df: FrameType,
     time_axis: pl.Series,
     partition: Grouper,
     closed: IntervalType,
-    fill_strategy: FillStrategyType,
-    fill_sentinel: Union[float, int],
+    null_strategy: NullStrategyType,
+    null_sentinel_numeric: Union[float, int],
 ) -> FrameType:
     resampled = impl_resample_categories(df, time_axis, partition, closed)
     realigned = impl_align_values(
         df,
         resampled,
         partition,
         retain_values="lhs",
-        fill_strategy=fill_strategy,
-        fill_sentinel=fill_sentinel,
+        null_strategy=null_strategy,
+        null_sentinel_numeric=null_sentinel_numeric,
     )
 
     return realigned
 
 
 def impl_resample_categories(
     df: FrameType,
@@ -71,54 +71,42 @@
 
 
 def impl_align_values(
     lhs: FrameType,
     rhs: FrameType,
     partition: Grouper,
     retain_values: RetainValuesType,
-    fill_strategy: FillStrategyType,
-    fill_sentinel: Union[float, int],
+    null_strategy: NullStrategyType,
+    null_sentinel_numeric: Union[float, int],
 ) -> FrameType:
+    rhs_cat_cols = Grouper.categories(rhs, include_time=True)
+    rhs_grid = rhs.select(rhs_cat_cols)
+
     if retain_values == "lhs":
         # strip away rhs values
-        rhs = impl_categories(rhs, include_time=True)
+        rhs = rhs_grid
 
     if retain_values == "rhs":
         # strip away lhs values
-        lhs = impl_categories(lhs, include_time=True)
+        lhs_cat_cols = Grouper.categories(lhs, include_time=True)
+        lhs = lhs.select(lhs_cat_cols)
 
     assert isinstance(lhs, type(rhs)) and (
         isinstance(lhs, pl.LazyFrame) or isinstance(lhs, pl.DataFrame)
     )
 
-    grouper_cols: List[str] = partition.by_common().apply(lhs, rhs)
+    grouper_cols: List[str] = partition.apply(lhs, rhs)
 
     result = (
         lhs.join(rhs, on=["time", *grouper_cols], how="outer_coalesce")
         .filter(pl.col("time").is_not_null())
         .sort("time", *grouper_cols)
         .unique(keep="first", maintain_order=True)
     )
 
-    if fill_strategy == "sentinel":
-        result = result.with_columns(pl.col(pl.NUMERIC_DTYPES).fill_null(fill_sentinel))
-
-    elif fill_strategy == "forward":
-        result = result.with_columns(
-            pl.exclude("time").forward_fill().over(grouper_cols)
-        )
-
-    elif fill_strategy == "backward":
-        result = result.with_columns(
-            pl.exclude("time").backward_fill().over(grouper_cols)
-        )
-
-    elif fill_strategy == "none":
-        pass
-
-    else:
-        raise ValueError(f"Unexpected fill strategy: {fill_strategy}")
+    result = impl_apply_null_strategy(
+        result, null_strategy, null_sentinel_numeric, partition
+    )
 
-    rhs_grid = impl_categories(rhs, include_time=True)
-    result = result.join(rhs_grid, on=rhs_grid.columns, how="inner")
+    result = result.join(rhs_grid, on=rhs_cat_cols, how="inner")
 
     return result
```

### Comparing `polars_ts-0.0.5/polars_ts/time.py` & `polars_ts-0.0.6/polars_ts/time.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/time_helper/__init__.py` & `polars_ts-0.0.6/polars_ts/time_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/polars_ts/utils.py` & `polars_ts-0.0.6/polars_ts/utils.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/src/expressions.rs` & `polars_ts-0.0.6/src/expressions.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/src/math/mod.rs` & `polars_ts-0.0.6/src/math/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/src/utils.rs` & `polars_ts-0.0.6/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/tests/grouper/test_grouper.py` & `polars_ts-0.0.6/tests/grouper/test_grouper.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,20 @@
 
     assert Grouper.omitting_time_and("catsa").apply(df) == ["catsb"]
     assert Grouper.omitting_time_and("time", "catsa").apply(df) == ["catsb"]
 
     assert Grouper.by_all().apply(df) == ["catsa", "catsb"]
     assert Grouper.by_time_and_all().apply(df) == ["time", "catsa", "catsb"]
 
-    assert Grouper.by_common().apply(df, df) == ["catsa", "catsb"]
-    assert Grouper.by_time_and_common().apply(df, df) == ["time", "catsa", "catsb"]
+    assert Grouper.by_common_excluding_time().apply(df, df) == ["catsa", "catsb"]
+    assert Grouper.by_common_including_time().apply(df, df) == [
+        "time",
+        "catsa",
+        "catsb",
+    ]
 
     with pytest.raises(ValueError, match="Empty Grouper Specification"):
         assert Grouper.omitting_time_and("catsa", "catsb").apply(df) == []
 
     with pytest.raises(ValueError, match="Empty Grouper Specification"):
         assert Grouper.omitting("time", "catsa", "catsb").apply(df) == []
```

### Comparing `polars_ts-0.0.5/tests/resample/test_resample.py` & `polars_ts-0.0.6/tests/resample/test_resample.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/tests/test_rust_templates.py` & `polars_ts-0.0.6/tests/test_rust_templates.py`

 * *Files identical despite different names*

### Comparing `polars_ts-0.0.5/Cargo.lock` & `polars_ts-0.0.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -671,15 +671,15 @@
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-ts"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
  "jemallocator",
  "polars",
  "pyo3",
  "pyo3-polars",
  "rand",
  "rand_distr",
```

### Comparing `polars_ts-0.0.5/PKG-INFO` & `polars_ts-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-ts
-Version: 0.0.5
+Version: 0.0.6
 Requires-Dist: polars >=0.20.21
 Requires-Dist: polars-xdt
 Requires-Dist: hvplot
 Requires-Dist: pyarrow
 Requires-Dist: hvplot ; extra == 'dev'
 Requires-Dist: pyarrow ; extra == 'dev'
 Provides-Extra: dev
```

