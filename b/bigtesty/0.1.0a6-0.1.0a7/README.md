# Comparing `tmp/bigtesty-0.1.0a6.tar.gz` & `tmp/bigtesty-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigtesty-0.1.0a6.tar", last modified: Fri Apr 19 18:49:55 2024, max compression
+gzip compressed data, was "bigtesty-0.1.0a7.tar", last modified: Fri Apr 19 18:56:34 2024, max compression
```

## Comparing `bigtesty-0.1.0a6.tar` & `bigtesty-0.1.0a7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:55.023568 bigtesty-0.1.0a6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-19 18:49:55.023568 bigtesty-0.1.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:55.019568 bigtesty-0.1.0a6/bigtesty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:55.019568 bigtesty-0.1.0a6/bigtesty/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/dataset_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/definition_test_config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/definition_test_file_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/files_loader_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:55.019568 bigtesty-0.1.0a6/bigtesty/given/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/given/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/given/insertion_test_data_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:55.019568 bigtesty-0.1.0a6/bigtesty/infra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/infra/create_iac_for_datasets_with_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/infra/datasets_with_tables_config_file_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/infra/datasets_with_tables_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/infra/launch_tests_ephemeral_infra.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/lambda_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:55.023568 bigtesty-0.1.0a6/bigtesty/then/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/then/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/then/assertion_and_tests_reports_result.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 18:49:40.000000 bigtesty-0.1.0a6/bigtesty/then/failure_test_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:49:55.019568 bigtesty-0.1.0a6/bigtesty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-19 18:49:54.000000 bigtesty-0.1.0a6/bigtesty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-19 18:49:54.000000 bigtesty-0.1.0a6/bigtesty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:49:54.000000 bigtesty-0.1.0a6/bigtesty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 18:49:54.000000 bigtesty-0.1.0a6/bigtesty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 18:49:54.000000 bigtesty-0.1.0a6/bigtesty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 18:49:54.000000 bigtesty-0.1.0a6/bigtesty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:49:55.023568 bigtesty-0.1.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-19 18:49:41.000000 bigtesty-0.1.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:34.676365 bigtesty-0.1.0a7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-19 18:56:34.676365 bigtesty-0.1.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:34.676365 bigtesty-0.1.0a7/bigtesty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:34.676365 bigtesty-0.1.0a7/bigtesty/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/dataset_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/definition_test_config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/definition_test_file_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/files_loader_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:34.676365 bigtesty-0.1.0a7/bigtesty/given/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/given/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/given/insertion_test_data_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:34.676365 bigtesty-0.1.0a7/bigtesty/infra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/infra/create_iac_for_datasets_with_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/infra/datasets_with_tables_config_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/infra/datasets_with_tables_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/infra/launch_tests_ephemeral_infra.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/lambda_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:34.676365 bigtesty-0.1.0a7/bigtesty/then/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/then/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/then/assertion_and_tests_reports_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/bigtesty/then/failure_test_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:56:34.676365 bigtesty-0.1.0a7/bigtesty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-19 18:56:34.000000 bigtesty-0.1.0a7/bigtesty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-19 18:56:34.000000 bigtesty-0.1.0a7/bigtesty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:56:34.000000 bigtesty-0.1.0a7/bigtesty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 18:56:34.000000 bigtesty-0.1.0a7/bigtesty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 18:56:34.000000 bigtesty-0.1.0a7/bigtesty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 18:56:34.000000 bigtesty-0.1.0a7/bigtesty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:56:34.676365 bigtesty-0.1.0a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-19 18:56:20.000000 bigtesty-0.1.0a7/setup.py
```

### Comparing `bigtesty-0.1.0a6/LICENSE` & `bigtesty-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a6/PKG-INFO` & `bigtesty-0.1.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtesty
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: BigTesty is an integration testing framework for BigQuery
 Home-page: https://github.com/tosun-si/bigtesty
 Author: Mazlum TOSUN
 Author-email: mazlum.tosun@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigtesty-0.1.0a6/README.md` & `bigtesty-0.1.0a7/README.md`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a6/bigtesty/cli/main.py` & `bigtesty-0.1.0a7/bigtesty/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     print(f"tables-config-file : {tables_config_file_path}")
     print(f"destroy-infra : {destroy_infra}")
 
     launch_tests_ephemeral_infra(
         root_test_folder=root_test_folder,
         root_tables_folder=root_tables_folder,
         tables_config_file_path=tables_config_file_path,
-        destroy_ephemeral_infra=destroy_infra
+        destroy_infra=destroy_infra
     )
 
 
 @app.command("info")
 def display_bigtesty_info():
     print("BigTesty is an integration testing framework for BigQuery")
```

