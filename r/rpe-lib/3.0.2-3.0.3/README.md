# Comparing `tmp/rpe-lib-3.0.2.tar.gz` & `tmp/rpe-lib-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpe-lib-3.0.2.tar", last modified: Tue Dec 13 16:51:49 2022, max compression
+gzip compressed data, was "rpe-lib-3.0.3.tar", last modified: Fri Apr 19 21:11:56 2024, max compression
```

## Comparing `rpe-lib-3.0.2.tar` & `rpe-lib-3.0.3.tar`

### file list

```diff
@@ -1,175 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.318875 rpe-lib-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.250875 rpe-lib-3.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.258875 rpe-lib-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      337 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2022-12-13 16:51:49.318875 rpe-lib-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.262875 rpe-lib-3.0.2/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/exclusions.rego
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.274875 rpe-lib-3.0.2/policy/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/_util.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/appengine_instances_disallow_debug_mode.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/bigquery_datasets_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/bigquery_datasets_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/bigtable_instances_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/bigtable_instances_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/cloudfunctions_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/cloudfunctions_disallow_default_service_account.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/cloudfunctions_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/cloudresourcemanager_projects_require_all_audit_logs.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/compute_disks_disallow_unapproved_images.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/compute_firewalls_disallow_public_management_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/compute_firewalls_require_logging.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/compute_subnets_require_private_google_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/compute_subnetworks_require_flow_logging.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/container_clusters_disallow_kubernetes_dashboard.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/container_clusters_disallow_legacy_abac.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/container_clusters_require_stackdriver_logging.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/container_clusters_require_stackdriver_monitoring.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/container_nodepools_require_autoupgrade_and_autorepair.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/container_nodepools_require_cos_image.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/dataproc_clusters_disallow_default_serviceaccount.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/dataproc_clusters_disallow_extended_use.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/dataproc_clusters_require_approved_image.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/dataproc_clusters_require_job_logging.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/dataproc_clusters_require_kerberos.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/dataproc_clusters_require_stackdriver_logging.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/dataproc_clusters_require_yarn_logging.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/pubsub_subscriptions_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/pubsub_subscriptions_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/pubsub_topics_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/pubsub_topics_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/sql_instances_disallow_public_network_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/sql_instances_require_backup_configuration.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/sql_instances_require_ssl.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/storage_buckets_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/storage_buckets_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/storage_buckets_require_object_versioning.rego
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.290875 rpe-lib-3.0.2/policy/gcp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/appengine_instances_disallow_debug_mode_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/bigquery_datasets_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/bigquery_datasets_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/bigtable_instances_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/bigtable_instances_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/cloudfunctions_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/cloudfunctions_disallow_default_service_account_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/cloudfunctions_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/compute_disks_disallow_unapproved_images_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/compute_firewalls_disallow_public_management_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/compute_firewalls_require_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)      895 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/compute_subnets_require_private_google_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)      920 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/compute_subnetworks_require_flow_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/container_clusters_disallow_kubernetes_dashboard_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/container_clusters_disallow_legacy_abac_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/container_clusters_require_stackdriver_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/container_clusters_require_stackdriver_monitoring_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/container_nodepools_require_autoupgrade_and_autorepair_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/container_nodepools_require_cos_image_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_disallow_default_serviceaccount_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_disallow_extended_use_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_require_approved_image_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_require_job_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_require_kerberos_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_require_stackdriver_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_require_yarn_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/pubsub_subscriptions_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/pubsub_subscriptions_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/pubsub_topics_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/pubsub_topics_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/sql_instances_disallow_public_network_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/sql_instances_require_backup_configuration_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/sql_instances_require_ssl_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/storage_buckets_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/storage_buckets_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/gcp/tests/storage_buckets_require_object_versioning_test.rego
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/policies.rego
--rw-r--r--   0 runner    (1001) docker     (123)      873 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/policy/util.rego
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.290875 rpe-lib-3.0.2/rpe/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.294875 rpe-lib-3.0.2/rpe/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/engines/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/engines/opa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/engines/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.294875 rpe-lib-3.0.2/rpe/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/extractors/gcp_auditlogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/extractors/micromanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/extractors/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/extractors/pubsub_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.298875 rpe-lib-3.0.2/rpe/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/resources/__init__.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    33058 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/resources/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/rpe/rpe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.298875 rpe-lib-3.0.2/rpe_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2022-12-13 16:51:48.000000 rpe-lib-3.0.2/rpe_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2022-12-13 16:51:49.000000 rpe-lib-3.0.2/rpe_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 16:51:48.000000 rpe-lib-3.0.2/rpe_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-13 16:51:48.000000 rpe-lib-3.0.2/rpe_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-13 16:51:48.000000 rpe-lib-3.0.2/rpe_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 16:51:49.318875 rpe-lib-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.302875 rpe-lib-3.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:51:49.318875 rpe-lib-3.0.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/app-engine-debug.json
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/bigtable-set-iam-policy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/bq-ds-set-iam-policy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/cloudfunctions-set-iam-policy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/cloudsql-protoPayload.request.body.json
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/cloudsql-protoPayload.request.resource.instanceName.instanceId.json
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/cloudsql-resource.labels.json
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute-firewalls-enable-logs-policy.json
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute-hardened-images.json
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute-subnetworks-enable-flow-logs.json
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute-subnetworks-set-private-ip-google-access.json
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute_instance_creation_logs_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute_instance_creation_logs_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute_instance_creation_logs_3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute_instance_creation_logs_4.json
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute_instance_creation_logs_5.json
--rw-r--r--   0 runner    (1001) docker     (123)      419 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute_instance_micromanager.json
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute_networks_insert_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute_networks_insert_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/compute_networks_insert_3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/dataflow-job-step.json
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/datafusion-create-instance.json
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/datafusion-update-instance.json
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/dataproc_createcluster.json
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/gke-cluster-update.json
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/gke-nodepool-set.json
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/memorystore-redis.json
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/project_get_iam.json
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/project_set_iam.json
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/pubsub-subscription-set-iam-policy.json
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/pubsub-topic-set-iam-policy.json
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/servicemanagement-activate-service.json
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/servicemanagement-deactivate-service.json
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/servicemanagement-disable-service.json
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/servicemanagement-enable-service.json
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/serviceusage-batchenable.json
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/serviceusage-disable.json
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/serviceusage-enable.json
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/storage_bucket_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/storage_bucket_micromanager.json
--rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/storage_bucket_no_metadata_micromanager.json
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/data/storage_bucket_update.json
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/test_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/test_gcp_resource_inferred_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17416 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tests/test_resources_cai.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-13 16:51:34.000000 rpe-lib-3.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.258701 rpe-lib-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.234701 rpe-lib-3.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.234701 rpe-lib-3.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-19 21:11:56.258701 rpe-lib-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.238701 rpe-lib-3.0.3/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/exclusions.rego
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.242701 rpe-lib-3.0.3/policy/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/_util.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/appengine_instances_disallow_debug_mode.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/bigquery_datasets_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/bigquery_datasets_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/bigtable_instances_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/bigtable_instances_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_default_service_account.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/cloudresourcemanager_projects_require_all_audit_logs.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/compute_disks_disallow_unapproved_images.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/compute_firewalls_disallow_public_management_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/compute_firewalls_require_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/compute_subnets_require_private_google_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/compute_subnetworks_require_flow_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_clusters_disallow_kubernetes_dashboard.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_clusters_disallow_legacy_abac.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_clusters_require_stackdriver_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_clusters_require_stackdriver_monitoring.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_nodepools_require_autoupgrade_and_autorepair.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_nodepools_require_cos_image.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_disallow_default_serviceaccount.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_disallow_extended_use.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_approved_image.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_job_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_kerberos.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_stackdriver_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_yarn_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/pubsub_subscriptions_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/pubsub_subscriptions_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/pubsub_topics_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/pubsub_topics_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/sql_instances_disallow_public_network_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/sql_instances_require_backup_configuration.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/sql_instances_require_ssl.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/storage_buckets_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/storage_buckets_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/storage_buckets_require_object_versioning.rego
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.246701 rpe-lib-3.0.3/policy/gcp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/appengine_instances_disallow_debug_mode_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/bigquery_datasets_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/bigquery_datasets_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/bigtable_instances_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/bigtable_instances_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_default_service_account_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/compute_disks_disallow_unapproved_images_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/compute_firewalls_disallow_public_management_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/compute_firewalls_require_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/compute_subnets_require_private_google_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/compute_subnetworks_require_flow_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_clusters_disallow_kubernetes_dashboard_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_clusters_disallow_legacy_abac_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_clusters_require_stackdriver_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_clusters_require_stackdriver_monitoring_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_nodepools_require_autoupgrade_and_autorepair_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_nodepools_require_cos_image_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_disallow_default_serviceaccount_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_disallow_extended_use_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_approved_image_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_job_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_kerberos_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_stackdriver_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_yarn_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/pubsub_subscriptions_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/pubsub_subscriptions_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/pubsub_topics_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/pubsub_topics_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/sql_instances_disallow_public_network_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/sql_instances_require_backup_configuration_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/sql_instances_require_ssl_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_require_object_versioning_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/policies.rego
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/util.rego
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/rpe/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/rpe/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/engines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/engines/opa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/engines/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/rpe/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17188 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/extractors/gcp_auditlogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/extractors/micromanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/extractors/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/extractors/pubsub_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/rpe/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/resources/__init__.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35199 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/resources/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/rpe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/rpe_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-19 21:11:55.000000 rpe-lib-3.0.3/rpe_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-19 21:11:56.000000 rpe-lib-3.0.3/rpe_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:11:55.000000 rpe-lib-3.0.3/rpe_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 21:11:55.000000 rpe-lib-3.0.3/rpe_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 21:11:55.000000 rpe-lib-3.0.3/rpe_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:11:56.258701 rpe-lib-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.258701 rpe-lib-3.0.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/app-engine-debug.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/bigtable-set-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/bq-ds-set-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/cloudfunctions-set-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/cloudsql-protoPayload.request.body.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/cloudsql-protoPayload.request.resource.instanceName.instanceId.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/cloudsql-resource.labels.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute-firewalls-enable-logs-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute-hardened-images.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute-subnetworks-enable-flow-logs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute-subnetworks-set-private-ip-google-access.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_micromanager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_networks_insert_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_networks_insert_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_networks_insert_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/dataflow-job-step.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/dataform-create-repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/dataform-create-workspace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/dataform-update-repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/datafusion-create-instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/datafusion-update-instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/dataproc_createcluster.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/gke-cluster-update.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/gke-nodepool-set.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/memorystore-redis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/project_get_iam.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/project_set_iam.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/pubsub-subscription-set-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/pubsub-topic-set-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/servicemanagement-activate-service.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/servicemanagement-deactivate-service.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/servicemanagement-disable-service.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/servicemanagement-enable-service.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/serviceusage-batchenable.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/serviceusage-disable.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/serviceusage-enable.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/storage_bucket_delete.json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/storage_bucket_micromanager.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/storage_bucket_no_metadata_micromanager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/storage_bucket_update.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/test_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/test_gcp_resource_inferred_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18739 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/test_resources_cai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tox.ini
```

### Comparing `rpe-lib-3.0.2/.github/workflows/build.yml` & `rpe-lib-3.0.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/.github/workflows/release.yml` & `rpe-lib-3.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/CONTRIBUTING.md` & `rpe-lib-3.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/LICENSE` & `rpe-lib-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/PKG-INFO` & `rpe-lib-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpe-lib
-Version: 3.0.2
+Version: 3.0.3
 Summary: A resource policy evaluation library
 Home-page: https://github.com/cleardataeng/resource-policy-evaluation-library
 Author: Joe Ceresini
 License: Apache 2.0
 Description: # resource-policy-evaluation-library
         
         rpe-lib is made up of `Policy Engines (rpe.engines.Engine)`, `Resources (rpe.resources.Resource)`, and `Extractors (rpe.resources.Extractor)`.
