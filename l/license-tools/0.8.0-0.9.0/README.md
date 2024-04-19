# Comparing `tmp/license_tools-0.8.0.tar.gz` & `tmp/license_tools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_tools-0.8.0.tar", last modified: Wed Feb 28 11:58:41 2024, max compression
+gzip compressed data, was "license_tools-0.9.0.tar", last modified: Sat Mar 23 11:05:27 2024, max compression
```

## Comparing `license_tools-0.8.0.tar` & `license_tools-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,53 @@
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2024-02-28 11:58:41.982160 license_tools-0.8.0/
--rw-r--r--   0 sdostal   (6000) users      (100)    11358 2022-05-16 19:23:11.000000 license_tools-0.8.0/LICENSE.txt
--rw-r--r--   0 sdostal   (6000) users      (100)      210 2024-02-12 16:31:04.000000 license_tools-0.8.0/MANIFEST.in
--rw-r--r--   0 sdostal   (6000) users      (100)     7663 2024-02-28 11:58:41.982160 license_tools-0.8.0/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)     6350 2024-02-28 11:41:07.000000 license_tools-0.8.0/README.md
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2024-02-28 11:58:41.970160 license_tools-0.8.0/license_tools/
--rw-r--r--   0 sdostal   (6000) users      (100)        0 2021-01-11 15:34:09.000000 license_tools-0.8.0/license_tools/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)     3547 2024-02-14 13:40:58.000000 license_tools-0.8.0/license_tools/__main__.py
--rw-r--r--   0 sdostal   (6000) users      (100)        1 2023-08-21 12:26:22.000000 license_tools-0.8.0/license_tools/py.typed
--rw-r--r--   0 sdostal   (6000) users      (100)    19903 2024-02-16 08:50:02.000000 license_tools-0.8.0/license_tools/retrieval.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2024-02-28 11:58:41.970160 license_tools-0.8.0/license_tools/tools/
--rw-r--r--   0 sdostal   (6000) users      (100)        0 2024-01-10 13:29:52.000000 license_tools-0.8.0/license_tools/tools/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)     8874 2024-02-12 08:56:44.000000 license_tools-0.8.0/license_tools/tools/font_tools.py
--rw-r--r--   0 sdostal   (6000) users      (100)     2328 2024-01-22 14:50:21.000000 license_tools-0.8.0/license_tools/tools/linking_tools.py
--rw-r--r--   0 sdostal   (6000) users      (100)     2489 2024-02-16 08:48:39.000000 license_tools-0.8.0/license_tools/tools/pip_tools.py
--rw-r--r--   0 sdostal   (6000) users      (100)    22508 2024-01-12 10:50:11.000000 license_tools-0.8.0/license_tools/tools/rpm_tools.py
--rw-r--r--   0 sdostal   (6000) users      (100)     9778 2024-02-12 08:50:18.000000 license_tools-0.8.0/license_tools/tools/scancode_tools.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2024-02-28 11:58:41.974160 license_tools-0.8.0/license_tools/utils/
--rw-r--r--   0 sdostal   (6000) users      (100)        0 2024-01-09 12:23:19.000000 license_tools-0.8.0/license_tools/utils/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)     1753 2024-01-15 11:59:39.000000 license_tools-0.8.0/license_tools/utils/archive_utils.py
--rw-r--r--   0 sdostal   (6000) users      (100)     1772 2024-02-12 09:42:53.000000 license_tools-0.8.0/license_tools/utils/path_utils.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2024-02-28 11:58:41.970160 license_tools-0.8.0/license_tools.egg-info/
--rw-r--r--   0 sdostal   (6000) users      (100)     7663 2024-02-28 11:58:41.000000 license_tools-0.8.0/license_tools.egg-info/PKG-INFO
--rw-r--r--   0 sdostal   (6000) users      (100)     1348 2024-02-28 11:58:41.000000 license_tools-0.8.0/license_tools.egg-info/SOURCES.txt
--rw-r--r--   0 sdostal   (6000) users      (100)        1 2024-02-28 11:58:41.000000 license_tools-0.8.0/license_tools.egg-info/dependency_links.txt
--rw-r--r--   0 sdostal   (6000) users      (100)      219 2024-02-28 11:58:41.000000 license_tools-0.8.0/license_tools.egg-info/requires.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       14 2024-02-28 11:58:41.000000 license_tools-0.8.0/license_tools.egg-info/top_level.txt
--rw-r--r--   0 sdostal   (6000) users      (100)       61 2024-02-06 13:50:57.000000 license_tools-0.8.0/pyproject.toml
--rw-r--r--   0 sdostal   (6000) users      (100)       38 2024-02-28 11:58:41.982160 license_tools-0.8.0/setup.cfg
--rw-r--r--   0 sdostal   (6000) users      (100)     1744 2024-02-28 11:57:14.000000 license_tools-0.8.0/setup.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2024-02-28 11:58:41.974160 license_tools-0.8.0/tests/
--rw-r--r--   0 sdostal   (6000) users      (100)     1510 2024-02-16 09:22:59.000000 license_tools-0.8.0/tests/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)    18409 2024-02-16 09:22:59.000000 license_tools-0.8.0/tests/data.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2024-02-28 11:58:41.978160 license_tools-0.8.0/tests/files/
--rw-r--r--   0 sdostal   (6000) users      (100)   593908 2023-05-02 23:59:44.000000 license_tools-0.8.0/tests/files/Carlito-Regular.ttf
--rw-r--r--   0 sdostal   (6000) users      (100)   189956 2023-11-29 21:28:14.000000 license_tools-0.8.0/tests/files/Font Awesome 6 Free-Regular-400.otf
--rw-r--r--   0 sdostal   (6000) users      (100)      687 2023-12-08 10:24:43.000000 license_tools-0.8.0/tests/files/LICENSE.md
--rw-r--r--   0 sdostal   (6000) users      (100)     4515 2023-12-08 10:03:54.000000 license_tools-0.8.0/tests/files/LICENSE_Carlito-Regular.txt
--rw-r--r--   0 sdostal   (6000) users      (100)     7427 2023-11-29 21:28:14.000000 license_tools-0.8.0/tests/files/LICENSE_Font Awesome 6 Free-Regular-400.txt
--rw-r--r--   0 sdostal   (6000) users      (100)     7427 2023-11-29 21:28:14.000000 license_tools-0.8.0/tests/files/LICENSE_fa-solid-900.txt
--rw-r--r--   0 sdostal   (6000) users      (100)     4495 2023-12-08 10:17:28.000000 license_tools-0.8.0/tests/files/LICENSE_weathericons-regular-webfont.txt
--rw-r--r--   0 sdostal   (6000) users      (100)   156496 2023-11-29 21:28:14.000000 license_tools-0.8.0/tests/files/fa-solid-900.woff2
--rw-r--r--   0 sdostal   (6000) users      (100)    56468 2023-12-08 10:14:15.000000 license_tools-0.8.0/tests/files/weathericons-regular-webfont.woff
--rw-r--r--   0 sdostal   (6000) users      (100)    33528 2024-02-16 09:24:10.000000 license_tools-0.8.0/tests/test_retrieval.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2024-02-28 11:58:41.978160 license_tools-0.8.0/tests/tools/
--rw-r--r--   0 sdostal   (6000) users      (100)        0 2024-01-10 13:30:22.000000 license_tools-0.8.0/tests/tools/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)    17505 2024-02-16 09:22:59.000000 license_tools-0.8.0/tests/tools/test_font_tools.py
--rw-r--r--   0 sdostal   (6000) users      (100)     5403 2024-02-16 09:22:59.000000 license_tools-0.8.0/tests/tools/test_linking_tools.py
--rw-r--r--   0 sdostal   (6000) users      (100)     3444 2024-02-16 09:22:59.000000 license_tools-0.8.0/tests/tools/test_pip_tools.py
--rw-r--r--   0 sdostal   (6000) users      (100)    31938 2024-02-16 09:23:47.000000 license_tools-0.8.0/tests/tools/test_rpm_tools.py
--rw-r--r--   0 sdostal   (6000) users      (100)    10184 2024-02-16 09:23:49.000000 license_tools-0.8.0/tests/tools/test_scancode_tools.py
-drwxr-xr-x   0 sdostal   (6000) users      (100)        0 2024-02-28 11:58:41.982160 license_tools-0.8.0/tests/utils/
--rw-r--r--   0 sdostal   (6000) users      (100)        0 2024-01-09 12:45:44.000000 license_tools-0.8.0/tests/utils/__init__.py
--rw-r--r--   0 sdostal   (6000) users      (100)    19354 2024-02-16 09:22:59.000000 license_tools-0.8.0/tests/utils/test_archive_utils.py
--rw-r--r--   0 sdostal   (6000) users      (100)     2670 2024-02-12 09:35:48.000000 license_tools-0.8.0/tests/utils/test_path_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:27.191201 license_tools-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-23 11:05:20.000000 license_tools-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-23 11:05:20.000000 license_tools-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-03-23 11:05:27.191201 license_tools-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-03-23 11:05:20.000000 license_tools-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:27.183201 license_tools-0.9.0/license_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19903 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:27.183201 license_tools-0.9.0/license_tools/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/tools/font_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/tools/linking_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/tools/pip_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22508 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/tools/rpm_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/tools/scancode_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:27.183201 license_tools-0.9.0/license_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/utils/archive_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-23 11:05:20.000000 license_tools-0.9.0/license_tools/utils/path_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:27.187201 license_tools-0.9.0/license_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-03-23 11:05:27.000000 license_tools-0.9.0/license_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-23 11:05:27.000000 license_tools-0.9.0/license_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 11:05:27.000000 license_tools-0.9.0/license_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-23 11:05:27.000000 license_tools-0.9.0/license_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-23 11:05:27.000000 license_tools-0.9.0/license_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-23 11:05:20.000000 license_tools-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 11:05:27.191201 license_tools-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-23 11:05:20.000000 license_tools-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:27.183201 license_tools-0.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:27.187201 license_tools-0.9.0/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (127)   593908 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/files/Carlito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   189956 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/files/Font Awesome 6 Free-Regular-400.otf
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/files/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/files/LICENSE_Carlito-Regular.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/files/LICENSE_Font Awesome 6 Free-Regular-400.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/files/LICENSE_fa-solid-900.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/files/LICENSE_weathericons-regular-webfont.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   156496 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/files/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    56468 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/files/weathericons-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    33528 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/test_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:27.187201 license_tools-0.9.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17505 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/tools/test_font_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/tools/test_linking_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/tools/test_pip_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31938 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/tools/test_rpm_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/tools/test_scancode_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:27.187201 license_tools-0.9.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/utils/test_archive_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-03-23 11:05:20.000000 license_tools-0.9.0/tests/utils/test_path_utils.py
```

### Comparing `license_tools-0.8.0/LICENSE.txt` & `license_tools-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/PKG-INFO` & `license_tools-0.9.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,25 @@
-Metadata-Version: 2.1
-Name: license_tools
-Version: 0.8.0
-Summary: Collection of tools for working with Open Source licenses
-Home-page: https://github.com/stefan6419846/license_tools
-Author: stefan6419846
-License: Apache-2.0
-Keywords: open source,license,package,dependency,licensing
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: scancode-toolkit
-Requires-Dist: typecode-libmagic
-Requires-Dist: joblib
-Requires-Dist: fontTools[woff]
-Requires-Dist: pip-licenses-lib
-Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flake8-bugbear; extra == "dev"
-Requires-Dist: pep8-naming; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: requests; extra == "dev"
-Requires-Dist: types-requests; extra == "dev"
-Requires-Dist: importlib_resources; python_version < "3.9" and extra == "dev"
-Provides-Extra: extended-rpm
-Requires-Dist: rpmfile; extra == "extended-rpm"
-
 # License tools
 
 Collection of tools for working with Open Source licenses, focusing on Python packages.
 
