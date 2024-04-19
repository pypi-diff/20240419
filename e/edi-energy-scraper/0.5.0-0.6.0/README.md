# Comparing `tmp/edi_energy_scraper-0.5.0.tar.gz` & `tmp/edi_energy_scraper-0.6.0.tar.gz`

## Comparing `edi_energy_scraper-0.5.0.tar` & `edi_energy_scraper-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/README.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/mwe.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/requirements.txt
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/tox.ini
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.github/workflows/black.yml
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-test_packaging.in
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-test_packaging.txt
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/src/_edi_energy_scraper_version.py
--rw-r--r--   0        0        0    17371 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/src/edi_energy_scraper/__init__.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/src/edi_energy_scraper/epoch.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/src/edi_energy_scraper/py.typed
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/LICENSE
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 edi_energy_scraper-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/README.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/mwe.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/requirements.txt
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/tox.ini
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.github/workflows/black.yml
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-test_packaging.in
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-test_packaging.txt
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/src/_edi_energy_scraper_version.py
+-rw-r--r--   0        0        0    21186 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/src/edi_energy_scraper/__init__.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/src/edi_energy_scraper/epoch.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/src/edi_energy_scraper/py.typed
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 edi_energy_scraper-0.6.0/PKG-INFO
```

### Comparing `edi_energy_scraper-0.5.0/.pre-commit-config.yaml` & `edi_energy_scraper-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/README.md` & `edi_energy_scraper-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/requirements.txt` & `edi_energy_scraper-0.6.0/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile pyproject.toml
 #
-aiodns==3.1.1
+aiodns==3.2.0
     # via aiohttp
-aiohttp[speedups]==3.9.3
+aiohttp[speedups]==3.9.4
     # via
     #   aiohttp-requests
     #   edi_energy_scraper (pyproject.toml)
 aiohttp-requests==0.2.3
     # via edi_energy_scraper (pyproject.toml)
 aiosignal==1.3.1
     # via aiohttp
@@ -26,15 +26,15 @@
     # via pycares
 coworker==2.0.1
     # via aiohttp-requests
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-idna==3.6
+idna==3.7
     # via yarl
 marshmallow==3.21.1
     # via maus
 maus==0.4.2
     # via edi_energy_scraper (pyproject.toml)
 more-itertools==10.2.0
     # via maus
@@ -42,17 +42,17 @@
     # via
     #   aiohttp
     #   yarl
 packaging==24.0
     # via marshmallow
 pycares==4.4.0
     # via aiodns
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pypdf==4.1.0
+pypdf==4.2.0
     # via edi_energy_scraper (pyproject.toml)
 pytz==2024.1
     # via edi_energy_scraper (pyproject.toml)
 soupsieve==2.5
     # via beautifulsoup4
 yarl==1.9.4
     # via aiohttp