```

### Comparing `rpe-lib-3.0.2/README.md` & `rpe-lib-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/config.yaml` & `rpe-lib-3.0.3/policy/config.yaml`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/exclusions.rego` & `rpe-lib-3.0.3/policy/exclusions.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/appengine_instances_disallow_debug_mode.rego` & `rpe-lib-3.0.3/policy/gcp/appengine_instances_disallow_debug_mode.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/bigquery_datasets_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/bigquery_datasets_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/bigquery_datasets_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/bigquery_datasets_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/bigtable_instances_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/bigtable_instances_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/bigtable_instances_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/bigtable_instances_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/cloudfunctions_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/cloudfunctions_disallow_default_service_account.rego` & `rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_default_service_account.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/cloudfunctions_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/cloudresourcemanager_projects_require_all_audit_logs.rego` & `rpe-lib-3.0.3/policy/gcp/cloudresourcemanager_projects_require_all_audit_logs.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/compute_disks_disallow_unapproved_images.rego` & `rpe-lib-3.0.3/policy/gcp/compute_disks_disallow_unapproved_images.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/compute_firewalls_disallow_public_management_access.rego` & `rpe-lib-3.0.3/policy/gcp/compute_firewalls_disallow_public_management_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/compute_firewalls_require_logging.rego` & `rpe-lib-3.0.3/policy/gcp/compute_firewalls_require_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/compute_subnets_require_private_google_access.rego` & `rpe-lib-3.0.3/policy/gcp/compute_subnets_require_private_google_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/compute_subnetworks_require_flow_logging.rego` & `rpe-lib-3.0.3/policy/gcp/compute_subnetworks_require_flow_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/container_clusters_disallow_kubernetes_dashboard.rego` & `rpe-lib-3.0.3/policy/gcp/container_clusters_disallow_kubernetes_dashboard.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/container_clusters_disallow_legacy_abac.rego` & `rpe-lib-3.0.3/policy/gcp/container_clusters_disallow_legacy_abac.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/container_clusters_require_stackdriver_logging.rego` & `rpe-lib-3.0.3/policy/gcp/container_clusters_require_stackdriver_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/container_clusters_require_stackdriver_monitoring.rego` & `rpe-lib-3.0.3/policy/gcp/container_clusters_require_stackdriver_monitoring.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/container_nodepools_require_autoupgrade_and_autorepair.rego` & `rpe-lib-3.0.3/policy/gcp/container_nodepools_require_autoupgrade_and_autorepair.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/container_nodepools_require_cos_image.rego` & `rpe-lib-3.0.3/policy/gcp/container_nodepools_require_cos_image.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/dataproc_clusters_disallow_default_serviceaccount.rego` & `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_disallow_default_serviceaccount.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/dataproc_clusters_disallow_extended_use.rego` & `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_disallow_extended_use.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/dataproc_clusters_require_approved_image.rego` & `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_approved_image.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/dataproc_clusters_require_job_logging.rego` & `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_job_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/dataproc_clusters_require_kerberos.rego` & `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_kerberos.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/dataproc_clusters_require_stackdriver_logging.rego` & `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_stackdriver_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/dataproc_clusters_require_yarn_logging.rego` & `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_yarn_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/pubsub_subscriptions_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/pubsub_subscriptions_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/pubsub_subscriptions_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/pubsub_subscriptions_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/pubsub_topics_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/pubsub_topics_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/pubsub_topics_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/pubsub_topics_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/sql_instances_disallow_public_network_access.rego` & `rpe-lib-3.0.3/policy/gcp/sql_instances_disallow_public_network_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/sql_instances_require_backup_configuration.rego` & `rpe-lib-3.0.3/policy/gcp/sql_instances_require_backup_configuration.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/sql_instances_require_ssl.rego` & `rpe-lib-3.0.3/policy/gcp/sql_instances_require_ssl.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/storage_buckets_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/storage_buckets_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/storage_buckets_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.3/policy/gcp/storage_buckets_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/storage_buckets_require_object_versioning.rego` & `rpe-lib-3.0.3/policy/gcp/storage_buckets_require_object_versioning.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/appengine_instances_disallow_debug_mode_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/appengine_instances_disallow_debug_mode_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/bigquery_datasets_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/bigquery_datasets_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/bigquery_datasets_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/bigquery_datasets_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/bigtable_instances_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/bigtable_instances_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/bigtable_instances_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/bigtable_instances_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/cloudfunctions_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/cloudfunctions_disallow_default_service_account_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_default_service_account_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/cloudfunctions_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/compute_disks_disallow_unapproved_images_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/compute_disks_disallow_unapproved_images_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/compute_firewalls_disallow_public_management_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/compute_firewalls_disallow_public_management_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/compute_firewalls_require_logging_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/compute_firewalls_require_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/compute_subnets_require_private_google_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/compute_subnets_require_private_google_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/compute_subnetworks_require_flow_logging_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/compute_subnetworks_require_flow_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/container_clusters_disallow_kubernetes_dashboard_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/container_clusters_disallow_kubernetes_dashboard_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/container_clusters_disallow_legacy_abac_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/container_clusters_disallow_legacy_abac_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/container_clusters_require_stackdriver_logging_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/container_clusters_require_stackdriver_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/container_clusters_require_stackdriver_monitoring_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/container_clusters_require_stackdriver_monitoring_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/container_nodepools_require_autoupgrade_and_autorepair_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/container_nodepools_require_autoupgrade_and_autorepair_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/container_nodepools_require_cos_image_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/container_nodepools_require_cos_image_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_disallow_default_serviceaccount_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_disallow_default_serviceaccount_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_disallow_extended_use_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_disallow_extended_use_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_require_approved_image_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_approved_image_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_require_job_logging_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_job_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_require_kerberos_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_kerberos_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_require_stackdriver_logging_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_stackdriver_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/dataproc_clusters_require_yarn_logging_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_yarn_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/pubsub_subscriptions_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/pubsub_subscriptions_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/pubsub_subscriptions_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/pubsub_subscriptions_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/pubsub_topics_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/pubsub_topics_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/pubsub_topics_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/pubsub_topics_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/sql_instances_disallow_public_network_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/sql_instances_disallow_public_network_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/sql_instances_require_backup_configuration_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/sql_instances_require_backup_configuration_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/sql_instances_require_ssl_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/sql_instances_require_ssl_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/storage_buckets_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/storage_buckets_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/gcp/tests/storage_buckets_require_object_versioning_test.rego` & `rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_require_object_versioning_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/policies.rego` & `rpe-lib-3.0.3/policy/policies.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/policy/util.rego` & `rpe-lib-3.0.3/policy/util.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe/__init__.py` & `rpe-lib-3.0.3/rpe/__init__.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe/engines/__init__.py` & `rpe-lib-3.0.3/rpe/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe/engines/opa.py` & `rpe-lib-3.0.3/rpe/engines/opa.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe/engines/python.py` & `rpe-lib-3.0.3/rpe/engines/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,17 @@
 
 from dataclasses import asdict
 
 from rpe.policy import Evaluation, EvaluationResult, Policy
 
 
 class PythonPolicyEngine:
-
     counter = 0
 
     def __init__(self, package_path):
-
         self._policies = {}
         self.package_path = package_path
         PythonPolicyEngine.counter += 1
         self.package_name = "rpe.plugins.policies.py_" + str(PythonPolicyEngine.counter)
 
         self._load_policies()
 
@@ -81,15 +79,14 @@
 
         # Loop over policy and build evals, so we can catch exceptions
 
         evals = []
 
         for policy_name, policy_cls in matched_policies.items():
             try:
-
                 if hasattr(policy_cls, "evaluate"):
                     eval_result = policy_cls.evaluate(resource)
                     if not isinstance(eval_result, EvaluationResult):
                         raise ValueError(
                             'Python policy "evaluate" function must return an EvaluationResult object'
                         )
```

