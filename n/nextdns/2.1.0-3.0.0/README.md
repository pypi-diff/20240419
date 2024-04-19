# Comparing `tmp/nextdns-2.1.0.tar.gz` & `tmp/nextdns-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextdns-2.1.0.tar", last modified: Sun Nov 26 11:33:19 2023, max compression
+gzip compressed data, was "nextdns-3.0.0.tar", last modified: Fri Apr 19 14:00:01 2024, max compression
```

## Comparing `nextdns-2.1.0.tar` & `nextdns-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 11:33:19.964311 nextdns-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2023-11-26 11:33:03.000000 nextdns-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-26 11:33:03.000000 nextdns-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2023-11-26 11:33:19.964311 nextdns-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-11-26 11:33:03.000000 nextdns-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 11:33:19.964311 nextdns-2.1.0/nextdns/
--rw-r--r--   0 runner    (1001) docker     (127)    18323 2023-11-26 11:33:03.000000 nextdns-2.1.0/nextdns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15228 2023-11-26 11:33:03.000000 nextdns-2.1.0/nextdns/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-26 11:33:03.000000 nextdns-2.1.0/nextdns/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12160 2023-11-26 11:33:03.000000 nextdns-2.1.0/nextdns/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-26 11:33:03.000000 nextdns-2.1.0/nextdns/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 11:33:19.964311 nextdns-2.1.0/nextdns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2023-11-26 11:33:19.000000 nextdns-2.1.0/nextdns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-11-26 11:33:19.000000 nextdns-2.1.0/nextdns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 11:33:19.000000 nextdns-2.1.0/nextdns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-26 11:33:19.000000 nextdns-2.1.0/nextdns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-26 11:33:19.000000 nextdns-2.1.0/nextdns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2023-11-26 11:33:03.000000 nextdns-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-11-26 11:33:03.000000 nextdns-2.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-26 11:33:03.000000 nextdns-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 11:33:19.964311 nextdns-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-11-26 11:33:03.000000 nextdns-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 11:33:19.964311 nextdns-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18641 2023-11-26 11:33:03.000000 nextdns-2.1.0/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:01.811663 nextdns-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-19 13:59:52.000000 nextdns-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 13:59:52.000000 nextdns-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-19 14:00:01.811663 nextdns-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-19 13:59:52.000000 nextdns-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:01.811663 nextdns-3.0.0/nextdns/
+-rw-r--r--   0 runner    (1001) docker     (127)    18324 2024-04-19 13:59:52.000000 nextdns-3.0.0/nextdns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-19 13:59:52.000000 nextdns-3.0.0/nextdns/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-19 13:59:52.000000 nextdns-3.0.0/nextdns/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-04-19 13:59:52.000000 nextdns-3.0.0/nextdns/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:59:52.000000 nextdns-3.0.0/nextdns/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:01.811663 nextdns-3.0.0/nextdns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-19 14:00:01.000000 nextdns-3.0.0/nextdns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-19 14:00:01.000000 nextdns-3.0.0/nextdns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:00:01.000000 nextdns-3.0.0/nextdns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 14:00:01.000000 nextdns-3.0.0/nextdns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 14:00:01.000000 nextdns-3.0.0/nextdns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-19 13:59:52.000000 nextdns-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-19 13:59:52.000000 nextdns-3.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 13:59:52.000000 nextdns-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:00:01.811663 nextdns-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-19 13:59:52.000000 nextdns-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:01.811663 nextdns-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-04-19 13:59:52.000000 nextdns-3.0.0/tests/test_init.py
```

### Comparing `nextdns-2.1.0/LICENSE` & `nextdns-3.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Maciej Bieniek
+   Copyright 2024 Maciej Bieniek
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `nextdns-2.1.0/PKG-INFO` & `nextdns-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: nextdns
-Version: 2.1.0
+Version: 3.0.0
 Summary: Python wrapper for NextDNS API.
 Home-page: https://github.com/bieniu/nextdns
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.0
 
 [![GitHub Release][releases-shield]][releases]
 [![PyPI][pypi-releases-shield]][pypi-releases]
 [![PyPI - Downloads][pypi-downloads]][pypi-statistics]
```

