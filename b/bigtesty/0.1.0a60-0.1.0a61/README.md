# Comparing `tmp/bigtesty-0.1.0a60.tar.gz` & `tmp/bigtesty-0.1.0a61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigtesty-0.1.0a60.tar", last modified: Fri Apr 19 17:32:27 2024, max compression
+gzip compressed data, was "bigtesty-0.1.0a61.tar", last modified: Fri Apr 19 18:18:20 2024, max compression
```

## Comparing `bigtesty-0.1.0a60.tar` & `bigtesty-0.1.0a61.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:27.841491 bigtesty-0.1.0a60/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 17:32:27.841491 bigtesty-0.1.0a60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:27.837491 bigtesty-0.1.0a60/bigtesty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:27.841491 bigtesty-0.1.0a60/bigtesty/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/dataset_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/definition_test_config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/definition_test_file_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/files_loader_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:27.841491 bigtesty-0.1.0a60/bigtesty/given/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/given/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/given/insertion_test_data_bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:27.841491 bigtesty-0.1.0a60/bigtesty/infra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/infra/create_iac_for_datasets_with_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/infra/datasets_with_tables_config_file_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/infra/datasets_with_tables_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/infra/launch_tests_ephemeral_infra.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/lambda_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:27.841491 bigtesty-0.1.0a60/bigtesty/then/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/then/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/then/assertion_and_tests_reports_result.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/bigtesty/then/failure_test_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:32:27.841491 bigtesty-0.1.0a60/bigtesty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 17:32:27.000000 bigtesty-0.1.0a60/bigtesty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-19 17:32:27.000000 bigtesty-0.1.0a60/bigtesty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:32:27.000000 bigtesty-0.1.0a60/bigtesty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 17:32:27.000000 bigtesty-0.1.0a60/bigtesty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 17:32:27.000000 bigtesty-0.1.0a60/bigtesty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 17:32:27.000000 bigtesty-0.1.0a60/bigtesty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:32:27.841491 bigtesty-0.1.0a60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-19 17:32:13.000000 bigtesty-0.1.0a60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:20.466490 bigtesty-0.1.0a61/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 18:18:20.466490 bigtesty-0.1.0a61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:20.462490 bigtesty-0.1.0a61/bigtesty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:20.462490 bigtesty-0.1.0a61/bigtesty/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/dataset_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/definition_test_config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/definition_test_file_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/files_loader_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:20.462490 bigtesty-0.1.0a61/bigtesty/given/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/given/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/given/insertion_test_data_bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:20.466490 bigtesty-0.1.0a61/bigtesty/infra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/infra/create_iac_for_datasets_with_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/infra/datasets_with_tables_config_file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/infra/datasets_with_tables_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/infra/launch_tests_ephemeral_infra.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/lambda_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:20.466490 bigtesty-0.1.0a61/bigtesty/then/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/then/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/then/assertion_and_tests_reports_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/bigtesty/then/failure_test_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 18:18:20.462490 bigtesty-0.1.0a61/bigtesty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 18:18:20.000000 bigtesty-0.1.0a61/bigtesty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-19 18:18:20.000000 bigtesty-0.1.0a61/bigtesty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 18:18:20.000000 bigtesty-0.1.0a61/bigtesty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 18:18:20.000000 bigtesty-0.1.0a61/bigtesty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 18:18:20.000000 bigtesty-0.1.0a61/bigtesty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 18:18:20.000000 bigtesty-0.1.0a61/bigtesty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 18:18:20.466490 bigtesty-0.1.0a61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-19 18:18:05.000000 bigtesty-0.1.0a61/setup.py
```

### Comparing `bigtesty-0.1.0a60/LICENSE` & `bigtesty-0.1.0a61/LICENSE`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a60/PKG-INFO` & `bigtesty-0.1.0a61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtesty
-Version: 0.1.0a60
+Version: 0.1.0a61
 Summary: BigTesty is an integration testing framework for BigQuery
 Home-page: https://github.com/tosun-si/bigtesty
 Author: Mazlum TOSUN
 Author-email: mazlum.tosun@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigtesty-0.1.0a60/README.md` & `bigtesty-0.1.0a61/README.md`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a60/bigtesty/cli/main.py` & `bigtesty-0.1.0a61/bigtesty/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 app = typer.Typer()
 
 
 @app.command("test")
 def run_tests(root_test_folder: Annotated[str, typer.Option("--root-test-folder")],
               root_tables_folder: Annotated[str, typer.Option("--root-tables-folder")],
               tables_config_file_path: Annotated[str, typer.Option("--tables-config-file")],
-              destroy_ephemeral_infra: Annotated[bool, typer.Option("--tables-config-file")] = True):
+              destroy_infra: Annotated[bool, typer.Option("--destroy-infra")] = True):
     print(f"####################### The CLI is invoked with params : ")
 
