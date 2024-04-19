# Comparing `tmp/gender-local-0.0.6.tar.gz` & `tmp/gender_local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender-local-0.0.6.tar", last modified: Thu Oct  5 22:17:10 2023, max compression
+gzip compressed data, was "gender_local-0.0.7.tar", last modified: Fri Apr 19 03:18:39 2024, max compression
```

## Comparing `gender-local-0.0.6.tar` & `gender_local-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 22:17:10.493174 gender-local-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-10-05 22:17:10.493174 gender-local-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-05 22:16:39.000000 gender-local-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 22:17:10.489174 gender-local-0.0.6/gender_local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 22:16:39.000000 gender-local-0.0.6/gender_local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 22:17:10.493174 gender-local-0.0.6/gender_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-05 22:16:39.000000 gender-local-0.0.6/gender_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-10-05 22:16:39.000000 gender-local-0.0.6/gender_local/src/constants_gender_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-05 22:16:39.000000 gender-local-0.0.6/gender_local/src/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-05 22:16:39.000000 gender-local-0.0.6/gender_local/src/gender_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 22:17:10.489174 gender-local-0.0.6/gender_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-10-05 22:17:10.000000 gender-local-0.0.6/gender_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-10-05 22:17:10.000000 gender-local-0.0.6/gender_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 22:17:10.000000 gender-local-0.0.6/gender_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-05 22:17:10.000000 gender-local-0.0.6/gender_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-10-05 22:16:39.000000 gender-local-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 22:17:10.493174 gender-local-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-10-05 22:16:39.000000 gender-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:18:39.275221 gender_local-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 03:18:39.275221 gender_local-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-19 03:18:11.000000 gender_local-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:18:39.271221 gender_local-0.0.7/gender_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:18:39.271221 gender_local-0.0.7/gender_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:18:11.000000 gender_local-0.0.7/gender_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-19 03:18:11.000000 gender_local-0.0.7/gender_local/src/constants_gender_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-19 03:18:11.000000 gender_local-0.0.7/gender_local/src/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-19 03:18:11.000000 gender_local-0.0.7/gender_local/src/gender_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:18:39.271221 gender_local-0.0.7/gender_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-19 03:18:39.000000 gender_local-0.0.7/gender_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 03:18:39.000000 gender_local-0.0.7/gender_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:18:39.000000 gender_local-0.0.7/gender_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 03:18:39.000000 gender_local-0.0.7/gender_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 03:18:39.000000 gender_local-0.0.7/gender_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-19 03:18:11.000000 gender_local-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:18:39.275221 gender_local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-19 03:18:11.000000 gender_local-0.0.7/setup.py
```

### Comparing `gender-local-0.0.6/README.md` & `gender_local-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 # python-package-template
+
 To create local package and remote package layers (not to create GraphQL and REST-API layers)
 
 # directory structure
-Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e. location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br> 
+
+Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e.
+location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br>
 /location_local<br>
 /location_local/get_country_name<br>
 /location_local/get_country_name/src<br>
 /location_local/get_country_name/src/get_country_name.py<br>
 /location_local/get_country_name/tests<br>
 /location_local/get_country_name/tests/test_get_country_name.py<br>
 
 # database Python scripts in /db folder
+
 Please place <table-name>.py in /db<br>
 No need for seperate file for _ml table<br>
 Please delete the example file if not needed<br>
-  
+
 # Create the files to create the database schema, tables, view and populate Meta Data and Test Date
+
 /db/<table-name>.py - CREATE SCHEMA ... CREATE TABLE ... CREATE VIEW ...<br>
 /db/<table-name>_insert.py to create records
 
 # Update the setup.py (i.e.name, version)
- 
+
 # Please create test directory inside the directory of the project i.e. /<project-name>/tests
 
 # Update the serverless.yml in the root directory
+
 provider:
-  stage: play1
-  
+stage: play1
+
 Update the endpoints in serverless.yml
 
 # Working with VS Code
+
 Please make sure you push to the repo launch.json fie that enables to run and debug the code<br>
 
 # Unit-Test
+
 We prefer using pytest and not unittest package<br>
 
 Please create pytest.init in the project directory and not in the root directory
+
 ```
 [pytest]
 markers =
     test: custom mark for tests
 ```
```

### Comparing `gender-local-0.0.6/gender_local/src/constants_gender_local.py` & `gender_local-0.0.7/gender_local/src/constants_gender_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
+
 class ConstantsGenderLocal:
     GENDER_LOCAL_PYTHON_PACKAGE_COMPONENT_ID = 201
     GENDER_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME = 'gender-local-python-package'
 
     OBJECT_FOR_LOGGER_CODE = {
         'component_id': GENDER_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
         'component_name': GENDER_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME,
```

### Comparing `gender-local-0.0.6/pyproject.toml` & `gender_local-0.0.7/pyproject.toml`

 * *Files identical despite different names*
