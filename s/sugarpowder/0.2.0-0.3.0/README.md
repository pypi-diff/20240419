# Comparing `tmp/sugarpowder-0.2.0.tar.gz` & `tmp/sugarpowder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sugarpowder-0.2.0.tar", last modified: Thu Mar 14 01:39:37 2024, max compression
+gzip compressed data, was "sugarpowder-0.3.0.tar", last modified: Fri Apr 19 07:17:53 2024, max compression
```

## Comparing `sugarpowder-0.2.0.tar` & `sugarpowder-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-03-14 01:39:37.101122 sugarpowder-0.2.0/
--rw-r--r--   0 docker    (1000) docker    (1000)     1083 2023-05-31 23:29:34.000000 sugarpowder-0.2.0/LICENSE
--rw-r--r--   0 docker    (1000) docker    (1000)     2442 2024-03-14 01:39:37.101122 sugarpowder-0.2.0/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)      601 2024-01-25 08:26:57.000000 sugarpowder-0.2.0/README.md
--rw-r--r--   0 docker    (1000) docker    (1000)      731 2024-03-14 01:31:00.000000 sugarpowder-0.2.0/pyproject.toml
--rw-r--r--   0 docker    (1000) docker    (1000)       38 2024-03-14 01:39:37.101122 sugarpowder-0.2.0/setup.cfg
--rw-r--r--   0 docker    (1000) docker    (1000)       70 2024-03-14 01:30:53.000000 sugarpowder-0.2.0/setup.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-03-14 01:39:37.101122 sugarpowder-0.2.0/src/
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-03-14 01:39:37.101122 sugarpowder-0.2.0/src/sugarpowder/
--rw-r--r--   0 docker    (1000) docker    (1000)      100 2023-05-31 23:41:04.000000 sugarpowder-0.2.0/src/sugarpowder/__init__.py
--rw-r--r--   0 docker    (1000) docker    (1000)      163 2024-03-14 01:36:51.000000 sugarpowder-0.2.0/src/sugarpowder/dates.py
--rw-r--r--   0 docker    (1000) docker    (1000)      239 2023-06-19 02:47:01.000000 sugarpowder-0.2.0/src/sugarpowder/mark_time.py
--rw-r--r--   0 docker    (1000) docker    (1000)     5322 2024-03-14 01:35:30.000000 sugarpowder-0.2.0/src/sugarpowder/pipes.py
--rw-r--r--   0 docker    (1000) docker    (1000)      645 2024-03-14 01:33:56.000000 sugarpowder-0.2.0/src/sugarpowder/utils.py
--rw-r--r--   0 docker    (1000) docker    (1000)     1049 2024-03-14 01:35:49.000000 sugarpowder-0.2.0/src/sugarpowder/witherr.py
-drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-03-14 01:39:37.101122 sugarpowder-0.2.0/src/sugarpowder.egg-info/
--rw-r--r--   0 docker    (1000) docker    (1000)     2442 2024-03-14 01:39:37.000000 sugarpowder-0.2.0/src/sugarpowder.egg-info/PKG-INFO
--rw-r--r--   0 docker    (1000) docker    (1000)      406 2024-03-14 01:39:37.000000 sugarpowder-0.2.0/src/sugarpowder.egg-info/SOURCES.txt
--rw-r--r--   0 docker    (1000) docker    (1000)        1 2024-03-14 01:39:37.000000 sugarpowder-0.2.0/src/sugarpowder.egg-info/dependency_links.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       22 2024-03-14 01:39:37.000000 sugarpowder-0.2.0/src/sugarpowder.egg-info/requires.txt
--rw-r--r--   0 docker    (1000) docker    (1000)       17 2024-03-14 01:39:37.000000 sugarpowder-0.2.0/src/sugarpowder.egg-info/top_level.txt
--rw-r--r--   0 docker    (1000) docker    (1000)     1798 2024-01-26 00:47:26.000000 sugarpowder-0.2.0/src/test.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-04-19 07:17:53.410915 sugarpowder-0.3.0/
+-rw-r--r--   0 docker    (1000) docker    (1000)     1083 2023-05-31 23:29:34.000000 sugarpowder-0.3.0/LICENSE
+-rw-r--r--   0 docker    (1000) docker    (1000)     2447 2024-04-19 07:17:53.410915 sugarpowder-0.3.0/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)      601 2024-01-25 08:26:57.000000 sugarpowder-0.3.0/README.md
+-rw-r--r--   0 docker    (1000) docker    (1000)      736 2024-04-19 07:17:06.000000 sugarpowder-0.3.0/pyproject.toml
+-rw-r--r--   0 docker    (1000) docker    (1000)       38 2024-04-19 07:17:53.410915 sugarpowder-0.3.0/setup.cfg
+-rw-r--r--   0 docker    (1000) docker    (1000)       70 2024-03-14 01:30:53.000000 sugarpowder-0.3.0/setup.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-04-19 07:17:53.410915 sugarpowder-0.3.0/src/
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-04-19 07:17:53.410915 sugarpowder-0.3.0/src/sugarpowder/
+-rw-r--r--   0 docker    (1000) docker    (1000)      100 2023-05-31 23:41:04.000000 sugarpowder-0.3.0/src/sugarpowder/__init__.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      163 2024-03-14 01:36:51.000000 sugarpowder-0.3.0/src/sugarpowder/dates.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      239 2023-06-19 02:47:01.000000 sugarpowder-0.3.0/src/sugarpowder/mark_time.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     5322 2024-03-25 00:37:55.000000 sugarpowder-0.3.0/src/sugarpowder/pipes.py
+-rw-r--r--   0 docker    (1000) docker    (1000)      875 2024-04-19 07:14:39.000000 sugarpowder-0.3.0/src/sugarpowder/utils.py
+-rw-r--r--   0 docker    (1000) docker    (1000)     1049 2024-03-14 01:35:49.000000 sugarpowder-0.3.0/src/sugarpowder/witherr.py
+drwxr-xr-x   0 docker    (1000) docker    (1000)        0 2024-04-19 07:17:53.410915 sugarpowder-0.3.0/src/sugarpowder.egg-info/
+-rw-r--r--   0 docker    (1000) docker    (1000)     2447 2024-04-19 07:17:53.000000 sugarpowder-0.3.0/src/sugarpowder.egg-info/PKG-INFO
+-rw-r--r--   0 docker    (1000) docker    (1000)      406 2024-04-19 07:17:53.000000 sugarpowder-0.3.0/src/sugarpowder.egg-info/SOURCES.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)        1 2024-04-19 07:17:53.000000 sugarpowder-0.3.0/src/sugarpowder.egg-info/dependency_links.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       22 2024-04-19 07:17:53.000000 sugarpowder-0.3.0/src/sugarpowder.egg-info/requires.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)       17 2024-04-19 07:17:53.000000 sugarpowder-0.3.0/src/sugarpowder.egg-info/top_level.txt
+-rw-r--r--   0 docker    (1000) docker    (1000)     1894 2024-04-19 07:16:56.000000 sugarpowder-0.3.0/src/test.py
```

### Comparing `sugarpowder-0.2.0/LICENSE` & `sugarpowder-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sugarpowder-0.2.0/PKG-INFO` & `sugarpowder-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sugarpowder
-Version: 0.2.0
+Version: 0.3.0
 Summary: Package of Python syntactic sugars inspired by Elixir, Go, Rust, Julia, and other languages
 Author-email: Geunseong Jung <dreamwayjgs@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Geunseong Jung (정근성)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/dreamwayjgs/sugarpowder
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Bug Tracker, https://github.com/dreamwayjgs/sugarpowder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sugarpowder-0.2.0/README.md` & `sugarpowder-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sugarpowder-0.2.0/pyproject.toml` & `sugarpowder-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sugarpowder"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Geunseong Jung", email="dreamwayjgs@gmail.com" },
 ]
 description = "Package of Python syntactic sugars inspired by Elixir, Go, Rust, Julia, and other languages"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
