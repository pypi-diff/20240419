# Comparing `tmp/pulumiverse_exoscale-0.56.0.tar.gz` & `tmp/pulumiverse_exoscale-0.57.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_exoscale-0.56.0.tar", last modified: Sun Mar  3 20:47:37 2024, max compression
+gzip compressed data, was "pulumiverse_exoscale-0.57.0.tar", last modified: Fri Apr 19 01:46:55 2024, max compression
```

## Comparing `pulumiverse_exoscale-0.56.0.tar` & `pulumiverse_exoscale-0.57.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:47:37.897314 pulumiverse_exoscale-0.56.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-03 20:47:37.897314 pulumiverse_exoscale-0.56.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:47:37.897314 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    86391 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    59185 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    53981 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/compute_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:47:37.897314 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    44465 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    19826 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_compute_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_compute_instance_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_compute_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_compute_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_database_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_iam_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_iam_org_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_iam_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_iamapi_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_instance_pool_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_nlb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_nlb_service_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_private_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    19972 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_sks_cluster_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_sks_nodepool_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)    16908 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/iam_access_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/iam_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/iam_org_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16323 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/iam_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/iamapi_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    53550 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    37861 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    21070 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/nic.py
--rw-r--r--   0 runner    (1001) docker     (127)    16554 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/nlb.py
--rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/nlb_service.py
--rw-r--r--   0 runner    (1001) docker     (127)   135733 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/private_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/secondary_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    40730 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/security_group_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/security_group_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    23739 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/sks_kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    44736 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/ssh_keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 20:47:37.897314 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/pulumiverse_exoscale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 20:47:37.897314 pulumiverse_exoscale-0.56.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-03 20:47:37.000000 pulumiverse_exoscale-0.56.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86391 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59185 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54141 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/compute_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44469 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13350 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19986 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21444 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14811 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_instance_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_database_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_org_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iamapi_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_instance_pool_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_nlb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_nlb_service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21258 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15270 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_cluster_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_nodepool_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17064 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_org_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16323 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iamapi_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53710 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37861 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21070 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16712 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nlb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26879 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nlb_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136459 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20265 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/secondary_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12016 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40890 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45736 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23739 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44896 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ssh_keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 01:46:55.000000 pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 01:46:55.317381 pulumiverse_exoscale-0.57.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-19 01:46:54.000000 pulumiverse_exoscale-0.57.0/setup.py
```

### Comparing `pulumiverse_exoscale-0.56.0/PKG-INFO` & `pulumiverse_exoscale-0.57.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_exoscale
-Version: 0.56.0
+Version: 0.57.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_exoscale-0.56.0/README.md` & `pulumiverse_exoscale-0.57.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/__init__.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/_inputs.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/_utilities.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/affinity.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/affinity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/anti_affinity_group.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/anti_affinity_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,35 +102,37 @@
         """
         Manage Exoscale [Anti-Affinity Groups](https://community.exoscale.com/documentation/compute/anti-affinity-groups/).
 
         Corresponding data source: exoscale_anti_affinity_group.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_anti_affinity_group = exoscale.AntiAffinityGroup("myAntiAffinityGroup", description="Prevent compute instances to run on the same host")
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing anti-affinity group may be imported by `<ID>`:
 
         ```sh
         $ pulumi import exoscale:index/antiAffinityGroup:AntiAffinityGroup \\
         ```
 
-         exoscale_anti_affinity_group.my_anti_affinity_group \\
+          exoscale_anti_affinity_group.my_anti_affinity_group \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: ❗ A free-form text describing the group.
         :param pulumi.Input[str] name: ❗ The anti-affinity group name.
         """
         ...
@@ -142,35 +144,37 @@
         """
         Manage Exoscale [Anti-Affinity Groups](https://community.exoscale.com/documentation/compute/anti-affinity-groups/).
 
         Corresponding data source: exoscale_anti_affinity_group.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_anti_affinity_group = exoscale.AntiAffinityGroup("myAntiAffinityGroup", description="Prevent compute instances to run on the same host")
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing anti-affinity group may be imported by `<ID>`:
 
         ```sh
         $ pulumi import exoscale:index/antiAffinityGroup:AntiAffinityGroup \\
         ```
 
-         exoscale_anti_affinity_group.my_anti_affinity_group \\
+          exoscale_anti_affinity_group.my_anti_affinity_group \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param AntiAffinityGroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/compute.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/compute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/compute_instance.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/compute_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -701,42 +701,44 @@
 
         Corresponding data sources: exoscale_compute_instance, exoscale_compute_instance_list.
 
         After the creation, you can retrieve the password of an instance with [Exoscale CLI](https://github.com/exoscale/cli): `exo compute instance reveal-password NAME`.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_exoscale as exoscale
         import pulumiverse_exoscale as exoscale
 
         my_template = exoscale.get_template(zone="ch-gva-2",
             name="Linux Ubuntu 22.04 LTS 64-bit")
         my_instance = exoscale.ComputeInstance("myInstance",
             zone="ch-gva-2",
             template_id=my_template.id,
             type="standard.medium",
             disk_size=10)
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing compute instance may be imported by `<ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/computeInstance:ComputeInstance \\
         ```
 
-         exoscale_compute_instance.my_instance \\
+          exoscale_compute_instance.my_instance \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: ❗ A list of exoscale*anti*affinity_group (IDs) to attach to the instance (may only be set at creation time).
         :param pulumi.Input[str] deploy_target_id: ❗ A deploy target ID.
         :param pulumi.Input[bool] destroy_protected: Mark the instance as protected, the Exoscale API will refuse to delete the instance until the protection is removed (boolean; default: `false`).
         :param pulumi.Input[int] disk_size: The instance disk size (GiB; at least `10`). Can not be decreased after creation. **WARNING**: updating this attribute stops/restarts the instance.
@@ -766,42 +768,44 @@
 
         Corresponding data sources: exoscale_compute_instance, exoscale_compute_instance_list.
 
         After the creation, you can retrieve the password of an instance with [Exoscale CLI](https://github.com/exoscale/cli): `exo compute instance reveal-password NAME`.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_exoscale as exoscale
         import pulumiverse_exoscale as exoscale
 
         my_template = exoscale.get_template(zone="ch-gva-2",
             name="Linux Ubuntu 22.04 LTS 64-bit")
         my_instance = exoscale.ComputeInstance("myInstance",
             zone="ch-gva-2",
             template_id=my_template.id,
             type="standard.medium",
             disk_size=10)
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing compute instance may be imported by `<ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/computeInstance:ComputeInstance \\
         ```
 
-         exoscale_compute_instance.my_instance \\
+          exoscale_compute_instance.my_instance \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param ComputeInstanceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/config/vars.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/database.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -621,17 +621,17 @@
 
         An existing database service may be imported by `<name>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/database:Database \\
         ```
 
-         exoscale_database.my_database \\
+          exoscale_database.my_database \\
 
-         my-database@ch-gva-2
+          my-database@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['DatabaseGrafanaArgs']] grafana: *grafana* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[pulumi.InputType['DatabaseKafkaArgs']] kafka: *kafka* database service type specific arguments. Structure is documented below.
         :param pulumi.Input[str] maintenance_dow: The day of week to perform the automated database service maintenance (`never`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`).
         :param pulumi.Input[str] maintenance_time: The time of day to perform the automated database service maintenance (`HH:MM:SS`)
@@ -658,17 +658,17 @@
 
         An existing database service may be imported by `<name>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/database:Database \\
         ```
 
-         exoscale_database.my_database \\
+          exoscale_database.my_database \\
 
-         my-database@ch-gva-2
+          my-database@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param DatabaseArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/domain.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,37 +157,39 @@
         """
         Manage Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domains.
 
         Corresponding data source: exoscale_domain.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_domain = exoscale.Domain("myDomain")
         ```
+        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_domain_record(s) to the domain.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing DNS domain may be imported by `ID`:
 
         ```sh
         $ pulumi import exoscale:index/domain:Domain \\
         ```
 
-         exoscale_domain.my_domain \\
+          exoscale_domain.my_domain \\
 
-         89083a5c-b648-474a-0000-0000000f67bd
+          89083a5c-b648-474a-0000-0000000f67bd
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: ❗ The DNS domain name.
         """
         ...
     @overload
@@ -198,37 +200,39 @@
         """
         Manage Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domains.
 
         Corresponding data source: exoscale_domain.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_domain = exoscale.Domain("myDomain")
         ```
+        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_domain_record(s) to the domain.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing DNS domain may be imported by `ID`:
 
         ```sh
         $ pulumi import exoscale:index/domain:Domain \\
         ```
 
-         exoscale_domain.my_domain \\
+          exoscale_domain.my_domain \\
 