-    print(f"root_test_folder : {root_test_folder}")
-    print(f"root_tables_folder : {root_tables_folder}")
-    print(f"tables_config_file_path : {tables_config_file_path}")
-    print(f"destroy_ephemeral_infra : {destroy_ephemeral_infra}")
+    print(f"root-test-folder : {root_test_folder}")
+    print(f"root-tables-folder : {root_tables_folder}")
+    print(f"tables-config-file : {tables_config_file_path}")
+    print(f"destroy-infra : {destroy_infra}")
 
     launch_tests_ephemeral_infra(
         root_test_folder=root_test_folder,
         root_tables_folder=root_tables_folder,
         tables_config_file_path=tables_config_file_path,
-        destroy_ephemeral_infra=destroy_ephemeral_infra
+        destroy_ephemeral_infra=destroy_infra
     )
 
 
 @app.command("info")
 def display_bigtesty_info():
     print("BigTesty is an integration testing framework for BigQuery")
```

### Comparing `bigtesty-0.1.0a60/bigtesty/definition_test_config_helper.py` & `bigtesty-0.1.0a61/bigtesty/definition_test_config_helper.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a60/bigtesty/given/insertion_test_data_bigquery.py` & `bigtesty-0.1.0a61/bigtesty/given/insertion_test_data_bigquery.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a60/bigtesty/infra/create_iac_for_datasets_with_tables.py` & `bigtesty-0.1.0a61/bigtesty/infra/create_iac_for_datasets_with_tables.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a60/bigtesty/infra/datasets_with_tables_config_file_loader.py` & `bigtesty-0.1.0a61/bigtesty/infra/datasets_with_tables_config_file_loader.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a60/bigtesty/infra/datasets_with_tables_factory.py` & `bigtesty-0.1.0a61/bigtesty/infra/datasets_with_tables_factory.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a60/bigtesty/infra/launch_tests_ephemeral_infra.py` & `bigtesty-0.1.0a61/bigtesty/infra/launch_tests_ephemeral_infra.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a60/bigtesty/then/assertion_and_tests_reports_result.py` & `bigtesty-0.1.0a61/bigtesty/then/assertion_and_tests_reports_result.py`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a60/bigtesty.egg-info/PKG-INFO` & `bigtesty-0.1.0a61/bigtesty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigtesty
-Version: 0.1.0a60
+Version: 0.1.0a61
 Summary: BigTesty is an integration testing framework for BigQuery
 Home-page: https://github.com/tosun-si/bigtesty
 Author: Mazlum TOSUN
 Author-email: mazlum.tosun@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bigtesty-0.1.0a60/bigtesty.egg-info/SOURCES.txt` & `bigtesty-0.1.0a61/bigtesty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bigtesty-0.1.0a60/setup.py` & `bigtesty-0.1.0a61/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The text of the README file
 long_desc = ""
 if os.path.isfile(path):
     long_desc = path.read_text()
 
 setup(
     name="bigtesty",
-    version="0.1.0a60",
+    version="0.1.0a61",
     entry_points='''
         [console_scripts]
         bigtesty=bigtesty.cli.main:run
     ''',
     install_requires=[
         "pulumi-gcp==6.67.0",
         "google-cloud-bigquery==3.7.0",
```