@@ -20,8 +20,8 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/dreamwayjgs/sugarpowder"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Bug Tracker" = "https://github.com/dreamwayjgs/sugarpowder/issues"
```

### Comparing `sugarpowder-0.2.0/src/sugarpowder/pipes.py` & `sugarpowder-0.3.0/src/sugarpowder/pipes.py`

 * *Files identical despite different names*

### Comparing `sugarpowder-0.2.0/src/sugarpowder/utils.py` & `sugarpowder-0.3.0/src/sugarpowder/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from io import BytesIO
 from typing import Iterable, TypeVar
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 def df_to_parquetstream(df: pd.DataFrame) -> bytes:
     pqstream = BytesIO()
     pq.write_table(pa.Table.from_pandas(df), pqstream)
     pqbytes = pqstream.getvalue()
     return pqbytes
 
 
 def parquetstream_to_df(pqbytes: bytes) -> pd.DataFrame:
     pqstream = BytesIO(pqbytes)
     pqtable = pq.read_table(pqstream)
-
     return pqtable.to_pandas()
 
 
+def df_to_hex(df: pd.DataFrame) -> str:
+    pqbytes = df_to_parquetstream(df)
+    return pqbytes.hex()
+
+
+def hex_to_df(hexed_df: str) -> pd.DataFrame:
+    pqbytes = bytes.fromhex(hexed_df)
+    return parquetstream_to_df(pqbytes)
+
+
 def deduplist(seq: Iterable[T], keep_order=True) -> list[T]:
     if keep_order:
         return list(dict.fromkeys(seq))
     return list(set(seq))