-         89083a5c-b648-474a-0000-0000000f67bd
+          89083a5c-b648-474a-0000-0000000f67bd
 
         :param str resource_name: The name of the resource.
         :param DomainArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/domain_record.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/domain_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,43 +263,45 @@
         """
         Manage Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domain Records.
 
         Corresponding data source: exoscale_domain_record.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_domain = exoscale.Domain("myDomain")
         my_host = exoscale.DomainRecord("myHost",
             domain=my_domain.id,
             record_type="A",
             content="1.2.3.4")
         my_host_alias = exoscale.DomainRecord("myHostAlias",
             domain=my_domain.id,
             record_type="CNAME",
             content=my_host.hostname)
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing DNS domain record may be imported by `<ID>`:
 
         ```sh
         $ pulumi import exoscale:index/domainRecord:DomainRecord \\
         ```
 
-         exoscale_domain_record.my_host \\
+          exoscale_domain_record.my_host \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] content: The record value.
         :param pulumi.Input[str] domain: ❗ The parent Domain to attach the record to.
         :param pulumi.Input[str] name: The record name, Leave blank (`""`) to create a root record (similar to using `@` in a DNS zone file).
         :param pulumi.Input[int] prio: The record priority (for types that support it; minimum `0`).
@@ -315,43 +317,45 @@
         """
         Manage Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domain Records.
 
         Corresponding data source: exoscale_domain_record.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_domain = exoscale.Domain("myDomain")
         my_host = exoscale.DomainRecord("myHost",
             domain=my_domain.id,
             record_type="A",
             content="1.2.3.4")
         my_host_alias = exoscale.DomainRecord("myHostAlias",
             domain=my_domain.id,
             record_type="CNAME",
             content=my_host.hostname)
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing DNS domain record may be imported by `<ID>`:
 
         ```sh
         $ pulumi import exoscale:index/domainRecord:DomainRecord \\
         ```
 
-         exoscale_domain_record.my_host \\
+          exoscale_domain_record.my_host \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param DomainRecordArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/elastic_ip.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/elastic_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,23 +269,26 @@
 
         Corresponding data source: exoscale_elastic_ip.
 
         ## Example Usage
 
         *Unmanaged* EIPv4:
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_elastic_ip = exoscale.ElasticIp("myElasticIp", zone="ch-gva-2")
         ```
+        <!--End PulumiCodeChooser -->
 
         *Managed* EIPv6:
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_managed_elastic_ip = exoscale.ElasticIp("myManagedElasticIp",
             address_family="inet6",
             healthcheck=exoscale.ElasticIpHealthcheckArgs(
@@ -297,29 +300,30 @@
                 timeout=3,
                 tls_sni="example.net",
                 uri="/health",
             ),
             reverse_dns="example.net",
             zone="ch-gva-2")
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing Elastic IP (EIP) may be imported by `<ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/elasticIp:ElasticIp \\
         ```
 
-         exoscale_elastic_ip.my_elastic_ip \\
+          exoscale_elastic_ip.my_elastic_ip \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address_family: ❗ The Elastic IP (EIP) address family (`inet4` or `inet6`; default: `inet4`).
         :param pulumi.Input[str] description: A free-form text describing the Elastic IP (EIP).
         :param pulumi.Input[pulumi.InputType['ElasticIpHealthcheckArgs']] healthcheck: Healthcheck configuration for *managed* EIPs. It can not be added to an existing *Unmanaged* EIP.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
@@ -337,23 +341,26 @@
 
         Corresponding data source: exoscale_elastic_ip.
 
         ## Example Usage
 
         *Unmanaged* EIPv4:
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_elastic_ip = exoscale.ElasticIp("myElasticIp", zone="ch-gva-2")
         ```
+        <!--End PulumiCodeChooser -->
 
         *Managed* EIPv6:
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_managed_elastic_ip = exoscale.ElasticIp("myManagedElasticIp",
             address_family="inet6",
             healthcheck=exoscale.ElasticIpHealthcheckArgs(
@@ -365,29 +372,30 @@
                 timeout=3,
                 tls_sni="example.net",
                 uri="/health",
             ),
             reverse_dns="example.net",
             zone="ch-gva-2")
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing Elastic IP (EIP) may be imported by `<ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/elasticIp:ElasticIp \\
         ```
 
