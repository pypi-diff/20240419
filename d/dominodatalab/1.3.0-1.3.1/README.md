# Comparing `tmp/dominodatalab-1.3.0.tar.gz` & `tmp/dominodatalab-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/olson.dimanche/repos/python-domino/dist/.tmp-6w16a3ks/dominodatalab-1.3.0.tar", last modified: Fri Jan 19 18:59:40 2024, max compression
+gzip compressed data, was "dominodatalab-1.3.1.tar", last modified: Fri Apr 19 13:15:35 2024, max compression
```

## Comparing `dominodatalab-1.3.0.tar` & `dominodatalab-1.3.1.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    11358 2022-06-06 14:00:07.000000 dominodatalab-1.3.0/LICENSE.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)       14 2022-06-21 20:35:17.000000 dominodatalab-1.3.0/MANIFEST.in
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    23030 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/PKG-INFO
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    22487 2024-01-19 18:52:22.000000 dominodatalab-1.3.0/README.md
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/domino/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      105 2022-06-21 20:35:17.000000 dominodatalab-1.3.0/domino/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9576 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_custom_metrics.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/domino/_impl/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)        0 2022-10-18 20:07:39.000000 dominodatalab-1.3.0/domino/_impl/__init__.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      821 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    58419 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/api_client.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      214 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      972 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/path_to_api.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/paths/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      253 2022-10-18 20:07:39.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/paths/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/paths/api_metric_alerts_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/paths/api_metric_values_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      184 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/paths/api_metric_values_v1_model_monitoring_id_metric.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      383 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/tag_to_api.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/tags/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      336 2022-10-18 20:07:39.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/tags/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      750 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15937 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/configuration.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4416 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/exceptions.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      360 2022-10-18 20:07:39.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/failure_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/failure_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/metadata_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/metadata_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4856 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_alert_request_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4888 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_tag_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_tag_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4529 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_value_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4561 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_value_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4054 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4118 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     5730 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/new_metric_value_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     5762 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/new_metric_value_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3557 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3589 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4848 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/target_range_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4449 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/model/target_range_v1.pyi
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/models/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1236 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/models/__init__.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      508 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/__init__.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15351 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15120 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15377 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15146 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      405 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    16879 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    16648 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    10493 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/rest.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    96843 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/_impl/custommetrics/schemas.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)       22 2024-01-19 16:22:01.000000 dominodatalab-1.3.0/domino/_version.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/domino/airflow/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      259 2022-06-21 20:35:17.000000 dominodatalab-1.3.0/domino/airflow/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    11462 2023-01-05 19:13:36.000000 dominodatalab-1.3.0/domino/airflow/_operator.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3612 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/authentication.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1513 2023-01-18 14:15:18.000000 dominodatalab-1.3.0/domino/constants.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      723 2022-07-27 14:46:07.000000 dominodatalab-1.3.0/domino/data_sources.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9038 2024-01-19 15:58:01.000000 dominodatalab-1.3.0/domino/datasets.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    54320 2024-01-19 15:58:01.000000 dominodatalab-1.3.0/domino/domino.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1626 2022-07-06 17:07:45.000000 dominodatalab-1.3.0/domino/exceptions.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2426 2022-08-22 21:15:27.000000 dominodatalab-1.3.0/domino/helpers.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2890 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/domino/http_request_manager.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9454 2024-01-19 15:58:01.000000 dominodatalab-1.3.0/domino/routes.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      787 2022-06-21 20:35:17.000000 dominodatalab-1.3.0/domino/training_sets.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/dominodatalab.egg-info/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    23030 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/dominodatalab.egg-info/PKG-INFO
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3540 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/dominodatalab.egg-info/SOURCES.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)        1 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/dominodatalab.egg-info/dependency_links.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      424 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/dominodatalab.egg-info/requires.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)        7 2024-01-19 18:59:39.000000 dominodatalab-1.3.0/dominodatalab.egg-info/top_level.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      882 2024-01-19 18:59:26.000000 dominodatalab-1.3.0/requirements.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)       38 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/setup.cfg
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2184 2024-01-19 15:58:01.000000 dominodatalab-1.3.0/setup.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-01-19 18:59:40.000000 dominodatalab-1.3.0/tests/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9863 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/tests/test_basic_auth.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      675 2022-08-22 21:15:27.000000 dominodatalab-1.3.0/tests/test_data_sources.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     5108 2024-01-19 15:58:01.000000 dominodatalab-1.3.0/tests/test_datasets.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      608 2024-01-19 15:58:01.000000 dominodatalab-1.3.0/tests/test_domino.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2015 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/tests/test_environments.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9105 2022-07-06 17:07:45.000000 dominodatalab-1.3.0/tests/test_jobs.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1969 2022-06-21 20:35:17.000000 dominodatalab-1.3.0/tests/test_models.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      505 2022-08-22 21:15:27.000000 dominodatalab-1.3.0/tests/test_no_data_sources.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2280 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/tests/test_operator.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9614 2023-12-14 22:20:12.000000 dominodatalab-1.3.0/tests/test_projects.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3120 2023-03-20 13:24:47.000000 dominodatalab-1.3.0/tests/test_spark_operator.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:35.022921 dominodatalab-1.3.1/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    11358 2022-06-06 14:00:07.000000 dominodatalab-1.3.1/LICENSE.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)       14 2022-06-21 20:35:17.000000 dominodatalab-1.3.1/MANIFEST.in
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    24348 2024-04-19 13:15:35.021533 dominodatalab-1.3.1/PKG-INFO
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    22833 2024-04-19 12:58:12.000000 dominodatalab-1.3.1/README.md
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.766755 dominodatalab-1.3.1/domino/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      105 2022-06-21 20:35:17.000000 dominodatalab-1.3.1/domino/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9576 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_custom_metrics.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.767623 dominodatalab-1.3.1/domino/_impl/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)        0 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/__init__.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.779576 dominodatalab-1.3.1/domino/_impl/custommetrics/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      821 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    58419 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/api_client.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.857266 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      214 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      972 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/path_to_api.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.863336 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/paths/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      253 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/paths/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/paths/api_metric_alerts_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/paths/api_metric_values_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      184 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/paths/api_metric_values_v1_model_monitoring_id_metric.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      383 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/tag_to_api.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.865630 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/tags/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      336 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/tags/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      750 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15937 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/configuration.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4416 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/exceptions.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.909076 dominodatalab-1.3.1/domino/_impl/custommetrics/model/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      360 2022-10-18 20:07:39.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/failure_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/failure_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metadata_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metadata_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4856 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_alert_request_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4888 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_tag_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_tag_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4529 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_value_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4561 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_value_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4054 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4118 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     5730 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_value_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     5762 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_value_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3557 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3589 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4848 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/target_range_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4449 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/model/target_range_v1.pyi
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.964660 dominodatalab-1.3.1/domino/_impl/custommetrics/models/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1236 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/models/__init__.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.966859 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      508 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/__init__.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.972200 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15351 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15120 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.977750 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15377 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15146 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.996467 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      405 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    16879 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    16648 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    10493 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/rest.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    96843 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/_impl/custommetrics/schemas.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)       22 2024-04-19 12:46:23.000000 dominodatalab-1.3.1/domino/_version.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:34.999103 dominodatalab-1.3.1/domino/airflow/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      259 2022-06-21 20:35:17.000000 dominodatalab-1.3.1/domino/airflow/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    11462 2023-01-05 19:13:36.000000 dominodatalab-1.3.1/domino/airflow/_operator.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3612 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/domino/authentication.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1513 2023-01-18 14:15:18.000000 dominodatalab-1.3.1/domino/constants.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      723 2022-07-27 14:46:07.000000 dominodatalab-1.3.1/domino/data_sources.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9038 2024-01-19 15:58:01.000000 dominodatalab-1.3.1/domino/datasets.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    54359 2024-04-19 12:44:33.000000 dominodatalab-1.3.1/domino/domino.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1626 2022-07-06 17:07:45.000000 dominodatalab-1.3.1/domino/exceptions.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2426 2022-08-22 21:15:27.000000 dominodatalab-1.3.1/domino/helpers.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3408 2024-04-18 11:57:59.000000 dominodatalab-1.3.1/domino/http_request_manager.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9454 2024-01-19 15:58:01.000000 dominodatalab-1.3.1/domino/routes.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      787 2022-06-21 20:35:17.000000 dominodatalab-1.3.1/domino/training_sets.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:35.017349 dominodatalab-1.3.1/dominodatalab.egg-info/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    24348 2024-04-19 13:15:34.000000 dominodatalab-1.3.1/dominodatalab.egg-info/PKG-INFO
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3540 2024-04-19 13:15:34.000000 dominodatalab-1.3.1/dominodatalab.egg-info/SOURCES.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)        1 2024-04-19 13:15:34.000000 dominodatalab-1.3.1/dominodatalab.egg-info/dependency_links.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      424 2024-04-19 13:15:34.000000 dominodatalab-1.3.1/dominodatalab.egg-info/requires.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)        7 2024-04-19 13:15:34.000000 dominodatalab-1.3.1/dominodatalab.egg-info/top_level.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      879 2024-04-19 13:15:10.000000 dominodatalab-1.3.1/requirements.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)       38 2024-04-19 13:15:35.023150 dominodatalab-1.3.1/setup.cfg
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2184 2024-04-18 11:57:59.000000 dominodatalab-1.3.1/setup.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-19 13:15:35.015797 dominodatalab-1.3.1/tests/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9921 2024-04-18 11:57:59.000000 dominodatalab-1.3.1/tests/test_basic_auth.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      675 2022-08-22 21:15:27.000000 dominodatalab-1.3.1/tests/test_data_sources.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     5183 2024-04-19 12:44:33.000000 dominodatalab-1.3.1/tests/test_datasets.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1492 2024-04-18 11:57:59.000000 dominodatalab-1.3.1/tests/test_domino.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2015 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/tests/test_environments.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9142 2024-04-19 12:44:33.000000 dominodatalab-1.3.1/tests/test_jobs.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1969 2022-06-21 20:35:17.000000 dominodatalab-1.3.1/tests/test_models.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      505 2022-08-22 21:15:27.000000 dominodatalab-1.3.1/tests/test_no_data_sources.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2280 2023-03-20 13:24:47.000000 dominodatalab-1.3.1/tests/test_operator.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9614 2023-12-14 22:20:12.000000 dominodatalab-1.3.1/tests/test_projects.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3472 2024-04-19 12:44:33.000000 dominodatalab-1.3.1/tests/test_spark_operator.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dominodatalab-1.3.0/LICENSE.txt` & `dominodatalab-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/PKG-INFO` & `dominodatalab-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,30 @@
-Metadata-Version: 2.1
-Name: dominodatalab
-Version: 1.3.0
-Summary: Python bindings for the Domino API
-Home-page: https://github.com/dominodatalab/python-domino
-Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.3.0.zip
-Author: Domino Data Lab
-Author-email: support@dominodatalab.com
-License: Apache Software License (Apache 2.0)
-Keywords: Domino Data Lab,API
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: airflow
-Provides-Extra: data
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 This library provides bindings for the Domino APIs.  It ships with the Domino Standard Environment (DSE).
 
 See this documentation for details about the APIs:
 
 -   [Latest public Domino
     APIs](https://docs.dominodatalab.com/en/latest/api_guide/8c929e/domino-public-apis/)
 
 -   [Legacy APIs](https://dominodatalab.github.io/api-docs/)
 
-The latest released version of `python-domino` is `1.3.0`.
+The latest released version of `python-domino` is `1.3.1`.
 
 # Version compatibility matrix
 
 The `python-domino` library is compatible with different versions of
 Domino:
 
 | Domino Versions |                                    Python-Domino                                    |
 |-----------------|:-----------------------------------------------------------------------------------:|
 | 3.6.x or lower  |      [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)       |
 | 4.1.0 or higher | [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher |
 | 5.3.0 or higher | [1.2.0]https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
 | 5.5.0 or higher | [1.2.2](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.2.zip) or Higher |
-| 5.10.0 or higher | [1.3.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.0.zip) or Higher |
+| 5.10.0 or higher | [1.3.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.1.zip) or Higher |
 
 # Development
 
 The current `python-domino` is based on Python 3.9, which is therefore recommended for development. `Pipenv` is also recommended to manage the dependencies.
 
 To use the Python binding in a Domino workbook session, include `dominodatalab` in your project's requirements.txt file.
 This makes the Python binding available for each new workbook session (or batch run) started within the project.
@@ -112,20 +95,26 @@
     You can change the log level by setting `DOMINO_LOG_LEVEL`, for example to `DEBUG`.
 
 - `DOMINO_VERIFY_CERTIFICATE`
   
     For testing purposes and issues with SSL certificates, set `DOMINO_VERIFY_CERTIFICATE` to `false`. 
     Be sure to unset this variable when not in use.
 
+- `DOMINO_MAX_RETRIES`
+    
+    Default Retry is set to 4 
+    Determines the number of attempts for the request session in case of a ConnectionError
+    Get more info on request max timeout/error durations based on Retry and backoff factors [here](https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry)
+
 # Methods
 
 ## Projects
 
 See
-[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/example_projects_usage.py)
+[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_projects_usage.py)
 for example code.
 
 ### project_create(project_name, owner_username=None)
 
 Create a new project with given project name.
 
 -   *project_name:* The name of the project.
@@ -153,15 +142,15 @@
 Project tags are an easy way to add freeform metadata to a project. Tags
 help colleagues and consumers organize and find the Domino projects that
 interest them. Tags can be used to describe the subject explored by a
 project, the packages and libraries it uses, or the source of the data
 within.
 
 See
-[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/example_projects_usage.py)
+[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_projects_usage.py)
 for example code.
 
 ### tags_list(\*project_id)
 
 List a project’s tags.
 
 -   *project_id:* The project identifier.
@@ -197,17 +186,17 @@
 
 -   *project_id:* (Defaults to current project id) The project ID.
 
 ## Executions
 
 See these code example files:
 
--   [`start_run_and_check_status.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/start_run_and_check_status.py)
+-   [`start_run_and_check_status.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/start_run_and_check_status.py)
 
--   [`export_runs.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/export_runs.py)
+-   [`export_runs.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/export_runs.py)
 
 ### runs_list()
 
 List the executions on the selected project.
 
 ### runs_start(command, isDirect, commitId, title, tier, publishApiEndpoint)
 
@@ -283,17 +272,17 @@
 
 -   *runId:* string that identifies the execution
 
 ## Files and blobs
 
 See these code example files:
 
--   [`upload_file.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/upload_file.py)
+-   [`upload_file.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/upload_file.py)
 
--   [`upload_and_run_file_and_download_results.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/upload_and_run_file_and_download_results.py)
+-   [`upload_and_run_file_and_download_results.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/upload_and_run_file_and_download_results.py)
 
 ### files_list(commitId, path)
 
 List the files in a folder in the Domino project.
 
 -   *commitId:* The `commitId` to list files from.
 
@@ -442,15 +431,15 @@
 executions as a filesystem directory. A dataset always reflects the most
 recent version of the data. You can modify the contents of a dataset
 through the Domino UI or through workload executions.
 
 See [Domino
 Datasets](https://docs.dominodatalab.com/en/latest/user_guide/0a8d11/datasets-overview/)
 for more details, and
-[`example_dataset.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/example_dataset.py)
+[`example_dataset.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_dataset.py)
 for example code.
 
 ### datasets_list(project_id=None)
 
 Provide a JSON list of all the available datasets.
 
 -   *project_id (string):* (Defaults to None) The project identifier.
```

### Comparing `dominodatalab-1.3.0/README.md` & `dominodatalab-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,70 @@
+Metadata-Version: 2.1
+Name: dominodatalab
+Version: 1.3.1
+Summary: Python bindings for the Domino API
+Home-page: https://github.com/dominodatalab/python-domino
+Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.3.1.zip
+Author: Domino Data Lab
+Author-email: support@dominodatalab.com
+License: Apache Software License (Apache 2.0)
+Keywords: Domino Data Lab,API
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: packaging
+Requires-Dist: requests>=2.4.2
+Requires-Dist: beautifulsoup4~=4.11
+Requires-Dist: polling2~=0.5.0
+Requires-Dist: urllib3~=1.26.12
+Requires-Dist: typing-extensions~=4.4.0
+Requires-Dist: frozendict~=2.3.4
+Requires-Dist: python-dateutil~=2.8.2
+Requires-Dist: retry==0.9.2
+Provides-Extra: airflow
+Requires-Dist: apache-airflow==2.2.4; extra == "airflow"
+Provides-Extra: data
+Requires-Dist: dominodatalab-data>=0.1.0; extra == "data"
+Provides-Extra: dev
+Requires-Dist: black==22.3.0; extra == "dev"
+Requires-Dist: flake8==4.0.1; extra == "dev"
+Requires-Dist: Jinja2==2.11.3; extra == "dev"
+Requires-Dist: nbconvert==6.3.0; extra == "dev"
+Requires-Dist: packaging==21.3; extra == "dev"
+Requires-Dist: polling2==0.5.0; extra == "dev"
+Requires-Dist: pre-commit==2.19.0; extra == "dev"
+Requires-Dist: pyspark==3.3.0; extra == "dev"
+Requires-Dist: pytest==6.2.2; extra == "dev"
+Requires-Dist: requests_mock==1.9.3; extra == "dev"
+Requires-Dist: tox==3.25.1; extra == "dev"
+Requires-Dist: frozendict==2.3.4; extra == "dev"
+
 This library provides bindings for the Domino APIs.  It ships with the Domino Standard Environment (DSE).
 
 See this documentation for details about the APIs:
 
 -   [Latest public Domino
     APIs](https://docs.dominodatalab.com/en/latest/api_guide/8c929e/domino-public-apis/)
 
 -   [Legacy APIs](https://dominodatalab.github.io/api-docs/)
 
-The latest released version of `python-domino` is `1.3.0`.
+The latest released version of `python-domino` is `1.3.1`.
 
 # Version compatibility matrix
 
 The `python-domino` library is compatible with different versions of
 Domino:
 
 | Domino Versions |                                    Python-Domino                                    |
 |-----------------|:-----------------------------------------------------------------------------------:|
 | 3.6.x or lower  |      [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)       |
 | 4.1.0 or higher | [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher |
 | 5.3.0 or higher | [1.2.0]https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
 | 5.5.0 or higher | [1.2.2](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.2.zip) or Higher |
-| 5.10.0 or higher | [1.3.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.0.zip) or Higher |
+| 5.10.0 or higher | [1.3.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.1.zip) or Higher |
 
 # Development
 
 The current `python-domino` is based on Python 3.9, which is therefore recommended for development. `Pipenv` is also recommended to manage the dependencies.
 
 To use the Python binding in a Domino workbook session, include `dominodatalab` in your project's requirements.txt file.
 This makes the Python binding available for each new workbook session (or batch run) started within the project.
@@ -95,20 +135,26 @@
     You can change the log level by setting `DOMINO_LOG_LEVEL`, for example to `DEBUG`.
 
 - `DOMINO_VERIFY_CERTIFICATE`
   
     For testing purposes and issues with SSL certificates, set `DOMINO_VERIFY_CERTIFICATE` to `false`. 
     Be sure to unset this variable when not in use.
 
+- `DOMINO_MAX_RETRIES`
+    
+    Default Retry is set to 4 
+    Determines the number of attempts for the request session in case of a ConnectionError
+    Get more info on request max timeout/error durations based on Retry and backoff factors [here](https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry)
+
 # Methods
 
 ## Projects
 
 See
-[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/example_projects_usage.py)
+[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_projects_usage.py)
 for example code.
 
 ### project_create(project_name, owner_username=None)
 
 Create a new project with given project name.
 
 -   *project_name:* The name of the project.
@@ -136,15 +182,15 @@
 Project tags are an easy way to add freeform metadata to a project. Tags
 help colleagues and consumers organize and find the Domino projects that
 interest them. Tags can be used to describe the subject explored by a
 project, the packages and libraries it uses, or the source of the data
 within.
 
 See
-[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/example_projects_usage.py)
+[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_projects_usage.py)
 for example code.
 
 ### tags_list(\*project_id)
 
 List a project’s tags.
 
 -   *project_id:* The project identifier.
@@ -180,17 +226,17 @@
 
 -   *project_id:* (Defaults to current project id) The project ID.
 
 ## Executions
 
 See these code example files:
 
--   [`start_run_and_check_status.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/start_run_and_check_status.py)
+-   [`start_run_and_check_status.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/start_run_and_check_status.py)
 
--   [`export_runs.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/export_runs.py)
+-   [`export_runs.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/export_runs.py)
 
 ### runs_list()
 
 List the executions on the selected project.
 
 ### runs_start(command, isDirect, commitId, title, tier, publishApiEndpoint)
 
@@ -266,17 +312,17 @@
 
 -   *runId:* string that identifies the execution
 
 ## Files and blobs
 
 See these code example files:
 
--   [`upload_file.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/upload_file.py)
+-   [`upload_file.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/upload_file.py)
 
--   [`upload_and_run_file_and_download_results.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/upload_and_run_file_and_download_results.py)
+-   [`upload_and_run_file_and_download_results.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/upload_and_run_file_and_download_results.py)
 
 ### files_list(commitId, path)
 
 List the files in a folder in the Domino project.
 
 -   *commitId:* The `commitId` to list files from.
 
@@ -425,15 +471,15 @@
 executions as a filesystem directory. A dataset always reflects the most
 recent version of the data. You can modify the contents of a dataset
 through the Domino UI or through workload executions.
 
 See [Domino
 Datasets](https://docs.dominodatalab.com/en/latest/user_guide/0a8d11/datasets-overview/)
 for more details, and
-[`example_dataset.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/example_dataset.py)
+[`example_dataset.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_dataset.py)
 for example code.
 
 ### datasets_list(project_id=None)
 
 Provide a JSON list of all the available datasets.
 
 -   *project_id (string):* (Defaults to None) The project identifier.
```

### Comparing `dominodatalab-1.3.0/domino/_custom_metrics.py` & `dominodatalab-1.3.1/domino/_custom_metrics.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/__init__.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/api_client.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/api_client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/apis/path_to_api.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/configuration.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/configuration.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/exceptions.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/failure_envelope_v1.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/failure_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/failure_envelope_v1.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/failure_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/metadata_v1.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metadata_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/metadata_v1.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metadata_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_alert_request_v1.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_alert_request_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_tag_v1.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_tag_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_tag_v1.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_tag_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_value_v1.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_value_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_value_v1.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_value_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/new_metric_value_v1.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_value_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/new_metric_value_v1.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_value_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/target_range_v1.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/target_range_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/model/target_range_v1.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/model/target_range_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/models/__init__.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi` & `dominodatalab-1.3.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/rest.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/rest.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/_impl/custommetrics/schemas.py` & `dominodatalab-1.3.1/domino/_impl/custommetrics/schemas.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/airflow/_operator.py` & `dominodatalab-1.3.1/domino/airflow/_operator.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/authentication.py` & `dominodatalab-1.3.1/domino/authentication.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/constants.py` & `dominodatalab-1.3.1/domino/constants.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/data_sources.py` & `dominodatalab-1.3.1/domino/data_sources.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/datasets.py` & `dominodatalab-1.3.1/domino/datasets.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/domino.py` & `dominodatalab-1.3.1/domino/domino.py`

 * *Files 1% similar despite different names*

```diff
@@ -1171,15 +1171,15 @@
         return self._get(url)
 
     # Hardware Tier Functions
     def hardware_tiers_list(self):
         url = self._routes.hardware_tiers_list(self.project_id)
         return self._get(url)
 
-    def get_hardware_tier_id_from_name(self, hardware_tier_name):
+    def get_hardware_tier_id_from_name(self, hardware_tier_name: str):
         for hardware_tier in self.hardware_tiers_list():
             if hardware_tier_name == hardware_tier["hardwareTier"]["name"]:
                 return hardware_tier["hardwareTier"]["id"]
         return None
 
     def process_log(self, log):
         """
@@ -1212,33 +1212,33 @@
         useable_environment_list_url = self._routes.useable_environments_list(
             self.project_id
         )
         return self.request_manager.get(useable_environment_list_url).json()[
             "environments"
         ]
 
-    def _validate_environment_id(self, environment_id):
+    def _validate_environment_id(self, environment_id) -> bool:
         self.log.debug(f"Validating environment id: {environment_id}")
         for environment in self._useable_environments_list():
             if environment_id == environment["id"]:
                 return True
         raise exceptions.EnvironmentNotFoundException(
             f"{environment_id} environment not found"
         )
 
-    def _validate_hardware_tier_id(self, hardware_tier_id):
+    def _validate_hardware_tier_id(self, hardware_tier_id: str) -> bool:
         self.log.debug(f"Validating hardware tier id: {hardware_tier_id}")
         for hardware_tier in self.hardware_tiers_list():
             if hardware_tier_id == hardware_tier["hardwareTier"]["id"]:
                 return True
         raise exceptions.HardwareTierNotFoundException(
             f"{hardware_tier_id} hardware tier Id not found"
         )
 
-    def _validate_hardware_tier_name(self, hardware_tier_name):
+    def _validate_hardware_tier_name(self, hardware_tier_name: str) -> bool:
         self.log.debug(f"Validating hardware tier name: {hardware_tier_name}")
         count = 0
         for hardware_tier in self.hardware_tiers_list():
             if hardware_tier_name == hardware_tier["hardwareTier"]["name"]:
                 count += 1
 
         if count == 0:
```

### Comparing `dominodatalab-1.3.0/domino/exceptions.py` & `dominodatalab-1.3.1/domino/exceptions.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/helpers.py` & `dominodatalab-1.3.1/domino/helpers.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/http_request_manager.py` & `dominodatalab-1.3.1/domino/http_request_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 import logging
 import os
 from http import HTTPStatus
 
 import requests
 from bs4 import BeautifulSoup
+from requests.adapters import HTTPAdapter, Retry
 from requests.auth import AuthBase
 
 from ._version import __version__
 from .constants import DOMINO_VERIFY_CERTIFICATE
 from .exceptions import ReloginRequiredException
 
+
+R_SESSION_MAX_RETRIES = 4
+
 class _SessionInitializer:
     def __initialize__(self, session):
         raise NotImplementedError('Session initializers must be callable.')
 
 class _HttpRequestManager:
     """
     This class is responsible for
     making Http request calls
     """
 
     def __init__(self, auth: AuthBase):
         self.auth = auth
         self._logger = logging.getLogger(__name__)
-        self.request_session = requests.Session()
-        self.request_session.headers["User-Agent"] = f"python-domino/{__version__}"
+        self.request_session = self._set_session()
 
         if isinstance(self.auth, _SessionInitializer):
-            self.auth.__initialize__(self.request_session)
+            self.auth.__initialize__(self._set_session())
+
+    def _set_session(self):
+        """
+        Initialize a request session with retry to help manage connections drop.
+        """
+        self.session = requests.Session()
+        retries = Retry(
+            total=int(os.getenv("DOMINO_MAX_RETRIES", str(R_SESSION_MAX_RETRIES))),
+            backoff_factor=1,  # retry seconds
+            status_forcelist=[408, 502, 503, 504],
+        )
 
         if os.environ.get(DOMINO_VERIFY_CERTIFICATE, None) in ["false", "f", "n", "no"]:
             warning = "InsecureRequestWarning: Bypassing certificate verification is strongly ill-advised"
             logging.warning(warning)
             print(warning)
-            self.request_session.verify = False
+            self.session.verify = False
+
+        retry_adapter = HTTPAdapter(max_retries=retries)
+        self.session.mount("https://", retry_adapter)
+        return self.session
 
     def post(self, url, data=None, json=None, **kwargs):
         return self._raise_for_status(
             self.request_session.post(
                 url, auth=self.auth, data=data, json=json, **kwargs
             )
         )
```

### Comparing `dominodatalab-1.3.0/domino/routes.py` & `dominodatalab-1.3.1/domino/routes.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/domino/training_sets.py` & `dominodatalab-1.3.1/domino/training_sets.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/dominodatalab.egg-info/PKG-INFO` & `dominodatalab-1.3.1/dominodatalab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,70 @@
 Metadata-Version: 2.1
 Name: dominodatalab
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python bindings for the Domino API
 Home-page: https://github.com/dominodatalab/python-domino
-Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.3.0.zip
+Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.3.1.zip
 Author: Domino Data Lab
 Author-email: support@dominodatalab.com
 License: Apache Software License (Apache 2.0)
 Keywords: Domino Data Lab,API
-Requires-Python: >=3.7.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: packaging
+Requires-Dist: requests>=2.4.2
+Requires-Dist: beautifulsoup4~=4.11
+Requires-Dist: polling2~=0.5.0
+Requires-Dist: urllib3~=1.26.12
+Requires-Dist: typing-extensions~=4.4.0
+Requires-Dist: frozendict~=2.3.4
+Requires-Dist: python-dateutil~=2.8.2
+Requires-Dist: retry==0.9.2
 Provides-Extra: airflow
+Requires-Dist: apache-airflow==2.2.4; extra == "airflow"
 Provides-Extra: data
+Requires-Dist: dominodatalab-data>=0.1.0; extra == "data"
 Provides-Extra: dev
-License-File: LICENSE.txt
+Requires-Dist: black==22.3.0; extra == "dev"
+Requires-Dist: flake8==4.0.1; extra == "dev"
+Requires-Dist: Jinja2==2.11.3; extra == "dev"
+Requires-Dist: nbconvert==6.3.0; extra == "dev"
+Requires-Dist: packaging==21.3; extra == "dev"
+Requires-Dist: polling2==0.5.0; extra == "dev"
+Requires-Dist: pre-commit==2.19.0; extra == "dev"
+Requires-Dist: pyspark==3.3.0; extra == "dev"
+Requires-Dist: pytest==6.2.2; extra == "dev"
+Requires-Dist: requests_mock==1.9.3; extra == "dev"
+Requires-Dist: tox==3.25.1; extra == "dev"
+Requires-Dist: frozendict==2.3.4; extra == "dev"
 
 This library provides bindings for the Domino APIs.  It ships with the Domino Standard Environment (DSE).
 
 See this documentation for details about the APIs:
 
 -   [Latest public Domino
     APIs](https://docs.dominodatalab.com/en/latest/api_guide/8c929e/domino-public-apis/)
 
 -   [Legacy APIs](https://dominodatalab.github.io/api-docs/)
 
-The latest released version of `python-domino` is `1.3.0`.
+The latest released version of `python-domino` is `1.3.1`.
 
 # Version compatibility matrix
 
 The `python-domino` library is compatible with different versions of
 Domino:
 
 | Domino Versions |                                    Python-Domino                                    |
 |-----------------|:-----------------------------------------------------------------------------------:|
 | 3.6.x or lower  |      [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)       |
 | 4.1.0 or higher | [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher |
 | 5.3.0 or higher | [1.2.0]https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
 | 5.5.0 or higher | [1.2.2](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.2.zip) or Higher |
-| 5.10.0 or higher | [1.3.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.0.zip) or Higher |
+| 5.10.0 or higher | [1.3.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.1.zip) or Higher |
 
 # Development
 
 The current `python-domino` is based on Python 3.9, which is therefore recommended for development. `Pipenv` is also recommended to manage the dependencies.
 
 To use the Python binding in a Domino workbook session, include `dominodatalab` in your project's requirements.txt file.
 This makes the Python binding available for each new workbook session (or batch run) started within the project.
@@ -112,20 +135,26 @@
     You can change the log level by setting `DOMINO_LOG_LEVEL`, for example to `DEBUG`.
 
 - `DOMINO_VERIFY_CERTIFICATE`
   
     For testing purposes and issues with SSL certificates, set `DOMINO_VERIFY_CERTIFICATE` to `false`. 
     Be sure to unset this variable when not in use.
 
+- `DOMINO_MAX_RETRIES`
+    
+    Default Retry is set to 4 
+    Determines the number of attempts for the request session in case of a ConnectionError
+    Get more info on request max timeout/error durations based on Retry and backoff factors [here](https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry)
+
 # Methods
 
 ## Projects
 
 See
-[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/example_projects_usage.py)
+[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_projects_usage.py)
 for example code.
 
 ### project_create(project_name, owner_username=None)
 
 Create a new project with given project name.
 
 -   *project_name:* The name of the project.
@@ -153,15 +182,15 @@
 Project tags are an easy way to add freeform metadata to a project. Tags
 help colleagues and consumers organize and find the Domino projects that
 interest them. Tags can be used to describe the subject explored by a
 project, the packages and libraries it uses, or the source of the data
 within.
 
 See
-[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/example_projects_usage.py)
+[`example_projects_usage.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_projects_usage.py)
 for example code.
 
 ### tags_list(\*project_id)
 
 List a project’s tags.
 
 -   *project_id:* The project identifier.
@@ -197,17 +226,17 @@
 
 -   *project_id:* (Defaults to current project id) The project ID.
 
 ## Executions
 
 See these code example files:
 
--   [`start_run_and_check_status.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/start_run_and_check_status.py)
+-   [`start_run_and_check_status.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/start_run_and_check_status.py)
 
--   [`export_runs.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/export_runs.py)
+-   [`export_runs.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/export_runs.py)
 
 ### runs_list()
 
 List the executions on the selected project.
 
 ### runs_start(command, isDirect, commitId, title, tier, publishApiEndpoint)
 
@@ -283,17 +312,17 @@
 
 -   *runId:* string that identifies the execution
 
 ## Files and blobs
 
 See these code example files:
 
--   [`upload_file.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/upload_file.py)
+-   [`upload_file.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/upload_file.py)
 
--   [`upload_and_run_file_and_download_results.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/upload_and_run_file_and_download_results.py)
+-   [`upload_and_run_file_and_download_results.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/upload_and_run_file_and_download_results.py)
 
 ### files_list(commitId, path)
 
 List the files in a folder in the Domino project.
 
 -   *commitId:* The `commitId` to list files from.
 
@@ -442,15 +471,15 @@
 executions as a filesystem directory. A dataset always reflects the most
 recent version of the data. You can modify the contents of a dataset
 through the Domino UI or through workload executions.
 
 See [Domino
 Datasets](https://docs.dominodatalab.com/en/latest/user_guide/0a8d11/datasets-overview/)
 for more details, and
-[`example_dataset.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.0/examples/example_dataset.py)
+[`example_dataset.py`](https://github.com/dominodatalab/python-domino/blob/release-1.3.1/examples/example_dataset.py)
 for example code.
 
 ### datasets_list(project_id=None)
 
 Provide a JSON list of all the available datasets.
 
 -   *project_id (string):* (Defaults to None) The project identifier.
```

### Comparing `dominodatalab-1.3.0/dominodatalab.egg-info/SOURCES.txt` & `dominodatalab-1.3.1/dominodatalab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/requirements.txt` & `dominodatalab-1.3.1/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile setup.py
 #
 beautifulsoup4==4.12.3
     # via dominodatalab (setup.py)
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 decorator==5.1.1
     # via retry
 frozendict==2.3.10
     # via dominodatalab (setup.py)
-idna==3.6
+idna==3.7
     # via requests
-packaging==23.2
+packaging==24.0
     # via dominodatalab (setup.py)
 polling2==0.5.0
     # via dominodatalab (setup.py)
 py==1.11.0
     # via retry
 python-dateutil==2.8.2
     # via dominodatalab (setup.py)
 requests==2.31.0
     # via dominodatalab (setup.py)
 retry==0.9.2
     # via dominodatalab (setup.py)
 six==1.16.0
     # via python-dateutil
-soupsieve==2.4.1
+soupsieve==2.5
     # via beautifulsoup4
 typing-extensions==4.4.0
     # via dominodatalab (setup.py)
 urllib3==1.26.18
     # via
     #   dominodatalab (setup.py)
     #   requests
```

### Comparing `dominodatalab-1.3.0/setup.py` & `dominodatalab-1.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     url="https://github.com/dominodatalab/python-domino",
     download_url=f"https://github.com/dominodatalab/python-domino/archive/release-{get_version()}.zip",
     license="Apache Software License (Apache 2.0)",
     description="Python bindings for the Domino API",
     long_description=README,
     long_description_content_type="text/markdown",
     keywords=["Domino Data Lab", "API"],
-    python_requires='>=3.7.0',
+    python_requires='>=3.9.0',
     install_requires=["packaging", "requests>=2.4.2", "beautifulsoup4~=4.11", "polling2~=0.5.0",
                       "urllib3~=1.26.12", "typing-extensions~=4.4.0", "frozendict~=2.3.4", "python-dateutil~=2.8.2",
                       "retry==0.9.2"],
     extras_require={
         "airflow": ["apache-airflow==2.2.4"],
         "data": ["dominodatalab-data>=0.1.0"],
         "dev": [
```

### Comparing `dominodatalab-1.3.0/tests/test_basic_auth.py` & `dominodatalab-1.3.1/tests/test_basic_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,20 @@
     Confirm that trying to instantiate a Domino object with an invalid token file
     raises a FileNotFoundError exception.
     """
     dummy_host = "http://domino.somefakecompany.com"
     invalid_file = "non_existent_token_file.txt"
 
     with pytest.raises(FileNotFoundError):
-        Domino(
+        test_domino = Domino(
             host=dummy_host,
             project="anyuser/quick-start",
             domino_token_file=invalid_file,
         )
+        test_domino.runs_list()["data"]
 
 
 def test_malformed_project_input_error(caplog):
     """
     Confirm that passing in a project name without the user name raises a ValueError.
     """
     # This test uses the provided pytest fixture, caplog. For more info, see:
@@ -93,29 +94,29 @@
 def test_object_creation_with_api_proxy():
     """
     Confirm that the expected auth type is used when using api proxy.
     """
     dummy_host = "http://domino.somefakecompany.com"
     dummy_api_proxy = "localhost:1234"
 
-    d = Domino(host=dummy_host, project="anyuser/quick-start", api_key=dummy_api_proxy)
+    d = Domino(host=dummy_host, project="anyuser/quick-start", api_proxy=dummy_api_proxy)
     assert isinstance(
         d.request_manager.auth, domino.authentication.ProxyAuth
     ), "Authentication using API proxy should be of type domino.authentication.ProxyAuth"
     assert d.request_manager.auth.api_proxy == "http://localhost:1234"
 
 @pytest.mark.usefixtures("mock_domino_version_response", "clear_token_file_from_env")
 def test_object_creation_with_api_proxy_with_scheme():
     """
     Confirm that the expected auth type is used when using api proxy.
     """
     dummy_host = "http://domino.somefakecompany.com"
     dummy_api_proxy = "https://localhost:1234"
 
-    d = Domino(host=dummy_host, project="anyuser/quick-start", api_key=dummy_api_proxy)
+    d = Domino(host=dummy_host, project="anyuser/quick-start", api_proxy=dummy_api_proxy)
     assert isinstance(
         d.request_manager.auth, domino.authentication.ProxyAuth
     ), "Authentication using API proxy should be of type domino.authentication.ProxyAuth"
     assert d.request_manager.auth.api_proxy == "https://localhost:1234"
 
 
 @pytest.mark.usefixtures("mock_domino_version_response")
```

### Comparing `dominodatalab-1.3.0/tests/test_data_sources.py` & `dominodatalab-1.3.1/tests/test_data_sources.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/tests/test_datasets.py` & `dominodatalab-1.3.1/tests/test_datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import random
 
 import pytest
 
 from domino.helpers import domino_is_reachable
 
 
@@ -94,30 +95,31 @@
 
 
 @pytest.mark.skipif(
     not domino_is_reachable(), reason="No access to a live Domino deployment"
 )
 def test_datasets_upload(default_domino_client):
     datasets_id = default_domino_client.datasets_ids(default_domino_client.project_id)[
-        1
+        0
     ]
-    local_path_to_file = "test_datasets.py"
+    local_path_to_file = "tests/test_datasets.py"
     response = default_domino_client.datasets_upload_files(datasets_id, local_path_to_file)
 
     assert "test_datasets.py" in response
 
 
 @pytest.mark.skipif(
     not domino_is_reachable(), reason="No access to a live Domino deployment"
 )
 def test_datasets_upload_with_sub_dir(default_domino_client):
     datasets_id = default_domino_client.datasets_ids(default_domino_client.project_id)[
-        1
+        0
     ]
-    local_path_to_file = "test_datasets.py"
+    assert "test_datasets.py" in os.listdir("tests")
+    local_path_to_file = "tests/test_datasets.py"
     response = default_domino_client.datasets_upload_files(datasets_id, local_path_to_file,
                                                            target_relative_path="sub_d")
 
     assert "test_datasets.py" in response
 
 
 @pytest.mark.skipif(
```

### Comparing `dominodatalab-1.3.0/tests/test_environments.py` & `dominodatalab-1.3.1/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/tests/test_jobs.py` & `dominodatalab-1.3.1/tests/test_jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,51 +116,52 @@
 )
 def test_job_start_override_hardware_tier_id(default_domino_client):
     """
     Confirm that we can start a job using the v4 API and override the hardware tier id
     """
     hardware_tiers = default_domino_client.hardware_tiers_list()
     non_default_hardware_tiers = [
-        hwt for hwt in hardware_tiers if not hwt["hardwareTier"]["isDefault"]
+        hwt for hwt in hardware_tiers if not hwt["hardwareTier"]["hwtFlags"]["isDefault"]
     ]
     if len(non_default_hardware_tiers) == 0:
         pytest.xfail("No non-default hardware tiers found: cannot run test")
 
     override_hardware_tier_id = non_default_hardware_tiers[0]["hardwareTier"]["id"]
     job_status = default_domino_client.job_start_blocking(
         command="main.py", hardware_tier_id=override_hardware_tier_id
     )
     assert job_status["statuses"]["isCompleted"] is True
     job_red = default_domino_client.job_runtime_execution_details(job_status["id"])
-    assert job_red["hardwareTierId"] == override_hardware_tier_id
+    assert job_red["hardwareTier"]["id"] == override_hardware_tier_id
 
 
 # deprecated but ensuring it still works for now
 @pytest.mark.skipif(
     not domino_is_reachable(), reason="No access to a live Domino deployment"
 )
 def test_job_start_override_hardware_tier_name(default_domino_client):
     """
     Confirm that we can start a job using the v4 API and override the hardware tier via hardware_tier_name
     """
     hardware_tiers = default_domino_client.hardware_tiers_list()
+
     non_default_hardware_tiers = [
-        hwt for hwt in hardware_tiers if not hwt["hardwareTier"]["isDefault"]
+        hwt for hwt in hardware_tiers if not hwt["hardwareTier"]["hwtFlags"]["isDefault"]
     ]
     if len(non_default_hardware_tiers) == 0:
         pytest.xfail("No non-default hardware tiers found: cannot run test")
 
     override_hardware_tier_name = non_default_hardware_tiers[0]["hardwareTier"]["name"]
     job_status = default_domino_client.job_start_blocking(
         command="main.py", hardware_tier_name=override_hardware_tier_name
     )
 
     assert job_status["statuses"]["isCompleted"] is True
     job_red = default_domino_client.job_runtime_execution_details(job_status["id"])
-    assert job_red["hardwareTier"] == override_hardware_tier_name
+    assert job_red["hardwareTier"]["name"] == override_hardware_tier_name
 
 
 @pytest.mark.skipif(
     not domino_is_reachable(), reason="No access to a live Domino deployment"
 )
 def test_runs_list(default_domino_client):
     """
```

### Comparing `dominodatalab-1.3.0/tests/test_models.py` & `dominodatalab-1.3.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/tests/test_operator.py` & `dominodatalab-1.3.1/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/tests/test_projects.py` & `dominodatalab-1.3.1/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.3.0/tests/test_spark_operator.py` & `dominodatalab-1.3.1/tests/test_spark_operator.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from domino.airflow import DominoSparkOperator
 from domino.exceptions import RunFailedException
 from domino.helpers import domino_is_reachable
 
 TEST_PROJECT = os.environ.get("DOMINO_SPARK_TEST_PROJECT")
 dag_id = "test_spark_operator"
 
-
+@pytest.mark.skipif(os.getenv("SPARK_DEP") != "yes", reason="Extra dependency required")
 @pytest.mark.skipif(
     not domino_is_reachable(), reason="No access to a live Domino deployment"
 )
 def test_spark_operator_no_cluster():
     execution_dt = datetime.now()
 
     dag = DAG(dag_id, start_date=execution_dt)
@@ -32,15 +32,15 @@
         project=TEST_PROJECT,
         command="test_spark.py",
     )
     task.run()
     ti = TaskInstance(task=task, execution_date=execution_dt)
     task.execute(ti.get_template_context())
 
-
+@pytest.mark.skipif(os.getenv("SPARK_DEP") != "yes", reason="Extra dependency required")
 @pytest.mark.skipif(
     not domino_is_reachable(), reason="No access to a live Domino deployment"
 )
 def test_spark_operator_with_cluster(spark_cluster_env_id):
 
     execution_dt = datetime.now()
     dag = DAG(dag_id, start_date=execution_dt)
@@ -54,15 +54,15 @@
             "executorCount": 3,
         },
     )
     task.run()
     ti = TaskInstance(task=task, execution_date=execution_dt)
     task.execute(ti.get_template_context())
 
-
+@pytest.mark.skipif(os.getenv("SPARK_DEP") != "yes", reason="Extra dependency required")
 @pytest.mark.skipif(
     not domino_is_reachable(), reason="No access to a live Domino deployment"
 )
 def test_spark_operator_with_compute_cluster_properties(spark_cluster_env_id):
     execution_dt = datetime.now()
 
     dag = DAG(dag_id, start_date=execution_dt)
@@ -79,15 +79,15 @@
             "workerCount": 3,
         },
     )
     task.run()
     ti = TaskInstance(task=task, execution_date=execution_dt)
     task.execute(ti.get_template_context())
 
-
+@pytest.mark.skipif(os.getenv("SPARK_DEP") != "yes", reason="Extra dependency required")
 @pytest.mark.skipif(
     not domino_is_reachable(), reason="No access to a live Domino deployment"
 )
 def test_spark_operator_no_cluster_failed():
     execution_dt = datetime.now()
 
     dag = DAG(dag_id, start_date=execution_dt)
```

