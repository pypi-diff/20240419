# Comparing `tmp/dagster-airflow-1.7.2rc2.tar.gz` & `tmp/dagster-airflow-1.7.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airflow-1.7.2rc2.tar", last modified: Tue Apr 16 20:35:35 2024, max compression
+gzip compressed data, was "dagster-airflow-1.7.2rc3.tar", last modified: Thu Apr 18 21:16:44 2024, max compression
```

## Comparing `dagster-airflow-1.7.2rc2.tar` & `dagster-airflow-1.7.2rc3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:35.611982 dagster-airflow-1.7.2rc2/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      105 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      659 2024-04-16 20:35:35.611982 dagster-airflow-1.7.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:35.603982 dagster-airflow-1.7.2rc2/dagster_airflow/
--rw-r--r--   0 root         (0) root         (0)     2474 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3815 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/airflow_dag_converter.py
--rw-r--r--   0 root         (0) root         (0)     7765 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/dagster_asset_factory.py
--rw-r--r--   0 root         (0) root         (0)     8234 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/dagster_factory.py
--rw-r--r--   0 root         (0) root         (0)     3900 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/dagster_job_factory.py
--rw-r--r--   0 root         (0) root         (0)     1763 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/dagster_schedule_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:35.607982 dagster-airflow-1.7.2rc2/dagster_airflow/hooks/
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9070 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/hooks/dagster_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:35.607982 dagster-airflow-1.7.2rc2/dagster_airflow/links/
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/links/dagster_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:35.607982 dagster-airflow-1.7.2rc2/dagster_airflow/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/operators/dagster_operator.py
--rw-r--r--   0 root         (0) root         (0)      651 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/patch_airflow_example_dag.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:35.611982 dagster-airflow-1.7.2rc2/dagster_airflow/resources/
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3651 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/resources/airflow_db.py
--rw-r--r--   0 root         (0) root         (0)     3659 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/resources/airflow_ephemeral_db.py
--rw-r--r--   0 root         (0) root         (0)     4037 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/resources/airflow_persistent_db.py
--rw-r--r--   0 root         (0) root         (0)     4496 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/utils.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/dagster_airflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:35:35.603982 dagster-airflow-1.7.2rc2/dagster_airflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      659 2024-04-16 20:35:35.000000 dagster-airflow-1.7.2rc2/dagster_airflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2024-04-16 20:35:35.000000 dagster-airflow-1.7.2rc2/dagster_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:35:35.000000 dagster-airflow-1.7.2rc2/dagster_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      168 2024-04-16 20:35:35.000000 dagster-airflow-1.7.2rc2/dagster_airflow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      554 2024-04-16 20:35:35.000000 dagster-airflow-1.7.2rc2/dagster_airflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-16 20:35:35.000000 dagster-airflow-1.7.2rc2/dagster_airflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      192 2024-04-16 20:35:35.635982 dagster-airflow-1.7.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3114 2024-04-16 20:26:55.000000 dagster-airflow-1.7.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:44.309716 dagster-airflow-1.7.2rc3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      105 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      659 2024-04-18 21:16:44.309716 dagster-airflow-1.7.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:44.301716 dagster-airflow-1.7.2rc3/dagster_airflow/
+-rw-r--r--   0 root         (0) root         (0)     2474 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/airflow_dag_converter.py
+-rw-r--r--   0 root         (0) root         (0)     7765 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/dagster_asset_factory.py
+-rw-r--r--   0 root         (0) root         (0)     8234 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/dagster_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/dagster_job_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/dagster_schedule_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:44.301716 dagster-airflow-1.7.2rc3/dagster_airflow/hooks/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9070 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/hooks/dagster_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:44.305716 dagster-airflow-1.7.2rc3/dagster_airflow/links/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/links/dagster_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:44.305716 dagster-airflow-1.7.2rc3/dagster_airflow/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/operators/dagster_operator.py
+-rw-r--r--   0 root         (0) root         (0)      651 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/patch_airflow_example_dag.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:44.309716 dagster-airflow-1.7.2rc3/dagster_airflow/resources/
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3651 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/resources/airflow_db.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/resources/airflow_ephemeral_db.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/resources/airflow_persistent_db.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/utils.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/dagster_airflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:16:44.301716 dagster-airflow-1.7.2rc3/dagster_airflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      659 2024-04-18 21:16:44.000000 dagster-airflow-1.7.2rc3/dagster_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-04-18 21:16:44.000000 dagster-airflow-1.7.2rc3/dagster_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:16:44.000000 dagster-airflow-1.7.2rc3/dagster_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-18 21:16:44.000000 dagster-airflow-1.7.2rc3/dagster_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      554 2024-04-18 21:16:44.000000 dagster-airflow-1.7.2rc3/dagster_airflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-18 21:16:44.000000 dagster-airflow-1.7.2rc3/dagster_airflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2024-04-18 21:16:44.329716 dagster-airflow-1.7.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3114 2024-04-18 21:10:09.000000 dagster-airflow-1.7.2rc3/setup.py
```

### Comparing `dagster-airflow-1.7.2rc2/LICENSE` & `dagster-airflow-1.7.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/PKG-INFO` & `dagster-airflow-1.7.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airflow
-Version: 1.7.2rc2
+Version: 1.7.2rc3
 Summary: Airflow plugin for Dagster
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: project-url/documentation, https://docs.dagster.io
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/__init__.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/airflow_dag_converter.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/airflow_dag_converter.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/dagster_asset_factory.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/dagster_asset_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/dagster_factory.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/dagster_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/dagster_job_factory.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/dagster_job_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/dagster_schedule_factory.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/dagster_schedule_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/hooks/dagster_hook.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/hooks/dagster_hook.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/links/dagster_link.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/links/dagster_link.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/operators/dagster_operator.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/operators/dagster_operator.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/patch_airflow_example_dag.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/patch_airflow_example_dag.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/resources/airflow_db.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/resources/airflow_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/resources/airflow_ephemeral_db.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/resources/airflow_ephemeral_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/resources/airflow_persistent_db.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/resources/airflow_persistent_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow/utils.py` & `dagster-airflow-1.7.2rc3/dagster_airflow/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow.egg-info/PKG-INFO` & `dagster-airflow-1.7.2rc3/dagster_airflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airflow
-Version: 1.7.2rc2
+Version: 1.7.2rc3
 Summary: Airflow plugin for Dagster
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: project-url/documentation, https://docs.dagster.io
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow.egg-info/SOURCES.txt` & `dagster-airflow-1.7.2rc3/dagster_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.7.2rc2/dagster_airflow.egg-info/requires.txt` & `dagster-airflow-1.7.2rc3/dagster_airflow.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dagster==1.7.2rc2
+dagster==1.7.2rc3
 docker<6.0.0,>=5.0.3
 urllib3<2
 lazy_object_proxy
 
 [kubernetes]
 kubernetes>=3.0.0
 cryptography>=2.0.0
```

### Comparing `dagster-airflow-1.7.2rc2/setup.py` & `dagster-airflow-1.7.2rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airflow_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.2rc2",
+        "dagster==1.7.2rc3",
         "docker>=5.0.3,<6.0.0",
         "urllib3<2",  # docker version pinned above requires this but has no pin
         "lazy_object_proxy",
     ],
     project_urls={
         # airflow will embed a link this in the providers page UI
         "project-url/documentation": "https://docs.dagster.io",
```

