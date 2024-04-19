# Comparing `tmp/q_alchemy_sdk_py-0.2.3.tar.gz` & `tmp/q_alchemy_sdk_py-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q_alchemy_sdk_py-0.2.3.tar", last modified: Wed Apr 17 18:12:00 2024, max compression
+gzip compressed data, was "q_alchemy_sdk_py-0.2.4.tar", last modified: Fri Apr 19 13:36:25 2024, max compression
```

## Comparing `q_alchemy_sdk_py-0.2.3.tar` & `q_alchemy_sdk_py-0.2.4.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0    11556 2024-03-19 19:59:43.321774 q_alchemy_sdk_py-0.2.3/LICENSE
--rw-r--r--   0        0        0     3132 2024-04-03 07:57:53.501345 q_alchemy_sdk_py-0.2.3/README.md
--rw-r--r--   0        0        0      647 2024-04-17 18:12:00.597887 q_alchemy_sdk_py-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      599 2024-04-03 07:57:53.523366 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/__init__.py
--rw-r--r--   0        0        0      844 2024-04-17 17:54:37.354574 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/__init__.py
--rw-r--r--   0        0        0      771 2024-04-17 17:54:32.473184 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/base_relations.py
--rw-r--r--   0        0        0     1237 2024-04-17 17:54:11.519581 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/enterapi.py
--rw-r--r--   0        0        0      645 2024-04-17 17:54:15.151139 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/exceptions.py
--rw-r--r--   0        0        0      599 2024-04-17 17:55:17.420851 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/__init__.py
--rw-r--r--   0        0        0     2955 2024-04-17 17:54:56.794799 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/action_hco.py
--rw-r--r--   0        0        0     3906 2024-04-17 17:54:59.617204 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/action_with_parameters_hco.py
--rw-r--r--   0        0        0     2002 2024-04-17 17:55:02.356072 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/download_link_hco.py
--rw-r--r--   0        0        0     4062 2024-04-17 17:55:05.889416 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/hco_base.py
--rw-r--r--   0        0        0     2573 2024-04-17 17:55:09.246155 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/link_hco.py
--rw-r--r--   0        0        0     5287 2024-04-17 17:55:12.020199 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/upload_action_hco.py
--rw-r--r--   0        0        0      793 2024-04-17 17:54:18.992349 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/http_headers.py
--rw-r--r--   0        0        0     1225 2024-04-17 17:54:21.836368 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/media_types.py
--rw-r--r--   0        0        0      599 2024-04-17 17:54:43.443856 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/__init__.py
--rw-r--r--   0        0        0      825 2024-04-17 17:54:47.871461 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/error.py
--rw-r--r--   0        0        0     6303 2024-04-17 17:54:50.396063 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/sirenmodels.py
--rw-r--r--   0        0        0     1715 2024-04-17 17:54:25.520035 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/polling.py
--rw-r--r--   0        0        0     7752 2024-04-17 17:54:28.807755 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/sirenaccess.py
--rw-r--r--   0        0        0      745 2024-04-17 17:58:05.367005 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/__init__.py
--rw-r--r--   0        0        0     2118 2024-04-17 17:58:05.443658 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/enterjma.py
--rw-r--r--   0        0        0     1009 2024-04-17 17:55:21.823595 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/__init__.py
--rw-r--r--   0        0        0     3006 2024-04-17 17:55:24.271483 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/entrypoint_hco.py
--rw-r--r--   0        0        0     1991 2024-04-17 17:58:05.380312 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/info_hco.py
--rw-r--r--   0        0        0     3704 2024-04-17 17:55:34.427616 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py
--rw-r--r--   0        0        0     8200 2024-04-17 17:55:38.341171 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_hco.py
--rw-r--r--   0        0        0     3678 2024-04-17 17:55:42.295023 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_query_result_hco.py
--rw-r--r--   0        0        0     1591 2024-04-17 17:55:46.843240 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py
--rw-r--r--   0        0        0     4361 2024-04-17 17:55:50.628166 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/jobsroot_hco.py
--rw-r--r--   0        0        0     2149 2024-04-17 17:55:54.343397 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py
--rw-r--r--   0        0        0     3727 2024-04-17 17:55:57.027348 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processing_step_hco.py
--rw-r--r--   0        0        0     1714 2024-04-17 17:56:00.072771 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py
--rw-r--r--   0        0        0     3937 2024-04-17 17:56:03.543447 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py
--rw-r--r--   0        0        0     4471 2024-04-17 17:56:06.626480 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py
--rw-r--r--   0        0        0     1749 2024-04-17 17:56:09.508138 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/user_hco.py
--rw-r--r--   0        0        0     5694 2024-04-17 17:56:12.858256 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_hco.py
--rw-r--r--   0        0        0     3616 2024-04-17 17:56:15.879756 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py
--rw-r--r--   0        0        0     1734 2024-04-17 17:58:05.405575 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_used_tags_query_result_hco.py
--rw-r--r--   0        0        0     4772 2024-04-17 17:58:05.393524 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdataroot_hco.py
--rw-r--r--   0        0        0     1223 2024-04-17 17:57:39.063985 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/known_relations.py
--rw-r--r--   0        0        0      636 2024-04-17 17:56:40.970595 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/__init__.py
--rw-r--r--   0        0        0    29427 2024-04-17 17:53:00.614623 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/open_api_generated.py
--rw-r--r--   0        0        0     3923 2024-04-17 17:58:05.415173 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/sirenentities.py
--rw-r--r--   0        0        0      623 2024-04-17 17:57:03.466217 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/tool/__init__.py
--rw-r--r--   0        0        0    14478 2024-04-17 17:58:05.423395 q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/tool/job.py
--rw-r--r--   0        0        0        0 2024-04-03 07:57:53.558405 q_alchemy_sdk_py-0.2.3/src/q_alchemy/__init__.py
--rw-r--r--   0        0        0     7106 2024-04-17 18:09:47.453203 q_alchemy_sdk_py-0.2.3/src/q_alchemy/qiskit_integration.py
--rw-r--r--   0        0        0      603 2024-03-19 19:59:43.347535 q_alchemy_sdk_py-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0    16512 2024-03-19 19:59:43.350535 q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.10.1.npy
--rw-r--r--   0        0        0    65664 2024-03-19 19:59:43.351535 q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.12.1.npy
--rw-r--r--   0        0        0     2176 2024-03-19 19:59:43.352534 q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.7.1.npy
--rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 q_alchemy_sdk_py-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11556 2024-03-19 19:59:43.321774 q_alchemy_sdk_py-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3132 2024-04-19 13:35:07.213197 q_alchemy_sdk_py-0.2.4/README.md
+-rw-r--r--   0        0        0      672 2024-04-19 13:36:25.319781 q_alchemy_sdk_py-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      599 2024-04-19 13:35:07.228950 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/__init__.py
+-rw-r--r--   0        0        0      844 2024-04-19 13:35:07.230172 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-19 13:35:07.230172 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/base_relations.py
+-rw-r--r--   0        0        0     1237 2024-04-19 13:35:07.230172 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/enterapi.py
+-rw-r--r--   0        0        0      645 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/exceptions.py
+-rw-r--r--   0        0        0      599 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/__init__.py
+-rw-r--r--   0        0        0     2955 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/action_hco.py
+-rw-r--r--   0        0        0     3906 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/action_with_parameters_hco.py
+-rw-r--r--   0        0        0     2002 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/download_link_hco.py
+-rw-r--r--   0        0        0     4062 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/hco_base.py
+-rw-r--r--   0        0        0     2573 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/link_hco.py
+-rw-r--r--   0        0        0     5287 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/upload_action_hco.py
+-rw-r--r--   0        0        0      793 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/http_headers.py
+-rw-r--r--   0        0        0     1225 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/media_types.py
+-rw-r--r--   0        0        0      599 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/model/__init__.py
+-rw-r--r--   0        0        0      825 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/model/error.py
+-rw-r--r--   0        0        0     6303 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/model/sirenmodels.py
+-rw-r--r--   0        0        0     1715 2024-04-19 13:35:07.235133 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/polling.py
+-rw-r--r--   0        0        0     7752 2024-04-19 13:35:07.235133 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/sirenaccess.py
+-rw-r--r--   0        0        0      745 2024-04-19 13:35:07.235133 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/__init__.py
+-rw-r--r--   0        0        0     2118 2024-04-19 13:35:07.236487 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/enterjma.py
+-rw-r--r--   0        0        0     1009 2024-04-19 13:35:07.236487 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/__init__.py
+-rw-r--r--   0        0        0     3006 2024-04-19 13:35:07.236487 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/entrypoint_hco.py
+-rw-r--r--   0        0        0     1991 2024-04-19 13:35:07.237685 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/info_hco.py
+-rw-r--r--   0        0        0     3704 2024-04-19 13:35:07.237685 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py
+-rw-r--r--   0        0        0     8200 2024-04-19 13:35:07.237685 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/job_hco.py
+-rw-r--r--   0        0        0     3678 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/job_query_result_hco.py
+-rw-r--r--   0        0        0     1591 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py
+-rw-r--r--   0        0        0     4361 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/jobsroot_hco.py
+-rw-r--r--   0        0        0     2149 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py
+-rw-r--r--   0        0        0     3727 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/processing_step_hco.py
+-rw-r--r--   0        0        0     1714 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py
+-rw-r--r--   0        0        0     3937 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py
+-rw-r--r--   0        0        0     4471 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py
+-rw-r--r--   0        0        0     1749 2024-04-19 13:35:07.241868 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/user_hco.py
+-rw-r--r--   0        0        0     5694 2024-04-19 13:35:07.241868 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/workdata_hco.py
+-rw-r--r--   0        0        0     3616 2024-04-19 13:35:07.241868 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py
+-rw-r--r--   0        0        0     1734 2024-04-19 13:35:07.242875 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/workdata_used_tags_query_result_hco.py
+-rw-r--r--   0        0        0     4772 2024-04-19 13:35:07.242875 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/workdataroot_hco.py
+-rw-r--r--   0        0        0     1223 2024-04-19 13:35:07.242875 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/known_relations.py
+-rw-r--r--   0        0        0      636 2024-04-19 13:35:07.244338 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/model/__init__.py
+-rw-r--r--   0        0        0    29427 2024-04-19 13:35:07.244338 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/model/open_api_generated.py
+-rw-r--r--   0        0        0     3923 2024-04-19 13:35:07.244338 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/model/sirenentities.py
+-rw-r--r--   0        0        0      623 2024-04-19 13:35:07.245525 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/tool/__init__.py
+-rw-r--r--   0        0        0    14478 2024-04-19 13:35:07.245525 q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/tool/job.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:35:07.245525 q_alchemy_sdk_py-0.2.4/src/q_alchemy/__init__.py
+-rw-r--r--   0        0        0     8056 2024-04-19 13:35:07.246725 q_alchemy_sdk_py-0.2.4/src/q_alchemy/qiskit_integration.py
+-rw-r--r--   0        0        0     4354 2024-04-19 13:35:07.246725 q_alchemy_sdk_py-0.2.4/src/q_alchemy/qiskit_to_pennylane.py
+-rw-r--r--   0        0        0      603 2024-03-19 19:59:43.347535 q_alchemy_sdk_py-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0    16512 2024-03-19 19:59:43.350535 q_alchemy_sdk_py-0.2.4/tests/data/test_baa_state.10.1.npy
+-rw-r--r--   0        0        0    65664 2024-03-19 19:59:43.351535 q_alchemy_sdk_py-0.2.4/tests/data/test_baa_state.12.1.npy
+-rw-r--r--   0        0        0     2176 2024-03-19 19:59:43.352534 q_alchemy_sdk_py-0.2.4/tests/data/test_baa_state.7.1.npy
+-rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 q_alchemy_sdk_py-0.2.4/PKG-INFO
```

### Comparing `q_alchemy_sdk_py-0.2.3/LICENSE` & `q_alchemy_sdk_py-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/README.md` & `q_alchemy_sdk_py-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/pyproject.toml` & `q_alchemy_sdk_py-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "q-alchemy-sdk-py"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = [
     { name = "Carsten Blank", email = "blank@data-cybernetics.com" },
 ]
 dependencies = [
     "qiskit>=1.0.2",
     "pydantic>=2.6.4",
     "httpx<1.0.0,>=0.25.0",
+    "pennylane>=0.35.1",
 ]
 requires-python = "<4,>=3.11"
 readme = "README.md"
 
 [project.license]
 text = "Apache"
