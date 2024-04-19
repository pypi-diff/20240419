# Comparing `tmp/across_burstcube-0.0.2.tar.gz` & `tmp/across_burstcube-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "across_burstcube-0.0.2.tar", last modified: Wed Apr 17 18:26:14 2024, max compression
+gzip compressed data, was "across_burstcube-0.4.tar", last modified: Fri Apr 19 18:58:37 2024, max compression
```

## Comparing `across_burstcube-0.0.2.tar` & `across_burstcube-0.4.tar`

### file list

```diff
@@ -1,33 +1,41 @@
-drwxr-xr-x   0 jamie      (503) staff       (20)        0 2024-04-17 18:26:14.087973 across_burstcube-0.0.2/
--rw-r--r--   0 jamie      (503) staff       (20)     1741 2024-04-17 18:26:14.087755 across_burstcube-0.0.2/PKG-INFO
--rw-r--r--   0 jamie      (503) staff       (20)      868 2024-04-17 18:24:00.000000 across_burstcube-0.0.2/README.md
-drwxr-xr-x   0 jamie      (503) staff       (20)        0 2024-04-17 18:26:14.087520 across_burstcube-0.0.2/across_burstcube.egg-info/
--rw-r--r--   0 jamie      (503) staff       (20)     1741 2024-04-17 18:26:14.000000 across_burstcube-0.0.2/across_burstcube.egg-info/PKG-INFO
--rw-r--r--   0 jamie      (503) staff       (20)      775 2024-04-17 18:26:14.000000 across_burstcube-0.0.2/across_burstcube.egg-info/SOURCES.txt
--rw-r--r--   0 jamie      (503) staff       (20)        1 2024-04-17 18:26:14.000000 across_burstcube-0.0.2/across_burstcube.egg-info/dependency_links.txt
--rw-r--r--   0 jamie      (503) staff       (20)       79 2024-04-17 18:26:14.000000 across_burstcube-0.0.2/across_burstcube.egg-info/requires.txt
--rw-r--r--   0 jamie      (503) staff       (20)       14 2024-04-17 18:26:14.000000 across_burstcube-0.0.2/across_burstcube.egg-info/top_level.txt
-drwxr-xr-x   0 jamie      (503) staff       (20)        0 2024-04-17 18:26:14.085256 across_burstcube-0.0.2/across_client/
--rw-r--r--   0 jamie      (503) staff       (20)        0 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/__init__.py
-drwxr-xr-x   0 jamie      (503) staff       (20)        0 2024-04-17 18:26:14.085594 across_burstcube-0.0.2/across_client/across/
--rw-r--r--   0 jamie      (503) staff       (20)        0 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/across/__init__.py
--rw-r--r--   0 jamie      (503) staff       (20)     1994 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/across/resolve.py
--rw-r--r--   0 jamie      (503) staff       (20)     1534 2024-04-08 01:04:28.000000 across_burstcube-0.0.2/across_client/across/schema.py
-drwxr-xr-x   0 jamie      (503) staff       (20)        0 2024-04-17 18:26:14.086547 across_burstcube-0.0.2/across_client/base/
--rw-r--r--   0 jamie      (503) staff       (20)        0 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/base/__init__.py
--rw-r--r--   0 jamie      (503) staff       (20)    14492 2024-04-10 16:57:25.000000 across_burstcube-0.0.2/across_client/base/common.py
--rw-r--r--   0 jamie      (503) staff       (20)     1443 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/base/coords.py
--rw-r--r--   0 jamie      (503) staff       (20)      749 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/base/daterange.py
--rw-r--r--   0 jamie      (503) staff       (20)     4929 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/base/schema.py
--rw-r--r--   0 jamie      (503) staff       (20)      383 2024-04-08 01:04:28.000000 across_burstcube-0.0.2/across_client/base/user.py
-drwxr-xr-x   0 jamie      (503) staff       (20)        0 2024-04-17 18:26:14.087232 across_burstcube-0.0.2/across_client/burstcube/
--rw-r--r--   0 jamie      (503) staff       (20)      253 2024-04-17 18:24:00.000000 across_burstcube-0.0.2/across_client/burstcube/__init__.py
--rw-r--r--   0 jamie      (503) staff       (20)       22 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/burstcube/constants.py
--rw-r--r--   0 jamie      (503) staff       (20)        0 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/burstcube/fov.py
--rw-r--r--   0 jamie      (503) staff       (20)     3890 2024-04-14 17:57:19.000000 across_burstcube-0.0.2/across_client/burstcube/schema.py
--rw-r--r--   0 jamie      (503) staff       (20)     6813 2024-04-14 17:58:45.000000 across_burstcube-0.0.2/across_client/burstcube/toorequest.py
--rw-r--r--   0 jamie      (503) staff       (20)      160 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/constants.py
--rw-r--r--   0 jamie      (503) staff       (20)     5328 2024-04-08 01:02:06.000000 across_burstcube-0.0.2/across_client/functions.py
--rw-r--r--   0 jamie      (503) staff       (20)        0 2024-04-08 01:01:30.000000 across_burstcube-0.0.2/across_client/py.typed
--rw-r--r--   0 jamie      (503) staff       (20)     1138 2024-04-17 18:26:02.000000 across_burstcube-0.0.2/pyproject.toml
--rw-r--r--   0 jamie      (503) staff       (20)       38 2024-04-17 18:26:14.088019 across_burstcube-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.469876 across_burstcube-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.461876 across_burstcube-0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.461876 across_burstcube-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-19 18:58:32.000000 across_burstcube-0.4/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 18:58:32.000000 across_burstcube-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 18:58:32.000000 across_burstcube-0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 18:58:37.469876 across_burstcube-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-19 18:58:32.000000 across_burstcube-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_burstcube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 18:58:37.000000 across_burstcube-0.4/across_burstcube.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/across/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/across/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/daterange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/base/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:37.465876 across_burstcube-0.4/across_client/burstcube/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/fov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/burstcube/toorequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:58:32.000000 across_burstcube-0.4/across_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-19 18:58:32.000000 across_burstcube-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:58:37.469876 across_burstcube-0.4/setup.cfg
```

### Comparing `across_burstcube-0.0.2/PKG-INFO` & `across_burstcube-0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 Metadata-Version: 2.1
 Name: across-burstcube
