# Comparing `tmp/pystac-client-0.7.6.tar.gz` & `tmp/pystac_client-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac-client-0.7.6.tar", last modified: Wed Feb 28 14:03:21 2024, max compression
+gzip compressed data, was "pystac_client-0.7.7.tar", last modified: Fri Apr 19 13:07:43 2024, max compression
```

## Comparing `pystac-client-0.7.6.tar` & `pystac_client-0.7.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:03:21.105512 pystac-client-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-28 14:03:01.000000 pystac-client-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-28 14:03:01.000000 pystac-client-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-02-28 14:03:21.105512 pystac-client-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-28 14:03:01.000000 pystac-client-0.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:03:21.097512 pystac-client-0.7.6/pystac_client/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    26259 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/conformance.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    32806 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/item_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/stac_api_io.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-02-28 14:03:01.000000 pystac-client-0.7.6/pystac_client/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:03:21.101512 pystac-client-0.7.6/pystac_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-02-28 14:03:21.000000 pystac-client-0.7.6/pystac_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-28 14:03:21.000000 pystac-client-0.7.6/pystac_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 14:03:21.000000 pystac-client-0.7.6/pystac_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-28 14:03:21.000000 pystac-client-0.7.6/pystac_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-28 14:03:21.000000 pystac-client-0.7.6/pystac_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-28 14:03:21.000000 pystac-client-0.7.6/pystac_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 14:03:21.105512 pystac-client-0.7.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:03:21.101512 pystac-client-0.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-02-28 14:03:01.000000 pystac-client-0.7.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    26178 2024-02-28 14:03:01.000000 pystac-client-0.7.6/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-02-28 14:03:01.000000 pystac-client-0.7.6/tests/test_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    29723 2024-02-28 14:03:01.000000 pystac-client-0.7.6/tests/test_item_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2024-02-28 14:03:01.000000 pystac-client-0.7.6/tests/test_stac_api_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:07:43.132527 pystac_client-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 13:07:19.000000 pystac_client-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 13:07:19.000000 pystac_client-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-19 13:07:43.132527 pystac_client-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-19 13:07:19.000000 pystac_client-0.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:07:43.128527 pystac_client-0.7.7/pystac_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26442 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32798 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/item_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/stac_api_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-19 13:07:19.000000 pystac_client-0.7.7/pystac_client/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:07:43.128527 pystac_client-0.7.7/pystac_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 13:07:43.000000 pystac_client-0.7.7/pystac_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:07:43.132527 pystac_client-0.7.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:07:43.128527 pystac_client-0.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-19 13:07:19.000000 pystac_client-0.7.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27234 2024-04-19 13:07:19.000000 pystac_client-0.7.7/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-19 13:07:19.000000 pystac_client-0.7.7/tests/test_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29723 2024-04-19 13:07:19.000000 pystac_client-0.7.7/tests/test_item_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-19 13:07:19.000000 pystac_client-0.7.7/tests/test_stac_api_io.py
```

### Comparing `pystac-client-0.7.6/LICENSE` & `pystac_client-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.6/PKG-INFO` & `pystac_client-0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 Metadata-Version: 2.1
 Name: pystac-client
-Version: 0.7.6
+Version: 0.7.7
 Summary: Python library for working with SpatioTemporal Asset Catalog (STAC) APIs.
 Author-email: Jon Duckworth <duckontheweb@gmail.com>, Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac-client
 Project-URL: documentation, https://pystac-client.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac-client.git
 Project-URL: changelog, https://github.com/stac-utils/pystac-client/blob/main/CHANGELOG.md
 Project-URL: discussions, https://github.com/radiantearth/stac-spec/discussions/categories/stac-software
 Keywords: pystac,imagery,raster,catalog,STAC
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.28.2
-Requires-Dist: pystac[validation]>=1.8.2
+Requires-Dist: pystac[validation]>=1.10.0
 Requires-Dist: python-dateutil>=2.8.2
 Provides-Extra: dev
 Requires-Dist: black~=24.0; extra == "dev"
 Requires-Dist: codespell~=2.2.4; extra == "dev"
 Requires-Dist: coverage~=7.2; extra == "dev"
 Requires-Dist: doc8~=1.1.1; extra == "dev"
 Requires-Dist: importlib-metadata~=7.0; extra == "dev"
 Requires-Dist: mypy~=1.2; extra == "dev"
 Requires-Dist: orjson~=3.8; extra == "dev"
 Requires-Dist: pre-commit~=3.2; extra == "dev"
 Requires-Dist: pytest-benchmark~=4.0.0; extra == "dev"
 Requires-Dist: pytest-console-scripts~=1.4.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
