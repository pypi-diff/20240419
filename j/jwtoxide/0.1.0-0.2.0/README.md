# Comparing `tmp/jwtoxide-0.1.0.tar.gz` & `tmp/jwtoxide-0.2.0.tar.gz`

## Comparing `jwtoxide-0.1.0.tar` & `jwtoxide-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,45 @@
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 jwtoxide-0.1.0/Cargo.toml
--rw-r--r--   0     1000     1000     5218 2024-03-16 03:09:28.000000 jwtoxide-0.1.0/.github/workflows/release.yml
--rw-r--r--   0     1000     1000     1143 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/.github/workflows/test.yml
--rw-r--r--   0     1000     1000     1159 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/.github/workflows/version.yml
--rw-r--r--   0     1000     1000     3085 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/.gitignore
--rw-r--r--   0     1000     1000      813 2024-03-16 01:04:24.000000 jwtoxide-0.1.0/.readthedocs.yaml
--rw-r--r--   0     1000     1000      103 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/Dockerfile
--rw-r--r--   0     1000     1000     1070 2024-03-09 16:20:32.000000 jwtoxide-0.1.0/LICENSE
--rw-r--r--   0     1000     1000      204 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/Makefile
--rw-r--r--   0     1000     1000      611 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/README.rst
--rw-r--r--   0     1000     1000     1750 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/benchmark.py
--rw-r--r--   0     1000     1000      634 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/docs/Makefile
--rw-r--r--   0     1000     1000     1071 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/docs/conf.py
--rw-r--r--   0     1000     1000       34 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/docs/example.rst
--rw-r--r--   0     1000     1000      473 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/docs/index.rst
--rw-r--r--   0     1000     1000      800 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/docs/make.bat
--rw-r--r--   0     1000     1000      817 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/docs/modules.rst
--rw-r--r--   0     1000     1000       27 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/docs/readme.rst
--rw-r--r--   0     1000     1000     3513 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/example/README.rst
--rw-r--r--   0     1000     1000      257 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/example/docker-compose.yaml
--rw-r--r--   0     1000     1000     1972 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/example/server.py
--rw-r--r--   0     1000     1000     3854 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/jwtoxide.pyi
--rw-r--r--   0     1000     1000     4430 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/src/claims.rs
--rw-r--r--   0     1000     1000     5406 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/src/decoding_key.rs
--rw-r--r--   0     1000     1000     3092 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/src/encoding_key.rs
--rw-r--r--   0     1000     1000       50 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/src/header.rs
--rw-r--r--   0     1000     1000     1408 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/src/jwk/algorithm.rs
--rw-r--r--   0     1000     1000     3578 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/src/jwk/common.rs
--rw-r--r--   0     1000     1000     2006 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/src/jwk/mod.rs
--rw-r--r--   0     1000     1000     4627 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/src/keyring.rs
--rw-r--r--   0     1000     1000     8970 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/src/lib.rs
--rw-r--r--   0     1000     1000     4210 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/src/validation.rs
--rw-r--r--   0     1000     1000     8879 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/tests/test_decode.py
--rw-r--r--   0     1000     1000      346 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/tests/test_encode.py
--rw-r--r--   0     1000     1000     1466 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/tests/test_jwk.py
--rw-r--r--   0     1000     1000    29504 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/Cargo.lock
--rw-r--r--   0     1000     1000     1157 2024-03-16 01:04:18.000000 jwtoxide-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 jwtoxide-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 jwtoxide-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127     4457 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0     1001      127      966 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/.github/workflows/on-pr.yml
+-rw-r--r--   0     1001      127     5218 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     4532 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/.github/workflows/test-main.yml
+-rw-r--r--   0     1001      127     1173 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     1159 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/.github/workflows/version.yml
+-rw-r--r--   0     1001      127     3085 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/.gitignore
+-rw-r--r--   0     1001      127      818 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/.readthedocs.yaml
+-rw-r--r--   0     1001      127      103 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/Dockerfile
+-rw-r--r--   0     1001      127     1070 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/LICENSE
+-rw-r--r--   0     1001      127      320 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/Makefile
+-rw-r--r--   0     1001      127      334 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/NEWS.rst
+-rw-r--r--   0     1001      127      693 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/README.rst
+-rw-r--r--   0     1001      127     1750 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/benchmark.py
+-rw-r--r--   0     1001      127        0 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/changes/.gitkeep
+-rw-r--r--   0     1001      127      634 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/docs/Makefile
+-rw-r--r--   0     1001      127        0 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/docs/_static/.gitkeep
+-rw-r--r--   0     1001      127     1071 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/docs/conf.py
+-rw-r--r--   0     1001      127       34 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/docs/example.rst
+-rw-r--r--   0     1001      127      473 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/docs/index.rst
+-rw-r--r--   0     1001      127      800 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/docs/make.bat
+-rw-r--r--   0     1001      127      817 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/docs/modules.rst
+-rw-r--r--   0     1001      127       27 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/docs/readme.rst
+-rw-r--r--   0     1001      127      651 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/docs/requirements.txt
+-rw-r--r--   0     1001      127     3513 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/example/README.rst
+-rw-r--r--   0     1001      127      257 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/example/docker-compose.yaml
+-rw-r--r--   0     1001      127     1971 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/example/server.py
+-rw-r--r--   0     1001      127     3842 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/jwtoxide.pyi
+-rw-r--r--   0     1001      127     4500 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/src/claims.rs
+-rw-r--r--   0     1001      127     5493 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/src/decoding_key.rs
+-rw-r--r--   0     1001      127     3180 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/src/encoding_key.rs
+-rw-r--r--   0     1001      127       50 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/src/header.rs
+-rw-r--r--   0     1001      127     1408 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/src/jwk/algorithm.rs
+-rw-r--r--   0     1001      127     3625 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/src/jwk/common.rs
+-rw-r--r--   0     1001      127     2020 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/src/jwk/mod.rs
+-rw-r--r--   0     1001      127     4628 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/src/keyring.rs
+-rw-r--r--   0     1001      127     9167 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      127     4713 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/src/validation.rs
+-rw-r--r--   0     1001      127     9550 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/tests/test_decode.py
+-rw-r--r--   0     1001      127      346 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/tests/test_encode.py
+-rw-r--r--   0     1001      127     1466 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/tests/test_jwk.py
+-rw-r--r--   0     1001      127    29504 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/Cargo.lock
+-rw-r--r--   0     1001      127     1399 2024-04-19 16:19:01.000000 jwtoxide-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1495 1970-01-01 00:00:00.000000 jwtoxide-0.2.0/PKG-INFO
```

### Comparing `jwtoxide-0.1.0/Cargo.toml` & `jwtoxide-0.2.0/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "jwtoxide"
-version = "0.1.0"
+version = "0.2.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "jwtoxide"
 crate-type = ["cdylib"]
 