-Version: 0.0.2
-Summary: ACROSS API Python client for BurstCube
+Version: 0.4
+Summary: ACROSS API Python client
 Author-email: "Jamie A. Kennea" <jak51@psu.edu>
 Maintainer-email: "Jamie A. Kennea" <jak51@psu.edu>
+Project-URL: Homepage, https://github.com/jak574/across-api-client
+Project-URL: Bug Reports, https://github.com/jak574/across-api-client/issues
+Project-URL: Source, https://github.com/jak574/across-api-client/
 Keywords: astronomy,api,across
 Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pydantic
 Requires-Dist: astropy
 Requires-Dist: python-dateutil
+Requires-Dist: authlib
 Requires-Dist: types-python-dateutil
 Requires-Dist: types-requests
+Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
 
-# ACROSS API Python BurstCubeTOO Client
+# ACROSS API Python Client
 
-This is the Python API for the Astrophysics Cross-Observatory Science Support
-(ACROSS), a NASA initiative to provide cross-observatory support for
-time-domain and multi-messenger (TDAMM) coordination and observation planning.
+This is the Python API for the Astrophysics Cross-Observatory Science Support (ACROSS), a NASA initiative to provide cross-observatory support for time-domain and multi-messenger (TDAMM) coordination and observation planning.
 
-The client provides support for accessing the BurstCube TOO interface that
-ACROSS provides.
+To install the `across_client` Python module, please do the following:
 
-To install the client, enter the command `pip install across-burstcube-client`.
+1. Clone the repository to your computer.
+2. Enter the directory and install the module using `pip install .`
 
-The `across_client` module should now be available for use. The relevant
-classes are:
-
-`BurstCubeTOO`
-
-Main interface for submitting, updating, fetching and deleting BurstCube TOO
-requests.
-
-`BurstCubeTriggerInfo`
-
-Class that provides extended information on the triggering event, this is an
-parameter for `BurstCubeTOO`.
-
-`BurstCubeTOORequests`
-
-Allows to fetch multiple `BurstCubeTOO` entries using various filter criteria.
+The `across_client` module should now be available for use.
```

### Comparing `across_burstcube-0.0.2/across_burstcube.egg-info/PKG-INFO` & `across_burstcube-0.4/across_burstcube.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 Metadata-Version: 2.1
 Name: across-burstcube
-Version: 0.0.2
-Summary: ACROSS API Python client for BurstCube
+Version: 0.4
+Summary: ACROSS API Python client
 Author-email: "Jamie A. Kennea" <jak51@psu.edu>
 Maintainer-email: "Jamie A. Kennea" <jak51@psu.edu>
+Project-URL: Homepage, https://github.com/jak574/across-api-client
+Project-URL: Bug Reports, https://github.com/jak574/across-api-client/issues
+Project-URL: Source, https://github.com/jak574/across-api-client/
 Keywords: astronomy,api,across
 Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pydantic
 Requires-Dist: astropy
 Requires-Dist: python-dateutil
