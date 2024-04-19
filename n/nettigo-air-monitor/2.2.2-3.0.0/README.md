# Comparing `tmp/nettigo_air_monitor-2.2.2.tar.gz` & `tmp/nettigo_air_monitor-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nettigo_air_monitor-2.2.2.tar", last modified: Sun Nov 26 20:09:24 2023, max compression
+gzip compressed data, was "nettigo_air_monitor-3.0.0.tar", last modified: Fri Apr 19 13:53:59 2024, max compression
```

## Comparing `nettigo_air_monitor-2.2.2.tar` & `nettigo_air_monitor-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:09:24.145194 nettigo_air_monitor-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2023-11-26 20:09:24.145194 nettigo_air_monitor-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:09:24.145194 nettigo_air_monitor-2.2.2/nettigo_air_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/nettigo_air_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/nettigo_air_monitor/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/nettigo_air_monitor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/nettigo_air_monitor/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/nettigo_air_monitor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:09:24.145194 nettigo_air_monitor-2.2.2/nettigo_air_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2023-11-26 20:09:24.000000 nettigo_air_monitor-2.2.2/nettigo_air_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-11-26 20:09:24.000000 nettigo_air_monitor-2.2.2/nettigo_air_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-26 20:09:24.000000 nettigo_air_monitor-2.2.2/nettigo_air_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-26 20:09:24.000000 nettigo_air_monitor-2.2.2/nettigo_air_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-26 20:09:24.000000 nettigo_air_monitor-2.2.2/nettigo_air_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-26 20:09:24.145194 nettigo_air_monitor-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-26 20:09:24.145194 nettigo_air_monitor-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2023-11-26 20:09:07.000000 nettigo_air_monitor-2.2.2/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:53:59.030881 nettigo_air_monitor-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 13:53:59.030881 nettigo_air_monitor-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:53:59.026881 nettigo_air_monitor-3.0.0/nettigo_air_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:53:59.030881 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 13:53:58.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-19 13:53:58.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:53:58.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 13:53:58.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 13:53:58.000000 nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:53:59.030881 nettigo_air_monitor-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:53:59.026881 nettigo_air_monitor-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-04-19 13:53:51.000000 nettigo_air_monitor-3.0.0/tests/test_init.py
```

### Comparing `nettigo_air_monitor-2.2.2/LICENSE` & `nettigo_air_monitor-3.0.0/LICENSE`

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

### Comparing `nettigo_air_monitor-2.2.2/PKG-INFO` & `nettigo_air_monitor-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: nettigo_air_monitor
-Version: 2.2.2
+Version: 3.0.0
 Summary: Python wrapper for getting air quality data from Nettigo Air Monitor devices.
 Home-page: https://github.com/bieniu/nettigo-air-monitor
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
 Requires-Dist: aqipy-atmotech
 Requires-Dist: dacite>=1.7.0
 
 [![GitHub Release][releases-shield]][releases]
```

### Comparing `nettigo_air_monitor-2.2.2/README.md` & `nettigo_air_monitor-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-2.2.2/nettigo_air_monitor/__init__.py` & `nettigo_air_monitor-3.0.0/nettigo_air_monitor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Python wrapper for getting air quality data from Nettigo Air Monitor devices."""
+
 from __future__ import annotations
 
-import asyncio
 import logging
 import re
 from http import HTTPStatus
 from typing import Any
 
 from aiohttp import ClientConnectorError, ClientResponseError, ClientSession
 from aqipy import caqi_eu
@@ -105,15 +105,15 @@
             )
         except ClientResponseError as error:
             if error.status == HTTPStatus.UNAUTHORIZED.value:
                 raise AuthFailedError("Authorization has failed") from error
             raise ApiError(
                 f"Invalid response from device {self.host}: {error.status}"
             ) from error
-        except (ClientConnectorError, asyncio.TimeoutError) as error:
+        except (TimeoutError, ClientConnectorError) as error:
             _LOGGER.info("Invalid response from device: %s", self.host)
             raise NotRespondingError(
                 f"The device {self.host} is not responding"
             ) from error
 
         _LOGGER.debug("Data retrieved from %s, status: %s", self.host, resp.status)
         if resp.status != HTTPStatus.OK.value:
```

### Comparing `nettigo_air_monitor-2.2.2/nettigo_air_monitor/const.py` & `nettigo_air_monitor-3.0.0/nettigo_air_monitor/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants for nettigo-air-monitor library."""
+
 from typing import Final
 
 from aiohttp.client import ClientTimeout
 
 ATTR_CONFIG: Final[str] = "config"
 ATTR_DATA: Final[str] = "data"
 ATTR_OTA: Final[str] = "ota"