```

### Comparing `edi_energy_scraper-0.5.0/tox.ini` & `edi_energy_scraper-0.6.0/tox.ini`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/.github/dependabot.yml` & `edi_energy_scraper-0.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/.github/workflows/black.yml` & `edi_energy_scraper-0.6.0/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/.github/workflows/codeql-analysis.yml` & `edi_energy_scraper-0.6.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/.github/workflows/coverage.yml` & `edi_energy_scraper-0.6.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/.github/workflows/dependabot_automerge.yml` & `edi_energy_scraper-0.6.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/.github/workflows/packaging_test.yml` & `edi_energy_scraper-0.6.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/.github/workflows/python-publish.yml` & `edi_energy_scraper-0.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/.github/workflows/pythonlint.yml` & `edi_energy_scraper-0.6.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/.github/workflows/unittests.yml` & `edi_energy_scraper-0.6.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/dev_requirements/requirements-test_packaging.txt` & `edi_energy_scraper-0.6.0/dev_requirements/requirements-test_packaging.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 #
 # This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile dev_requirements/requirements-test_packaging.in
 #
-build==1.1.1
-    # via -r dev_requirements/requirements-test_packaging.in
+build==1.2.1
+    # via -r requirements-test_packaging.in
 certifi==2024.2.2
     # via requests
+cffi==1.16.0
+    # via cryptography
 charset-normalizer==3.3.2
     # via requests
+cryptography==42.0.5
+    # via secretstorage
 docutils==0.20.1
     # via readme-renderer
-idna==3.6
+idna==3.7
     # via requests
 importlib-metadata==7.1.0
     # via twine
 jaraco-classes==3.3.1
     # via keyring
 jaraco-context==4.3.0
     # via keyring
 jaraco-functools==4.0.0
     # via keyring
+jeepney==0.8.0
+    # via
+    #   keyring
+    #   secretstorage
 keyring==25.0.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
@@ -34,14 +42,16 @@
     #   jaraco-functools
 nh3==0.2.17
     # via readme-renderer
 packaging==24.0
     # via build
 pkginfo==1.10.0
     # via twine
+pycparser==2.22
+    # via cffi
 pygments==2.17.2
     # via
     #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
 readme-renderer==43.0
@@ -52,15 +62,17 @@
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.7.1
     # via twine
+secretstorage==3.3.3
+    # via keyring
 twine==5.0.0
-    # via -r dev_requirements/requirements-test_packaging.in
+    # via -r requirements-test_packaging.in
 urllib3==2.2.1
     # via
     #   requests
     #   twine
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `edi_energy_scraper-0.5.0/dev_requirements/requirements-tests.txt` & `edi_energy_scraper-0.6.0/dev_requirements/requirements-tests.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #
 # This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile dev_requirements/requirements-tests.in
 #
-aiohttp==3.9.3
+aiohttp==3.9.4
     # via aioresponses
 aioresponses==0.7.6
-    # via -r dev_requirements/requirements-tests.in
+    # via -r requirements-tests.in
 aiosignal==1.3.1
     # via aiohttp
 attrs==23.2.0
     # via aiohttp
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
-idna==3.6
+idna==3.7
     # via yarl
 iniconfig==2.0.0
     # via pytest
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 packaging==24.0
     # via pytest
 pluggy==1.4.0
     # via pytest
 pytest==8.1.1
     # via
-    #   -r dev_requirements/requirements-tests.in
+    #   -r requirements-tests.in
     #   pytest-asyncio
     #   pytest-datafiles
     #   pytest-mock
 pytest-asyncio==0.22.0
-    # via -r dev_requirements/requirements-tests.in
+    # via -r requirements-tests.in
 pytest-datafiles==3.0.0
-    # via -r dev_requirements/requirements-tests.in
+    # via -r requirements-tests.in
 pytest-mock==3.14.0
-    # via -r dev_requirements/requirements-tests.in
+    # via -r requirements-tests.in
 yarl==1.9.4
     # via aiohttp
```

### Comparing `edi_energy_scraper-0.5.0/src/edi_energy_scraper/__init__.py` & `edi_energy_scraper-0.6.0/src/edi_energy_scraper/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import itertools
 import logging
 import os
 import re
 from email.message import Message
 from pathlib import Path
 from random import randint
-from typing import Awaitable, Dict, List, Optional, Set, Tuple, Union
+from typing import Awaitable, Dict, List, Optional, Set, Union
 
 import aiohttp
 import pytz
 from aiohttp import ServerDisconnectedError
 from aiohttp_requests import Requests  # type:ignore[import]
 from bs4 import BeautifulSoup, Comment  # type:ignore[import]
 from maus.edifact import EdifactFormat, EdifactFormatVersion, get_edifact_format_version
@@ -66,15 +66,15 @@
         if not url.startswith("http"):
             url = f"{self._root_url}/{url.strip('/')}"  # remove trailing slashes from relative link
         response = await self.requests.get(url, timeout=5)
         soup = BeautifulSoup(await response.text(), "html.parser")
         EdiEnergyScraper.remove_comments(soup)
         return soup
 
