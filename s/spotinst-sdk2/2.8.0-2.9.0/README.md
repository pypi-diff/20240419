# Comparing `tmp/spotinst-sdk2-2.8.0.tar.gz` & `tmp/spotinst-sdk2-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-sdk2-2.8.0.tar", last modified: Fri Mar 29 13:03:48 2024, max compression
+gzip compressed data, was "spotinst-sdk2-2.9.0.tar", last modified: Fri Apr 19 15:55:56 2024, max compression
```

## Comparing `spotinst-sdk2-2.8.0.tar` & `spotinst-sdk2-2.9.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    11356 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/LICENSE
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       43 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/NOTICE.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/PKG-INFO
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     7177 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/README.md
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     3543 2023-11-02 17:25:54.000000 spotinst-sdk2-2.8.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     5154 2024-01-27 17:33:52.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15928 2023-11-20 13:07:49.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12645 2024-02-01 18:22:35.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/admin/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/elastigroup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    91237 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/elastigroup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/functions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3184 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/functions/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/hpc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3376 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/hpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/managed_instance/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11698 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/managed_instance/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/mcs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      916 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/mcs/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/mrscaler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2024-02-25 21:58:42.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/mrscaler/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/ocean/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    58159 2024-03-29 13:02:23.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/ocean/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/ocean_cd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30586 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/ocean_cd/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/setup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5562 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/setup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/stateful_node/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16650 2023-11-25 09:32:13.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/stateful_node/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/subscription/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3859 2024-01-27 17:33:52.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/clients/subscription/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/admin/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/admin/user_mapping.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    42478 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/asg.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1278 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/deployment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      931 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/stateful.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/azure/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15655 2024-02-25 21:58:42.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/azure/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1449 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/azure/task.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/azure_v3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21715 2023-11-08 04:20:46.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/gcp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17709 2023-08-16 14:46:57.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/functions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3685 2023-11-08 04:25:02.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/functions/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/hpc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 14:21:47.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/hpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/hpc/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4954 2023-11-08 04:25:02.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/hpc/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/managed_instance/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/managed_instance/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/managed_instance/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15973 2024-02-25 21:58:42.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/managed_instance/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/mrscaler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/mrscaler/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/mrscaler/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18653 2024-02-25 21:58:42.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/mrscaler/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36517 2024-02-25 21:58:42.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean/azure/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19808 2024-03-29 13:02:23.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean/azure/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      806 2023-04-11 10:16:17.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2988 2023-11-08 04:23:08.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/rollout.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8887 2023-04-11 10:16:17.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4154 2023-04-11 10:16:17.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/strategy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2652 2023-11-08 04:23:37.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/verification_provider.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9061 2023-11-08 04:23:47.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/verification_template.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/setup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/setup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/setup/azure/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1082 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/setup/azure/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/setup/gcp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2023-02-24 13:45:28.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/setup/gcp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/stateful_node/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27588 2024-02-25 21:58:42.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/stateful_node/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.589745 spotinst-sdk2-2.8.0/spotinst_sdk2/models/subscription/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-11-08 04:24:10.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/models/subscription/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-11-08 04:24:57.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/session.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-03-29 13:02:23.000000 spotinst-sdk2-2.8.0/spotinst_sdk2/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-29 13:03:48.585743 spotinst-sdk2-2.8.0/spotinst_sdk2.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-03-29 13:03:48.000000 spotinst-sdk2-2.8.0/spotinst_sdk2.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2447 2024-03-29 13:03:48.000000 spotinst-sdk2-2.8.0/spotinst_sdk2.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-03-29 13:03:48.000000 spotinst-sdk2-2.8.0/spotinst_sdk2.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-03-29 13:03:48.000000 spotinst-sdk2-2.8.0/spotinst_sdk2.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-03-29 13:03:48.000000 spotinst-sdk2-2.8.0/spotinst_sdk2.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    11356 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/LICENSE
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       43 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/NOTICE.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/PKG-INFO
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     7177 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/README.md
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       63 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     3543 2024-04-19 15:27:21.000000 spotinst-sdk2-2.9.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     5154 2024-04-19 15:27:21.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15928 2023-11-20 13:07:49.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12645 2024-02-01 18:22:35.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/admin/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/elastigroup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    91237 2024-04-19 15:27:21.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/elastigroup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/functions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3184 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/functions/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/hpc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3376 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/hpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/managed_instance/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11698 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/managed_instance/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/mcs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      916 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/mcs/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/mrscaler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2024-02-25 21:58:42.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/mrscaler/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/ocean/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    58159 2024-04-19 15:54:27.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/ocean/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/ocean_cd/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30586 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/ocean_cd/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/setup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5562 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/setup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/stateful_node/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16650 2023-11-25 09:32:13.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/stateful_node/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/subscription/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3859 2024-01-27 17:33:52.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/clients/subscription/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/admin/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/admin/user_mapping.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    40959 2024-04-19 15:27:36.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/asg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1278 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/deployment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      931 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/stateful.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/azure/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15407 2024-04-19 15:27:36.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/azure/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1449 2024-04-19 15:27:21.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/azure/task.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/azure_v3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21715 2023-11-08 04:20:46.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17709 2023-08-16 14:46:57.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/functions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3685 2023-11-08 04:25:02.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/functions/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/hpc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 14:21:47.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/hpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/hpc/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4954 2023-11-08 04:25:02.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/hpc/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/managed_instance/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/managed_instance/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/managed_instance/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15583 2024-04-19 15:27:36.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/managed_instance/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/mrscaler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/mrscaler/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/mrscaler/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18653 2024-02-25 21:58:42.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/mrscaler/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36517 2024-02-25 21:58:42.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean/azure/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19808 2024-04-19 15:54:27.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean/azure/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      806 2023-04-11 10:16:17.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2988 2023-11-08 04:23:08.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/rollout.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8887 2023-04-11 10:16:17.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4154 2023-04-11 10:16:17.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/strategy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2652 2023-11-08 04:23:37.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/verification_provider.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9061 2023-11-08 04:23:47.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/verification_template.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/setup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/setup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/setup/azure/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1082 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/setup/azure/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/setup/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2023-02-24 13:45:28.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/setup/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/stateful_node/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27588 2024-02-25 21:58:42.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/stateful_node/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.700643 spotinst-sdk2-2.9.0/spotinst_sdk2/models/subscription/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-11-08 04:24:10.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/models/subscription/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-11-08 04:24:57.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/session.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2024-04-19 15:54:48.000000 spotinst-sdk2-2.9.0/spotinst_sdk2/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 15:55:56.696644 spotinst-sdk2-2.9.0/spotinst_sdk2.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-04-19 15:55:56.000000 spotinst-sdk2-2.9.0/spotinst_sdk2.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2447 2024-04-19 15:55:56.000000 spotinst-sdk2-2.9.0/spotinst_sdk2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-19 15:55:56.000000 spotinst-sdk2-2.9.0/spotinst_sdk2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-04-19 15:55:56.000000 spotinst-sdk2-2.9.0/spotinst_sdk2.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-19 15:55:56.000000 spotinst-sdk2-2.9.0/spotinst_sdk2.egg-info/top_level.txt
```

### Comparing `spotinst-sdk2-2.8.0/LICENSE` & `spotinst-sdk2-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/NOTICE.md` & `spotinst-sdk2-2.9.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/PKG-INFO` & `spotinst-sdk2-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-sdk2
-Version: 2.8.0
+Version: 2.9.0
 Summary: A Python SDK for Spotinst
 Home-page: https://github.com/spotinst/spotinst-sdk-python
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst spot instances aws azure ec2 cloud infrastructure development elastigroup
 Platform: UNKNOWN
