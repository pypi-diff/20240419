# Comparing `tmp/fastapi_cdn_host-0.4.1.tar.gz` & `tmp/fastapi_cdn_host-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cdn_host-0.4.1.tar", max compression
+gzip compressed data, was "fastapi_cdn_host-0.4.2.tar", max compression
```

## Comparing `fastapi_cdn_host-0.4.1.tar` & `fastapi_cdn_host-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1086 2023-12-03 10:13:01.678736 fastapi_cdn_host-0.4.1/LICENSE
--rw-r--r--   0        0        0     2466 2023-12-29 15:22:24.861442 fastapi_cdn_host-0.4.1/README.md
--rw-r--r--   0        0        0      356 2024-04-11 07:19:56.277789 fastapi_cdn_host-0.4.1/fastapi_cdn_host/__init__.py
--rw-r--r--   0        0        0    18466 2024-04-11 07:19:56.278335 fastapi_cdn_host-0.4.1/fastapi_cdn_host/client.py
--rw-r--r--   0        0        0        0 2023-12-06 13:45:09.634356 fastapi_cdn_host-0.4.1/fastapi_cdn_host/py.typed
--rw-r--r--   0        0        0      980 2024-04-11 09:10:18.051455 fastapi_cdn_host-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 fastapi_cdn_host-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-12-03 10:13:01.678736 fastapi_cdn_host-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2349 2024-04-19 02:58:25.003391 fastapi_cdn_host-0.4.2/README.md
+-rw-r--r--   0        0        0      387 2024-04-18 09:57:50.755481 fastapi_cdn_host-0.4.2/fastapi_cdn_host/__init__.py
+-rw-r--r--   0        0        0    18466 2024-04-11 07:19:56.278335 fastapi_cdn_host-0.4.2/fastapi_cdn_host/client.py
+-rw-r--r--   0        0        0        0 2023-12-06 13:45:09.634356 fastapi_cdn_host-0.4.2/fastapi_cdn_host/py.typed
+-rw-r--r--   0        0        0     1079 2024-04-19 02:05:58.080259 fastapi_cdn_host-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2908 1970-01-01 00:00:00.000000 fastapi_cdn_host-0.4.2/PKG-INFO
```

### Comparing `fastapi_cdn_host-0.4.1/LICENSE` & `fastapi_cdn_host-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cdn_host-0.4.1/README.md` & `fastapi_cdn_host-0.4.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 # FastAPI CDN host Selector for docs ui
 ![Python Versions](https://img.shields.io/pypi/pyversions/fastapi-cdn-host)
 [![LatestVersionInPypi](https://img.shields.io/pypi/v/fastapi-cdn-host.svg?style=flat)](https://pypi.python.org/pypi/fastapi-cdn-host)
 [![GithubActionResult](https://github.com/waketzheng/fastapi-cdn-host/workflows/ci/badge.svg)](https://github.com/waketzheng/fastapi-cdn-host/actions?query=workflow:ci)
 [![Coverage Status](https://coveralls.io/repos/github/waketzheng/fastapi-cdn-host/badge.svg?branch=main)](https://coveralls.io/github/waketzheng/fastapi-cdn-host?branch=main)
-[![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 Auto find swagger-ui in local files, if exist use them.
 Otherwise make concurrent http requests by httpx to find out which third part cdn host is the fastest one.
 
-**English** | [中文](./README.zh-hans.md)
+**English** | [中文](./README.zh.md)
 
 ## Install
 
 ```bash
 pip install fastapi-cdn-host
 ```
 
 ## Usage
 1. Let's say that the default docs CDN host https://cdn.jsdelivr.net is too slow in your network, while unpkg.com is much faster.
 ```py
+import fastapi_cdn_host
 from fastapi import FastAPI
-from fastapi_cdn_host import monkey_patch_for_docs_ui
 
 app = FastAPI()
 # include_routes ...
 
-monkey_patch_for_docs_ui(app)  # Will use `unpkg.com` to replace the `cdn.jsdelivr.net/npm`
+fastapi_cdn_host.patch_docs(app)  # Will use `unpkg.com`(or other faster host) to replace the `cdn.jsdelivr.net/npm`
 ```
 2. In case of there are swagger-ui asset files in local directory named `static`
 ```py
 # Will auto mount static, then use `/static/swagger-ui-bundle.js` and `/static/swagger-ui.css` as docs assets
-monkey_patch_for_docs_ui(app)
+fastapi_cdn_host.patch_docs(app)
 ```
 This line is much more simple to serve offline docs then the example in official document:
 https://fastapi.tiangolo.com/how-to/custom-docs-ui-assets/?h=static#self-hosting-javascript-and-css-for-docs
 
 3. If asset files are ready in private cdn
 ```py
 # Will render /docs with the following asset urls:
 #   http://my-cdn.com/swagger-ui@latest/swagger-ui-bundle.js
 #   http://my-cdn.com/swagger-ui@latest/swagger-ui.css
 # render /redoc with: `http://my-cdn.com/redoc/next/redoc.standalone.js`
-monkey_patch_for_docs_ui(app, docs_cdn_host=('http://my-cdn.com', ('/swagger-ui@latest/', '/redoc/next/')))
+fastapi_cdn_host.patch_docs(app, docs_cdn_host=('http://my-cdn.com', ('/swagger-ui@latest/', '/redoc/next/')))
 ```
 
 ## License
 
 [MIT](./LICENSE)
```

### Comparing `fastapi_cdn_host-0.4.1/fastapi_cdn_host/client.py` & `fastapi_cdn_host-0.4.2/fastapi_cdn_host/client.py`

 * *Files identical despite different names*

### Comparing `fastapi_cdn_host-0.4.1/pyproject.toml` & `fastapi_cdn_host-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 [tool.poetry]
 name = "fastapi-cdn-host"
-version = "0.4.1"
+version = "0.4.2"
 description = ""
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = {version = ">=0.100"}
 httpx = {version = ">=0.23"}
 
 
 [tool.poetry.group.dev.dependencies]
-fast-tort-cli = {extras = ["all"], version="*", python=">=3.11"}
+fast-dev-cli = {extras = ["all"], version=">=0.7.0", python=">=3.11"}
 asyncur = {version=">=0.4.2", python=">=3.11"}
 uvicorn = {extras = ["standard"], version = "*"}
-isort = "*"
-black = "*"
-ruff = "*"
+bandit = "^1.7.8"
+ruff = ">=0.3"
 mypy = "*"
 pytest = "*"
 coverage = "*"
-bandit = "^1.7.8"
 starlette = "*"
 pydantic = "*"
+click = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.isort]
-profile="black"
-
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
 explicit_package_bases = true
 check_untyped_defs = true
 
 [tool.ruff.lint.per-file-ignores]
 "test_*.py" = ["E501"]
 
 [tool.coverage.run]
 branch = true
 parallel=true
 source = ["fastapi_cdn_host"]
 [tool.coverage.report]
-omit = ["tests/*"]
+omit = ["*/tests/*", "test_*"]
+exclude_lines = [
+    "pragma: no cover",
+    "@overload",
+    'if __name__ == "__main__":',
+    "if TYPE_CHECKING:",
+]
```

### Comparing `fastapi_cdn_host-0.4.1/PKG-INFO` & `fastapi_cdn_host-0.4.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cdn-host
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,54 +16,53 @@
 Description-Content-Type: text/markdown
 
 # FastAPI CDN host Selector for docs ui
 ![Python Versions](https://img.shields.io/pypi/pyversions/fastapi-cdn-host)
 [![LatestVersionInPypi](https://img.shields.io/pypi/v/fastapi-cdn-host.svg?style=flat)](https://pypi.python.org/pypi/fastapi-cdn-host)
 [![GithubActionResult](https://github.com/waketzheng/fastapi-cdn-host/workflows/ci/badge.svg)](https://github.com/waketzheng/fastapi-cdn-host/actions?query=workflow:ci)
 [![Coverage Status](https://coveralls.io/repos/github/waketzheng/fastapi-cdn-host/badge.svg?branch=main)](https://coveralls.io/github/waketzheng/fastapi-cdn-host?branch=main)
-[![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 
 Auto find swagger-ui in local files, if exist use them.
 Otherwise make concurrent http requests by httpx to find out which third part cdn host is the fastest one.
 
-**English** | [中文](./README.zh-hans.md)
+**English** | [中文](./README.zh.md)
 
 ## Install
 
 ```bash
 pip install fastapi-cdn-host
 ```
 
 ## Usage
 1. Let's say that the default docs CDN host https://cdn.jsdelivr.net is too slow in your network, while unpkg.com is much faster.
 ```py
+import fastapi_cdn_host
 from fastapi import FastAPI
-from fastapi_cdn_host import monkey_patch_for_docs_ui
 
 app = FastAPI()
 # include_routes ...
 
-monkey_patch_for_docs_ui(app)  # Will use `unpkg.com` to replace the `cdn.jsdelivr.net/npm`
+fastapi_cdn_host.patch_docs(app)  # Will use `unpkg.com`(or other faster host) to replace the `cdn.jsdelivr.net/npm`
 ```
 2. In case of there are swagger-ui asset files in local directory named `static`
 ```py
 # Will auto mount static, then use `/static/swagger-ui-bundle.js` and `/static/swagger-ui.css` as docs assets
-monkey_patch_for_docs_ui(app)
+fastapi_cdn_host.patch_docs(app)
 ```
 This line is much more simple to serve offline docs then the example in official document:
 https://fastapi.tiangolo.com/how-to/custom-docs-ui-assets/?h=static#self-hosting-javascript-and-css-for-docs
 
 3. If asset files are ready in private cdn
 ```py
 # Will render /docs with the following asset urls:
 #   http://my-cdn.com/swagger-ui@latest/swagger-ui-bundle.js
 #   http://my-cdn.com/swagger-ui@latest/swagger-ui.css
 # render /redoc with: `http://my-cdn.com/redoc/next/redoc.standalone.js`
-monkey_patch_for_docs_ui(app, docs_cdn_host=('http://my-cdn.com', ('/swagger-ui@latest/', '/redoc/next/')))
+fastapi_cdn_host.patch_docs(app, docs_cdn_host=('http://my-cdn.com', ('/swagger-ui@latest/', '/redoc/next/')))
 ```
 
 ## License
 
 [MIT](./LICENSE)
```