### Comparing `rpe-lib-3.0.2/rpe/exceptions.py` & `rpe-lib-3.0.3/rpe/exceptions.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe/extractors/__init__.py` & `rpe-lib-3.0.3/rpe/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe/extractors/gcp_auditlogs.py` & `rpe-lib-3.0.3/rpe/extractors/gcp_auditlogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,14 @@
         return ExtractedResources(
             resources=resources,
             metadata=metadata,
         )
 
     @classmethod
     def is_audit_log(cls, message_data):
-
         log_type = jmespath.search('protoPayload."@type"', message_data)
         log_name = message_data.get("logName", "")
 
         # normal activity logs have logName in this form:
         #  projects/<p>/logs/cloudaudit.googleapis.com%2Factivity
         # data access logs have a logName field that looks like:
         #  projects/<p>/logs/cloudaudit.googleapis.com%2Fdata_access
@@ -79,15 +78,14 @@
                 log_type == "type.googleapis.com/google.cloud.audit.AuditLog",
                 log_name.split("/")[-1].startswith("cloudaudit.googleapis.com"),
             ]
         )
 
     @classmethod
     def get_metadata(cls, message_data):
-
         method_name = jmespath.search("protoPayload.methodName", message_data)
         insert_id = message_data.get("insertId")
 
         log_timestamp = message_data.get("timestamp")
         timestamp = dateutil.parser.parse(log_timestamp)
 
         principal_email = jmespath.search(
@@ -102,15 +100,14 @@
             method_name=method_name,
             operation=operation,
             principal=principal_email,
         )
 
     @classmethod
     def get_operation_type(cls, method_name):
