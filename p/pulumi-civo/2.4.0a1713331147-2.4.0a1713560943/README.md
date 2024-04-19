# Comparing `tmp/pulumi_civo-2.4.0a1713331147.tar.gz` & `tmp/pulumi_civo-2.4.0a1713560943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_civo-2.4.0a1713331147.tar", last modified: Wed Apr 17 05:23:34 2024, max compression
+gzip compressed data, was "pulumi_civo-2.4.0a1713560943.tar", last modified: Fri Apr 19 21:11:42 2024, max compression
```

## Comparing `pulumi_civo-2.4.0a1713331147.tar` & `pulumi_civo-2.4.0a1713560943.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:23:34.658341 pulumi_civo-2.4.0a1713331147/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-17 05:23:34.658341 pulumi_civo-2.4.0a1713331147/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:23:34.654341 pulumi_civo-2.4.0a1713331147/pulumi_civo/
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41211 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:23:34.658341 pulumi_civo-2.4.0a1713331147/pulumi_civo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    22759 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    24234 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_database_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_disk_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_kubernetes_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    47548 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/instance_reserved_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    15596 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    55857 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo/volume_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:23:34.658341 pulumi_civo-2.4.0a1713331147/pulumi_civo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-17 05:23:34.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-17 05:23:34.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:23:34.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 05:23:34.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 05:23:34.000000 pulumi_civo-2.4.0a1713331147/pulumi_civo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-17 05:23:28.000000 pulumi_civo-2.4.0a1713331147/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:23:34.658341 pulumi_civo-2.4.0a1713331147/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:42.157178 pulumi_civo-2.4.0a1713560943/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-19 21:11:42.157178 pulumi_civo-2.4.0a1713560943/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:42.153178 pulumi_civo-2.4.0a1713560943/pulumi_civo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41211 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:42.157178 pulumi_civo-2.4.0a1713560943/pulumi_civo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23846 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18933 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24234 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_database_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_disk_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_kubernetes_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47548 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10425 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/instance_reserved_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15788 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55857 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14331 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo/volume_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:42.157178 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-19 21:11:42.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-19 21:11:42.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:11:42.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:11:42.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 21:11:42.000000 pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-19 21:11:35.000000 pulumi_civo-2.4.0a1713560943/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:11:42.157178 pulumi_civo-2.4.0a1713560943/setup.cfg
```

### Comparing `pulumi_civo-2.4.0a1713331147/PKG-INFO` & `pulumi_civo-2.4.0a1713560943/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1713331147
+Version: 2.4.0a1713560943
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi,civo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1713331147/README.md` & `pulumi_civo-2.4.0a1713560943/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/__init__.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/_inputs.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/_utilities.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/config/__init__.pyi` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/config/vars.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/database.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/dns_domain_name.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/dns_domain_name.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Create a new domain name
-        main = civo.DnsDomainName("main")
+        main = civo.DnsDomainName("main", name="mydomain.com")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         using domain name
 
@@ -122,15 +122,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Create a new domain name
-        main = civo.DnsDomainName("main")
+        main = civo.DnsDomainName("main", name="mydomain.com")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         using domain name
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/dns_domain_record.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/firewall.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/firewall.py`

 * *Files 20% similar despite different names*

```diff
@@ -232,67 +232,14 @@
                  name: Optional[pulumi.Input[str]] = None,
                  network_id: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Civo firewall resource. This can be used to create, modify, and delete firewalls.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_civo as civo
-
-        # Create a network
-        custom_net = civo.Network("customNet", label="my-custom-network")
-        # Create a firewall
-        www_firewall = civo.Firewall("wwwFirewall", network_id=custom_net.id)
-        # Create a firewall with the default rules
-        www_index_firewall_firewall = civo.Firewall("wwwIndex/firewallFirewall",
-            network_id=custom_net.id,
-            create_default_rules=True)
-        # Create a firewall withouth the default rules but with a custom rule
-        www_civo_index_firewall_firewall = civo.Firewall("wwwCivoIndex/firewallFirewall",
-            network_id=custom_net.id,
-            create_default_rules=False,
-            ingress_rules=[
-                civo.FirewallIngressRuleArgs(
-                    label="k8s",
-                    protocol="tcp",
-                    port_range="6443",
-                    cidrs=[
-                        "192.168.1.1/32",
-                        "192.168.10.4/32",
-                        "192.168.10.10/32",
-                    ],
-                    action="allow",
-                ),
-                civo.FirewallIngressRuleArgs(
-                    label="ssh",
-                    protocol="tcp",
-                    port_range="22",
-                    cidrs=[
-                        "192.168.1.1/32",
-                        "192.168.10.4/32",
-                        "192.168.10.10/32",
-                    ],
-                    action="allow",
-                ),
-            ],
-            egress_rules=[civo.FirewallEgressRuleArgs(
-                label="all",
-                protocol="tcp",
-                port_range="1-65535",
-                cidrs=["0.0.0.0/0"],
-                action="allow",
-            )])
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/firewall:Firewall www b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
         ```
