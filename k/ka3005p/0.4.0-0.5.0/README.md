# Comparing `tmp/ka3005p-0.4.0.tar.gz` & `tmp/ka3005p-0.5.0.tar.gz`

## Comparing `ka3005p-0.4.0.tar` & `ka3005p-0.5.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 ka3005p-0.4.0/Cargo.toml
--rw-rw-r--   0     1000     1000      100 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/ISSUE_TEMPLATE/blank.md
--rw-rw-r--   0     1000     1000     1851 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/ISSUE_TEMPLATE/bug.md
--rw-rw-r--   0     1000     1000      873 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/ISSUE_TEMPLATE/documentation.md
--rw-rw-r--   0     1000     1000      923 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/ISSUE_TEMPLATE/feature.md
--rw-rw-r--   0     1000     1000      993 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/ISSUE_TEMPLATE/refactoring.md
--rw-rw-r--   0     1000     1000     1094 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/ISSUE_TEMPLATE/security.md
--rw-rw-r--   0     1000     1000      529 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/actions/ka3005p-dev/action.yml
--rw-rw-r--   0     1000     1000      676 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/dependabot.yml
--rw-rw-r--   0     1000     1000      254 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/workflows/cd.yml
--rw-rw-r--   0     1000     1000      378 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/workflows/ci.yml
--rw-rw-r--   0     1000     1000      610 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/workflows/gh-pages.yml
--rw-rw-r--   0     1000     1000      248 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/workflows/pr-merge.yml
--rw-rw-r--   0     1000     1000     3599 2024-02-21 21:40:53.000000 ka3005p-0.4.0/.github/workflows/rust.yml
--rw-rw-r--   0     1000     1000       96 2024-04-17 13:29:47.000000 ka3005p-0.4.0/.gitignore
--rw-rw-r--   0     1000     1000    24099 2024-04-17 13:29:47.000000 ka3005p-0.4.0/Cargo.lock
--rw-rw-r--   0     1000     1000     1071 2024-02-21 21:40:53.000000 ka3005p-0.4.0/LICENSE
--rw-rw-r--   0     1000     1000    10847 2024-02-21 21:40:53.000000 ka3005p-0.4.0/LICENSE-APACHE
--rw-rw-r--   0     1000     1000     3681 2024-04-17 10:20:25.000000 ka3005p-0.4.0/README.md
--rwxrwxr-x   0     1000     1000   232953 2024-02-21 21:40:53.000000 ka3005p-0.4.0/TenmaPSU.jpg
--rw-rw-r--   0     1000     1000        5 2024-02-21 21:40:53.000000 ka3005p-0.4.0/doc/.gitignore
--rw-rw-r--   0     1000     1000      103 2024-02-21 21:40:53.000000 ka3005p-0.4.0/doc/book.toml
--rw-rw-r--   0     1000     1000     3681 2024-04-17 10:20:25.000000 ka3005p-0.4.0/doc/src/README.md
--rw-rw-r--   0     1000     1000       65 2024-02-21 21:40:53.000000 ka3005p-0.4.0/doc/src/SUMMARY.md
--rwxrwxr-x   0     1000     1000   232953 2024-02-21 21:40:53.000000 ka3005p-0.4.0/doc/src/TenmaPSU.jpg
--rw-rw-r--   0     1000     1000     1879 2024-02-21 21:40:53.000000 ka3005p-0.4.0/doc/src/development.md
--rw-rw-r--   0     1000     1000       14 2024-02-21 21:40:53.000000 ka3005p-0.4.0/doc/src/doc/src/development.md
--rw-rw-r--   0     1000     1000       14 2024-02-21 21:40:53.000000 ka3005p-0.4.0/doc/src/src/development.md
--rw-rw-r--   0     1000     1000      442 2024-02-21 21:40:53.000000 ka3005p-0.4.0/justfile
--rw-rw-r--   0     1000     1000        0 2024-04-19 08:13:14.000000 ka3005p-0.4.0/ka30/README.md
--rw-rw-r--   0     1000     1000     1096 2024-04-18 15:47:10.000000 ka3005p-0.4.0/ka30/typeshed.pyi
--rw-rw-r--   0     1000     1000      173 2024-04-17 12:17:58.000000 ka3005p-0.4.0/scripts/power_supply.py
--rwxrwxr-x   0     1000     1000     1483 2024-04-17 10:20:25.000000 ka3005p-0.4.0/scripts/ramp.py
--rw-rw-r--   0     1000     1000     1908 2024-04-17 13:29:47.000000 ka3005p-0.4.0/src/bin/main.rs
--rw-rw-r--   0     1000     1000     2527 2024-04-16 12:03:52.000000 ka3005p-0.4.0/src/cli.rs
--rw-rw-r--   0     1000     1000    13402 2024-04-19 08:49:14.000000 ka3005p-0.4.0/src/lib.rs
--rw-rw-r--   0     1000     1000     6710 2024-04-19 09:56:43.000000 ka3005p-0.4.0/src/py_module.rs
--rw-rw-r--   0     1000     1000      462 2024-04-19 09:08:38.000000 ka3005p-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4682 1970-01-01 00:00:00.000000 ka3005p-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 ka3005p-0.5.0/Cargo.toml
+-rw-r--r--   0     1001      127      100 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/ISSUE_TEMPLATE/blank.md
+-rw-r--r--   0     1001      127     1851 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0     1001      127      873 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0     1001      127      923 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0     1001      127      993 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/ISSUE_TEMPLATE/refactoring.md
+-rw-r--r--   0     1001      127     1094 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0     1001      127      529 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/actions/ka3005p-dev/action.yml
+-rw-r--r--   0     1001      127      676 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/dependabot.yml
+-rw-r--r--   0     1001      127      254 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/workflows/cd.yml
+-rw-r--r--   0     1001      127      378 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      610 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/workflows/gh-pages.yml
+-rw-r--r--   0     1001      127      248 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/workflows/pr-merge.yml
+-rw-r--r--   0     1001      127     3390 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/workflows/pymodule.yml
+-rw-r--r--   0     1001      127     3129 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127       96 2024-04-19 15:27:31.000000 ka3005p-0.5.0/.gitignore
+-rw-r--r--   0     1001      127    24099 2024-04-19 15:27:31.000000 ka3005p-0.5.0/Cargo.lock
+-rw-r--r--   0     1001      127     1071 2024-04-19 15:27:31.000000 ka3005p-0.5.0/LICENSE
+-rw-r--r--   0     1001      127    10847 2024-04-19 15:27:31.000000 ka3005p-0.5.0/LICENSE-APACHE
+-rw-r--r--   0     1001      127     3681 2024-04-19 15:27:31.000000 ka3005p-0.5.0/README.md
+-rwxr-xr-x   0     1001      127   232953 2024-04-19 15:27:31.000000 ka3005p-0.5.0/TenmaPSU.jpg
+-rw-r--r--   0     1001      127        5 2024-04-19 15:27:31.000000 ka3005p-0.5.0/doc/.gitignore
+-rw-r--r--   0     1001      127      103 2024-04-19 15:27:31.000000 ka3005p-0.5.0/doc/book.toml
+-rw-r--r--   0     1001      127     3681 2024-04-19 15:27:31.000000 ka3005p-0.5.0/doc/src/README.md
+-rw-r--r--   0     1001      127       65 2024-04-19 15:27:31.000000 ka3005p-0.5.0/doc/src/SUMMARY.md
+-rwxr-xr-x   0     1001      127   232953 2024-04-19 15:27:31.000000 ka3005p-0.5.0/doc/src/TenmaPSU.jpg
+-rw-r--r--   0     1001      127     1879 2024-04-19 15:27:31.000000 ka3005p-0.5.0/doc/src/development.md
+-rw-r--r--   0     1001      127       14 2024-04-19 15:27:31.000000 ka3005p-0.5.0/doc/src/doc/src/development.md
+-rw-r--r--   0     1001      127       14 2024-04-19 15:27:31.000000 ka3005p-0.5.0/doc/src/src/development.md
+-rw-r--r--   0     1001      127      442 2024-04-19 15:27:31.000000 ka3005p-0.5.0/justfile
+-rw-r--r--   0     1001      127     2752 2024-04-19 15:27:31.000000 ka3005p-0.5.0/python/README.md
+-rw-r--r--   0     1001      127      743 2024-04-19 15:27:31.000000 ka3005p-0.5.0/python/examples/basics.py
+-rw-r--r--   0     1001      127       32 2024-04-19 15:27:31.000000 ka3005p-0.5.0/python/ka3005p/__init__.py
+-rw-r--r--   0     1001      127     1058 2024-04-19 15:27:31.000000 ka3005p-0.5.0/python/ka3005p/typeshed.pyi
+-rw-r--r--   0     1001      127      173 2024-04-19 15:27:31.000000 ka3005p-0.5.0/scripts/power_supply.py
+-rwxr-xr-x   0     1001      127     1483 2024-04-19 15:27:31.000000 ka3005p-0.5.0/scripts/ramp.py
+-rw-r--r--   0     1001      127     1892 2024-04-19 15:27:31.000000 ka3005p-0.5.0/src/bin/main.rs
+-rw-r--r--   0     1001      127     2527 2024-04-19 15:27:31.000000 ka3005p-0.5.0/src/cli.rs
+-rw-r--r--   0     1001      127    13440 2024-04-19 15:27:31.000000 ka3005p-0.5.0/src/lib.rs
+-rw-r--r--   0     1001      127     6635 2024-04-19 15:27:31.000000 ka3005p-0.5.0/src/py_module.rs
+-rw-r--r--   0     1001      127      863 2024-04-19 15:27:31.000000 ka3005p-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4009 1970-01-01 00:00:00.000000 ka3005p-0.5.0/PKG-INFO
```

### Comparing `ka3005p-0.4.0/Cargo.toml` & `ka3005p-0.5.0/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 [package]
 name = "ka3005p"
