# Comparing `tmp/lacuscore-1.9.1.tar.gz` & `tmp/lacuscore-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.9.1.tar", max compression
+gzip compressed data, was "lacuscore-1.9.2.tar", max compression
```

## Comparing `lacuscore-1.9.1.tar` & `lacuscore-1.9.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2024-03-29 16:56:05.329609 lacuscore-1.9.1/LICENSE
--rw-r--r--   0        0        0      941 2024-03-29 16:56:05.329609 lacuscore-1.9.1/README.md
--rw-r--r--   0        0        0      321 2024-03-29 16:56:05.329609 lacuscore-1.9.1/lacuscore/__init__.py
--rw-r--r--   0        0        0     2775 2024-03-29 16:56:05.329609 lacuscore-1.9.1/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    44397 2024-03-29 16:56:05.329609 lacuscore-1.9.1/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2024-03-29 16:56:05.329609 lacuscore-1.9.1/lacuscore/py.typed
--rw-r--r--   0        0        0     1873 2024-03-29 16:56:05.329609 lacuscore-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 lacuscore-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1516 2024-04-19 10:50:12.818198 lacuscore-1.9.2/LICENSE
+-rw-r--r--   0        0        0      941 2024-04-19 10:50:12.818198 lacuscore-1.9.2/README.md
+-rw-r--r--   0        0        0      321 2024-04-19 10:50:12.818198 lacuscore-1.9.2/lacuscore/__init__.py
+-rw-r--r--   0        0        0     2775 2024-04-19 10:50:12.818198 lacuscore-1.9.2/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    44432 2024-04-19 10:50:12.818198 lacuscore-1.9.2/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:50:12.818198 lacuscore-1.9.2/lacuscore/py.typed
+-rw-r--r--   0        0        0     1873 2024-04-19 10:50:12.822198 lacuscore-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 lacuscore-1.9.2/PKG-INFO
```

### Comparing `lacuscore-1.9.1/LICENSE` & `lacuscore-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.1/README.md` & `lacuscore-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.1/lacuscore/lacus_monitoring.py` & `lacuscore-1.9.2/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.9.1/lacuscore/lacuscore.py` & `lacuscore-1.9.2/lacuscore/lacuscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,15 +612,16 @@
                 general_timeout = to_capture.get('general_timeout_in_sec')
                 stats_pipeline.sadd(f'stats:{today}:captures', url)
                 async with Capture(
                         browser=browser_engine,
                         device_name=to_capture.get('device_name'),
                         proxy=proxy,
                         general_timeout_in_sec=general_timeout,
-                        loglevel=self.master_logger.getEffectiveLevel()) as capture:
+                        loglevel=self.master_logger.getEffectiveLevel(),
+                        uuid=uuid) as capture:
                     # required by Mypy: https://github.com/python/mypy/issues/3004
                     capture.headers = to_capture.get('headers')  # type: ignore[assignment]
                     capture.cookies = to_capture.get('cookies')  # type: ignore[assignment]
                     capture.viewport = to_capture.get('viewport')  # type: ignore[assignment]
                     capture.user_agent = to_capture.get('user_agent')  # type: ignore[assignment]
                     capture.http_credentials = to_capture.get('http_credentials')  # type: ignore[assignment]
                     capture.geolocation = to_capture.get('geolocation')  # type: ignore[assignment]
```

### Comparing `lacuscore-1.9.1/pyproject.toml` & `lacuscore-1.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.9.1"
+version = "1.9.2"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -30,28 +30,28 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 Sphinx = [
    {version = "<7.2", python = "<3.9", optional = true},
    {version = "^7.2", python = ">=3.9", optional = true}
 ]
-playwrightcapture = {extras = ["recaptcha"], version = "^1.24.1"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.24.5"}
 defang = "^0.5.3"
 ua-parser = "^0.18.0"
 redis = {version = "^5.0.3", extras = ["hiredis"]}
 dnspython = "^2.6.1"
 async-timeout = {version = "^4.0.3", python = "<3.11"}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
-types-redis = {version = "^4.6.0.20240311"}
+types-redis = {version = "^4.6.0.20240417"}
 mypy = "^1.9.0"
-types-requests = "^2.31.0.20240311"
+types-requests = "^2.31.0.20240406"
 types-beautifulsoup4 = "^4.12.0.20240229"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.18.0", python = ">=3.9"},
     {version = "^8.19.0", python = ">=3.10"}
 ]
 pytest = "^8.1.1"
```

### Comparing `lacuscore-1.9.1/PKG-INFO` & `lacuscore-1.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.9.1
+Version: 1.9.2
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,15 +24,15 @@
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (<7.2) ; (python_version < "3.9") and (extra == "docs")
 Requires-Dist: Sphinx (>=7.2,<8.0) ; (python_version >= "3.9") and (extra == "docs")
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0) ; python_version < "3.11"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
 Requires-Dist: dnspython (>=2.6.1,<3.0.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.24.1,<2.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.24.5,<2.0.0)
 Requires-Dist: redis[hiredis] (>=5.0.3,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ua-parser (>=0.18.0,<0.19.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
```

