# Comparing `tmp/ccdexplorer_schema_parser-0.1.6.tar.gz` & `tmp/ccdexplorer_schema_parser-0.1.7.tar.gz`

## Comparing `ccdexplorer_schema_parser-0.1.6.tar` & `ccdexplorer_schema_parser-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.6/Cargo.toml
--rw-r--r--   0     1001      127        4 2024-04-17 07:50:45.000000 ccdexplorer_schema_parser-0.1.6/.dockerignore
--rw-r--r--   0     1001      127     2452 2024-04-17 07:50:45.000000 ccdexplorer_schema_parser-0.1.6/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      690 2024-04-17 07:50:45.000000 ccdexplorer_schema_parser-0.1.6/.gitignore
--rw-r--r--   0     1001      127    11357 2024-04-17 07:50:45.000000 ccdexplorer_schema_parser-0.1.6/LICENSE.md
--rw-r--r--   0     1001      127     1961 2024-04-17 07:50:45.000000 ccdexplorer_schema_parser-0.1.6/README.md
--rw-r--r--   0     1001      127     1246 2024-04-17 07:50:45.000000 ccdexplorer_schema_parser-0.1.6/python/ccdexplorer_schema_parser/Schema.py
--rw-r--r--   0     1001      127        0 2024-04-17 07:50:45.000000 ccdexplorer_schema_parser-0.1.6/python/ccdexplorer_schema_parser/__init__.py
--rw-r--r--   0     1001      127       10 2024-04-17 07:50:45.000000 ccdexplorer_schema_parser-0.1.6/requirements.txt
--rw-r--r--   0     1001      127     3672 2024-04-17 07:50:45.000000 ccdexplorer_schema_parser-0.1.6/src/lib.rs
--rw-r--r--   0     1001      127    50137 2024-04-17 07:50:53.000000 ccdexplorer_schema_parser-0.1.6/Cargo.lock
--rw-r--r--   0     1001      127      430 2024-04-17 07:50:45.000000 ccdexplorer_schema_parser-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.7/Cargo.toml
+-rw-r--r--   0     1001      127        4 2024-04-19 07:59:49.000000 ccdexplorer_schema_parser-0.1.7/.dockerignore
+-rw-r--r--   0     1001      127     2452 2024-04-19 07:59:49.000000 ccdexplorer_schema_parser-0.1.7/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      690 2024-04-19 07:59:49.000000 ccdexplorer_schema_parser-0.1.7/.gitignore
+-rw-r--r--   0     1001      127    11357 2024-04-19 07:59:49.000000 ccdexplorer_schema_parser-0.1.7/LICENSE.md
+-rw-r--r--   0     1001      127     1961 2024-04-19 07:59:49.000000 ccdexplorer_schema_parser-0.1.7/README.md
+-rw-r--r--   0     1001      127     1474 2024-04-19 07:59:49.000000 ccdexplorer_schema_parser-0.1.7/python/ccdexplorer_schema_parser/Schema.py
+-rw-r--r--   0     1001      127        0 2024-04-19 07:59:49.000000 ccdexplorer_schema_parser-0.1.7/python/ccdexplorer_schema_parser/__init__.py
+-rw-r--r--   0     1001      127       10 2024-04-19 07:59:49.000000 ccdexplorer_schema_parser-0.1.7/requirements.txt
+-rw-r--r--   0     1001      127     4529 2024-04-19 07:59:49.000000 ccdexplorer_schema_parser-0.1.7/src/lib.rs
+-rw-r--r--   0     1001      127    50137 2024-04-19 07:59:54.000000 ccdexplorer_schema_parser-0.1.7/Cargo.lock
+-rw-r--r--   0     1001      127      430 2024-04-19 07:59:49.000000 ccdexplorer_schema_parser-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.7/PKG-INFO
```

### Comparing `ccdexplorer_schema_parser-0.1.6/.github/workflows/CI.yml` & `ccdexplorer_schema_parser-0.1.7/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.6/.gitignore` & `ccdexplorer_schema_parser-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.6/LICENSE.md` & `ccdexplorer_schema_parser-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.6/README.md` & `ccdexplorer_schema_parser-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.6/python/ccdexplorer_schema_parser/Schema.py` & `ccdexplorer_schema_parser-0.1.7/python/ccdexplorer_schema_parser/Schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,12 +20,18 @@
 
     def event_to_json(self, contractName, eventData):
         response = ccdexplorer_schema_parser.parse_event_ffi(
             self.schema, contractName, eventData
         )
         return json.loads(response)
 