-version = "0.4.0"
-authors = ["Nicola Coretti <nico.coretti@gmail.com>", "Daniel Hartig <daniel-hartig@gmx.de>", "Jack Newman <Jack.Newman12@gmail.com>"]
+version = "0.5.0"
+authors = [
+    "Nicola Coretti <nico.coretti@gmail.com>", 
+    "Daniel Hartig <daniel-hartig@gmx.de>",
+    "Jack Newman <Jack.Newman12@gmail.com>"
+]
 edition = "2021"
 autobins = false
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 description = "cli tool to remote control a ka3005p power supply"
 homepage = "https://github.com/Nicoretti/ka3005p"
 repository = "https://github.com/Nicoretti/ka3005p"
@@ -17,18 +21,18 @@
 [dependencies]
 serialport = "4.*"
 human-panic = "1.*"
 anyhow = "1.*"
 clap = { version = "4.*", features = ["derive"] }
 log = "0.4.21"
 env_logger = "0.11.3"
-pyo3 = { version = "0.21.2" } #,  optional = true }
+pyo3 = { version = "0.21.2",  optional = true }
 
-#[features]
-#python_module = ["pyo3"]
+[features]
+python_module = ["pyo3"]
 
 [lib]
 name = "ka3005p"
 path = "src/lib.rs"
 crate-type = ["rlib", "cdylib"]
 
 [[bin]]
