# Comparing `tmp/great_expectations_cloud-20240418.0.tar.gz` & `tmp/great_expectations_cloud-20240419.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240418.0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240419.0.dev0.tar", max compression
```

## Comparing `great_expectations_cloud-20240418.0.tar` & `great_expectations_cloud-20240419.0.dev0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2084 2024-04-18 04:42:17.870576 great_expectations_cloud-20240418.0/LICENSE
--rw-r--r--   0        0        0     7568 2024-04-18 04:42:17.870576 great_expectations_cloud-20240418.0/README.md
--rw-r--r--   0        0        0      150 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      862 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     3054 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py
--rw-r--r--   0        0        0     2993 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      733 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    16465 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0     1951 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4598 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0      362 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/agent/warnings.py
--rw-r--r--   0        0        0     1762 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     3130 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9416 2024-04-18 04:42:17.902576 great_expectations_cloud-20240418.0/pyproject.toml
--rw-r--r--   0        0        0     8897 1970-01-01 00:00:00.000000 great_expectations_cloud-20240418.0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-04-19 16:10:17.827527 great_expectations_cloud-20240419.0.dev0/LICENSE
+-rw-r--r--   0        0        0     8305 2024-04-19 16:10:17.827527 great_expectations_cloud-20240419.0.dev0/README.md
+-rw-r--r--   0        0        0      150 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     3054 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py
+-rw-r--r--   0        0        0     2993 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      733 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    16465 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0     1951 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4598 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0      362 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/warnings.py
+-rw-r--r--   0        0        0     1762 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     3130 2024-04-19 16:10:17.855527 great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0     9421 2024-04-19 16:10:17.859527 great_expectations_cloud-20240419.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     9639 1970-01-01 00:00:00.000000 great_expectations_cloud-20240419.0.dev0/PKG-INFO
```

### Comparing `great_expectations_cloud-20240418.0/LICENSE` & `great_expectations_cloud-20240419.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/README.md` & `great_expectations_cloud-20240419.0.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -200,7 +200,17 @@
 
 ```console
 invoke release
 ```
 
 This will create a new release version. On the next merge to `main`, the release will be uploaded to PyPi.
 A new docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
+
+#### Github Workflow for releasing
+
+We use the GitHub Actions workflow to automate the release and pre-release process. There are two workflows involved:
+
+1. [CI](./.github/workflows/ci.yml) - This workflow runs on each pull request and will update the version in `pyproject.toml` to the pre-release version if the version is not already manually updated in the PR. It will also run the tests and linting.
+
+2. [Containerize Agent](./.github/workflows/containerize-agent.yml) - This workflows runs on merge with `main` and will create a new docker image and push it to Docker Hub and PyPi. It uses the version in `pyproject.toml`.
+
+A visual representation of the workflow is shown [here](./.github/workflows/agent_release_workflows.png)
```

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_column_descriptive_metrics_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/run_metric_list_action.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/actions/unknown.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/agent.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/event_handler.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/great_expectations_cloud/logging/logging_cfg.py` & `great_expectations_cloud-20240419.0.dev0/great_expectations_cloud/logging/logging_cfg.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240418.0/pyproject.toml` & `great_expectations_cloud-20240419.0.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240418.0"
+version = "20240419.0.dev0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
```

### Comparing `great_expectations_cloud-20240418.0/PKG-INFO` & `great_expectations_cloud-20240419.0.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240418.0
+Version: 20240419.0.dev0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -234,7 +234,17 @@
 ```console
 invoke release
 ```
 
 This will create a new release version. On the next merge to `main`, the release will be uploaded to PyPi.
 A new docker tag will also be generated and pushed to [Docker Hub](https://hub.docker.com/r/greatexpectations/agent)
 
+#### Github Workflow for releasing
+
+We use the GitHub Actions workflow to automate the release and pre-release process. There are two workflows involved:
+
+1. [CI](./.github/workflows/ci.yml) - This workflow runs on each pull request and will update the version in `pyproject.toml` to the pre-release version if the version is not already manually updated in the PR. It will also run the tests and linting.
+
+2. [Containerize Agent](./.github/workflows/containerize-agent.yml) - This workflows runs on merge with `main` and will create a new docker image and push it to Docker Hub and PyPi. It uses the version in `pyproject.toml`.
+
+A visual representation of the workflow is shown [here](./.github/workflows/agent_release_workflows.png)
+
```