-
         last = method_name.split(".")[-1].lower()
         # For batch methods, look for the verb after the word 'batch'
         if last.startswith("batch"):
             last = last[5:]
 
         read_prefixes = ("get", "list")
         if last.startswith(read_prefixes):
@@ -144,15 +141,14 @@
         if last.startswith(delete_prefixes):
             return "delete"
 
         return None
 
     @classmethod
     def get_resources(cls, message):
-
         resources = []
 
         res_type = jmespath.search("resource.type", message)
         if res_type is None:
             return resources
 
         # just shortening the many calls to jmespath throughout this function
@@ -166,15 +162,14 @@
             resources.append(res)
 
         method_name = prop("protoPayload.methodName")
 
         if res_type == "cloudsql_database" and method_name.startswith(
             "cloudsql.instances"
         ):
-
             resource_data = {
                 "resource_type": "sqladmin.googleapis.com/Instance",
                 # CloudSQL logs are inconsistent. See https://issuetracker.google.com/issues/137629452
                 "name": (
                     prop("resource.labels.database_id").split(":")[-1]
                     or prop("protoPayload.request.body.name")
                     or prop("protoPayload.request.resource.instanceName.instanceId")
@@ -229,15 +224,14 @@
             add_resource()
 
         elif res_type == "audited_resource" and (
             "EnableService" in method_name
             or "DisableService" in method_name
             or "ctivateService" in method_name
         ):
-
             resource_data = {
                 "resource_type": "serviceusage.googleapis.com/Service",
                 "project_id": prop("resource.labels.project_id"),
             }
 
             # Check if multiple services were included in the request
             # The Google Cloud Console generates (De)activate calls that logs a different format so we check both
@@ -294,15 +288,14 @@
                 "app": instance_data[1],
                 "service": instance_data[3],
                 "version": instance_data[5],
             }
             add_resource()
 
         elif res_type == "gce_instance":
-
             instance_name = prop("protoPayload.resourceName").split("/")[-1]
 
             resource_data = {
                 "resource_type": "compute.googleapis.com/Instance",
                 "name": instance_name,
                 "location": prop("resource.labels.zone"),
                 "project_id": prop("resource.labels.project_id"),
@@ -317,15 +310,14 @@
 
             add_resource()
 
             # Also add disk resources since theres not a separate log message for these
             disks = prop("protoPayload.request.disks") or []
 
             for disk in disks:
-
                 # The name of the disk is complicated. If the diskName is set in initParams use that
                 # If not AND its the boot disk, use the instance name
                 # Otherwise use the device name
 
                 disk_name = jmespath.search("initializeParams.diskName", disk)
                 device_name = jmespath.search("deviceName", disk)
                 boot = jmespath.search("boot", disk)
@@ -429,8 +421,26 @@
                 "name": name_bits[5],
                 "project_id": name_bits[1],
                 "location": name_bits[3],
                 "resource_type": "datafusion.googleapis.com/Instance",
             }
             add_resource()
 
+        elif (
+            res_type == "audited_resource"
+            and prop("resource.labels.service") == "dataform.googleapis.com"
+        ):
+            name_bits = prop("protoPayload.resourceName").split("/")
+            resource_data = {
+                "name": name_bits[len(name_bits) - 1],
+                "project_id": name_bits[1],
+                "location": name_bits[3],
+            }
+            if len(name_bits) == 6 and name_bits[4] == "repositories":
+                resource_data["resource_type"] = "dataform.googleapis.com/Repository"
+                add_resource()
+            elif len(name_bits) == 8 and name_bits[6] == "workspaces":
+                resource_data["resource_type"] = "dataform.googleapis.com/Workspace"
+                resource_data["repository"] = name_bits[4]
+                add_resource()
+
         return resources
```

### Comparing `rpe-lib-3.0.2/rpe/extractors/micromanager.py` & `rpe-lib-3.0.3/rpe/extractors/micromanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 class MicromanagerMetadata(PubsubMessageMetadata, ExtractedMetadata):
     pass
 
 
 class MicromanagerEvaluationRequest(Extractor):
     @classmethod
     def extract(cls, message):
-
         message_data = json.loads(message.data)
 
         name = message_data.get("name")
         asset_type = message_data.get("asset_type")
         project_id = message_data.get("project_id")
         metadata = message_data.get("metadata") or {}
         metadata.update((get_pubsub_message_metadata(message)).dict())
```

### Comparing `rpe-lib-3.0.2/rpe/extractors/models.py` & `rpe-lib-3.0.3/rpe/extractors/models.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe/extractors/pubsub_metadata.py` & `rpe-lib-3.0.3/rpe/extractors/pubsub_metadata.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe/policy.py` & `rpe-lib-3.0.3/rpe/policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     policy_id: str
 
 
 # To support python policies building their own evaluation, we need a class
 # that has the results of an eval without details about what triggered it
 @dataclass
 class EvaluationResult:
-
     compliant: bool
     remediable: bool
 
     # Static attributes on a given policy
     # Examples: severity, description, owner, etc.
     policy_attributes: Optional[Dict[str, Any]] = field(default_factory=dict)
```

### Comparing `rpe-lib-3.0.2/rpe/resources/__init__.py` & `rpe-lib-3.0.3/rpe/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe/resources/__init__.pyc` & `rpe-lib-3.0.3/rpe/resources/__init__.pyc`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe/resources/base.py` & `rpe-lib-3.0.3/rpe/resources/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 
 from abc import ABC, abstractmethod
 
 
 class Resource(ABC):
-
     # Returns a dictionary representing the resource. Must contain a 'type' key
     # indicating what type of resource it is
     @abstractmethod
     def get(self):
         pass
 
     # Performs remediation based on a json representation of how to remediate a
```

### Comparing `rpe-lib-3.0.2/rpe/resources/gcp.py` & `rpe-lib-3.0.3/rpe/resources/gcp.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     is_retryable_exception,
 )
 
 from .base import Resource
 
 
 class GoogleAPIResource(Resource):
-
     # Names of the get method of the root resource
     get_method = "get"
     required_resource_data = ["name"]
 
     # jmespath expression for getting labels
     resource_labels_path = "resource.labels"
 
@@ -52,15 +51,14 @@
     readiness_key = None
     readiness_value = None
     readiness_terminal_values = []
 
     inferred_data_map = None
 
     def __init__(self, client_kwargs=None, http=None, **resource_data):
-
         if client_kwargs is None:
             client_kwargs = {}
 
         self._http = http
         # Set some defaults
         self._service = None
         self._resource_metadata = None
@@ -74,15 +72,14 @@
         self._client_kwargs = client_kwargs
 
         self._ancestry = None
 
     def _validate_resource_data(self):
         """Verify we have all the required data for this resource"""
         if not all(arg in self._resource_data for arg in self.required_resource_data):
