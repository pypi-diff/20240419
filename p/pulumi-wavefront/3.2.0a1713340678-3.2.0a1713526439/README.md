# Comparing `tmp/pulumi_wavefront-3.2.0a1713340678.tar.gz` & `tmp/pulumi_wavefront-3.2.0a1713526439.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_wavefront-3.2.0a1713340678.tar", last modified: Wed Apr 17 08:27:55 2024, max compression
+gzip compressed data, was "pulumi_wavefront-3.2.0a1713526439.tar", last modified: Fri Apr 19 11:36:34 2024, max compression
```

## Comparing `pulumi_wavefront-3.2.0a1713340678.tar` & `pulumi_wavefront-3.2.0a1713526439.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:27:55.211811 pulumi_wavefront-3.2.0a1713340678/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-17 08:27:55.211811 pulumi_wavefront-3.2.0a1713340678/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:27:55.211811 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    81066 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    55354 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    33307 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/alert_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    46961 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_app_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_aws_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    30771 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    26210 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_azure_activity_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    28989 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_cloud_trail.py
--rw-r--r--   0 runner    (1001) docker     (127)    36755 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_cloud_watch.py
--rw-r--r--   0 runner    (1001) docker     (127)    24249 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29433 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    23850 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_gcp_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)    26370 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_new_relic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:27:55.211811 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    31524 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    17455 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/dashboard_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    25134 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/external_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    17832 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)    19926 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_default_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_derived_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_external_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_maintenance_window_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/ingestion_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    34638 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)   217889 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    14549 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:27:55.211811 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-17 08:27:55.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-17 08:27:55.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:27:55.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 08:27:55.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 08:27:55.000000 pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-17 08:27:47.000000 pulumi_wavefront-3.2.0a1713340678/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:27:55.211811 pulumi_wavefront-3.2.0a1713340678/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81066 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55416 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33393 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/alert_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47037 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_app_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_aws_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30849 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26288 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_azure_activity_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29065 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_cloud_trail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36831 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_cloud_watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24325 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23892 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_gcp_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_new_relic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31524 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/dashboard_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15267 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25202 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/external_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17918 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20016 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_default_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16099 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_derived_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_external_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14128 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_maintenance_window_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/ingestion_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34638 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13179 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   217889 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14177 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14549 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-19 11:36:34.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-19 11:36:34.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:36:34.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 11:36:34.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 11:36:34.000000 pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 11:36:27.000000 pulumi_wavefront-3.2.0a1713526439/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:36:34.247644 pulumi_wavefront-3.2.0a1713526439/setup.cfg
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/PKG-INFO` & `pulumi_wavefront-3.2.0a1713526439/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_wavefront
-Version: 3.2.0a1713340678
+Version: 3.2.0a1713526439
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi,wavefront
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/README.md` & `pulumi_wavefront-3.2.0a1713526439/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/__init__.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/_inputs.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/_utilities.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/alert.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,24 +686,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         foobar = wavefront.Alert("foobar",
+            name="Test Alert",
+            target="test@example.com,target:alert-target-id",
             condition="100-ts(\\"cpu.usage_idle\\", environment=preprod and cpu=cpu-total ) > 80",
             display_expression="100-ts(\\"cpu.usage_idle\\", environment=preprod and cpu=cpu-total )",
             minutes=5,
             resolve_after_minutes=5,
             severity="WARN",
             tags=[
                 "terraform",
                 "test",
-            ],
-            target="test@example.com,target:alert-target-id")
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Alerts can be imported using the `id`, e.g.
 