@@ -17,14 +17,14 @@
 lto = true
 debug = false
 codegen-units = 1
 panic = "abort"
 strip = "debuginfo"
 
 [dependencies]
-pyo3 = "0.20.2"
-jsonwebtoken = "9"
+pyo3 = { version = "0.21" }
+jsonwebtoken = ">=9.3.0, <10"
 serde = {version = "1.0", features = ["derive"] }
 serde_json = "1.0"  
 
 [dev-dependencies]
 cargo-llvm-cov = "0.6"
```

### Comparing `jwtoxide-0.1.0/.github/workflows/release.yml` & `jwtoxide-0.2.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This is a basic workflow to help you get started with Actions
 
-name: Build and Test
+name: Build, Test and Release
 
 # Controls when the workflow will run
-on: 
+on:
   push:
-    branches:
-      - main
+    tags:
+      - 'v*'
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 # A workflow run is made up of one or more jobs that can run sequentially or in parallel
 jobs:
   build-sdist:
@@ -132,9 +132,9 @@
       # retrieve your distributions here
       - uses: actions/download-artifact@v4
         with:
           path: dist
           merge-multiple: true
       - name: Display structure of downloaded files
         run: ls -R
-      # - name: Publish package distributions to PyPI
-      #   uses: pypa/gh-action-pypi-publish@release/v1
+      - name: Publish package distributions to PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `jwtoxide-0.1.0/.github/workflows/test.yml` & `jwtoxide-0.2.0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 name: Test
 
 # Controls when the workflow will run
 on: 
   push:
     branches-ignore:
       - main
+    tags-ignore:
+      - "v*"
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 # A workflow run is made up of one or more jobs that can run sequentially or in parallel
 jobs:
   build:
```

### Comparing `jwtoxide-0.1.0/.github/workflows/version.yml` & `jwtoxide-0.2.0/.github/workflows/version.yml`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/.gitignore` & `jwtoxide-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/.readthedocs.yaml` & `jwtoxide-0.2.0/.readthedocs.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 #    - epub
 
 # Optional but recommended, declare the Python requirements required
 # to build your documentation
 # See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
 python:
    install:
-   - requirements: make install-dev
+   - requirements: docs/requirements.txt
```

### Comparing `jwtoxide-0.1.0/LICENSE` & `jwtoxide-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/README.rst` & `jwtoxide-0.2.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 jwtoxide
 ========
 
+`Read the Docs`_
+
 PyO3 bindings to the `jsonwebtoken` library in Rust.
 
 This library provides Python bindings to the jsonwebtoken_ Rust library. The JSON Web Token (JWT)
 has become the de-facto standard for API authentication on the web. 
 
 This is a pure Rust implementation and requires no other dependencies to use.
 
@@ -19,7 +21,8 @@
 
 Development
 -----------
 
 Building for development requires `maturin`. Once installed run `make install-dev`.
 
 .. _jsonwebtoken: https://docs.rs/jsonwebtoken/latest/jsonwebtoken/
+.. _`Read the Docs`: https://jwtoxide.readthedocs.io/en/latest/
```

### Comparing `jwtoxide-0.1.0/benchmark.py` & `jwtoxide-0.2.0/benchmark.py`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/docs/Makefile` & `jwtoxide-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/docs/conf.py` & `jwtoxide-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/docs/make.bat` & `jwtoxide-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/docs/modules.rst` & `jwtoxide-0.2.0/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/example/README.rst` & `jwtoxide-0.2.0/example/README.rst`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/example/server.py` & `jwtoxide-0.2.0/example/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Example JWT Authentication for FastAPI using Keycloak as an OIDC provider.
 
 To run, first start a Keycloak server using the provided docker-compose file.
 Once started, log in to the Keycloak admin console at http://localhost:8080
 using the username `admin` and password `admin`. Then, create a new confidential
 client called "fastapi" and set the "Valid Redirect URIs" to "http://localhost:8000/*".
 