+Requires-Dist: pytest-cov~=5.0; extra == "dev"
 Requires-Dist: pytest-recording~=0.13; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: recommonmark~=0.7.1; extra == "dev"
-Requires-Dist: requests-mock~=1.11.0; extra == "dev"
-Requires-Dist: ruff==0.2.2; extra == "dev"
+Requires-Dist: requests-mock~=1.12; extra == "dev"
+Requires-Dist: ruff==0.4.0; extra == "dev"
 Requires-Dist: tomli~=2.0; python_version < "3.11" and extra == "dev"
-Requires-Dist: types-python-dateutil~=2.8.19; extra == "dev"
+Requires-Dist: types-python-dateutil<2.10.0,>=2.8.19; extra == "dev"
 Requires-Dist: types-requests~=2.31.0; extra == "dev"
 Requires-Dist: urllib3<2; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: Sphinx~=6.2; extra == "docs"
 Requires-Dist: boto3~=1.26; extra == "docs"
 Requires-Dist: cartopy~=0.21; extra == "docs"
 Requires-Dist: geojson~=3.1.0; extra == "docs"
```

### Comparing `pystac-client-0.7.6/README.md` & `pystac_client-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.6/pyproject.toml` & `pystac_client-0.7.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 ]
 maintainers = [{ name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }]
 keywords = ["pystac", "imagery", "raster", "catalog", "STAC"]
 license = { text = "Apache-2.0" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "requests>=2.28.2",
-    "pystac[validation]>=1.8.2",
+    "pystac[validation]>=1.10.0",
     "python-dateutil>=2.8.2",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 stac-client = "pystac_client.cli:cli"
 
@@ -44,22 +44,22 @@
     "doc8~=1.1.1",
     "importlib-metadata~=7.0",
     "mypy~=1.2",
     "orjson~=3.8",
     "pre-commit~=3.2",
     "pytest-benchmark~=4.0.0",
     "pytest-console-scripts~=1.4.0",
-    "pytest-cov~=4.1.0",
+    "pytest-cov~=5.0",
     "pytest-recording~=0.13",
     "pytest~=8.0",
     "recommonmark~=0.7.1",
-    "requests-mock~=1.11.0",
-    "ruff==0.2.2",
+    "requests-mock~=1.12",
+    "ruff==0.4.0",
     "tomli~=2.0; python_version<'3.11'",
-    "types-python-dateutil~=2.8.19",
+    "types-python-dateutil>=2.8.19,<2.10.0",
     "types-requests~=2.31.0",
     # temporary pin https://github.com/stac-utils/pystac-client/issues/509
     "urllib3<2",
 ]
 docs = [
     "Sphinx~=6.2",
     "boto3~=1.26",
```

### Comparing `pystac-client-0.7.6/pystac_client/_utils.py` & `pystac_client-0.7.7/pystac_client/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import warnings
-from typing import Callable, Optional, Union
+from typing import Any, Callable, Dict, Optional, Union
 
 import pystac
 
 from pystac_client.errors import IgnoredResultWarning
 
-Modifiable = Union[pystac.Collection, pystac.Item, pystac.ItemCollection, dict]
+Modifiable = Union[
+    pystac.Collection, pystac.Item, pystac.ItemCollection, Dict[Any, Any]
+]
 
 
 def call_modifier(
     modifier: Optional[Callable[[Modifiable], None]], obj: Modifiable
 ) -> None:
     """Calls the user's modifier and validates that the result is None."""
     if modifier is None:
```

### Comparing `pystac-client-0.7.6/pystac_client/cli.py` & `pystac_client-0.7.7/pystac_client/cli.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.6/pystac_client/client.py` & `pystac_client-0.7.7/pystac_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     cast,
 )
 
 import pystac
 import pystac.utils
 import pystac.validation
 from pystac import CatalogType, Collection
+from pystac.layout import APILayoutStrategy, HrefLayoutStrategy
 from requests import Request
 
 from pystac_client._utils import Modifiable, call_modifier
 from pystac_client.collection_client import CollectionClient
 from pystac_client.conformance import ConformanceClasses
 from pystac_client.errors import ClientTypeError
 from pystac_client.exceptions import APIError