-
             raise ResourceException(
                 "Missing data required for resource creation. Expected data: {}; Got: {}".format(
                     ",".join(self.required_resource_data),
                     ",".join(self._resource_data.keys()),
                 )
             )
 
@@ -100,28 +97,34 @@
             "app": r"/apps/([^\/]+)/",
             "service": r"/services/([^\/]+)/",
             "version": r"/versions/([^\/]+)/",
             #  NodePools
             "cluster": r"/clusters/([^\/]+)/",
             # ServiceAccounts
             "service_account": r"serviceAccounts/([^\/]+)/",
+            # Dataform repository, used to query dataform workspaces
+            "repository": r"/repositories/([^\/]+)/",
         }
 
         resource_data = {}
 
         # Extract available resource data from resource name
         for field_name in fields:
             m = re.search(fields[field_name], name)
             if m:
                 resource_data[field_name] = m.group(1)
 
         return resource_data
 
     @classmethod
     def subclass_by_type(cls, resource_type):
+        # maps resource_type to the actual resource for cai events and audit log events
+        # cai events use the from_cai_data method to pass in the asset_type, which is used to map to the resource
+        # audit log events use from_resource_data from_resource_data to pass in the resource_type,
+        # which is used to map to the resource
         mapper = {res_cls.resource_type: res_cls for res_cls in cls.__subclasses__()}
 
         try:
             return mapper[resource_type]
         except KeyError:
             raise ResourceException(
                 "Unrecognized resource type: {}".format(resource_type)
@@ -152,15 +155,14 @@
         # if the project_id was passed, and its wasnt found in the resource name, add it
         if project_id and "project_id" not in resource_data:
             resource_data["project_id"] = project_id
 
         return res_cls(client_kwargs=client_kwargs, http=http, **resource_data)
 
     def to_dict(self):
-
         self._refresh_inferred_data()
 
         details = self._resource_data.copy()
         details.update(
             {
                 "resource_type": self.resource_type,
             }
@@ -171,15 +173,14 @@
         except Exception:
             details["full_resource_name"] = None
 
         return details
 
     # Some useful resource data may not be available when instantiated
     def _refresh_inferred_data(self):
-
         if not self.inferred_data_map:
             return
 
         try:
             resource_metadata = self.get(refresh=False)["resource"]
         except Exception:
             return
@@ -206,15 +207,14 @@
     # resources. None of the API's seem to implement it (except Cloud Asset
     # Inventory). This attempts to generate it from the discovery-based api
     # client's generated http request url.
     #
     # If we inject it into the resource, we can use it in policy evaluation to
     # simplify the structure of our policies
     def gen_full_resource_name(self):
-
         method = getattr(self.service, self.get_method)
         uri = method(**self._get_request_args()).uri
 
         uri_parsed = urlparse(uri)
         domain = uri_parsed.netloc
         path_segments = uri_parsed.path[1:].split("/")
 
@@ -289,15 +289,14 @@
 
         method = getattr(self.service, method_name)
 
         component_metadata = method(**req_arg_method()).execute()
         return component_metadata
 
     def get(self, refresh=True):
-
         if not refresh and self._resource_metadata:
             return self._resource_metadata
 
         method = getattr(self.service, self.get_method)
 
         # If the resource has readiness criteria, wait for it
         if self.readiness_key and self.readiness_value:
@@ -406,24 +405,22 @@
 
     @property
     def client_kwargs(self):
         return self._client_kwargs
 
     @client_kwargs.setter
     def client_kwargs(self, client_kwargs):
-
         # Invalidate service/parent because client_kwargs changed
         self._service = None
 
         self._client_kwargs = client_kwargs
 
     @property
     def service(self):
         if self._service is None:
-
             full_resource_path = "{}.{}".format(self.service_name, self.resource_path)
             self._service = build_subresource(
                 full_resource_path, self.version, **self._client_kwargs, http=self._http
             )
         return self._service
 
     @property
@@ -458,15 +455,14 @@
     def uniquifier(self):
         self._refresh_inferred_data()
 
         return self._resource_data.get("uniquifier")
 
 
 class GcpAppEngineInstance(GoogleAPIResource):
-
     service_name = "appengine"
     resource_path = "apps.services.versions.instances"
     version = "v1"
     readiness_key = "vmStatus"
     readiness_value = "RUNNING"
 
     resource_type = "appengine.googleapis.com/Instance"  # this is made-up based on existing appengine types
@@ -483,15 +479,14 @@
             "servicesId": self._resource_data["service"],
             "versionsId": self._resource_data["version"],
             "instancesId": self._resource_data["name"],
         }
 
 
 class GcpBigqueryDataset(GoogleAPIResource):
-
     service_name = "bigquery"
     resource_path = "datasets"
     version = "v2"
 
     required_resource_data = ["name", "project_id"]
 
     resource_type = "bigquery.googleapis.com/Dataset"
@@ -504,15 +499,14 @@
         return {
             "datasetId": self._resource_data["name"],
             "projectId": self._resource_data["project_id"],
         }
 
 
 class GcpBigtableInstance(GoogleAPIResource):
-
     service_name = "bigtableadmin"
     resource_path = "projects.instances"
     version = "v2"
     readiness_key = "state"
     readiness_value = "READY"
 
     resource_components = {
@@ -535,15 +529,14 @@
             "resource": "projects/{}/instances/{}".format(
                 self._resource_data["project_id"], self._resource_data["name"]
             ),
         }
 
 
 class GcpCloudFunction(GoogleAPIResource):
-
     service_name = "cloudfunctions"
     resource_path = "projects.locations.functions"
     version = "v1"
 
     resource_components = {
         "iam": "getIamPolicy",
     }
@@ -576,15 +569,14 @@
                 self._resource_data["location"],
                 self._resource_data["name"],
             ),
         }
 
 
 class GcpComputeInstance(GoogleAPIResource):
-
     service_name = "compute"
     resource_path = "instances"
     version = "v1"
 
     required_resource_data = ["name", "location", "project_id"]
 
     resource_type = "compute.googleapis.com/Instance"
@@ -598,15 +590,14 @@
             "instance": self._resource_data["name"],
             "zone": self._resource_data["location"],
             "project": self._resource_data["project_id"],
         }
 
 
 class GcpComputeDisk(GoogleAPIResource):
-
     service_name = "compute"
     resource_path = "disks"
     version = "v1"
 
     required_resource_data = ["name", "location", "project_id"]
 
     resource_type = "compute.googleapis.com/Disk"
@@ -620,15 +611,14 @@
             "project": self._resource_data["project_id"],
             "zone": self._resource_data["location"],
             "disk": self._resource_data["name"],
         }
 
 
 class GcpComputeRegionDisk(GoogleAPIResource):
-
     service_name = "compute"
     resource_path = "regionDisks"
     version = "v1"
 
     required_resource_data = ["name", "location", "project_id"]
 
     resource_type = "compute.googleapis.com/RegionDisk"
@@ -642,15 +632,14 @@
             "project": self._resource_data["project_id"],
             "region": self._resource_data["location"],
             "disk": self._resource_data["name"],
         }
 
 
 class GcpComputeNetwork(GoogleAPIResource):
