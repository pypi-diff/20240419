# Comparing `tmp/playwrightcapture-1.24.4.tar.gz` & `tmp/playwrightcapture-1.24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.24.4.tar", max compression
+gzip compressed data, was "playwrightcapture-1.24.5.tar", max compression
```

## Comparing `playwrightcapture-1.24.4.tar` & `playwrightcapture-1.24.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/LICENSE
--rw-r--r--   0        0        0     1441 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/README.md
--rw-r--r--   0        0        0      511 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    62432 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1764 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1487 2024-04-15 10:02:20.145546 playwrightcapture-1.24.4/pyproject.toml
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.4/PKG-INFO
+-rw-r--r--   0        0        0     1775 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/LICENSE
+-rw-r--r--   0        0        0     1441 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/README.md
+-rw-r--r--   0        0        0      511 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    63307 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1764 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1487 2024-04-19 10:36:39.457454 playwrightcapture-1.24.5/pyproject.toml
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.5/PKG-INFO
```

### Comparing `playwrightcapture-1.24.4/LICENSE` & `playwrightcapture-1.24.5/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.4/README.md` & `playwrightcapture-1.24.5/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.4/playwrightcapture/capture.py` & `playwrightcapture-1.24.5/playwrightcapture/capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 import random
 import re
 import sys
 import time
 
 from base64 import b64decode
 from io import BytesIO
+from logging import LoggerAdapter, Logger
 from tempfile import NamedTemporaryFile
-from typing import Any, TypedDict, Literal, TYPE_CHECKING
+from typing import Any, TypedDict, Literal, TYPE_CHECKING, MutableMapping
 from urllib.parse import urlparse, unquote, urljoin
 from zipfile import ZipFile
 
 import dateparser
 import requests
 import urllib3
 
@@ -75,36 +76,53 @@
 
     # One day, playwright will support getting the favicon from the capture itself
     # favicon: Optional[bytes]
     # in the meantime, we need a workaround: https://github.com/Lookyloo/PlaywrightCapture/issues/45
     potential_favicons: set[bytes] | None
 
 
+class PlaywrightCaptureLogAdapter(LoggerAdapter):  # type: ignore[type-arg]
+    """
+    Prepend log entry with the UUID of the capture
+    """
+    def process(self, msg: str, kwargs: MutableMapping[str, Any]) -> tuple[str, MutableMapping[str, Any]]:
+        if self.extra:
+            return '[{}] {}'.format(self.extra['uuid'], msg), kwargs
+        return msg, kwargs
+
+
 class Capture():
 
     _browsers: list[BROWSER] = ['chromium', 'firefox', 'webkit']
     _default_viewport: ViewportSize = {'width': 1920, 'height': 1080}
     _default_timeout: int = 90  # set to 90s by default
     _minimal_timeout: int = 15  # set to 15s - It makes little sense to attempt a capture below that limit.
 
     _requests: dict[str, bytes] = {}
 
     def __init__(self, browser: BROWSER | None=None, device_name: str | None=None,
                  proxy: str | dict[str, str] | None=None,
-                 general_timeout_in_sec: int | None = None, loglevel: str | int='INFO'):
+                 general_timeout_in_sec: int | None = None, loglevel: str | int='INFO',
+                 uuid: str | None=None):
         """Captures a page with Playwright.
 
         :param browser: The browser to use for the capture.
         :param device_name: The pre-defined device to use for the capture (from playwright).)
         :param proxy: The external proxy to use for the capture.
         :param general_timeout_in_sec: The general timeout for the capture, including children.
         :param loglevel: Python loglevel
+        :param uuid: The UUID of the capture.
         """
-        self.logger = logging.getLogger('playwrightcapture')
-        self.logger.setLevel(loglevel)
+        master_logger = logging.getLogger('playwrightcapture')
+        master_logger.setLevel(loglevel)
+        self.logger: Logger | PlaywrightCaptureLogAdapter
+        if uuid is not None:
+            self.logger = PlaywrightCaptureLogAdapter(master_logger, {'uuid': uuid})
+        else:
+            self.logger = master_logger
         self.browser_name: BROWSER = browser if browser else 'chromium'
 
         if general_timeout_in_sec is None:
             self._capture_timeout = self._default_timeout
         else:
             self._capture_timeout = general_timeout_in_sec
             if self._capture_timeout < self._minimal_timeout:
@@ -678,17 +696,14 @@
                                 raise e
                             to_return['error'] = f"Error while downloading: {error_msg}"
                             self.logger.info(to_return['error'])
                             self.should_retry = True
                         except Exception:
                             raise e
                 else:
-                    if not self._exception_is_network_error(initial_error):
-                        # TODO: Do something?
-                        self.logger.warning(f'Unexpected error: {initial_error}')
                     raise initial_error
             else:
                 await page.bring_to_front()
                 self.logger.debug('Page moved to front.')
 
                 # page instrumentation
                 await self._wait_for_random_timeout(page, 5)  # Wait 5 sec after document loaded
@@ -865,15 +880,19 @@
                 self.should_retry = True
             elif e.name in ['Download is starting',
                             'Connection closed',
                             'Navigation interrupted by another one',
                             'Navigation failed because page was closed!',
                             'Protocol error (Page.bringToFront): Not attached to an active page',
                             'Peer failed to perform TLS handshake: The TLS connection was non-properly terminated.',
-                            'Load cannot follow more than 20 redirections']:
+                            'Peer failed to perform TLS handshake: Error sending data: Connection reset by peer',
+                            'Peer sent fatal TLS alert: The server name sent was not recognized',
+                            'Load cannot follow more than 20 redirections',
+                            'Page crashed',
+                            'Error receiving data: Connection reset by peer']:
                 # Other errors, let's give it another shot
                 self.logger.info(f'Issue with {url} (retrying): {e.message}')
                 self.should_retry = True
             elif e.name in ['Target page, context or browser has been closed']:
                 # The browser barfed, let's try again
                 self.logger.info(f'Browser barfed on {url} (retrying): {e.message}')
                 self.should_retry = True
```

### Comparing `playwrightcapture-1.24.4/playwrightcapture/helpers.py` & `playwrightcapture-1.24.5/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.4/pyproject.toml` & `playwrightcapture-1.24.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.24.4"
+version = "1.24.5"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -40,13 +40,13 @@
 
 [tool.poetry.group.dev.dependencies]
 types-beautifulsoup4 = "^4.12.0.20240229"
 pytest = "^8.1.1"
 mypy = "^1.9.0"
 types-dateparser = "^1.1.4.20240331"
 types-requests = "^2.31.0.20240406"
-types-pytz = "^2024.1.0.20240203"
+types-pytz = "^2024.1.0.20240417"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `playwrightcapture-1.24.4/PKG-INFO` & `playwrightcapture-1.24.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightCapture
-Version: 1.24.4
+Version: 1.24.5
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