```

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/__init__.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/__init__.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/base_relations.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/base_relations.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/enterapi.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/enterapi.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/exceptions.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/__init__.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/action_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/action_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/action_with_parameters_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/action_with_parameters_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/download_link_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/download_link_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/hco_base.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/hco_base.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/link_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/link_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/hco/upload_action_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/hco/upload_action_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/http_headers.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/http_headers.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/media_types.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/media_types.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/__init__.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/error.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/model/error.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/model/sirenmodels.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/model/sirenmodels.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/polling.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/polling.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/core/sirenaccess.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/core/sirenaccess.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/__init__.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/enterjma.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/enterjma.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/__init__.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/entrypoint_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/entrypoint_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/info_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/info_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/job_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_query_result_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/job_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/jobsroot_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/jobsroot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processing_step_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/processing_step_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/user_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/user_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/workdata_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdata_used_tags_query_result_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/workdata_used_tags_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/hcos/workdataroot_hco.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/hcos/workdataroot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/known_relations.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/known_relations.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/__init__.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/model/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/open_api_generated.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/model/open_api_generated.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/model/sirenentities.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/model/sirenentities.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/tool/__init__.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/hypermedia_client/job_management/tool/job.py` & `q_alchemy_sdk_py-0.2.4/src/hypermedia_client/job_management/tool/job.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/src/q_alchemy/qiskit_integration.py` & `q_alchemy_sdk_py-0.2.4/src/q_alchemy/qiskit_integration.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
+import inspect
 import logging
 import os
 import hashlib
 from dataclasses import dataclass, field
 from typing import List, Dict, Tuple
 
 import httpx
@@ -40,16 +41,25 @@
     api_key: str = field(default_factory=lambda: os.getenv("Q_ALCHEMY_API_KEY"))
     host: str = field(default="jobs.api.q-alchemy.com")
     schema: str = field(default="https")
     added_headers: Dict[str, str] = field(default_factory=dict)
     isometry_scheme: str = field(default="ccd")
     unitary_scheme: str = field(default="qsd")
     job_completion_timeout_sec: int = field(default=300)
-    basis_gates: List[str] = field(default_factory=lambda: ["u1", "u2", "u3", "cx"])
+    basis_gates: List[str] = field(default_factory=lambda: ["rx", "ry", "rz", "cx"])
     image_size: Tuple[int, int] = field(default=(-1, -1))
+    with_debug_data: bool = field(default=False)
+    assign_data_hash: bool = field(default=True)
+
+    @classmethod
+    def from_dict(cls, env):
+        return cls(**{
+            k: v for k, v in env.items()
+            if k in inspect.signature(cls).parameters
+        })
 
 
 class QAlchemyInitialize(Instruction):
     """
     State preparation using Q-Alchemy API
 
     This class implements a state preparation gate.
@@ -79,14 +89,15 @@
 
             unitary_scheme: string
                 Scheme used to decompose unitaries.
                 Possible values are ``'csd'`` (cosine-sine decomposition) and ``'qsd'`` (quantum
                 Shannon decomposition).
                 Default is ``unitary_scheme='qsd'``.
         """
+        params = np.asarray(params, dtype=complex).tolist()
         num_qubits = int(np.ceil(np.log2(len(params))))
         if opt_params is None:
             self.opt_params = OptParams()
         elif isinstance(opt_params, OptParams):
             self.opt_params = opt_params
         else:
             self.opt_params = OptParams(**opt_params)
@@ -97,46 +108,62 @@
             label = "QAl"
         self.client = httpx.Client(
             base_url=f"{self.opt_params.schema}://{self.opt_params.host}",
             headers=headers,
             timeout=httpx.Timeout(timeout=self.opt_params.job_completion_timeout_sec + 10.0, connect=10.0)
         )
         super().__init__("q-alchemy", num_qubits, 0, params=params, label=label)
-        self.param_hash = hashlib.md5(np.asarray(self.params).tobytes()).hexdigest()
+        if self.opt_params.assign_data_hash:
+            self.param_hash = hashlib.md5(np.asarray(self.params).tobytes()).hexdigest()
+        else:
+            self.param_hash = datetime.datetime.utcnow().timestamp()
 
     def _define(self):
-        sequence_wd_tags = [f"Hash={self.param_hash}", "Source=Qiskit-Integration", f"ImageSize={self.opt_params.image_size}"]
+        sequence_wd_tags = [
+            f"Hash={self.param_hash}",
+            "Source=Qiskit-Integration",
+            f"ImageSize={self.opt_params.image_size}"
+        ]
+        sequence_wd_tags += self.opt_params.job_tags
         wd_root = enter_jma(self.client).work_data_root_link.navigate()
 
         existing_wd_query = wd_root.query_action.execute(WorkDataQueryParameters(
             filter=WorkDataFilterParameter(tags_by_and=sequence_wd_tags)
         ))
 
         if existing_wd_query.total_entities == 0:
             wd_root = enter_jma(self.client).work_data_root_link.navigate()
             wd_link = wd_root.upload_action.execute(UploadParameters(
                 filename=f"{self.param_hash}.bin",
-                binary=np.asarray(self.params).tobytes(),
+                binary=np.asarray(self.params, dtype=np.complex128).tobytes(),
                 mediatype=MediaTypes.OCTET_STREAM,
             ))
-            wd_link.navigate().edit_tags_action.execute(SetTagsWorkDataParameters(tags=sequence_wd_tags))
+            wd_link.navigate().edit_tags_action.execute(
+                SetTagsWorkDataParameters(tags=sequence_wd_tags)
+            )
         else:
             wd_link = existing_wd_query.workdatas[0].self_link
 
         job_timeout = self.opt_params.job_completion_timeout_sec * 1000
+        processing_name = "convert_circuit_layers_qasm_only"
+        job_parameters = dict(
+            min_fidelity=1.0 - self.opt_params.max_fidelity_loss,
+            basis_gates=self.opt_params.basis_gates,
+        )
+        if all(i > 0 for i in self.opt_params.image_size) or self.opt_params.with_debug_data:
+            processing_name = "convert_circuit_layers"
+            job_parameters.update(dict(
+                image_shape_x=self.opt_params.image_size[0],
+                image_shape_y=self.opt_params.image_size[1]
+            ))
         job = (
             Job(self.client)
             .create(name=f'Execute Transformation ({datetime.datetime.now()})')
-            .select_processing(processing_step='convert_circuit_layers')
-            .configure_parameters(
-                min_fidelity=1.0 - self.opt_params.max_fidelity_loss,
-                basis_gates=self.opt_params.basis_gates,
-                image_shape_x=self.opt_params.image_size[0],
-                image_shape_y=self.opt_params.image_size[1]
-            )
+            .select_processing(processing_step=processing_name)
+            .configure_parameters(**job_parameters)
             .assign_input_dataslot(0, wd_link)
             .allow_output_data_deletion()
             .start()
             .wait_for_state(JobStates.completed, timeout_ms=job_timeout)
         )
         self.result_summary: dict = job.get_result()
         inner_job = job._job
```