### Comparing `nextdns-2.1.0/README.md` & `nextdns-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nextdns-2.1.0/nextdns/__init__.py` & `nextdns-3.0.0/nextdns/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Python wrapper for NextDNS API."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 from collections.abc import Iterable
 from http import HTTPStatus
 from typing import Any, cast
```

### Comparing `nextdns-2.1.0/nextdns/const.py` & `nextdns-3.0.0/nextdns/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """NextDNS constants."""
+
 from .model import (
     ApiNames,
     ParentalControlCategories,
     ParentalControlCategoriesAttrs,
     ParentalControlServices,
     ParentalControlServicesAttrs,
     SettingDescription,
```

### Comparing `nextdns-2.1.0/nextdns/exceptions.py` & `nextdns-3.0.0/nextdns/exceptions.py`

 * *Files identical despite different names*

### Comparing `nextdns-2.1.0/nextdns/model.py` & `nextdns-3.0.0/nextdns/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,14 @@
 """Type definitions for NextDNS."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
-from enum import Enum
-from typing import Any, TypeVar
-
-_StrEnumSelfT = TypeVar("_StrEnumSelfT", bound="StrEnum")
-
-
-class StrEnum(str, Enum):
-    """Partial backport of Python 3.11's StrEnum for our basic use cases."""
-
-    value: str
-
-    def __new__(
-        cls: type[_StrEnumSelfT], value: str, *args: Any, **kwargs: Any
-    ) -> _StrEnumSelfT:  # noqa: PYI019
-        """Create a new StrEnum instance."""
-        if not isinstance(value, str):
-            raise TypeError(f"{value!r} is not a string")
-        return super().__new__(cls, value, *args, **kwargs)
-
-    def __str__(self) -> str:
-        """Return self.value."""
-        return self.value
-
-    @staticmethod
-    def _generate_next_value_(
-        name: str, start: int, count: int, last_values: list[Any]
-    ) -> Any:
-        """Make `auto()` explicitly unsupported."""
-        raise TypeError("auto() is not supported by this implementation")
+from enum import StrEnum
+from typing import Any
 
 
 @dataclass
 class NextDnsData:
     """NextDNS data class."""
 
 
@@ -186,15 +160,15 @@
 @dataclass
 class Profile(NextDnsData):
     """Profile class."""
 
     allowlist: list[dict[str, Any]]
     denylist: list[dict[str, Any]]
     fingerprint: str
-    id: str  # noqa: A003
+    id: str
     name: str
     parental_control: dict[str, Any]
     privacy: dict[str, Any]
     rewrites: list
     security: dict[str, Any]
     settings: dict[str, Any]
     setup: dict[str, Any]
@@ -286,15 +260,15 @@
     block_video_streaming: bool
 
 
 @dataclass
 class ProfileInfo(NextDnsData):
     """ProfileInfo class."""
 
-    id: str  # noqa: A003
+    id: str
     fingerprint: str
     name: str
 
 
 @dataclass
 class ConnectionStatus(NextDnsData):
     """ConnectionStatus class."""
```

### Comparing `nextdns-2.1.0/nextdns.egg-info/PKG-INFO` & `nextdns-3.0.0/nextdns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: nextdns
-Version: 2.1.0
+Version: 3.0.0
 Summary: Python wrapper for NextDNS API.
 Home-page: https://github.com/bieniu/nextdns
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.0
 
 [![GitHub Release][releases-shield]][releases]
 [![PyPI][pypi-releases-shield]][pypi-releases]
 [![PyPI - Downloads][pypi-downloads]][pypi-statistics]
```

### Comparing `nextdns-2.1.0/setup.py` & `nextdns-3.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """Setup module for nextdns."""
+
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "2.1.0"
+VERSION = "3.0.0"
 
 setup(
     name="nextdns",
     version=VERSION,
     author="Maciej Bieniek",
     description="Python wrapper for NextDNS API.",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/bieniu/nextdns",
     license="Apache-2.0 License",
     packages=["nextdns"],
     package_data={"nextdns": ["py.typed"]},
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     install_requires=["aiohttp>=3.7.0"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Typing :: Typed",
     ],
 )
```