-
     service_name = "compute"
     resource_path = "networks"
     version = "v1"
 
     required_resource_data = ["name", "project_id"]
 
     resource_type = "compute.googleapis.com/Network"
@@ -663,15 +652,14 @@
         return {
             "project": self._resource_data["project_id"],
             "network": self._resource_data["name"],
         }
 
 
 class GcpComputeSubnetwork(GoogleAPIResource):
-
     service_name = "compute"
     resource_path = "subnetworks"
     version = "v1"
 
     required_resource_data = ["name", "location", "project_id"]
 
     resource_type = "compute.googleapis.com/Subnetwork"
@@ -685,15 +673,14 @@
             "project": self._resource_data["project_id"],
             "region": self._resource_data["location"],
             "subnetwork": self._resource_data["name"],
         }
 
 
 class GcpComputeFirewall(GoogleAPIResource):
-
     service_name = "compute"
     resource_path = "firewalls"
     version = "v1"
 
     required_resource_data = ["name", "project_id"]
 
     resource_type = "compute.googleapis.com/Firewall"
@@ -767,15 +754,14 @@
                 self._resource_data["location"],
                 self._resource_data["name"],
             )
         }
 
 
 class GcpGkeCluster(GoogleAPIResource):
-
     service_name = "container"
     resource_path = "projects.locations.clusters"
     version = "v1"
     readiness_key = "status"
     readiness_value = "RUNNING"
     readiness_terminal_values = ["ERROR", "DEGRADED", "STOPPING", "STATUS_UNSPECIFIED"]
 
@@ -796,15 +782,14 @@
                 self._resource_data["location"],
                 self._resource_data["name"],
             )
         }
 
 
 class GcpGkeClusterNodepool(GoogleAPIResource):
-
     service_name = "container"
     resource_path = "projects.locations.clusters.nodePools"
     version = "v1"
     readiness_key = "status"
     readiness_value = "RUNNING"
     readiness_terminal_values = [
         "ERROR",
@@ -825,15 +810,14 @@
                 self._resource_data["cluster"],
                 self._resource_data["name"],
             )
         }
 
 
 class GcpIamServiceAccount(GoogleAPIResource):
-
     service_name = "iam"
     resource_path = "projects.serviceAccounts"
     version = "v1"
 
     required_resource_data = ["name", "project_id"]
 
     resource_type = "iam.googleapis.com/ServiceAccount"
@@ -847,15 +831,14 @@
             "name": "projects/{}/serviceAccounts/{}".format(
                 self._resource_data["project_id"], self._resource_data["name"]
             )
         }
 
 
 class GcpIamServiceAccountKey(GoogleAPIResource):
-
     service_name = "iam"
     resource_path = "projects.serviceAccounts.keys"
     version = "v1"
 
     required_resource_data = ["name", "service_account", "project_id"]
 
     resource_type = "iam.googleapis.com/ServiceAccountKey"
@@ -871,15 +854,14 @@
                 self._resource_data["service_account"],
                 self._resource_data["name"],
             )
         }
 
 
 class GcpPubsubSubscription(GoogleAPIResource):
-
     service_name = "pubsub"
     resource_path = "projects.subscriptions"
     version = "v1"
 
     required_resource_data = ["name", "project_id"]
 
     resource_components = {
@@ -900,15 +882,14 @@
             "resource": "projects/{}/subscriptions/{}".format(
                 self._resource_data["project_id"], self._resource_data["name"]
             )
         }
 
 
 class GcpPubsubTopic(GoogleAPIResource):
-
     service_name = "pubsub"
     resource_path = "projects.topics"
     version = "v1"
 
     required_resource_data = ["name", "project_id"]
 
     resource_components = {
@@ -929,15 +910,14 @@
             "resource": "projects/{}/topics/{}".format(
                 self._resource_data["project_id"], self._resource_data["name"]
             )
         }
 
 
 class GcpStorageBucket(GoogleAPIResource):
-
     service_name = "storage"
     resource_path = "buckets"
     version = "v1"
 
     resource_components = {
         "iam": "getIamPolicy",
     }
@@ -954,15 +934,14 @@
     def _get_request_args(self):
         return {
             "bucket": self._resource_data["name"],
         }
 
 
 class GcpSqlInstance(GoogleAPIResource):
-
     service_name = "sqladmin"
     resource_path = "instances"
     version = "v1beta4"
     readiness_key = "state"
     readiness_value = "RUNNABLE"
     readiness_terminal_values = ["FAILED", "MAINTENANCE", "SUSPENDED", "UNKNOWN_STATE"]
 
@@ -974,15 +953,14 @@
         return {
             "instance": self._resource_data["name"],
             "project": self._resource_data["project_id"],
         }
 
 
 class GcpOrganization(GoogleAPIResource):
-
     service_name = "cloudresourcemanager"
     resource_path = "organizations"
     version = "v1"
 
     resource_components = {
         "iam": "getIamPolicy",
     }
@@ -993,15 +971,14 @@
         return {"name": "organizations/" + self._resource_data["name"]}
 
     def _get_iam_request_args(self):
         return {"resource": "organizations/" + self._resource_data["name"]}
 
 
 class GcpProject(GoogleAPIResource):
-
     service_name = "cloudresourcemanager"
     resource_path = "projects"
     version = "v1"
 
     resource_components = {
         "iam": "getIamPolicy",
     }
@@ -1016,15 +993,14 @@
         return {"projectId": self._resource_data["name"]}
 
     def _get_iam_request_args(self):
         return {"resource": self._resource_data["name"], "body": {}}
 
 
 class GcpProjectService(GoogleAPIResource):
-
     service_name = "serviceusage"
     resource_path = "services"
     version = "v1"
 
     required_resource_data = ["name", "project_id"]
 
     resource_type = "serviceusage.googleapis.com/Service"
@@ -1034,15 +1010,14 @@
             "name": "projects/{}/services/{}".format(
                 self._resource_data["project_id"], self._resource_data["name"]
             )
         }
 
 
 class GcpDataflowJob(GoogleAPIResource):
-
     service_name = "dataflow"
     resource_path = "projects.locations.jobs"
     version = "v1b3"
 
     required_resource_data = ["name", "project_id", "location"]
 
     resource_type = "dataflow.googleapis.com/Job"
@@ -1057,15 +1032,14 @@
             "projectId": self._resource_data["project_id"],
             "location": self._resource_data["location"],
             "view": "JOB_VIEW_DESCRIPTION",
         }
 
 
 class GcpRedisInstance(GoogleAPIResource):
-
     service_name = "redis"
     resource_path = "projects.locations.instances"
     version = "v1"
 
     readiness_key = "state"
     readiness_value = "READY"
     readiness_terminal_values = ["DELETING", "STATE_UNSPECIFIED"]
@@ -1085,15 +1059,14 @@
                 self._resource_data["location"],
                 self._resource_data["name"],
             ),
         }
 
 
 class GcpMemcacheInstance(GoogleAPIResource):
-
     service_name = "memcache"
     resource_path = "projects.locations.instances"
     version = "v1"
 
     readiness_key = "state"
     readiness_value = "READY"
     readiness_terminal_values = ["DELETING", "STATE_UNSPECIFIED"]