```

### Comparing `spotinst-sdk2-2.8.0/README.md` & `spotinst-sdk2-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/setup.py` & `spotinst-sdk2-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/client.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/client.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/admin/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/elastigroup/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/elastigroup/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/functions/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/hpc/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/hpc/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/managed_instance/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/managed_instance/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/mcs/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/mcs/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/mrscaler/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/mrscaler/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/ocean/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/ocean_cd/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/ocean_cd/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/setup/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/stateful_node/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/stateful_node/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/clients/subscription/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/clients/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/admin/user_mapping.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/admin/user_mapping.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,39 +11,36 @@
     description: str
     region: str
     capacity: Capacity
     strategy: Strategy
     compute: Compute
     scaling: Scaling
     scheduling: Scheduling
-    multai: Multai
     third_parties_integration: ThirdPartyIntegrations
     """
 
     def __init__(
             self,
             name=none,
             description=none,
             region=none,
             capacity=none,
             strategy=none,
             compute=none,
             scaling=none,
             scheduling=none,
-            multai=none,
             third_parties_integration=none):
 
         self.name = name
         self.description = description
         self.region = region
         self.capacity = capacity
         self.strategy = strategy
         self.scaling = scaling
         self.scheduling = scheduling
-        self.multai = multai
         self.third_parties_integration = third_parties_integration
         self.compute = compute
 
 
 # endregion
 
 # region Strategy
@@ -476,54 +473,14 @@
         self.adjustment = adjustment
         self.adjustment_percentage = adjustment_percentage
         self.start_time = start_time
 
 
 # endregion
 
-# region Multai
-class Multai:
-    """
-    # Arguments
-    token: str
-    balancers: str
-    """
-
-    def __init__(self, token=none, balancers=none):
-
-        self.token = token
-        self.balancers = balancers
-
-
-class MultaiLoadBalancer:
-    """
-    # Arguments
-    project_id: str
-    balancer_id: str
-    target_set_id: str
-    az_awareness: bool
-    auto_weight: bool
-    """
-
-    def __init__(
-            self,
-            project_id=none,
-            balancer_id=none,
-            target_set_id=none,
-            az_awareness=none,
-            auto_weight=none):
-
-        self.project_id = project_id
-        self.balancer_id = balancer_id
-        self.target_set_id = target_set_id
-        self.az_awareness = az_awareness
-        self.auto_weight = auto_weight
-
-
-# endregion
 
 # region ThirdPartyIntegrations
 class Rancher:
     """
     # Arguments
     access_key: str
     secret_key: str