### Comparing `q_alchemy_sdk_py-0.2.3/tests/__init__.py` & `q_alchemy_sdk_py-0.2.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.10.1.npy` & `q_alchemy_sdk_py-0.2.4/tests/data/test_baa_state.10.1.npy`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.12.1.npy` & `q_alchemy_sdk_py-0.2.4/tests/data/test_baa_state.12.1.npy`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/tests/data/test_baa_state.7.1.npy` & `q_alchemy_sdk_py-0.2.4/tests/data/test_baa_state.7.1.npy`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.3/PKG-INFO` & `q_alchemy_sdk_py-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: q-alchemy-sdk-py
-Version: 0.2.3
+Version: 0.2.4
 Author-Email: Carsten Blank <blank@data-cybernetics.com>
 License: Apache
 Requires-Python: <4,>=3.11
 Requires-Dist: qiskit>=1.0.2
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: httpx<1.0.0,>=0.25.0
+Requires-Dist: pennylane>=0.35.1
 Description-Content-Type: text/markdown
 
 # Q-Alchemy Python SDK
 
 This is the Python-SDK for using the data cybernetics [Q-Alchemy](https://www.q-alchemy.com) 
 API which helps quantum computing researchers to put classical data into the quantum computer.
 This is all also called: the loading problem, encoding problem, or quantum state preparation.
```