@@ -1110,7 +1083,66 @@
         return {
             "name": "projects/{}/locations/{}/instances/{}".format(
                 self._resource_data["project_id"],
                 self._resource_data["location"],
                 self._resource_data["name"],
             ),
         }
+
+
+class GcpDataformRepository(GoogleAPIResource):
+    service_name = "dataform"
+    resource_path = "projects.locations.repositories"
+    version = "v1beta1"
+
+    required_resource_data = ["name", "location", "project_id"]
+
+    resource_components = {
+        "iam": "getIamPolicy",
+    }
+
+    resource_type = "dataform.googleapis.com/Repository"
+
+    inferred_data_map = {
+        "uniquifier": "createTime",
+    }
+
+    def _get_resource_string(self):
+        return "projects/{}/locations/{}/repositories/{}".format(
+            self._resource_data["project_id"],
+            self._resource_data["location"],
+            self._resource_data["name"],
+        )
+
+    def _get_request_args(self):
+        return {"name": self._get_resource_string()}
+
+    def _get_iam_request_args(self):
+        return {"resource": self._get_resource_string()}
+
+
+class GcpDataformWorkspace(GoogleAPIResource):
+    service_name = "dataform"
+    resource_path = "projects.locations.repositories.workspaces"
+    version = "v1beta1"
+
+    required_resource_data = ["name", "location", "project_id", "repository"]
+
+    resource_components = {
+        "iam": "getIamPolicy",
+    }
+
+    resource_type = "dataform.googleapis.com/Workspace"
+
+    def _get_resource_string(self):
+        return "projects/{}/locations/{}/repositories/{}/workspaces/{}".format(
+            self._resource_data["project_id"],
+            self._resource_data["location"],
+            self._resource_data["repository"],
+            self._resource_data["name"],
+        )
+
+    def _get_request_args(self):
+        return {"name": self._get_resource_string()}
+
+    def _get_iam_request_args(self):
+        return {"resource": self._get_resource_string()}
```

### Comparing `rpe-lib-3.0.2/rpe/rpe.py` & `rpe-lib-3.0.3/rpe/rpe.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/rpe_lib.egg-info/PKG-INFO` & `rpe-lib-3.0.3/rpe_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpe-lib
-Version: 3.0.2
+Version: 3.0.3
 Summary: A resource policy evaluation library
 Home-page: https://github.com/cleardataeng/resource-policy-evaluation-library
 Author: Joe Ceresini
 License: Apache 2.0
 Description: # resource-policy-evaluation-library
         
         rpe-lib is made up of `Policy Engines (rpe.engines.Engine)`, `Resources (rpe.resources.Resource)`, and `Extractors (rpe.resources.Extractor)`.
```

### Comparing `rpe-lib-3.0.2/rpe_lib.egg-info/SOURCES.txt` & `rpe-lib-3.0.3/rpe_lib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -133,14 +133,17 @@
 tests/data/compute_instance_creation_logs_4.json
 tests/data/compute_instance_creation_logs_5.json
 tests/data/compute_instance_micromanager.json
 tests/data/compute_networks_insert_1.json
 tests/data/compute_networks_insert_2.json
 tests/data/compute_networks_insert_3.json
 tests/data/dataflow-job-step.json
+tests/data/dataform-create-repository.json
+tests/data/dataform-create-workspace.json
+tests/data/dataform-update-repository.json
 tests/data/datafusion-create-instance.json
 tests/data/datafusion-update-instance.json
 tests/data/dataproc_createcluster.json
 tests/data/gke-cluster-update.json
 tests/data/gke-nodepool-set.json
 tests/data/memorystore-redis.json
 tests/data/project_get_iam.json
```

### Comparing `rpe-lib-3.0.2/setup.py` & `rpe-lib-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/__init__.py` & `rpe-lib-3.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/app-engine-debug.json` & `rpe-lib-3.0.3/tests/data/app-engine-debug.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/bigtable-set-iam-policy.json` & `rpe-lib-3.0.3/tests/data/bigtable-set-iam-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/bq-ds-set-iam-policy.json` & `rpe-lib-3.0.3/tests/data/bq-ds-set-iam-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/cloudfunctions-set-iam-policy.json` & `rpe-lib-3.0.3/tests/data/cloudfunctions-set-iam-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/cloudsql-protoPayload.request.body.json` & `rpe-lib-3.0.3/tests/data/cloudsql-protoPayload.request.body.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/cloudsql-protoPayload.request.resource.instanceName.instanceId.json` & `rpe-lib-3.0.3/tests/data/cloudsql-protoPayload.request.resource.instanceName.instanceId.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/cloudsql-resource.labels.json` & `rpe-lib-3.0.3/tests/data/cloudsql-resource.labels.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute-firewalls-enable-logs-policy.json` & `rpe-lib-3.0.3/tests/data/compute-firewalls-enable-logs-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute-hardened-images.json` & `rpe-lib-3.0.3/tests/data/compute-hardened-images.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute-subnetworks-enable-flow-logs.json` & `rpe-lib-3.0.3/tests/data/compute-subnetworks-enable-flow-logs.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute-subnetworks-set-private-ip-google-access.json` & `rpe-lib-3.0.3/tests/data/compute-subnetworks-set-private-ip-google-access.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute_instance_creation_logs_1.json` & `rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_1.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute_instance_creation_logs_2.json` & `rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_2.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute_instance_creation_logs_3.json` & `rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_3.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute_instance_creation_logs_4.json` & `rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_4.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute_instance_creation_logs_5.json` & `rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_5.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute_networks_insert_1.json` & `rpe-lib-3.0.3/tests/data/compute_networks_insert_1.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute_networks_insert_2.json` & `rpe-lib-3.0.3/tests/data/compute_networks_insert_2.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/compute_networks_insert_3.json` & `rpe-lib-3.0.3/tests/data/compute_networks_insert_3.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/dataflow-job-step.json` & `rpe-lib-3.0.3/tests/data/dataflow-job-step.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/datafusion-create-instance.json` & `rpe-lib-3.0.3/tests/data/datafusion-create-instance.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/datafusion-update-instance.json` & `rpe-lib-3.0.3/tests/data/datafusion-update-instance.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/dataproc_createcluster.json` & `rpe-lib-3.0.3/tests/data/dataproc_createcluster.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/gke-cluster-update.json` & `rpe-lib-3.0.3/tests/data/gke-cluster-update.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/gke-nodepool-set.json` & `rpe-lib-3.0.3/tests/data/gke-nodepool-set.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/memorystore-redis.json` & `rpe-lib-3.0.3/tests/data/memorystore-redis.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/project_get_iam.json` & `rpe-lib-3.0.3/tests/data/project_get_iam.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/project_set_iam.json` & `rpe-lib-3.0.3/tests/data/project_set_iam.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/pubsub-subscription-set-iam-policy.json` & `rpe-lib-3.0.3/tests/data/pubsub-subscription-set-iam-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/pubsub-topic-set-iam-policy.json` & `rpe-lib-3.0.3/tests/data/pubsub-topic-set-iam-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/servicemanagement-activate-service.json` & `rpe-lib-3.0.3/tests/data/servicemanagement-activate-service.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/servicemanagement-deactivate-service.json` & `rpe-lib-3.0.3/tests/data/servicemanagement-deactivate-service.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/servicemanagement-disable-service.json` & `rpe-lib-3.0.3/tests/data/servicemanagement-disable-service.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/servicemanagement-enable-service.json` & `rpe-lib-3.0.3/tests/data/servicemanagement-enable-service.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/serviceusage-batchenable.json` & `rpe-lib-3.0.3/tests/data/serviceusage-batchenable.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/serviceusage-disable.json` & `rpe-lib-3.0.3/tests/data/serviceusage-disable.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/serviceusage-enable.json` & `rpe-lib-3.0.3/tests/data/serviceusage-enable.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/storage_bucket_delete.json` & `rpe-lib-3.0.3/tests/data/storage_bucket_delete.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/data/storage_bucket_update.json` & `rpe-lib-3.0.3/tests/data/storage_bucket_update.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/test_extractors.py` & `rpe-lib-3.0.3/tests/test_extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,32 @@
     ("dataflow-job-step.json", "dataflow.googleapis.com/Job", "create", "job-id"),
     (
         "memorystore-redis.json",
         "redis.googleapis.com/Instance",
         "create",
         "test-instance",
     ),
