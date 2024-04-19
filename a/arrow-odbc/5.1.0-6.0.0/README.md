# Comparing `tmp/arrow_odbc-5.1.0.tar.gz` & `tmp/arrow_odbc-6.0.0.tar.gz`

## Comparing `arrow_odbc-5.1.0.tar` & `arrow_odbc-6.0.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 arrow_odbc-5.1.0/Cargo.toml
--rw-r--r--   0      501       20      136 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.gitattributes
--rw-r--r--   0      501       20      213 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.github/dependabot.yml
--rw-r--r--   0      501       20     1762 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.github/workflows/test.yml
--rw-r--r--   0      501       20     2648 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.github/workflows/wheel.yml
--rw-r--r--   0      501       20      286 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.gitignore
--rw-r--r--   0      501       20      841 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/.readthedocs.yaml
--rw-r--r--   0      501       20    11859 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/Changelog.md
--rw-r--r--   0      501       20     1954 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/Contributing.md
--rw-r--r--   0      501       20     1069 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/LICENSE
--rw-r--r--   0      501       20     7988 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/README.md
--rw-r--r--   0      501       20       14 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/cbindgen.toml
--rw-r--r--   0      501       20      623 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/conftest.py
--rw-r--r--   0      501       20      638 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/Makefile
--rw-r--r--   0      501       20      804 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/make.bat
--rw-r--r--   0      501       20       16 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/requirements.txt
--rw-r--r--   0      501       20      155 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/source/arrow_odbc.rst
--rw-r--r--   0      501       20     1965 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/source/conf.py
--rw-r--r--   0      501       20      458 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/source/index.rst
--rw-r--r--   0      501       20       67 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/doc/source/modules.rst
--rw-r--r--   0      501       20      348 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/docker-compose.yml
--rw-r--r--   0      501       20      564 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/manylinux/Dockerfile
--rw-r--r--   0      501       20      121 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/manylinux/Readme.md
--rw-r--r--   0      501       20      148 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/manylinux/WHEEL
--rw-r--r--   0      501       20     1256 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/manylinux/build_wheel.sh
--rw-r--r--   0      501       20      446 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/__init__.py
--rw-r--r--   0      501       20     1946 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/connect.py
--rw-r--r--   0      501       20      672 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/error.py
--rw-r--r--   0      501       20      788 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/log.py
--rw-r--r--   0      501       20      578 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/pool.py
--rw-r--r--   0      501       20    25180 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/reader.py
--rw-r--r--   0      501       20     9625 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/python/arrow_odbc/writer.py
--rw-r--r--   0      501       20     2322 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/error.rs
--rw-r--r--   0      501       20     3434 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/lib.rs
--rw-r--r--   0      501       20      655 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/logging.rs
--rw-r--r--   0      501       20     1239 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/parameter.rs
--rw-r--r--   0      501       20      421 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/pool.rs
--rw-r--r--   0      501       20     8757 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/reader/arrow_odbc_reader.rs
--rw-r--r--   0      501       20    12865 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/reader.rs
--rw-r--r--   0      501       20     3545 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/src/writer.rs
--rw-r--r--   0      501       20   274432 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/temp_db.duckdb
--rw-r--r--   0      501       20        0 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/tests/__init__.py
--rw-r--r--   0      501       20     4115 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/tests/iris.csv
--rw-r--r--   0      501       20     2413 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/tests/iris.parquet
--rw-r--r--   0      501       20    29032 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/tests/test_arrow_odbc.py
--rw-r--r--   0      501       20    43514 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/Cargo.lock
--rw-r--r--   0      501       20      825 2024-04-08 22:09:47.000000 arrow_odbc-5.1.0/pyproject.toml
--rw-r--r--   0        0        0     8600 1970-01-01 00:00:00.000000 arrow_odbc-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 arrow_odbc-6.0.0/Cargo.toml
+-rw-r--r--   0      501       20      136 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.gitattributes
+-rw-r--r--   0      501       20      213 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.github/dependabot.yml
+-rw-r--r--   0      501       20     1762 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.github/workflows/test.yml
+-rw-r--r--   0      501       20     2648 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.github/workflows/wheel.yml
+-rw-r--r--   0      501       20      286 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.gitignore
+-rw-r--r--   0      501       20      841 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/.readthedocs.yaml
+-rw-r--r--   0      501       20    11859 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/Changelog.md
+-rw-r--r--   0      501       20     1954 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/Contributing.md
+-rw-r--r--   0      501       20     1069 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/LICENSE
+-rw-r--r--   0      501       20     7988 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/README.md
+-rw-r--r--   0      501       20       14 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/cbindgen.toml
+-rw-r--r--   0      501       20      623 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/conftest.py
+-rw-r--r--   0      501       20      638 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/Makefile
+-rw-r--r--   0      501       20      804 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/make.bat
+-rw-r--r--   0      501       20       16 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/requirements.txt
+-rw-r--r--   0      501       20      155 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/source/arrow_odbc.rst
+-rw-r--r--   0      501       20     1965 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/source/conf.py
+-rw-r--r--   0      501       20      458 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/source/index.rst
+-rw-r--r--   0      501       20       67 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/doc/source/modules.rst
+-rw-r--r--   0      501       20      348 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/docker-compose.yml
+-rw-r--r--   0      501       20      564 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/manylinux/Dockerfile
+-rw-r--r--   0      501       20      121 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/manylinux/Readme.md
+-rw-r--r--   0      501       20      148 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/manylinux/WHEEL
+-rw-r--r--   0      501       20     1256 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/manylinux/build_wheel.sh
+-rw-r--r--   0      501       20      446 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/__init__.py
+-rw-r--r--   0      501       20     1946 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/connect.py
+-rw-r--r--   0      501       20      672 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/error.py
+-rw-r--r--   0      501       20      788 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/log.py
+-rw-r--r--   0      501       20      578 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/pool.py
+-rw-r--r--   0      501       20    25180 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/reader.py
+-rw-r--r--   0      501       20     9625 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/python/arrow_odbc/writer.py
+-rw-r--r--   0      501       20     2322 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/error.rs
+-rw-r--r--   0      501       20     3434 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/lib.rs
+-rw-r--r--   0      501       20      655 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/logging.rs
+-rw-r--r--   0      501       20     1239 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/parameter.rs
+-rw-r--r--   0      501       20      421 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/pool.rs
+-rw-r--r--   0      501       20     8757 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/reader/arrow_odbc_reader.rs
+-rw-r--r--   0      501       20    12865 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/reader.rs
+-rw-r--r--   0      501       20     3545 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/src/writer.rs
+-rw-r--r--   0      501       20   274432 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/temp_db.duckdb
+-rw-r--r--   0      501       20        0 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/tests/__init__.py
+-rw-r--r--   0      501       20     4115 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/tests/iris.csv
+-rw-r--r--   0      501       20     2413 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/tests/iris.parquet
+-rw-r--r--   0      501       20    29032 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/tests/test_arrow_odbc.py
+-rw-r--r--   0      501       20    43744 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/Cargo.lock
+-rw-r--r--   0      501       20      825 2024-04-19 21:29:26.000000 arrow_odbc-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8600 1970-01-01 00:00:00.000000 arrow_odbc-6.0.0/PKG-INFO
```

### Comparing `arrow_odbc-5.1.0/Cargo.toml` & `arrow_odbc-6.0.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [lib]
 # Name needs to be identical to python package name
 name = "arrow_odbc"
 crate-type = ["cdylib"]
 
 [dependencies]