@@ -710,25 +667,14 @@
     """
 
     def __init__(self, evaluation_periods=none):
 
         self.evaluation_periods = evaluation_periods
 
 
-class MlbRuntimeConfiguration:
-    """
-    # Arguments
-    deployment_id: str
-    """
-
-    def __init__(self, deployment_id=none):
-
-        self.deployment_id = deployment_id
-
-
 class KubernetesConfiguration:
     """
     # Arguments
     api_server: str
     token: str
     integration_mode: str
     cluster_identifier: str
@@ -1106,15 +1052,14 @@
     mesosphere: Mesosphere
     elastic_beanstalk: ElasticBeanstalk
     ecs: EcsConfiguration
     kubernetes: KubernetesConfiguration
     right_scale: RightScaleConfiguration
     ops_works: OpsWorksConfiguration
     chef: ChefConfiguration
-    mlb_runtime: MlbRuntimeConfiguration
     code_deploy: CodeDeployConfiguration
     nomad: NomadConfiguration
     docker_swarm: DockerSwarmConfiguration
     route53: Route53Configuration
     """
 
     def __init__(
@@ -1123,29 +1068,27 @@
             mesosphere=none,
             elastic_beanstalk=none,
             ecs=none,
             kubernetes=none,
             right_scale=none,
             ops_works=none,
             chef=none,
-            mlb_runtime=none,
             code_deploy=none,
             nomad=none,
             docker_swarm=none,
             route53=none):
 
         self.rancher = rancher
         self.mesosphere = mesosphere
         self.elastic_beanstalk = elastic_beanstalk
         self.ecs = ecs
         self.kubernetes = kubernetes
         self.right_scale = right_scale
         self.ops_works = ops_works
         self.chef = chef
-        self.mlb_runtime = mlb_runtime
         self.code_deploy = code_deploy
         self.nomad = nomad
         self.docker_swarm = docker_swarm
         self.route53 = route53
 
 
 # endregion
@@ -1387,37 +1330,25 @@
 
 class LoadBalancer:
     """
     # Arguments
     type: str
     arn: str
     name: str
