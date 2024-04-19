# Comparing `tmp/umami_analytics-0.2.15.tar.gz` & `tmp/umami_analytics-0.2.17.tar.gz`

## Comparing `umami_analytics-0.2.15.tar` & `umami_analytics-0.2.17.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 umami_analytics-0.2.15/umami/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 umami_analytics-0.2.15/umami/urls.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 umami_analytics-0.2.15/umami/errors/__init__.py
--rw-r--r--   0        0        0    20299 2020-02-02 00:00:00.000000 umami_analytics-0.2.15/umami/impl/__init__.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 umami_analytics-0.2.15/umami/models/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 umami_analytics-0.2.15/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 umami_analytics-0.2.15/LICENSE
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 umami_analytics-0.2.15/pyproject.toml
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 umami_analytics-0.2.15/../README.md
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 umami_analytics-0.2.15/PKG-INFO
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 umami_analytics-0.2.17/umami/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 umami_analytics-0.2.17/umami/urls.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 umami_analytics-0.2.17/umami/errors/__init__.py
+-rw-r--r--   0        0        0    20363 2020-02-02 00:00:00.000000 umami_analytics-0.2.17/umami/impl/__init__.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 umami_analytics-0.2.17/umami/models/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 umami_analytics-0.2.17/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 umami_analytics-0.2.17/LICENSE
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 umami_analytics-0.2.17/pyproject.toml
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 umami_analytics-0.2.17/../README.md
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 umami_analytics-0.2.17/PKG-INFO
```

### Comparing `umami_analytics-0.2.15/umami/__init__.py` & `umami_analytics-0.2.17/umami/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from umami import impl
 from . import errors  # noqa: F401, E402
 from . import models  # noqa: F401, E402
-from .impl import login_async, login, heartbeat  # noqa: F401, E402
+from .impl import login_async, login, is_logged_in, heartbeat  # noqa: F401, E402
 from .impl import new_event_async, new_event  # noqa: F401, E402
 from .impl import new_page_view, new_page_view_async  # noqa: F401, E402
 from .impl import set_url_base, set_website_id, set_hostname  # noqa: F401, E402
 from .impl import verify_token_async, verify_token  # noqa: F401, E402
 from .impl import websites_async, websites  # noqa: F401, E402
 
 __author__ = 'Michael Kennedy <michael@talkpython.fm>'
 __version__ = impl.__version__
 user_agent = impl.user_agent
 
 __all__ = [
     models,
     errors,
     set_url_base, set_website_id, set_hostname,
-    login_async, login,
+    login_async, login, is_logged_in,
     websites_async, websites,
     new_event_async, new_event,
     new_page_view, new_page_view_async,
     verify_token_async, verify_token,
     heartbeat,
 ]
```

### Comparing `umami_analytics-0.2.15/umami/impl/__init__.py` & `umami_analytics-0.2.17/umami/impl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from typing import Optional
 
 import httpx
 
 from umami import models, urls
 
-__version__ = '0.2.15'
+__version__ = '0.2.17'
 
 from umami.errors import ValidationError, OperationNotAllowedError
 
 url_base: Optional[str] = None
 auth_token: Optional[str] = None
 default_website_id: Optional[str] = None
 default_hostname: Optional[str] = None
@@ -63,14 +63,18 @@
     Args:
         hostname: Hostname to use when one is not specified, e.g. 'talkpython.fm'
     """
     global default_hostname
     default_hostname = hostname
 
 
+def is_logged_in() -> bool:
+    return auth_token is not None
+
+
 async def login_async(username: str, password: str) -> models.LoginResponse:
     """
         Logs into Umami and retrieves a temporary auth token. If the token is expired,
         you'll need to log in again. This can be checked with verify_token().
         Args:
             username: Your Umami username
             password: Your Umami password
```

### Comparing `umami_analytics-0.2.15/umami/models/__init__.py` & `umami_analytics-0.2.17/umami/models/__init__.py`

 * *Files identical despite different names*

### Comparing `umami_analytics-0.2.15/LICENSE` & `umami_analytics-0.2.17/LICENSE`

 * *Files identical despite different names*

### Comparing `umami_analytics-0.2.15/pyproject.toml` & `umami_analytics-0.2.17/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     "website",
     "umami",
 ]
 authors = [
     { name = "Michael Kennedy", email = "michael@talkpython.fm" },
 ]
 classifiers = [
-    'Development Status :: 2 - Pre-Alpha',
+    'Development Status :: 4 - Beta',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 dependencies = [
     "httpx",
     "pydantic",
 ]
-version = "0.2.15"
+version = "0.2.17"
 
 
 [project.urls]
 Homepage = "https://github.com/mikeckennedy/umami-python"
 Tracker = "https://github.com/mikeckennedy/umami-python/issues"
 Source = "https://github.com/mikeckennedy/umami-python"
```

### Comparing `umami_analytics-0.2.15/../README.md` & `umami_analytics-0.2.17/../README.md`

 * *Files identical despite different names*

### Comparing `umami_analytics-0.2.15/PKG-INFO` & `umami_analytics-0.2.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: umami-analytics
-Version: 0.2.15
+Version: 0.2.17
 Summary: Umami Analytics Client for Python
 Project-URL: Homepage, https://github.com/mikeckennedy/umami-python
 Project-URL: Tracker, https://github.com/mikeckennedy/umami-python/issues
 Project-URL: Source, https://github.com/mikeckennedy/umami-python
 Author-email: Michael Kennedy <michael@talkpython.fm>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: analytics,umami,website
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

