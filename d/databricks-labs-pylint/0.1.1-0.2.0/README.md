# Comparing `tmp/databricks_labs_pylint-0.1.1.tar.gz` & `tmp/databricks_labs_pylint-0.2.0.tar.gz`

## Comparing `databricks_labs_pylint-0.1.1.tar` & `databricks_labs_pylint-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/__init__.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/airflow.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/all.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/cli.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/dbutils.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/legacy.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/mocking.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/notebooks.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/spark.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/LICENSE
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/NOTICE
--rw-r--r--   0        0        0    16007 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/README.md
--rw-r--r--   0        0        0    26416 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/pylint/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/pylint/__init__.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/pylint/airflow.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/pylint/all.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/pylint/cli.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/pylint/dbutils.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/pylint/legacy.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/pylint/mocking.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/pylint/notebooks.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/databricks/labs/pylint/spark.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/LICENSE
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/NOTICE
+-rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/README.md
+-rw-r--r--   0        0        0    26416 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    20009 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.2.0/PKG-INFO
```

### Comparing `databricks_labs_pylint-0.1.1/databricks/labs/pylint/airflow.py` & `databricks_labs_pylint-0.2.0/databricks/labs/pylint/airflow.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/databricks/labs/pylint/all.py` & `databricks_labs_pylint-0.2.0/databricks/labs/pylint/all.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/databricks/labs/pylint/cli.py` & `databricks_labs_pylint-0.2.0/databricks/labs/pylint/cli.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/databricks/labs/pylint/dbutils.py` & `databricks_labs_pylint-0.2.0/databricks/labs/pylint/dbutils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/databricks/labs/pylint/legacy.py` & `databricks_labs_pylint-0.2.0/databricks/labs/pylint/legacy.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/databricks/labs/pylint/mocking.py` & `databricks_labs_pylint-0.2.0/databricks/labs/pylint/mocking.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/databricks/labs/pylint/notebooks.py` & `databricks_labs_pylint-0.2.0/databricks/labs/pylint/notebooks.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/databricks/labs/pylint/spark.py` & `databricks_labs_pylint-0.2.0/databricks/labs/pylint/spark.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/.gitignore` & `databricks_labs_pylint-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/LICENSE` & `databricks_labs_pylint-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/NOTICE` & `databricks_labs_pylint-0.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.1/README.md` & `databricks_labs_pylint-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 
 and then use it with `pylint`:
 
 ```bash
 pylint --load-plugins=databricks.labs.pylint.all <your-python-file>.py
 ```
 
