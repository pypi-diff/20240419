# Comparing `tmp/tinybird-cdk-0.17.5.tar.gz` & `tmp/tinybird_cdk-0.17.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cdk-0.17.5.tar", last modified: Tue Apr  9 10:52:23 2024, max compression
+gzip compressed data, was "tinybird_cdk-0.17.7.tar", last modified: Fri Apr 19 14:00:09 2024, max compression
```

## Comparing `tinybird-cdk-0.17.5.tar` & `tinybird_cdk-0.17.7.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.335281 tinybird-cdk-0.17.5/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 10:52:23.335281 tinybird-cdk-0.17.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25352 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:52:23.335281 tinybird-cdk-0.17.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.327281 tinybird-cdk-0.17.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tests/test_gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.331281 tinybird-cdk-0.17.5/tinybird_cdk/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.331281 tinybird-cdk-0.17.5/tinybird_cdk/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/cloud/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/cloud/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/cloud/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/cloud/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.335281 tinybird-cdk-0.17.5/tinybird_cdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/connectors/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12911 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/tinybird.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 10:52:17.000000 tinybird-cdk-0.17.5/tinybird_cdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:52:23.335281 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 10:52:23.000000 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 10:52:23.000000 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:52:23.000000 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 10:52:23.000000 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 10:52:23.000000 tinybird-cdk-0.17.5/tinybird_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.291656 tinybird_cdk-0.17.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-19 14:00:09.291656 tinybird_cdk-0.17.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26052 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:00:09.291656 tinybird_cdk-0.17.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.283656 tinybird_cdk-0.17.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tests/test_gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.287656 tinybird_cdk-0.17.7/tinybird_cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.287656 tinybird_cdk-0.17.7/tinybird_cdk/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/cloud/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/cloud/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/cloud/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/cloud/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.291656 tinybird_cdk-0.17.7/tinybird_cdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12911 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/tinybird.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.291656 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-19 14:00:09.000000 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-19 14:00:09.000000 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:00:09.000000 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 14:00:09.000000 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 14:00:09.000000 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/top_level.txt
```

### Comparing `tinybird-cdk-0.17.5/README.md` & `tinybird_cdk-0.17.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 - [CDK Development](#cdk-development)
   - [TL;DR](#tldr)
   - [Python](#python)
   - [Virtual Environment](#virtual-environment)
   - [Project Dependencies](#project-dependencies)
   - [Docker Compose](#docker-compose)
   - [Tests](#tests)
+  - [Release](#release)
 - [Connector Development](#connector-development)
   - [Execution Environment](#execution-environment)
   - [Conventions](#conventions)
   - [Connectors Factory](#connectors-factory)
   - [Configuration](#configuration)
     - [Tinybird](#tinybird)
     - [Pass-Through Driver Environment Variables](#pass-through-driver-environment-variables)
@@ -66,15 +67,15 @@
 
 Everything is detailed later, but this is the gist of it:
 
 1. Install Python >= 3.8
 1. Install Docker Compose
 1. Setup and activate a virtual environment
 1. Set the environment variable `TB_CDK_TEST_SUITE_TOKEN` (ask for its value)
-1. Run `bin/reqs`
+1. Run `pip install -e .["dev"]`
 1. Run `bin/test`
 
 You should see the test suite passing.
 
 <a id="markdown-python" name="python"></a>
 ### Python
 
@@ -99,15 +100,15 @@
 
 <a id="markdown-project-dependencies" name="project-dependencies"></a>
 ### Project Dependencies
 
 In order to install project dependencies execute
 
 ```
-% bin/reqs
+% pip install -r requirements.txt -r requirements-dev.txt
 ```
 
 in the project root directory.
 
 <a id="markdown-docker-compose" name="docker-compose"></a>
 ### Docker Compose
 
@@ -166,14 +167,31 @@
 
 You can also pass multiple options as in
 
 ```
 % bin/test -s -k TestCloudS3
 ```
 
+<a id="markdown-release" name="release"></a>
+### Release
+
+To release a new version, you'll need to bump the version number by running
+
+```
+% bumpversion patch # or minor, or major
+```
+
+This will update the version number in `pyproject.toml`, `tinybird_cdk/__init__.py` and `.bumpversion.cfg`, and create a new commit.  
+Then, push the changes to the repository.
+
+When the PR is merged to `main`, the CI will run release steps:
+* A new tag will be created by the CI.
+* The CI will build the package and upload it to PyPI.
+* A docker image will be built and pushed to the registry with two tags: `X.Y.Z` and `X.Y`.
+
 <a id="markdown-connector-development" name="connector-development"></a>
 ## Connector Development
 
 <a id="markdown-execution-environment" name="execution-environment"></a>
 ### Execution Environment
 
 Connectors should be able to run in client infraestructure and therefore can
```

### Comparing `tinybird-cdk-0.17.5/tests/test_gcp.py` & `tinybird_cdk-0.17.7/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/cloud/__init__.py` & `tinybird_cdk-0.17.7/tinybird_cdk/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/cloud/abstract_client.py` & `tinybird_cdk-0.17.7/tinybird_cdk/cloud/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/cloud/gcp.py` & `tinybird_cdk-0.17.7/tinybird_cdk/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/cloud/gcs.py` & `tinybird_cdk-0.17.7/tinybird_cdk/cloud/gcs.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/cloud/s3.py` & `tinybird_cdk-0.17.7/tinybird_cdk/cloud/s3.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/config.py` & `tinybird_cdk-0.17.7/tinybird_cdk/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/connector.py` & `tinybird_cdk-0.17.7/tinybird_cdk/connector.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/connectors/bigquery.py` & `tinybird_cdk-0.17.7/tinybird_cdk/connectors/bigquery.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/connectors/kinesis.py` & `tinybird_cdk-0.17.7/tinybird_cdk/connectors/kinesis.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/connectors/mysql.py` & `tinybird_cdk-0.17.7/tinybird_cdk/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/connectors/postgresql.py` & `tinybird_cdk-0.17.7/tinybird_cdk/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/connectors/snowflake.py` & `tinybird_cdk-0.17.7/tinybird_cdk/connectors/snowflake.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/connectors/sqlite.py` & `tinybird_cdk-0.17.7/tinybird_cdk/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/errors.py` & `tinybird_cdk-0.17.7/tinybird_cdk/errors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/export.py` & `tinybird_cdk-0.17.7/tinybird_cdk/export.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/formats.py` & `tinybird_cdk-0.17.7/tinybird_cdk/formats.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/logger.py` & `tinybird_cdk-0.17.7/tinybird_cdk/logger.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/migration.py` & `tinybird_cdk-0.17.7/tinybird_cdk/migration.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/schema.py` & `tinybird_cdk-0.17.7/tinybird_cdk/schema.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk/tinybird.py` & `tinybird_cdk-0.17.7/tinybird_cdk/tinybird.py`

 * *Files identical despite different names*

### Comparing `tinybird-cdk-0.17.5/tinybird_cdk.egg-info/SOURCES.txt` & `tinybird_cdk-0.17.7/tinybird_cdk.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+DESCRIPTION.md
 README.md
-setup.py
+pyproject.toml
+requirements-dev.txt
+requirements.txt
 tests/test_gcp.py
 tinybird_cdk/__init__.py
 tinybird_cdk/config.py
 tinybird_cdk/connector.py
 tinybird_cdk/errors.py
 tinybird_cdk/export.py
 tinybird_cdk/formats.py
```