```

### Comparing `nettigo_air_monitor-2.2.2/nettigo_air_monitor/exceptions.py` & `nettigo_air_monitor-3.0.0/nettigo_air_monitor/exceptions.py`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-2.2.2/nettigo_air_monitor/model.py` & `nettigo_air_monitor-3.0.0/nettigo_air_monitor/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type definitions for NAM."""
+
 from dataclasses import dataclass
 
 import aiohttp
 
 
 @dataclass
 class ConnectionOptions:
```

### Comparing `nettigo_air_monitor-2.2.2/nettigo_air_monitor.egg-info/PKG-INFO` & `nettigo_air_monitor-3.0.0/nettigo_air_monitor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
-Name: nettigo-air-monitor
-Version: 2.2.2
+Name: nettigo_air_monitor
+Version: 3.0.0
 Summary: Python wrapper for getting air quality data from Nettigo Air Monitor devices.
 Home-page: https://github.com/bieniu/nettigo-air-monitor
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
 Requires-Dist: aqipy-atmotech
 Requires-Dist: dacite>=1.7.0
 
 [![GitHub Release][releases-shield]][releases]
```

### Comparing `nettigo_air_monitor-2.2.2/setup.py` & `nettigo_air_monitor-3.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Setup module for nettigo_air_monitor."""
+
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "2.2.2"
+VERSION = "3.0.0"
 
 setup(
     name="nettigo_air_monitor",
     version=VERSION,
     author="Maciej Bieniek",
     description=(
         "Python wrapper for getting air quality data from Nettigo Air Monitor devices."
@@ -17,22 +18,21 @@
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/bieniu/nettigo-air-monitor",
     license="Apache-2.0 License",
     packages=["nettigo_air_monitor"],
     package_data={"nettigo_air_monitor": ["py.typed"]},
-    python_requires=">=3.10",
+    python_requires=">=3.11",
     install_requires=["aiohttp>=3.7.0", "aqipy-atmotech", "dacite>=1.7.0"],
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

### Comparing `nettigo_air_monitor-2.2.2/tests/test_init.py` & `nettigo_air_monitor-3.0.0/tests/test_init.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Tests for nettigo package."""
-import asyncio
+
 import json
 from http import HTTPStatus
+from typing import Any
 from unittest.mock import Mock, patch
 
 import aiohttp
 import pytest
 from aiohttp import ClientResponseError
 from aioresponses import aioresponses
+from syrupy import SnapshotAssertion
 
 from nettigo_air_monitor import (
     ApiError,
     AuthFailedError,
     CannotGetMacError,
     ConnectionOptions,
     InvalidSensorDataError,
@@ -20,81 +22,50 @@
 
 VALID_IP = "192.168.172.12"
 INVALID_HOST = "http://nam.org"
 
 VALUES = "MAC: AA:BB:CC:DD:EE:FF<br/>"
 
 
-@pytest.mark.asyncio
-async def test_valid_data():
+@pytest.mark.asyncio()
+async def test_valid_data(
+    snapshot: SnapshotAssertion, valid_data: dict[str, Any]
+) -> None:
     """Test with valid data."""
-    with open("tests/fixtures/valid_data.json", encoding="utf-8") as file:
-        data = json.load(file)
-
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
             payload={"www_basicauth_enabled": False},
         )
         session_mock.get(
             "http://192.168.172.12/data.json",
-            payload=data,
+            payload=valid_data,
         )
         session_mock.get(
             "http://192.168.172.12/values",
             payload=VALUES,
         )
 
         nam = await NettigoAirMonitor.create(session, options)
         mac = await nam.async_get_mac_address()
-        result = await nam.async_update()
+        sensors = await nam.async_update()
 
     await session.close()
 
     assert mac == "AA:BB:CC:DD:EE:FF"
 
     assert nam.software_version == "NAMF-2020-36"