-         exoscale_elastic_ip.my_elastic_ip \\
+          exoscale_elastic_ip.my_elastic_ip \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param ElasticIpArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_affinity.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_affinity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_anti_affinity_group.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_anti_affinity_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,21 +74,23 @@
     """
     Fetch Exoscale [Anti-Affinity Groups](https://community.exoscale.com/documentation/compute/anti-affinity-groups/) data.
 
     Corresponding resource: exoscale_anti_affinity_group.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_anti_affinity_group = exoscale.get_anti_affinity_group(name="my-anti-affinity-group")
     pulumi.export("myAntiAffinityGroupId", my_anti_affinity_group.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The anti-affinity group ID to match (conflicts with `name`).
     :param str name: The group name to match (conflicts with `id`).
@@ -112,21 +114,23 @@
     """
     Fetch Exoscale [Anti-Affinity Groups](https://community.exoscale.com/documentation/compute/anti-affinity-groups/) data.
 
     Corresponding resource: exoscale_anti_affinity_group.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_anti_affinity_group = exoscale.get_anti_affinity_group(name="my-anti-affinity-group")
     pulumi.export("myAntiAffinityGroupId", my_anti_affinity_group.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The anti-affinity group ID to match (conflicts with `name`).
     :param str name: The group name to match (conflicts with `id`).
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_compute.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_compute_instance.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,22 +303,24 @@
     """
     Fetch Exoscale [Compute Instances](https://community.exoscale.com/documentation/compute/) data.
 
     Corresponding resource: exoscale_compute_instance.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_instance = exoscale.get_compute_instance(zone="ch-gva-2",
         name="my-instance")
     pulumi.export("myInstanceId", my_instance.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The compute instance ID to match (conflicts with `name`).
     :param str name: The instance name to match (conflicts with `id`).
@@ -364,22 +366,24 @@
     """
     Fetch Exoscale [Compute Instances](https://community.exoscale.com/documentation/compute/) data.
 
     Corresponding resource: exoscale_compute_instance.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_instance = exoscale.get_compute_instance(zone="ch-gva-2",
         name="my-instance")
     pulumi.export("myInstanceId", my_instance.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The compute instance ID to match (conflicts with `name`).
     :param str name: The instance name to match (conflicts with `id`).
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_compute_instance_list.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_instance_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_compute_ip_address.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_compute_template.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_compute_template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_database_uri.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_database_uri.py`

 * *Files 9% similar despite different names*

```diff
@@ -105,15 +105,16 @@
 
 def get_database_uri(name: Optional[str] = None,
                      timeouts: Optional[pulumi.InputType['GetDatabaseUriTimeoutsArgs']] = None,
                      type: Optional[str] = None,
                      zone: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDatabaseUriResult:
     """
-    Use this data source to access information about an existing resource.
+    ## Example Usage
+
 
     :param str name: The database name to match.
     :param str type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
     :param str zone: The Exoscale Zone name.
     """
     __args__ = dict()
     __args__['name'] = name
@@ -135,14 +136,15 @@
 @_utilities.lift_output_func(get_database_uri)
 def get_database_uri_output(name: Optional[pulumi.Input[str]] = None,
                             timeouts: Optional[pulumi.Input[Optional[pulumi.InputType['GetDatabaseUriTimeoutsArgs']]]] = None,
                             type: Optional[pulumi.Input[str]] = None,
                             zone: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseUriResult]:
     """
-    Use this data source to access information about an existing resource.
+    ## Example Usage
+
 
     :param str name: The database name to match.
     :param str type: The type of the database service (`kafka`, `mysql`, `opensearch`, `pg`, `redis`).
     :param str zone: The Exoscale Zone name.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_domain.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_domain.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,21 +61,23 @@
     """
     Fetch Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domains data.
 
     Corresponding resource: exoscale_domain.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_domain = exoscale.get_domain(name="my.domain")
     pulumi.export("myDomainId", my_domain.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str name: The DNS domain name to match.
     """
@@ -95,21 +97,23 @@
     """
     Fetch Exoscale [DNS](https://community.exoscale.com/documentation/dns/) Domains data.
 
     Corresponding resource: exoscale_domain.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_domain = exoscale.get_domain(name="my.domain")
     pulumi.export("myDomainId", my_domain.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str name: The DNS domain name to match.
     """
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_domain_record.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_elastic_ip.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_elastic_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,22 +149,24 @@
     """
     Fetch Exoscale [Elastic IPs (EIP)](https://community.exoscale.com/documentation/compute/eip/) data.
 
     Corresponding resource: exoscale_elastic_ip.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_elastic_ip = exoscale.get_elastic_ip(zone="ch-gva-2",
         ip_address="1.2.3.4")
     pulumi.export("myElasticIpId", my_elastic_ip.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The Elastic IP (EIP) ID to match (conflicts with `ip_address` and `labels`).
     :param str ip_address: The EIP IPv4 or IPv6 address to match (conflicts with `id` and `labels`).
@@ -200,22 +202,24 @@
     """
     Fetch Exoscale [Elastic IPs (EIP)](https://community.exoscale.com/documentation/compute/eip/) data.
 
     Corresponding resource: exoscale_elastic_ip.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_elastic_ip = exoscale.get_elastic_ip(zone="ch-gva-2",
         ip_address="1.2.3.4")
     pulumi.export("myElasticIpId", my_elastic_ip.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The Elastic IP (EIP) ID to match (conflicts with `ip_address` and `labels`).
     :param str ip_address: The EIP IPv4 or IPv6 address to match (conflicts with `id` and `labels`).
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_iam_api_key.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_iam_org_policy.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_org_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_iam_role.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iam_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_iamapi_key.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_iamapi_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_instance_pool.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_instance_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,22 +281,24 @@
     """
     Fetch Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/) data.
 
     Corresponding resource: exoscale_instance_pool.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_instance_pool = exoscale.get_instance_pool(zone="ch-gva-2",
         name="my-instance-pool")
     pulumi.export("myInstancePoolId", my_instance_pool.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param Mapping[str, str] labels: A map of key/value labels.
     :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
@@ -341,22 +343,24 @@
     """
     Fetch Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/) data.
 
     Corresponding resource: exoscale_instance_pool.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_instance_pool = exoscale.get_instance_pool(zone="ch-gva-2",
         name="my-instance-pool")
     pulumi.export("myInstancePoolId", my_instance_pool.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param Mapping[str, str] labels: A map of key/value labels.
     :param str zone: The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_instance_pool_list.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_instance_pool_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_network.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_nlb.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_nlb.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,22 +123,24 @@
     """
     Fetch Exoscale [Network Load Balancers (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/) data.
 
     Corresponding resource: exoscale_nlb.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_nlb = exoscale.get_nlb(zone="ch-gva-2",
         name="my-nlb")
     pulumi.export("myNlbId", my_nlb.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The Network Load Balancers (NLB) ID to match (conflicts with `name`).
     :param str name: The NLB name to match (conflicts with `id`).
@@ -169,22 +171,24 @@
     """
     Fetch Exoscale [Network Load Balancers (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/) data.
 
     Corresponding resource: exoscale_nlb.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_nlb = exoscale.get_nlb(zone="ch-gva-2",
         name="my-nlb")
     pulumi.export("myNlbId", my_nlb.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The Network Load Balancers (NLB) ID to match (conflicts with `name`).
     :param str name: The NLB name to match (conflicts with `id`).
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_nlb_service_list.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_nlb_service_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_private_network.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_private_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,22 +137,24 @@
     """
     Fetch Exoscale [Private Networks](https://community.exoscale.com/documentation/compute/private-networks/) data.
 
     Corresponding resource: exoscale_private_network.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_private_network = exoscale.get_private_network(zone="ch-gva-2",
         name="my-private-network")
     pulumi.export("myPrivateNetworkId", my_private_network.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str description: The private network description.
     :param str id: The private network ID to match (conflicts with `name`).
@@ -190,22 +192,24 @@
     """
     Fetch Exoscale [Private Networks](https://community.exoscale.com/documentation/compute/private-networks/) data.
 
     Corresponding resource: exoscale_private_network.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_private_network = exoscale.get_private_network(zone="ch-gva-2",
         name="my-private-network")
     pulumi.export("myPrivateNetworkId", my_private_network.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str description: The private network description.
     :param str id: The private network ID to match (conflicts with `name`).
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_security_group.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_security_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,21 +74,23 @@
     """
     Fetch Exoscale [Security Groups](https://community.exoscale.com/documentation/compute/security-groups/) data.
 
     Corresponding resource: exoscale_security_group.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_security_group = exoscale.get_security_group(name="my-security-group")
     pulumi.export("mySecurityGroupId", my_security_group.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The security group ID to match (conflicts with `name`)
     :param str name: The name to match (conflicts with `id`)
@@ -112,21 +114,23 @@
     """
     Fetch Exoscale [Security Groups](https://community.exoscale.com/documentation/compute/security-groups/) data.
 
     Corresponding resource: exoscale_security_group.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_security_group = exoscale.get_security_group(name="my-security-group")
     pulumi.export("mySecurityGroupId", my_security_group.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The security group ID to match (conflicts with `name`)
     :param str name: The name to match (conflicts with `id`)
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_sks_cluster.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 
 @pulumi.output_type
 class GetSksClusterResult:
     """
     A collection of values returned by getSksCluster.
     """
-    def __init__(__self__, addons=None, aggregation_ca=None, auto_upgrade=None, cni=None, control_plane_ca=None, created_at=None, description=None, endpoint=None, exoscale_ccm=None, id=None, kubelet_ca=None, labels=None, metrics_server=None, name=None, nodepools=None, oidc=None, service_level=None, state=None, version=None, zone=None):
+    def __init__(__self__, addons=None, aggregation_ca=None, auto_upgrade=None, cni=None, control_plane_ca=None, created_at=None, description=None, endpoint=None, exoscale_ccm=None, exoscale_csi=None, id=None, kubelet_ca=None, labels=None, metrics_server=None, name=None, nodepools=None, oidc=None, service_level=None, state=None, version=None, zone=None):
         if addons and not isinstance(addons, list):
             raise TypeError("Expected argument 'addons' to be a list")
         pulumi.set(__self__, "addons", addons)
         if aggregation_ca and not isinstance(aggregation_ca, str):
             raise TypeError("Expected argument 'aggregation_ca' to be a str")
         pulumi.set(__self__, "aggregation_ca", aggregation_ca)
         if auto_upgrade and not isinstance(auto_upgrade, bool):
@@ -47,14 +47,17 @@
         pulumi.set(__self__, "description", description)
         if endpoint and not isinstance(endpoint, str):
             raise TypeError("Expected argument 'endpoint' to be a str")
         pulumi.set(__self__, "endpoint", endpoint)
         if exoscale_ccm and not isinstance(exoscale_ccm, bool):
             raise TypeError("Expected argument 'exoscale_ccm' to be a bool")
         pulumi.set(__self__, "exoscale_ccm", exoscale_ccm)
+        if exoscale_csi and not isinstance(exoscale_csi, bool):
+            raise TypeError("Expected argument 'exoscale_csi' to be a bool")
+        pulumi.set(__self__, "exoscale_csi", exoscale_csi)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if kubelet_ca and not isinstance(kubelet_ca, str):
             raise TypeError("Expected argument 'kubelet_ca' to be a str")
         pulumi.set(__self__, "kubelet_ca", kubelet_ca)
         if labels and not isinstance(labels, dict):
@@ -154,14 +157,22 @@
     def exoscale_ccm(self) -> Optional[bool]:
         """
         Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "exoscale_ccm")
 
     @property
+    @pulumi.getter(name="exoscaleCsi")
+    def exoscale_csi(self) -> Optional[bool]:
+        """
+        Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
+        """
+        return pulumi.get(self, "exoscale_csi")
+
+    @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         The ID of this resource.
         """
         return pulumi.get(self, "id")
 
@@ -251,14 +262,15 @@
             auto_upgrade=self.auto_upgrade,
             cni=self.cni,
             control_plane_ca=self.control_plane_ca,
             created_at=self.created_at,
             description=self.description,
             endpoint=self.endpoint,
             exoscale_ccm=self.exoscale_ccm,
+            exoscale_csi=self.exoscale_csi,
             id=self.id,
             kubelet_ca=self.kubelet_ca,
             labels=self.labels,
             metrics_server=self.metrics_server,
             name=self.name,
             nodepools=self.nodepools,
             oidc=self.oidc,
@@ -273,14 +285,15 @@
                     auto_upgrade: Optional[bool] = None,
                     cni: Optional[str] = None,
                     control_plane_ca: Optional[str] = None,
                     created_at: Optional[str] = None,
                     description: Optional[str] = None,
                     endpoint: Optional[str] = None,
                     exoscale_ccm: Optional[bool] = None,
+                    exoscale_csi: Optional[bool] = None,
                     id: Optional[str] = None,
                     kubelet_ca: Optional[str] = None,
                     labels: Optional[Mapping[str, str]] = None,
                     metrics_server: Optional[bool] = None,
                     name: Optional[str] = None,
                     nodepools: Optional[Sequence[str]] = None,
                     oidc: Optional[pulumi.InputType['GetSksClusterOidcArgs']] = None,
@@ -296,14 +309,15 @@
     :param bool auto_upgrade: Enable automatic upgrading of the control plane version.
     :param str cni: The CNI plugin that is to be used. Available options are "calico" or "cilium". Defaults to "calico". Setting empty string will result in a cluster with no CNI.
     :param str control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
     :param str created_at: The cluster creation date.
     :param str description: A free-form text describing the cluster.
     :param str endpoint: The cluster API endpoint.
     :param bool exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
+    :param bool exoscale_csi: Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
     :param str id: The ID of this resource.
     :param str kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
     :param Mapping[str, str] labels: A map of key/value labels.
     :param bool metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
     :param Sequence[str] nodepools: The list of exoscale*sks*nodepool (IDs) attached to the cluster.
     :param pulumi.InputType['GetSksClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
     :param str service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
@@ -316,14 +330,15 @@
     __args__['autoUpgrade'] = auto_upgrade
     __args__['cni'] = cni
     __args__['controlPlaneCa'] = control_plane_ca
     __args__['createdAt'] = created_at
     __args__['description'] = description
     __args__['endpoint'] = endpoint
     __args__['exoscaleCcm'] = exoscale_ccm
+    __args__['exoscaleCsi'] = exoscale_csi
     __args__['id'] = id
     __args__['kubeletCa'] = kubelet_ca
     __args__['labels'] = labels
     __args__['metricsServer'] = metrics_server
     __args__['name'] = name
     __args__['nodepools'] = nodepools
     __args__['oidc'] = oidc
@@ -340,14 +355,15 @@
         auto_upgrade=pulumi.get(__ret__, 'auto_upgrade'),
         cni=pulumi.get(__ret__, 'cni'),
         control_plane_ca=pulumi.get(__ret__, 'control_plane_ca'),
         created_at=pulumi.get(__ret__, 'created_at'),
         description=pulumi.get(__ret__, 'description'),
         endpoint=pulumi.get(__ret__, 'endpoint'),
         exoscale_ccm=pulumi.get(__ret__, 'exoscale_ccm'),
+        exoscale_csi=pulumi.get(__ret__, 'exoscale_csi'),
         id=pulumi.get(__ret__, 'id'),
         kubelet_ca=pulumi.get(__ret__, 'kubelet_ca'),
         labels=pulumi.get(__ret__, 'labels'),
         metrics_server=pulumi.get(__ret__, 'metrics_server'),
         name=pulumi.get(__ret__, 'name'),
         nodepools=pulumi.get(__ret__, 'nodepools'),
         oidc=pulumi.get(__ret__, 'oidc'),
@@ -363,14 +379,15 @@
                            auto_upgrade: Optional[pulumi.Input[Optional[bool]]] = None,
                            cni: Optional[pulumi.Input[Optional[str]]] = None,
                            control_plane_ca: Optional[pulumi.Input[Optional[str]]] = None,
                            created_at: Optional[pulumi.Input[Optional[str]]] = None,
                            description: Optional[pulumi.Input[Optional[str]]] = None,
                            endpoint: Optional[pulumi.Input[Optional[str]]] = None,
                            exoscale_ccm: Optional[pulumi.Input[Optional[bool]]] = None,
+                           exoscale_csi: Optional[pulumi.Input[Optional[bool]]] = None,
                            id: Optional[pulumi.Input[Optional[str]]] = None,
                            kubelet_ca: Optional[pulumi.Input[Optional[str]]] = None,
                            labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                            metrics_server: Optional[pulumi.Input[Optional[bool]]] = None,
                            name: Optional[pulumi.Input[Optional[str]]] = None,
                            nodepools: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                            oidc: Optional[pulumi.Input[Optional[pulumi.InputType['GetSksClusterOidcArgs']]]] = None,
@@ -386,14 +403,15 @@
     :param bool auto_upgrade: Enable automatic upgrading of the control plane version.
     :param str cni: The CNI plugin that is to be used. Available options are "calico" or "cilium". Defaults to "calico". Setting empty string will result in a cluster with no CNI.
     :param str control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
     :param str created_at: The cluster creation date.
     :param str description: A free-form text describing the cluster.
     :param str endpoint: The cluster API endpoint.
     :param bool exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
+    :param bool exoscale_csi: Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
     :param str id: The ID of this resource.
     :param str kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
     :param Mapping[str, str] labels: A map of key/value labels.
     :param bool metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
     :param Sequence[str] nodepools: The list of exoscale*sks*nodepool (IDs) attached to the cluster.
     :param pulumi.InputType['GetSksClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
     :param str service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_sks_cluster_list.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_cluster_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetSksClusterListResult:
     """
     A collection of values returned by getSksClusterList.
     """
-    def __init__(__self__, aggregation_ca=None, auto_upgrade=None, clusters=None, cni=None, control_plane_ca=None, created_at=None, description=None, endpoint=None, exoscale_ccm=None, id=None, kubelet_ca=None, labels=None, metrics_server=None, name=None, service_level=None, state=None, version=None, zone=None):
+    def __init__(__self__, aggregation_ca=None, auto_upgrade=None, clusters=None, cni=None, control_plane_ca=None, created_at=None, description=None, endpoint=None, exoscale_ccm=None, exoscale_csi=None, id=None, kubelet_ca=None, labels=None, metrics_server=None, name=None, service_level=None, state=None, version=None, zone=None):
         if aggregation_ca and not isinstance(aggregation_ca, str):
             raise TypeError("Expected argument 'aggregation_ca' to be a str")
         pulumi.set(__self__, "aggregation_ca", aggregation_ca)
         if auto_upgrade and not isinstance(auto_upgrade, bool):
             raise TypeError("Expected argument 'auto_upgrade' to be a bool")
         pulumi.set(__self__, "auto_upgrade", auto_upgrade)
         if clusters and not isinstance(clusters, list):
@@ -46,14 +46,17 @@
         pulumi.set(__self__, "description", description)
         if endpoint and not isinstance(endpoint, str):
             raise TypeError("Expected argument 'endpoint' to be a str")
         pulumi.set(__self__, "endpoint", endpoint)
         if exoscale_ccm and not isinstance(exoscale_ccm, bool):
             raise TypeError("Expected argument 'exoscale_ccm' to be a bool")
         pulumi.set(__self__, "exoscale_ccm", exoscale_ccm)
+        if exoscale_csi and not isinstance(exoscale_csi, bool):
+            raise TypeError("Expected argument 'exoscale_csi' to be a bool")
+        pulumi.set(__self__, "exoscale_csi", exoscale_csi)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if kubelet_ca and not isinstance(kubelet_ca, str):
             raise TypeError("Expected argument 'kubelet_ca' to be a str")
         pulumi.set(__self__, "kubelet_ca", kubelet_ca)
         if labels and not isinstance(labels, dict):
@@ -144,14 +147,22 @@
     def exoscale_ccm(self) -> Optional[bool]:
         """
         Match against this bool
         """
         return pulumi.get(self, "exoscale_ccm")
 
     @property
+    @pulumi.getter(name="exoscaleCsi")
+    def exoscale_csi(self) -> Optional[bool]:
+        """
+        Match against this bool
+        """
+        return pulumi.get(self, "exoscale_csi")
+
+    @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Match against this string. If you supply a string that begins and ends with a "/" it will be matched as a regex.
         """
         return pulumi.get(self, "id")
 
@@ -231,14 +242,15 @@
             clusters=self.clusters,
             cni=self.cni,
             control_plane_ca=self.control_plane_ca,
             created_at=self.created_at,
             description=self.description,
             endpoint=self.endpoint,
             exoscale_ccm=self.exoscale_ccm,
+            exoscale_csi=self.exoscale_csi,
             id=self.id,
             kubelet_ca=self.kubelet_ca,
             labels=self.labels,
             metrics_server=self.metrics_server,
             name=self.name,
             service_level=self.service_level,
             state=self.state,
@@ -250,14 +262,15 @@
                          auto_upgrade: Optional[bool] = None,
                          cni: Optional[str] = None,
                          control_plane_ca: Optional[str] = None,
                          created_at: Optional[str] = None,
                          description: Optional[str] = None,
                          endpoint: Optional[str] = None,
                          exoscale_ccm: Optional[bool] = None,
+                         exoscale_csi: Optional[bool] = None,
                          id: Optional[str] = None,
                          kubelet_ca: Optional[str] = None,
                          labels: Optional[Mapping[str, str]] = None,
                          metrics_server: Optional[bool] = None,
                          name: Optional[str] = None,
                          service_level: Optional[str] = None,
                          state: Optional[str] = None,
@@ -272,14 +285,15 @@
     __args__['autoUpgrade'] = auto_upgrade
     __args__['cni'] = cni
     __args__['controlPlaneCa'] = control_plane_ca
     __args__['createdAt'] = created_at
     __args__['description'] = description
     __args__['endpoint'] = endpoint
     __args__['exoscaleCcm'] = exoscale_ccm
+    __args__['exoscaleCsi'] = exoscale_csi
     __args__['id'] = id
     __args__['kubeletCa'] = kubelet_ca
     __args__['labels'] = labels
     __args__['metricsServer'] = metrics_server
     __args__['name'] = name
     __args__['serviceLevel'] = service_level
     __args__['state'] = state
@@ -294,14 +308,15 @@
         clusters=pulumi.get(__ret__, 'clusters'),
         cni=pulumi.get(__ret__, 'cni'),
         control_plane_ca=pulumi.get(__ret__, 'control_plane_ca'),
         created_at=pulumi.get(__ret__, 'created_at'),
         description=pulumi.get(__ret__, 'description'),
         endpoint=pulumi.get(__ret__, 'endpoint'),
         exoscale_ccm=pulumi.get(__ret__, 'exoscale_ccm'),
+        exoscale_csi=pulumi.get(__ret__, 'exoscale_csi'),
         id=pulumi.get(__ret__, 'id'),
         kubelet_ca=pulumi.get(__ret__, 'kubelet_ca'),
         labels=pulumi.get(__ret__, 'labels'),
         metrics_server=pulumi.get(__ret__, 'metrics_server'),
         name=pulumi.get(__ret__, 'name'),
         service_level=pulumi.get(__ret__, 'service_level'),
         state=pulumi.get(__ret__, 'state'),
@@ -314,14 +329,15 @@
                                 auto_upgrade: Optional[pulumi.Input[Optional[bool]]] = None,
                                 cni: Optional[pulumi.Input[Optional[str]]] = None,
                                 control_plane_ca: Optional[pulumi.Input[Optional[str]]] = None,
                                 created_at: Optional[pulumi.Input[Optional[str]]] = None,
                                 description: Optional[pulumi.Input[Optional[str]]] = None,
                                 endpoint: Optional[pulumi.Input[Optional[str]]] = None,
                                 exoscale_ccm: Optional[pulumi.Input[Optional[bool]]] = None,
+                                exoscale_csi: Optional[pulumi.Input[Optional[bool]]] = None,
                                 id: Optional[pulumi.Input[Optional[str]]] = None,
                                 kubelet_ca: Optional[pulumi.Input[Optional[str]]] = None,
                                 labels: Optional[pulumi.Input[Optional[Mapping[str, str]]]] = None,
                                 metrics_server: Optional[pulumi.Input[Optional[bool]]] = None,
                                 name: Optional[pulumi.Input[Optional[str]]] = None,
                                 service_level: Optional[pulumi.Input[Optional[str]]] = None,
                                 state: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_sks_nodepool.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_nodepool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_sks_nodepool_list.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_sks_nodepool_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_template.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,22 +98,24 @@
                  zone: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTemplateResult:
     """
     Fetch Exoscale [Compute Instance Templates](https://community.exoscale.com/documentation/compute/custom-templates/) data.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_template = exoscale.get_template(zone="ch-gva-2",
         name="Linux Ubuntu 22.04 LTS 64-bit")
     pulumi.export("myTemplateId", my_template.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The compute instance template ID to match (conflicts with `name`).
     :param str name: The template name to match (conflicts with `id`) (when multiple templates have the same name, the newest one will be returned).
@@ -143,22 +145,24 @@
                         zone: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTemplateResult]:
     """
     Fetch Exoscale [Compute Instance Templates](https://community.exoscale.com/documentation/compute/custom-templates/) data.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     my_template = exoscale.get_template(zone="ch-gva-2",
         name="Linux Ubuntu 22.04 LTS 64-bit")
     pulumi.export("myTemplateId", my_template.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
 
 
     :param str id: The compute instance template ID to match (conflicts with `name`).
     :param str name: The template name to match (conflicts with `id`) (when multiple templates have the same name, the newest one will be returned).
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/get_zones.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/get_zones.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,21 +58,23 @@
 
 def get_zones(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetZonesResult:
     """
     Lists all zones.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     example_zones = exoscale.get_zones()
     pulumi.export("zonesOutput", example_zones.zones)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('exoscale:index/getZones:getZones', __args__, opts=opts, typ=GetZonesResult).value
@@ -85,19 +87,21 @@
 @_utilities.lift_output_func(get_zones)
 def get_zones_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetZonesResult]:
     """
     Lists all zones.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_exoscale as exoscale
 
     example_zones = exoscale.get_zones()
     pulumi.export("zonesOutput", example_zones.zones)
     ```
+    <!--End PulumiCodeChooser -->
 
     Please refer to the examples
     directory for complete configuration examples.
     """
     ...
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/iam_access_key.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_access_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,26 +208,28 @@
                  operations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  resources: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sos_access_key = exoscale.IamAccessKey("mySosAccessKey",
             operations=[
                 "get-sos-object",
                 "list-sos-bucket",
             ],
             resources=["sos/bucket:my-bucket"])
         my_sks_access_key = exoscale.IamAccessKey("mySksAccessKey", tags=["sks"])
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         > **NOTE:** You can retrieve the list of available operations and tags using the [Exoscale CLI](https://github.com/exoscale/cli/): `exo iam access-key list-operations`.
 
         :param str resource_name: The name of the resource.
@@ -242,26 +244,28 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[IamAccessKeyArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sos_access_key = exoscale.IamAccessKey("mySosAccessKey",
             operations=[
                 "get-sos-object",
                 "list-sos-bucket",
             ],
             resources=["sos/bucket:my-bucket"])
         my_sks_access_key = exoscale.IamAccessKey("mySksAccessKey", tags=["sks"])
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         > **NOTE:** You can retrieve the list of available operations and tags using the [Exoscale CLI](https://github.com/exoscale/cli/): `exo iam access-key list-operations`.
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/iam_api_key.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_api_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -154,28 +154,30 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  role_id: Optional[pulumi.Input[str]] = None,
                  timeouts: Optional[pulumi.Input[pulumi.InputType['IamApiKeyTimeoutsArgs']]] = None,
                  __props__=None):
         """
-        Create a IamApiKey resource with the given unique name, props, and options.
+        ## Example Usage
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: ❗ IAM API Key name.
         :param pulumi.Input[str] role_id: ❗ IAM API role ID.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IamApiKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a IamApiKey resource with the given unique name, props, and options.
+        ## Example Usage
+
         :param str resource_name: The name of the resource.
         :param IamApiKeyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(IamApiKeyArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/iam_org_policy.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_org_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,28 +121,30 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  default_service_strategy: Optional[pulumi.Input[str]] = None,
                  services: Optional[pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['IamOrgPolicyServicesArgs']]]]] = None,
                  timeouts: Optional[pulumi.Input[pulumi.InputType['IamOrgPolicyTimeoutsArgs']]] = None,
                  __props__=None):
         """
-        Create a IamOrgPolicy resource with the given unique name, props, and options.
+        ## Example Usage
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_service_strategy: Default service strategy (`allow` or `deny`).
         :param pulumi.Input[Mapping[str, pulumi.Input[pulumi.InputType['IamOrgPolicyServicesArgs']]]] services: IAM policy services.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IamOrgPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a IamOrgPolicy resource with the given unique name, props, and options.
+        ## Example Usage
+
         :param str resource_name: The name of the resource.
         :param IamOrgPolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(IamOrgPolicyArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/iam_role.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iam_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/iamapi_key.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/iamapi_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/instance_pool.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/instance_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -744,43 +744,45 @@
         """
         Manage Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/).
 
         Corresponding data sources: exoscale_instance_pool, exoscale_instance_pool_list.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_exoscale as exoscale
         import pulumiverse_exoscale as exoscale
 
         my_template = exoscale.get_template(zone="ch-gva-2",
             name="Linux Ubuntu 22.04 LTS 64-bit")
         my_instance_pool = exoscale.InstancePool("myInstancePool",
             zone="ch-gva-2",
             template_id=my_template.id,
             instance_type="standard.medium",
             disk_size=10,
             size=3)
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing instance pool may be imported by `<ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/instancePool:InstancePool \\
         ```
 
-         exoscale_instance_pool.my_instance_pool \\
+          exoscale_instance_pool.my_instance_pool \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] affinity_group_ids: A list of exoscale*anti*affinity_group (IDs; may only be set at creation time).
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
         :param pulumi.Input[int] disk_size: The managed instances disk size (GiB).
@@ -810,43 +812,45 @@
         """
         Manage Exoscale [Instance Pools](https://community.exoscale.com/documentation/compute/instance-pools/).
 
         Corresponding data sources: exoscale_instance_pool, exoscale_instance_pool_list.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_exoscale as exoscale
         import pulumiverse_exoscale as exoscale
 
         my_template = exoscale.get_template(zone="ch-gva-2",
             name="Linux Ubuntu 22.04 LTS 64-bit")
         my_instance_pool = exoscale.InstancePool("myInstancePool",
             zone="ch-gva-2",
             template_id=my_template.id,
             instance_type="standard.medium",
             disk_size=10,
             size=3)
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing instance pool may be imported by `<ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/instancePool:InstancePool \\
         ```
 
-         exoscale_instance_pool.my_instance_pool \\
+          exoscale_instance_pool.my_instance_pool \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param InstancePoolArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/ip_address.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/network.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/nic.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nic.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/nlb.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nlb.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,39 +231,41 @@
         """
         Manage Exoscale [Network Load Balancers (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/).
 
         Corresponding data source: exoscale_nlb.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_nlb = exoscale.Nlb("myNlb", zone="ch-gva-2")
         ```
+        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_nlb_service(s) to the NLB.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing network load balancer (NLB) may be imported by `<ID>@<zone>`:
 
-         console
+        console
 
         ```sh
         $ pulumi import exoscale:index/nlb:Nlb \\
         ```
 
-         exoscale_nlb.my_nlb \\
+          exoscale_nlb.my_nlb \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the NLB.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The network load balancer (NLB) name.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
@@ -277,39 +279,41 @@
         """
         Manage Exoscale [Network Load Balancers (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/).
 
         Corresponding data source: exoscale_nlb.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_nlb = exoscale.Nlb("myNlb", zone="ch-gva-2")
         ```
+        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_nlb_service(s) to the NLB.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing network load balancer (NLB) may be imported by `<ID>@<zone>`:
 
-         console
+        console
 
         ```sh
         $ pulumi import exoscale:index/nlb:Nlb \\
         ```
 
-         exoscale_nlb.my_nlb \\
+          exoscale_nlb.my_nlb \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param NlbArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/nlb_service.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/nlb_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,14 +372,15 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage Exoscale [Network Load Balancer (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/) Services.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_nlb = exoscale.Nlb("myNlb", zone="ch-gva-2")
         my_nlb_service = exoscale.NlbService("myNlbService",
             nlb_id=my_nlb.id,
@@ -395,29 +396,30 @@
                 uri="/healthz",
                 tls_sni="example.net",
                 interval=5,
                 timeout=3,
                 retries=1,
             )])
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing NLB service may be imported by `<nlb-ID>/<service-ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/nlbService:NlbService \\
         ```
 
-         exoscale_nlb_service.my_nlb_service \\
+          exoscale_nlb_service.my_nlb_service \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the NLB service.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NlbServiceHealthcheckArgs']]]] healthchecks: The service health checking configuration.
         :param pulumi.Input[str] instance_pool_id: ❗ The exoscale*instance*pool (ID) to forward traffic to.
         :param pulumi.Input[str] name: The NLB service name.
@@ -435,14 +437,15 @@
                  args: NlbServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage Exoscale [Network Load Balancer (NLB)](https://community.exoscale.com/documentation/compute/network-load-balancer/) Services.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_nlb = exoscale.Nlb("myNlb", zone="ch-gva-2")
         my_nlb_service = exoscale.NlbService("myNlbService",
             nlb_id=my_nlb.id,
@@ -458,29 +461,30 @@
                 uri="/healthz",
                 tls_sni="example.net",
                 interval=5,
                 timeout=3,
                 retries=1,
             )])
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing NLB service may be imported by `<nlb-ID>/<service-ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/nlbService:NlbService \\
         ```
 
-         exoscale_nlb_service.my_nlb_service \\
+          exoscale_nlb_service.my_nlb_service \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param NlbServiceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/outputs.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2983,14 +2983,15 @@
                  state: str,
                  version: str,
                  zone: str,
                  auto_upgrade: Optional[bool] = None,
                  cni: Optional[str] = None,
                  description: Optional[str] = None,
                  exoscale_ccm: Optional[bool] = None,
+                 exoscale_csi: Optional[bool] = None,
                  id: Optional[str] = None,
                  labels: Optional[Mapping[str, str]] = None,
                  metrics_server: Optional[bool] = None,
                  name: Optional[str] = None,
                  service_level: Optional[str] = None):
         """
         :param str aggregation_ca: The CA certificate (in PEM format) for TLS communications between the control plane and the aggregation layer (e.g. `metrics-server`).
@@ -3002,14 +3003,15 @@
         :param 'GetSksClusterListClusterOidcArgs' oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         :param str state: The cluster state.
         :param str version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
         :param bool auto_upgrade: Enable automatic upgrading of the control plane version.
         :param str cni: The CNI plugin that is to be used. Available options are "calico" or "cilium". Defaults to "calico". Setting empty string will result in a cluster with no CNI.
         :param str description: A free-form text describing the cluster.
         :param bool exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param bool exoscale_csi: Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
         :param Mapping[str, str] labels: A map of key/value labels.
         :param bool metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param str service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
         """
         pulumi.set(__self__, "addons", addons)
         pulumi.set(__self__, "aggregation_ca", aggregation_ca)
         pulumi.set(__self__, "control_plane_ca", control_plane_ca)
@@ -3025,14 +3027,16 @@
             pulumi.set(__self__, "auto_upgrade", auto_upgrade)
         if cni is not None:
             pulumi.set(__self__, "cni", cni)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if exoscale_ccm is not None:
             pulumi.set(__self__, "exoscale_ccm", exoscale_ccm)
+        if exoscale_csi is not None:
+            pulumi.set(__self__, "exoscale_csi", exoscale_csi)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if metrics_server is not None:
             pulumi.set(__self__, "metrics_server", metrics_server)
         if name is not None:
@@ -3154,14 +3158,22 @@
     def exoscale_ccm(self) -> Optional[bool]:
         """
         Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "exoscale_ccm")
 
     @property
+    @pulumi.getter(name="exoscaleCsi")
+    def exoscale_csi(self) -> Optional[bool]:
+        """
+        Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
+        """
+        return pulumi.get(self, "exoscale_csi")
+
+    @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[Mapping[str, str]]:
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/private_network.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/private_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,48 +268,52 @@
 
         Corresponding data source: exoscale_private_network.
 
         ## Example Usage
 
         *Unmanaged* private network:
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_private_network = exoscale.PrivateNetwork("myPrivateNetwork", zone="ch-gva-2")
         ```
+        <!--End PulumiCodeChooser -->
 
         *Managed* private network:
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_managed_private_network = exoscale.PrivateNetwork("myManagedPrivateNetwork",
             end_ip="10.0.0.253",
             netmask="255.255.255.0",
             start_ip="10.0.0.20",
             zone="ch-gva-2")
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing private network may be imported by `<ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/privateNetwork:PrivateNetwork \\
         ```
 
-         exoscale_private_network.my_private_network \\
+          exoscale_private_network.my_private_network \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: A free-form text describing the network.
         :param pulumi.Input[str] end_ip: (For managed Privnets) The first/last IPv4 addresses used by the DHCP service for dynamic leases.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[str] name: The private network name.
@@ -328,48 +332,52 @@
 
         Corresponding data source: exoscale_private_network.
 
         ## Example Usage
 
         *Unmanaged* private network:
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_private_network = exoscale.PrivateNetwork("myPrivateNetwork", zone="ch-gva-2")
         ```
+        <!--End PulumiCodeChooser -->
 
         *Managed* private network:
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_managed_private_network = exoscale.PrivateNetwork("myManagedPrivateNetwork",
             end_ip="10.0.0.253",
             netmask="255.255.255.0",
             start_ip="10.0.0.20",
             zone="ch-gva-2")
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing private network may be imported by `<ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/privateNetwork:PrivateNetwork \\
         ```
 
-         exoscale_private_network.my_private_network \\
+          exoscale_private_network.my_private_network \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param PrivateNetworkArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/provider.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/secondary_ip_address.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/secondary_ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/security_group.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,37 +135,39 @@
         """
         Manage Exoscale [Security Groups](https://community.exoscale.com/documentation/compute/security-groups/).
 
         Corresponding data source: exoscale_security_group.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_security_group = exoscale.SecurityGroup("mySecurityGroup")
         ```
+        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_security_group_rule(s) to the group.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing security group may be imported by `<ID>`:
 
         ```sh
         $ pulumi import exoscale:index/securityGroup:SecurityGroup \\
         ```
 
-         exoscale_security_group.my_security_group \\
+          exoscale_security_group.my_security_group \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: ❗ A free-form text describing the group.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] external_sources: A list of external network sources, in [CIDR](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notatio) notation.
         :param pulumi.Input[str] name: ❗ The security group name.
         """
@@ -178,37 +180,39 @@
         """
         Manage Exoscale [Security Groups](https://community.exoscale.com/documentation/compute/security-groups/).
 
         Corresponding data source: exoscale_security_group.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_security_group = exoscale.SecurityGroup("mySecurityGroup")
         ```
+        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_security_group_rule(s) to the group.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing security group may be imported by `<ID>`:
 
         ```sh
         $ pulumi import exoscale:index/securityGroup:SecurityGroup \\
         ```
 
-         exoscale_security_group.my_security_group \\
+          exoscale_security_group.my_security_group \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6
 
         :param str resource_name: The name of the resource.
         :param SecurityGroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/security_group_rule.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,42 +486,44 @@
                  user_security_group_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage Exoscale [Security Group](https://community.exoscale.com/documentation/compute/security-groups/) Rules.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_security_group = exoscale.SecurityGroup("mySecurityGroup")
         my_security_group_rule = exoscale.SecurityGroupRule("mySecurityGroupRule",
             security_group_id=my_security_group.id,
             type="INGRESS",
             protocol="TCP",
             cidr="0.0.0.0/0",
             start_port=80,
             end_port=80)
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing security group rule may be imported by `<security-group-ID>/<security-group-rule-ID>`:
 
         ```sh
         $ pulumi import exoscale:index/securityGroupRule:SecurityGroupRule \\
         ```
 
-         exoscale_security_group_rule.my_security_group_rule \\
+          exoscale_security_group_rule.my_security_group_rule \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cidr: ❗ An (`INGRESS`) source / (`EGRESS`) destination IP subnet (in [CIDR notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation)) to match (conflicts with `public_security_group`/`user_security_group`/`user_security_group_id`).
         :param pulumi.Input[str] description: ❗ A free-form text describing the security group rule.
         :param pulumi.Input[int] end_port: ❗ A `TCP`/`UDP` port range to match.
         :param pulumi.Input[int] icmp_code: ❗ An ICMP/ICMPv6 [type/code](https://en.wikipedia.org/wiki/Internet_Control_Message_Protocol#Control_messages) to match.
@@ -542,42 +544,44 @@
                  args: SecurityGroupRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage Exoscale [Security Group](https://community.exoscale.com/documentation/compute/security-groups/) Rules.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_security_group = exoscale.SecurityGroup("mySecurityGroup")
         my_security_group_rule = exoscale.SecurityGroupRule("mySecurityGroupRule",
             security_group_id=my_security_group.id,
             type="INGRESS",
             protocol="TCP",
             cidr="0.0.0.0/0",
             start_port=80,
             end_port=80)
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing security group rule may be imported by `<security-group-ID>/<security-group-rule-ID>`:
 
         ```sh
         $ pulumi import exoscale:index/securityGroupRule:SecurityGroupRule \\
         ```
 
-         exoscale_security_group_rule.my_security_group_rule \\
+          exoscale_security_group_rule.my_security_group_rule \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524
 
         :param str resource_name: The name of the resource.
         :param SecurityGroupRuleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/security_group_rules.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/security_group_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/sks_cluster.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,29 @@
     def __init__(__self__, *,
                  zone: pulumi.Input[str],
                  addons: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  auto_upgrade: Optional[pulumi.Input[bool]] = None,
                  cni: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  exoscale_ccm: Optional[pulumi.Input[bool]] = None,
+                 exoscale_csi: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  metrics_server: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  oidc: Optional[pulumi.Input['SksClusterOidcArgs']] = None,
                  service_level: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SksCluster resource.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] cni: The CNI plugin that is to be used. Available options are "calico" or "cilium". Defaults to "calico". Setting empty string will result in a cluster with no CNI.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_csi: Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
         :param pulumi.Input['SksClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
         :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
         """
@@ -52,14 +54,16 @@
             pulumi.set(__self__, "auto_upgrade", auto_upgrade)
         if cni is not None:
             pulumi.set(__self__, "cni", cni)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if exoscale_ccm is not None:
             pulumi.set(__self__, "exoscale_ccm", exoscale_ccm)
+        if exoscale_csi is not None:
+            pulumi.set(__self__, "exoscale_csi", exoscale_csi)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if metrics_server is not None:
             pulumi.set(__self__, "metrics_server", metrics_server)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if oidc is not None:
@@ -138,14 +142,26 @@
         return pulumi.get(self, "exoscale_ccm")
 
     @exoscale_ccm.setter
     def exoscale_ccm(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "exoscale_ccm", value)
 
     @property
+    @pulumi.getter(name="exoscaleCsi")
+    def exoscale_csi(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
+        """
+        return pulumi.get(self, "exoscale_csi")
+
+    @exoscale_csi.setter
+    def exoscale_csi(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "exoscale_csi", value)
+
+    @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         A map of key/value labels.
         """
         return pulumi.get(self, "labels")
 
@@ -222,14 +238,15 @@
                  auto_upgrade: Optional[pulumi.Input[bool]] = None,
                  cni: Optional[pulumi.Input[str]] = None,
                  control_plane_ca: Optional[pulumi.Input[str]] = None,
                  created_at: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  exoscale_ccm: Optional[pulumi.Input[bool]] = None,
+                 exoscale_csi: Optional[pulumi.Input[bool]] = None,
                  kubelet_ca: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  metrics_server: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  nodepools: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  oidc: Optional[pulumi.Input['SksClusterOidcArgs']] = None,
                  service_level: Optional[pulumi.Input[str]] = None,
@@ -242,14 +259,15 @@
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] cni: The CNI plugin that is to be used. Available options are "calico" or "cilium". Defaults to "calico". Setting empty string will result in a cluster with no CNI.
         :param pulumi.Input[str] control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
         :param pulumi.Input[str] created_at: The cluster creation date.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[str] endpoint: The cluster API endpoint.
         :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_csi: Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
         :param pulumi.Input[str] kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] nodepools: The list of exoscale*sks*nodepool (IDs) attached to the cluster.
         :param pulumi.Input['SksClusterOidcArgs'] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
@@ -274,14 +292,16 @@
             pulumi.set(__self__, "created_at", created_at)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if endpoint is not None:
             pulumi.set(__self__, "endpoint", endpoint)
         if exoscale_ccm is not None:
             pulumi.set(__self__, "exoscale_ccm", exoscale_ccm)
+        if exoscale_csi is not None:
+            pulumi.set(__self__, "exoscale_csi", exoscale_csi)
         if kubelet_ca is not None:
             pulumi.set(__self__, "kubelet_ca", kubelet_ca)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if metrics_server is not None:
             pulumi.set(__self__, "metrics_server", metrics_server)
         if name is not None:
@@ -404,14 +424,26 @@
         return pulumi.get(self, "exoscale_ccm")
 
     @exoscale_ccm.setter
     def exoscale_ccm(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "exoscale_ccm", value)
 
     @property
+    @pulumi.getter(name="exoscaleCsi")
+    def exoscale_csi(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
+        """
+        return pulumi.get(self, "exoscale_csi")
+
+    @exoscale_csi.setter
+    def exoscale_csi(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "exoscale_csi", value)
+
+    @property
     @pulumi.getter(name="kubeletCa")
     def kubelet_ca(self) -> Optional[pulumi.Input[str]]:
         """
         The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
         """
         return pulumi.get(self, "kubelet_ca")
 
@@ -534,58 +566,62 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  addons: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  auto_upgrade: Optional[pulumi.Input[bool]] = None,
                  cni: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  exoscale_ccm: Optional[pulumi.Input[bool]] = None,
+                 exoscale_csi: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  metrics_server: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  oidc: Optional[pulumi.Input[pulumi.InputType['SksClusterOidcArgs']]] = None,
                  service_level: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage Exoscale [Scalable Kubernetes Service (SKS)](https://community.exoscale.com/documentation/sks/) Clusters.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sks_cluster = exoscale.SksCluster("mySksCluster", zone="ch-gva-2")
         pulumi.export("mySksClusterEndpoint", my_sks_cluster.endpoint)
         ```
+        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_sks_nodepool(s) to the cluster.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing SKS cluster may be imported by `<ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/sksCluster:SksCluster \\
         ```
 
-         exoscale_sks_cluster.my_sks_cluster \\
+          exoscale_sks_cluster.my_sks_cluster \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] cni: The CNI plugin that is to be used. Available options are "calico" or "cilium". Defaults to "calico". Setting empty string will result in a cluster with no CNI.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_csi: Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
         :param pulumi.Input[pulumi.InputType['SksClusterOidcArgs']] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
         :param pulumi.Input[str] version: The version of the control plane (default: latest version available from the API; see `exo compute sks versions` for reference; may only be set at creation time).
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
@@ -597,38 +633,40 @@
                  args: SksClusterArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage Exoscale [Scalable Kubernetes Service (SKS)](https://community.exoscale.com/documentation/sks/) Clusters.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sks_cluster = exoscale.SksCluster("mySksCluster", zone="ch-gva-2")
         pulumi.export("mySksClusterEndpoint", my_sks_cluster.endpoint)
         ```
+        <!--End PulumiCodeChooser -->
 
         Next step is to attach exoscale_sks_nodepool(s) to the cluster.
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing SKS cluster may be imported by `<ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/sksCluster:SksCluster \\
         ```
 
-         exoscale_sks_cluster.my_sks_cluster \\
+          exoscale_sks_cluster.my_sks_cluster \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param SksClusterArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -642,14 +680,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  addons: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  auto_upgrade: Optional[pulumi.Input[bool]] = None,
                  cni: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  exoscale_ccm: Optional[pulumi.Input[bool]] = None,
+                 exoscale_csi: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  metrics_server: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  oidc: Optional[pulumi.Input[pulumi.InputType['SksClusterOidcArgs']]] = None,
                  service_level: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None,
@@ -663,14 +702,15 @@
             __props__ = SksClusterArgs.__new__(SksClusterArgs)
 
             __props__.__dict__["addons"] = addons
             __props__.__dict__["auto_upgrade"] = auto_upgrade
             __props__.__dict__["cni"] = cni
             __props__.__dict__["description"] = description
             __props__.__dict__["exoscale_ccm"] = exoscale_ccm
+            __props__.__dict__["exoscale_csi"] = exoscale_csi
             __props__.__dict__["labels"] = labels
             __props__.__dict__["metrics_server"] = metrics_server
             __props__.__dict__["name"] = name
             __props__.__dict__["oidc"] = oidc
             __props__.__dict__["service_level"] = service_level
             __props__.__dict__["version"] = version
             if zone is None and not opts.urn:
@@ -698,14 +738,15 @@
             auto_upgrade: Optional[pulumi.Input[bool]] = None,
             cni: Optional[pulumi.Input[str]] = None,
             control_plane_ca: Optional[pulumi.Input[str]] = None,
             created_at: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             endpoint: Optional[pulumi.Input[str]] = None,
             exoscale_ccm: Optional[pulumi.Input[bool]] = None,
+            exoscale_csi: Optional[pulumi.Input[bool]] = None,
             kubelet_ca: Optional[pulumi.Input[str]] = None,
             labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             metrics_server: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             nodepools: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             oidc: Optional[pulumi.Input[pulumi.InputType['SksClusterOidcArgs']]] = None,
             service_level: Optional[pulumi.Input[str]] = None,
@@ -723,14 +764,15 @@
         :param pulumi.Input[bool] auto_upgrade: Enable automatic upgrading of the control plane version.
         :param pulumi.Input[str] cni: The CNI plugin that is to be used. Available options are "calico" or "cilium". Defaults to "calico". Setting empty string will result in a cluster with no CNI.
         :param pulumi.Input[str] control_plane_ca: The CA certificate (in PEM format) for TLS communications between control plane components.
         :param pulumi.Input[str] created_at: The cluster creation date.
         :param pulumi.Input[str] description: A free-form text describing the cluster.
         :param pulumi.Input[str] endpoint: The cluster API endpoint.
         :param pulumi.Input[bool] exoscale_ccm: Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
+        :param pulumi.Input[bool] exoscale_csi: Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
         :param pulumi.Input[str] kubelet_ca: The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: A map of key/value labels.
         :param pulumi.Input[bool] metrics_server: Deploy the [Kubernetes Metrics Server](https://github.com/kubernetes-sigs/metrics-server/) in the control plane (boolean; default: `true`; may only be set at creation time).
         :param pulumi.Input[str] name: The SKS cluster name.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] nodepools: The list of exoscale*sks*nodepool (IDs) attached to the cluster.
         :param pulumi.Input[pulumi.InputType['SksClusterOidcArgs']] oidc: An OpenID Connect configuration to provide to the Kubernetes API server (may only be set at creation time). Structure is documented below.
         :param pulumi.Input[str] service_level: The service level of the control plane (`pro` or `starter`; default: `pro`; may only be set at creation time).
@@ -747,14 +789,15 @@
         __props__.__dict__["auto_upgrade"] = auto_upgrade
         __props__.__dict__["cni"] = cni
         __props__.__dict__["control_plane_ca"] = control_plane_ca
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["description"] = description
         __props__.__dict__["endpoint"] = endpoint
         __props__.__dict__["exoscale_ccm"] = exoscale_ccm
+        __props__.__dict__["exoscale_csi"] = exoscale_csi
         __props__.__dict__["kubelet_ca"] = kubelet_ca
         __props__.__dict__["labels"] = labels
         __props__.__dict__["metrics_server"] = metrics_server
         __props__.__dict__["name"] = name
         __props__.__dict__["nodepools"] = nodepools
         __props__.__dict__["oidc"] = oidc
         __props__.__dict__["service_level"] = service_level
@@ -832,14 +875,22 @@
     def exoscale_ccm(self) -> pulumi.Output[Optional[bool]]:
         """
         Deploy the Exoscale [Cloud Controller Manager](https://github.com/exoscale/exoscale-cloud-controller-manager/) in the control plane (boolean; default: `true`; may only be set at creation time).
         """
         return pulumi.get(self, "exoscale_ccm")
 
     @property
+    @pulumi.getter(name="exoscaleCsi")
+    def exoscale_csi(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Deploy the Exoscale [Container Storage Interface](https://github.com/exoscale/exoscale-csi-driver/) on worker nodes (boolean; default: `false`; may only be set at creation time).
+        """
+        return pulumi.get(self, "exoscale_csi")
+
+    @property
     @pulumi.getter(name="kubeletCa")
     def kubelet_ca(self) -> pulumi.Output[str]:
         """
         The CA certificate (in PEM format) for TLS communications between kubelets and the control plane.
         """
         return pulumi.get(self, "kubelet_ca")
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/sks_kubeconfig.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/sks_nodepool.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/sks_nodepool.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,40 +597,42 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage Exoscale [Scalable Kubernetes Service (SKS)](https://community.exoscale.com/documentation/sks/) Node Pools.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sks_cluster = exoscale.SksCluster("mySksCluster", zone="ch-gva-2")
         my_sks_nodepool = exoscale.SksNodepool("mySksNodepool",
             cluster_id=my_sks_cluster.id,
             zone=my_sks_cluster.zone,
             instance_type="standard.medium",
             size=3)
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing SKS node pool may be imported by `<cluster-ID>/<nodepool-ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/sksNodepool:SksNodepool \\
         ```
 
-         exoscale_sks_nodepool.my_sks_nodepool \\
+          exoscale_sks_nodepool.my_sks_nodepool \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] anti_affinity_group_ids: A list of exoscale*anti*affinity_group (IDs) to be attached to the managed instances.
         :param pulumi.Input[str] cluster_id: ❗ The parent exoscale*sks*cluster ID.
         :param pulumi.Input[str] deploy_target_id: A deploy target ID.
         :param pulumi.Input[str] description: A free-form text describing the pool.
@@ -652,40 +654,42 @@
                  args: SksNodepoolArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage Exoscale [Scalable Kubernetes Service (SKS)](https://community.exoscale.com/documentation/sks/) Node Pools.
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumiverse_exoscale as exoscale
 
         my_sks_cluster = exoscale.SksCluster("mySksCluster", zone="ch-gva-2")
         my_sks_nodepool = exoscale.SksNodepool("mySksNodepool",
             cluster_id=my_sks_cluster.id,
             zone=my_sks_cluster.zone,
             instance_type="standard.medium",
             size=3)
         ```
+        <!--End PulumiCodeChooser -->
 
         Please refer to the examples
         directory for complete configuration examples.
 
         ## Import
 
         An existing SKS node pool may be imported by `<cluster-ID>/<nodepool-ID>@<zone>`:
 
         ```sh
         $ pulumi import exoscale:index/sksNodepool:SksNodepool \\
         ```
 
-         exoscale_sks_nodepool.my_sks_nodepool \\
+          exoscale_sks_nodepool.my_sks_nodepool \\
 
-         f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
+          f81d4fae-7dec-11d0-a765-00a0c91e6bf6/9ecc6b8b-73d4-4211-8ced-f7f29bb79524@ch-gva-2
 
         :param str resource_name: The name of the resource.
         :param SksNodepoolArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/ssh_key.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ssh_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,17 +119,17 @@
 
         An existing SSH key may be imported as a resource by `<name>`:
 
         ```sh
         $ pulumi import exoscale:index/sshKey:SshKey \\
         ```
 
-         exoscale_ssh_key.my_ssh_key \\
+          exoscale_ssh_key.my_ssh_key \\
 
-         my-ssh-key
+          my-ssh-key
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: ❗ The SSH key name.
         :param pulumi.Input[str] public_key: ❗ The SSH *public* key that will be authorized in compute instances.
         """
         ...
@@ -143,17 +143,17 @@
 
         An existing SSH key may be imported as a resource by `<name>`:
 
         ```sh
         $ pulumi import exoscale:index/sshKey:SshKey \\
         ```
 
-         exoscale_ssh_key.my_ssh_key \\
+          exoscale_ssh_key.my_ssh_key \\
 
-         my-ssh-key
+          my-ssh-key
 
         :param str resource_name: The name of the resource.
         :param SshKeyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale/ssh_keypair.py` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale/ssh_keypair.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale.egg-info/PKG-INFO` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-exoscale
-Version: 0.56.0
+Version: 0.57.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_exoscale-0.56.0/pulumiverse_exoscale.egg-info/SOURCES.txt` & `pulumiverse_exoscale-0.57.0/pulumiverse_exoscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.56.0/setup.py` & `pulumiverse_exoscale-0.57.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.56.0"
+VERSION = "0.57.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "exoscale Pulumi Package - Development Version"
```