+You can also add `databricks.labs.pylint.all` to `load-plugins` configuration in your [`pylintrc` or `pyproject.toml` file](https://stackoverflow.com/q/22448731/277035).
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 # Integration with Databricks CLI
 
 You can use this plugin with Databricks CLI to check individual notebooks or entire directories. 
 
 First, you need to install this plugin locally:
@@ -121,140 +123,180 @@
  - `{I,C,R,W,E,F}` mean for `Info`, `Convention`, `Refactor`, `Warning`, `Error`, and `Fatal`.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 <!-- CHECKS -->
 
 ## `databricks-airflow` checker
+To use this checker, add `databricks.labs.pylint.airflow` to `load-plugins` configuration in your `pylintrc` or `pyproject.toml` file.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `W8901`: `missing-data-security-mode`
 
 XXX cluster missing `data_security_mode` required for Unity Catalog compatibility. Before you enable Unity Catalog, you must set the `data_security_mode` to 'NONE', so that your existing jobs would keep the same behavior. Failure to do so may cause your jobs to fail with unexpected errors.
 
+To disable this check on a specific line, add `# pylint: disable=missing-data-security-mode` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `W8902`: `unsupported-runtime`
 
 XXX cluster has unsupported runtime: XXX. The runtime version is not supported by Unity Catalog. Please upgrade to a runtime greater than or equal to 11.3.
 
+To disable this check on a specific line, add `# pylint: disable=unsupported-runtime` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ## `databricks-dbutils` checker
+To use this checker, add `databricks.labs.pylint.dbutils` to `load-plugins` configuration in your `pylintrc` or `pyproject.toml` file.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8903`: `dbutils-fs-cp`
 
 Use Databricks SDK instead: w.dbfs.copy(XXX, XXX). Migrate all usage of dbutils to Databricks SDK. See the more detailed documentation at https://databricks-sdk-py.readthedocs.io/en/latest/workspace/files/dbfs.html
 
+To disable this check on a specific line, add `# pylint: disable=dbutils-fs-cp` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8904`: `dbutils-fs-head`
 
 Use Databricks SDK instead: with w.dbfs.download(XXX) as f: f.read(). Migrate all usage of dbutils to Databricks SDK. See the more detailed documentation at https://databricks-sdk-py.readthedocs.io/en/latest/workspace/files/dbfs.html
 
+To disable this check on a specific line, add `# pylint: disable=dbutils-fs-head` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8905`: `dbutils-fs-ls`
 
 Use Databricks SDK instead: w.dbfs.list(XXX). Migrate all usage of dbutils to Databricks SDK. See the more detailed documentation at https://databricks-sdk-py.readthedocs.io/en/latest/workspace/files/dbfs.html
 
+To disable this check on a specific line, add `# pylint: disable=dbutils-fs-ls` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8906`: `dbutils-fs-mount`
 
 Mounts are not supported with Unity Catalog, switch to using Unity Catalog Volumes instead. Migrate all usage to Unity Catalog
 
+To disable this check on a specific line, add `# pylint: disable=dbutils-fs-mount` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8907`: `dbutils-credentials`
 
 Credentials utility is not supported with Unity Catalog. Migrate all usage to Unity Catalog
 
+To disable this check on a specific line, add `# pylint: disable=dbutils-credentials` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8908`: `dbutils-notebook-run`
 
 Use Databricks SDK instead: w.jobs.submit(
                 tasks=[jobs.SubmitTask(existing_cluster_id=...,
                                        notebook_task=jobs.NotebookTask(notebook_path=XXX),
                                        task_key=...)
                 ]).result(timeout=timedelta(minutes=XXX)). Migrate all usage of dbutils to Databricks SDK. See the more detailed documentation at https://databricks-sdk-py.readthedocs.io/en/latest/workspace/jobs/jobs.html
 
+To disable this check on a specific line, add `# pylint: disable=dbutils-notebook-run` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8909`: `pat-token-leaked`
 
 Use Databricks SDK instead: from databricks.sdk import WorkspaceClient(); w = WorkspaceClient(). Do not hardcode secrets in code, use Databricks SDK instead, which natively authenticates in Databricks Notebooks. See more at https://databricks-sdk-py.readthedocs.io/en/latest/authentication.html
 
+To disable this check on a specific line, add `# pylint: disable=pat-token-leaked` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8910`: `internal-api`
 
 Do not use internal APIs, rewrite using Databricks SDK: XXX. Do not use internal APIs. Use Databricks SDK for Python: https://databricks-sdk-py.readthedocs.io/en/latest/index.html
 
+To disable this check on a specific line, add `# pylint: disable=internal-api` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ## `databricks-legacy` checker
+To use this checker, add `databricks.labs.pylint.legacy` to `load-plugins` configuration in your `pylintrc` or `pyproject.toml` file.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8911`: `legacy-cli`
 
 Don't use databricks_cli, use databricks.sdk instead: pip install databricks-sdk. Migrate all usage of Legacy CLI to Databricks SDK. See the more detailed documentation at https://databricks-sdk-py.readthedocs.io/en/latest/index.html
 
+To disable this check on a specific line, add `# pylint: disable=legacy-cli` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `W8912`: `incompatible-with-uc`
 
 Incompatible with Unity Catalog: XXX. Migrate all usage to Databricks Unity Catalog. Use https://github.com/databrickslabs/ucx for more details
 
+To disable this check on a specific line, add `# pylint: disable=incompatible-with-uc` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ## `databricks-notebooks` checker
+To use this checker, add `databricks.labs.pylint.notebooks` to `load-plugins` configuration in your `pylintrc` or `pyproject.toml` file.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `C8913`: `notebooks-too-many-cells`
 
 Notebooks should not have more than 75 cells. Otherwise, it's hard to maintain and understand the notebook for other people and the future you
 
+To disable this check on a specific line, add `# pylint: disable=notebooks-too-many-cells` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8914`: `notebooks-percent-run`
 
 Using %run is not allowed. Use functions instead of %run to avoid side effects and make the code more testable. If you need to share code between notebooks, consider creating a library. If still need to call another code as a separate job, use Databricks SDK for Python: https://databricks-sdk-py.readthedocs.io/en/latest/index.html
 
+To disable this check on a specific line, add `# pylint: disable=notebooks-percent-run` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ## `spark` checker
+To use this checker, add `databricks.labs.pylint.spark` to `load-plugins` configuration in your `pylintrc` or `pyproject.toml` file.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `C8915`: `spark-outside-function`
 
 Using spark outside the function is leading to untestable code. Do not use global spark object, pass it as an argument to the function instead, so that the function becomes testable in a CI/CD pipelines.
 
+To disable this check on a specific line, add `# pylint: disable=spark-outside-function` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `C8917`: `use-display-instead-of-show`
 
 Rewrite to display in a notebook: display(XXX). Use display() instead of show() to visualize the data in a notebook.
 
+To disable this check on a specific line, add `# pylint: disable=use-display-instead-of-show` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `W8916`: `no-spark-argument-in-function`
 
 Function XXX is missing a 'spark' argument. Function refers to a global spark variable, which may not always be available. Pass the spark object as an argument to the function instead, so that the function becomes testable in a CI/CD pipelines.
 
+To disable this check on a specific line, add `# pylint: disable=no-spark-argument-in-function` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ## `mocking` checker
+To use this checker, add `databricks.labs.pylint.mocking` to `load-plugins` configuration in your `pylintrc` or `pyproject.toml` file.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8918`: `explicit-dependency-required`
 
 Obscure implicit test dependency with mock.patch(XXX). Rewrite to inject dependencies through constructor.. Using `patch` to mock dependencies in unit tests can introduce implicit 
 dependencies within a class, making it unclear to other developers. Constructor arguments, on the other hand, 
@@ -272,25 +314,29 @@
 dependency inversion, enabling the use of interfaces to decouple the class under test from concrete classes.
 This decoupling facilitates unit testing, as it allows for the substitution of mock objects for concrete
 implementations, ensuring that the class under test behaves as expected. By following this approach, you can
 create more robust and maintainable unit tests, improving the overall quality of your codebase.
 
 Use `require-explicit-dependency` option to specify the package names that contain code for your project.
 
+To disable this check on a specific line, add `# pylint: disable=explicit-dependency-required` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ### `R8919`: `obscure-mock`
 
 Obscure implicit test dependency with MagicMock(). Rewrite with create_autospec(ConcreteType).. Using `MagicMock` to mock dependencies in unit tests can introduce implicit dependencies 
 within a class, making it unclear to other developers. create_autospec(ConcreteType) is a better alternative, as it
 automatically creates a mock object with the same attributes and methods as the concrete class. This
 approach ensures that the mock object behaves like the concrete class, allowing for more robust and
 maintainable unit tests. Moreover, reliance on `MagicMock` for testing leads to issues during refactoring,
 as updates to underlying implementations would necessitate changes across multiple unrelated unit tests.
 
+To disable this check on a specific line, add `# pylint: disable=obscure-mock` at the end of it.
+
 [[back to top](#pylint-plugin-for-databricks)]
 
 ## Testing in isolation
 To test this plugin in isolation, you can use the following command:
 
 ```bash
 pylint --load-plugins=databricks.labs.pylint.all --disable=all --enable=missing-data-security-mode,unsupported-runtime,dbutils-fs-cp,dbutils-fs-head,dbutils-fs-ls,dbutils-fs-mount,dbutils-credentials,dbutils-notebook-run,pat-token-leaked,internal-api,legacy-cli,incompatible-with-uc,notebooks-too-many-cells,notebooks-percent-run,spark-outside-function,use-display-instead-of-show,no-spark-argument-in-function,explicit-dependency-required,obscure-mock .
```

### Comparing `databricks_labs_pylint-0.1.1/pyproject.toml` & `databricks_labs_pylint-0.2.0/pyproject.toml`

 * *Files identical despite different names*