@@ -57,36 +58,39 @@
     <https://github.com/radiantearth/stac-spec/blob/master/catalog-spec/catalog-spec.md>`_
     APIs that have a ``"conformsTo"`` indicate that it supports additional
     functionality on top of a normal STAC Catalog,
     such as searching items (e.g., /search endpoint).
     """
 
     _stac_io: Optional[StacApiIO]
+    _fallback_strategy: HrefLayoutStrategy = APILayoutStrategy()
 
     def __init__(
         self,
         id: str,
         description: str,
         title: Optional[str] = None,
         stac_extensions: Optional[List[str]] = None,
         extra_fields: Optional[Dict[str, Any]] = None,
         href: Optional[str] = None,
         catalog_type: CatalogType = CatalogType.ABSOLUTE_PUBLISHED,
+        strategy: Optional[HrefLayoutStrategy] = None,
         *,
         modifier: Optional[Callable[[Modifiable], None]] = None,
         **kwargs: Dict[str, Any],
     ):
         super().__init__(
             id,
             description,
             title=title,
             stac_extensions=stac_extensions,
             extra_fields=extra_fields,
             href=href,
             catalog_type=catalog_type,
+            strategy=strategy,
             **kwargs,
         )
         self.modifier = modifier
 
     def __repr__(self) -> str:
         return "<Client id={}>".format(self.id)
 
@@ -514,16 +518,16 @@
                 the response, it will automatically retry with
                 ``"GET"`` for all subsequent requests.
             max_items : The maximum number of items to return from the search, even
                 if there are more matching results. This client to limit the
                 total number of Items returned from the :meth:`items`,
                 :meth:`item_collections`, and :meth:`items_as_dicts methods`. The client
                 will continue to request pages of items until the number of max items is
-                reached. This parameter defaults to 100. Setting this to ``None`` will
-                allow iteration over a possibly very large number of results.
+                reached. Setting this to ``None`` will allow iteration over a possibly
+                very large number of results.
             limit: A recommendation to the service as to the number of items to return
                 *per page* of results. Defaults to 100.
             ids: List of one or more Item ids to filter on.
             collections: List of one or more Collection IDs or
                 :class:`pystac.Collection` instances. Only Items in one
                 of the provided Collections will be searched
             bbox: A list, tuple, or iterator representing a bounding box of 2D
```

### Comparing `pystac-client-0.7.6/pystac_client/collection_client.py` & `pystac_client-0.7.7/pystac_client/collection_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     List,
     Optional,
     Union,
     cast,
 )
 
 import pystac
+from pystac.layout import APILayoutStrategy, HrefLayoutStrategy
 
 from pystac_client._utils import Modifiable, call_modifier
 from pystac_client.conformance import ConformanceClasses
 from pystac_client.exceptions import APIError
 from pystac_client.item_search import ItemSearch
 from pystac_client.mixins import QueryablesMixin
 from pystac_client.stac_api_io import StacApiIO
@@ -28,14 +29,15 @@
 
     from pystac_client import Client
 
 
 class CollectionClient(pystac.Collection, QueryablesMixin):
     modifier: Callable[[Modifiable], None]
     _stac_io: StacApiIO
+    _fallback_strategy: HrefLayoutStrategy = APILayoutStrategy()
 
     def __init__(
         self,
         id: str,
         description: str,
         extent: pystac.Extent,
         title: Optional[str] = None,
@@ -43,32 +45,35 @@
         href: Optional[str] = None,
         extra_fields: Optional[Dict[str, Any]] = None,
         catalog_type: Optional[pystac.CatalogType] = None,
         license: str = "proprietary",
         keywords: Optional[List[str]] = None,
         providers: Optional[List[pystac.Provider]] = None,
         summaries: Optional[pystac.Summaries] = None,
+        assets: Optional[Dict[str, pystac.Asset]] = None,
+        strategy: Optional[HrefLayoutStrategy] = None,
         *,
         modifier: Optional[Callable[[Modifiable], None]] = None,
         **kwargs: Dict[str, Any],
     ):
-        # TODO(pystac==1.6.0): Add `assets` as a regular keyword
         super().__init__(
             id,
             description,
             extent,
             title,
             stac_extensions,
             href,
             extra_fields,
             catalog_type,
             license,
             keywords,
             providers,
             summaries,
+            assets,
+            strategy,
             **kwargs,
         )
         # error: Cannot assign to a method  [assignment]
         # https://github.com/python/mypy/issues/2427
         setattr(self, "modifier", modifier)
 
     @classmethod
```

### Comparing `pystac-client-0.7.6/pystac_client/conformance.py` & `pystac_client-0.7.7/pystac_client/conformance.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.6/pystac_client/item_search.py` & `pystac_client-0.7.7/pystac_client/item_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     r"(?P<remainder>([Tt])\d{2}:\d{2}:\d{2}(\.\d+)?"
     r"(?P<tz_info>[Zz]|([-+])(\d{2}):(\d{2}))?)?)?)?$"
 )
 
 
 class GeoInterface(Protocol):
     @property
-    def __geo_interface__(self) -> Dict[str, Any]:
-        ...
+    def __geo_interface__(self) -> Dict[str, Any]: ...
 
 
 DatetimeOrTimestamp = Optional[Union[datetime_, str]]
 Datetime = str
 DatetimeLike = Union[
     DatetimeOrTimestamp,
     Tuple[DatetimeOrTimestamp, DatetimeOrTimestamp],
```

### Comparing `pystac-client-0.7.6/pystac_client/mixins.py` & `pystac_client-0.7.7/pystac_client/mixins.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.6/pystac_client/stac_api_io.py` & `pystac_client-0.7.7/pystac_client/stac_api_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,18 @@
             prepped = self.session.prepare_request(modified or request)
             msg = f"{prepped.method} {prepped.url} Headers: {prepped.headers}"
             if method == "POST":
                 msg += f" Payload: {json.dumps(request.json)}"
             if self.timeout is not None:
                 msg += f" Timeout: {self.timeout}"
             logger.debug(msg)
-            resp = self.session.send(prepped, timeout=self.timeout)
+            send_kwargs = self.session.merge_environment_settings(
+                prepped.url, proxies={}, stream=None, verify=True, cert=None
+            )
+            resp = self.session.send(prepped, timeout=self.timeout, **send_kwargs)
         except Exception as err:
             logger.debug(err)
             raise APIError(str(err))
         if resp.status_code != 200:
             raise APIError.from_response(resp)
         try:
             return resp.content.decode("utf-8")
```

### Comparing `pystac-client-0.7.6/pystac_client/warnings.py` & `pystac_client-0.7.7/pystac_client/warnings.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.6/pystac_client.egg-info/PKG-INFO` & `pystac_client-0.7.7/pystac_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 Metadata-Version: 2.1
 Name: pystac-client
-Version: 0.7.6
+Version: 0.7.7
 Summary: Python library for working with SpatioTemporal Asset Catalog (STAC) APIs.
 Author-email: Jon Duckworth <duckontheweb@gmail.com>, Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac-client
 Project-URL: documentation, https://pystac-client.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac-client.git
 Project-URL: changelog, https://github.com/stac-utils/pystac-client/blob/main/CHANGELOG.md
 Project-URL: discussions, https://github.com/radiantearth/stac-spec/discussions/categories/stac-software
 Keywords: pystac,imagery,raster,catalog,STAC
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.28.2
-Requires-Dist: pystac[validation]>=1.8.2
+Requires-Dist: pystac[validation]>=1.10.0
 Requires-Dist: python-dateutil>=2.8.2
 Provides-Extra: dev
 Requires-Dist: black~=24.0; extra == "dev"
 Requires-Dist: codespell~=2.2.4; extra == "dev"
 Requires-Dist: coverage~=7.2; extra == "dev"
 Requires-Dist: doc8~=1.1.1; extra == "dev"
 Requires-Dist: importlib-metadata~=7.0; extra == "dev"
 Requires-Dist: mypy~=1.2; extra == "dev"
 Requires-Dist: orjson~=3.8; extra == "dev"
 Requires-Dist: pre-commit~=3.2; extra == "dev"
 Requires-Dist: pytest-benchmark~=4.0.0; extra == "dev"
 Requires-Dist: pytest-console-scripts~=1.4.0; extra == "dev"
-Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
+Requires-Dist: pytest-cov~=5.0; extra == "dev"
 Requires-Dist: pytest-recording~=0.13; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: recommonmark~=0.7.1; extra == "dev"
-Requires-Dist: requests-mock~=1.11.0; extra == "dev"
-Requires-Dist: ruff==0.2.2; extra == "dev"
+Requires-Dist: requests-mock~=1.12; extra == "dev"
+Requires-Dist: ruff==0.4.0; extra == "dev"
 Requires-Dist: tomli~=2.0; python_version < "3.11" and extra == "dev"
-Requires-Dist: types-python-dateutil~=2.8.19; extra == "dev"
+Requires-Dist: types-python-dateutil<2.10.0,>=2.8.19; extra == "dev"
 Requires-Dist: types-requests~=2.31.0; extra == "dev"
 Requires-Dist: urllib3<2; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: Sphinx~=6.2; extra == "docs"
 Requires-Dist: boto3~=1.26; extra == "docs"
 Requires-Dist: cartopy~=0.21; extra == "docs"
 Requires-Dist: geojson~=3.1.0; extra == "docs"
```

### Comparing `pystac-client-0.7.6/pystac_client.egg-info/SOURCES.txt` & `pystac_client-0.7.7/pystac_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.6/tests/test_cli.py` & `pystac_client-0.7.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.6/tests/test_client.py` & `pystac_client-0.7.7/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -708,7 +708,47 @@
 
 @pytest.mark.vcr
 def test_non_recursion_on_fallback() -> None:
     path = "https://raw.githubusercontent.com/stac-utils/pystac/v1.9.0/docs/example-catalog/catalog.json"
     catalog = Client.from_file(path)
     with pytest.warns(FallbackToPystac):
         [i for i in catalog.get_items()]
+
+
+@pytest.mark.vcr
+def test_fallback_strategy() -> None:
+    """Make sure links get recreated correctly using APILayoutStrategy."""
+
+    client = Client.open(
+        "https://planetarycomputer.microsoft.com/api/stac/v1/",
+    )
+    col = client.get_collection("landsat-c2-l2")
+    item = next(col.get_items())
+
+    item_href = item.self_href
+    col_href = col.self_href
+    root_href = client.self_href
+
+    col.links = []
+    item.links = []
+
+    client.add_child(col)
+    col.add_item(item)
+
+    assert col.self_href == col_href
+
+    assert (col_parent := col.get_single_link("parent"))
+    assert col_parent.href == root_href
+
+    assert (col_root := col.get_single_link("root"))
+    assert col_root.href == root_href
+
+    assert item.self_href == item_href
+
+    assert (item_col := item.get_single_link("collection"))
+    assert item_col.href == col_href
+
+    assert (item_parent := item.get_single_link("parent"))
+    assert item_parent.href == col_href
+
+    assert (item_root := item.get_single_link("root"))
+    assert item_root.href == root_href
```

### Comparing `pystac-client-0.7.6/tests/test_collection_client.py` & `pystac_client-0.7.7/tests/test_collection_client.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.6/tests/test_item_search.py` & `pystac_client-0.7.7/tests/test_item_search.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.6/tests/test_stac_api_io.py` & `pystac_client-0.7.7/tests/test_stac_api_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing
 from pathlib import Path
 from urllib.parse import parse_qs, urlsplit
 
 import pytest
+from pytest import MonkeyPatch
 from requests_mock.mocker import Mocker
 
 from pystac_client.exceptions import APIError
 from pystac_client.stac_api_io import StacApiIO
 
 from .helpers import STAC_URLS
 
@@ -262,7 +263,14 @@
     @pytest.mark.vcr
     def test_timeout_smoke_test(self) -> None:
         # Testing timeout behavior is hard, so we just have a simple smoke test to make
         # sure that providing a timeout doesn't break anything.
         stac_api_io = StacApiIO(timeout=42)
         response = stac_api_io.read_text(STAC_URLS["PLANETARY-COMPUTER"])
         assert isinstance(response, str)
+
+    @pytest.mark.parametrize("name", ("REQUESTS_CA_BUNDLE", "CURL_CA_BUNDLE"))
+    def test_respect_env_for_certs(self, monkeypatch: MonkeyPatch, name: str) -> None:
+        monkeypatch.setenv(name, "/not/a/real/file")
+        stac_api_io = StacApiIO()
+        with pytest.raises(APIError):
+            stac_api_io.request("https://earth-search.aws.element84.com/v1/")
```