@@ -311,67 +258,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[FirewallArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Civo firewall resource. This can be used to create, modify, and delete firewalls.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_civo as civo
-
-        # Create a network
-        custom_net = civo.Network("customNet", label="my-custom-network")
-        # Create a firewall
-        www_firewall = civo.Firewall("wwwFirewall", network_id=custom_net.id)
-        # Create a firewall with the default rules
-        www_index_firewall_firewall = civo.Firewall("wwwIndex/firewallFirewall",
-            network_id=custom_net.id,
-            create_default_rules=True)
-        # Create a firewall withouth the default rules but with a custom rule
-        www_civo_index_firewall_firewall = civo.Firewall("wwwCivoIndex/firewallFirewall",
-            network_id=custom_net.id,
-            create_default_rules=False,
-            ingress_rules=[
-                civo.FirewallIngressRuleArgs(
-                    label="k8s",
-                    protocol="tcp",
-                    port_range="6443",
-                    cidrs=[
-                        "192.168.1.1/32",
-                        "192.168.10.4/32",
-                        "192.168.10.10/32",
-                    ],
-                    action="allow",
-                ),
-                civo.FirewallIngressRuleArgs(
-                    label="ssh",
-                    protocol="tcp",
-                    port_range="22",
-                    cidrs=[
-                        "192.168.1.1/32",
-                        "192.168.10.4/32",
-                        "192.168.10.10/32",
-                    ],
-                    action="allow",
-                ),
-            ],
-            egress_rules=[civo.FirewallEgressRuleArgs(
-                label="all",
-                protocol="tcp",
-                port_range="1-65535",
-                cidrs=["0.0.0.0/0"],
-                action="allow",
-            )])
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         using ID
 
         ```sh
         $ pulumi import civo:index/firewall:Firewall www b8ecd2ab-2267-4a5e-8692-cbf1d32583e3
         ```
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/firewall_rule.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_database.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_database_version.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_database_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_disk_image.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_disk_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_dns_domain_name.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_dns_domain_record.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_firewall.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_instance.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_instances.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     ```python
     import pulumi
     import pulumi_civo as civo
 
     small_size = civo.get_instances(region="LON1",
         filters=[civo.GetInstancesFilterArgs(
             key="size",
-            values=[g3["small"]],
+            values=[small],
         )])
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetInstancesFilterArgs']] filters: One or more key/value pairs on which to filter results
     :param Sequence[pulumi.InputType['GetInstancesSortArgs']] sorts: One or more key/direction pairs on which to sort results
@@ -150,15 +150,15 @@
     ```python
     import pulumi
     import pulumi_civo as civo
 
     small_size = civo.get_instances(region="LON1",
         filters=[civo.GetInstancesFilterArgs(
             key="size",
-            values=[g3["small"]],
+            values=[small],
         )])
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetInstancesFilterArgs']] filters: One or more key/value pairs on which to filter results
     :param Sequence[pulumi.InputType['GetInstancesSortArgs']] sorts: One or more key/direction pairs on which to sort results
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_kubernetes_cluster.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_kubernetes_version.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_kubernetes_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_load_balancer.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_load_balancer.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
+    # TODO
     my_lb = civo.get_load_balancer(name="lb-name",
         region="LON1")
     pulumi.export("civoLoadbalancerOutput", my_lb.public_ip)
     ```
     <!--End PulumiCodeChooser -->
 
 
@@ -262,14 +263,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
+    # TODO
     my_lb = civo.get_load_balancer(name="lb-name",
         region="LON1")
     pulumi.export("civoLoadbalancerOutput", my_lb.public_ip)
     ```
     <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_network.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_object_store.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_object_store_credential.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_object_store_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,20 +116,22 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
-    backup_object_store_credential = civo.get_object_store_credential(name="backup-server")
+    # Read a credential for the object store
+    backup = civo.get_object_store_credential(name="backup-server")
     # Use the credential to create a bucket
-    backup_object_store = civo.ObjectStore("backupObjectStore",
+    backup_object_store = civo.ObjectStore("backup",
+        name="backup-server",
         max_size_gb=500,
         region="LON1",
-        access_key_id=backup_object_store_credential.access_key_id)
+        access_key_id=backup.access_key_id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Object Store Credential
     :param str name: The name of the Object Store Credential
     :param str region: The region of an existing Object Store
@@ -163,20 +165,22 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_civo as civo
 
-    backup_object_store_credential = civo.get_object_store_credential(name="backup-server")
+    # Read a credential for the object store
+    backup = civo.get_object_store_credential(name="backup-server")
     # Use the credential to create a bucket
-    backup_object_store = civo.ObjectStore("backupObjectStore",
+    backup_object_store = civo.ObjectStore("backup",
+        name="backup-server",
         max_size_gb=500,
         region="LON1",
-        access_key_id=backup_object_store_credential.access_key_id)
+        access_key_id=backup.access_key_id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str id: The ID of the Object Store Credential
     :param str name: The name of the Object Store Credential
     :param str region: The region of an existing Object Store
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_region.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_reserved_ip.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_size.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_ssh_key.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/get_volume.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/instance.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/instance_reserved_ip_assignment.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/instance_reserved_ip_assignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,19 +137,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Send to create a reserved IP
-        www = civo.ReservedIp("www")
+        www = civo.ReservedIp("www", name="nginx-www")
         # We assign the reserved IP to the instance
         webserver_www = civo.InstanceReservedIpAssignment("webserver-www",
-            instance_id=civo_instance["www"]["id"],
-            reserved_ip_id=civo_reserved_ip["web-server"]["id"])
+            instance_id=www_civo_instance["id"],
+            reserved_ip_id=web_server["id"])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] instance_id: The instance id
         :param pulumi.Input[str] region: The region of the ip
@@ -168,19 +168,19 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
         # Send to create a reserved IP
-        www = civo.ReservedIp("www")
+        www = civo.ReservedIp("www", name="nginx-www")
         # We assign the reserved IP to the instance
         webserver_www = civo.InstanceReservedIpAssignment("webserver-www",
-            instance_id=civo_instance["www"]["id"],
-            reserved_ip_id=civo_reserved_ip["web-server"]["id"])
+            instance_id=www_civo_instance["id"],
+            reserved_ip_id=web_server["id"])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InstanceReservedIpAssignmentArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/kubernetes_cluster.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/kubernetes_node_pool.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/kubernetes_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/network.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        custom_net = civo.Network("customNet", label="test_network")
+        custom_net = civo.Network("custom_net", label="test_network")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
@@ -169,15 +169,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        custom_net = civo.Network("customNet", label="test_network")
+        custom_net = civo.Network("custom_net", label="test_network")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/object_store.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/object_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,18 +203,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        backup_object_store = civo.ObjectStore("backupObjectStore",
+        backup_object_store = civo.ObjectStore("backup",
+            name="backup-server",
             max_size_gb=500,
             region="LON1")
-        backup_object_store_credential = civo.get_object_store_credential_output(id=backup_object_store.access_key_id)
+        # If you create the bucket without credentials, you can read the credentials in this way
+        backup = civo.get_object_store_credential_output(id=backup_object_store.access_key_id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
@@ -241,18 +243,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        backup_object_store = civo.ObjectStore("backupObjectStore",
+        backup_object_store = civo.ObjectStore("backup",
+            name="backup-server",
             max_size_gb=500,
             region="LON1")
-        backup_object_store_credential = civo.get_object_store_credential_output(id=backup_object_store.access_key_id)
+        # If you create the bucket without credentials, you can read the credentials in this way
+        backup = civo.get_object_store_credential_output(id=backup_object_store.access_key_id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/object_store_credential.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/object_store_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,24 +187,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        backup_object_store_credential = civo.get_object_store_credential(name="backup-server")
+        # Create a simple credential for the object store
+        backup = civo.get_object_store_credential(name="backup-server")
         # Create a credential for the object store with a specific access key and secret key
-        backup_index_object_store_credential_object_store_credential = civo.ObjectStoreCredential("backupIndex/objectStoreCredentialObjectStoreCredential",
+        backup_object_store_credential = civo.ObjectStoreCredential("backup",
+            name="backup-server",
             access_key_id="my-access-key",
             secret_access_key="my-secret-key")
         # Use the credential to create a bucket
-        backup_object_store = civo.ObjectStore("backupObjectStore",
+        backup_object_store = civo.ObjectStore("backup",
+            name="backup-server",
             max_size_gb=500,
             region="LON1",
-            access_key_id=backup_index / object_store_credential_object_store_credential["accessKeyId"])
+            access_key_id=backup_object_store_credential.access_key_id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
@@ -231,24 +234,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        backup_object_store_credential = civo.get_object_store_credential(name="backup-server")
+        # Create a simple credential for the object store
+        backup = civo.get_object_store_credential(name="backup-server")
         # Create a credential for the object store with a specific access key and secret key
-        backup_index_object_store_credential_object_store_credential = civo.ObjectStoreCredential("backupIndex/objectStoreCredentialObjectStoreCredential",
+        backup_object_store_credential = civo.ObjectStoreCredential("backup",
+            name="backup-server",
             access_key_id="my-access-key",
             secret_access_key="my-secret-key")
         # Use the credential to create a bucket
-        backup_object_store = civo.ObjectStore("backupObjectStore",
+        backup_object_store = civo.ObjectStore("backup",
+            name="backup-server",
             max_size_gb=500,
             region="LON1",
-            access_key_id=backup_index / object_store_credential_object_store_credential["accessKeyId"])
+            access_key_id=backup_object_store_credential.access_key_id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/outputs.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/provider.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/reserved_ip.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/reserved_ip.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        www = civo.ReservedIp("www")
+        www = civo.ReservedIp("www", name="nginx-www")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         terrafom import civo_reserved_ip.www 9f0e86fc-b2c6-46b4-82ed-2f28419f8ae3
 
@@ -150,15 +150,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
-        www = civo.ReservedIp("www")
+        www = civo.ReservedIp("www", name="nginx-www")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         terrafom import civo_reserved_ip.www 9f0e86fc-b2c6-46b4-82ed-2f28419f8ae3
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/ssh_key.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/ssh_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,16 +119,19 @@
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
+        import pulumi_std as std
 
-        my_user = civo.SshKey("my-user", public_key=(lambda path: open(path).read())("~/.ssh/id_rsa.pub"))
+        my_user = civo.SshKey("my-user",
+            name="my-user",
+            public_key=std.file(input="~/.ssh/id_rsa.pub").result)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
 
@@ -152,16 +155,19 @@
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
+        import pulumi_std as std
 
-        my_user = civo.SshKey("my-user", public_key=(lambda path: open(path).read())("~/.ssh/id_rsa.pub"))
+        my_user = civo.SshKey("my-user",
+            name="my-user",
+            public_key=std.file(input="~/.ssh/id_rsa.pub").result)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         using ID
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/volume.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,17 +185,19 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
+        # Get network
         default_network = civo.get_network(label="Default")
         # Create volume
         db = civo.Volume("db",
+            name="backup-data",
             size_gb=5,
             network_id=default_network.id,
             opts=pulumi.ResourceOptions(depends_on=[default_network]))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -225,17 +227,19 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_civo as civo
 
+        # Get network
         default_network = civo.get_network(label="Default")
         # Create volume
         db = civo.Volume("db",
+            name="backup-data",
             size_gb=5,
             network_id=default_network.id,
             opts=pulumi.ResourceOptions(depends_on=[default_network]))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo/volume_attachment.py` & `pulumi_civo-2.4.0a1713560943/pulumi_civo/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo.egg-info/PKG-INFO` & `pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1713331147
+Version: 2.4.0a1713560943
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi,civo
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1713331147/pulumi_civo.egg-info/SOURCES.txt` & `pulumi_civo-2.4.0a1713560943/pulumi_civo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1713331147/pyproject.toml` & `pulumi_civo-2.4.0a1713560943/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_civo"
   description = "A Pulumi package for creating and managing Civo cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "civo"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.4.0a1713331147"
+  version = "2.4.0a1713560943"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-civo"
 
 [build-system]
```