### Comparing `bigtesty-0.1.0a6/bigtesty/definition_test_config_helper.py` & `bigtesty-0.1.0a7/bigtesty/definition_test_config_helper.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a6/bigtesty/given/insertion_test_data_bigquery.py` & `bigtesty-0.1.0a7/bigtesty/given/insertion_test_data_bigquery.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a6/bigtesty/infra/create_iac_for_datasets_with_tables.py` & `bigtesty-0.1.0a7/bigtesty/infra/create_iac_for_datasets_with_tables.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a6/bigtesty/infra/datasets_with_tables_config_file_loader.py` & `bigtesty-0.1.0a7/bigtesty/infra/datasets_with_tables_config_file_loader.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a6/bigtesty/infra/datasets_with_tables_factory.py` & `bigtesty-0.1.0a7/bigtesty/infra/datasets_with_tables_factory.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a6/bigtesty/infra/launch_tests_ephemeral_infra.py` & `bigtesty-0.1.0a7/bigtesty/infra/launch_tests_ephemeral_infra.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from bigtesty.then.assertion_and_tests_reports_result import execute_query_and_build_reports_result, \
     check_any_failed_test_in_reports
 
 
 def launch_tests_ephemeral_infra(root_test_folder: str,
                                  root_tables_folder: str,
                                  tables_config_file_path: str,
-                                 destroy_ephemeral_infra: bool):
+                                 destroy_infra: bool):
     project_id = os.environ["GOOGLE_PROJECT"]
     region = os.environ["GOOGLE_REGION"]
     stack_name = os.environ["BIGTESTY_STACK_NAME"]
 
     datasets_hash = get_datasets_hash(5)
 
     scenarios = get_scenarios(root_test_folder)
@@ -95,17 +95,17 @@
             show_secrets=False,
             log_flow=True,
             log_verbosity=3
         )
 
         sys.exit(-1)
 
-    print(f"################### Parameter to destroy the ephemeral infra (true/false) : {destroy_ephemeral_infra}")
+    print(f"################### Parameter to destroy the infra (true/false) : {destroy_infra}")
 
-    if destroy_ephemeral_infra:
+    if destroy_infra:
         print("################### Destroying the ephemeral infra and tests assertions...")
         stack.destroy(
             on_output=print,
             color="always",
             show_secrets=False,
             log_flow=True,
             log_verbosity=3
```

### Comparing `bigtesty-0.1.0a6/bigtesty/then/assertion_and_tests_reports_result.py` & `bigtesty-0.1.0a7/bigtesty/then/assertion_and_tests_reports_result.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a6/bigtesty.egg-info/PKG-INFO` & `bigtesty-0.1.0a7/bigtesty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtesty
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: BigTesty is an integration testing framework for BigQuery
 Home-page: https://github.com/tosun-si/bigtesty
 Author: Mazlum TOSUN
 Author-email: mazlum.tosun@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigtesty-0.1.0a6/bigtesty.egg-info/SOURCES.txt` & `bigtesty-0.1.0a7/bigtesty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a6/setup.py` & `bigtesty-0.1.0a7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The text of the README file
 long_desc = ""
 if os.path.isfile(path):
     long_desc = path.read_text()
 
 setup(
     name="bigtesty",
-    version="0.1.0a6",
+    version="0.1.0a7",
     entry_points='''
         [console_scripts]
         bigtesty=bigtesty.cli.main:run
     ''',
     install_requires=[
         "pulumi-gcp==6.67.0",
         "google-cloud-bigquery==3.7.0",
```

