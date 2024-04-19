# Comparing `tmp/h2o_cloud_discovery-1.1.1.tar.gz` & `tmp/h2o_cloud_discovery-2.0.0.tar.gz`

## Comparing `h2o_cloud_discovery-1.1.1.tar` & `h2o_cloud_discovery-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/src/h2o_discovery/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/src/h2o_discovery/_version.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/src/h2o_discovery/error.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/src/h2o_discovery/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/src/h2o_discovery/py.typed
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/src/h2o_discovery/_internal/client.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/src/h2o_discovery/_internal/compat.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/src/h2o_discovery/_internal/config.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/src/h2o_discovery/_internal/load.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/src/h2o_discovery/_internal/lookup.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/tests/test_model.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/tests/test_version.py
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/tests/_internal/test_client.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/tests/_internal/test_config.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/tests/_internal/load/test_load_credentials.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/tests/_internal/load/test_load_discovery.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/tests/_internal/lookup/test_determine_local_config_path.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/tests/_internal/lookup/test_determine_uri.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/LICENSE
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/README.md
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 h2o_cloud_discovery-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/src/h2o_discovery/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/src/h2o_discovery/_version.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/src/h2o_discovery/error.py
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/src/h2o_discovery/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/src/h2o_discovery/py.typed
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/src/h2o_discovery/_internal/client.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/src/h2o_discovery/_internal/compat.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/src/h2o_discovery/_internal/config.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/src/h2o_discovery/_internal/load.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/src/h2o_discovery/_internal/lookup.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/tests/test_model.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/tests/test_version.py
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/tests/_internal/test_client.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/tests/_internal/test_config.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/tests/_internal/load/test_load_credentials.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/tests/_internal/load/test_load_discovery.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/tests/_internal/lookup/test_determine_local_config_path.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/tests/_internal/lookup/test_determine_uri.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/README.md
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 h2o_cloud_discovery-2.0.0/PKG-INFO
```

### Comparing `h2o_cloud_discovery-1.1.1/CHANGELOG.md` & `h2o_cloud_discovery-2.0.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,30 @@
 # Changelog
 