+    def parameter_to_json(self, contractName, parameterData):
+        response = ccdexplorer_schema_parser.parse_parameter_ffi(
+            self.schema, contractName, parameterData
+        )
+        return json.loads(response)
+
     def return_value_to_json(self, contractName, functionName, returnValueData):
         response = ccdexplorer_schema_parser.parse_return_value_ffi(
             self.schema, contractName, functionName, returnValueData
         )
         return json.loads(response)
```

### Comparing `ccdexplorer_schema_parser-0.1.6/src/lib.rs` & `ccdexplorer_schema_parser-0.1.7/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 /// A Python module implemented in Rust.
 #[pymodule]
 fn ccdexplorer_schema_parser(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(extract_schema_ffi, m)?)?;
     m.add_function(wrap_pyfunction!(extract_schema_pair_ffi, m)?)?;
     m.add_function(wrap_pyfunction!(parse_event_ffi, m)?)?;
     m.add_function(wrap_pyfunction!(parse_return_value_ffi, m)?)?;
+    m.add_function(wrap_pyfunction!(parse_parameter_ffi, m)?)?;
     Ok(())
 }
 
 #[pyfunction]
 fn extract_schema_ffi(versioned_module_source: Vec<u8>) -> PyResult<Vec<u8>> {
     let module = match WasmModule::from_slice(&versioned_module_source) {
         Ok(m) => m,
@@ -105,7 +106,31 @@
         Ok(s) => match s.to_json_string_pretty(&return_value_data) {
             Ok(v) => Ok(v),
             Err(e) => Err(PyValueError::new_err(format!("Unable to parse event: {e}"))),
         },
         Err(e) => Err(PyValueError::new_err(format!("No event schema: {e}"))),
     }
 }
+
+#[pyfunction]
+fn parse_parameter_ffi(
+    versioned_module_schema: Vec<u8>,
+    contract_name: &str,
+    function_name: &str,
+    parameter_data: Vec<u8>,
+) -> PyResult<String> {
+    let schema: VersionedModuleSchema = match from_bytes(&versioned_module_schema) {
+        Ok(s) => s,
+        Err(e) => {
+            return Err(PyValueError::new_err(format!(
+                "Unable to parse schema: {e}"
+            )))
+        }
+    };
+    match schema.get_receive_param_schema(contract_name, function_name) {
+        Ok(s) => match s.to_json_string_pretty(&parameter_data) {
+            Ok(v) => Ok(v),
+            Err(e) => Err(PyValueError::new_err(format!("Unable to parse event: {e}"))),
+        },
+        Err(e) => Err(PyValueError::new_err(format!("No event schema: {e}"))),
+    }
+}
```

### Comparing `ccdexplorer_schema_parser-0.1.6/Cargo.lock` & `ccdexplorer_schema_parser-0.1.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
 name = "cc"
 version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 
 [[package]]
 name = "ccdexplorer-schema-parser"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "concordium-contracts-common",
  "concordium-smart-contract-engine",
  "concordium_base",
  "pyo3",
 ]
```

### Comparing `ccdexplorer_schema_parser-0.1.6/PKG-INFO` & `ccdexplorer_schema_parser-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ccdexplorer-schema-parser
-Version: 0.1.6
+Version: 0.1.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