-## Features
+## About
+
+This tool initially started as some convenience wrapper around the [ScanCode toolkit](https://github.com/nexB/scancode-toolkit/) by nexB Inc. to be used as either a standalone CLI or library. In the meantime, I added some functionality which involves further tooling sometimes irrelevant for ScanCode, sometimes not (yet) implemented there.
 
-At the moment, this primarily provides some convenience wrappers around the [ScanCode toolkit](https://github.com/nexB/scancode-toolkit/) by nexB Inc. to be used as either as standalone CLI or library.
+I wrote this tool to simplify the initial scanning steps for third-party packages, mostly tailored to my specific use-cases. For this reason, some implementation or representation details might be opionated and rather tailored to my specific needs. I decided to make this library available as a dedicated package nevertheless, as easy-to-use license compliance (scanner) tooling is sparse, while everyone should care about such topics. If you think that something can be generalized or improved, feel free to open a corresponding issue to discuss this before possibly getting started with an actual PR.
+
+## Features
 
 * Automatically download a specific Python package from PyPI and analyze it.
 * Aggregate how often each license has been used inside the current artifact.
 * Look into shared object files and ELF binaries to see what they are linking to (dynamically).
 * Look into font files to easily analyze their metadata.
 * Look into RPM file metadata.
+* Look into Python package metadata.
 * Recursively look into nested archives, for example by unpacking the actual upstream source code archives inside RPM (source) files.
 * Make everything available from the terminal.
 
 ## Installation
 
 You can install this package from PyPI:
 
@@ -67,70 +37,73 @@
 python -m license_tools --help
 ```
 
 Example: To see the licenses of a specific *pypdf* package version, use something like this:
 
 ```bash
 $ python -m license_tools --package "pypdf==3.4.17"
-              pypdf-3.17.4.dist-info/LICENSE                                    BSD-3-Clause [100.0]
-             pypdf-3.17.4.dist-info/METADATA                                    BSD-3-Clause [99.0]
-               pypdf-3.17.4.dist-info/RECORD                                    
-                pypdf-3.17.4.dist-info/WHEEL                                    
-                           pypdf/__init__.py                                    
-                              pypdf/_cmap.py                                    
-                   pypdf/_codecs/__init__.py                                    
-               pypdf/_codecs/adobe_glyphs.py                                    BSD-3-Clause [100.0]
-                     pypdf/_codecs/pdfdoc.py                                    
-                        pypdf/_codecs/std.py                                    
-                     pypdf/_codecs/symbol.py                                    
-                   pypdf/_codecs/zapfding.py                                    
-          pypdf/_crypt_providers/__init__.py                                    BSD-3-Clause [100.0]
-             pypdf/_crypt_providers/_base.py                                    BSD-3-Clause [100.0]
-     pypdf/_crypt_providers/_cryptography.py                                    BSD-3-Clause [100.0]
-         pypdf/_crypt_providers/_fallback.py                                    BSD-3-Clause [100.0]
-     pypdf/_crypt_providers/_pycryptodome.py                                    BSD-3-Clause [100.0]
-                        pypdf/_encryption.py                                    BSD-3-Clause [100.0]
-                            pypdf/_merger.py                                    BSD-3-Clause [100.0]
-                              pypdf/_page.py                                    BSD-3-Clause [100.0]
-                       pypdf/_page_labels.py                                    
-                         pypdf/_protocols.py                                    
-                            pypdf/_reader.py                                    BSD-3-Clause [100.0]
-          pypdf/_text_extraction/__init__.py                                    
-                             pypdf/_utils.py                                    BSD-3-Clause [100.0]
-                           pypdf/_version.py                                    
-                            pypdf/_writer.py                                    BSD-3-Clause [100.0]
-                pypdf/_xobj_image_helpers.py                                    
-               pypdf/annotations/__init__.py                                    
-                  pypdf/annotations/_base.py                                    
-    pypdf/annotations/_markup_annotations.py                                    
-pypdf/annotations/_non_markup_annotations.py                                    
-                          pypdf/constants.py                                    
-                             pypdf/errors.py                                    
-                            pypdf/filters.py                                    BSD-3-Clause [100.0]
-                   pypdf/generic/__init__.py                                    BSD-3-Clause [100.0]
-                      pypdf/generic/_base.py                                    BSD-3-Clause [100.0]
-           pypdf/generic/_data_structures.py                                    BSD-3-Clause [100.0]
-                       pypdf/generic/_fit.py                                    
-                   pypdf/generic/_outline.py                                    
-                 pypdf/generic/_rectangle.py                                    
-                     pypdf/generic/_utils.py                                    
-                pypdf/generic/_viewerpref.py                                    BSD-3-Clause [100.0]
-                          pypdf/pagerange.py                                    BSD-3-Clause [99.0]
-                         pypdf/papersizes.py                                    
-                              pypdf/py.typed                                    
-                              pypdf/types.py                                    
-                                pypdf/xmp.py                                    
+              pypdf-3.17.4.dist-info/LICENSE                            BSD-3-Clause [100.0]
+             pypdf-3.17.4.dist-info/METADATA                            BSD-3-Clause [99.0]
+               pypdf-3.17.4.dist-info/RECORD                            
+                pypdf-3.17.4.dist-info/WHEEL                            
+                           pypdf/__init__.py                            
+                              pypdf/_cmap.py                            
+                   pypdf/_codecs/__init__.py                            
+               pypdf/_codecs/adobe_glyphs.py                            BSD-3-Clause [100.0]
+                     pypdf/_codecs/pdfdoc.py                            
+                        pypdf/_codecs/std.py                            
+                     pypdf/_codecs/symbol.py                            
+                   pypdf/_codecs/zapfding.py                            
+          pypdf/_crypt_providers/__init__.py                            BSD-3-Clause [100.0]
+             pypdf/_crypt_providers/_base.py                            BSD-3-Clause [100.0]
+     pypdf/_crypt_providers/_cryptography.py                            BSD-3-Clause [100.0]
+         pypdf/_crypt_providers/_fallback.py                            BSD-3-Clause [100.0]
+     pypdf/_crypt_providers/_pycryptodome.py                            BSD-3-Clause [100.0]
+                        pypdf/_encryption.py                            BSD-3-Clause [100.0]
+                            pypdf/_merger.py                            BSD-3-Clause [100.0]
+                              pypdf/_page.py                            BSD-3-Clause [100.0]
+                       pypdf/_page_labels.py                            
+                         pypdf/_protocols.py                            
+                            pypdf/_reader.py                            BSD-3-Clause [100.0]
+          pypdf/_text_extraction/__init__.py                            
+                             pypdf/_utils.py                            BSD-3-Clause [100.0]
+                           pypdf/_version.py                            
+                            pypdf/_writer.py                            BSD-3-Clause [100.0]
+                pypdf/_xobj_image_helpers.py                            
+               pypdf/annotations/__init__.py                            
+                  pypdf/annotations/_base.py                            
+    pypdf/annotations/_markup_annotations.py                            
+pypdf/annotations/_non_markup_annotations.py                            
+                          pypdf/constants.py                            
+                             pypdf/errors.py                            
+                            pypdf/filters.py                            BSD-3-Clause [100.0]
+                   pypdf/generic/__init__.py                            BSD-3-Clause [100.0]
+                      pypdf/generic/_base.py                            BSD-3-Clause [100.0]
+           pypdf/generic/_data_structures.py                            BSD-3-Clause [100.0]
+                       pypdf/generic/_fit.py                            
+                   pypdf/generic/_outline.py                            
+                 pypdf/generic/_rectangle.py                            
+                     pypdf/generic/_utils.py                            
+                pypdf/generic/_viewerpref.py                            BSD-3-Clause [100.0]
+                          pypdf/pagerange.py                            BSD-3-Clause [99.0]
+                         pypdf/papersizes.py                            
+                              pypdf/py.typed                            
+                              pypdf/types.py                            
+                                pypdf/xmp.py                            
 
-====================================================================================================
+=============================================================================================
 
                                                           BSD-3-Clause  20
                                                                   None  28
 ```
 
-If you want to use the package as a library, have a look at the `license_tools.retrieval.run` method for example to see how everything interacts.
+If you want to use the package as a library, have a look at the `license_tools.retrieval.run` method for example to see how everything interacts. In general:
+
+* `license_tools.retrieval` implements most of the CLI/glue code for handling the different source types and starting the actual scanning process as well as displaying the results.
+* `license_tools.tools` implements most of the actual checks and wrappers for the third-party libraries used for scanning/checking.
 
 ## License
 
 This package is subject to the terms of the Apache-2.0 license.
 
 ## Disclaimer
```

### Comparing `license_tools-0.8.0/license_tools/__main__.py` & `license_tools-0.9.0/license_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/license_tools/retrieval.py` & `license_tools-0.9.0/license_tools/retrieval.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/license_tools/tools/font_tools.py` & `license_tools-0.9.0/license_tools/tools/font_tools.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/license_tools/tools/linking_tools.py` & `license_tools-0.9.0/license_tools/tools/linking_tools.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/license_tools/tools/pip_tools.py` & `license_tools-0.9.0/license_tools/tools/pip_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,19 @@
     """
     Analyze the Python package metadata for the given directory.
 
     :param path: The directory to analyze. Should either be a `.dist-info` one or the parent.
     :return: The package metadata.
     """
     path = Path(path)
-    if not path.suffix == ".dist-info":
-        path = next(path.glob("*.dist-info"))
+    if path.suffix not in {".dist-info", ".egg-info"}:
+        try:
+            path = next(path.glob("*.dist-info"))
+        except StopIteration:
+            path = next(path.rglob("*.egg-info"))
     distribution = PathDistribution(path)
     return get_package_info(distribution)
 
 
 def check_metadata(path: Path | str) -> str:
     """
     Render the relevant details for the given package.
```

### Comparing `license_tools-0.8.0/license_tools/tools/rpm_tools.py` & `license_tools-0.9.0/license_tools/tools/rpm_tools.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/license_tools/tools/scancode_tools.py` & `license_tools-0.9.0/license_tools/tools/scancode_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,17 +151,19 @@
     score: float
     start_line: int
     end_line: int
     matched_length: int
     match_coverage: float
     matcher: str
     license_expression: str
+    spdx_license_expression: str
     rule_identifier: str
     rule_relevance: int
     rule_url: str | None
+    from_file: str | None
     matched_text: str | None = None
 
 
 @dataclass
 class LicenseClue(LicenseMatch):
     """
     Enriched matching information about a license.
@@ -173,14 +175,15 @@
 @dataclass
 class LicenseDetection:
     """
     Information on a specific detected license.
     """
 
     license_expression: str
+    license_expression_spdx: str
     identifier: str
     matches: list[LicenseMatch] = dataclass_field(default_factory=list)
 
     def __post_init__(self) -> None:
         self.matches = [LicenseMatch(**x) if not isinstance(x, LicenseMatch) else x for x in self.matches]  # type: ignore[arg-type]
 
 
@@ -203,15 +206,19 @@
         self.license_clues = [
             LicenseClue(**x) if not isinstance(x, LicenseClue) else x for x in self.license_clues  # type: ignore[arg-type]
         ]
 
     def get_scores_of_detected_license_expression_spdx(self) -> list[float]:
         scores = []
         for detection in self.license_detections:
-            if detection.license_expression == self.detected_license_expression:
+            if (
+                detection.license_expression == self.detected_license_expression
+                or detection.license_expression_spdx
+                == self.detected_license_expression_spdx
+            ):
                 for match in detection.matches:
                     scores.append(match.score)
                 return scores
         return scores
 
 
 @dataclass
@@ -290,15 +297,17 @@
     homepage_url: str | None = None
     keywords: list[str] = dataclass_field(default_factory=list)
     license_detections: list[LicenseDetection] = dataclass_field(default_factory=list)
     md5: str | None = None
     name: str | None = None
     namespace: str | None = None
     notice_text: str | None = None
-    other_license_detections: list[LicenseDetection] = dataclass_field(default_factory=list)
+    other_license_detections: list[LicenseDetection] = dataclass_field(
+        default_factory=list
+    )
     other_license_expression: str | None = None
     other_license_expression_spdx: str | None = None
     parties: list[Party] = dataclass_field(default_factory=list)
     primary_language: str | None = None
     purl: str | None = None
     qualifiers: dict[str, str] = dataclass_field(default_factory=dict)
     release_date: datetime.date | None = None
@@ -322,20 +331,20 @@
             LicenseDetection(**x) if not isinstance(x, LicenseDetection) else x for x in self.other_license_detections  # type: ignore[arg-type]
         ]
         self.parties = [
             Party(**x) if not isinstance(x, Party) else x for x in self.parties  # type: ignore[arg-type]
         ]
 
     @classmethod
-    def from_rpm(cls, path: Path) -> 'PackageResults':
+    def from_rpm(cls, path: Path) -> "PackageResults":
         # Drop some keys which we do not handle for now.
         data = next(RpmArchiveHandler.parse(path)).to_dict()
-        data.pop('dependencies', None)
-        data.pop('extra_data', None)
-        data.pop('file_references', None)
+        data.pop("dependencies", None)
+        data.pop("extra_data", None)
+        data.pop("file_references", None)
         return cls(**data)
 
 
 def cleanup(directory: Path | str) -> None:
     """
     Remove the given directory.
     """
```

### Comparing `license_tools-0.8.0/license_tools/utils/archive_utils.py` & `license_tools-0.9.0/license_tools/utils/archive_utils.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/license_tools/utils/path_utils.py` & `license_tools-0.9.0/license_tools/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/license_tools.egg-info/PKG-INFO` & `license_tools-0.9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: license-tools
-Version: 0.8.0
+Name: license_tools
+Version: 0.9.0
 Summary: Collection of tools for working with Open Source licenses
 Home-page: https://github.com/stefan6419846/license_tools
 Author: stefan6419846
 License: Apache-2.0
 Keywords: open source,license,package,dependency,licensing
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -13,43 +13,48 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: scancode-toolkit
+Requires-Dist: scancode-toolkit>=32.1.0
 Requires-Dist: typecode-libmagic
 Requires-Dist: joblib
 Requires-Dist: fontTools[woff]
 Requires-Dist: pip-licenses-lib
+Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: flake8-bugbear; extra == "dev"
 Requires-Dist: pep8-naming; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
-Requires-Dist: requests; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: importlib_resources; python_version < "3.9" and extra == "dev"
 Provides-Extra: extended-rpm
 Requires-Dist: rpmfile; extra == "extended-rpm"
 
 # License tools
 
 Collection of tools for working with Open Source licenses, focusing on Python packages.
 
-## Features
+## About
+
+This tool initially started as some convenience wrapper around the [ScanCode toolkit](https://github.com/nexB/scancode-toolkit/) by nexB Inc. to be used as either a standalone CLI or library. In the meantime, I added some functionality which involves further tooling sometimes irrelevant for ScanCode, sometimes not (yet) implemented there.
 
-At the moment, this primarily provides some convenience wrappers around the [ScanCode toolkit](https://github.com/nexB/scancode-toolkit/) by nexB Inc. to be used as either as standalone CLI or library.
+I wrote this tool to simplify the initial scanning steps for third-party packages, mostly tailored to my specific use-cases. For this reason, some implementation or representation details might be opionated and rather tailored to my specific needs. I decided to make this library available as a dedicated package nevertheless, as easy-to-use license compliance (scanner) tooling is sparse, while everyone should care about such topics. If you think that something can be generalized or improved, feel free to open a corresponding issue to discuss this before possibly getting started with an actual PR.
+
+## Features
 
 * Automatically download a specific Python package from PyPI and analyze it.
 * Aggregate how often each license has been used inside the current artifact.
 * Look into shared object files and ELF binaries to see what they are linking to (dynamically).
 * Look into font files to easily analyze their metadata.
 * Look into RPM file metadata.
+* Look into Python package metadata.
 * Recursively look into nested archives, for example by unpacking the actual upstream source code archives inside RPM (source) files.
 * Make everything available from the terminal.
 
 ## Installation
 
 You can install this package from PyPI:
 
@@ -67,70 +72,73 @@
 python -m license_tools --help
 ```
 
 Example: To see the licenses of a specific *pypdf* package version, use something like this:
 
 ```bash
 $ python -m license_tools --package "pypdf==3.4.17"
-              pypdf-3.17.4.dist-info/LICENSE                                    BSD-3-Clause [100.0]
-             pypdf-3.17.4.dist-info/METADATA                                    BSD-3-Clause [99.0]
-               pypdf-3.17.4.dist-info/RECORD                                    
-                pypdf-3.17.4.dist-info/WHEEL                                    
-                           pypdf/__init__.py                                    
-                              pypdf/_cmap.py                                    
-                   pypdf/_codecs/__init__.py                                    
-               pypdf/_codecs/adobe_glyphs.py                                    BSD-3-Clause [100.0]
-                     pypdf/_codecs/pdfdoc.py                                    
-                        pypdf/_codecs/std.py                                    
-                     pypdf/_codecs/symbol.py                                    
-                   pypdf/_codecs/zapfding.py                                    
-          pypdf/_crypt_providers/__init__.py                                    BSD-3-Clause [100.0]
-             pypdf/_crypt_providers/_base.py                                    BSD-3-Clause [100.0]
-     pypdf/_crypt_providers/_cryptography.py                                    BSD-3-Clause [100.0]
-         pypdf/_crypt_providers/_fallback.py                                    BSD-3-Clause [100.0]
-     pypdf/_crypt_providers/_pycryptodome.py                                    BSD-3-Clause [100.0]
-                        pypdf/_encryption.py                                    BSD-3-Clause [100.0]
-                            pypdf/_merger.py                                    BSD-3-Clause [100.0]
-                              pypdf/_page.py                                    BSD-3-Clause [100.0]
-                       pypdf/_page_labels.py                                    
-                         pypdf/_protocols.py                                    
-                            pypdf/_reader.py                                    BSD-3-Clause [100.0]
-          pypdf/_text_extraction/__init__.py                                    
-                             pypdf/_utils.py                                    BSD-3-Clause [100.0]
-                           pypdf/_version.py                                    
-                            pypdf/_writer.py                                    BSD-3-Clause [100.0]
-                pypdf/_xobj_image_helpers.py                                    
-               pypdf/annotations/__init__.py                                    
-                  pypdf/annotations/_base.py                                    
-    pypdf/annotations/_markup_annotations.py                                    
-pypdf/annotations/_non_markup_annotations.py                                    
-                          pypdf/constants.py                                    
-                             pypdf/errors.py                                    
-                            pypdf/filters.py                                    BSD-3-Clause [100.0]
-                   pypdf/generic/__init__.py                                    BSD-3-Clause [100.0]
-                      pypdf/generic/_base.py                                    BSD-3-Clause [100.0]
-           pypdf/generic/_data_structures.py                                    BSD-3-Clause [100.0]
-                       pypdf/generic/_fit.py                                    
-                   pypdf/generic/_outline.py                                    
-                 pypdf/generic/_rectangle.py                                    
-                     pypdf/generic/_utils.py                                    
-                pypdf/generic/_viewerpref.py                                    BSD-3-Clause [100.0]
-                          pypdf/pagerange.py                                    BSD-3-Clause [99.0]
-                         pypdf/papersizes.py                                    
-                              pypdf/py.typed                                    
-                              pypdf/types.py                                    
-                                pypdf/xmp.py                                    
+              pypdf-3.17.4.dist-info/LICENSE                            BSD-3-Clause [100.0]
+             pypdf-3.17.4.dist-info/METADATA                            BSD-3-Clause [99.0]
+               pypdf-3.17.4.dist-info/RECORD                            
+                pypdf-3.17.4.dist-info/WHEEL                            
+                           pypdf/__init__.py                            
+                              pypdf/_cmap.py                            
+                   pypdf/_codecs/__init__.py                            
+               pypdf/_codecs/adobe_glyphs.py                            BSD-3-Clause [100.0]
+                     pypdf/_codecs/pdfdoc.py                            
+                        pypdf/_codecs/std.py                            
+                     pypdf/_codecs/symbol.py                            
+                   pypdf/_codecs/zapfding.py                            
+          pypdf/_crypt_providers/__init__.py                            BSD-3-Clause [100.0]
+             pypdf/_crypt_providers/_base.py                            BSD-3-Clause [100.0]
+     pypdf/_crypt_providers/_cryptography.py                            BSD-3-Clause [100.0]
+         pypdf/_crypt_providers/_fallback.py                            BSD-3-Clause [100.0]
+     pypdf/_crypt_providers/_pycryptodome.py                            BSD-3-Clause [100.0]
+                        pypdf/_encryption.py                            BSD-3-Clause [100.0]
+                            pypdf/_merger.py                            BSD-3-Clause [100.0]
+                              pypdf/_page.py                            BSD-3-Clause [100.0]
+                       pypdf/_page_labels.py                            
+                         pypdf/_protocols.py                            
+                            pypdf/_reader.py                            BSD-3-Clause [100.0]
+          pypdf/_text_extraction/__init__.py                            
+                             pypdf/_utils.py                            BSD-3-Clause [100.0]
+                           pypdf/_version.py                            
+                            pypdf/_writer.py                            BSD-3-Clause [100.0]
+                pypdf/_xobj_image_helpers.py                            
+               pypdf/annotations/__init__.py                            
+                  pypdf/annotations/_base.py                            
+    pypdf/annotations/_markup_annotations.py                            
+pypdf/annotations/_non_markup_annotations.py                            
+                          pypdf/constants.py                            
+                             pypdf/errors.py                            
+                            pypdf/filters.py                            BSD-3-Clause [100.0]
+                   pypdf/generic/__init__.py                            BSD-3-Clause [100.0]
+                      pypdf/generic/_base.py                            BSD-3-Clause [100.0]
+           pypdf/generic/_data_structures.py                            BSD-3-Clause [100.0]
+                       pypdf/generic/_fit.py                            
+                   pypdf/generic/_outline.py                            
+                 pypdf/generic/_rectangle.py                            
+                     pypdf/generic/_utils.py                            
+                pypdf/generic/_viewerpref.py                            BSD-3-Clause [100.0]
+                          pypdf/pagerange.py                            BSD-3-Clause [99.0]
+                         pypdf/papersizes.py                            
+                              pypdf/py.typed                            
+                              pypdf/types.py                            
+                                pypdf/xmp.py                            
 
-====================================================================================================
+=============================================================================================
 
                                                           BSD-3-Clause  20
                                                                   None  28
 ```
 
-If you want to use the package as a library, have a look at the `license_tools.retrieval.run` method for example to see how everything interacts.
+If you want to use the package as a library, have a look at the `license_tools.retrieval.run` method for example to see how everything interacts. In general:
+
+* `license_tools.retrieval` implements most of the CLI/glue code for handling the different source types and starting the actual scanning process as well as displaying the results.
+* `license_tools.tools` implements most of the actual checks and wrappers for the third-party libraries used for scanning/checking.
 
 ## License
 
 This package is subject to the terms of the Apache-2.0 license.
 
 ## Disclaimer
```

### Comparing `license_tools-0.8.0/license_tools.egg-info/SOURCES.txt` & `license_tools-0.9.0/license_tools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 license_tools/tools/linking_tools.py
 license_tools/tools/pip_tools.py
 license_tools/tools/rpm_tools.py
 license_tools/tools/scancode_tools.py
 license_tools/utils/__init__.py
 license_tools/utils/archive_utils.py
 license_tools/utils/path_utils.py
-tests/__init__.py
-tests/data.py
 tests/test_retrieval.py
 tests/files/Carlito-Regular.ttf
 tests/files/Font Awesome 6 Free-Regular-400.otf
 tests/files/LICENSE.md
 tests/files/LICENSE_Carlito-Regular.txt
 tests/files/LICENSE_Font Awesome 6 Free-Regular-400.txt
 tests/files/LICENSE_fa-solid-900.txt
```

### Comparing `license_tools-0.8.0/setup.py` & `license_tools-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 
 ROOT_DIRECTORY = Path(__file__).parent.resolve()
 
 
 setuptools.setup(
     name="license_tools",
     description="Collection of tools for working with Open Source licenses",
-    version="0.8.0",
+    version="0.9.0",
     license="Apache-2.0",
     long_description=Path(ROOT_DIRECTORY / "README.md").read_text(encoding="UTF-8"),
     long_description_content_type="text/markdown",
     author="stefan6419846",
     url="https://github.com/stefan6419846/license_tools",
     packages=setuptools.find_packages(include=["license_tools", "license_tools.*"]),
     include_package_data=True,
     python_requires=">=3.8, <4",
     install_requires=[
-        "scancode-toolkit",
+        "scancode-toolkit>=32.1.0",
         "typecode-libmagic",
         "joblib",
         "fontTools[woff]",
         "pip-licenses-lib",
+        "requests",
     ],
     extras_require={
         "dev": [
             "flake8",
             "flake8-bugbear",
             "pep8-naming",
             "mypy",
-            "requests",
             "types-requests",
             "importlib_resources; python_version<'3.9'",
         ],
         "extended_rpm": [
             "rpmfile",
         ],
     },
```

### Comparing `license_tools-0.8.0/tests/files/Carlito-Regular.ttf` & `license_tools-0.9.0/tests/files/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/files/Font Awesome 6 Free-Regular-400.otf` & `license_tools-0.9.0/tests/files/Font Awesome 6 Free-Regular-400.otf`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/files/LICENSE.md` & `license_tools-0.9.0/tests/files/LICENSE.md`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/files/LICENSE_Carlito-Regular.txt` & `license_tools-0.9.0/tests/files/LICENSE_Carlito-Regular.txt`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/files/LICENSE_Font Awesome 6 Free-Regular-400.txt` & `license_tools-0.9.0/tests/files/LICENSE_Font Awesome 6 Free-Regular-400.txt`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/files/LICENSE_fa-solid-900.txt` & `license_tools-0.9.0/tests/files/LICENSE_fa-solid-900.txt`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/files/LICENSE_weathericons-regular-webfont.txt` & `license_tools-0.9.0/tests/files/LICENSE_weathericons-regular-webfont.txt`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/files/fa-solid-900.woff2` & `license_tools-0.9.0/tests/files/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/files/weathericons-regular-webfont.woff` & `license_tools-0.9.0/tests/files/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/test_retrieval.py` & `license_tools-0.9.0/tests/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/tools/test_font_tools.py` & `license_tools-0.9.0/tests/tools/test_font_tools.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/tools/test_linking_tools.py` & `license_tools-0.9.0/tests/tools/test_linking_tools.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/tools/test_pip_tools.py` & `license_tools-0.9.0/tests/tools/test_pip_tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from unittest import TestCase
 
 from license_tools.tools import pip_tools
 from license_tools.utils import archive_utils
 from tests import get_from_url
-from tests.data import PYPDF__3_17_4__WHEEL
+from tests.data import JWCRYPTO__1_5_4__TAR_GZ, PYPDF__3_17_4__WHEEL
 
 
 class AnalyzeMetadataTestCase(TestCase):
     def test_valid(self) -> None:
         with get_from_url(PYPDF__3_17_4__WHEEL) as path, TemporaryDirectory() as tempdir:
             directory = Path(tempdir)
             archive_utils.extract(
                 archive_path=path, target_directory=directory
             )
 
-            result1 = pip_tools.analyze_metadata(directory / 'pypdf-3.17.4.dist-info')
-            result1.pop('distribution')
+            result1 = pip_tools.analyze_metadata(directory / "pypdf-3.17.4.dist-info")
+            result1.pop("distribution")
             result2 = pip_tools.analyze_metadata(directory)
-            result2.pop('distribution')
+            result2.pop("distribution")
             self.assertEqual(result1, result2)
 
     def test_invalid(self) -> None:
         with TemporaryDirectory() as tempdir:
             directory = Path(tempdir)
-            directory.joinpath('other').mkdir()
+            directory.joinpath("other").mkdir()
             with self.assertRaises(StopIteration):
                 pip_tools.analyze_metadata(directory)
 
 
 class CheckMetadataTestCase(TestCase):
-    def test_check_metadata(self) -> None:
+    def test_check_metadata__dist_info(self) -> None:
         with get_from_url(PYPDF__3_17_4__WHEEL) as path, TemporaryDirectory() as tempdir:
             directory = Path(tempdir)
             archive_utils.extract(
                 archive_path=path, target_directory=directory
             )
             result = pip_tools.check_metadata(directory)
             self.assertEqual(f"""
@@ -72,7 +72,29 @@
           Homepage: https://github.com/py-pdf/pypdf
             Author: Mathieu Fenniak <biziqe@mathieu.fenniak.net>
         Maintainer: Martin Thoma <info@martin-thoma.de>
            License: UNKNOWN
            Summary: A pure-python PDF library capable of splitting, merging, cropping, and transforming PDF files
 License classifier: BSD License
 """[1:-1], result)
+
+    def test_check_metadata__egg_info(self) -> None:
+        with get_from_url(JWCRYPTO__1_5_4__TAR_GZ) as path, TemporaryDirectory() as tempdir:
+            directory = Path(tempdir)
+            archive_utils.extract(
+                archive_path=path, target_directory=directory
+            )
+            result = pip_tools.check_metadata(directory)
+            self.assertEqual(f"""
+              Name: jwcrypto
+           Version: 1.5.4
+      License file: {tempdir}/jwcrypto-1.5.4/LICENSE
+      Requirements:
+                     * cryptography>=3.4
+                     * typing_extensions>=4.5.0
+          Homepage: https://github.com/latchset/jwcrypto
+            Author: UNKNOWN
+        Maintainer: JWCrypto Project Contributors
+           License: LGPLv3+
+           Summary: Implementation of JOSE Web standards
+License classifier:
+"""[1:-1], result)
```

### Comparing `license_tools-0.8.0/tests/tools/test_rpm_tools.py` & `license_tools-0.9.0/tests/tools/test_rpm_tools.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/tools/test_scancode_tools.py` & `license_tools-0.9.0/tests/tools/test_scancode_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,21 +194,23 @@
                     'The\nPOSIX async I/O facility requires this library to provide\nkernel-accelerated async I/O capabilities, as do applications that\n'
                     'require the Linux-native async I/O API.'
                 ),
                 download_url=None, extracted_license_statement='LGPL-2.1+', holder=None,
                 homepage_url='http://kernel.org/pub/linux/libs/aio/', keywords=[],
                 license_detections=[
                     LicenseDetection(
-                        license_expression='lgpl-2.1-plus', identifier='lgpl_2_1_plus-d0bddf88-13b4-4982-bdf5-ce866a0e8394',
+                        license_expression='lgpl-2.1-plus', license_expression_spdx='LGPL-2.1-or-later',
+                        identifier='lgpl_2_1_plus-d0bddf88-13b4-4982-bdf5-ce866a0e8394',
                         matches=[
                             LicenseMatch(
                                 score=100.0, start_line=1, end_line=1, matched_length=3, match_coverage=100.0, matcher='1-hash',
                                 license_expression='lgpl-2.1-plus', rule_identifier='lgpl-2.1-plus_64.RULE', rule_relevance=100,
                                 rule_url='https://github.com/nexB/scancode-toolkit/tree/develop/src/licensedcode/data/rules/lgpl-2.1-plus_64.RULE',
-                                matched_text='LGPL-2.1+'
+                                matched_text='LGPL-2.1+',
+                                spdx_license_expression='LGPL-2.1-or-later', from_file=None,
                             )
                         ]
                     )
                 ],
                 md5=None, name='libaio1', namespace=None, notice_text=None, other_license_detections=[], other_license_expression=None,
                 other_license_expression_spdx=None,
                 parties=[
```

### Comparing `license_tools-0.8.0/tests/utils/test_archive_utils.py` & `license_tools-0.9.0/tests/utils/test_archive_utils.py`

 * *Files identical despite different names*

### Comparing `license_tools-0.8.0/tests/utils/test_path_utils.py` & `license_tools-0.9.0/tests/utils/test_path_utils.py`

 * *Files identical despite different names*