+## [2.0.0](https://github.com/h2oai/cloud-discovery-py/compare/v1.1.1...v2.0.0) (2024-04-19)
+
+
+### ⚠ BREAKING CHANGES
+
+* Python 3.7 is no longer supported. The minimum supported version is now Python 3.8.
+
+### Documentation
+
+* 📝 remove confusing example from README ([#95](https://github.com/h2oai/cloud-discovery-py/issues/95)) ([3da6c74](https://github.com/h2oai/cloud-discovery-py/commit/3da6c7451368fabf835e5966ac258ee79cf790e8))
+
+
+### Build System
+
+* 💥 remove support for Python 3.7 ([be67542](https://github.com/h2oai/cloud-discovery-py/commit/be67542550151c2673e38d640391793b8295bde2))
+
+
+### Continuous Integration
+
+* 👷 extend testing matrix of the httpx dependency ([#88](https://github.com/h2oai/cloud-discovery-py/issues/88)) ([b6fca62](https://github.com/h2oai/cloud-discovery-py/commit/b6fca62f0ed94b5edb9825945ca6d0028b7f65c1))
+
 ## [1.1.1](https://github.com/h2oai/cloud-discovery-py/compare/v1.1.0...v1.1.1) (2023-12-04)
 
 
 ### Documentation
 
 * 📝 Reflect new features in the README ([#79](https://github.com/h2oai/cloud-discovery-py/issues/79)) ([375969b](https://github.com/h2oai/cloud-discovery-py/commit/375969b3ca8682f1ce94a0d06028b8bd5fddd92d))
```

### Comparing `h2o_cloud_discovery-1.1.1/src/h2o_discovery/__init__.py` & `h2o_cloud_discovery-2.0.0/src/h2o_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/src/h2o_discovery/model.py` & `h2o_cloud_discovery-2.0.0/src/h2o_discovery/model.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/src/h2o_discovery/_internal/client.py` & `h2o_cloud_discovery-2.0.0/src/h2o_discovery/_internal/client.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/src/h2o_discovery/_internal/config.py` & `h2o_cloud_discovery-2.0.0/src/h2o_discovery/_internal/config.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/src/h2o_discovery/_internal/load.py` & `h2o_cloud_discovery-2.0.0/src/h2o_discovery/_internal/load.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/src/h2o_discovery/_internal/lookup.py` & `h2o_cloud_discovery-2.0.0/src/h2o_discovery/_internal/lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 def _discovery_uri_from_environment(environment: str):
     return urllib.parse.urljoin(environment + "/", _WELL_KNOWN_PATH)
 
 
 def determine_local_config_path(
-    config_path: Optional[Optional[Union[str, bytes, os.PathLike]]] = None
+    config_path: Optional[Optional[Union[str, bytes, os.PathLike]]] = None,
 ) -> Optional[str]:
     """Uses passed parameter, environment variable and H2O CLI default to get the
     path to the local config file.
     """
     if config_path is not None:
         return str(os.fspath(config_path))
```

### Comparing `h2o_cloud_discovery-1.1.1/tests/test_model.py` & `h2o_cloud_discovery-2.0.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/tests/_internal/test_client.py` & `h2o_cloud_discovery-2.0.0/tests/_internal/test_client.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/tests/_internal/test_config.py` & `h2o_cloud_discovery-2.0.0/tests/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/tests/_internal/load/test_load_credentials.py` & `h2o_cloud_discovery-2.0.0/tests/_internal/load/test_load_credentials.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/tests/_internal/load/test_load_discovery.py` & `h2o_cloud_discovery-2.0.0/tests/_internal/load/test_load_discovery.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/tests/_internal/lookup/test_determine_local_config_path.py` & `h2o_cloud_discovery-2.0.0/tests/_internal/lookup/test_determine_local_config_path.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/tests/_internal/lookup/test_determine_uri.py` & `h2o_cloud_discovery-2.0.0/tests/_internal/lookup/test_determine_uri.py`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/LICENSE` & `h2o_cloud_discovery-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `h2o_cloud_discovery-1.1.1/README.md` & `h2o_cloud_discovery-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -39,43 +39,15 @@
 
 # Connect to the my service.
 my_service_client = my_service.client(address=discovery.services["my-service"].uri)
 ```
 
 ## Examples
 
-### Example: Use with H2O.ai MLOps Python Client within the Wave App
-
-```python
-import h2o_authn
-import h2o_discovery
-import h2o_mlops_client as mlops
-from h2o_wave import Q, app, ui
-from h2o_wave import main
-
-@app("/")
-async def serve(q: Q):
-    discovery = await h2o_discovery.discover_async()
-
-    token_provider = h2o_authn.AsyncTokenProvider(
-        refresh_token=q.auth.refresh_token,
-        issuer_url=discovery.environment.issuer_url,
-        client_id=discovery.clients["platform"].oauth2_client_id,
-    )
-
-    mlops_client = mlops.Client(
-        gateway_url=discovery.services["mlops-api"].uri,
-        token_provider=token_provider,
-    )
-
-    ...
-
-```
-
-### Example 2: Use within a notebook to connect to the H2O AI Drive
+### Example: Use within a notebook to connect to the H2O AI Drive
 
 ```py
 # Install required packages.
 
 import sys
 !{sys.executable} -m pip install h2o-cloud-discovery h2o-authn[discovery]
 ```
```

### Comparing `h2o_cloud_discovery-1.1.1/pyproject.toml` & `h2o_cloud_discovery-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -19,38 +19,41 @@
   "tomli >= 1.1.0 ; python_version < '3.11'",
 ]
 description = 'H2O Cloud Discovery Python CLient'
 keywords = []
 license = "Apache-2.0"
 name = "h2o-cloud-discovery"
 readme = "README.md"
-requires-python = ">=3.7"
-version = "1.1.1"
+requires-python = ">=3.8"
+version = "2.0.0"
 
 [project.urls]
 Documentation = "https://github.com/h2oai/cloud-discovery-py#readme"
 Issues = "https://github.com/h2oai/cloud-discovery-py/issues"
 Source = "https://github.com/h2oai/cloud-discovery-py"
 
 [tool.hatch.build.targets.sdist]
 include = ["/src", "/tests", "CHANGELOG.md"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/h2o_discovery"]
 
 [[tool.hatch.envs.test.matrix]]
-httpx = ["httpx0.16", "httpx0.21", "httpx0.22", "httpx0.23"]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+httpx = ["httpx0.16", "httpx0.21", "httpx0.22", "httpx0.23", "httpx0.24", "httpx0.25", "httpx0.26"]
+python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.test.overrides]
 matrix.httpx.dependencies = [
   {value = "httpx==0.16.*", if = ["httpx0.16"]},
   {value = "httpx==0.21.*", if = ["httpx0.21"]},
   {value = "httpx==0.22.*", if = ["httpx0.22"]},
   {value = "httpx==0.23.*", if = ["httpx0.23"]},
+  {value = "httpx==0.24.*", if = ["httpx0.24"]},
+  {value = "httpx==0.25.*", if = ["httpx0.25"]},
+  {value = "httpx==0.26.*", if = ["httpx0.26"]},
 ]
 
 [tool.hatch.envs.test]
 dependencies = [
   "pytest-asyncio==0.20.2",
   "pytest==7.2",
   "respx>=0.16",
@@ -62,48 +65,48 @@
 
 [tool.hatch.envs.devtest]
 dev-mode = true
 template = "test"
 
 [tool.hatch.envs.lint]
 dependencies = [
-  "black==22.10.0",
   "mypy~=1.1",
-  "ruff==0.0.286",
+  "ruff==0.1.11",
 ]
 
 [tool.hatch.envs.lint.scripts]
 check = [
-  "black --check .",
+  "ruff format --check .",
   "ruff check .",
   "mypy src",
 ]
 fix = [
   "ruff check --fix .",
-  "black .",
+  "ruff format .",
   "check",
 ]
 
 [tool.hatch.envs.docs]
 dependencies = [
   "pydoc-markdown~=4.8",
 ]
 
 [tool.hatch.envs.docs.scripts]
 generate = "pydoc-markdown"
 
-[tool.black]
-skip-magic-trailing-comma = true
-
 [tool.ruff]
 extend-select = ["I", "B", "A", "ERA"]
 line-length = 88 # Same as black.
 src = ["src", "test"]
 target-version = "py37"
 
+[tool.ruff.format]
+docstring-code-format = true
+skip-magic-trailing-comma = true
+
 [tool.ruff.isort]
 case-sensitive = false
 force-single-line = true
 force-sort-within-sections = true
 known-first-party = ["h2o_discovery"]
 order-by-type = false
 relative-imports-order = "closest-to-furthest"
```

### Comparing `h2o_cloud_discovery-1.1.1/PKG-INFO` & `h2o_cloud_discovery-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: h2o-cloud-discovery
-Version: 1.1.1
+Version: 2.0.0
 Summary: H2O Cloud Discovery Python CLient
 Project-URL: Documentation, https://github.com/h2oai/cloud-discovery-py#readme
 Project-URL: Issues, https://github.com/h2oai/cloud-discovery-py/issues
 Project-URL: Source, https://github.com/h2oai/cloud-discovery-py
 Author-email: "H2O.ai" <support@h2o.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: httpx>=0.16
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # `h2o-cloud-discovery`
 
 [![licence](https://img.shields.io/github/license/h2oai/cloud-discovery-py?style=flat-square)](https://github.com/h2oai/cloud-discovery-py/blob/main/LICENSE)
@@ -60,43 +60,15 @@
 
 # Connect to the my service.
 my_service_client = my_service.client(address=discovery.services["my-service"].uri)
 ```
 
 ## Examples
 
-### Example: Use with H2O.ai MLOps Python Client within the Wave App
-
-```python
-import h2o_authn
-import h2o_discovery
-import h2o_mlops_client as mlops
-from h2o_wave import Q, app, ui
-from h2o_wave import main
-
-@app("/")
-async def serve(q: Q):
-    discovery = await h2o_discovery.discover_async()
-
-    token_provider = h2o_authn.AsyncTokenProvider(
-        refresh_token=q.auth.refresh_token,
-        issuer_url=discovery.environment.issuer_url,
-        client_id=discovery.clients["platform"].oauth2_client_id,
-    )
-
-    mlops_client = mlops.Client(
-        gateway_url=discovery.services["mlops-api"].uri,
-        token_provider=token_provider,
-    )
-
-    ...
-
-```
-
-### Example 2: Use within a notebook to connect to the H2O AI Drive
+### Example: Use within a notebook to connect to the H2O AI Drive
 
 ```py
 # Install required packages.
 
 import sys
 !{sys.executable} -m pip install h2o-cloud-discovery h2o-authn[discovery]
 ```
```