-Afterwards, install both FastAPI and httpx using pip. Then start this script, 
+Afterwards, install both FastAPI and httpx using pip. Then start this script,
 go to localhost:8000/docs to see the authenticated endpoints.
 """
 
 from typing import Annotated
 
 from fastapi import FastAPI, HTTPException, Depends, status
 from fastapi.security import OpenIdConnect
```

### Comparing `jwtoxide-0.1.0/jwtoxide.pyi` & `jwtoxide-0.2.0/jwtoxide.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 ) -> str: ...
 def decode(
     token: str,
     key: EncodingKey | str,
     validation_options: ValidationOptions,
 ) -> dict[str, JsonType]: ...
 
-
 class DecodingKey(object):
-
     @classmethod
     def from_secret(self, content: bytes) -> "DecodingKey": ...
     @classmethod
     def from_base64_secret(self, content: str) -> "DecodingKey": ...
     @classmethod
     def from_rsa_pem(self, content: str) -> "DecodingKey": ...
     @classmethod
@@ -45,15 +43,14 @@
         x509_url: Optional[str] = None,
         x509_chain: Optional[list[str]] = None,
         x509_sha1_fingerprint: Optional[str] = None,
         x509_sha256_fingerprint: Optional[str] = None,
     ) -> None: ...
 
 class EncodingKey(object):
-
     @classmethod
     def from_secret(self, content: bytes) -> "EncodingKey": ...
     @classmethod
     def from_base64_secret(self, content: str) -> "EncodingKey": ...
     @classmethod
     def from_rsa_pem(self, content: str) -> "EncodingKey": ...
     @classmethod
@@ -71,14 +68,15 @@
     def __init__(
         self,
         aud: Optional[set[str]],
         iss: Optional[set[str]],
         sub: Optional[str] = None,
         verify_signature=True,
         required_spec_claims: set[str] = {"exp", "iat", "nbf"},
+        early_expiration_seconds: int = 0,
         leeway_seconds=60,
         validate_exp=True,
         validate_nbf=True,
         validate_aud=True,
         algorithms: list[str] = {
             "RS256",
             "RS384",
@@ -88,56 +86,34 @@
             "PS256",
             "PS384",
             "PS512",
             "EdDSA",
         },
     ) -> None: ...
 
-class InvalidTokenError(Exception):
-    ...
-
-class DecodeError(InvalidTokenError):
-    ...
-
-class InvalidSignatureError(DecodeError):
-    ...
-
-class MissingRequiredClaimError(InvalidTokenError):
-    ...
-
-class ExpiredSignatureError(InvalidTokenError):
-    ...
-
-class InvalidIssuerError(InvalidTokenError):
-    ...
-
-class InvalidAudienceError(InvalidTokenError):
-    ...
-
-class InvalidSubjectError(InvalidTokenError):
-    ...
-
-class ImmatureSignatureError(InvalidTokenError):
-    ...
-
-class InvalidAlgorithmError(InvalidTokenError):
-    ...
+class InvalidTokenError(Exception): ...
+class DecodeError(InvalidTokenError): ...
+class InvalidSignatureError(DecodeError): ...
+class MissingRequiredClaimError(InvalidTokenError): ...
+class ExpiredSignatureError(InvalidTokenError): ...
+class InvalidIssuerError(InvalidTokenError): ...
+class InvalidAudienceError(InvalidTokenError): ...
+class InvalidSubjectError(InvalidTokenError): ...
+class ImmatureSignatureError(InvalidTokenError): ...
+class InvalidAlgorithmError(InvalidTokenError): ...
 
 class Jwk:
     @classmethod
     def from_json(cls, content: str) -> "Jwk": ...
-
     def __str__(self) -> str: ...
 
 class JwkSet:
     @classmethod
     def from_json(cls, content: str) -> "JwkSet": ...
-
     def __str__(self) -> str: ...
 
 class KeyRing:
     @classmethod
     def from_jwkset(cls, jwk_set: JwkSet) -> "KeyRing": ...
-
     def decode(
         self, token: str, validation_options: ValidationOptions
     ) -> dict[str, JsonType]: ...
```

### Comparing `jwtoxide-0.1.0/src/claims.rs` & `jwtoxide-0.2.0/src/claims.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,114 +2,112 @@
 use pyo3::types::{PyBool, PyDict, PyFloat, PyList, PyLong, PyString};
 use serde::{Deserialize, Serialize};
 
 #[derive(Debug, Serialize, Deserialize)]
 pub struct Claim(serde_json::Value);
 
 impl FromPyObject<'_> for Claim {
-    fn extract(ob: &PyAny) -> PyResult<Self> {
-        let value = extract_value(ob)?;
+    fn extract_bound(obj: &Bound<'_, PyAny>) -> PyResult<Self> {
+        let value = extract_value_bound(obj)?;
         Ok(Claim(value))
     }
 }
 
 /// Converts a Python object to a serde_json::Value.
-fn extract_value(value: &PyAny) -> PyResult<serde_json::Value> {
+fn extract_value_bound(value: &Bound<'_, PyAny>) -> PyResult<serde_json::Value> {
     if let Ok(dict) = value.downcast::<PyDict>() {
         let mut map = serde_json::Map::new();
         for (key, value) in dict {
             let key: String = key.extract()?;
-            let value = extract_value(value)?;
+            let value = extract_value_bound(&value)?;
             map.insert(key, value);
         }
-        Ok(serde_json::Value::Object(map))
-    // Need to check bool before int otherwise it will mapped to (0, 1)
+        return Ok(serde_json::Value::Object(map));
     } else if let Ok(val) = value.downcast::<PyBool>() {
         let rval = val.extract::<bool>()?;
-        Ok(serde_json::Value::Bool(rval))
+        return Ok(serde_json::Value::Bool(rval));
     } else if let Ok(val) = value.downcast::<PyString>() {
-        Ok(serde_json::Value::String(val.to_string()))
+        return Ok(serde_json::Value::String(val.to_string()));
     } else if let Ok(val) = value.downcast::<PyLong>() {
         let rval = val.extract::<i64>()?;
-        Ok(serde_json::Value::Number(serde_json::Number::from(rval)))
+        return Ok(serde_json::Value::Number(serde_json::Number::from(rval)));
     } else if let Ok(val) = value.downcast::<PyFloat>() {
         let rval = val.extract::<f64>()?;
-        Ok(serde_json::Value::Number(
+        return Ok(serde_json::Value::Number(
             serde_json::Number::from_f64(rval).unwrap(),
-        ))
+        ));
     } else if let Ok(val) = value.downcast::<PyList>() {
-        let rval = val.extract::<Vec<&PyAny>>()?;
-        let vec: Result<Vec<serde_json::Value>, _> = rval.into_iter().map(extract_value).collect();
-        Ok(serde_json::Value::Array(vec?))
+        let list_iter = |val| extract_value_bound(&val);
+        let vec: Result<Vec<serde_json::Value>, _> = val.into_iter().map(list_iter).collect();
+        return Ok(serde_json::Value::Array(vec?));
     } else if value.is_none() {
-        Ok(serde_json::Value::Null)
-    } else {
-        Err(PyErr::new::<pyo3::exceptions::PyTypeError, _>(
-            "Invalid value type",
-        ))
+        return Ok(serde_json::Value::Null);
     }
+    Err(PyErr::new::<pyo3::exceptions::PyTypeError, _>(
+        "Invalid value type",
+    ))
 }
 
 impl ToPyObject for Claim {
     fn to_object(&self, py: Python) -> PyObject {
         match &self.0 {
             serde_json::Value::Null => py.None(),
-            serde_json::Value::Bool(b) => PyBool::new(py, *b).to_object(py),
+            serde_json::Value::Bool(b) => PyBool::new_bound(py, *b).to_object(py),
             serde_json::Value::Number(n) => {
                 if let Some(i) = n.as_i64() {
                     i.to_object(py)
                 } else if let Some(f) = n.as_f64() {
-                    PyFloat::new(py, f).to_object(py)
+                    PyFloat::new_bound(py, f).to_object(py)
                 } else {
                     panic!("Failed to convert number to i64 or f64")
                 }
             }
-            serde_json::Value::String(s) => PyString::new(py, s).to_object(py),
+            serde_json::Value::String(s) => PyString::new_bound(py, s).to_object(py),
             serde_json::Value::Array(arr) => {
-                let pylist = PyList::empty(py);
+                let pylist = PyList::empty_bound(py);
                 for item in arr {
                     pylist.append(Claim(item.clone()).to_object(py)).unwrap();
                 }
                 pylist.to_object(py)
             }
             serde_json::Value::Object(obj) => {
-                let dict = PyDict::new(py);
+                let dict = PyDict::new_bound(py);
                 for (k, v) in obj {
                     dict.set_item(k, Claim(v.clone()).to_object(py)).unwrap();
                 }
                 dict.to_object(py)
             }
         }
     }
 }
 
 impl IntoPy<PyObject> for Claim {
     fn into_py(self, py: Python<'_>) -> PyObject {
         match &self.0 {
             serde_json::Value::Null => py.None(),
-            serde_json::Value::Bool(b) => PyBool::new(py, *b).to_object(py),
+            serde_json::Value::Bool(b) => PyBool::new_bound(py, *b).to_object(py),
             serde_json::Value::Number(n) => {
                 if let Some(i) = n.as_i64() {
                     i.to_object(py)
                 } else if let Some(f) = n.as_f64() {
-                    PyFloat::new(py, f).to_object(py)
+                    PyFloat::new_bound(py, f).to_object(py)
                 } else {
                     panic!("Failed to convert number to i64 or f64")
                 }
             }
-            serde_json::Value::String(s) => PyString::new(py, s).to_object(py),
+            serde_json::Value::String(s) => PyString::new_bound(py, s).to_object(py),
             serde_json::Value::Array(arr) => {
-                let pylist = PyList::empty(py);
+                let pylist = PyList::empty_bound(py);
                 for item in arr {
                     pylist.append(Claim(item.clone()).to_object(py)).unwrap();
                 }
                 pylist.to_object(py)
             }
             serde_json::Value::Object(obj) => {
-                let dict = PyDict::new(py);
+                let dict = PyDict::new_bound(py);
                 for (k, v) in obj {
                     dict.set_item(k, Claim(v.clone()).to_object(py)).unwrap();
                 }
                 dict.to_object(py)
             }
         }
     }
```

### Comparing `jwtoxide-0.1.0/src/decoding_key.rs` & `jwtoxide-0.2.0/src/decoding_key.rs`

 * *Files 16% similar despite different names*

```diff
@@ -19,30 +19,30 @@
     /// :param content: The secret key.
     /// :type content: bytes
     /// :return: The key.
     /// :rtype: DecodingKey
     ///
     #[classmethod]
     #[pyo3(signature = (content))]
-    pub fn from_secret(_cls: &PyType, content: &[u8]) -> PyResult<Self> {
+    pub fn from_secret(_cls: &Bound<'_, PyType>, content: &[u8]) -> PyResult<Self> {
         let instance = DecodingKey {
             key: jsonwebtoken::DecodingKey::from_secret(content),
         };
         Ok(instance)
     }
 
     /// Create a key from base64 encoded bytes.
     ///
     /// :param content: The secret key that hase been base64 encoded.
     /// :type content: str
     /// :return: The key.
     /// :rtype: DecodingKey
     ///
     #[classmethod]
-    pub fn from_base64_secret(_cls: &PyType, content: &str) -> PyResult<Self> {
+    pub fn from_base64_secret(_cls: &Bound<'_, PyType>, content: &str) -> PyResult<Self> {
         let key = match jsonwebtoken::DecodingKey::from_base64_secret(content) {
             Ok(key) => key,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid base64 secret: {}",
                     e
                 )))
@@ -56,126 +56,126 @@
     ///
     /// :param content: The contents of a PEM file.
     /// :type content: str
     /// :return: The key.
     /// :rtype: DecodingKey
     ///
     #[classmethod]
-    pub fn from_rsa_pem(_cls: &PyType, content: &str) -> PyResult<Self> {
+    pub fn from_rsa_pem(_cls: &Bound<'_, PyType>, content: &str) -> PyResult<Self> {
         let key = match jsonwebtoken::DecodingKey::from_rsa_pem(content.as_bytes()) {
             Ok(key) => key,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid RSA PEM: {}",
                     e
                 )))
             }
         };
         let instance = DecodingKey { key };
         Ok(instance)
     }
 
     /// Create a key from a EC PEM file.
-    /// 
+    ///
     /// :param content: The contents of a PEM file.
     /// :type content: str
     /// :return: The key.
     /// :rtype: DecodingKey
-    /// 
+    ///
     #[classmethod]
-    pub fn from_ec_pem(_cls: &PyType, content: &str) -> PyResult<Self> {
+    pub fn from_ec_pem(_cls: &Bound<'_, PyType>, content: &str) -> PyResult<Self> {
         let key = match jsonwebtoken::DecodingKey::from_ec_pem(content.as_bytes()) {
             Ok(key) => key,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid EC PEM: {}",
                     e
                 )))
             }
         };
         let instance = DecodingKey { key };
         Ok(instance)
     }
 
     /// Create a key from a Ed PEM file.
-    /// 
+    ///
     /// :param content: The contents of a PEM file.
     /// :type content: str
     /// :return: The key.
     /// :rtype: DecodingKey
-    /// 
+    ///
     #[classmethod]
-    fn from_ed_pem(_cls: &PyType, content: &str) -> PyResult<Self> {
+    fn from_ed_pem(_cls: &Bound<'_, PyType>, content: &str) -> PyResult<Self> {
         let key = match jsonwebtoken::DecodingKey::from_ed_pem(content.as_bytes()) {
             Ok(key) => key,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid Ed PEM: {}",
                     e
                 )))
             }
         };
         let instance = DecodingKey { key };
         Ok(instance)
     }
 
     /// Create a key from a RSA DER file.
-    /// 
+    ///
     /// :param content: The contents of a DER file.
     /// :type content: bytes
     /// :return: The key.
     /// :rtype: DecodingKey
-    /// 
+    ///
     #[classmethod]
-    fn from_rsa_der(_cls: &PyType, content: &[u8]) -> PyResult<Self> {
+    fn from_rsa_der(_cls: &Bound<'_, PyType>, content: &[u8]) -> PyResult<Self> {
         let instance = DecodingKey {
             key: jsonwebtoken::DecodingKey::from_rsa_der(content),
         };
         Ok(instance)
     }
 
     /// Create a key from a EC DER file.
-    /// 
+    ///
     /// :param content: The contents of a DER file.
     /// :type content: bytes
     /// :return: The key.
     /// :rtype: DecodingKey
-    /// 
+    ///
     #[classmethod]
-    fn from_ec_der(_cls: &PyType, content: &[u8]) -> PyResult<Self> {
+    fn from_ec_der(_cls: &Bound<'_, PyType>, content: &[u8]) -> PyResult<Self> {
         let instance = DecodingKey {
             key: jsonwebtoken::DecodingKey::from_ec_der(content),
         };
         Ok(instance)
     }
 
     /// Create a key from a Ed DER file.
-    /// 
+    ///
     /// :param content: The contents of a DER file.
     /// :type content: bytes
     /// :return: The key.
     /// :rtype: DecodingKey
-    /// 
+    ///
     #[classmethod]
-    fn from_ed_der(_cls: &PyType, content: &[u8]) -> PyResult<Self> {
+    fn from_ed_der(_cls: &Bound<'_, PyType>, content: &[u8]) -> PyResult<Self> {
         let instance = DecodingKey {
             key: jsonwebtoken::DecodingKey::from_ed_der(content),
         };
         Ok(instance)
     }
 
     /// Create a key from a JSON Web Key (JWK).
-    /// 
+    ///
     /// :param jwk: The JWK.
     /// :type jwk: Jwk
     /// :return: The key.
     /// :rtype: DecodingKey
-    /// 
+    ///
     #[classmethod]
-    pub fn from_jwk(_cls: &PyType, jwk: &Jwk) -> PyResult<Self> {
+    pub fn from_jwk(_cls: &Bound<'_, PyType>, jwk: &Jwk) -> PyResult<Self> {
         let key = match jsonwebtoken::DecodingKey::from_jwk(&jwk.jwk) {
             Ok(key) => key,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid JWK: {}",
                     e
                 )))
```

### Comparing `jwtoxide-0.1.0/src/encoding_key.rs` & `jwtoxide-0.2.0/src/encoding_key.rs`

 * *Files 8% similar despite different names*

```diff
@@ -6,98 +6,98 @@
 pub struct EncodingKey {
     pub key: jsonwebtoken::EncodingKey,
 }
 
 #[pymethods]
 impl EncodingKey {
     #[classmethod]
-    pub fn from_secret(_cls: &PyType, content: &[u8]) -> PyResult<Self> {
+    pub fn from_secret(_cls: &Bound<'_, PyType>, content: &[u8]) -> PyResult<Self> {
         let instance = EncodingKey {
             key: jsonwebtoken::EncodingKey::from_secret(content),
         };
         Ok(instance)
     }
 
     #[classmethod]
-    pub fn from_base64_secret(_cls: &PyType, content: &str) -> PyResult<Self> {
+    pub fn from_base64_secret(_cls: &Bound<'_, PyType>, content: &str) -> PyResult<Self> {
         let key = match jsonwebtoken::EncodingKey::from_base64_secret(content) {
             Ok(key) => key,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid base64 secret: {}",
                     e
                 )))
             }
         };
         let instance = EncodingKey { key };
         Ok(instance)
     }
 
     #[classmethod]
-    pub fn from_rsa_pem(_cls: &PyType, content: &str) -> PyResult<Self> {
+    pub fn from_rsa_pem(_cls: &Bound<'_, PyType>, content: &str) -> PyResult<Self> {
         let key = match jsonwebtoken::EncodingKey::from_rsa_pem(content.as_bytes()) {
             Ok(key) => key,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid RSA PEM: {}",
                     e
                 )))
             }
         };
         let instance = EncodingKey { key };
         Ok(instance)
     }
 
     #[classmethod]
-    pub fn from_ec_pem(_cls: &PyType, content: &str) -> PyResult<Self> {
+    pub fn from_ec_pem(_cls: &Bound<'_, PyType>, content: &str) -> PyResult<Self> {
         let key = match jsonwebtoken::EncodingKey::from_ec_pem(content.as_bytes()) {
             Ok(key) => key,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid EC PEM: {}",
                     e
                 )))
             }
         };
         let instance = EncodingKey { key };
         Ok(instance)
     }
 
     #[classmethod]
-    fn from_ed_pem(_cls: &PyType, content: &str) -> PyResult<Self> {
+    fn from_ed_pem(_cls: &Bound<'_, PyType>, content: &str) -> PyResult<Self> {
         let key = match jsonwebtoken::EncodingKey::from_ed_pem(content.as_bytes()) {
             Ok(key) => key,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid Ed PEM: {}",
                     e
                 )))
             }
         };
         let instance = EncodingKey { key };
         Ok(instance)
     }
 
     #[classmethod]
-    fn from_rsa_der(_cls: &PyType, content: &[u8]) -> PyResult<Self> {
+    fn from_rsa_der(_cls: &Bound<'_, PyType>, content: &[u8]) -> PyResult<Self> {
         let instance = EncodingKey {
             key: jsonwebtoken::EncodingKey::from_rsa_der(content),
         };
         Ok(instance)
     }
 
     #[classmethod]
-    fn from_ec_der(_cls: &PyType, content: &[u8]) -> PyResult<Self> {
+    fn from_ec_der(_cls: &Bound<'_, PyType>, content: &[u8]) -> PyResult<Self> {
         let instance = EncodingKey {
             key: jsonwebtoken::EncodingKey::from_ec_der(content),
         };
         Ok(instance)
     }
 
     #[classmethod]
-    fn from_ed_der(_cls: &PyType, content: &[u8]) -> PyResult<Self> {
+    fn from_ed_der(_cls: &Bound<'_, PyType>, content: &[u8]) -> PyResult<Self> {
         let instance = EncodingKey {
             key: jsonwebtoken::EncodingKey::from_ed_der(content),
         };
         Ok(instance)
     }
 }
```

### Comparing `jwtoxide-0.1.0/src/jwk/algorithm.rs` & `jwtoxide-0.2.0/src/jwk/algorithm.rs`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/src/jwk/common.rs` & `jwtoxide-0.2.0/src/jwk/common.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use std::str::FromStr;
 
 use pyo3::exceptions::PyException;
 use pyo3::prelude::*;
+use pyo3::pybacked::PyBackedStr;
 
 struct PublicKeyUse(jsonwebtoken::jwk::PublicKeyUse);
 
 impl FromStr for PublicKeyUse {
     type Err = PyErr;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
@@ -44,30 +45,30 @@
 #[pyclass]
 #[allow(dead_code)]
 pub struct CommonParameters {
     common_parameters: jsonwebtoken::jwk::CommonParameters,
 }
 
 fn map_key_operations(
-    key_operations: Vec<&str>,
+    key_operations: Vec<PyBackedStr>,
 ) -> Result<Vec<jsonwebtoken::jwk::KeyOperations>, PyErr> {
     key_operations
         .iter()
         .map(|s| KeyOperations::from_str(s).map(|KeyOperations(inner)| inner))
         .collect()
 }
 
 #[pymethods]
 impl CommonParameters {
     #[new]
     #[pyo3(signature = (public_key_use=None, key_operations=None, key_algorithm=None, key_id=None, x509_url=None, x509_chain=None, x509_sha1_fingerprint=None, x509_sha256_fingerprint=None ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
         public_key_use: Option<&str>,
-        key_operations: Option<Vec<&str>>,
+        key_operations: Option<Vec<PyBackedStr>>,
         key_algorithm: Option<&str>,
         key_id: Option<String>,
         x509_url: Option<String>,
         x509_chain: Option<Vec<String>>,
         x509_sha1_fingerprint: Option<String>,
         x509_sha256_fingerprint: Option<String>,
     ) -> Result<Self, PyErr> {
```

### Comparing `jwtoxide-0.1.0/src/jwk/mod.rs` & `jwtoxide-0.2.0/src/jwk/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 use pyo3::{prelude::*, types::PyType};
 
 pub mod algorithm;
 pub mod common;
 
-
 /// A JSON Web Key (JWK) that can be used to validate a JWT.
-/// 
+///
 #[pyclass]
 pub struct Jwk {
     pub jwk: jsonwebtoken::jwk::Jwk,
 }
 
 #[pymethods]
 impl Jwk {
     /// Create a Jwk from a JSON string.
-    /// 
+    ///
     /// :param content: The JSON string.
     /// :type content: str
     /// :return: The JWK.
     /// :rtype: Jwk
     /// :raises: ValueError: If the JSON is invalid.
-    /// 
+    ///
     #[classmethod]
-    pub fn from_json(_cls: &PyType, content: &str) -> PyResult<Self> {
+    pub fn from_json(_cls: &Bound<'_, PyType>, content: &str) -> PyResult<Self> {
         let deserialized: jsonwebtoken::jwk::Jwk = match serde_json::from_str(content) {
             Ok(jwk) => jwk,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid JWK: {}",
                     e
                 )))
@@ -36,34 +35,33 @@
     }
 
     pub fn __str__(&self) -> String {
         format!("{:?}", self.jwk)
     }
 }
 
-
 /// A set of JSON Web Keys (JWKs) that can be used to validate a JWT.
-/// 
+///
 #[pyclass]
 pub struct JwkSet {
     pub jwkset: jsonwebtoken::jwk::JwkSet,
 }
 
 #[pymethods]
 impl JwkSet {
     /// Create a JwkSet from a JSON string.
-    /// 
+    ///
     /// :param content: The JSON string.
     /// :type content: str
     /// :return: The JwkSet.
     /// :rtype: JwkSet
     /// :raises: ValueError: If the JSON is invalid.
-    /// 
+    ///
     #[classmethod]
-    pub fn from_json(_cls: &PyType, content: &str) -> PyResult<Self> {
+    pub fn from_json(_cls: &Bound<'_, PyType>, content: &str) -> PyResult<Self> {
         let deserialized: jsonwebtoken::jwk::JwkSet = match serde_json::from_str(content) {
             Ok(jwk) => jwk,
             Err(e) => {
                 return Err(PyErr::new::<pyo3::exceptions::PyValueError, _>(format!(
                     "Invalid JWK Set: {}",
                     e
                 )))
```

### Comparing `jwtoxide-0.1.0/src/keyring.rs` & `jwtoxide-0.2.0/src/keyring.rs`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 #[derive(Debug, Serialize, Deserialize)]
 struct DecodedClaims {
     #[serde(flatten)]
     extra_fields: HashMap<String, claims::Claim>,
 }
 
-/// A set of JWKs that have been mapped to their key id. 
-/// 
+/// A set of JWKs that have been mapped to their key id.
+///
 /// This is primary API for validating JWTs from an oAuth2/OIDC provider.
-/// 
+///
 /// :example:
-/// 
+///
 /// .. code-block:: python  
-/// 
+///
 ///   from base64 import urlsafe_b64encode
 ///   import time
 ///
 ///   import jwt # get using `pip install PyJWT``
 ///
 ///   from jwtoxide import KeyRing, ValidationOptions
 ///
@@ -52,37 +52,37 @@
 ///       "iss": "test-issuer",
 ///   }
 ///   encoded_jwt = jwt.encode(
 ///       data, encoding_key, algorithm="HS256", headers={"kid": "key1"}
 ///   )
 ///   jwk_set = JwkSet.from_json(jwk_set_json)
 ///   key_ring = KeyRing.from_jwkset(jwk_set)
-/// 
+///
 ///   validation_options = ValidationOptions(
 ///       aud={"test"}, iss={"test-issuer"}, algorithms=["HS256"]
 ///   )
 ///   claims = key_ring.decode(encoded_jwt, validation_options=validation_options)
 ///
 #[derive(Clone)]
 #[pyclass]
 pub struct KeyRing {
     pub keys: HashMap<String, jsonwebtoken::DecodingKey>,
 }
 
 #[pymethods]
 impl KeyRing {
     /// Create a KeyRing from a JwkSet.
-    /// 
+    ///
     /// :param jwkset: The JwkSet.
     /// :type jwkset: JwkSet
     /// :return: The KeyRing.
     /// :rtype: KeyRing
-    /// 
+    ///
     #[classmethod]
-    pub fn from_jwkset(_cls: &PyType, jwkset: &JwkSet) -> PyResult<Self> {
+    pub fn from_jwkset(_cls: &Bound<'_, PyType>, jwkset: &JwkSet) -> PyResult<Self> {
         let mut keys = HashMap::new();
 
         for k in &jwkset.jwkset.keys {
             if let Some(kid) = &k.common.key_id {
                 let key = jsonwebtoken::DecodingKey::from_jwk(k).map_err(|_| {
                     PyErr::new::<exceptions::PyValueError, _>(
                         "Failed to create DecodingKey from Jwk",
@@ -92,23 +92,23 @@
             }
         }
 
         Ok(KeyRing { keys })
     }
 
     /// Decode a JWT token.
-    /// 
+    ///
     /// :param token: The JWT to decode.
     /// :type token: str
     /// :param validation_options: The options for token validation.
     /// :type validation_options: ValidationOptions
     /// :return: The decoded claims.
     /// :rtype: dict
     /// :raises: :class:`InvalidTokenError`: If the token fails validation.
-    /// 
+    ///
     pub fn decode(
         &self,
         token: &str,
         validation_options: &ValidationOptions,
     ) -> PyResult<HashMap<String, claims::Claim>> {
         let header = jsonwebtoken::decode_header(token).map_err(|e| match e.kind() {
             jsonwebtoken::errors::ErrorKind::InvalidToken => {
```

### Comparing `jwtoxide-0.1.0/src/lib.rs` & `jwtoxide-0.2.0/src/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -80,38 +80,38 @@
 }
 
 pub enum JsonValue {
     String(String),
 }
 
 fn encode_claims(
-    claim_value: &HashMap<&str, claims::Claim>,
+    claim_value: &HashMap<String, claims::Claim>,
     key: jsonwebtoken::EncodingKey,
     algorithm: &str,
 ) -> Result<String, Error> {
     let algorithm = jsonwebtoken::Algorithm::from_str(algorithm)?;
     let header = jsonwebtoken::Header::new(algorithm);
     jsonwebtoken::encode(&header, &claim_value, &key)
 }
 
-fn get_encoding_key(key: &PyAny) -> Result<EncodingKey, PyErr> {
+fn get_encoding_key(key: &Bound<'_, PyAny>) -> Result<EncodingKey, PyErr> {
     if let Ok(py_key) = key.downcast::<pyo3::types::PyString>() {
         let key_string = py_key.to_string();
         let secret_bytes = key_string.as_bytes();
         Ok(EncodingKey::from_secret(secret_bytes))
     } else if let Ok(py_key) = key.extract::<encoding_key::EncodingKey>() {
         Ok(py_key.key)
     } else {
         Err(PyErr::new::<exceptions::PyException, _>(
             "Invalid key type, expected str or EncodingKey class.",
         ))
     }
 }
 
-fn get_decoding_key(key: &PyAny) -> Result<DecodingKey, PyErr> {
+fn get_decoding_key(key: &Bound<'_, PyAny>) -> Result<DecodingKey, PyErr> {
     if let Ok(py_key) = key.downcast::<pyo3::types::PyString>() {
         let key_string = py_key.to_string();
         let secret_bytes = key_string.as_bytes();
         Ok(DecodingKey::from_secret(secret_bytes))
     } else if let Ok(py_key) = key.extract::<decoding_key::DecodingKey>() {
         Ok(py_key.key)
     } else {
@@ -131,18 +131,18 @@
 /// :type algorithm: str
 /// :return: The encoded token.
 /// :rtype: str
 /// :raises:  Exception: If an error occurs during encoding
 #[pyfunction]
 #[pyo3(signature = (payload, key, algorithm="HS256", header=None))]
 fn encode(
-    payload: HashMap<&str, claims::Claim>,
-    key: &PyAny,
+    payload: HashMap<String, claims::Claim>,
+    key: &Bound<'_, PyAny>,
     algorithm: &str,
-    header: Option<&PyAny>,
+    header: Option<&Bound<'_, PyAny>>,
 ) -> PyResult<String> {
     if header.is_some() {
         //let header_value = header.unwrap();
         //let header_dict = header_value.extract::<Header>()?;
         return Err(PyErr::new::<exceptions::PyException, _>(
             "Header is not supported yet",
         ));
@@ -177,74 +177,83 @@
         }
         ErrorKind::InvalidAlgorithm => PyErr::new::<InvalidAlgorithmError, _>("Invalid algorithm."),
         _ => PyErr::new::<exceptions::PyException, _>(format!("Failed to decode token: {}", error)),
     }
 }
 
 /// Decode a JWT using the provided keys.
-/// 
+///
 /// This is a lower level api. Most users should rely on :class:`KeyRing` to decode tokens from a SSO provider.
 ///
 /// :param token: The JWT to decode.
 /// :type token: str
 /// :param key: The key to use for decoding. This can be an DecodingKey or a string representing an utf-8 encoded secret key.
 /// :type key: Union[DecodingKey, str]
 /// :param validation_options: The options for token validation.
 /// :type validation_options: ValidationOptions
 /// :return: The decoded claims.
 /// :rtype: dict
 /// :raises: :class:`InvalidTokenError`: If the token fails validation.
-/// 
+///
 #[pyfunction]
 #[pyo3(name = "decode")]
 fn py_decode(
     token: &str,
-    key: &PyAny,
+    key: &Bound<'_, PyAny>,
     validation_options: &validation::ValidationOptions,
 ) -> PyResult<HashMap<String, claims::Claim>> {
     let decoding_key = get_decoding_key(key)?;
     let validation = &validation_options.validation;
     let token_data: TokenData<DecodedClaims> = match decode(token, &decoding_key, validation) {
         Ok(c) => c,
         Err(e) => return Err(parse_decode_error(e)),
     };
     Ok(token_data.claims.extra_fields)
 }
 
 /// PyO3 Bindings to the jsonwebtoken library.
 #[pymodule]
-fn jwtoxide(_py: Python, m: &PyModule) -> PyResult<()> {
+fn jwtoxide(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
-    m.add("InvalidTokenError", _py.get_type::<InvalidTokenError>())?;
-    m.add("DecodeError", _py.get_type::<DecodeError>())?;
+    m.add(
+        "InvalidTokenError",
+        _py.get_type_bound::<InvalidTokenError>(),
+    )?;
+    m.add("DecodeError", _py.get_type_bound::<DecodeError>())?;
     m.add(
         "InvalidSignatureError",
-        _py.get_type::<InvalidSignatureError>(),
+        _py.get_type_bound::<InvalidSignatureError>(),
     )?;
     m.add(
         "MissingRequiredClaimError",
-        _py.get_type::<MissingRequiredClaimError>(),
+        _py.get_type_bound::<MissingRequiredClaimError>(),
     )?;
     m.add(
         "ExpiredSignatureError",
-        _py.get_type::<ExpiredSignatureError>(),
+        _py.get_type_bound::<ExpiredSignatureError>(),
+    )?;
+    m.add(
+        "InvalidIssuerError",
+        _py.get_type_bound::<InvalidIssuerError>(),
     )?;
-    m.add("InvalidIssuerError", _py.get_type::<InvalidIssuerError>())?;
     m.add(
         "InvalidAudienceError",
-        _py.get_type::<InvalidAudienceError>(),
+        _py.get_type_bound::<InvalidAudienceError>(),
+    )?;
+    m.add(
+        "InvalidSubjectError",
+        _py.get_type_bound::<InvalidSubjectError>(),
     )?;
-    m.add("InvalidSubjectError", _py.get_type::<InvalidSubjectError>())?;
     m.add(
         "ImmatureSignatureError",
-        _py.get_type::<ImmatureSignatureError>(),
+        _py.get_type_bound::<ImmatureSignatureError>(),
     )?;
     m.add(
         "InvalidAlgorithmError",
-        _py.get_type::<InvalidAlgorithmError>(),
+        _py.get_type_bound::<InvalidAlgorithmError>(),
     )?;
     m.add_function(wrap_pyfunction!(encode, m)?)?;
     m.add_function(wrap_pyfunction!(py_decode, m)?)?;
     m.add_class::<CommonParameters>()?;
     m.add_class::<EllipticCurveKeyParameters>()?;
     m.add_class::<encoding_key::EncodingKey>()?;
     m.add_class::<decoding_key::DecodingKey>()?;
```

### Comparing `jwtoxide-0.1.0/src/validation.rs` & `jwtoxide-0.2.0/src/validation.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use jsonwebtoken::Algorithm;
 use pyo3::prelude::*;
+use pyo3::pybacked::PyBackedStr;
 use std::collections::HashSet;
 use std::str::FromStr;
 
 const DEFAULT_ALGORITHMS: [Algorithm; 9] = [
     Algorithm::RS256,
     Algorithm::RS384,
     Algorithm::RS512,
@@ -26,14 +27,19 @@
 /// :param sub: Optional; The required subject claim, if set to None then no checking
 ///     is performed. Defaults to None.
 /// :type sub: str, optional
 /// :param required_spec_claims: The claims that are required to be present in the JWT.
 ///     Note only checks for presences of the claim, does not validate the value.
 ///     Defaults to {"exp", "iat", "nbf"}.
 /// :type required_spec_claims: set[str], optional
+/// :param early_expiration_seconds: Reject a token some time (in seconds)
+///     before the exp to prevent expiration in transit over the network.
+///     The value is the inverse of leeway, subtracting from the validation time.
+///     Defaults to 0
+/// :type early_expiration_seconds: int, optional
 /// :param leeway_seconds: The leeway for validating time based claims in second.
 ///     Defaults to 5 seconds.
 /// :type leeway_seconds: int, optional
 /// :param validate_exp: Whether to validate the expiration time claim, defaults to True.
 /// :type validate_exp: bool, optional
 /// :param validate_nbf: Whether to validate the not-before time claim, defaults to True.
 /// :type validate_nbf: bool, optional
@@ -54,32 +60,34 @@
 impl ValidationOptions {
     #[new]
     #[pyo3(signature = (
         aud,
         iss,
         sub = None,
         required_spec_claims = None,
+        early_expiration_seconds = 0,
         leeway_seconds = 5,
         validate_exp = true,
         validate_nbf = true,
         validate_aud = true,
         algorithms = None,
         verify_signature = true,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
         aud: Option<HashSet<String>>,
         iss: Option<HashSet<String>>,
         sub: Option<String>,
         required_spec_claims: Option<HashSet<String>>,
+        early_expiration_seconds: u64,
         leeway_seconds: u64,
         validate_exp: bool,
         validate_nbf: bool,
         validate_aud: bool,
-        algorithms: Option<Vec<&str>>,
+        algorithms: Option<Vec<PyBackedStr>>,
         verify_signature: bool,
     ) -> Self {
         let mut validation = jsonwebtoken::Validation::new(Algorithm::EdDSA);
         let algorithm_vec = match algorithms {
             Some(algos) => algos
                 .iter()
                 .map(|s| Algorithm::from_str(s).unwrap())
@@ -94,14 +102,15 @@
                 claims.insert("exp".to_string());
                 claims.insert("iat".to_string());
                 claims.insert("nbf".to_string());
                 claims
             }
         };
         validation.required_spec_claims = req_spec_claims;
+        validation.reject_tokens_expiring_in_less_than = early_expiration_seconds;
         validation.leeway = leeway_seconds;
         validation.validate_exp = validate_exp;
         validation.validate_nbf = validate_nbf;
         validation.validate_aud = validate_aud;
         validation.iss = iss;
         validation.aud = aud;
         validation.sub = sub;
```

### Comparing `jwtoxide-0.1.0/tests/test_decode.py` & `jwtoxide-0.2.0/tests/test_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,36 @@
     encoded_jwt = jwt.encode(data, "secret", algorithm="HS256")
     validation_options = ValidationOptions(aud=None, iss=None, algorithms=["HS256"])
 
     with pytest.raises(ExpiredSignatureError):
         decode(encoded_jwt, "secret", validation_options=validation_options)
 
 
+def test_early_expired_signature():
+    """Test that error raised when the token has expired."""
+    data = {
+        "sub": "1234567890",
+        "exp": int(time.time()) + 2,
+        "iat": int(time.time()) - 5000,
+        "nbf": int(time.time()) - 5000,
+        "name": "John Doe",
+    }
+    encoded_jwt = jwt.encode(data, "secret", algorithm="HS256")
+    validation_options = ValidationOptions(
+        early_expiration_seconds=3,
+        leeway_seconds=0,
+        aud=None,
+        iss=None,
+        algorithms=["HS256"],
+    )
+
+    with pytest.raises(ExpiredSignatureError):
+        decode(encoded_jwt, "secret", validation_options=validation_options)
+
+
 def test_invalid_exp():
     """Test that error raised when the exp claim is an invalid type."""
     data = {
         "sub": "1234567890",
         "exp": str(int(time.time()) - 1000),
         "iat": int(time.time()) - 5000,
         "nbf": int(time.time()) - 5000,
@@ -142,15 +164,17 @@
         "sub": "1234567890",
         "exp": int(time.time()) - 50,
         "iat": int(time.time()) - 120,
         "nbf": int(time.time()) - 120,
         "name": "John Doe",
     }
     encoded_jwt = jwt.encode(data, "secret", algorithm="HS256")
-    validation_options = ValidationOptions(aud=None, iss=None, leeway_seconds = 60, algorithms=["HS256"])
+    validation_options = ValidationOptions(
+        aud=None, iss=None, leeway_seconds=60, algorithms=["HS256"]
+    )
 
     decode(encoded_jwt, "secret", validation_options=validation_options)
 
 
 def test_invalid_issuer():
     """Test that error raised when the issuer is invalid."""
     data = {"iss": "foo"}
```

### Comparing `jwtoxide-0.1.0/tests/test_jwk.py` & `jwtoxide-0.2.0/tests/test_jwk.py`

 * *Files identical despite different names*

### Comparing `jwtoxide-0.1.0/Cargo.lock` & `jwtoxide-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -270,30 +270,30 @@
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "jsonwebtoken"
-version = "9.2.0"
+version = "9.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c7ea04a7c5c055c175f189b6dc6ba036fd62306b58c66c9f6389036c503a3f4"
+checksum = "b9ae10193d25051e74945f1ea2d0b42e03cc3b890f7e4cc5faa44997d808193f"
 dependencies = [
  "base64",
  "js-sys",
  "pem",
  "ring",
  "serde",
  "serde_json",
  "simple_asn1",
 ]
 
 [[package]]
 name = "jwtoxide"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "cargo-llvm-cov",
  "jsonwebtoken",
  "pyo3",
  "serde",
  "serde_json",
 ]
@@ -482,17 +482,17 @@
 checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -500,49 +500,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 2.0.52",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn 2.0.52",
 ]
```

### Comparing `jwtoxide-0.1.0/pyproject.toml` & `jwtoxide-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 strip = true
 
 [project.optional-dependencies]
 test = ["pytest", "pyjwt>=2.0.0"]
+changelog = ["towncrier"]
 docs = ["sphinx", "autodoc", "sphinx-rtd-theme"]
 lint = ["ruff"]
 version = ["bump-my-version"]
 
 [tool.bumpversion]
-current_version = "0.1.0"
+current_version = "0.2.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = '\nversion = "{current_version}"'
 replace = '\nversion = "{new_version}"'
 regex = true
 ignore_missing_version = false
 tag = false
@@ -38,7 +39,16 @@
 allow_dirty = false
 commit = true
 message = "Bump version: {current_version} → {new_version}"
 commit_args = ""
 
 [[tool.bumpversion.files]]
 filename = "Cargo.toml"
+
+[[tool.bumpversion.files]]
+filename = "pyproject.toml"
+search = '\ncurrent_version = "{current_version}"'
+replace = '\ncurrent_version = "{new_version}"'
+
+[tool.towncrier]
+package = "jwtoxide"
+directory = "changes"
```

### Comparing `jwtoxide-0.1.0/PKG-INFO` & `jwtoxide-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jwtoxide
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pyjwt >=2.0.0 ; extra == 'test'
+Requires-Dist: towncrier ; extra == 'changelog'
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: autodoc ; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme ; extra == 'docs'
 Requires-Dist: ruff ; extra == 'lint'
 Requires-Dist: bump-my-version ; extra == 'version'
 Provides-Extra: test
+Provides-Extra: changelog
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: version
 License-File: LICENSE
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst; charset=UTF-8
 
 jwtoxide
 ========
 
+`Read the Docs`_
+
 PyO3 bindings to the `jsonwebtoken` library in Rust.
 
 This library provides Python bindings to the jsonwebtoken_ Rust library. The JSON Web Token (JWT)
 has become the de-facto standard for API authentication on the web. 
 
 This is a pure Rust implementation and requires no other dependencies to use.
 
@@ -40,8 +44,9 @@
 
 Development
 -----------
 
 Building for development requires `maturin`. Once installed run `make install-dev`.
 
 .. _jsonwebtoken: https://docs.rs/jsonwebtoken/latest/jsonwebtoken/
+.. _`Read the Docs`: https://jwtoxide.readthedocs.io/en/latest/
```