-    async def _download_and_save_pdf(self, file_basename: str, link: str) -> Path:
+    async def _download_and_save_pdf(self, file_basename: str, link: str) -> List[Path]:
         """
         Downloads a PDF file from a given link and stores it under the file name in a folder that has the same name
         as the directory if the pdf does not exist yet or if the metadata has changed since the last download.
         Returns the path to the downloaded pdf.
         """
         if not link.startswith("http"):
             link = f"{self._root_url}/{link.strip('/')}"  # remove trailing slashes from relative link
@@ -102,52 +102,70 @@
                 break
             except asyncio.TimeoutError:
                 _logger.exception("Timeout while reading content of '%s'", file_name, exc_info=True)
                 if number_of_tries <= 0:
                     raise
                 await asyncio.sleep(delay=randint(5, 10))  # cool down...
 
-        file_path = self._get_file_path(file_name=file_name)
-        Path.mkdir(file_path.parent, parents=True, exist_ok=True)
+        file_paths = self._get_file_paths(file_name=file_name)
+        for file_path in file_paths:
+            Path.mkdir(file_path.parent, parents=True, exist_ok=True)
+
+            # Save file if it does not exist yet
+            if not os.path.isfile(file_path):
+                with open(file_path, "wb+") as outfile:  # pdfs are written as binaries
+                    _logger.debug("Saving new PDF %s", file_path)
+                    outfile.write(response_content)
+                continue
 
-        # Save file if it does not exist yet
-        if not os.path.isfile(file_path):
-            with open(file_path, "wb+") as outfile:  # pdfs are written as binaries
-                _logger.debug("Saving new PDF %s", file_path)
-                outfile.write(response_content)
-            return file_path
-
-        # First fix, different file types do just the same as before, only with correct file extension
-        if not file_name.endswith(".pdf"):
-            with open(file_path, "wb+") as outfile:
-                _logger.debug("Saving %s", file_path)
-                outfile.write(response_content)
-            return file_path
-
-        # Check if metadata has changed
-        metadata_has_changed = self._have_different_metadata(response_content, file_path)
-        if metadata_has_changed:  # delete old file and replace with new one
-            _logger.debug("Metadata for PDF %s changed; Replacing it", file_path)
-            os.remove(file_path)
-            with open(file_path, "wb+") as outfile:  # pdfs are written as binaries
-                outfile.write(response_content)
-        else:
-            _logger.debug("Meta data haven't changed for %s", file_path)
-        return file_path
+            # First fix, different file types do just the same as before, only with correct file extension
+            if not file_name.endswith(".pdf"):
+                with open(file_path, "wb+") as outfile:
+                    _logger.debug("Saving %s", file_path)
+                    outfile.write(response_content)
+                continue
+
+            # Check if metadata has changed
+            metadata_has_changed = self._have_different_metadata(response_content, file_path)
+            if metadata_has_changed:  # delete old file and replace with new one
+                _logger.debug("Metadata for PDF %s changed; Replacing it", file_path)
+                os.remove(file_path)
+                with open(file_path, "wb+") as outfile:  # pdfs are written as binaries
+                    outfile.write(response_content)
+            else:
+                _logger.debug("Meta data haven't changed for %s", file_path)
+        return file_paths
 
     def _get_file_path(self, file_name: str) -> Path:
         if "/" in file_name:
             raise ValueError(f"file names must not contain slashes: '{file_name}'")
         format_version: EdifactFormatVersion = get_edifact_version_from_filename(path=Path(file_name))
         file_path = Path(self._root_dir).joinpath(
             f"{format_version}/{file_name}"  # e.g "{root_dir}/future/ahbmabis_99991231_20210401.pdf"
         )
 
         return file_path
 