+    (
+        "dataform-create-repository.json",
+        "dataform.googleapis.com/Repository",
+        "create",
+        "test-repository",
+    ),
+    (
+        "dataform-create-workspace.json",
+        "dataform.googleapis.com/Workspace",
+        "create",
+        "test-workspace",
+    ),
+    (
+        "dataform-update-repository.json",
+        "dataform.googleapis.com/Repository",
+        "update",
+        "test-repository",
+    ),
 ]
 
 test_micromanager_log = [
     (
         "compute_instance_micromanager.json",
         "test-instance",
         GcpComputeInstance,
```

### Comparing `rpe-lib-3.0.2/tests/test_gcp_resource_inferred_data.py` & `rpe-lib-3.0.3/tests/test_gcp_resource_inferred_data.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.2/tests/test_resources.py` & `rpe-lib-3.0.3/tests/test_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     GcpComputeDisk,
     GcpComputeFirewall,
     GcpComputeInstance,
     GcpComputeSubnetwork,
     GcpDataflowJob,
     GcpDatafusionInstance,
     GcpDataprocCluster,
+    GcpDataformRepository,
+    GcpDataformWorkspace,
     GcpGkeCluster,
     GcpGkeClusterNodepool,
     GcpMemcacheInstance,
     GcpOrganization,
     GcpProject,
     GcpProjectService,
     GcpPubsubSubscription,
@@ -432,14 +434,49 @@
             [
                 ({"status": 200}, '{"createTime":"createTime"}'),
                 ({"status": 200}, "{}"),
             ]
         ),
         uniquifier="createTime",
     ),
+    ResourceTestCase(
+        resource_data={
+            "name": test_resource_name,
+            "location": "us-central1",
+            "project_id": test_project,
+        },
+        cls=GcpDataformRepository,
+        resource_type="dataform.googleapis.com/Repository",
+        name="//dataform.googleapis.com/projects/my_project/locations/us-central1/repositories/my_resource",
+        http=HttpMockSequence(
+            [
+                ({"status": 200}, '{"createTime":"createTime"}'),
+                ({"status": 200}, "{}"),
+            ]
+        ),
+        uniquifier="createTime",
+    ),
+    ResourceTestCase(
+        resource_data={
+            "name": test_resource_name,
+            "location": "us-central1",
+            "project_id": test_project,
+            "repository": "test_repository",
+        },
+        cls=GcpDataformWorkspace,
+        resource_type="dataform.googleapis.com/Workspace",
+        name="//dataform.googleapis.com/projects/my_project/locations/us-central1/repositories/test_repository/workspaces/test_resource_name",
+        http=HttpMockSequence(
+            [
+                ({"status": 200}, '{"createTime":"createTime"}'),
+                ({"status": 200}, "{}"),
+            ]
+        ),
+        uniquifier="createTime",
+    ),
 ]
 
 
 @pytest.mark.parametrize(
     "case", test_cases, ids=[case.cls.__name__ for case in test_cases]
 )
 def test_gcp_from_resource(case):
@@ -488,15 +525,14 @@
         **case.resource_data
     )
     assert r.location == case.resource_data.get("location")
 
 
 def test_missing_resource_data():
     with pytest.raises(ResourceException) as excinfo:
-
         GcpAppEngineInstance(name=test_resource_name)
 
     assert "Missing data required for resource creation" in str(excinfo.value)
 
 
 def test_gcp_to_dict():
     r = GoogleAPIResource.from_resource_data(
```

### Comparing `rpe-lib-3.0.2/tests/test_resources_cai.py` & `rpe-lib-3.0.3/tests/test_resources_cai.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     GcpComputeFirewall,
     GcpComputeInstance,
     GcpComputeRegionDisk,
     GcpComputeSubnetwork,
     GcpDataflowJob,
     GcpDatafusionInstance,
     GcpDataprocCluster,
+    GcpDataformRepository,
+    GcpDataformWorkspace,
     GcpGkeCluster,
     GcpGkeClusterNodepool,
     GcpIamServiceAccount,
     GcpIamServiceAccountKey,
     GcpMemcacheInstance,
     GcpOrganization,
     GcpProject,
@@ -224,14 +226,28 @@
     CaiTestCase(
         data={
             "name": "//memcache.googleapis.com/projects/test-project/locations/us-central1/instances/test-resource",
             "asset_type": "memcache.googleapis.com/Instance",
         },
         resource_cls=GcpMemcacheInstance,
     ),
+    CaiTestCase(
+        data={
+            "name": "//dataform.googleapis.com/projects/test-project/locations/us-central1/repositories/test-resource",
+            "asset_type": "dataform.googleapis.com/Repository",
+        },
+        resource_cls=GcpDataformRepository,
+    ),
+    CaiTestCase(
+        data={
+            "name": "//dataform.googleapis.com/projects/test-project/locations/us-central1/repositories/test-repository/workspaces/test-resource",
+            "asset_type": "dataform.googleapis.com/Workspace",
+        },
+        resource_cls=GcpDataformWorkspace,
+    ),
 ]
 
 
 @pytest.mark.parametrize(
     "case", test_cases, ids=[case.resource_cls.__name__ for case in test_cases]
 )
 def test_gcp_resource_from_cai_data(case):
@@ -241,15 +257,14 @@
         client_kwargs=client_kwargs,
     )
     assert r.__class__ == case.resource_cls
     assert r.full_resource_name() == case.data.get("name")
 
 
 def test_bad_resource_type():
-
     with pytest.raises(ResourceException) as excinfo:
         GoogleAPIResource.from_cai_data(
             "//cloudfakeservice.googleapis.com/widgets/test-resource",
             "cloudfakeservice.googleapis.com/Widget",
             client_kwargs=client_kwargs,
         )
```