@@ -758,24 +759,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         foobar = wavefront.Alert("foobar",
+            name="Test Alert",
+            target="test@example.com,target:alert-target-id",
             condition="100-ts(\\"cpu.usage_idle\\", environment=preprod and cpu=cpu-total ) > 80",
             display_expression="100-ts(\\"cpu.usage_idle\\", environment=preprod and cpu=cpu-total )",
             minutes=5,
             resolve_after_minutes=5,
             severity="WARN",
             tags=[
                 "terraform",
                 "test",
-            ],
-            target="test@example.com,target:alert-target-id")
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Alerts can be imported using the `id`, e.g.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/alert_target.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/alert_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,22 +428,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        test_target = wavefront.AlertTarget("testTarget",
+        test_target = wavefront.AlertTarget("test_target",
+            name="Terraform Test Target",
+            description="Test target",
+            method="WEBHOOK",
+            recipient="https://hooks.slack.com/services/test/me",
             content_type="application/json",
             custom_headers={
                 "Testing": "true",
             },
-            description="Test target",
-            method="WEBHOOK",
-            recipient="https://hooks.slack.com/services/test/me",
             template="{}",
             triggers=[
                 "ALERT_OPENED",
                 "ALERT_RESOLVED",
             ])
         ```
         <!--End PulumiCodeChooser -->
@@ -485,22 +486,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        test_target = wavefront.AlertTarget("testTarget",
+        test_target = wavefront.AlertTarget("test_target",
+            name="Terraform Test Target",
+            description="Test target",
+            method="WEBHOOK",
+            recipient="https://hooks.slack.com/services/test/me",
             content_type="application/json",
             custom_headers={
                 "Testing": "true",
             },
-            description="Test target",
-            method="WEBHOOK",
-            recipient="https://hooks.slack.com/services/test/me",
             template="{}",
             triggers=[
                 "ALERT_OPENED",
                 "ALERT_RESOLVED",
             ])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_app_dynamics.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_app_dynamics.py`

 * *Files 1% similar despite different names*

```diff
@@ -605,18 +605,19 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        app_dynamics = wavefront.CloudIntegrationAppDynamics("appDynamics",
+        app_dynamics = wavefront.CloudIntegrationAppDynamics("app_dynamics",
+            name="Test Integration",
+            user_name="example",
             controller_name="exampleController",
-            encrypted_password="encryptedPassword",
-            user_name="example")
+            encrypted_password="encryptedPassword")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         AppDynamic Cloud Integrations can be imported by using the `id`, e.g.:
 
@@ -659,18 +660,19 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        app_dynamics = wavefront.CloudIntegrationAppDynamics("appDynamics",
+        app_dynamics = wavefront.CloudIntegrationAppDynamics("app_dynamics",
+            name="Test Integration",
+            user_name="example",
             controller_name="exampleController",
-            encrypted_password="encryptedPassword",
-            user_name="example")
+            encrypted_password="encryptedPassword")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         AppDynamic Cloud Integrations can be imported by using the `id`, e.g.:
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_aws_external_id.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_aws_external_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        external_id = wavefront.CloudIntegrationAwsExternalId("externalId")
+        external_id = wavefront.CloudIntegrationAwsExternalId("external_id")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         External IDs can be imported by using the `id`, e.g.:
 
@@ -63,15 +63,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        external_id = wavefront.CloudIntegrationAwsExternalId("externalId")
+        external_id = wavefront.CloudIntegrationAwsExternalId("external_id")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         External IDs can be imported by using the `id`, e.g.:
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_azure.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_azure.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,16 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azureActivityLog",
+        azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azure_activity_log",
+            name="Test Integration",
             client_id="client-id2",
             client_secret="client-secret2",
             tenant="my-tenant2")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -445,15 +446,16 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azureActivityLog",
+        azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azure_activity_log",
+            name="Test Integration",
             client_id="client-id2",
             client_secret="client-secret2",
             tenant="my-tenant2")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_azure_activity_log.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_azure_activity_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,15 +333,16 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azureActivityLog",
+        azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azure_activity_log",
+            name="Test Integration",
             category_filters=["ADMINISTRATIVE"],
             client_id="client-id2",
             client_secret="client-secret2",
             tenant="my-tenant2")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -378,15 +379,16 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azureActivityLog",
+        azure_activity_log = wavefront.CloudIntegrationAzureActivityLog("azure_activity_log",
+            name="Test Integration",
             category_filters=["ADMINISTRATIVE"],
             client_id="client-id2",
             client_secret="client-secret2",
             tenant="my-tenant2")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_cloud_trail.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_cloud_trail.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,16 +398,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        ext_id = wavefront.CloudIntegrationAwsExternalId("extId")
+        ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         cloudtrail = wavefront.CloudIntegrationCloudTrail("cloudtrail",
+            name="Test Integration",
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id,
             region="us-west-2",
             bucket_name="example-s3-bucket")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -446,16 +447,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        ext_id = wavefront.CloudIntegrationAwsExternalId("extId")
+        ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         cloudtrail = wavefront.CloudIntegrationCloudTrail("cloudtrail",
+            name="Test Integration",
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id,
             region="us-west-2",
             bucket_name="example-s3-bucket")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_cloud_watch.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_cloud_watch.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,16 +453,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        ext_id = wavefront.CloudIntegrationAwsExternalId("extId")
+        ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         cloudwatch = wavefront.CloudIntegrationCloudWatch("cloudwatch",
+            name="Test Integration",
             force_save=True,
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -506,16 +507,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        ext_id = wavefront.CloudIntegrationAwsExternalId("extId")
+        ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         cloudwatch = wavefront.CloudIntegrationCloudWatch("cloudwatch",
+            name="Test Integration",
             force_save=True,
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_ec2.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,16 +309,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        ext_id = wavefront.CloudIntegrationAwsExternalId("extId")
+        ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         ec2 = wavefront.CloudIntegrationEc2("ec2",
+            name="Test Integration",
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -354,16 +355,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        ext_id = wavefront.CloudIntegrationAwsExternalId("extId")
+        ext_id = wavefront.CloudIntegrationAwsExternalId("ext_id")
         ec2 = wavefront.CloudIntegrationEc2("ec2",
+            name="Test Integration",
             role_arn="arn:aws::1234567:role/example-arn",
             external_id=ext_id.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_gcp.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,18 +355,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         gcp = wavefront.CloudIntegrationGcp("gcp",
-            json_key=\"\"\"{...your gcp key ...}
-
-        \"\"\",
-            project_id="example-gcp-project")
+            name="Test Integration",
+            project_id="example-gcp-project",
+            json_key="{...your gcp key ...}\\n")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         GCP Cloud Integrations can be imported by using the `id`, e.g.:
 
@@ -405,18 +404,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         gcp = wavefront.CloudIntegrationGcp("gcp",
-            json_key=\"\"\"{...your gcp key ...}
-
-        \"\"\",
-            project_id="example-gcp-project")
+            name="Test Integration",
+            project_id="example-gcp-project",
+            json_key="{...your gcp key ...}\\n")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         GCP Cloud Integrations can be imported by using the `id`, e.g.:
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_gcp_billing.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_gcp_billing.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,20 +304,19 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        gcp_billing = wavefront.CloudIntegrationGcpBilling("gcpBilling",
+        gcp_billing = wavefront.CloudIntegrationGcpBilling("gcp_billing",
+            name="Test Integration",
+            project_id="example-gcp-project",
             api_key="example-api-key",
-            json_key=\"\"\"{...your gcp key ...}
-
-        \"\"\",
-            project_id="example-gcp-project")
+            json_key="{...your gcp key ...}\\n")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         GCP Billing Cloud Integrations can be imported by using the `id`, e.g.:
 
@@ -350,20 +349,19 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        gcp_billing = wavefront.CloudIntegrationGcpBilling("gcpBilling",
+        gcp_billing = wavefront.CloudIntegrationGcpBilling("gcp_billing",
+            name="Test Integration",
+            project_id="example-gcp-project",
             api_key="example-api-key",
-            json_key=\"\"\"{...your gcp key ...}
-
-        \"\"\",
-            project_id="example-gcp-project")
+            json_key="{...your gcp key ...}\\n")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         GCP Billing Cloud Integrations can be imported by using the `id`, e.g.:
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/cloud_integration_new_relic.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/cloud_integration_new_relic.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        newrelic = wavefront.CloudIntegrationNewRelic("newrelic", api_key="example-api-key")
+        newrelic = wavefront.CloudIntegrationNewRelic("newrelic",
+            name="Test Integration",
+            api_key="example-api-key")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         NewRelic Integrations can be imported by using the `id`, e.g.:
 
@@ -378,15 +380,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        newrelic = wavefront.CloudIntegrationNewRelic("newrelic", api_key="example-api-key")
+        newrelic = wavefront.CloudIntegrationNewRelic("newrelic",
+            name="Test Integration",
+            api_key="example-api-key")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         NewRelic Integrations can be imported by using the `id`, e.g.:
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/config/vars.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/dashboard.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/dashboard_json.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/dashboard_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,134 +75,133 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        test_dashboard_json = wavefront.DashboardJson("testDashboardJson", dashboard_json=\"\"\"  {
-            "acl": {
-              "canModify": [
-                "group-uuid",
-                "role-uuid"
-              ],
-              "canView": [
-                "group-uuid",
-                "role-uuid"
-              ]
-            },
-            "name": "Terraform Test Dashboard Json",
-            "description": "a",
-            "eventFilterType": "BYCHART",
-            "eventQuery": "",
-            "defaultTimeWindow": "",
-            "url": "tftestimport",
-            "displayDescription": false,
-            "displaySectionTableOfContents": true,
-            "displayQueryParameters": false,
-            "sections": [
-              {
-                "name": "section 1",
-                "rows": [
-                  {
-                    "charts": [
-                      {
-                        "name": "chart 1",
-                        "sources": [
-                          {
-                            "name": "source 1",
-                            "query": "ts()",
-                            "scatterPlotSource": "Y",
-                            "querybuilderEnabled": false,
-                            "sourceDescription": ""
-                          }
+        test_dashboard_json = wavefront.DashboardJson("test_dashboard_json", dashboard_json=\"\"\"{
+          "acl": {
+            "canModify": [
+              "group-uuid",
+              "role-uuid"
+            ],
+            "canView": [
+              "group-uuid",
+              "role-uuid"
+            ]
+          },
+          "name": "Terraform Test Dashboard Json",
+          "description": "a",
+          "eventFilterType": "BYCHART",
+          "eventQuery": "",
+          "defaultTimeWindow": "",
+          "url": "tftestimport",
+          "displayDescription": false,
+          "displaySectionTableOfContents": true,
+          "displayQueryParameters": false,
+          "sections": [
+            {
+              "name": "section 1",
+              "rows": [
+                {
+                  "charts": [
+                    {
+                      "name": "chart 1",
+                      "sources": [
+                        {
+                          "name": "source 1",
+                          "query": "ts()",
+                          "scatterPlotSource": "Y",
+                          "querybuilderEnabled": false,
+                          "sourceDescription": ""
+                        }
+                      ],
+                      "units": "someunit",
+                      "base": 0,
+                      "noDefaultEvents": false,
+                      "interpolatePoints": false,
+                      "includeObsoleteMetrics": false,
+                      "description": "This is chart 1, showing something",
+                      "chartSettings": {
+                        "type": "markdown-widget",
+                        "max": 100,
+                        "expectedDataSpacing": 120,
+                        "windowing": "full",
+                        "windowSize": 10,
+                        "autoColumnTags": false,
+                        "columnTags": "deprecated",
+                        "tagMode": "all",
+                        "numTags": 2,
+                        "customTags": [
+                          "tag1",
+                          "tag2"
+                        ],
+                        "groupBySource": true,
+                        "y1Max": 100,
+                        "y1Units": "units",
+                        "y0ScaleSIBy1024": true,
+                        "y1ScaleSIBy1024": true,
+                        "y0UnitAutoscaling": true,
+                        "y1UnitAutoscaling": true,
+                        "fixedLegendEnabled": true,
+                        "fixedLegendUseRawStats": true,
+                        "fixedLegendPosition": "RIGHT",
+                        "fixedLegendDisplayStats": [
+                          "stat1",
+                          "stat2"
                         ],
-                        "units": "someunit",
-                        "base": 0,
-                        "noDefaultEvents": false,
-                        "interpolatePoints": false,
-                        "includeObsoleteMetrics": false,
-                        "description": "This is chart 1, showing something",
-                        "chartSettings": {
-                          "type": "markdown-widget",
-                          "max": 100,
-                          "expectedDataSpacing": 120,
-                          "windowing": "full",
-                          "windowSize": 10,
-                          "autoColumnTags": false,
-                          "columnTags": "deprecated",
-                          "tagMode": "all",
-                          "numTags": 2,
-                          "customTags": [
-                            "tag1",
-                            "tag2"
-                          ],
-                          "groupBySource": true,
-                          "y1Max": 100,
-                          "y1Units": "units",
-                          "y0ScaleSIBy1024": true,
-                          "y1ScaleSIBy1024": true,
-                          "y0UnitAutoscaling": true,
-                          "y1UnitAutoscaling": true,
-                          "fixedLegendEnabled": true,
-                          "fixedLegendUseRawStats": true,
-                          "fixedLegendPosition": "RIGHT",
-                          "fixedLegendDisplayStats": [
-                            "stat1",
-                            "stat2"
-                          ],
-                          "fixedLegendFilterSort": "TOP",
-                          "fixedLegendFilterLimit": 1,
-                          "fixedLegendFilterField": "CURRENT",
-                          "plainMarkdownContent": "markdown content"
-                        },
-                        "chartAttributes": {
-                          "dashboardLinks": {
-                            "*": {
-                              "variables": {
-                                "xxx": "xxx"
-                              },
-                              "destination": "/dashboards/xxxx"
-                            }
+                        "fixedLegendFilterSort": "TOP",
+                        "fixedLegendFilterLimit": 1,
+                        "fixedLegendFilterField": "CURRENT",
+                        "plainMarkdownContent": "markdown content"
+                      },
+                      "chartAttributes": {
+                        "dashboardLinks": {
+                          "*": {
+                            "variables": {
+                              "xxx": "xxx"
+                            },
+                            "destination": "/dashboards/xxxx"
                           }
-                        },
-                        "summarization": "MEAN"
-                      }
-                    ],
-                    "heightFactor": 50
-                  }
-                ]
-              }
-            ],
-            "parameterDetails": {
-              "param": {
-                "hideFromView": false,
-                "description": null,
-                "allowAll": null,
-                "tagKey": null,
-                "queryValue": null,
-                "dynamicFieldType": null,
-                "reverseDynSort": null,
-                "parameterType": "SIMPLE",
-                "label": "test",
-                "defaultValue": "Label",
-                "valuesToReadableStrings": {
-                  "Label": "test"
-                },
-                "selectedLabel": "Label",
-                "value": "test"
-              }
-            },
-            "tags": {
-              "customerTags": [
-                "terraform"
+                        }
+                      },
+                      "summarization": "MEAN"
+                    }
+                  ],
+                  "heightFactor": 50
+                }
               ]
             }
+          ],
+          "parameterDetails": {
+            "param": {
+              "hideFromView": false,
+              "description": null,
+              "allowAll": null,
+              "tagKey": null,
+              "queryValue": null,
+              "dynamicFieldType": null,
+              "reverseDynSort": null,
+              "parameterType": "SIMPLE",
+              "label": "test",
+              "defaultValue": "Label",
+              "valuesToReadableStrings": {
+                "Label": "test"
+              },
+              "selectedLabel": "Label",
+              "value": "test"
+            }
+          },
+          "tags": {
+            "customerTags": [
+              "terraform"
+            ]
           }
-
+        }
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         * 
         *Note:
         ** If there are dynamic variables in the Wavefront dashboard json, then these variables must be present in a separate file as mentioned in the section below.
@@ -232,134 +231,133 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        test_dashboard_json = wavefront.DashboardJson("testDashboardJson", dashboard_json=\"\"\"  {
-            "acl": {
-              "canModify": [
-                "group-uuid",
-                "role-uuid"
-              ],
-              "canView": [
-                "group-uuid",
-                "role-uuid"
-              ]
-            },
-            "name": "Terraform Test Dashboard Json",
-            "description": "a",
-            "eventFilterType": "BYCHART",
-            "eventQuery": "",
-            "defaultTimeWindow": "",
-            "url": "tftestimport",
-            "displayDescription": false,
-            "displaySectionTableOfContents": true,
-            "displayQueryParameters": false,
-            "sections": [
-              {
-                "name": "section 1",
-                "rows": [
-                  {
-                    "charts": [
-                      {
-                        "name": "chart 1",
-                        "sources": [
-                          {
-                            "name": "source 1",
-                            "query": "ts()",
-                            "scatterPlotSource": "Y",
-                            "querybuilderEnabled": false,
-                            "sourceDescription": ""
-                          }
+        test_dashboard_json = wavefront.DashboardJson("test_dashboard_json", dashboard_json=\"\"\"{
+          "acl": {
+            "canModify": [
+              "group-uuid",
+              "role-uuid"
+            ],
+            "canView": [
+              "group-uuid",
+              "role-uuid"
+            ]
+          },
+          "name": "Terraform Test Dashboard Json",
+          "description": "a",
+          "eventFilterType": "BYCHART",
+          "eventQuery": "",
+          "defaultTimeWindow": "",
+          "url": "tftestimport",
+          "displayDescription": false,
+          "displaySectionTableOfContents": true,
+          "displayQueryParameters": false,
+          "sections": [
+            {
+              "name": "section 1",
+              "rows": [
+                {
+                  "charts": [
+                    {
+                      "name": "chart 1",
+                      "sources": [
+                        {
+                          "name": "source 1",
+                          "query": "ts()",
+                          "scatterPlotSource": "Y",
+                          "querybuilderEnabled": false,
+                          "sourceDescription": ""
+                        }
+                      ],
+                      "units": "someunit",
+                      "base": 0,
+                      "noDefaultEvents": false,
+                      "interpolatePoints": false,
+                      "includeObsoleteMetrics": false,
+                      "description": "This is chart 1, showing something",
+                      "chartSettings": {
+                        "type": "markdown-widget",
+                        "max": 100,
+                        "expectedDataSpacing": 120,
+                        "windowing": "full",
+                        "windowSize": 10,
+                        "autoColumnTags": false,
+                        "columnTags": "deprecated",
+                        "tagMode": "all",
+                        "numTags": 2,
+                        "customTags": [
+                          "tag1",
+                          "tag2"
+                        ],
+                        "groupBySource": true,
+                        "y1Max": 100,
+                        "y1Units": "units",
+                        "y0ScaleSIBy1024": true,
+                        "y1ScaleSIBy1024": true,
+                        "y0UnitAutoscaling": true,
+                        "y1UnitAutoscaling": true,
+                        "fixedLegendEnabled": true,
+                        "fixedLegendUseRawStats": true,
+                        "fixedLegendPosition": "RIGHT",
+                        "fixedLegendDisplayStats": [
+                          "stat1",
+                          "stat2"
                         ],
-                        "units": "someunit",
-                        "base": 0,
-                        "noDefaultEvents": false,
-                        "interpolatePoints": false,
-                        "includeObsoleteMetrics": false,
-                        "description": "This is chart 1, showing something",
-                        "chartSettings": {
-                          "type": "markdown-widget",
-                          "max": 100,
-                          "expectedDataSpacing": 120,
-                          "windowing": "full",
-                          "windowSize": 10,
-                          "autoColumnTags": false,
-                          "columnTags": "deprecated",
-                          "tagMode": "all",
-                          "numTags": 2,
-                          "customTags": [
-                            "tag1",
-                            "tag2"
-                          ],
-                          "groupBySource": true,
-                          "y1Max": 100,
-                          "y1Units": "units",
-                          "y0ScaleSIBy1024": true,
-                          "y1ScaleSIBy1024": true,
-                          "y0UnitAutoscaling": true,
-                          "y1UnitAutoscaling": true,
-                          "fixedLegendEnabled": true,
-                          "fixedLegendUseRawStats": true,
-                          "fixedLegendPosition": "RIGHT",
-                          "fixedLegendDisplayStats": [
-                            "stat1",
-                            "stat2"
-                          ],
-                          "fixedLegendFilterSort": "TOP",
-                          "fixedLegendFilterLimit": 1,
-                          "fixedLegendFilterField": "CURRENT",
-                          "plainMarkdownContent": "markdown content"
-                        },
-                        "chartAttributes": {
-                          "dashboardLinks": {
-                            "*": {
-                              "variables": {
-                                "xxx": "xxx"
-                              },
-                              "destination": "/dashboards/xxxx"
-                            }
+                        "fixedLegendFilterSort": "TOP",
+                        "fixedLegendFilterLimit": 1,
+                        "fixedLegendFilterField": "CURRENT",
+                        "plainMarkdownContent": "markdown content"
+                      },
+                      "chartAttributes": {
+                        "dashboardLinks": {
+                          "*": {
+                            "variables": {
+                              "xxx": "xxx"
+                            },
+                            "destination": "/dashboards/xxxx"
                           }
-                        },
-                        "summarization": "MEAN"
-                      }
-                    ],
-                    "heightFactor": 50
-                  }
-                ]
-              }
-            ],
-            "parameterDetails": {
-              "param": {
-                "hideFromView": false,
-                "description": null,
-                "allowAll": null,
-                "tagKey": null,
-                "queryValue": null,
-                "dynamicFieldType": null,
-                "reverseDynSort": null,
-                "parameterType": "SIMPLE",
-                "label": "test",
-                "defaultValue": "Label",
-                "valuesToReadableStrings": {
-                  "Label": "test"
-                },
-                "selectedLabel": "Label",
-                "value": "test"
-              }
-            },
-            "tags": {
-              "customerTags": [
-                "terraform"
+                        }
+                      },
+                      "summarization": "MEAN"
+                    }
+                  ],
+                  "heightFactor": 50
+                }
               ]
             }
+          ],
+          "parameterDetails": {
+            "param": {
+              "hideFromView": false,
+              "description": null,
+              "allowAll": null,
+              "tagKey": null,
+              "queryValue": null,
+              "dynamicFieldType": null,
+              "reverseDynSort": null,
+              "parameterType": "SIMPLE",
+              "label": "test",
+              "defaultValue": "Label",
+              "valuesToReadableStrings": {
+                "Label": "test"
+              },
+              "selectedLabel": "Label",
+              "value": "test"
+            }
+          },
+          "tags": {
+            "customerTags": [
+              "terraform"
+            ]
           }
-
+        }
         \"\"\")
         ```
         <!--End PulumiCodeChooser -->
 
         * 
         *Note:
         ** If there are dynamic variables in the Wavefront dashboard json, then these variables must be present in a separate file as mentioned in the section below.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/derived_metric.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/derived_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         derived = wavefront.DerivedMetric("derived",
+            name="dummy derived metric",
             minutes=5,
             query="aliasMetric(5, \\"some.metric\\")")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -243,14 +244,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         derived = wavefront.DerivedMetric("derived",
+            name="dummy derived metric",
             minutes=5,
             query="aliasMetric(5, \\"some.metric\\")")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/event.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,18 +196,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         event = wavefront.Event("event",
+            name="terraform-test",
             annotations={
-                "details": "description",
                 "severity": "info",
                 "type": "event type",
+                "details": "description",
             },
             tags=["eventTag1"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -237,18 +238,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         event = wavefront.Event("event",
+            name="terraform-test",
             annotations={
-                "details": "description",
                 "severity": "info",
                 "type": "event type",
+                "details": "description",
             },
             tags=["eventTag1"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/external_link.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/external_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,14 +281,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.ExternalLink("basic",
+            name="External Link",
             description="An external link description",
             template="https://example.com/source={{{source}}}&startTime={{startEpochMillis}}")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -324,14 +325,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.ExternalLink("basic",
+            name="External Link",
             description="An external link description",
             template="https://example.com/source={{{source}}}&startTime={{startEpochMillis}}")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_alert.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,14 +339,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about the alert.
     example = wavefront.get_alert(id="alert-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the alert data to be fetched.
     :param Mapping[str, str] targets: A comma-separated list of the email addresses or integration endpoints (such as PagerDuty or webhook) to notify when the alert status changes. Multiple target types can be in the list.
@@ -395,14 +396,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about the alert.
     example = wavefront.get_alert(id="alert-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the alert data to be fetched.
     :param Mapping[str, str] targets: A comma-separated list of the email addresses or integration endpoints (such as PagerDuty or webhook) to notify when the alert status changes. Multiple target types can be in the list.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_alerts.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_alerts.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about all alerts.
     example = wavefront.get_alerts(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
@@ -120,14 +121,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about all alerts.
     example = wavefront.get_alerts(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_dashboard.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_dashboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -389,14 +389,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about a dashboard.
     example = wavefront.get_dashboard(id="dashboard-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the dashboard data to be fetched.
     """
@@ -452,14 +453,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about a dashboard.
     example = wavefront.get_dashboard(id="dashboard-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the dashboard data to be fetched.
     """
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_dashboards.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_dashboards.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about all dashboards.
     example = wavefront.get_dashboards(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
@@ -120,14 +121,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about all dashboards.
     example = wavefront.get_dashboards(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_default_user_group.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_default_user_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the default user group "Everyone"
     everyone_group = wavefront.get_default_user_group()
     ```
     <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getDefaultUserGroup:getDefaultUserGroup', __args__, opts=opts, typ=GetDefaultUserGroupResult).value
@@ -89,12 +90,13 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the default user group "Everyone"
     everyone_group = wavefront.get_default_user_group()
     ```
     <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_derived_metric.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_derived_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    #Get the information about a derived metric.
     example = wavefront.get_derived_metric(id="derived_metric_id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the derived metric data to be fetched.
     """
@@ -380,14 +381,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    #Get the information about a derived metric.
     example = wavefront.get_derived_metric(id="derived_metric_id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the derived metric data to be fetched.
     """
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_derived_metrics.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_derived_metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about all derived metrics.
     example = wavefront.get_derived_metrics(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
@@ -120,14 +121,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about all derived metrics.
     example = wavefront.get_derived_metrics(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_event.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about a Wavefront event by its ID.
     example = wavefront.get_event(id="sample-event-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the event data to be fetched.
     """
@@ -195,14 +196,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about a Wavefront event by its ID.
     example = wavefront.get_event(id="sample-event-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the event data to be fetched.
     """
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_events.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,18 +110,19 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
-    example = wavefront.get_events(earliest_start_time_epoch_millis=1665427195,
+    # Get the information about all events
+    example = wavefront.get_events(limit=10,
+        offset=0,
         latest_start_time_epoch_millis=1665427195,
-        limit=10,
-        offset=0)
+        earliest_start_time_epoch_millis=1665427195)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int earliest_start_time_epoch_millis: The earliest start time in epoch milliseconds.
     :param int latest_start_time_epoch_millis: The latest start time in epoch milliseconds.
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
@@ -156,18 +157,19 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
-    example = wavefront.get_events(earliest_start_time_epoch_millis=1665427195,
+    # Get the information about all events
+    example = wavefront.get_events(limit=10,
+        offset=0,
         latest_start_time_epoch_millis=1665427195,
-        limit=10,
-        offset=0)
+        earliest_start_time_epoch_millis=1665427195)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int earliest_start_time_epoch_millis: The earliest start time in epoch milliseconds.
     :param int latest_start_time_epoch_millis: The latest start time in epoch milliseconds.
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_external_link.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_external_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about a specific external links.
     example = wavefront.get_external_link(id="sample-external-link-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the external link.
     """
@@ -227,14 +228,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about a specific external links.
     example = wavefront.get_external_link(id="sample-external-link-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the external link.
     """
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_external_links.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_external_links.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about all external links.
     example = wavefront.get_external_links(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
@@ -120,14 +121,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about all external links.
     example = wavefront.get_external_links(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_maintenance_window.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_maintenance_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about specific maintenance window.
     example = wavefront.get_maintenance_window(id="sample-maintenance-window-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the maintenance window.
     """
@@ -308,14 +309,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about specific maintenance window.
     example = wavefront.get_maintenance_window(id="sample-maintenance-window-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the maintenance window.
     """
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_maintenance_window_all.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_maintenance_window_all.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_metrics_policy.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_role.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_role.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about the role.
     example = wavefront.get_role(id="role-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the role data to be fetched.
     """
@@ -120,14 +121,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about the role.
     example = wavefront.get_role(id="role-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the role data to be fetched.
     """
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_roles.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get all Roles
     roles = wavefront.get_roles(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
@@ -120,14 +121,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get all Roles
     roles = wavefront.get_roles(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_user.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the info for user "example.user@example.com"
     example = wavefront.get_user(email="example.user@example.com")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str email: The email associated with the user data to be fetched.
     """
@@ -143,14 +144,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the info for user "example.user@example.com"
     example = wavefront.get_user(email="example.user@example.com")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str email: The email associated with the user data to be fetched.
     """
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_user_group.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about the user group.
     example = wavefront.get_user_group(id="user-group-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the user group data to be fetched.
     """
@@ -133,14 +134,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get the information about the user group.
     example = wavefront.get_user_group(id="user-group-id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID associated with the user group data to be fetched.
     """
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_user_groups.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_user_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get all user groups
     groups = wavefront.get_user_groups(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
@@ -120,14 +121,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get all user groups
     groups = wavefront.get_user_groups(limit=10,
         offset=0)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param int limit: Limit is the maximum number of results to be returned. Defaults to 100.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/get_users.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/get_users.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get all users
     users = wavefront.get_users()
     ```
     <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('wavefront:index/getUsers:getUsers', __args__, opts=opts, typ=GetUsersResult).value
@@ -89,12 +90,13 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_wavefront as wavefront
 
+    # Get all users
     users = wavefront.get_users()
     ```
     <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/ingestion_policy.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/ingestion_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        basic = wavefront.IngestionPolicy("basic", description="An ingestion policy for testing")
+        basic = wavefront.IngestionPolicy("basic",
+            name="test_ingestion",
+            description="An ingestion policy for testing")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         ingestion policies can be imported by using the `id`, e.g.:
 
@@ -288,15 +290,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        basic = wavefront.IngestionPolicy("basic", description="An ingestion policy for testing")
+        basic = wavefront.IngestionPolicy("basic",
+            name="test_ingestion",
+            description="An ingestion policy for testing")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         ingestion policies can be imported by using the `id`, e.g.:
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/maintenance_window.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/maintenance_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,22 +377,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.MaintenanceWindow("basic",
-            end_time_in_seconds=1601123456,
             reason="Routine maintenance for 2020",
+            title="Routine maintenance",
+            start_time_in_seconds=1600123456,
+            end_time_in_seconds=1601123456,
             relevant_host_names=[
                 "my_hostname",
                 "my_other_hostname",
-            ],
-            start_time_in_seconds=1600123456,
-            title="Routine maintenance")
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Maintenance windows can be imported using the `id`, e.g.
 
@@ -436,22 +436,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.MaintenanceWindow("basic",
-            end_time_in_seconds=1601123456,
             reason="Routine maintenance for 2020",
+            title="Routine maintenance",
+            start_time_in_seconds=1600123456,
+            end_time_in_seconds=1601123456,
             relevant_host_names=[
                 "my_hostname",
                 "my_other_hostname",
-            ],
-            start_time_in_seconds=1600123456,
-            title="Routine maintenance")
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Maintenance windows can be imported using the `id`, e.g.
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/metrics_policy.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/metrics_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,16 +144,16 @@
         ### Example
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        policy_metrics_policy = wavefront.get_metrics_policy()
-        pulumi.export("policy", policy_metrics_policy)
+        policy = wavefront.get_metrics_policy()
+        pulumi.export("policy", policy)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported by using the `updated_epoch_millis`, e.g.:
 
@@ -200,16 +200,16 @@
         ### Example
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        policy_metrics_policy = wavefront.get_metrics_policy()
-        pulumi.export("policy", policy_metrics_policy)
+        policy = wavefront.get_metrics_policy()
+        pulumi.export("policy", policy)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported by using the `updated_epoch_millis`, e.g.:
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/outputs.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/provider.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/role.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        role = wavefront.Role("role")
+        role = wavefront.Role("role", name="Test Role")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Roles can be imported by using the `id`, e.g.:
 
@@ -216,15 +216,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        role = wavefront.Role("role")
+        role = wavefront.Role("role", name="Test Role")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Roles can be imported by using the `id`, e.g.:
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/service_account.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/service_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,16 +245,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.ServiceAccount("basic",
-            active=True,
-            identifier="sa::tftesting")
+            identifier="sa::tftesting",
+            active=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service accounts can be imported by using `identifier`, e.g.:
 
@@ -286,16 +286,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
         basic = wavefront.ServiceAccount("basic",
-            active=True,
-            identifier="sa::tftesting")
+            identifier="sa::tftesting",
+            active=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service accounts can be imported by using `identifier`, e.g.:
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/user.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront/user_group.py` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront/user_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        basic = wavefront.UserGroup("basic", description="Basic User Group for Unit Tests")
+        basic = wavefront.UserGroup("basic",
+            name="Basic User Group",
+            description="Basic User Group for Unit Tests")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         User Groups can be imported by using the `id`, e.g.:
 
@@ -137,15 +139,17 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_wavefront as wavefront
 
-        basic = wavefront.UserGroup("basic", description="Basic User Group for Unit Tests")
+        basic = wavefront.UserGroup("basic",
+            name="Basic User Group",
+            description="Basic User Group for Unit Tests")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         User Groups can be imported by using the `id`, e.g.:
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront.egg-info/PKG-INFO` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_wavefront
-Version: 3.2.0a1713340678
+Version: 3.2.0a1713526439
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi,wavefront
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_wavefront-3.2.0a1713340678/pulumi_wavefront.egg-info/SOURCES.txt` & `pulumi_wavefront-3.2.0a1713526439/pulumi_wavefront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-3.2.0a1713340678/pyproject.toml` & `pulumi_wavefront-3.2.0a1713526439/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_wavefront"
   description = "A Pulumi package for creating and managing wavefront cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "wavefront"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.2.0a1713340678"
+  version = "3.2.0a1713526439"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-wavefront"
 
 [build-system]
```