+Requires-Dist: authlib
 Requires-Dist: types-python-dateutil
 Requires-Dist: types-requests
+Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+Provides-Extra: test
+Requires-Dist: coverage; extra == "test"
 
-# ACROSS API Python BurstCubeTOO Client
+# ACROSS API Python Client
 
-This is the Python API for the Astrophysics Cross-Observatory Science Support
-(ACROSS), a NASA initiative to provide cross-observatory support for
-time-domain and multi-messenger (TDAMM) coordination and observation planning.
+This is the Python API for the Astrophysics Cross-Observatory Science Support (ACROSS), a NASA initiative to provide cross-observatory support for time-domain and multi-messenger (TDAMM) coordination and observation planning.
 
-The client provides support for accessing the BurstCube TOO interface that
-ACROSS provides.
+To install the `across_client` Python module, please do the following:
 
-To install the client, enter the command `pip install across-burstcube-client`.
+1. Clone the repository to your computer.
+2. Enter the directory and install the module using `pip install .`
 
-The `across_client` module should now be available for use. The relevant
-classes are:
-
-`BurstCubeTOO`
-
-Main interface for submitting, updating, fetching and deleting BurstCube TOO
-requests.
-
-`BurstCubeTriggerInfo`
-
-Class that provides extended information on the triggering event, this is an
-parameter for `BurstCubeTOO`.
-
-`BurstCubeTOORequests`
-
-Allows to fetch multiple `BurstCubeTOO` entries using various filter criteria.
+The `across_client` module should now be available for use.
```

### Comparing `across_burstcube-0.0.2/across_burstcube.egg-info/SOURCES.txt` & `across_burstcube-0.4/across_burstcube.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+.gitignore
+.pre-commit-config.yaml
 README.md
 pyproject.toml
+.github/ISSUE_TEMPLATE.md
+.github/PULL_REQUEST_TEMPLATE.md
+.github/workflows/deploy.yml
+.github/workflows/pylint.yml
 across_burstcube.egg-info/PKG-INFO
 across_burstcube.egg-info/SOURCES.txt
 across_burstcube.egg-info/dependency_links.txt
 across_burstcube.egg-info/requires.txt
 across_burstcube.egg-info/top_level.txt
 across_client/__init__.py
 across_client/constants.py
```

### Comparing `across_burstcube-0.0.2/across_client/across/resolve.py` & `across_burstcube-0.4/across_client/across/resolve.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.2/across_client/across/schema.py` & `across_burstcube-0.4/across_client/across/schema.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.2/across_client/base/common.py` & `across_burstcube-0.4/across_client/base/common.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.2/across_client/base/coords.py` & `across_burstcube-0.4/across_client/base/coords.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.2/across_client/base/daterange.py` & `across_burstcube-0.4/across_client/base/daterange.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.2/across_client/base/schema.py` & `across_burstcube-0.4/across_client/base/schema.py`

 * *Files identical despite different names*

### Comparing `across_burstcube-0.0.2/across_client/burstcube/schema.py` & `across_burstcube-0.4/across_client/burstcube/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,14 @@
     trigger_time: datetime
     trigger_info: BurstCubeTriggerInfo
     exposure: int
     offset: int
     reject_reason: TOOReason = TOOReason.none
     status: TOOStatus = TOOStatus.requested
     too_info: str = ""
-    healpix_filename: Optional[str] = None
-    version: int
 
 
 class BurstCubeTOODelSchema(BaseSchema):
     """
     Schema for BurstCubeTOO DELETE API call.
 
     Attributes
```

### Comparing `across_burstcube-0.0.2/across_client/burstcube/toorequest.py` & `across_burstcube-0.4/across_client/burstcube/toorequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,14 @@
     ra: Optional[float] = None
     dec: Optional[float] = None
     error_radius: Optional[float] = None
     healpix_filename: Optional[FilePath] = None
     healpix_file: Union[io.BytesIO, io.BufferedReader, None] = None
     reject_reason: TOOReason = TOOReason.none
     status: TOOStatus = TOOStatus.requested
-    version: Optional[int] = None
 
     # API definitions
     _mission = MISSION
     _api_name = "TOO"
     _schema = BurstCubeTOOSchema
     _put_schema = BurstCubeTOOPutSchema
     _post_schema = BurstCubeTOOPostSchema
```

### Comparing `across_burstcube-0.0.2/across_client/functions.py` & `across_burstcube-0.4/across_client/functions.py`

 * *Files identical despite different names*

