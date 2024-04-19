# Comparing `tmp/reasoner_validator-4.0.0.tar.gz` & `tmp/reasoner_validator-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.0.0.tar", max compression
+gzip compressed data, was "reasoner_validator-4.0.1.tar", max compression
```

## Comparing `reasoner_validator-4.0.0.tar` & `reasoner_validator-4.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/LICENSE
--rw-r--r--   0        0        0    13503 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/README.md
--rw-r--r--   0        0        0      131 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/conf.py
--rw-r--r--   0        0        0    20365 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/index.rst
--rw-r--r--   0        0        0      795 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/make.bat
--rw-r--r--   0        0        0      136 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    39468 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2888 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    85875 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    43025 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/github.py
--rw-r--r--   0        0        0     3973 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/message.py
--rw-r--r--   0        0        0    46755 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    14288 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    35564 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/validator.py
--rw-r--r--   0        0        0    11943 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      838 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     2407 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/conftest.py
--rw-r--r--   0        0        0   138310 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    41247 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    27195 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_validate.py
--rw-r--r--   0        0        0    30223 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_validation_report.py
--rw-r--r--   0        0        0     2734 2024-04-03 01:08:55.989091 reasoner_validator-4.0.0/tests/test_workflows.py
--rw-r--r--   0        0        0    15838 1970-01-01 00:00:00.000000 reasoner_validator-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/LICENSE
+-rw-r--r--   0        0        0    13645 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/README.md
+-rw-r--r--   0        0        0      131 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/conf.py
+-rw-r--r--   0        0        0    20365 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-04-19 18:37:22.404448 reasoner_validator-4.0.1/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    39468 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2937 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    85875 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    43025 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3973 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/message.py
+-rw-r--r--   0        0        0    46755 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    14288 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    35564 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    11943 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      838 2024-04-19 18:37:22.408448 reasoner_validator-4.0.1/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     2407 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/conftest.py
+-rw-r--r--   0        0        0   138310 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    41247 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    27195 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_validate.py
+-rw-r--r--   0        0        0    30223 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2734 2024-04-19 18:37:22.412448 reasoner_validator-4.0.1/tests/test_workflows.py
+-rw-r--r--   0        0        0    15951 1970-01-01 00:00:00.000000 reasoner_validator-4.0.1/PKG-INFO
```

### Comparing `reasoner_validator-4.0.0/LICENSE` & `reasoner_validator-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/README.md` & `reasoner_validator-4.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 ./trapi_validator.py --help
 ```
 
 (*) Thank you Eric Deutsch for the prototype code for this script
 
 ## Running tests
 
-To run the test locally install with the `dev` dependencies group if not already done:
+To run the test locally install with the `dev` dependencies, if not already done (e.g. by **`--all-extras`** above):
 
 ```bash
 poetry install --extras dev
 ```
 
 Run the tests with coverage report:
 
@@ -106,15 +106,15 @@
 python -m http.server 3000 --directory ./htmlcov
 ```
 
 ## Building the Documentation Locally
 
 All paths here are relative to the root project directory.
 
-First install the documentation-specific dependencies.
+First install the documentation-specific dependencies, if not already done (e.g. by **`--all-extras`** above):
 
 ```bash
 poetry install --extras docs  # or poetry install --all-extras
 ```
 
 The validation codes MarkDown file should first be regenerated if needed (i.e. if it was revised):
 