```

### Comparing `ka3005p-0.4.0/.github/ISSUE_TEMPLATE/bug.md` & `ka3005p-0.5.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/.github/ISSUE_TEMPLATE/documentation.md` & `ka3005p-0.5.0/.github/ISSUE_TEMPLATE/documentation.md`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/.github/ISSUE_TEMPLATE/feature.md` & `ka3005p-0.5.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/.github/ISSUE_TEMPLATE/refactoring.md` & `ka3005p-0.5.0/.github/ISSUE_TEMPLATE/refactoring.md`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/.github/ISSUE_TEMPLATE/security.md` & `ka3005p-0.5.0/.github/ISSUE_TEMPLATE/security.md`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/.github/actions/ka3005p-dev/action.yml` & `ka3005p-0.5.0/.github/actions/ka3005p-dev/action.yml`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/.github/dependabot.yml` & `ka3005p-0.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/.github/workflows/gh-pages.yml` & `ka3005p-0.5.0/.github/workflows/gh-pages.yml`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/.github/workflows/rust.yml` & `ka3005p-0.5.0/.github/workflows/rust.yml`

 * *Files 22% similar despite different names*

```diff
@@ -65,14 +65,22 @@
     - name: Tests
       if: contains(matrix.os, 'x86_64')
       uses: actions-rs/cargo@v1
       with:
           command: test
           args: --target ${{ matrix.os }} --verbose
 
+    - name: "Publish to crates.io"
+      if: matrix.os == 'x86_64' && startsWith(github.ref, 'refs/tags/')
+      uses: actions-rs/cargo@v1
+      with:
+          command: publish
+          args: --token ${{ secrets.CRATES_IO }}
+
+
   clippy_check:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v1
       - name: Install Rust
         uses: actions-rs/toolchain@v1
         with:
@@ -98,31 +106,7 @@
         override: true
         profile: minimal
         components: rustfmt
     - name: Check formatting
       run: |
         cargo fmt --all -- --check 
       
-  rustdoc:
-    runs-on: ubuntu-latest
-    steps:
-    - uses: actions/checkout@v2
-
-    - name: Install Rust toolchain
-      uses: actions-rs/toolchain@v1
-      with:
-        toolchain: stable
-        profile: minimal
-        override: true
-        target: x86_64-unknown-linux-musl
-        components: rustfmt, rust-src
-
-    - name: Build Documentation
-      run: cargo doc --all --no-deps  --target x86_64-unknown-linux-musl
-
-    - name: Deploy Docs
-      uses: peaceiris/actions-gh-pages@v3
-      if: ${{ github.ref == 'refs/heads/master' }}
-      with:
-        github_token: ${{ secrets.GITHUB_TOKEN }}
-        publish_branch: gh-pages
-        publish_dir: ./target/x86_64-unknown-linux-musl/doc/
```