-arrow-odbc = "8.3.0"
+arrow-odbc = "9.0.0"
 # arrow would be included indirectly using arrow-odbc, but we need to explicitly specify the ffi
 # feature.
 arrow = { version = "51.0.0", default-features = false, features = ["ffi"] }
 stderrlog = "0.6.0"
 log = "0.4.21"
 
 [profile.release]
```

### Comparing `arrow_odbc-5.1.0/.github/workflows/test.yml` & `arrow_odbc-6.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/.github/workflows/wheel.yml` & `arrow_odbc-6.0.0/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/.readthedocs.yaml` & `arrow_odbc-6.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/Changelog.md` & `arrow_odbc-6.0.0/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changelog
 
-## 5.1.0
+## 6.0.0
 
 - Support for passing desired packet size to the ODBC driver. This may help with packet loss on fragile connections if the ODBC driver supports it.
 
 ## 5.0.0
 
 - Fix: Database connection have not been cleaned up in case the parameters caused a type error.
 - Changend `BatchReader.to_pyarrow_record_batch_reader` into `BatchReader.into_pyarrow_record_batch_reader`. The new method fully passes ownership and leaves self empty.
```

### Comparing `arrow_odbc-5.1.0/Contributing.md` & `arrow_odbc-6.0.0/Contributing.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/LICENSE` & `arrow_odbc-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/README.md` & `arrow_odbc-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/conftest.py` & `arrow_odbc-6.0.0/conftest.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/doc/Makefile` & `arrow_odbc-6.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/doc/make.bat` & `arrow_odbc-6.0.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/doc/source/conf.py` & `arrow_odbc-6.0.0/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "arrow-odbc"
 copyright = "2021, Markus Klein"
 author = "Markus Klein"
 
 # The full version, including alpha/beta/rc tags