+    def _get_file_paths(self, file_name: str) -> List[Path]:
+        """
+        Returns a list of file paths for all valid format versions of a given file.
+        """
+
+        file_paths = []
+
+        format_version_range = get_edifact_format_version_range_from_filename(path=Path(file_name))
+
+        for format_version in format_version_range:
+            file_path = Path(self._root_dir).joinpath(
+                f"{format_version}/{file_name}"  # e.g "{root_dir}/FV2310/ahbmabis_99991231_20210401.pdf"
+            )
+            file_paths.append(file_path)
+
+        return file_paths
+
     @staticmethod
     def _add_file_extension_to_file_basename(headers: dict, file_basename: str) -> str:
         """Extracts the extension of a file from a response header and add it to the file basename."""
         content_disposition = headers["Content-Disposition"]
         params = Message()
         params["content-type"] = content_disposition
         file_extension = Path(str(params.get_param("filename"))).suffix
@@ -290,15 +308,15 @@
             _logger.debug("Removing %s which has been removed online", path)
             os.remove(path)
 
         return no_longer_online_files
 
     async def _download(
         self, file_basename: str, link: str, optional_success_msg: Optional[str] = None
-    ) -> Optional[Path]:
+    ) -> Optional[List[Path]]:
         try:
             file_path = await self._download_and_save_pdf(file_basename=file_basename, link=link)
             if optional_success_msg is not None:
                 _logger.debug(optional_success_msg)
         except KeyError as key_error:
             if key_error.args[0].lower() == "content-disposition":
                 _logger.exception("Failed to download '%s'", file_basename, exc_info=True)
@@ -330,28 +348,28 @@
         for _epoch, epoch_link in epoch_links.items():
             _logger.info("Processing %s", _epoch)
             epoch_soup = await self._get_soup(epoch_link)
             epoch_path: Path = Path(self._root_dir, f"{_epoch}.html")  # e.g. "future.html"
             with open(epoch_path, "w+", encoding="utf8") as outfile:
                 outfile.write(epoch_soup.prettify())
             file_map = EdiEnergyScraper.get_epoch_file_map(epoch_soup)
-            download_tasks: List[Awaitable[Optional[Path]]] = []
+            download_tasks: List[Awaitable[Optional[List[Path]]]] = []
             file_counter = itertools.count()
             for file_basename, link in file_map.items():
                 download_tasks.append(
                     self._download(
                         file_basename,
                         link,
                         f"Successfully downloaded {_epoch} file {next(file_counter)}/{len(file_map)}",
                     )
                 )
-            download_results: List[Optional[Path]] = await asyncio.gather(*download_tasks)
+            download_results: List[Optional[List[Path]]] = await asyncio.gather(*download_tasks)
             for download_result in download_results:
                 if download_result is not None:
-                    new_file_paths.add(download_result)
+                    new_file_paths.update(download_result)
         self.remove_no_longer_online_files(new_file_paths)
         _logger.info("Finished mirroring")
 
 
 def get_edifact_version_from_filename(path: Path) -> EdifactFormatVersion:
     """
     Determines the edifact formats and the version of a given file.
@@ -364,7 +382,92 @@
     date_string = filename.split("_")[-1]  # Assuming date is in the last part of filename
     date_format = "%Y%m%d"
     berlin = pytz.timezone("Europe/Berlin")
     berlin_local_time = datetime.datetime.strptime(date_string, date_format).astimezone(berlin)
     format_version = get_edifact_format_version(berlin_local_time)
 
     return format_version
+
+
+def get_publication_date_from_filename(path: Path) -> datetime.datetime:
+    """
+    Determines the publication date of a given file.
+    """
+    filename = path.stem
+    publication_date_string = filename.split("_")[-1]  # Assuming date is the "publication date"
+    date_format = "%Y%m%d"
+    berlin = pytz.timezone("Europe/Berlin")
+    publication_date = datetime.datetime.strptime(publication_date_string, date_format).astimezone(berlin)
+
+    return publication_date
+
+
+def get_valid_to_date_from_filename(path: Path) -> datetime.datetime:
+    """
+    Determines the valid to date of a given file.
+    """
+    filename = path.stem
+    valid_to_date_string = filename.split("_")[-2]  # Assuming date is the "valid to" date
+
+    if valid_to_date_string == "99991231":
+        return datetime.datetime(9999, 12, 31, tzinfo=datetime.timezone.utc)
+
+    date_format = "%Y%m%d"
+    berlin = pytz.timezone("Europe/Berlin")
+    valid_to_date = datetime.datetime.strptime(valid_to_date_string, date_format).astimezone(berlin)
+
+    return valid_to_date
+
+
+def get_current_format_version() -> EdifactFormatVersion:
+    """
+    Determines the current format version.
+    """
+    return get_edifact_format_version(datetime.datetime.now(tz=datetime.timezone.utc))
+
+
+def get_next_format_version() -> EdifactFormatVersion:
+    """
+    Determines the next format version.
+    """
+    current_format_version = get_edifact_format_version(datetime.datetime.now(tz=datetime.timezone.utc))
+
+    format_versions = [efv.value for efv in EdifactFormatVersion]
+    next_format_version = format_versions[format_versions.index(current_format_version.value) + 1]
+
+    return EdifactFormatVersion(next_format_version)
+
+
+def get_edifact_format_version_range_from_filename(path: Path) -> List[EdifactFormatVersion]:
+    """
+    Determines range of valid format versions of a given file.
+    A document can be valid for multiple format versions.
+    Therefore, a list of all valid format versions is returned.
+
+    example:
+      - 'IFTSTAMIG2.0e_20240930_20231001.pdf' -> [FV2310, FV2404]
+      - 'IFTSTAMIG2.0e_99991231_20231001.pdf' -> [FV2310, FV2404, ...]  all future format versions
+    """
+
+    publication_date: datetime.datetime = get_publication_date_from_filename(path)
+    valid_to_date: datetime.datetime = get_valid_to_date_from_filename(path)
+
+    next_format_version = get_next_format_version()
+
+    format_version_start = get_edifact_format_version(publication_date)
+
+    format_version_end = get_edifact_format_version(valid_to_date)
+
+    is_format_version_end_greater_than_next_format_version = format_version_end > next_format_version
+    if is_format_version_end_greater_than_next_format_version:
+        format_version_end = next_format_version
+
+    format_versions = [efv.value for efv in EdifactFormatVersion]
+
+    format_version_range = [
+        EdifactFormatVersion(format_version)
+        for format_version in format_versions[
+            format_versions.index(format_version_start.value) : format_versions.index(format_version_end.value) + 1
+        ]
+    ]
+
+    return format_version_range
```

### Comparing `edi_energy_scraper-0.5.0/src/edi_energy_scraper/epoch.py` & `edi_energy_scraper-0.6.0/src/edi_energy_scraper/epoch.py`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/.gitignore` & `edi_energy_scraper-0.6.0/.gitignore`

 * *Files 25% similar despite different names*

```diff
@@ -124,11 +124,40 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
+# General
+.DS_Store
+.AppleDouble
+.LSOverride
+
+# Icon must end with two \r
+Icon
+
+
+# Thumbnails
+._*
+
+# Files that might appear in the root of a volume
+.DocumentRevisions-V100
+.fseventsd
+.Spotlight-V100
+.TemporaryItems
+.Trashes
+.VolumeIcon.icns
+.com.apple.timemachine.donotpresent
+
+# Directories potentially created on remote AFP share
+.AppleDB
+.AppleDesktop
+Network Trash Folder
+Temporary Items
+.apdisk
+
+
 .idea/
 
 # vscode settings
 .vscode/
```

### Comparing `edi_energy_scraper-0.5.0/LICENSE` & `edi_energy_scraper-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/pyproject.toml` & `edi_energy_scraper-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edi_energy_scraper-0.5.0/PKG-INFO` & `edi_energy_scraper-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: edi_energy_scraper
-Version: 0.5.0
+Version: 0.6.0
 Summary: a scraper to mirror edi-energy.de
 Project-URL: Changelog, https://github.com/Hochfrequenz/edi_energy_scraper/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/edi_energy_scraper
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info+github@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
 Keywords: ahb,automation,bdew,edi@energy
```