-    assert result.bme280_humidity == 85.3
-    assert result.bme280_pressure == 989.206
-    assert result.bme280_temperature == 10.6
-    assert result.bmp180_pressure == 996.784
-    assert result.bmp180_temperature == 10.8
-    assert result.bmp280_pressure == 1022.012
-    assert result.bmp280_temperature == 5.6
-    assert result.dht22_humidity == 46.2
-    assert result.dht22_temperature == 6.3
-    assert result.heca_humidity == 59.7
-    assert result.heca_temperature == 15.1
-    assert result.mhz14a_carbon_dioxide == 865
-    assert result.pms_p0 == 6
-    assert result.pms_p1 == 10
-    assert result.pms_p2 == 11
-    assert result.pms_caqi == 19
-    assert result.pms_caqi_level == "very_low"
-    assert result.sds011_p1 == 22.7
-    assert result.sds011_p2 == 20
-    assert result.sds011_caqi == 34
-    assert result.sds011_caqi_level == "low"
-    assert result.sht3x_humidity == 34.7
-    assert result.sht3x_temperature == 6.3
-    assert result.signal == -85
-    assert result.sps30_p0 == 31.2
-    assert result.sps30_p1 == 21.2
-    assert result.sps30_p2 == 34.3
-    assert result.sps30_p4 == 24.7
-    assert result.sps30_caqi == 54
-    assert result.sps30_caqi_level == "medium"
-    assert result.uptime == 45632
+    assert sensors == snapshot
 
 
-@pytest.mark.asyncio
-async def test_caqi_value():
+@pytest.mark.asyncio()
+async def test_caqi_value(snapshot: SnapshotAssertion) -> None:
     """Test CAQI value when PM10 and PM2.5 is None."""
     data = {"software_version": "NAMF-2020-36", "sensordatavalues": []}
 
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
@@ -108,87 +79,58 @@
         )
         session_mock.get(
             "http://192.168.172.12/values",
             payload=VALUES,
         )
 
         nam = await NettigoAirMonitor.create(session, options)
-        result = await nam.async_update()
+        sensors = await nam.async_update()
 
     await session.close()
 
-    assert result.sds011_p1 is None
-    assert result.sds011_p2 is None
-    assert result.sds011_caqi is None
-    assert result.sds011_caqi_level is None
-    assert result.sps30_p1 is None
-    assert result.sps30_p2 is None
-    assert result.sps30_caqi is None
-    assert result.sps30_caqi_level is None
+    assert sensors == snapshot
 
 
-@pytest.mark.asyncio
-async def test_valid_data_with_auth():
+@pytest.mark.asyncio()
+async def test_valid_data_with_auth(
+    snapshot: SnapshotAssertion, valid_data: dict[str, Any]
+) -> None:
     """Test with valid data with authorization."""
-    with open("tests/fixtures/valid_data.json", encoding="utf-8") as file:
-        data = json.load(file)
-
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP, "user", "pass")
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
             payload={"www_basicauth_enabled": True},
         )
         session_mock.get(
             "http://192.168.172.12/data.json",
-            payload=data,
+            payload=valid_data,
         )
         session_mock.get(
             "http://192.168.172.12/values",
             payload=VALUES,
         )
 
         nam = await NettigoAirMonitor.create(session, options)
         mac = await nam.async_get_mac_address()
-        result = await nam.async_update()
+        sensors = await nam.async_update()
 
     await session.close()
 
     assert mac == "AA:BB:CC:DD:EE:FF"
 
     assert nam.software_version == "NAMF-2020-36"
     assert nam.auth_enabled is True
-    assert result.bme280_humidity == 85.3
-    assert result.bme280_pressure == 989.206
-    assert result.bme280_temperature == 10.6
-    assert result.bmp180_pressure == 996.784
-    assert result.bmp180_temperature == 10.8
-    assert result.bmp280_pressure == 1022.012
-    assert result.bmp280_temperature == 5.6
-    assert result.dht22_humidity == 46.2
-    assert result.dht22_temperature == 6.3
-    assert result.heca_humidity == 59.7
-    assert result.heca_temperature == 15.1
-    assert result.mhz14a_carbon_dioxide == 865
-    assert result.sds011_p1 == 22.7
-    assert result.sds011_p2 == 20
-    assert result.sht3x_humidity == 34.7
-    assert result.sht3x_temperature == 6.3
-    assert result.signal == -85
-    assert result.sps30_p0 == 31.2
-    assert result.sps30_p1 == 21.2
-    assert result.sps30_p2 == 34.3
-    assert result.sps30_p4 == 24.7
-    assert result.uptime == 45632
+    assert sensors == snapshot
 
 
-@pytest.mark.asyncio
-async def test_auth_failed():
+@pytest.mark.asyncio()
+async def test_auth_failed() -> None:
     """Test auth failed."""
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP, "user", "pass")
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
@@ -209,16 +151,16 @@
             await nam.async_restart()
 
     assert str(excinfo.value) == "Authorization has failed"
 
     await session.close()
 
 