### Comparing `ka3005p-0.4.0/Cargo.lock` & `ka3005p-0.5.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
 dependencies = [
  "core-foundation-sys",
  "mach2",
 ]
 
 [[package]]
 name = "ka3005p"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "anyhow",
  "clap",
  "env_logger",
  "human-panic",
  "log",
  "pyo3",
```

### Comparing `ka3005p-0.4.0/LICENSE` & `ka3005p-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/LICENSE-APACHE` & `ka3005p-0.5.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/README.md` & `ka3005p-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/TenmaPSU.jpg` & `ka3005p-0.5.0/TenmaPSU.jpg`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/doc/src/README.md` & `ka3005p-0.5.0/doc/src/README.md`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/doc/src/TenmaPSU.jpg` & `ka3005p-0.5.0/doc/src/TenmaPSU.jpg`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/doc/src/development.md` & `ka3005p-0.5.0/doc/src/development.md`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/ka30/typeshed.pyi` & `ka3005p-0.5.0/python/ka3005p/typeshed.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# power_supply.pyi
+# TODO: Fix outdated API bits
 from typing import List, Optional, Any, Union
 
 class PowerSupply:
 
     def __init__(self, serial_port: Optional[str] = None) -> None: ...
 
     @staticmethod
@@ -33,17 +33,14 @@
 
     @property
     def off(self) -> bool: ...
 
     @off.setter
     def off(self, disable: bool) -> None: ...
 
-    #@property
-    #def beep(self) -> bool: ...
-
     @beep.setter
     def beep(self, enable: bool) -> None: ...
 
     def save(self, id: int) -> None: ...
 
     def load(self, id: int) -> None: ...
```

### Comparing `ka3005p-0.4.0/scripts/ramp.py` & `ka3005p-0.5.0/scripts/ramp.py`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/src/bin/main.rs` & `ka3005p-0.5.0/src/bin/main.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #![deny(warnings)]
 use anyhow::Context;
 use clap::Parser;
 use std::convert::TryInto;
 use std::io::BufRead;
 use std::process::exit;
-use env_logger;
 
 fn main() -> ::anyhow::Result<(), anyhow::Error> {
     human_panic::setup_panic!();
     env_logger::init();
     let args = ka3005p::cli::Ka3005p::parse();
 
     if let ka3005p::cli::Command::List { verbose } = args.command {
```

### Comparing `ka3005p-0.4.0/src/cli.rs` & `ka3005p-0.5.0/src/cli.rs`

 * *Files identical despite different names*