```

### Comparing `sugarpowder-0.2.0/src/sugarpowder/witherr.py` & `sugarpowder-0.3.0/src/sugarpowder/witherr.py`

 * *Files identical despite different names*

### Comparing `sugarpowder-0.2.0/src/sugarpowder.egg-info/PKG-INFO` & `sugarpowder-0.3.0/src/sugarpowder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sugarpowder
-Version: 0.2.0
+Version: 0.3.0
 Summary: Package of Python syntactic sugars inspired by Elixir, Go, Rust, Julia, and other languages
 Author-email: Geunseong Jung <dreamwayjgs@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Geunseong Jung (정근성)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,15 +22,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/dreamwayjgs/sugarpowder
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Bug Tracker, https://github.com/dreamwayjgs/sugarpowder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sugarpowder-0.2.0/src/test.py` & `sugarpowder-0.3.0/src/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sugarpowder.witherr import witherr, Witherr
 from sugarpowder.pipes import take, select, where, tolist, tail
 from sugarpowder.mark_time import mark_time
-from sugarpowder.utils import df_to_parquetstream, parquetstream_to_df
+from sugarpowder.utils import df_to_hex, df_to_parquetstream, hex_to_df, parquetstream_to_df
 from datetime import datetime
 import pandas as pd
 from pandas.testing import assert_frame_equal
 
 
 @witherr
 def div1(x: float, y: float) -> float:
@@ -59,17 +59,20 @@
     Y = ["a", "b", "c", "d"]
     Z = [datetime(2020, 1, 1), datetime(2020, 1, 2), datetime(2020, 1, 3), datetime(2020, 1, 4)]
 
     df = pd.DataFrame({"X": X, "Y": Y, "Z": Z})
     pq = df_to_parquetstream(df)
     ndf = parquetstream_to_df(pq)
 
+    dfhex = df_to_hex(df)
+    hexdf = hex_to_df(dfhex)
+
     try:
         assert_frame_equal(df, ndf)
-        assert True
+        assert_frame_equal(df, hexdf)
     except:
         assert False, "Frame Eqaul Failed"
 
 
 if __name__ == "__main__":
     print("Run Tests")
     s = mark_time()
```

