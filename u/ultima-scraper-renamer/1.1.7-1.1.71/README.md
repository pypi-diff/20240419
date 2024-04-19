# Comparing `tmp/ultima_scraper_renamer-1.1.7.tar.gz` & `tmp/ultima_scraper_renamer-1.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_renamer-1.1.7.tar", max compression
+gzip compressed data, was "ultima_scraper_renamer-1.1.71.tar", max compression
```

## Comparing `ultima_scraper_renamer-1.1.7.tar` & `ultima_scraper_renamer-1.1.71.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.7/README.md
--rw-r--r--   0        0        0      674 2024-01-06 09:30:35.836677 ultima_scraper_renamer-1.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.7/ultima_scraper_renamer/__init__.py
--rw-r--r--   0        0        0        0 2022-12-06 16:13:32.768074 ultima_scraper_renamer-1.1.7/ultima_scraper_renamer/py.typed
--rw-r--r--   0        0        0    10886 2024-01-05 21:01:51.127146 ultima_scraper_renamer-1.1.7/ultima_scraper_renamer/reformat.py
--rw-r--r--   0        0        0     7872 2023-05-14 17:44:23.086692 ultima_scraper_renamer-1.1.7/ultima_scraper_renamer/renamer.py
--rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.71/README.md
+-rw-r--r--   0        0        0      669 2024-04-19 12:23:19.723407 ultima_scraper_renamer-1.1.71/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-06 16:13:32.768074 ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/py.typed
+-rw-r--r--   0        0        0    11753 2024-04-19 12:21:59.361385 ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/reformat.py
+-rw-r--r--   0        0        0     7872 2023-05-14 17:44:23.086692 ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/renamer.py
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.1.71/PKG-INFO
```

### Comparing `ultima_scraper_renamer-1.1.7/pyproject.toml` & `ultima_scraper_renamer-1.1.71/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 [tool.poetry]
 name = "ultima-scraper-renamer"
-version = "1.1.7"
+version = "1.1.71"
 description = ""
-authors = [
-    "UltimaHoarder <1285176+UltimaHoarder@users.noreply.github.com>",
-]
+authors = ["UltimaHoarder <1285176+UltimaHoarder@users.noreply.github.com>"]
 readme = "README.md"
-packages = [{include = "ultima_scraper_renamer"}]
+packages = [{ include = "ultima_scraper_renamer" }]
 include = ["ultima_scraper_renamer/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 tqdm = "^4.64.1"
 orjson = "^3.8.3"
 ultima-scraper-api = "^2.0.0"
 ultima-scraper-collection = "^2.0.0"
 
 
-
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
 
 [build-system]
```

### Comparing `ultima_scraper_renamer-1.1.7/ultima_scraper_renamer/reformat.py` & `ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/reformat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import copy
-import os
 from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 from urllib.parse import urlparse
 
 from ultima_scraper_api.helpers import main_helper
 
 if TYPE_CHECKING:
     import ultima_scraper_api
+
+    user_types = ultima_scraper_api.user_types
     from ultima_scraper_collection.managers.filesystem_manager import (
         DirectoryManager,
         FilesystemManager,
     )
     from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
         MediaMetadata,
     )
@@ -194,14 +195,32 @@
     def __init__(
         self, authed: auth_types, filesystem_manager: FilesystemManager
     ) -> None:
         self.authed = authed
         self.filesystem_manager = filesystem_manager
         self.api = self.authed.get_api()
 
+    def prepare_user_reformat(
+        self, user: user_types, directory: Path, username: str | None = None
+    ):
+        user_username = username or user.username
+        authed = self.authed
+        assert self.filesystem_manager.directory_manager
+        site_config = self.filesystem_manager.directory_manager.site_config
+        reformat_item = ReformatItem()
+        reformat_item.site_name = authed.api.site_name
+        reformat_item.profile_username = authed.username
+        reformat_item.model_username = user_username
+        reformat_item.date = datetime.today()
+        download_setup = site_config.download_setup
+        reformat_item.date_format = download_setup.date_format
+        reformat_item.text_length = download_setup.text_length
+        reformat_item.directory = directory
+        return reformat_item
+
     def prepare_reformat(self, media_item: MediaMetadata):
         content_metadata = media_item.__content_metadata__
         final_api_type = "Uncategorized"
         content_metadata_dict: dict[str, Any] = {}
         if content_metadata:
             final_api_type = content_metadata.api_type
             content_metadata_dict = content_metadata.__dict__
```

### Comparing `ultima_scraper_renamer-1.1.7/ultima_scraper_renamer/renamer.py` & `ultima_scraper_renamer-1.1.71/ultima_scraper_renamer/renamer.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_renamer-1.1.7/PKG-INFO` & `ultima_scraper_renamer-1.1.71/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-renamer
-Version: 1.1.7
+Version: 1.1.71
 Summary: 
 Author: UltimaHoarder
 Author-email: 1285176+UltimaHoarder@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