### Comparing `ka3005p-0.4.0/src/lib.rs` & `ka3005p-0.5.0/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 use std::io;
 use std::str;
 use std::time;
 
 #[doc(hidden)] // Users of the library shouldn't use this
 pub mod cli;
 pub use serialport;
+#[cfg(feature = "python_module")]
 pub mod py_module;
 
 /// On / Off
 #[derive(Debug, PartialEq, Eq, Copy, Clone)]
 pub enum Switch {
     /// Enable the feature/output
     On,
@@ -305,15 +306,15 @@
 
     /// Retrieve status information from the power supply
     /// Returns a struct containing all the information about the power supply
     pub fn status(&mut self) -> anyhow::Result<Status> {
         let printable_ascii = |bytes: Vec<u8>| -> String {
             bytes
                 .into_iter()
-                .filter(|&b| b >= 32 && b <= 126)
+                .filter(|&b| (32..=126).contains(&b))
                 .collect::<Vec<u8>>()
                 .into_iter()
                 .map(|b| b as char)
                 .collect()
         };
 
         let flags: Flags = self.run_command_response("STATUS?")?[0].into();
```

### Comparing `ka3005p-0.4.0/src/py_module.rs` & `ka3005p-0.5.0/src/py_module.rs`

 * *Files 5% similar despite different names*

```diff
@@ -49,26 +49,23 @@
     ///
     /// Returns:
     ///     Result of executing the command.
     fn _execute(&mut self, command: Command) -> PyResult<()> {
         Ok(self
             .inner
             .execute(command)
-            .map_err(|e| Into::<Ka3005pError>::into(e))?)
+            .map_err(Into::<Ka3005pError>::into)?)
     }
 
     /// Get the status of the power supply.
     ///
     /// Returns:
     ///     Status of the power supply.
     fn _status(&mut self) -> PyResult<Status> {
-        Ok(self
-            .inner
-            .status()
-            .map_err(|e| Into::<Ka3005pError>::into(e))?)
+        Ok(self.inner.status().map_err(Into::<Ka3005pError>::into)?)
     }
 }
 
 #[pymethods]
 impl PowerSupply {
     #[new]
     /// Initialize a new PowerSupply instance.
@@ -77,18 +74,18 @@
     ///     serial_port: Optional serial port for communication.
     ///
     /// Returns:
     ///     New instance of PowerSupply.
     fn new(serial_port: Option<&str>) -> PyResult<Self> {
         let supply = match serial_port {
             Some(port) => PowerSupply {
-                inner: Ka3005p::new(port).map_err(|e| Into::<Ka3005pError>::into(e))?,
+                inner: Ka3005p::new(port).map_err(Into::<Ka3005pError>::into)?,
             },
             None => PowerSupply {
-                inner: find_serial_port().map_err(|e| Into::<Ka3005pError>::into(e))?,
+                inner: find_serial_port().map_err(Into::<Ka3005pError>::into)?,
             },
         };
         Ok(supply)
     }
 
     /// List all available and compatible power supplies.
     ///
@@ -109,15 +106,15 @@
     ///
     /// Returns:
     ///     Response from executing the command.
     fn execute(&mut self, command: &str) -> PyResult<Vec<u8>> {
         Ok(self
             .inner
             .run_command(command)
-            .map_err(|e| Into::<Ka3005pError>::into(e))?)
+            .map_err(Into::<Ka3005pError>::into)?)
     }
 
     /// Get the output current setting of the power supply.
     #[getter]
     fn get_current(&mut self) -> PyResult<f32> {
         let status = self._status()?;
         Ok(status.current)
@@ -179,15 +176,15 @@
         let status = self._status()?;
         Ok(status.flags.output.into())
     }
 
     /// Is beeping enabled.
     ///
     /// Returns:
-    ///     `True` if beeping is enabled, otherwise `False`. 
+    ///     `True` if beeping is enabled, otherwise `False`.
     #[getter]
     fn get_beep(&mut self) -> PyResult<bool> {
         let status = self._status()?;
         Ok(status.flags.beep.into())
     }
 
     /// Set the beep state of the power supply.
```