@@ -160,15 +160,15 @@
 - An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted). 
 - An **optional** `target_provenance` with an object dictionary (example shown) specifying the ARA and KP infores-specified knowledge sources expected to be recovered in the TRAPI query results (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "target_provenance" or any of the subsidiary tags may be omitted (default to None)
 - An **optional** `strict_validation` flag (default: None or 'false'). If 'true' then follow strict validation rules, such as treating as 'error' states the use of `category`, `predicate` and `attribute_type_id` that are of type `abstract` or `mixin`  as errors. 
 - A **mandatory** `message` tag should have as its value the complete JSON TRAPI **Response** to be validated (See the example below)
 
 ### Running the Web Service Directly
 
-First install the web-specific dependencies.
+First install the web-specific dependencies, if not already done (e.g. by **`--all-extras`** above):
 
 ```bash
 poetry install --extras web  # or poetry install --all-extras
 ```
 
 The service may be run directly as a Python module. The web services module may be directly run, as follows.
```

### Comparing `reasoner_validator-4.0.0/docs/Makefile` & `reasoner_validator-4.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/docs/conf.py` & `reasoner_validator-4.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/docs/index.rst` & `reasoner_validator-4.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/docs/make.bat` & `reasoner_validator-4.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/docs/validation_codes_dictionary.md` & `reasoner_validator-4.0.1/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/pyproject.toml` & `reasoner_validator-4.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.0.0"
+version = "4.0.1"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
@@ -47,20 +47,20 @@
 # jsonschema needs to be pinned to <= 4.18.0 for now,
 # since 4.18.0 appeared to break something for the
 # access and processing of JSON schemata
 jsonschema = "~4.17.3"
 dictdiffer = "^0.9.0"
 PyYAML = "^6.0"
 requests = "^2.28.1"
-pydantic = "^1.10.13"
+pydantic = "^2"
 urllib3 = "^1.26.15"
 numpydoc = {version = "^1.5.0", optional = true}
 sphinx = {version = "^6.2.1", optional = true}
 myst-parser = {version = "^2.0.0", optional = true}
-fastapi = {version = "^0.85.0", optional = true}
+fastapi = {version = "*", optional = true}
 uvicorn = {version = "*", optional = true}
 pytest-cov = {version = "^4.0.0"}
 pytest = {version = "^7.2.2"}
 sphinx-rtd-theme = {version = "^1.2.2", optional = true}
 
 # for more pre-implemented OpenTelemetry instrumentations:
 #   https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation
@@ -77,13 +77,16 @@
 "Change Log" = "https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/NCATSTranslator/reasoner-validator/issues"
 
 [tool.poetry.extras]
 docs = ["numpydoc", "sphinx", "myst-parser", "sphinx-rtd-theme"]
 web = ["fastapi", "uvicorn", "httpx", "opentelemetry-exporter-otlp-proto-http", "opentelemetry-instrumentation-fastapi", "opentelemetry-instrumentation-httpx"]
 
+[tool.poetry.group.dev.dependencies]
+setuptools = "^69.5.1"
+
 [tool.coverage.run]
 source = ["reasoner_validator"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `reasoner_validator-4.0.0/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.0.1/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/codes.yaml` & `reasoner_validator-4.0.1/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/github.py` & `reasoner_validator-4.0.1/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/message.py` & `reasoner_validator-4.0.1/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/report.py` & `reasoner_validator-4.0.1/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/sri/util.py` & `reasoner_validator-4.0.1/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.0.1/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.0.1/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/validation_codes.py` & `reasoner_validator-4.0.1/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/validator.py` & `reasoner_validator-4.0.1/reasoner_validator/validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/versioning.py` & `reasoner_validator-4.0.1/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/reasoner_validator/versions.yaml` & `reasoner_validator-4.0.1/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/tests/__init__.py` & `reasoner_validator-4.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.0.1/tests/test_biolink_compliance_validation.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.0.1/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/tests/test_response_validator.py` & `reasoner_validator-4.0.1/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/tests/test_semver.py` & `reasoner_validator-4.0.1/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/tests/test_trapi_versioning.py` & `reasoner_validator-4.0.1/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/tests/test_validate.py` & `reasoner_validator-4.0.1/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/tests/test_validation_report.py` & `reasoner_validator-4.0.1/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/tests/test_workflows.py` & `reasoner_validator-4.0.1/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.0.0/PKG-INFO` & `reasoner_validator-4.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.0.0
+Version: 4.0.1
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -20,23 +20,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Provides-Extra: docs
 Provides-Extra: web
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: bmt (>=1.1.4,<2.0.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
-Requires-Dist: fastapi (>=0.85.0,<0.86.0) ; extra == "web"
+Requires-Dist: fastapi ; extra == "web"
 Requires-Dist: httpx (>=0.18.2,<0.19.0) ; extra == "web"
 Requires-Dist: jsonschema (>=4.17.3,<4.18.0)
 Requires-Dist: myst-parser (>=2.0.0,<3.0.0) ; extra == "docs"
 Requires-Dist: numpydoc (>=1.5.0,<2.0.0) ; extra == "docs"
 Requires-Dist: opentelemetry-exporter-otlp-proto-http ; extra == "web"
 Requires-Dist: opentelemetry-instrumentation-fastapi ; extra == "web"
 Requires-Dist: opentelemetry-instrumentation-httpx ; extra == "web"
-Requires-Dist: pydantic (>=1.10.13,<2.0.0)
+Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sphinx (>=6.2.1,<7.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.2.2,<2.0.0) ; extra == "docs"
 Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
 Requires-Dist: uvicorn ; extra == "web"
@@ -111,15 +111,15 @@
 ./trapi_validator.py --help
 ```
 
 (*) Thank you Eric Deutsch for the prototype code for this script
 
 ## Running tests
 
-To run the test locally install with the `dev` dependencies group if not already done:
+To run the test locally install with the `dev` dependencies, if not already done (e.g. by **`--all-extras`** above):
 
 ```bash
 poetry install --extras dev
 ```
 
 Run the tests with coverage report:
 
@@ -154,15 +154,15 @@
 python -m http.server 3000 --directory ./htmlcov
 ```
 
 ## Building the Documentation Locally
 
 All paths here are relative to the root project directory.
 
-First install the documentation-specific dependencies.
+First install the documentation-specific dependencies, if not already done (e.g. by **`--all-extras`** above):
 
 ```bash
 poetry install --extras docs  # or poetry install --all-extras
 ```
 
 The validation codes MarkDown file should first be regenerated if needed (i.e. if it was revised):
 
@@ -208,15 +208,15 @@
 - An **optional** `biolink_version` tag can be given a value of the Biolink Model version against which the message knowledge graph semantic contents will be validated, expressed as a SemVer string (defaults to 'latest' Biolink Model Toolkit supported version, if omitted). 
 - An **optional** `target_provenance` with an object dictionary (example shown) specifying the ARA and KP infores-specified knowledge sources expected to be recovered in the TRAPI query results (specified by infores CURIE) and the expected KP provenance source type, i.e. 'primary' implies that the KP is tagged as a 'biolink:primary_knowledge_source'. Optional in that the root "target_provenance" or any of the subsidiary tags may be omitted (default to None)
 - An **optional** `strict_validation` flag (default: None or 'false'). If 'true' then follow strict validation rules, such as treating as 'error' states the use of `category`, `predicate` and `attribute_type_id` that are of type `abstract` or `mixin`  as errors. 
 - A **mandatory** `message` tag should have as its value the complete JSON TRAPI **Response** to be validated (See the example below)
 
 ### Running the Web Service Directly
 
-First install the web-specific dependencies.
+First install the web-specific dependencies, if not already done (e.g. by **`--all-extras`** above):
 
 ```bash
 poetry install --extras web  # or poetry install --all-extras
 ```
 
 The service may be run directly as a Python module. The web services module may be directly run, as follows.
```