-    target_set_id: str
-    balancer_id: str
-    auto_weight: bool
-    az_awareness: bool
     """
 
     def __init__(
             self,
             type=none,
             arn=none,
-            name=none,
-            target_set_id=none,
-            balancer_id=none,
-            auto_weight=none,
-            az_awareness=none):
+            name=none):
 
         self.type = type
         self.arn = arn
         self.name = name
-        self.target_set_id = target_set_id
-        self.balancer_id = balancer_id
-        self.auto_weight = auto_weight
-        self.az_awareness = az_awareness
 
 
 class IamRole:
     """
     # Arguments
     name: str
     arn: str
```

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/asg.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/asg.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/deployment.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/deployment.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/aws/stateful.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/aws/stateful.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/azure/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/azure/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,35 +569,23 @@
 # endregion
 
 
 # region Third Parties Integration
 class ThirdPartiesIntegration:
     """
     # Arguments
-    mlb_runtime: MlbRuntime
     kubernetes: Kubernetes
     hpc_grid_engine: HpcGridEngine
     """
 
-    def __init__(self, mlb_runtime=none, kubernetes=none, hpc_grid_engine=none):
-        self.mlb_runtime = mlb_runtime
+    def __init__(self, kubernetes=none, hpc_grid_engine=none):
         self.kubernetes = kubernetes
         self.hpc_grid_engine = hpc_grid_engine
 
 
-class MlbRuntime:
-    """
-    # Arguments
-    deployment_id: str
-    """
-
-    def __init__(self, deployment_id=none):
-        self.deployment_id = deployment_id
-
-
 class Kubernetes:
     """
     # Arguments
     cluster_identifier: str
     """
 
     def __init__(self, cluster_identifier=none):
```

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/azure/task.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/azure/task.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/functions/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/hpc/aws/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/hpc/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/managed_instance/aws/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/managed_instance/aws/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,30 +350,20 @@
 
 class LoadBalancer:
     """
     # Arguments
     name: str
     arn: str
     type: str
-    balancer_id: str
-    target_set_id: str
-    az_awareness: bool
-    auto_weight: bool
     """
 
-    def __init__(self, name: str = none, arn: str = none, type: str = none, balancer_id: str = none,
-                 target_set_id: str = none, az_awareness: bool = none,
-                 auto_weight: bool = none):
+    def __init__(self, name: str = none, arn: str = none, type: str = none):
         self.name = name
         self.arn = arn
         self.type = type
-        self.balancer_id = balancer_id
-        self.target_set_id = target_set_id
-        self.az_awareness = az_awareness
-        self.auto_weight = auto_weight
 
 
 class LoadBalancersConfiguration:
     """
     # Arguments
     load_balancers: list[LoadBalancer]
     """
```

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/mrscaler/aws/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/mrscaler/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean/aws/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean/azure/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/rollout.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/rollout.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/strategy.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/strategy.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/verification_provider.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/verification_provider.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/ocean_cd/verification_template.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/ocean_cd/verification_template.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/setup/azure/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/setup/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/setup/gcp/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/setup/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/stateful_node/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/stateful_node/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/models/subscription/__init__.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/models/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2/session.py` & `spotinst-sdk2-2.9.0/spotinst_sdk2/session.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2.egg-info/PKG-INFO` & `spotinst-sdk2-2.9.0/spotinst_sdk2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-sdk2
-Version: 2.8.0
+Version: 2.9.0
 Summary: A Python SDK for Spotinst
 Home-page: https://github.com/spotinst/spotinst-sdk-python
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst spot instances aws azure ec2 cloud infrastructure development elastigroup
 Platform: UNKNOWN
```

### Comparing `spotinst-sdk2-2.8.0/spotinst_sdk2.egg-info/SOURCES.txt` & `spotinst-sdk2-2.9.0/spotinst_sdk2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