-@pytest.mark.asyncio
-async def test_auth_enabled():
+@pytest.mark.asyncio()
+async def test_auth_enabled() -> None:
     """Test auth failed."""
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP, "user", "pass")
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
@@ -230,16 +172,16 @@
         nam = await NettigoAirMonitor.create(session, options)
 
     await session.close()
 
     assert nam.auth_enabled is True
 
 
-@pytest.mark.asyncio
-async def test_http_404_code():
+@pytest.mark.asyncio()
+async def test_http_404_code() -> None:
     """Test request ends with error."""
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP, "user", "pass")
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
@@ -251,16 +193,16 @@
             await NettigoAirMonitor.create(session, options)
 
     assert str(excinfo.value) == "Invalid response from device 192.168.172.12: 404"
 
     await session.close()
 
 
-@pytest.mark.asyncio
-async def test_api_error():
+@pytest.mark.asyncio()
+async def test_api_error() -> None:
     """Test API error."""
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
@@ -278,16 +220,16 @@
             await nam.async_update()
 
     assert str(excinfo.value) == "Invalid response from device 192.168.172.12: 202"
 
     await session.close()
 
 
-@pytest.mark.asyncio
-async def test_cache_empty():
+@pytest.mark.asyncio()
+async def test_cache_empty() -> None:
     """Test error request when cache is empty."""
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
@@ -295,81 +237,59 @@
         )
 
         nam = await NettigoAirMonitor.create(session, options)
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/data.json",
-            exception=asyncio.TimeoutError(Mock(), Mock()),
+            exception=TimeoutError(Mock(), Mock()),
         )
 
         with pytest.raises(ApiError) as excinfo:
             await nam.async_update()
 
     assert str(excinfo.value) == "The device 192.168.172.12 is not responding"
 
     await session.close()
 
 
-@pytest.mark.asyncio
-async def test_data_cached():
+@pytest.mark.asyncio()
+async def test_data_cached(
+    snapshot: SnapshotAssertion, valid_data: dict[str, Any]
+) -> None:
     """Test error request when the data is cached."""
-    with open("tests/fixtures/valid_data.json", encoding="utf-8") as file:
-        data = json.load(file)
-
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
             payload={"www_basicauth_enabled": False},
         )
         session_mock.get(
             "http://192.168.172.12/data.json",
-            payload=data,
+            payload=valid_data,
         )
         session_mock.get(
             "http://192.168.172.12/data.json",
-            exception=asyncio.TimeoutError(Mock(), Mock()),
+            exception=TimeoutError(Mock(), Mock()),
         )
 
         nam = await NettigoAirMonitor.create(session, options)
         await nam.async_update()
-        result = await nam.async_update()
+        sensors = await nam.async_update()
 
     await session.close()
 
     assert nam.software_version == "NAMF-2020-36"
-    assert result.bme280_humidity == 85.3
-    assert result.bme280_pressure == 989.206
-    assert result.bme280_temperature == 10.6
-    assert result.bmp180_pressure == 996.784
-    assert result.bmp180_temperature == 10.8
-    assert result.bmp280_pressure == 1022.012
-    assert result.bmp280_temperature == 5.6
-    assert result.dht22_humidity == 46.2
-    assert result.dht22_temperature == 6.3
-    assert result.heca_humidity == 59.7
-    assert result.heca_temperature == 15.1
-    assert result.mhz14a_carbon_dioxide == 865
-    assert result.sds011_p1 == 22.7
-    assert result.sds011_p2 == 20
-    assert result.sht3x_humidity == 34.7
-    assert result.sht3x_temperature == 6.3
-    assert result.signal == -85
-    assert result.sps30_p0 == 31.2
-    assert result.sps30_p1 == 21.2
-    assert result.sps30_p2 == 34.3
-    assert result.sps30_p4 == 24.7
-    assert result.uptime == 45632
+    assert sensors == snapshot
 
 
-@pytest.mark.asyncio
-async def test_invalid_sensor_data():
+@pytest.mark.asyncio()
+async def test_invalid_sensor_data() -> None:
     """Test InvalidSensorDataError."""
     with open("tests/fixtures/invalid_data.json", encoding="utf-8") as file:
         data = json.load(file)
 
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP)
 
