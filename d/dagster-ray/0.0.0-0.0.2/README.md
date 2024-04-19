# Comparing `tmp/dagster_ray-0.0.0.tar.gz` & `tmp/dagster_ray-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_ray-0.0.0.tar", max compression
+gzip compressed data, was "dagster_ray-0.0.2.tar", max compression
```

## Comparing `dagster_ray-0.0.0.tar` & `dagster_ray-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,20 @@
--rw-r--r--   0        0        0    11344 2023-08-31 14:33:58.682247 dagster_ray-0.0.0/LICENSE
--rw-r--r--   0        0        0      315 2023-09-01 18:07:37.230360 dagster_ray-0.0.0/README.md
--rw-r--r--   0        0        0       79 2023-09-01 18:07:37.407032 dagster_ray-0.0.0/dagster_ray/__init__.py
--rw-r--r--   0        0        0       76 2023-08-31 14:33:58.685580 dagster_ray-0.0.0/dagster_ray/_version.py
--rw-r--r--   0        0        0      283 2023-09-01 18:07:37.703709 dagster_ray-0.0.0/dagster_ray/configs.py
--rw-r--r--   0        0        0    16047 2023-09-01 08:05:16.983051 dagster_ray-0.0.0/dagster_ray/executor.py
--rw-r--r--   0        0        0    11474 2023-09-01 18:09:34.237753 dagster_ray-0.0.0/dagster_ray/executor_2.py
--rw-r--r--   0        0        0     1204 2023-09-01 16:44:20.286956 dagster_ray-0.0.0/dagster_ray/io_managers.py
--rw-r--r--   0        0        0        0 2023-08-31 14:33:58.685580 dagster_ray-0.0.0/dagster_ray/py.typed
--rw-r--r--   0        0        0     1582 2023-09-01 18:09:05.613426 dagster_ray-0.0.0/dagster_ray/resource.py
--rw-r--r--   0        0        0     2752 2023-08-31 15:26:45.685207 dagster_ray-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 dagster_ray-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-19 15:55:35.601741 dagster_ray-0.0.2/LICENSE
+-rw-r--r--   0        0        0     7527 2024-04-19 15:55:35.601741 dagster_ray-0.0.2/README.md
+-rw-r--r--   0        0        0      115 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/_base/__init__.py
+-rw-r--r--   0        0        0     3070 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/_base/resources.py
+-rw-r--r--   0        0        0       76 2024-04-19 15:55:56.717969 dagster_ray-0.0.2/dagster_ray/_version.py
+-rw-r--r--   0        0        0     1114 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/config.py
+-rw-r--r--   0        0        0      627 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/kuberay/__init__.py
+-rw-r--r--   0        0        0     2767 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/kuberay/configs.py
+-rw-r--r--   0        0        0      159 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/kuberay/constants.py
+-rw-r--r--   0        0        0      503 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/kuberay/jobs.py
+-rw-r--r--   0        0        0     2905 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/kuberay/ops.py
+-rw-r--r--   0        0        0    10258 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/kuberay/ray_cluster_api.py
+-rw-r--r--   0        0        0    12402 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/kuberay/resources.py
+-rw-r--r--   0        0        0      275 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/kuberay/schedules.py
+-rw-r--r--   0        0        0       73 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/local/__init__.py
+-rw-r--r--   0        0        0     1087 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/local/resources.py
+-rw-r--r--   0        0        0        0 2024-04-19 15:55:35.605741 dagster_ray-0.0.2/dagster_ray/py.typed
+-rw-r--r--   0        0        0     2836 2024-04-19 15:55:56.713969 dagster_ray-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8659 1970-01-01 00:00:00.000000 dagster_ray-0.0.2/PKG-INFO
```

### Comparing `dagster_ray-0.0.0/LICENSE` & `dagster_ray-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_ray-0.0.0/pyproject.toml` & `dagster_ray-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagster-ray"
-version = "0.0.0"
+version = "0.0.2"
 description = "Dagster integration library for Ray"
 authors = [
     "Daniel Gafni <danielgafni16@gmail.com>"
 ]
 readme = "README.md"
 packages = [{include = "dagster_ray"}]
 repository = "https://github.com/danielgafni/dagster-ray"
@@ -22,79 +22,61 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-dagster = "^1.3.5"
-pyarrow = ">=8.0.0"
-ray = "^2.6.3"
-dagster-k8s = "^0.20.10"
-
+python = ">=3.8.1,<3.13"
+pyyaml = ">=4.0.0"
+kubernetes = ">=20.0.0" # no idea what's a good lower bound
+tenacity = ">=8.0.0"
+ray = {extras = ["all"], version = ">=2.7.0"}
+dagster = ">=1.6.0"
+
+[tool.poetry.extras]
+kuberay = [
+    "pyyaml",
+    "kubernetes",
+    "python-client",
+]
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.77.0"
 pytest = "^7.3.1"
-deepdiff = "^6.3.0"
-isort = "^5.12.0"
-ruff = "^0.0.272"
+ruff = "^0.3.0"
 pyright = "^1.1.313"
-tox = "^4.6.0"
-tox-gh = "^1.0.0"
 pre-commit = "^3.3.2"
 dagit = "^1.3.9"
-black = "^23.3.0"
 pytest-cases = "^3.6.14"
+pytest-kubernetes = "^0.3.1"
+blacken-docs = "^1.16.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 strict = false
 vcs = "git"
 style = "pep440"
 dirty = true
 
 [tool.poetry-dynamic-versioning.substitution]
 files = [
     "pyproject.toml",
     "dagster_ray/_version.py"
 ]
 
 [tool.pytest.ini_options]
+addopts = "-vvv --capture=no --log-disable=faker"
 log_cli = true
 log_level = "INFO"
 
-[tool.isort]
-profile = "black"
-line_length = 120
-src_paths = ["dagster_ray", "tests"]
-
-[tool.black]
-line-length = 120
-target-version = ['py39']
-include = '\.pyi?$'
-exclude = '''
-/(
-    \.eggs
-  | \.git
-  | \.hg
-  | \.mypy_cache
-  | \.pytest_cache
-  | \.ruff_cache
-  | \.venv
-  | build
-  | dist
-  )/
-'''
-
 [tool.ruff]
 line-length = 120
 src = [
     "dagster_ray",
     "tests"
 ]
 exclude = [
@@ -114,15 +96,17 @@
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
 ]
-[tool.ruff.isort]
+[tool.ruff.lint]
+extend-select = ["I"]
+[tool.ruff.lint.isort]
 known-first-party = ["dagster_ray", "tests"]
 
 [tool.pyright]
 reportPropertyTypeMismatch = true
 reportImportCycles = true
 reportWildcardImportFromLibrary = true
 reportUntypedFunctionDecorator = true
@@ -148,8 +132,9 @@
     "__pypackages__",
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
+    "dagster_ray/kuberay/ray_cluster_api.py"  # taken from https://github.com/ray-project/kuberay/tree/master/clients/python-client/python_client
 ]
```