-release = "5.1.0"
+release = "6.0.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `arrow_odbc-5.1.0/manylinux/Dockerfile` & `arrow_odbc-6.0.0/manylinux/Dockerfile`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/manylinux/build_wheel.sh` & `arrow_odbc-6.0.0/manylinux/build_wheel.sh`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/python/arrow_odbc/connect.py` & `arrow_odbc-6.0.0/python/arrow_odbc/connect.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/python/arrow_odbc/error.py` & `arrow_odbc-6.0.0/python/arrow_odbc/error.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/python/arrow_odbc/log.py` & `arrow_odbc-6.0.0/python/arrow_odbc/log.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/python/arrow_odbc/pool.py` & `arrow_odbc-6.0.0/python/arrow_odbc/pool.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/python/arrow_odbc/reader.py` & `arrow_odbc-6.0.0/python/arrow_odbc/reader.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/python/arrow_odbc/writer.py` & `arrow_odbc-6.0.0/python/arrow_odbc/writer.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/src/error.rs` & `arrow_odbc-6.0.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/src/lib.rs` & `arrow_odbc-6.0.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/src/logging.rs` & `arrow_odbc-6.0.0/src/logging.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/src/parameter.rs` & `arrow_odbc-6.0.0/src/parameter.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/src/reader/arrow_odbc_reader.rs` & `arrow_odbc-6.0.0/src/reader/arrow_odbc_reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/src/reader.rs` & `arrow_odbc-6.0.0/src/reader.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/src/writer.rs` & `arrow_odbc-6.0.0/src/writer.rs`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/temp_db.duckdb` & `arrow_odbc-6.0.0/temp_db.duckdb`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/tests/iris.csv` & `arrow_odbc-6.0.0/tests/iris.csv`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/tests/iris.parquet` & `arrow_odbc-6.0.0/tests/iris.parquet`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/tests/test_arrow_odbc.py` & `arrow_odbc-6.0.0/tests/test_arrow_odbc.py`

 * *Files identical despite different names*

### Comparing `arrow_odbc-5.1.0/Cargo.lock` & `arrow_odbc-6.0.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -157,17 +157,17 @@
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-odbc"
-version = "8.3.0"
+version = "9.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d3e4f078ec0150fdc62b742b1866e3fdc3b792430ca3e6ca6468adfe8af44e0"
+checksum = "44c0f42b7fff9cdd6fcc1ba5a955b5e233ef645d5fe4b636b372e9bb4d36214a"
 dependencies = [
  "arrow",
  "chrono",
  "log",
  "odbc-api",
  "thiserror",
 ]
@@ -334,17 +334,17 @@
  "rustix",
  "slab",
  "thiserror",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.92"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
+checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cesu8"
@@ -362,31 +362,31 @@
 name = "cfg_aliases"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "combine"
-version = "4.6.6"
+version = "4.6.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
+checksum = "ba5a308b75df32fe02788e748662718f03fde005016435c444eea572398219fd"
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "concurrent-queue"
@@ -642,17 +642,17 @@
 name = "jni-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8eaf4bc02d17cbdd7ff4c7438cafcdf7fb9a4613313ad11b4f8fefe7d3fa0130"
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -735,15 +735,15 @@
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
@@ -805,17 +805,17 @@
 checksum = "8c196769dd60fd4f363e11d948139556a344e79d451aeb2fa2fd040738ef7691"
 dependencies = [
  "jni-sys",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "3135b08af27d103b0a51f2ae0f8632117b7b185ccf931445affa8df530576a41"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
@@ -902,17 +902,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "objc-sys"
-version = "0.3.2"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7c71324e4180d0899963fc83d9d241ac39e699609fc1025a850aadac8257459"
+checksum = "da284c198fb9b7b0603f8635185e85fbd5b64ee154b1ed406d489077de2d6d60"
 
 [[package]]
 name = "objc2"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "559c5a40fdd30eb5e344fbceacf7595a81e242529fb4e21cf5f43fb4f11ff98d"
 dependencies = [
@@ -989,26 +989,26 @@
 checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
 dependencies = [
  "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "raw-window-handle"
 version = "0.6.0"
@@ -1088,26 +1088,26 @@
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1145,17 +1145,17 @@
  "log",
  "termcolor",
  "thread_local",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1398,15 +1398,15 @@
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
@@ -1425,15 +1425,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
@@ -1460,25 +1460,26 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
@@ -1487,17 +1488,17 @@
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
@@ -1505,17 +1506,17 @@
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
@@ -1523,17 +1524,23 @@
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
@@ -1541,17 +1548,17 @@
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
@@ -1559,17 +1566,17 @@
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
@@ -1577,17 +1584,17 @@
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
@@ -1595,17 +1602,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winit"
 version = "0.29.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d59ad965a635657faf09c8f062badd885748428933dad8e8bdd64064d92e5ca"
 dependencies = [
```

### Comparing `arrow_odbc-5.1.0/pyproject.toml` & `arrow_odbc-6.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "maturin"
 
 [project]
 name = "arrow-odbc"
 authors = [{name = "Markus Klein"}]
 description="Read the data of an ODBC data source as sequence of Apache Arrow record batches."
 readme = "README.md"
-version = "5.1.0"
+version = "6.0.0"
 dependencies = ["cffi", "pyarrow >= 8.0.0"]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 test = ["pytest < 8.0.0", "pyodbc", "duckdb"]
```

### Comparing `arrow_odbc-5.1.0/PKG-INFO` & `arrow_odbc-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arrow-odbc
-Version: 5.1.0
+Version: 6.0.0
 Requires-Dist: cffi
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: pytest <8.0.0 ; extra == 'test'
 Requires-Dist: pyodbc ; extra == 'test'
 Requires-Dist: duckdb ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
```