@@ -391,16 +311,16 @@
             await nam.async_update()
 
     assert str(excinfo.value) == "Invalid sensor data"
 
     await session.close()
 
 
-@pytest.mark.asyncio
-async def test_cannot_get_mac():
+@pytest.mark.asyncio()
+async def test_cannot_get_mac() -> None:
     """Test CannotGetMacError error."""
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
@@ -419,36 +339,36 @@
             await nam.async_get_mac_address()
 
     assert str(excinfo.value) == "Cannot get MAC address from device"
 
     await session.close()
 
 
-@pytest.mark.asyncio
-async def test_init_device_not_repond():
+@pytest.mark.asyncio()
+async def test_init_device_not_repond() -> None:
     """Test init when device is not responding."""
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
-            exception=asyncio.TimeoutError(Mock(), Mock()),
+            exception=TimeoutError(Mock(), Mock()),
         )
 
         with pytest.raises(ApiError) as excinfo:
             await NettigoAirMonitor.create(session, options)
 
     assert str(excinfo.value) == "The device 192.168.172.12 is not responding"
 
     await session.close()
 
 
-@pytest.mark.asyncio
-async def test_get_ma_device_not_repond():
+@pytest.mark.asyncio()
+async def test_get_ma_device_not_repond() -> None:
     """Test get_mac when device is not responding."""
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
@@ -456,73 +376,76 @@
         )
 
         nam = await NettigoAirMonitor.create(session, options)
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/values",
-            exception=asyncio.TimeoutError(Mock(), Mock()),
+            exception=TimeoutError(Mock(), Mock()),
         )
 
         with pytest.raises(ApiError) as excinfo:
             await nam.async_get_mac_address()
 
     await session.close()
 
     assert str(excinfo.value) == "The device 192.168.172.12 is not responding"
 
 
-@pytest.mark.asyncio
-async def test_username_without_password():
+@pytest.mark.asyncio()
+async def test_username_without_password() -> None:
     """Test error when username is provided without password."""
     with pytest.raises(
         ValueError, match="Supply both username and password"
     ) as excinfo:
         ConnectionOptions(VALID_IP, "user")
 
     assert str(excinfo.value) == "Supply both username and password"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 @pytest.mark.parametrize(
     ("method", "endpoint"), [("async_restart", "reset"), ("async_ota_update", "ota")]
 )
-async def test_post_methods(method, endpoint):
+async def test_post_methods(method: str, endpoint: str) -> None:
     """Test post methods."""
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP)
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
             payload={"www_basicauth_enabled": False},
         )
 
         nam = await NettigoAirMonitor.create(session, options)
 
-    with aioresponses() as session_mock, patch(
-        "nettigo_air_monitor.NettigoAirMonitor._async_http_request"
-    ) as mock_request:
+    with (
+        aioresponses() as session_mock,
+        patch(
+            "nettigo_air_monitor.NettigoAirMonitor._async_http_request"
+        ) as mock_request,
+    ):
         session_mock.post(f"http://192.168.172.12/{endpoint}")
 
         method_to_call = getattr(nam, method)
         await method_to_call()
 
     await session.close()
 
     assert mock_request.call_count == 1
     assert mock_request.call_args[0][0] == "post"
     assert mock_request.call_args[0][1] == f"http://192.168.172.12/{endpoint}"
 
 
-@pytest.mark.asyncio
+@pytest.mark.asyncio()
 @pytest.mark.parametrize(
     ("method", "endpoint"), [("async_restart", "reset"), ("async_ota_update", "ota")]
 )
-async def test_post_methods_fail(method, endpoint):
+async def test_post_methods_fail(method: str, endpoint: str) -> None:
     """Test fail of the post methods."""
     session = aiohttp.ClientSession()
     options = ConnectionOptions(VALID_IP, "user", "pass")
 
     with aioresponses() as session_mock:
         session_mock.get(
             "http://192.168.172.12/config.json",
@@ -530,15 +453,15 @@
         )
 
         nam = await NettigoAirMonitor.create(session, options)
 
     with aioresponses() as session_mock:
         session_mock.post(
             f"http://192.168.172.12/{endpoint}",
-            exception=asyncio.TimeoutError(Mock(), Mock()),
+            exception=TimeoutError(Mock(), Mock()),
         )
 
         method_to_call = getattr(nam, method)
         with pytest.raises(ApiError) as excinfo:
             await method_to_call()
 
     assert str(excinfo.value) == "The device 192.168.172.12 is not responding"
```

