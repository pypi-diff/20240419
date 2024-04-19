# Comparing `tmp/pulumi_rancher2-6.2.0a1713337589.tar.gz` & `tmp/pulumi_rancher2-6.2.0a1713561342.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rancher2-6.2.0a1713337589.tar", last modified: Wed Apr 17 07:15:07 2024, max compression
+gzip compressed data, was "pulumi_rancher2-6.2.0a1713561342.tar", last modified: Fri Apr 19 21:23:37 2024, max compression
```

## Comparing `pulumi_rancher2-6.2.0a1713337589.tar` & `pulumi_rancher2-6.2.0a1713561342.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:15:07.608820 pulumi_rancher2-6.2.0a1713337589/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-17 07:15:07.608820 pulumi_rancher2-6.2.0a1713337589/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:15:07.604820 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1391177 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    41229 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    42239 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/app_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    81707 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_active_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_adfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35072 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (127)    79388 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_free_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    37584 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_okta.py
--rw-r--r--   0 runner    (1001) docker     (127)    79475 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_open_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    27436 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32888 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    34833 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    45542 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)   167286 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    39652 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    24090 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    25641 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    31618 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    25340 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    62895 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:15:07.608820 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    20013 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    32449 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/custom_user_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    22341 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    25608 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_global_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_node_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_node_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_pod_security_admission_configuration_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_principal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_role_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/global_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    21643 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/global_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    47171 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/machine_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    41806 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/node_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    83735 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/node_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    34584 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)  1818101 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/pod_security_admission_configuration_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    69311 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    37937 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    37864 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    25746 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    31939 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/role_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    23036 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    24712 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:15:07.608820 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-17 07:15:07.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-17 07:15:07.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:15:07.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 07:15:07.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 07:15:07.000000 pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-17 07:15:00.000000 pulumi_rancher2-6.2.0a1713337589/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:15:07.608820 pulumi_rancher2-6.2.0a1713337589/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:23:37.299469 pulumi_rancher2-6.2.0a1713561342/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-19 21:23:37.299469 pulumi_rancher2-6.2.0a1713561342/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:23:37.295469 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1391177 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41309 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42447 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/app_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81707 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_adfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35072 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79388 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_free_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37584 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_okta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79475 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_open_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37387 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33102 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34833 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45710 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)   167692 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25140 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39562 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24090 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25689 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31630 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25436 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62895 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:23:37.299469 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20013 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32495 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/custom_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22389 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25608 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11703 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_node_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_pod_security_admission_configuration_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_principal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_role_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23970 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/global_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22839 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/global_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/machine_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41908 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28289 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26791 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84059 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/node_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34632 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1818101 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/pod_security_admission_configuration_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69311 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38033 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25140 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37896 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25794 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21772 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32035 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/role_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21382 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23036 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12596 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23952 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17357 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:23:37.299469 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-19 21:23:37.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-19 21:23:37.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:23:37.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:23:37.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 21:23:37.000000 pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 21:23:31.000000 pulumi_rancher2-6.2.0a1713561342/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:23:37.299469 pulumi_rancher2-6.2.0a1713561342/setup.cfg
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/PKG-INFO` & `pulumi_rancher2-6.2.0a1713561342/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 6.2.0a1713337589
+Version: 6.2.0a1713561342
 Summary: A Pulumi package for creating and managing rancher2 resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi,rancher2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/README.md` & `pulumi_rancher2-6.2.0a1713561342/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/__init__.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/_inputs.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/_utilities.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/app.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -530,51 +530,54 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 App
         foo = rancher2.App("foo",
-            answers={
-                "foo": "bar",
-                "ingress.annotations.nginx.ingress.kubernetes.io/force-ssl-redirect": True,
-                "ingress_host": "test.xip.io",
-            },
             catalog_name="<catalog_name>",
+            name="foo",
             description="Foo app",
             project_id="<project_id>",
-            target_namespace="<namespace_name>",
             template_name="<template_name>",
-            template_version="<template_version>")
+            template_version="<template_version>",
+            target_namespace="<namespace_name>",
+            answers={
+                "ingress_host": "test.xip.io",
+                "foo": "bar",
+                "ingress.annotations.nginx.ingress.kubernetes.io/force-ssl-redirect": True,
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 App in a new namespace
-        foo_namespace = rancher2.Namespace("fooNamespace",
+        foo = rancher2.Namespace("foo",
+            name="foo",
             description="Foo namespace",
             project_id="<project_id>",
             resource_quota=rancher2.NamespaceResourceQuotaArgs(
                 limit=rancher2.NamespaceResourceQuotaLimitArgs(
                     limits_cpu="100m",
                     limits_memory="100Mi",
                     requests_storage="1Gi",
                 ),
             ))
-        foo_app = rancher2.App("fooApp",
+        foo_app = rancher2.App("foo",
             catalog_name="<catalog_name>",
+            name="foo",
             description="Foo app",
             project_id="<project_id>",
             template_name="<template_name>",
             template_version="<template_version>",
-            target_namespace=foo_namespace.id,
+            target_namespace=foo.id,
             answers={
                 "ingress_host": "test.xip.io",
                 "foo": "bar",
                 "ingress.annotations.nginx.ingress.kubernetes.io/force-ssl-redirect": True,
             })
         ```
         <!--End PulumiCodeChooser -->
@@ -627,51 +630,54 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 App
         foo = rancher2.App("foo",
-            answers={
-                "foo": "bar",
-                "ingress.annotations.nginx.ingress.kubernetes.io/force-ssl-redirect": True,
-                "ingress_host": "test.xip.io",
-            },
             catalog_name="<catalog_name>",
+            name="foo",
             description="Foo app",
             project_id="<project_id>",
-            target_namespace="<namespace_name>",
             template_name="<template_name>",
-            template_version="<template_version>")
+            template_version="<template_version>",
+            target_namespace="<namespace_name>",
+            answers={
+                "ingress_host": "test.xip.io",
+                "foo": "bar",
+                "ingress.annotations.nginx.ingress.kubernetes.io/force-ssl-redirect": True,
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 App in a new namespace
-        foo_namespace = rancher2.Namespace("fooNamespace",
+        foo = rancher2.Namespace("foo",
+            name="foo",
             description="Foo namespace",
             project_id="<project_id>",
             resource_quota=rancher2.NamespaceResourceQuotaArgs(
                 limit=rancher2.NamespaceResourceQuotaLimitArgs(
                     limits_cpu="100m",
                     limits_memory="100Mi",
                     requests_storage="1Gi",
                 ),
             ))
-        foo_app = rancher2.App("fooApp",
+        foo_app = rancher2.App("foo",
             catalog_name="<catalog_name>",
+            name="foo",
             description="Foo app",
             project_id="<project_id>",
             template_name="<template_name>",
             template_version="<template_version>",
-            target_namespace=foo_namespace.id,
+            target_namespace=foo.id,
             answers={
                 "ingress_host": "test.xip.io",
                 "foo": "bar",
                 "ingress.annotations.nginx.ingress.kubernetes.io/force-ssl-redirect": True,
             })
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/app_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/app_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -598,40 +598,43 @@
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
+        import pulumi_std as std
 
         # Create a new Rancher2 App V2 using
         foo = rancher2.AppV2("foo",
             cluster_id="<CLUSTER_ID>",
+            name="rancher-monitoring",
             namespace="cattle-monitoring-system",
             repo_name="rancher-charts",
             chart_name="rancher-monitoring",
             chart_version="9.4.200",
-            values=(lambda path: open(path).read())("values.yaml"))
+            values=std.file(input="values.yaml").result)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Create an App from a Helm Chart using a different registry
 
         The `system_default_registry` argument can override the global value at App installation. If argument is not provided, the global value for System Default Registry will be used instead.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        cis_benchmark = rancher2.AppV2("cisBenchmark",
-            chart_name="rancher-cis-benchmark",
+        cis_benchmark = rancher2.AppV2("cis_benchmark",
             cluster_id="<CLUSTER_ID>",
+            name="rancher-cis-benchmark",
             namespace="cis-operator-system",
             repo_name="rancher-charts",
+            chart_name="rancher-cis-benchmark",
             system_default_registry="<some.dns.here>:<PORT>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         V2 apps can be imported using the Rancher cluster ID and App V2 name, which is composed of `<namespace>/<application_name>`.
@@ -670,40 +673,43 @@
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
+        import pulumi_std as std
 
         # Create a new Rancher2 App V2 using
         foo = rancher2.AppV2("foo",
             cluster_id="<CLUSTER_ID>",
+            name="rancher-monitoring",
             namespace="cattle-monitoring-system",
             repo_name="rancher-charts",
             chart_name="rancher-monitoring",
             chart_version="9.4.200",
-            values=(lambda path: open(path).read())("values.yaml"))
+            values=std.file(input="values.yaml").result)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Create an App from a Helm Chart using a different registry
 
         The `system_default_registry` argument can override the global value at App installation. If argument is not provided, the global value for System Default Registry will be used instead.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        cis_benchmark = rancher2.AppV2("cisBenchmark",
-            chart_name="rancher-cis-benchmark",
+        cis_benchmark = rancher2.AppV2("cis_benchmark",
             cluster_id="<CLUSTER_ID>",
+            name="rancher-cis-benchmark",
             namespace="cis-operator-system",
             repo_name="rancher-charts",
+            chart_name="rancher-cis-benchmark",
             system_default_registry="<some.dns.here>:<PORT>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         V2 apps can be imported using the Rancher cluster ID and App V2 name, which is composed of `<namespace>/<application_name>`.
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_active_directory.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_adfs.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_adfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_azure_ad.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_free_ipa.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_free_ipa.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_github.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_keycloak.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_keycloak.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_okta.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_open_ldap.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_open_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/auth_config_ping.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/auth_config_ping.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/bootstrap.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,23 +372,18 @@
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        # Provider bootstrap config with alias
-        bootstrap = rancher2.Provider("bootstrap",
-            api_url="https://rancher.my-domain.com",
-            bootstrap=True)
         # Create a new rancher2_bootstrap using bootstrap provider config
         admin = rancher2.Bootstrap("admin",
             password="blahblah",
-            telemetry=True,
-            opts=pulumi.ResourceOptions(provider="rancher2.bootstrap"))
+            telemetry=True)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] initial_password: Initial password for Admin user. Default: `admin` (string)
         :param pulumi.Input[str] password: Password for Admin user or random generated if empty (string)
@@ -432,23 +427,18 @@
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        # Provider bootstrap config with alias
-        bootstrap = rancher2.Provider("bootstrap",
-            api_url="https://rancher.my-domain.com",
-            bootstrap=True)
         # Create a new rancher2_bootstrap using bootstrap provider config
         admin = rancher2.Bootstrap("admin",
             password="blahblah",
-            telemetry=True,
-            opts=pulumi.ResourceOptions(provider="rancher2.bootstrap"))
+            telemetry=True)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param BootstrapArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/catalog.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,23 +501,27 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Global Catalog
-        foo_global = rancher2.Catalog("foo-global", url="https://<CATALOG_URL>")
+        foo_global = rancher2.Catalog("foo-global",
+            name="foo-global",
+            url="https://<CATALOG_URL>")
         # Create a new Rancher2 Cluster Catalog
         foo_cluster = rancher2.Catalog("foo-cluster",
-            scope="cluster",
-            url="https://<CATALOG_URL>")
+            name="foo-cluster",
+            url="https://<CATALOG_URL>",
+            scope="cluster")
         # Create a new Rancher2 Project Catalog
         foo_project = rancher2.Catalog("foo-project",
-            scope="project",
-            url="https://<CATALOG_URL>")
+            name="foo-project",
+            url="https://<CATALOG_URL>",
+            scope="project")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Catalogs can be imported using the Rancher Catalog ID and its scope.
 
@@ -555,23 +559,27 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Global Catalog
-        foo_global = rancher2.Catalog("foo-global", url="https://<CATALOG_URL>")
+        foo_global = rancher2.Catalog("foo-global",
+            name="foo-global",
+            url="https://<CATALOG_URL>")
         # Create a new Rancher2 Cluster Catalog
         foo_cluster = rancher2.Catalog("foo-cluster",
-            scope="cluster",
-            url="https://<CATALOG_URL>")
+            name="foo-cluster",
+            url="https://<CATALOG_URL>",
+            scope="cluster")
         # Create a new Rancher2 Project Catalog
         foo_project = rancher2.Catalog("foo-project",
-            scope="project",
-            url="https://<CATALOG_URL>")
+            name="foo-project",
+            url="https://<CATALOG_URL>",
+            scope="project")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Catalogs can be imported using the Rancher Catalog ID and its scope.
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/catalog_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/certificate.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cloud_credential.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cloud_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -490,34 +490,38 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Cloud Credential
         foo = rancher2.CloudCredential("foo",
+            name="foo",
+            description="foo test",
             amazonec2_credential_config=rancher2.CloudCredentialAmazonec2CredentialConfigArgs(
                 access_key="<AWS_ACCESS_KEY>",
                 secret_key="<AWS_SECRET_KEY>",
-            ),
-            description="foo test")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_harvester_cluster_v2 = rancher2.get_cluster_v2(name="foo-harvester")
+        # Get imported harvester cluster info
+        foo_harvester = rancher2.get_cluster_v2(name="foo-harvester")
         # Create a new Cloud Credential for an imported Harvester cluster
-        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvesterCloudCredential", harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
-            cluster_id=foo_harvester_cluster_v2.cluster_v1_id,
-            cluster_type="imported",
-            kubeconfig_content=foo_harvester_cluster_v2.kube_config,
-        ))
+        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvester",
+            name="foo-harvester",
+            harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
+                cluster_id=foo_harvester.cluster_v1_id,
+                cluster_type="imported",
+                kubeconfig_content=foo_harvester.kube_config,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Cloud Credential can be imported using the Cloud Credential ID and the Driver name.
 
@@ -577,34 +581,38 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Cloud Credential
         foo = rancher2.CloudCredential("foo",
+            name="foo",
+            description="foo test",
             amazonec2_credential_config=rancher2.CloudCredentialAmazonec2CredentialConfigArgs(
                 access_key="<AWS_ACCESS_KEY>",
                 secret_key="<AWS_SECRET_KEY>",
-            ),
-            description="foo test")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_harvester_cluster_v2 = rancher2.get_cluster_v2(name="foo-harvester")
+        # Get imported harvester cluster info
+        foo_harvester = rancher2.get_cluster_v2(name="foo-harvester")
         # Create a new Cloud Credential for an imported Harvester cluster
-        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvesterCloudCredential", harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
-            cluster_id=foo_harvester_cluster_v2.cluster_v1_id,
-            cluster_type="imported",
-            kubeconfig_content=foo_harvester_cluster_v2.kube_config,
-        ))
+        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvester",
+            name="foo-harvester",
+            harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
+                cluster_id=foo_harvester.cluster_v1_id,
+                cluster_type="imported",
+                kubeconfig_content=foo_harvester.kube_config,
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Cloud Credential can be imported using the Cloud Credential ID and the Driver name.
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1286,15 +1286,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 imported Cluster
-        foo_imported = rancher2.Cluster("foo-imported", description="Foo rancher2 imported cluster")
+        foo_imported = rancher2.Cluster("foo-imported",
+            name="foo-imported",
+            description="Foo rancher2 imported cluster")
         ```
         <!--End PulumiCodeChooser -->
 
         Creating Rancher v2 RKE cluster
 
         ### Creating Rancher v2 RKE cluster enabling and customizing monitoring
 
@@ -1303,14 +1305,22 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 RKE Cluster
         foo_custom = rancher2.Cluster("foo-custom",
+            name="foo-custom",
+            description="Foo rancher2 custom cluster",
+            rke_config=rancher2.ClusterRkeConfigArgs(
+                network=rancher2.ClusterRkeConfigNetworkArgs(
+                    plugin="canal",
+                ),
+            ),
+            enable_cluster_monitoring=True,
             cluster_monitoring_input=rancher2.ClusterClusterMonitoringInputArgs(
                 answers={
                     "exporter-kubelets.https": True,
                     "exporter-node.enabled": True,
                     "exporter-node.ports.metrics.port": 9796,
                     "exporter-node.resources.limits.cpu": "200m",
                     "exporter-node.resources.limits.memory": "200Mi",
@@ -1325,34 +1335,28 @@
                     "prometheus.resources.core.limits.cpu": "1000m",
                     "prometheus.resources.core.limits.memory": "1500Mi",
                     "prometheus.resources.core.requests.cpu": "750m",
                     "prometheus.resources.core.requests.memory": "750Mi",
                     "prometheus.retention": "12h",
                 },
                 version="0.1.0",
-            ),
-            description="Foo rancher2 custom cluster",
-            enable_cluster_monitoring=True,
-            rke_config=rancher2.ClusterRkeConfigArgs(
-                network=rancher2.ClusterRkeConfigNetworkArgs(
-                    plugin="canal",
-                ),
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating Rancher v2 RKE cluster enabling/customizing monitoring and istio
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 RKE Cluster
-        foo_custom_cluster = rancher2.Cluster("foo-customCluster",
+        foo_custom = rancher2.Cluster("foo-custom",
+            name="foo-custom",
             description="Foo rancher2 custom cluster",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
             ),
             enable_cluster_monitoring=True,
@@ -1376,24 +1380,26 @@
                     "prometheus.resources.core.requests.cpu": "750m",
                     "prometheus.resources.core.requests.memory": "750Mi",
                     "prometheus.retention": "12h",
                 },
                 version="0.1.0",
             ))
         # Create a new rancher2 Cluster Sync for foo-custom cluster
-        foo_custom_cluster_sync = rancher2.ClusterSync("foo-customClusterSync",
-            cluster_id=foo_custom_cluster.id,
-            wait_monitoring=foo_custom_cluster.enable_cluster_monitoring)
+        foo_custom_cluster_sync = rancher2.ClusterSync("foo-custom",
+            cluster_id=foo_custom.id,
+            wait_monitoring=foo_custom.enable_cluster_monitoring)
         # Create a new rancher2 Namespace
         foo_istio = rancher2.Namespace("foo-istio",
+            name="istio-system",
             project_id=foo_custom_cluster_sync.system_project_id,
             description="istio namespace")
         # Create a new rancher2 App deploying istio (should wait until monitoring is up and running)
         istio = rancher2.App("istio",
             catalog_name="system-library",
+            name="cluster-istio",
             description="Terraform app acceptance test",
             project_id=foo_istio.project_id,
             template_name="rancher-istio",
             template_version="0.1.1",
             target_namespace=foo_istio.id,
             answers={
                 "certmanager.enabled": False,
@@ -1444,38 +1450,41 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 RKE Cluster
         foo_custom = rancher2.Cluster("foo-custom",
+            name="foo-custom",
             description="Foo rancher2 custom cluster",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
             ))
         # Create a new rancher2 Node Template
-        foo_node_template = rancher2.NodeTemplate("fooNodeTemplate",
+        foo = rancher2.NodeTemplate("foo",
+            name="foo",
             description="foo test",
             amazonec2_config=rancher2.NodeTemplateAmazonec2ConfigArgs(
                 access_key="<AWS_ACCESS_KEY>",
                 secret_key="<AWS_SECRET_KEY>",
                 ami="<AMI_ID>",
                 region="<REGION>",
                 security_groups=["<AWS_SECURITY_GROUP>"],
                 subnet_id="<SUBNET_ID>",
                 vpc_id="<VPC_ID>",
                 zone="<ZONE>",
             ))
         # Create a new rancher2 Node Pool
-        foo_node_pool = rancher2.NodePool("fooNodePool",
+        foo_node_pool = rancher2.NodePool("foo",
             cluster_id=foo_custom.id,
+            name="foo",
             hostname_prefix="foo-cluster-0",
-            node_template_id=foo_node_template.id,
+            node_template_id=foo.id,
             quantity=3,
             control_plane=True,
             etcd=True,
             worker=True)
         ```
         <!--End PulumiCodeChooser -->
 
@@ -1483,15 +1492,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 cluster template
-        foo_cluster_template = rancher2.ClusterTemplate("fooClusterTemplate",
+        foo = rancher2.ClusterTemplate("foo",
+            name="foo",
             members=[rancher2.ClusterTemplateMemberArgs(
                 access_type="owner",
                 user_principal_id="local://user-XXXXX",
             )],
             template_revisions=[rancher2.ClusterTemplateTemplateRevisionArgs(
                 name="V1",
                 cluster_config=rancher2.ClusterTemplateTemplateRevisionClusterConfigArgs(
@@ -1507,61 +1517,62 @@
                         ),
                     ),
                 ),
                 default=True,
             )],
             description="Test cluster template v2")
         # Create a new rancher2 RKE Cluster from template
-        foo_cluster = rancher2.Cluster("fooCluster",
-            cluster_template_id=foo_cluster_template.id,
-            cluster_template_revision_id=foo_cluster_template.template_revisions[0].id)
+        foo_cluster = rancher2.Cluster("foo",
+            name="foo",
+            cluster_template_id=foo.id,
+            cluster_template_revision_id=foo.template_revisions[0].id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating Rancher v2 RKE cluster with upgrade strategy. For Rancher v2.4.x and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform custom cluster",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
                 services=rancher2.ClusterRkeConfigServicesArgs(
                     etcd=rancher2.ClusterRkeConfigServicesEtcdArgs(
                         creation="6h",
                         retention="24h",
                     ),
                     kube_api=rancher2.ClusterRkeConfigServicesKubeApiArgs(
                         audit_log=rancher2.ClusterRkeConfigServicesKubeApiAuditLogArgs(
+                            enabled=True,
                             configuration=rancher2.ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs(
-                                format="json",
                                 max_age=5,
                                 max_backup=5,
                                 max_size=100,
                                 path="-",
+                                format="json",
                                 policy=\"\"\"apiVersion: audit.k8s.io/v1
         kind: Policy
         metadata:
           creationTimestamp: null
         omitStages:
         - RequestReceived
         rules:
         - level: RequestResponse
           resources:
           - resources:
             - pods
-
         \"\"\",
                             ),
-                            enabled=True,
                         ),
                     ),
                 ),
                 upgrade_strategy=rancher2.ClusterRkeConfigUpgradeStrategyArgs(
                     drain=True,
                     max_unavailable_worker="20%",
                 ),
@@ -1573,14 +1584,21 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo = rancher2.Cluster("foo",
+            name="foo",
+            description="Terraform cluster with agent customization",
+            rke_config=rancher2.ClusterRkeConfigArgs(
+                network=rancher2.ClusterRkeConfigNetworkArgs(
+                    plugin="canal",
+                ),
+            ),
             cluster_agent_deployment_customizations=[rancher2.ClusterClusterAgentDeploymentCustomizationArgs(
                 append_tolerations=[rancher2.ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs(
                     effect="NoSchedule",
                     key="tolerate/control-plane",
                     value="true",
                 )],
                 override_affinity=\"\"\"{
@@ -1594,61 +1612,56 @@
                     "true"
                   ]
                 }]
               }]
             }
           }
         }
-
         \"\"\",
                 override_resource_requirements=[rancher2.ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs(
                     cpu_limit="800",
                     cpu_request="500",
                     memory_limit="800",
                     memory_request="500",
                 )],
-            )],
-            description="Terraform cluster with agent customization",
-            rke_config=rancher2.ClusterRkeConfigArgs(
-                network=rancher2.ClusterRkeConfigNetworkArgs(
-                    plugin="canal",
-                ),
-            ))
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating Rancher v2 RKE cluster with Pod Security Admission Configuration Template (PSACT). For Rancher v2.7.2 and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Custom PSACT (if you wish to use your own)
-        foo_pod_security_admission_configuration_template = rancher2.PodSecurityAdmissionConfigurationTemplate("fooPodSecurityAdmissionConfigurationTemplate",
+        foo = rancher2.PodSecurityAdmissionConfigurationTemplate("foo",
+            name="custom-psact",
+            description="This is my custom Pod Security Admission Configuration Template",
             defaults=rancher2.PodSecurityAdmissionConfigurationTemplateDefaultsArgs(
                 audit="restricted",
                 audit_version="latest",
                 enforce="restricted",
                 enforce_version="latest",
                 warn="restricted",
                 warn_version="latest",
             ),
-            description="This is my custom Pod Security Admission Configuration Template",
             exemptions=rancher2.PodSecurityAdmissionConfigurationTemplateExemptionsArgs(
+                usernames=["testuser"],
+                runtime_classes=["testclass"],
                 namespaces=[
                     "ingress-nginx",
                     "kube-system",
                 ],
-                runtime_classes=["testclass"],
-                usernames=["testuser"],
             ))
-        foo_cluster = rancher2.Cluster("fooCluster",
-            default_pod_security_admission_configuration_template_name="<name>",
+        foo_cluster = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform cluster with PSACT",
+            default_pod_security_admission_configuration_template_name="<name>",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
             ))
         ```
         <!--End PulumiCodeChooser -->
@@ -1656,48 +1669,52 @@
         ### Importing EKS cluster to Rancher v2, using `eks_config_v2`. For Rancher v2.5.x and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
+        foo = rancher2.CloudCredential("foo",
+            name="foo",
             description="foo test",
             amazonec2_credential_config=rancher2.CloudCredentialAmazonec2CredentialConfigArgs(
                 access_key="<aws-access-key>",
                 secret_key="<aws-secret-key>",
             ))
-        foo_cluster = rancher2.Cluster("fooCluster",
+        foo_cluster = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform EKS cluster",
             eks_config_v2=rancher2.ClusterEksConfigV2Args(
-                cloud_credential_id=foo_cloud_credential.id,
+                cloud_credential_id=foo.id,
                 name="<cluster-name>",
                 region="<eks-region>",
                 imported=True,
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating EKS cluster from Rancher v2, using `eks_config_v2`. For Rancher v2.5.x and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
+        foo = rancher2.CloudCredential("foo",
+            name="foo",
             description="foo test",
             amazonec2_credential_config=rancher2.CloudCredentialAmazonec2CredentialConfigArgs(
                 access_key="<aws-access-key>",
                 secret_key="<aws-secret-key>",
             ))
-        foo_cluster = rancher2.Cluster("fooCluster",
+        foo_cluster = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform EKS cluster",
             eks_config_v2=rancher2.ClusterEksConfigV2Args(
-                cloud_credential_id=foo_cloud_credential.id,
+                cloud_credential_id=foo.id,
                 region="<EKS_REGION>",
                 kubernetes_version="1.24",
                 logging_types=[
                     "audit",
                     "api",
                 ],
                 node_groups=[
@@ -1726,24 +1743,26 @@
         Note: To use `launch_template` you must provide the ID (seen as `<EC2_LAUNCH_TEMPLATE_ID>`) to the template either as a static value. Or fetched via AWS data-source using one of: aws_ami first and provide the ID to that.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
+        foo = rancher2.CloudCredential("foo",
+            name="foo",
             description="foo test",
             amazonec2_credential_config=rancher2.CloudCredentialAmazonec2CredentialConfigArgs(
                 access_key="<aws-access-key>",
                 secret_key="<aws-secret-key>",
             ))
-        foo_cluster = rancher2.Cluster("fooCluster",
+        foo_cluster = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform EKS cluster",
             eks_config_v2=rancher2.ClusterEksConfigV2Args(
-                cloud_credential_id=foo_cloud_credential.id,
+                cloud_credential_id=foo.id,
                 region="<EKS_REGION>",
                 kubernetes_version="1.24",
                 logging_types=[
                     "audit",
                     "api",
                 ],
                 node_groups=[rancher2.ClusterEksConfigV2NodeGroupArgs(
@@ -1764,20 +1783,23 @@
         ### Creating AKS cluster from Rancher v2, using `aks_config_v2`. For Rancher v2.6.0 and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_aks = rancher2.CloudCredential("foo-aks", azure_credential_config=rancher2.CloudCredentialAzureCredentialConfigArgs(
-            client_id="<client-id>",
-            client_secret="<client-secret>",
-            subscription_id="<subscription-id>",
-        ))
+        foo_aks = rancher2.CloudCredential("foo-aks",
+            name="foo-aks",
+            azure_credential_config=rancher2.CloudCredentialAzureCredentialConfigArgs(
+                client_id="<client-id>",
+                client_secret="<client-secret>",
+                subscription_id="<subscription-id>",
+            ))
         foo = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform AKS cluster",
             aks_config_v2=rancher2.ClusterAksConfigV2Args(
                 cloud_credential_id=foo_aks.id,
                 resource_group="<resource-group>",
                 resource_location="<resource-location>",
                 dns_prefix="<dns-prefix>",
                 kubernetes_version="1.24.6",
@@ -1882,15 +1904,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 imported Cluster
-        foo_imported = rancher2.Cluster("foo-imported", description="Foo rancher2 imported cluster")
+        foo_imported = rancher2.Cluster("foo-imported",
+            name="foo-imported",
+            description="Foo rancher2 imported cluster")
         ```
         <!--End PulumiCodeChooser -->
 
         Creating Rancher v2 RKE cluster
 
         ### Creating Rancher v2 RKE cluster enabling and customizing monitoring
 
@@ -1899,14 +1923,22 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 RKE Cluster
         foo_custom = rancher2.Cluster("foo-custom",
+            name="foo-custom",
+            description="Foo rancher2 custom cluster",
+            rke_config=rancher2.ClusterRkeConfigArgs(
+                network=rancher2.ClusterRkeConfigNetworkArgs(
+                    plugin="canal",
+                ),
+            ),
+            enable_cluster_monitoring=True,
             cluster_monitoring_input=rancher2.ClusterClusterMonitoringInputArgs(
                 answers={
                     "exporter-kubelets.https": True,
                     "exporter-node.enabled": True,
                     "exporter-node.ports.metrics.port": 9796,
                     "exporter-node.resources.limits.cpu": "200m",
                     "exporter-node.resources.limits.memory": "200Mi",
@@ -1921,34 +1953,28 @@
                     "prometheus.resources.core.limits.cpu": "1000m",
                     "prometheus.resources.core.limits.memory": "1500Mi",
                     "prometheus.resources.core.requests.cpu": "750m",
                     "prometheus.resources.core.requests.memory": "750Mi",
                     "prometheus.retention": "12h",
                 },
                 version="0.1.0",
-            ),
-            description="Foo rancher2 custom cluster",
-            enable_cluster_monitoring=True,
-            rke_config=rancher2.ClusterRkeConfigArgs(
-                network=rancher2.ClusterRkeConfigNetworkArgs(
-                    plugin="canal",
-                ),
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating Rancher v2 RKE cluster enabling/customizing monitoring and istio
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 RKE Cluster
-        foo_custom_cluster = rancher2.Cluster("foo-customCluster",
+        foo_custom = rancher2.Cluster("foo-custom",
+            name="foo-custom",
             description="Foo rancher2 custom cluster",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
             ),
             enable_cluster_monitoring=True,
@@ -1972,24 +1998,26 @@
                     "prometheus.resources.core.requests.cpu": "750m",
                     "prometheus.resources.core.requests.memory": "750Mi",
                     "prometheus.retention": "12h",
                 },
                 version="0.1.0",
             ))
         # Create a new rancher2 Cluster Sync for foo-custom cluster
-        foo_custom_cluster_sync = rancher2.ClusterSync("foo-customClusterSync",
-            cluster_id=foo_custom_cluster.id,
-            wait_monitoring=foo_custom_cluster.enable_cluster_monitoring)
+        foo_custom_cluster_sync = rancher2.ClusterSync("foo-custom",
+            cluster_id=foo_custom.id,
+            wait_monitoring=foo_custom.enable_cluster_monitoring)
         # Create a new rancher2 Namespace
         foo_istio = rancher2.Namespace("foo-istio",
+            name="istio-system",
             project_id=foo_custom_cluster_sync.system_project_id,
             description="istio namespace")
         # Create a new rancher2 App deploying istio (should wait until monitoring is up and running)
         istio = rancher2.App("istio",
             catalog_name="system-library",
+            name="cluster-istio",
             description="Terraform app acceptance test",
             project_id=foo_istio.project_id,
             template_name="rancher-istio",
             template_version="0.1.1",
             target_namespace=foo_istio.id,
             answers={
                 "certmanager.enabled": False,
@@ -2040,38 +2068,41 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 RKE Cluster
         foo_custom = rancher2.Cluster("foo-custom",
+            name="foo-custom",
             description="Foo rancher2 custom cluster",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
             ))
         # Create a new rancher2 Node Template
-        foo_node_template = rancher2.NodeTemplate("fooNodeTemplate",
+        foo = rancher2.NodeTemplate("foo",
+            name="foo",
             description="foo test",
             amazonec2_config=rancher2.NodeTemplateAmazonec2ConfigArgs(
                 access_key="<AWS_ACCESS_KEY>",
                 secret_key="<AWS_SECRET_KEY>",
                 ami="<AMI_ID>",
                 region="<REGION>",
                 security_groups=["<AWS_SECURITY_GROUP>"],
                 subnet_id="<SUBNET_ID>",
                 vpc_id="<VPC_ID>",
                 zone="<ZONE>",
             ))
         # Create a new rancher2 Node Pool
-        foo_node_pool = rancher2.NodePool("fooNodePool",
+        foo_node_pool = rancher2.NodePool("foo",
             cluster_id=foo_custom.id,
+            name="foo",
             hostname_prefix="foo-cluster-0",
-            node_template_id=foo_node_template.id,
+            node_template_id=foo.id,
             quantity=3,
             control_plane=True,
             etcd=True,
             worker=True)
         ```
         <!--End PulumiCodeChooser -->
 
@@ -2079,15 +2110,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 cluster template
-        foo_cluster_template = rancher2.ClusterTemplate("fooClusterTemplate",
+        foo = rancher2.ClusterTemplate("foo",
+            name="foo",
             members=[rancher2.ClusterTemplateMemberArgs(
                 access_type="owner",
                 user_principal_id="local://user-XXXXX",
             )],
             template_revisions=[rancher2.ClusterTemplateTemplateRevisionArgs(
                 name="V1",
                 cluster_config=rancher2.ClusterTemplateTemplateRevisionClusterConfigArgs(
@@ -2103,61 +2135,62 @@
                         ),
                     ),
                 ),
                 default=True,
             )],
             description="Test cluster template v2")
         # Create a new rancher2 RKE Cluster from template
-        foo_cluster = rancher2.Cluster("fooCluster",
-            cluster_template_id=foo_cluster_template.id,
-            cluster_template_revision_id=foo_cluster_template.template_revisions[0].id)
+        foo_cluster = rancher2.Cluster("foo",
+            name="foo",
+            cluster_template_id=foo.id,
+            cluster_template_revision_id=foo.template_revisions[0].id)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating Rancher v2 RKE cluster with upgrade strategy. For Rancher v2.4.x and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform custom cluster",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
                 services=rancher2.ClusterRkeConfigServicesArgs(
                     etcd=rancher2.ClusterRkeConfigServicesEtcdArgs(
                         creation="6h",
                         retention="24h",
                     ),
                     kube_api=rancher2.ClusterRkeConfigServicesKubeApiArgs(
                         audit_log=rancher2.ClusterRkeConfigServicesKubeApiAuditLogArgs(
+                            enabled=True,
                             configuration=rancher2.ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs(
-                                format="json",
                                 max_age=5,
                                 max_backup=5,
                                 max_size=100,
                                 path="-",
+                                format="json",
                                 policy=\"\"\"apiVersion: audit.k8s.io/v1
         kind: Policy
         metadata:
           creationTimestamp: null
         omitStages:
         - RequestReceived
         rules:
         - level: RequestResponse
           resources:
           - resources:
             - pods
-
         \"\"\",
                             ),
-                            enabled=True,
                         ),
                     ),
                 ),
                 upgrade_strategy=rancher2.ClusterRkeConfigUpgradeStrategyArgs(
                     drain=True,
                     max_unavailable_worker="20%",
                 ),
@@ -2169,14 +2202,21 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         foo = rancher2.Cluster("foo",
+            name="foo",
+            description="Terraform cluster with agent customization",
+            rke_config=rancher2.ClusterRkeConfigArgs(
+                network=rancher2.ClusterRkeConfigNetworkArgs(
+                    plugin="canal",
+                ),
+            ),
             cluster_agent_deployment_customizations=[rancher2.ClusterClusterAgentDeploymentCustomizationArgs(
                 append_tolerations=[rancher2.ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs(
                     effect="NoSchedule",
                     key="tolerate/control-plane",
                     value="true",
                 )],
                 override_affinity=\"\"\"{
@@ -2190,61 +2230,56 @@
                     "true"
                   ]
                 }]
               }]
             }
           }
         }
-
         \"\"\",
                 override_resource_requirements=[rancher2.ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs(
                     cpu_limit="800",
                     cpu_request="500",
                     memory_limit="800",
                     memory_request="500",
                 )],
-            )],
-            description="Terraform cluster with agent customization",
-            rke_config=rancher2.ClusterRkeConfigArgs(
-                network=rancher2.ClusterRkeConfigNetworkArgs(
-                    plugin="canal",
-                ),
-            ))
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating Rancher v2 RKE cluster with Pod Security Admission Configuration Template (PSACT). For Rancher v2.7.2 and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Custom PSACT (if you wish to use your own)
-        foo_pod_security_admission_configuration_template = rancher2.PodSecurityAdmissionConfigurationTemplate("fooPodSecurityAdmissionConfigurationTemplate",
+        foo = rancher2.PodSecurityAdmissionConfigurationTemplate("foo",
+            name="custom-psact",
+            description="This is my custom Pod Security Admission Configuration Template",
             defaults=rancher2.PodSecurityAdmissionConfigurationTemplateDefaultsArgs(
                 audit="restricted",
                 audit_version="latest",
                 enforce="restricted",
                 enforce_version="latest",
                 warn="restricted",
                 warn_version="latest",
             ),
-            description="This is my custom Pod Security Admission Configuration Template",
             exemptions=rancher2.PodSecurityAdmissionConfigurationTemplateExemptionsArgs(
+                usernames=["testuser"],
+                runtime_classes=["testclass"],
                 namespaces=[
                     "ingress-nginx",
                     "kube-system",
                 ],
-                runtime_classes=["testclass"],
-                usernames=["testuser"],
             ))
-        foo_cluster = rancher2.Cluster("fooCluster",
-            default_pod_security_admission_configuration_template_name="<name>",
+        foo_cluster = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform cluster with PSACT",
+            default_pod_security_admission_configuration_template_name="<name>",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
             ))
         ```
         <!--End PulumiCodeChooser -->
@@ -2252,48 +2287,52 @@
         ### Importing EKS cluster to Rancher v2, using `eks_config_v2`. For Rancher v2.5.x and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
+        foo = rancher2.CloudCredential("foo",
+            name="foo",
             description="foo test",
             amazonec2_credential_config=rancher2.CloudCredentialAmazonec2CredentialConfigArgs(
                 access_key="<aws-access-key>",
                 secret_key="<aws-secret-key>",
             ))
-        foo_cluster = rancher2.Cluster("fooCluster",
+        foo_cluster = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform EKS cluster",
             eks_config_v2=rancher2.ClusterEksConfigV2Args(
-                cloud_credential_id=foo_cloud_credential.id,
+                cloud_credential_id=foo.id,
                 name="<cluster-name>",
                 region="<eks-region>",
                 imported=True,
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating EKS cluster from Rancher v2, using `eks_config_v2`. For Rancher v2.5.x and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
+        foo = rancher2.CloudCredential("foo",
+            name="foo",
             description="foo test",
             amazonec2_credential_config=rancher2.CloudCredentialAmazonec2CredentialConfigArgs(
                 access_key="<aws-access-key>",
                 secret_key="<aws-secret-key>",
             ))
-        foo_cluster = rancher2.Cluster("fooCluster",
+        foo_cluster = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform EKS cluster",
             eks_config_v2=rancher2.ClusterEksConfigV2Args(
-                cloud_credential_id=foo_cloud_credential.id,
+                cloud_credential_id=foo.id,
                 region="<EKS_REGION>",
                 kubernetes_version="1.24",
                 logging_types=[
                     "audit",
                     "api",
                 ],
                 node_groups=[
@@ -2322,24 +2361,26 @@
         Note: To use `launch_template` you must provide the ID (seen as `<EC2_LAUNCH_TEMPLATE_ID>`) to the template either as a static value. Or fetched via AWS data-source using one of: aws_ami first and provide the ID to that.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
+        foo = rancher2.CloudCredential("foo",
+            name="foo",
             description="foo test",
             amazonec2_credential_config=rancher2.CloudCredentialAmazonec2CredentialConfigArgs(
                 access_key="<aws-access-key>",
                 secret_key="<aws-secret-key>",
             ))
-        foo_cluster = rancher2.Cluster("fooCluster",
+        foo_cluster = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform EKS cluster",
             eks_config_v2=rancher2.ClusterEksConfigV2Args(
-                cloud_credential_id=foo_cloud_credential.id,
+                cloud_credential_id=foo.id,
                 region="<EKS_REGION>",
                 kubernetes_version="1.24",
                 logging_types=[
                     "audit",
                     "api",
                 ],
                 node_groups=[rancher2.ClusterEksConfigV2NodeGroupArgs(
@@ -2360,20 +2401,23 @@
         ### Creating AKS cluster from Rancher v2, using `aks_config_v2`. For Rancher v2.6.0 and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_aks = rancher2.CloudCredential("foo-aks", azure_credential_config=rancher2.CloudCredentialAzureCredentialConfigArgs(
-            client_id="<client-id>",
-            client_secret="<client-secret>",
-            subscription_id="<subscription-id>",
-        ))
+        foo_aks = rancher2.CloudCredential("foo-aks",
+            name="foo-aks",
+            azure_credential_config=rancher2.CloudCredentialAzureCredentialConfigArgs(
+                client_id="<client-id>",
+                client_secret="<client-secret>",
+                subscription_id="<subscription-id>",
+            ))
         foo = rancher2.Cluster("foo",
+            name="foo",
             description="Terraform AKS cluster",
             aks_config_v2=rancher2.ClusterAksConfigV2Args(
                 cloud_credential_id=foo_aks.id,
                 resource_group="<resource-group>",
                 resource_location="<resource-location>",
                 dns_prefix="<dns-prefix>",
                 kubernetes_version="1.24.6",
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_alert_group.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_alert_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,14 +340,15 @@
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Cluster Alert Group
         foo = rancher2.ClusterAlertGroup("foo",
             cluster_id="<cluster_id>",
+            name="foo",
             description="Terraform cluster alert group",
             group_interval_seconds=300,
             repeat_interval_seconds=3600)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -385,14 +386,15 @@
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Cluster Alert Group
         foo = rancher2.ClusterAlertGroup("foo",
             cluster_id="<cluster_id>",
+            name="foo",
             description="Terraform cluster alert group",
             group_interval_seconds=300,
             repeat_interval_seconds=3600)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_alert_rule.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_alert_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,23 +502,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Cluster Alert Group
-        foo_cluster_alert_group = rancher2.ClusterAlertGroup("fooClusterAlertGroup",
+        foo = rancher2.ClusterAlertGroup("foo",
             cluster_id="<cluster_id>",
+            name="foo",
             description="Terraform cluster alert group",
             group_interval_seconds=300,
             repeat_interval_seconds=3600)
         # Create a new Rancher2 Cluster Alert Rule
-        foo_cluster_alert_rule = rancher2.ClusterAlertRule("fooClusterAlertRule",
-            cluster_id=foo_cluster_alert_group.cluster_id,
-            group_id=foo_cluster_alert_group.id,
+        foo_cluster_alert_rule = rancher2.ClusterAlertRule("foo",
+            cluster_id=foo.cluster_id,
+            group_id=foo.id,
+            name="foo",
             group_interval_seconds=600,
             repeat_interval_seconds=6000)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -558,23 +560,25 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Cluster Alert Group
-        foo_cluster_alert_group = rancher2.ClusterAlertGroup("fooClusterAlertGroup",
+        foo = rancher2.ClusterAlertGroup("foo",
             cluster_id="<cluster_id>",
+            name="foo",
             description="Terraform cluster alert group",
             group_interval_seconds=300,
             repeat_interval_seconds=3600)
         # Create a new Rancher2 Cluster Alert Rule
-        foo_cluster_alert_rule = rancher2.ClusterAlertRule("fooClusterAlertRule",
-            cluster_id=foo_cluster_alert_group.cluster_id,
-            group_id=foo_cluster_alert_group.id,
+        foo_cluster_alert_rule = rancher2.ClusterAlertRule("foo",
+            cluster_id=foo.cluster_id,
+            group_id=foo.id,
+            name="foo",
             group_interval_seconds=600,
             repeat_interval_seconds=6000)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_driver.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_role_template_binding.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_role_template_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,14 +344,15 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Cluster Role Template Binding
         foo = rancher2.ClusterRoleTemplateBinding("foo",
+            name="foo",
             cluster_id="<cluster_id>",
             role_template_id="<role_template_id>",
             user_id="<user_id>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -390,14 +391,15 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Cluster Role Template Binding
         foo = rancher2.ClusterRoleTemplateBinding("foo",
+            name="foo",
             cluster_id="<cluster_id>",
             role_template_id="<role_template_id>",
             user_id="<user_id>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_sync.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,49 +334,53 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 rke Cluster 
-        foo_custom_cluster = rancher2.Cluster("foo-customCluster",
+        foo_custom = rancher2.Cluster("foo-custom",
+            name="foo-custom",
             description="Foo rancher2 custom cluster",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
             ))
         # Create a new rancher2 Node Template
-        foo_node_template = rancher2.NodeTemplate("fooNodeTemplate",
+        foo = rancher2.NodeTemplate("foo",
+            name="foo",
             description="foo test",
             amazonec2_config=rancher2.NodeTemplateAmazonec2ConfigArgs(
                 access_key="<AWS_ACCESS_KEY>",
                 secret_key="<AWS_SECRET_KEY>",
                 ami="<AMI_ID>",
                 region="<REGION>",
                 security_groups=["<AWS_SECURITY_GROUP>"],
                 subnet_id="<SUBNET_ID>",
                 vpc_id="<VPC_ID>",
                 zone="<ZONE>",
             ))
         # Create a new rancher2 Node Pool
-        foo_node_pool = rancher2.NodePool("fooNodePool",
-            cluster_id=foo_custom_cluster.id,
+        foo_node_pool = rancher2.NodePool("foo",
+            cluster_id=foo_custom.id,
+            name="foo",
             hostname_prefix="foo-cluster-0",
-            node_template_id=foo_node_template.id,
+            node_template_id=foo.id,
             quantity=3,
             control_plane=True,
             etcd=True,
             worker=True)
         # Create a new rancher2 Cluster Sync
-        foo_custom_cluster_sync = rancher2.ClusterSync("foo-customClusterSync",
-            cluster_id=foo_custom_cluster.id,
+        foo_custom_cluster_sync = rancher2.ClusterSync("foo-custom",
+            cluster_id=foo_custom.id,
             node_pool_ids=[foo_node_pool.id])
         # Create a new rancher2 Project
-        foo_project = rancher2.Project("fooProject",
+        foo_project = rancher2.Project("foo",
+            name="foo",
             cluster_id=foo_custom_cluster_sync.id,
             description="Terraform namespace acceptance test",
             resource_quota=rancher2.ProjectResourceQuotaArgs(
                 project_limit=rancher2.ProjectResourceQuotaProjectLimitArgs(
                     limits_cpu="2000m",
                     limits_memory="2000Mi",
                     requests_storage="2Gi",
@@ -418,49 +422,53 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 rke Cluster 
-        foo_custom_cluster = rancher2.Cluster("foo-customCluster",
+        foo_custom = rancher2.Cluster("foo-custom",
+            name="foo-custom",
             description="Foo rancher2 custom cluster",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
             ))
         # Create a new rancher2 Node Template
-        foo_node_template = rancher2.NodeTemplate("fooNodeTemplate",
+        foo = rancher2.NodeTemplate("foo",
+            name="foo",
             description="foo test",
             amazonec2_config=rancher2.NodeTemplateAmazonec2ConfigArgs(
                 access_key="<AWS_ACCESS_KEY>",
                 secret_key="<AWS_SECRET_KEY>",
                 ami="<AMI_ID>",
                 region="<REGION>",
                 security_groups=["<AWS_SECURITY_GROUP>"],
                 subnet_id="<SUBNET_ID>",
                 vpc_id="<VPC_ID>",
                 zone="<ZONE>",
             ))
         # Create a new rancher2 Node Pool
-        foo_node_pool = rancher2.NodePool("fooNodePool",
-            cluster_id=foo_custom_cluster.id,
+        foo_node_pool = rancher2.NodePool("foo",
+            cluster_id=foo_custom.id,
+            name="foo",
             hostname_prefix="foo-cluster-0",
-            node_template_id=foo_node_template.id,
+            node_template_id=foo.id,
             quantity=3,
             control_plane=True,
             etcd=True,
             worker=True)
         # Create a new rancher2 Cluster Sync
-        foo_custom_cluster_sync = rancher2.ClusterSync("foo-customClusterSync",
-            cluster_id=foo_custom_cluster.id,
+        foo_custom_cluster_sync = rancher2.ClusterSync("foo-custom",
+            cluster_id=foo_custom.id,
             node_pool_ids=[foo_node_pool.id])
         # Create a new rancher2 Project
-        foo_project = rancher2.Project("fooProject",
+        foo_project = rancher2.Project("foo",
+            name="foo",
             cluster_id=foo_custom_cluster_sync.id,
             description="Terraform namespace acceptance test",
             resource_quota=rancher2.ProjectResourceQuotaArgs(
                 project_limit=rancher2.ProjectResourceQuotaProjectLimitArgs(
                     limits_cpu="2000m",
                     limits_memory="2000Mi",
                     requests_storage="2Gi",
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_template.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,54 +259,56 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Cluster Template
         foo = rancher2.ClusterTemplate("foo",
-            description="Terraform cluster template foo",
+            name="foo",
             members=[rancher2.ClusterTemplateMemberArgs(
                 access_type="owner",
                 user_principal_id="local://user-XXXXX",
             )],
             template_revisions=[rancher2.ClusterTemplateTemplateRevisionArgs(
+                name="V1",
                 cluster_config=rancher2.ClusterTemplateTemplateRevisionClusterConfigArgs(
                     rke_config=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigArgs(
                         network=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigNetworkArgs(
                             plugin="canal",
                         ),
                         services=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesArgs(
                             etcd=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdArgs(
                                 creation="6h",
                                 retention="24h",
                             ),
                         ),
                     ),
                 ),
                 default=True,
-                name="V1",
-            )])
+            )],
+            description="Terraform cluster template foo")
         ```
         <!--End PulumiCodeChooser -->
 
         Creating Rancher v2 RKE cluster template with upgrade strategy. For Rancher v2.4.x and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Cluster Template
         foo = rancher2.ClusterTemplate("foo",
-            description="Terraform cluster template foo",
+            name="foo",
             members=[rancher2.ClusterTemplateMemberArgs(
                 access_type="owner",
                 user_principal_id="local://user-XXXXX",
             )],
             template_revisions=[rancher2.ClusterTemplateTemplateRevisionArgs(
+                name="V1",
                 cluster_config=rancher2.ClusterTemplateTemplateRevisionClusterConfigArgs(
                     rke_config=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigArgs(
                         network=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigNetworkArgs(
                             plugin="canal",
                         ),
                         services=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesArgs(
                             etcd=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdArgs(
@@ -317,16 +319,16 @@
                         upgrade_strategy=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigUpgradeStrategyArgs(
                             drain=True,
                             max_unavailable_worker="20%",
                         ),
                     ),
                 ),
                 default=True,
-                name="V1",
-            )])
+            )],
+            description="Terraform cluster template foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Cluster Template can be imported using the rancher Cluster Template ID
 
@@ -359,54 +361,56 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Cluster Template
         foo = rancher2.ClusterTemplate("foo",
-            description="Terraform cluster template foo",
+            name="foo",
             members=[rancher2.ClusterTemplateMemberArgs(
                 access_type="owner",
                 user_principal_id="local://user-XXXXX",
             )],
             template_revisions=[rancher2.ClusterTemplateTemplateRevisionArgs(
+                name="V1",
                 cluster_config=rancher2.ClusterTemplateTemplateRevisionClusterConfigArgs(
                     rke_config=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigArgs(
                         network=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigNetworkArgs(
                             plugin="canal",
                         ),
                         services=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesArgs(
                             etcd=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdArgs(
                                 creation="6h",
                                 retention="24h",
                             ),
                         ),
                     ),
                 ),
                 default=True,
-                name="V1",
-            )])
+            )],
+            description="Terraform cluster template foo")
         ```
         <!--End PulumiCodeChooser -->
 
         Creating Rancher v2 RKE cluster template with upgrade strategy. For Rancher v2.4.x and above.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Cluster Template
         foo = rancher2.ClusterTemplate("foo",
-            description="Terraform cluster template foo",
+            name="foo",
             members=[rancher2.ClusterTemplateMemberArgs(
                 access_type="owner",
                 user_principal_id="local://user-XXXXX",
             )],
             template_revisions=[rancher2.ClusterTemplateTemplateRevisionArgs(
+                name="V1",
                 cluster_config=rancher2.ClusterTemplateTemplateRevisionClusterConfigArgs(
                     rke_config=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigArgs(
                         network=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigNetworkArgs(
                             plugin="canal",
                         ),
                         services=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesArgs(
                             etcd=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdArgs(
@@ -417,16 +421,16 @@
                         upgrade_strategy=rancher2.ClusterTemplateTemplateRevisionClusterConfigRkeConfigUpgradeStrategyArgs(
                             drain=True,
                             max_unavailable_worker="20%",
                         ),
                     ),
                 ),
                 default=True,
-                name="V1",
-            )])
+            )],
+            description="Terraform cluster template foo")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Cluster Template can be imported using the rancher Cluster Template ID
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/cluster_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/cluster_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/config/__init__.pyi` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/config/vars.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/config_map_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/custom_user_token.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/custom_user_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,24 +462,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a rancher2 Token
-        foo_user = rancher2.User("fooUser",
+        foo = rancher2.User("foo",
+            name="foo",
             username="foo",
             password="changeme",
             enabled=True)
         foo_login = rancher2.GlobalRoleBinding("foo-login",
+            name="foo-login-binding",
             global_role_id="user-base",
-            user_id=foo_user.id)
-        foo_custom_user_token = rancher2.CustomUserToken("fooCustomUserToken",
-            username=foo_user.username,
-            password=foo_user.password,
+            user_id=foo.id)
+        foo_custom_user_token = rancher2.CustomUserToken("foo",
+            username=foo.username,
+            password=foo.password,
             description="foo token",
             ttl=0,
             opts=pulumi.ResourceOptions(depends_on=[foo_login]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
@@ -516,24 +518,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a rancher2 Token
-        foo_user = rancher2.User("fooUser",
+        foo = rancher2.User("foo",
+            name="foo",
             username="foo",
             password="changeme",
             enabled=True)
         foo_login = rancher2.GlobalRoleBinding("foo-login",
+            name="foo-login-binding",
             global_role_id="user-base",
-            user_id=foo_user.id)
-        foo_custom_user_token = rancher2.CustomUserToken("fooCustomUserToken",
-            username=foo_user.username,
-            password=foo_user.password,
+            user_id=foo.id)
+        foo_custom_user_token = rancher2.CustomUserToken("foo",
+            username=foo.username,
+            password=foo.password,
             description="foo token",
             ttl=0,
             opts=pulumi.ResourceOptions(depends_on=[foo_login]))
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/etcd_backup.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/etcd_backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,14 +322,15 @@
                     endpoint="endpoint",
                     folder="/folder",
                     region="region",
                     secret_key="secret_key",
                 ),
             ),
             cluster_id="<CLUSTER_ID>",
+            name="foo",
             filename="<FILENAME>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Etcd Backup can be imported using the Rancher etcd backup ID
@@ -379,14 +380,15 @@
                     endpoint="endpoint",
                     folder="/folder",
                     region="region",
                     secret_key="secret_key",
                 ),
             ),
             cluster_id="<CLUSTER_ID>",
+            name="foo",
             filename="<FILENAME>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Etcd Backup can be imported using the Rancher etcd backup ID
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/feature.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Feature
-        fleet = rancher2.Feature("fleet", value="<VALUE>")
+        fleet = rancher2.Feature("fleet",
+            name="fleet",
+            value="<VALUE>")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for feature object (map)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for feature object (map)
@@ -212,15 +214,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Feature
-        fleet = rancher2.Feature("fleet", value="<VALUE>")
+        fleet = rancher2.Feature("fleet",
+            name="fleet",
+            value="<VALUE>")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param FeatureArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_app.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_catalog.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_catalog_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_certificate.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,27 +133,29 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Project Certificate
     foo = rancher2.get_certificate(name="<name>",
         project_id="<project_id>")
     ```
     <!--End PulumiCodeChooser -->
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Namespaced Certificate
     foo = rancher2.get_certificate(name="<name>",
-        namespace_id="<namespace_id>",
-        project_id="<project_id>")
+        project_id="<project_id>",
+        namespace_id="<namespace_id>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the certificate (string)
     :param str namespace_id: The namespace id where to assign the namespaced certificate (string)
     :param str project_id: The project id where to assign the certificate (string)
@@ -191,27 +193,29 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Project Certificate
     foo = rancher2.get_certificate(name="<name>",
         project_id="<project_id>")
     ```
     <!--End PulumiCodeChooser -->
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Namespaced Certificate
     foo = rancher2.get_certificate(name="<name>",
-        namespace_id="<namespace_id>",
-        project_id="<project_id>")
+        project_id="<project_id>",
+        namespace_id="<namespace_id>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the certificate (string)
     :param str namespace_id: The namespace id where to assign the namespaced certificate (string)
     :param str project_id: The project id where to assign the certificate (string)
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cloud_credential.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_alert_group.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_alert_rule.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_driver.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_role_template_binding.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_role_template_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_cluster_role_template_binding(cluster_id="foo_id",
-        name="foo")
+    foo = rancher2.get_cluster_role_template_binding(name="foo",
+        cluster_id="foo_id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: The cluster id where bind cluster role template (string)
     :param str name: The name of the cluster role template binding (string)
     :param str role_template_id: The role template id from create cluster role template binding (string)
@@ -198,16 +198,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_cluster_role_template_binding(cluster_id="foo_id",
-        name="foo")
+    foo = rancher2.get_cluster_role_template_binding(name="foo",
+        cluster_id="foo_id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: The cluster id where bind cluster role template (string)
     :param str name: The name of the cluster role template binding (string)
     :param str role_template_id: The role template id from create cluster role template binding (string)
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_template.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_cluster_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_cluster_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,16 +234,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_cluster_v2(fleet_namespace="fleet-ns",
-        name="foo")
+    foo = rancher2.get_cluster_v2(name="foo",
+        fleet_namespace="fleet-ns")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str fleet_namespace: The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
     :param str name: The name of the Cluster v2 (string)
     """
@@ -283,16 +283,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_cluster_v2(fleet_namespace="fleet-ns",
-        name="foo")
+    foo = rancher2.get_cluster_v2(name="foo",
+        fleet_namespace="fleet-ns")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str fleet_namespace: The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
     :param str name: The name of the Cluster v2 (string)
     """
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_config_map_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_etcd_backup.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_global_dns_provider.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_global_role.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_global_role_binding.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_global_role_binding.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,16 +119,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_global_role_binding(global_role_id="foo_id",
-        name="foo")
+    foo = rancher2.get_global_role_binding(name="foo",
+        global_role_id="foo_id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str global_role_id: The global role id (string)
     :param str name: The name of the global role binding (string)
     """
@@ -158,16 +158,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_global_role_binding(global_role_id="foo_id",
-        name="foo")
+    foo = rancher2.get_global_role_binding(name="foo",
+        global_role_id="foo_id")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str global_role_id: The global role id (string)
     :param str name: The name of the global role binding (string)
     """
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_multi_cluster_app.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_namespace.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_namespace.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
     foo = rancher2.get_namespace(name="foo",
-        project_id=rancher2_cluster["foo-custom"]["default_project_id"])
+        project_id=foo_custom["defaultProjectId"])
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the namespace (string)
     :param str project_id: The project id where namespace is assigned (string)
     """
@@ -173,15 +173,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
     foo = rancher2.get_namespace(name="foo",
-        project_id=rancher2_cluster["foo-custom"]["default_project_id"])
+        project_id=foo_custom["defaultProjectId"])
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the namespace (string)
     :param str project_id: The project id where namespace is assigned (string)
     """
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_node_driver.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_node_pool.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_node_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_node_pool(cluster_id=rancher2_cluster["foo-custom"]["id"],
+    foo = rancher2.get_node_pool(cluster_id=foo_custom["id"],
         name="foo")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: The RKE cluster id to use Node Pool (string)
     :param str name: The name of the Node Pool (string)
@@ -238,15 +238,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_node_pool(cluster_id=rancher2_cluster["foo-custom"]["id"],
+    foo = rancher2.get_node_pool(cluster_id=foo_custom["id"],
         name="foo")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: The RKE cluster id to use Node Pool (string)
     :param str name: The name of the Node Pool (string)
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_node_template.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_notifier.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_notifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,16 +195,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_notifier(cluster_id="<cluster_id>",
-        name="foo")
+    foo = rancher2.get_notifier(name="foo",
+        cluster_id="<cluster_id>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: The cluster id where create notifier (string)
     :param pulumi.InputType['GetNotifierDingtalkConfigArgs'] dingtalk_config: (Computed) Dingtalk config for notifier (list maxitems:1)
     :param pulumi.InputType['GetNotifierMsteamsConfigArgs'] msteams_config: (Computed) MSTeams config for notifier (list maxitems:1)
@@ -246,16 +246,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_notifier(cluster_id="<cluster_id>",
-        name="foo")
+    foo = rancher2.get_notifier(name="foo",
+        cluster_id="<cluster_id>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str cluster_id: The cluster id where create notifier (string)
     :param pulumi.InputType['GetNotifierDingtalkConfigArgs'] dingtalk_config: (Computed) Dingtalk config for notifier (list maxitems:1)
     :param pulumi.InputType['GetNotifierMsteamsConfigArgs'] msteams_config: (Computed) MSTeams config for notifier (list maxitems:1)
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_pod_security_admission_configuration_template.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_pod_security_admission_configuration_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_pod_security_policy_template.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_principal.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_project.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_project_alert_group.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_project_alert_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,16 +156,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_project_alert_group(name="<project_alert_group_name>",
-        project_id="<project_id>")
+    foo = rancher2.get_project_alert_group(project_id="<project_id>",
+        name="<project_alert_group_name>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The project alert group name (string)
     :param str project_id: The project id where create project alert group (string)
     """
@@ -198,16 +198,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_project_alert_group(name="<project_alert_group_name>",
-        project_id="<project_id>")
+    foo = rancher2.get_project_alert_group(project_id="<project_id>",
+        name="<project_alert_group_name>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The project alert group name (string)
     :param str project_id: The project id where create project alert group (string)
     """
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_project_alert_rule.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_project_alert_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,16 +205,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_project_alert_rule(name="<project_alert_rule_name>",
-        project_id="<project_id>")
+    foo = rancher2.get_project_alert_rule(project_id="<project_id>",
+        name="<project_alert_rule_name>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param Mapping[str, Any] labels: (Computed) The project alert rule labels (map)
     :param str name: The project alert rule name (string)
     :param str project_id: The project id where create project alert rule (string)
@@ -254,16 +254,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
-    foo = rancher2.get_project_alert_rule(name="<project_alert_rule_name>",
-        project_id="<project_id>")
+    foo = rancher2.get_project_alert_rule(project_id="<project_id>",
+        name="<project_alert_rule_name>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param Mapping[str, Any] labels: (Computed) The project alert rule labels (map)
     :param str name: The project alert rule name (string)
     :param str project_id: The project id where create project alert rule (string)
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_project_role_template_binding.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_registry.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -134,27 +134,29 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Project Registry
     foo = rancher2.get_registry(name="<name>",
         project_id="<project_id>")
     ```
     <!--End PulumiCodeChooser -->
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Namespaced Registry
     foo = rancher2.get_registry(name="<name>",
-        namespace_id="<namespace_id>",
-        project_id="<project_id>")
+        project_id="<project_id>",
+        namespace_id="<namespace_id>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the registry (string)
     :param str namespace_id: The namespace id where to assign the namespaced registry (string)
     :param str project_id: The project id where to assign the registry (string)
@@ -192,27 +194,29 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Project Registry
     foo = rancher2.get_registry(name="<name>",
         project_id="<project_id>")
     ```
     <!--End PulumiCodeChooser -->
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Namespaced Registry
     foo = rancher2.get_registry(name="<name>",
-        namespace_id="<namespace_id>",
-        project_id="<project_id>")
+        project_id="<project_id>",
+        namespace_id="<namespace_id>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the registry (string)
     :param str namespace_id: The namespace id where to assign the namespaced registry (string)
     :param str project_id: The project id where to assign the registry (string)
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_role_template.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_secret.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_secret.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,27 +133,29 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Project Secret
     foo = rancher2.get_secret(name="<name>",
         project_id="<project_id>")
     ```
     <!--End PulumiCodeChooser -->
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Namespaced Secret
     foo = rancher2.get_secret(name="<name>",
-        namespace_id="<namespace_id>",
-        project_id="<project_id>")
+        project_id="<project_id>",
+        namespace_id="<namespace_id>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the secret (string)
     :param str namespace_id: The namespace id where to assign the namespaced secret (string)
     :param str project_id: The project id where to assign the secret (string)
@@ -191,27 +193,29 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Project Secret
     foo = rancher2.get_secret(name="<name>",
         project_id="<project_id>")
     ```
     <!--End PulumiCodeChooser -->
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_rancher2 as rancher2
 
+    # Retrieve a rancher2 Namespaced Secret
     foo = rancher2.get_secret(name="<name>",
-        namespace_id="<namespace_id>",
-        project_id="<project_id>")
+        project_id="<project_id>",
+        namespace_id="<namespace_id>")
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the secret (string)
     :param str namespace_id: The namespace id where to assign the namespaced secret (string)
     :param str project_id: The project id where to assign the secret (string)
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_secret_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_setting.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_storage_class_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/get_user.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/global_dns.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/global_dns.py`

 * *Files 7% similar despite different names*

```diff
@@ -302,51 +302,55 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global DNS Provider
-        foo_global_dns_provider = rancher2.GlobalDnsProvider("fooGlobalDnsProvider",
+        foo = rancher2.GlobalDnsProvider("foo",
+            name="foo",
             root_domain="example.com",
             route53_config=rancher2.GlobalDnsProviderRoute53ConfigArgs(
                 access_key="YYYYYYYYYYYYYYYYYYYY",
                 secret_key="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
                 zone_type="private",
                 region="us-east-1",
             ))
         # Create a new rancher2 Global DNS using project IDs
-        foo_global_dns = rancher2.GlobalDns("fooGlobalDns",
+        foo_global_dns = rancher2.GlobalDns("foo",
+            name="foo",
             fqdn="foo.example.com",
-            provider_id=foo_global_dns_provider.id,
+            provider_id=foo.id,
             project_ids=[
                 "project1",
                 "project2",
             ])
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global DNS Provider
-        foo_global_dns_provider = rancher2.GlobalDnsProvider("fooGlobalDnsProvider",
+        foo = rancher2.GlobalDnsProvider("foo",
+            name="foo",
             root_domain="example.com",
             route53_config=rancher2.GlobalDnsProviderRoute53ConfigArgs(
                 access_key="YYYYYYYYYYYYYYYYYYYY",
                 secret_key="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
                 zone_type="private",
                 region="us-east-1",
             ))
         # Create a new rancher2 Global DNS using MultiClusterApp ID
-        foo_global_dns = rancher2.GlobalDns("fooGlobalDns",
+        foo_global_dns = rancher2.GlobalDns("foo",
+            name="foo",
             fqdn="foo.example.com",
-            provider_id=foo_global_dns_provider.id,
+            provider_id=foo.id,
             multi_cluster_app_id="<MCA_ID>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Global DNS Entry can be imported using the Rancher Global DNS ID
@@ -379,51 +383,55 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global DNS Provider
-        foo_global_dns_provider = rancher2.GlobalDnsProvider("fooGlobalDnsProvider",
+        foo = rancher2.GlobalDnsProvider("foo",
+            name="foo",
             root_domain="example.com",
             route53_config=rancher2.GlobalDnsProviderRoute53ConfigArgs(
                 access_key="YYYYYYYYYYYYYYYYYYYY",
                 secret_key="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
                 zone_type="private",
                 region="us-east-1",
             ))
         # Create a new rancher2 Global DNS using project IDs
-        foo_global_dns = rancher2.GlobalDns("fooGlobalDns",
+        foo_global_dns = rancher2.GlobalDns("foo",
+            name="foo",
             fqdn="foo.example.com",
-            provider_id=foo_global_dns_provider.id,
+            provider_id=foo.id,
             project_ids=[
                 "project1",
                 "project2",
             ])
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global DNS Provider
-        foo_global_dns_provider = rancher2.GlobalDnsProvider("fooGlobalDnsProvider",
+        foo = rancher2.GlobalDnsProvider("foo",
+            name="foo",
             root_domain="example.com",
             route53_config=rancher2.GlobalDnsProviderRoute53ConfigArgs(
                 access_key="YYYYYYYYYYYYYYYYYYYY",
                 secret_key="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
                 zone_type="private",
                 region="us-east-1",
             ))
         # Create a new rancher2 Global DNS using MultiClusterApp ID
-        foo_global_dns = rancher2.GlobalDns("fooGlobalDns",
+        foo_global_dns = rancher2.GlobalDns("foo",
+            name="foo",
             fqdn="foo.example.com",
-            provider_id=foo_global_dns_provider.id,
+            provider_id=foo.id,
             multi_cluster_app_id="<MCA_ID>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Global DNS Entry can be imported using the Rancher Global DNS ID
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/global_dns_provider.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/global_dns_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,51 +265,54 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global DNS Provider - alidns
         foo = rancher2.GlobalDnsProvider("foo",
+            name="foo",
+            root_domain="example.com",
             alidns_config=rancher2.GlobalDnsProviderAlidnsConfigArgs(
                 access_key="YYYYYYYYYYYYYYYYYYYY",
                 secret_key="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
-            ),
-            root_domain="example.com")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global DNS Provider - cloudflare
         foo = rancher2.GlobalDnsProvider("foo",
+            name="foo",
+            root_domain="example.com",
             cloudflare_config=rancher2.GlobalDnsProviderCloudflareConfigArgs(
                 api_email="test@test.local",
                 api_key="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
                 proxy_setting=True,
-            ),
-            root_domain="example.com")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global DNS Provider - route53
         foo = rancher2.GlobalDnsProvider("foo",
+            name="foo",
             root_domain="example.com",
             route53_config=rancher2.GlobalDnsProviderRoute53ConfigArgs(
                 access_key="YYYYYYYYYYYYYYYYYYYY",
-                region="us-east-1",
                 secret_key="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
                 zone_type="private",
+                region="us-east-1",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Global DNS Providers can be imported using the Rancher Global DNS Provider ID
@@ -339,51 +342,54 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global DNS Provider - alidns
         foo = rancher2.GlobalDnsProvider("foo",
+            name="foo",
+            root_domain="example.com",
             alidns_config=rancher2.GlobalDnsProviderAlidnsConfigArgs(
                 access_key="YYYYYYYYYYYYYYYYYYYY",
                 secret_key="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
-            ),
-            root_domain="example.com")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global DNS Provider - cloudflare
         foo = rancher2.GlobalDnsProvider("foo",
+            name="foo",
+            root_domain="example.com",
             cloudflare_config=rancher2.GlobalDnsProviderCloudflareConfigArgs(
                 api_email="test@test.local",
                 api_key="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
                 proxy_setting=True,
-            ),
-            root_domain="example.com")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global DNS Provider - route53
         foo = rancher2.GlobalDnsProvider("foo",
+            name="foo",
             root_domain="example.com",
             route53_config=rancher2.GlobalDnsProviderRoute53ConfigArgs(
                 access_key="YYYYYYYYYYYYYYYYYYYY",
-                region="us-east-1",
                 secret_key="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
                 zone_type="private",
+                region="us-east-1",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Global DNS Providers can be imported using the Rancher Global DNS Provider ID
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/global_role.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/global_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,16 +290,17 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global Role
         foo = rancher2.GlobalRole("foo",
-            description="Terraform global role acceptance test",
+            name="foo",
             new_user_default=True,
+            description="Terraform global role acceptance test",
             rules=[rancher2.GlobalRoleRuleArgs(
                 api_groups=["*"],
                 resources=["secrets"],
                 verbs=["create"],
             )])
         ```
         <!--End PulumiCodeChooser -->
@@ -336,16 +337,17 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global Role
         foo = rancher2.GlobalRole("foo",
-            description="Terraform global role acceptance test",
+            name="foo",
             new_user_default=True,
+            description="Terraform global role acceptance test",
             rules=[rancher2.GlobalRoleRuleArgs(
                 api_groups=["*"],
                 resources=["secrets"],
                 verbs=["create"],
             )])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/global_role_binding.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/global_role_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,18 +246,20 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global Role Binding using user_id
         foo = rancher2.GlobalRoleBinding("foo",
+            name="foo",
             global_role_id="admin",
             user_id="user-XXXXX")
         # Create a new rancher2 Global Role Binding using group_principal_id
         foo2 = rancher2.GlobalRoleBinding("foo2",
+            name="foo2",
             global_role_id="admin",
             group_principal_id="local://g-XXXXX")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -292,18 +294,20 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Global Role Binding using user_id
         foo = rancher2.GlobalRoleBinding("foo",
+            name="foo",
             global_role_id="admin",
             user_id="user-XXXXX")
         # Create a new rancher2 Global Role Binding using group_principal_id
         foo2 = rancher2.GlobalRoleBinding("foo2",
+            name="foo2",
             global_role_id="admin",
             group_principal_id="local://g-XXXXX")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/machine_config_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/machine_config_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,46 +461,47 @@
         ### Using the Harvester Node Driver
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_harvester_cluster_v2 = rancher2.get_cluster_v2(name="foo-harvester")
+        # Get imported harvester cluster info
+        foo_harvester = rancher2.get_cluster_v2(name="foo-harvester")
         # Create a new Cloud Credential for an imported Harvester cluster
-        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvesterCloudCredential", harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
-            cluster_id=foo_harvester_cluster_v2.cluster_v1_id,
-            cluster_type="imported",
-            kubeconfig_content=foo_harvester_cluster_v2.kube_config,
-        ))
+        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvester",
+            name="foo-harvester",
+            harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
+                cluster_id=foo_harvester.cluster_v1_id,
+                cluster_type="imported",
+                kubeconfig_content=foo_harvester.kube_config,
+            ))
         # Create a new rancher2 machine config v2 using harvester node_driver
         foo_harvester_v2 = rancher2.MachineConfigV2("foo-harvester-v2",
             generate_name="foo-harvester-v2",
             harvester_config=rancher2.MachineConfigV2HarvesterConfigArgs(
                 vm_namespace="default",
                 cpu_count="2",
                 memory_size="4",
                 disk_info=\"\"\"    {
                 "disks": [{
                     "imageName": "harvester-public/image-57hzg",
                     "size": 40,
                     "bootOrder": 1
                 }]
             }
-            EOF,
-            networkInfo = <<EOF
-            {
+        \"\"\",
+                network_info=\"\"\"    {
                 "interfaces": [{
                     "networkName": "harvester-public/vlan1"
                 }]
             }
-            EOF,
-            sshUser = "ubuntu",
-            userData = <<EOF
-            package_update: true
+        \"\"\",
+                ssh_user="ubuntu",
+                user_data=\"\"\"    package_update: true
             packages:
               - qemu-guest-agent
               - iptables
             runcmd:
               - - systemctl
                 - enable
                 - '--now'
@@ -540,46 +541,47 @@
         ### Using the Harvester Node Driver
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_harvester_cluster_v2 = rancher2.get_cluster_v2(name="foo-harvester")
+        # Get imported harvester cluster info
+        foo_harvester = rancher2.get_cluster_v2(name="foo-harvester")
         # Create a new Cloud Credential for an imported Harvester cluster
-        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvesterCloudCredential", harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
-            cluster_id=foo_harvester_cluster_v2.cluster_v1_id,
-            cluster_type="imported",
-            kubeconfig_content=foo_harvester_cluster_v2.kube_config,
-        ))
+        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvester",
+            name="foo-harvester",
+            harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
+                cluster_id=foo_harvester.cluster_v1_id,
+                cluster_type="imported",
+                kubeconfig_content=foo_harvester.kube_config,
+            ))
         # Create a new rancher2 machine config v2 using harvester node_driver
         foo_harvester_v2 = rancher2.MachineConfigV2("foo-harvester-v2",
             generate_name="foo-harvester-v2",
             harvester_config=rancher2.MachineConfigV2HarvesterConfigArgs(
                 vm_namespace="default",
                 cpu_count="2",
                 memory_size="4",
                 disk_info=\"\"\"    {
                 "disks": [{
                     "imageName": "harvester-public/image-57hzg",
                     "size": 40,
                     "bootOrder": 1
                 }]
             }
-            EOF,
-            networkInfo = <<EOF
-            {
+        \"\"\",
+                network_info=\"\"\"    {
                 "interfaces": [{
                     "networkName": "harvester-public/vlan1"
                 }]
             }
-            EOF,
-            sshUser = "ubuntu",
-            userData = <<EOF
-            package_update: true
+        \"\"\",
+                ssh_user="ubuntu",
+                user_data=\"\"\"    package_update: true
             packages:
               - qemu-guest-agent
               - iptables
             runcmd:
               - - systemctl
                 - enable
                 - '--now'
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/multi_cluster_app.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/multi_cluster_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,61 +524,63 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Multi Cluster App
         foo = rancher2.MultiClusterApp("foo",
-            answers=[rancher2.MultiClusterAppAnswerArgs(
-                values={
-                    "ingressHost": "test.xip.io",
-                },
-            )],
             catalog_name="<catalog_name>",
-            roles=["project-member"],
+            name="foo",
             targets=[rancher2.MultiClusterAppTargetArgs(
                 project_id="<project_id>",
             )],
             template_name="<template_name>",
-            template_version="<template_version>")
+            template_version="<template_version>",
+            answers=[rancher2.MultiClusterAppAnswerArgs(
+                values={
+                    "ingress_host": "test.xip.io",
+                },
+            )],
+            roles=["project-member"])
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Multi Cluster App overriding answers
         foo = rancher2.MultiClusterApp("foo",
+            catalog_name="<catalog_name>",
+            name="foo",
+            targets=[
+                rancher2.MultiClusterAppTargetArgs(
+                    project_id="<project_id1>",
+                ),
+                rancher2.MultiClusterAppTargetArgs(
+                    project_id="<project_id2>",
+                ),
+            ],
+            template_name="<template_name>",
+            template_version="<template_version>",
             answers=[
                 rancher2.MultiClusterAppAnswerArgs(
                     values={
-                        "ingressHost": "test.xip.io",
+                        "ingress_host": "test.xip.io",
                     },
                 ),
                 rancher2.MultiClusterAppAnswerArgs(
                     project_id="<project_id2>",
                     values={
-                        "ingressHost": "test2.xip.io",
+                        "ingress_host": "test2.xip.io",
                     },
                 ),
             ],
-            catalog_name="<catalog_name>",
-            roles=["project-member"],
-            targets=[
-                rancher2.MultiClusterAppTargetArgs(
-                    project_id="<project_id1>",
-                ),
-                rancher2.MultiClusterAppTargetArgs(
-                    project_id="<project_id2>",
-                ),
-            ],
-            template_name="<template_name>",
-            template_version="<template_version>")
+            roles=["project-member"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Multi cluster app can be imported using the multi cluster app ID in the format `<multi_cluster_app_name>`
 
@@ -624,61 +626,63 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Multi Cluster App
         foo = rancher2.MultiClusterApp("foo",
-            answers=[rancher2.MultiClusterAppAnswerArgs(
-                values={
-                    "ingressHost": "test.xip.io",
-                },
-            )],
             catalog_name="<catalog_name>",
-            roles=["project-member"],
+            name="foo",
             targets=[rancher2.MultiClusterAppTargetArgs(
                 project_id="<project_id>",
             )],
             template_name="<template_name>",
-            template_version="<template_version>")
+            template_version="<template_version>",
+            answers=[rancher2.MultiClusterAppAnswerArgs(
+                values={
+                    "ingress_host": "test.xip.io",
+                },
+            )],
+            roles=["project-member"])
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Multi Cluster App overriding answers
         foo = rancher2.MultiClusterApp("foo",
+            catalog_name="<catalog_name>",
+            name="foo",
+            targets=[
+                rancher2.MultiClusterAppTargetArgs(
+                    project_id="<project_id1>",
+                ),
+                rancher2.MultiClusterAppTargetArgs(
+                    project_id="<project_id2>",
+                ),
+            ],
+            template_name="<template_name>",
+            template_version="<template_version>",
             answers=[
                 rancher2.MultiClusterAppAnswerArgs(
                     values={
-                        "ingressHost": "test.xip.io",
+                        "ingress_host": "test.xip.io",
                     },
                 ),
                 rancher2.MultiClusterAppAnswerArgs(
                     project_id="<project_id2>",
                     values={
-                        "ingressHost": "test2.xip.io",
+                        "ingress_host": "test2.xip.io",
                     },
                 ),
             ],
-            catalog_name="<catalog_name>",
-            roles=["project-member"],
-            targets=[
-                rancher2.MultiClusterAppTargetArgs(
-                    project_id="<project_id1>",
-                ),
-                rancher2.MultiClusterAppTargetArgs(
-                    project_id="<project_id2>",
-                ),
-            ],
-            template_name="<template_name>",
-            template_version="<template_version>")
+            roles=["project-member"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Multi cluster app can be imported using the multi cluster app ID in the format `<multi_cluster_app_name>`
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/namespace.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,47 +306,50 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Namespace
         foo = rancher2.Namespace("foo",
-            container_resource_limit=rancher2.NamespaceContainerResourceLimitArgs(
-                limits_cpu="20m",
-                limits_memory="20Mi",
-                requests_cpu="1m",
-                requests_memory="1Mi",
-            ),
-            description="foo namespace",
+            name="foo",
             project_id="<PROJECT_ID>",
+            description="foo namespace",
             resource_quota=rancher2.NamespaceResourceQuotaArgs(
                 limit=rancher2.NamespaceResourceQuotaLimitArgs(
                     limits_cpu="100m",
                     limits_memory="100Mi",
                     requests_storage="1Gi",
                 ),
+            ),
+            container_resource_limit=rancher2.NamespaceContainerResourceLimitArgs(
+                limits_cpu="20m",
+                limits_memory="20Mi",
+                requests_cpu="1m",
+                requests_memory="1Mi",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Cluster 
         foo_custom = rancher2.Cluster("foo-custom",
+            name="foo-custom",
             description="Foo rancher2 custom cluster",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
             ))
         # Create a new rancher2 Namespace assigned to default cluster project
         foo = rancher2.Namespace("foo",
+            name="foo",
             project_id=foo_custom.default_project_id,
             description="foo namespace",
             resource_quota=rancher2.NamespaceResourceQuotaArgs(
                 limit=rancher2.NamespaceResourceQuotaLimitArgs(
                     limits_cpu="100m",
                     limits_memory="100Mi",
                     requests_storage="1Gi",
@@ -400,47 +403,50 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Namespace
         foo = rancher2.Namespace("foo",
-            container_resource_limit=rancher2.NamespaceContainerResourceLimitArgs(
-                limits_cpu="20m",
-                limits_memory="20Mi",
-                requests_cpu="1m",
-                requests_memory="1Mi",
-            ),
-            description="foo namespace",
+            name="foo",
             project_id="<PROJECT_ID>",
+            description="foo namespace",
             resource_quota=rancher2.NamespaceResourceQuotaArgs(
                 limit=rancher2.NamespaceResourceQuotaLimitArgs(
                     limits_cpu="100m",
                     limits_memory="100Mi",
                     requests_storage="1Gi",
                 ),
+            ),
+            container_resource_limit=rancher2.NamespaceContainerResourceLimitArgs(
+                limits_cpu="20m",
+                limits_memory="20Mi",
+                requests_cpu="1m",
+                requests_memory="1Mi",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Cluster 
         foo_custom = rancher2.Cluster("foo-custom",
+            name="foo-custom",
             description="Foo rancher2 custom cluster",
             rke_config=rancher2.ClusterRkeConfigArgs(
                 network=rancher2.ClusterRkeConfigNetworkArgs(
                     plugin="canal",
                 ),
             ))
         # Create a new rancher2 Namespace assigned to default cluster project
         foo = rancher2.Namespace("foo",
+            name="foo",
             project_id=foo_custom.default_project_id,
             description="foo namespace",
             resource_quota=rancher2.NamespaceResourceQuotaArgs(
                 limit=rancher2.NamespaceResourceQuotaLimitArgs(
                     limits_cpu="100m",
                     limits_memory="100Mi",
                     requests_storage="1Gi",
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/node_driver.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/node_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,14 +406,15 @@
         # Create a new rancher2 Node Driver
         foo = rancher2.NodeDriver("foo",
             active=True,
             builtin=False,
             checksum="0x0",
             description="Foo description",
             external_id="foo_external",
+            name="foo",
             ui_url="local://ui",
             url="local://",
             whitelist_domains=["*.foo.com"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -457,14 +458,15 @@
         # Create a new rancher2 Node Driver
         foo = rancher2.NodeDriver("foo",
             active=True,
             builtin=False,
             checksum="0x0",
             description="Foo description",
             external_id="foo_external",
+            name="foo",
             ui_url="local://ui",
             url="local://",
             whitelist_domains=["*.foo.com"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/node_pool.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/node_template.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/node_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -962,43 +962,46 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Node Template up to Rancher 2.1.x
         foo = rancher2.NodeTemplate("foo",
+            name="foo",
+            description="foo test",
             amazonec2_config=rancher2.NodeTemplateAmazonec2ConfigArgs(
                 access_key="AWS_ACCESS_KEY",
+                secret_key="<AWS_SECRET_KEY>",
                 ami="<AMI_ID>",
                 region="<REGION>",
-                secret_key="<AWS_SECRET_KEY>",
                 security_groups=["<AWS_SECURITY_GROUP>"],
                 subnet_id="<SUBNET_ID>",
                 vpc_id="<VPC_ID>",
                 zone="<ZONE>",
-            ),
-            description="foo test")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Node Template from Rancher 2.2.x
-        foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
+        foo = rancher2.CloudCredential("foo",
+            name="foo",
             description="foo test",
             amazonec2_credential_config=rancher2.CloudCredentialAmazonec2CredentialConfigArgs(
                 access_key="<AWS_ACCESS_KEY>",
                 secret_key="<AWS_SECRET_KEY>",
             ))
-        foo_node_template = rancher2.NodeTemplate("fooNodeTemplate",
+        foo_node_template = rancher2.NodeTemplate("foo",
+            name="foo",
             description="foo test",
-            cloud_credential_id=foo_cloud_credential.id,
+            cloud_credential_id=foo.id,
             amazonec2_config=rancher2.NodeTemplateAmazonec2ConfigArgs(
                 ami="<AMI_ID>",
                 region="<REGION>",
                 security_groups=["<AWS_SECURITY_GROUP>"],
                 subnet_id="<SUBNET_ID>",
                 vpc_id="<VPC_ID>",
                 zone="<ZONE>",
@@ -1009,47 +1012,49 @@
         ### Using the Harvester Node Driver
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_harvester_cluster_v2 = rancher2.get_cluster_v2(name="foo-harvester")
+        # Get imported harvester cluster info
+        foo_harvester = rancher2.get_cluster_v2(name="foo-harvester")
         # Create a new Cloud Credential for an imported Harvester cluster
-        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvesterCloudCredential", harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
-            cluster_id=foo_harvester_cluster_v2.cluster_v1_id,
-            cluster_type="imported",
-            kubeconfig_content=foo_harvester_cluster_v2.kube_config,
-        ))
+        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvester",
+            name="foo-harvester",
+            harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
+                cluster_id=foo_harvester.cluster_v1_id,
+                cluster_type="imported",
+                kubeconfig_content=foo_harvester.kube_config,
+            ))
         # Create a new rancher2 Node Template using harvester node_driver
-        foo_harvester_node_template = rancher2.NodeTemplate("foo-harvesterNodeTemplate",
+        foo_harvester_node_template = rancher2.NodeTemplate("foo-harvester",
+            name="foo-harvester",
             cloud_credential_id=foo_harvester_cloud_credential.id,
             engine_install_url="https://releases.rancher.com/install-docker/20.10.sh",
             harvester_config=rancher2.NodeTemplateHarvesterConfigArgs(
                 vm_namespace="default",
                 cpu_count="2",
                 memory_size="4",
                 disk_info=\"\"\"    {
                 "disks": [{
                     "imageName": "harvester-public/image-57hzg",
                     "size": 40,
                     "bootOrder": 1
                 }]
             }
-            EOF,
-            networkInfo = <<EOF
-            {
+        \"\"\",
+                network_info=\"\"\"    {
                 "interfaces": [{
                     "networkName": "harvester-public/vlan1"
                 }]
             }
-            EOF,
-            sshUser = "ubuntu",
-            userData = <<EOF
-            package_update: true
+        \"\"\",
+                ssh_user="ubuntu",
+                user_data=\"\"\"    package_update: true
             packages:
               - qemu-guest-agent
               - iptables
             runcmd:
               - - systemctl
                 - enable
                 - '--now'
@@ -1063,21 +1068,23 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Node Template using hetzner node_driver
-        hetzner_node_driver = rancher2.NodeDriver("hetznerNodeDriver",
+        hetzner_node_driver = rancher2.NodeDriver("hetzner_node_driver",
             active=True,
             builtin=False,
+            name="Hetzner",
             ui_url="https://storage.googleapis.com/hcloud-rancher-v2-ui-driver/component.js",
             url="https://github.com/JonasProgrammer/docker-machine-driver-hetzner/releases/download/3.6.0/docker-machine-driver-hetzner_3.6.0_linux_amd64.tar.gz",
             whitelist_domains=["storage.googleapis.com"])
-        my_hetzner_node_template = rancher2.NodeTemplate("myHetznerNodeTemplate",
+        my_hetzner_node_template = rancher2.NodeTemplate("my_hetzner_node_template",
+            name="my-hetzner-node-template",
             driver_id=hetzner_node_driver.id,
             hetzner_config=rancher2.NodeTemplateHetznerConfigArgs(
                 api_token="XXXXXXXXXX",
                 image="ubuntu-18.04",
                 server_location="nbg1",
                 server_type="cx11",
             ))
@@ -1140,43 +1147,46 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Node Template up to Rancher 2.1.x
         foo = rancher2.NodeTemplate("foo",
+            name="foo",
+            description="foo test",
             amazonec2_config=rancher2.NodeTemplateAmazonec2ConfigArgs(
                 access_key="AWS_ACCESS_KEY",
+                secret_key="<AWS_SECRET_KEY>",
                 ami="<AMI_ID>",
                 region="<REGION>",
-                secret_key="<AWS_SECRET_KEY>",
                 security_groups=["<AWS_SECURITY_GROUP>"],
                 subnet_id="<SUBNET_ID>",
                 vpc_id="<VPC_ID>",
                 zone="<ZONE>",
-            ),
-            description="foo test")
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Node Template from Rancher 2.2.x
-        foo_cloud_credential = rancher2.CloudCredential("fooCloudCredential",
+        foo = rancher2.CloudCredential("foo",
+            name="foo",
             description="foo test",
             amazonec2_credential_config=rancher2.CloudCredentialAmazonec2CredentialConfigArgs(
                 access_key="<AWS_ACCESS_KEY>",
                 secret_key="<AWS_SECRET_KEY>",
             ))
-        foo_node_template = rancher2.NodeTemplate("fooNodeTemplate",
+        foo_node_template = rancher2.NodeTemplate("foo",
+            name="foo",
             description="foo test",
-            cloud_credential_id=foo_cloud_credential.id,
+            cloud_credential_id=foo.id,
             amazonec2_config=rancher2.NodeTemplateAmazonec2ConfigArgs(
                 ami="<AMI_ID>",
                 region="<REGION>",
                 security_groups=["<AWS_SECURITY_GROUP>"],
                 subnet_id="<SUBNET_ID>",
                 vpc_id="<VPC_ID>",
                 zone="<ZONE>",
@@ -1187,47 +1197,49 @@
         ### Using the Harvester Node Driver
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
-        foo_harvester_cluster_v2 = rancher2.get_cluster_v2(name="foo-harvester")
+        # Get imported harvester cluster info
+        foo_harvester = rancher2.get_cluster_v2(name="foo-harvester")
         # Create a new Cloud Credential for an imported Harvester cluster
-        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvesterCloudCredential", harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
-            cluster_id=foo_harvester_cluster_v2.cluster_v1_id,
-            cluster_type="imported",
-            kubeconfig_content=foo_harvester_cluster_v2.kube_config,
-        ))
+        foo_harvester_cloud_credential = rancher2.CloudCredential("foo-harvester",
+            name="foo-harvester",
+            harvester_credential_config=rancher2.CloudCredentialHarvesterCredentialConfigArgs(
+                cluster_id=foo_harvester.cluster_v1_id,
+                cluster_type="imported",
+                kubeconfig_content=foo_harvester.kube_config,
+            ))
         # Create a new rancher2 Node Template using harvester node_driver
-        foo_harvester_node_template = rancher2.NodeTemplate("foo-harvesterNodeTemplate",
+        foo_harvester_node_template = rancher2.NodeTemplate("foo-harvester",
+            name="foo-harvester",
             cloud_credential_id=foo_harvester_cloud_credential.id,
             engine_install_url="https://releases.rancher.com/install-docker/20.10.sh",
             harvester_config=rancher2.NodeTemplateHarvesterConfigArgs(
                 vm_namespace="default",
                 cpu_count="2",
                 memory_size="4",
                 disk_info=\"\"\"    {
                 "disks": [{
                     "imageName": "harvester-public/image-57hzg",
                     "size": 40,
                     "bootOrder": 1
                 }]
             }
-            EOF,
-            networkInfo = <<EOF
-            {
+        \"\"\",
+                network_info=\"\"\"    {
                 "interfaces": [{
                     "networkName": "harvester-public/vlan1"
                 }]
             }
-            EOF,
-            sshUser = "ubuntu",
-            userData = <<EOF
-            package_update: true
+        \"\"\",
+                ssh_user="ubuntu",
+                user_data=\"\"\"    package_update: true
             packages:
               - qemu-guest-agent
               - iptables
             runcmd:
               - - systemctl
                 - enable
                 - '--now'
@@ -1241,21 +1253,23 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Node Template using hetzner node_driver
-        hetzner_node_driver = rancher2.NodeDriver("hetznerNodeDriver",
+        hetzner_node_driver = rancher2.NodeDriver("hetzner_node_driver",
             active=True,
             builtin=False,
+            name="Hetzner",
             ui_url="https://storage.googleapis.com/hcloud-rancher-v2-ui-driver/component.js",
             url="https://github.com/JonasProgrammer/docker-machine-driver-hetzner/releases/download/3.6.0/docker-machine-driver-hetzner_3.6.0_linux_amd64.tar.gz",
             whitelist_domains=["storage.googleapis.com"])
-        my_hetzner_node_template = rancher2.NodeTemplate("myHetznerNodeTemplate",
+        my_hetzner_node_template = rancher2.NodeTemplate("my_hetzner_node_template",
+            name="my-hetzner-node-template",
             driver_id=hetzner_node_driver.id,
             hetzner_config=rancher2.NodeTemplateHetznerConfigArgs(
                 api_token="XXXXXXXXXX",
                 image="ubuntu-18.04",
                 server_location="nbg1",
                 server_type="cx11",
             ))
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/notifier.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/notifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -471,21 +471,22 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Notifier
         foo = rancher2.Notifier("foo",
+            name="foo",
             cluster_id="<cluster_id>",
             description="Terraform notifier acceptance test",
+            send_resolved=True,
             pagerduty_config=rancher2.NotifierPagerdutyConfigArgs(
-                proxy_url="http://proxy.test.io",
                 service_key="XXXXXXXX",
-            ),
-            send_resolved=True)
+                proxy_url="http://proxy.test.io",
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Notifiers can be imported using the Rancher nNtifier ID
 
@@ -523,21 +524,22 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Notifier
         foo = rancher2.Notifier("foo",
+            name="foo",
             cluster_id="<cluster_id>",
             description="Terraform notifier acceptance test",
+            send_resolved=True,
             pagerduty_config=rancher2.NotifierPagerdutyConfigArgs(
-                proxy_url="http://proxy.test.io",
                 service_key="XXXXXXXX",
-            ),
-            send_resolved=True)
+                proxy_url="http://proxy.test.io",
+            ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Notifiers can be imported using the Rancher nNtifier ID
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/outputs.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/pod_security_admission_configuration_template.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/pod_security_admission_configuration_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/pod_security_policy_template.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/project.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,44 +405,58 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Project
         foo = rancher2.Project("foo",
+            name="foo",
             cluster_id="<CLUSTER_ID>",
-            container_resource_limit=rancher2.ProjectContainerResourceLimitArgs(
-                limits_cpu="20m",
-                limits_memory="20Mi",
-                requests_cpu="1m",
-                requests_memory="1Mi",
-            ),
             resource_quota=rancher2.ProjectResourceQuotaArgs(
-                namespace_default_limit=rancher2.ProjectResourceQuotaNamespaceDefaultLimitArgs(
-                    limits_cpu="2000m",
-                    limits_memory="500Mi",
-                    requests_storage="1Gi",
-                ),
                 project_limit=rancher2.ProjectResourceQuotaProjectLimitArgs(
                     limits_cpu="2000m",
                     limits_memory="2000Mi",
                     requests_storage="2Gi",
                 ),
+                namespace_default_limit=rancher2.ProjectResourceQuotaNamespaceDefaultLimitArgs(
+                    limits_cpu="2000m",
+                    limits_memory="500Mi",
+                    requests_storage="1Gi",
+                ),
+            ),
+            container_resource_limit=rancher2.ProjectContainerResourceLimitArgs(
+                limits_cpu="20m",
+                limits_memory="20Mi",
+                requests_cpu="1m",
+                requests_memory="1Mi",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Project enabling and customizing monitoring
         foo = rancher2.Project("foo",
+            name="foo",
             cluster_id="<CLUSTER_ID>",
+            resource_quota=rancher2.ProjectResourceQuotaArgs(
+                project_limit=rancher2.ProjectResourceQuotaProjectLimitArgs(
+                    limits_cpu="2000m",
+                    limits_memory="2000Mi",
+                    requests_storage="2Gi",
+                ),
+                namespace_default_limit=rancher2.ProjectResourceQuotaNamespaceDefaultLimitArgs(
+                    limits_cpu="2000m",
+                    limits_memory="500Mi",
+                    requests_storage="1Gi",
+                ),
+            ),
             container_resource_limit=rancher2.ProjectContainerResourceLimitArgs(
                 limits_cpu="20m",
                 limits_memory="20Mi",
                 requests_cpu="1m",
                 requests_memory="1Mi",
             ),
             enable_project_monitoring=True,
@@ -463,26 +477,14 @@
                     "prometheus.persistent.useReleaseName": "true",
                     "prometheus.resources.core.limits.cpu": "1000m",
                     "prometheus.resources.core.limits.memory": "1500Mi",
                     "prometheus.resources.core.requests.cpu": "750m",
                     "prometheus.resources.core.requests.memory": "750Mi",
                     "prometheus.retention": "12h",
                 },
-            ),
-            resource_quota=rancher2.ProjectResourceQuotaArgs(
-                namespace_default_limit=rancher2.ProjectResourceQuotaNamespaceDefaultLimitArgs(
-                    limits_cpu="2000m",
-                    limits_memory="500Mi",
-                    requests_storage="1Gi",
-                ),
-                project_limit=rancher2.ProjectResourceQuotaProjectLimitArgs(
-                    limits_cpu="2000m",
-                    limits_memory="2000Mi",
-                    requests_storage="2Gi",
-                ),
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Projects can be imported using the Rancher Project ID
@@ -519,44 +521,58 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Project
         foo = rancher2.Project("foo",
+            name="foo",
             cluster_id="<CLUSTER_ID>",
-            container_resource_limit=rancher2.ProjectContainerResourceLimitArgs(
-                limits_cpu="20m",
-                limits_memory="20Mi",
-                requests_cpu="1m",
-                requests_memory="1Mi",
-            ),
             resource_quota=rancher2.ProjectResourceQuotaArgs(
-                namespace_default_limit=rancher2.ProjectResourceQuotaNamespaceDefaultLimitArgs(
-                    limits_cpu="2000m",
-                    limits_memory="500Mi",
-                    requests_storage="1Gi",
-                ),
                 project_limit=rancher2.ProjectResourceQuotaProjectLimitArgs(
                     limits_cpu="2000m",
                     limits_memory="2000Mi",
                     requests_storage="2Gi",
                 ),
+                namespace_default_limit=rancher2.ProjectResourceQuotaNamespaceDefaultLimitArgs(
+                    limits_cpu="2000m",
+                    limits_memory="500Mi",
+                    requests_storage="1Gi",
+                ),
+            ),
+            container_resource_limit=rancher2.ProjectContainerResourceLimitArgs(
+                limits_cpu="20m",
+                limits_memory="20Mi",
+                requests_cpu="1m",
+                requests_memory="1Mi",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Project enabling and customizing monitoring
         foo = rancher2.Project("foo",
+            name="foo",
             cluster_id="<CLUSTER_ID>",
+            resource_quota=rancher2.ProjectResourceQuotaArgs(
+                project_limit=rancher2.ProjectResourceQuotaProjectLimitArgs(
+                    limits_cpu="2000m",
+                    limits_memory="2000Mi",
+                    requests_storage="2Gi",
+                ),
+                namespace_default_limit=rancher2.ProjectResourceQuotaNamespaceDefaultLimitArgs(
+                    limits_cpu="2000m",
+                    limits_memory="500Mi",
+                    requests_storage="1Gi",
+                ),
+            ),
             container_resource_limit=rancher2.ProjectContainerResourceLimitArgs(
                 limits_cpu="20m",
                 limits_memory="20Mi",
                 requests_cpu="1m",
                 requests_memory="1Mi",
             ),
             enable_project_monitoring=True,
@@ -577,26 +593,14 @@
                     "prometheus.persistent.useReleaseName": "true",
                     "prometheus.resources.core.limits.cpu": "1000m",
                     "prometheus.resources.core.limits.memory": "1500Mi",
                     "prometheus.resources.core.requests.cpu": "750m",
                     "prometheus.resources.core.requests.memory": "750Mi",
                     "prometheus.retention": "12h",
                 },
-            ),
-            resource_quota=rancher2.ProjectResourceQuotaArgs(
-                namespace_default_limit=rancher2.ProjectResourceQuotaNamespaceDefaultLimitArgs(
-                    limits_cpu="2000m",
-                    limits_memory="500Mi",
-                    requests_storage="1Gi",
-                ),
-                project_limit=rancher2.ProjectResourceQuotaProjectLimitArgs(
-                    limits_cpu="2000m",
-                    limits_memory="2000Mi",
-                    requests_storage="2Gi",
-                ),
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Projects can be imported using the Rancher Project ID
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/project_alert_group.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/project_alert_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,17 +339,18 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Project Alert Group
         foo = rancher2.ProjectAlertGroup("foo",
+            name="foo",
             description="Terraform project alert group",
-            group_interval_seconds=300,
             project_id="<project_id>",
+            group_interval_seconds=300,
             repeat_interval_seconds=3600)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Project Alert Group can be imported using the Rancher project alert group ID
@@ -384,17 +385,18 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Project Alert Group
         foo = rancher2.ProjectAlertGroup("foo",
+            name="foo",
             description="Terraform project alert group",
-            group_interval_seconds=300,
             project_id="<project_id>",
+            group_interval_seconds=300,
             repeat_interval_seconds=3600)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Project Alert Group can be imported using the Rancher project alert group ID
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/project_alert_rule.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/project_alert_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,15 +469,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Project
-        foo_project = rancher2.Project("fooProject",
+        foo = rancher2.Project("foo",
+            name="foo",
             cluster_id="<cluster_id>",
             description="Terraform project ",
             resource_quota=rancher2.ProjectResourceQuotaArgs(
                 project_limit=rancher2.ProjectResourceQuotaProjectLimitArgs(
                     limits_cpu="2000m",
                     limits_memory="2000Mi",
                     requests_storage="2Gi",
@@ -491,23 +492,25 @@
             container_resource_limit=rancher2.ProjectContainerResourceLimitArgs(
                 limits_cpu="20m",
                 limits_memory="20Mi",
                 requests_cpu="1m",
                 requests_memory="1Mi",
             ))
         # Create a new Rancher2 Project Alert Group
-        foo_project_alert_group = rancher2.ProjectAlertGroup("fooProjectAlertGroup",
+        foo_project_alert_group = rancher2.ProjectAlertGroup("foo",
+            name="foo",
             description="Terraform project alert group",
-            project_id=foo_project.id,
+            project_id=foo.id,
             group_interval_seconds=300,
             repeat_interval_seconds=3600)
         # Create a new Rancher2 Project Alert Rule
-        foo_project_alert_rule = rancher2.ProjectAlertRule("fooProjectAlertRule",
+        foo_project_alert_rule = rancher2.ProjectAlertRule("foo",
             project_id=foo_project_alert_group.project_id,
             group_id=foo_project_alert_group.id,
+            name="foo",
             group_interval_seconds=600,
             repeat_interval_seconds=6000)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -546,15 +549,16 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new Rancher2 Project
-        foo_project = rancher2.Project("fooProject",
+        foo = rancher2.Project("foo",
+            name="foo",
             cluster_id="<cluster_id>",
             description="Terraform project ",
             resource_quota=rancher2.ProjectResourceQuotaArgs(
                 project_limit=rancher2.ProjectResourceQuotaProjectLimitArgs(
                     limits_cpu="2000m",
                     limits_memory="2000Mi",
                     requests_storage="2Gi",
@@ -568,23 +572,25 @@
             container_resource_limit=rancher2.ProjectContainerResourceLimitArgs(
                 limits_cpu="20m",
                 limits_memory="20Mi",
                 requests_cpu="1m",
                 requests_memory="1Mi",
             ))
         # Create a new Rancher2 Project Alert Group
-        foo_project_alert_group = rancher2.ProjectAlertGroup("fooProjectAlertGroup",
+        foo_project_alert_group = rancher2.ProjectAlertGroup("foo",
+            name="foo",
             description="Terraform project alert group",
-            project_id=foo_project.id,
+            project_id=foo.id,
             group_interval_seconds=300,
             repeat_interval_seconds=3600)
         # Create a new Rancher2 Project Alert Rule
-        foo_project_alert_rule = rancher2.ProjectAlertRule("fooProjectAlertRule",
+        foo_project_alert_rule = rancher2.ProjectAlertRule("foo",
             project_id=foo_project_alert_group.project_id,
             group_id=foo_project_alert_group.id,
+            name="foo",
             group_interval_seconds=600,
             repeat_interval_seconds=6000)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/project_role_template_binding.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/project_role_template_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,14 +344,15 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Project Role Template Binding
         foo = rancher2.ProjectRoleTemplateBinding("foo",
+            name="foo",
             project_id="<project_id>",
             role_template_id="<role_template_id>",
             user_id="<user_id>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -390,14 +391,15 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Project Role Template Binding
         foo = rancher2.ProjectRoleTemplateBinding("foo",
+            name="foo",
             project_id="<project_id>",
             role_template_id="<role_template_id>",
             user_id="<user_id>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/provider.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/registry.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,38 +276,40 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Project Registry
         foo = rancher2.Registry("foo",
+            name="foo",
             description="Terraform registry foo",
             project_id="<project_id>",
             registries=[rancher2.RegistryRegistryArgs(
                 address="test.io",
-                password="pass",
                 username="user",
+                password="pass",
             )])
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Namespaced Registry
         foo = rancher2.Registry("foo",
+            name="foo",
             description="Terraform registry foo",
-            namespace_id="<namespace_id>",
             project_id="<project_id>",
+            namespace_id="<namespace_id>",
             registries=[rancher2.RegistryRegistryArgs(
                 address="test.io",
-                password="pass",
                 username="user2",
+                password="pass",
             )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Registries can be imported using the registry ID in the format `<namespace_id>.<project_id>.<registry_id>`
@@ -345,38 +347,40 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Project Registry
         foo = rancher2.Registry("foo",
+            name="foo",
             description="Terraform registry foo",
             project_id="<project_id>",
             registries=[rancher2.RegistryRegistryArgs(
                 address="test.io",
-                password="pass",
                 username="user",
+                password="pass",
             )])
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Namespaced Registry
         foo = rancher2.Registry("foo",
+            name="foo",
             description="Terraform registry foo",
-            namespace_id="<namespace_id>",
             project_id="<project_id>",
+            namespace_id="<namespace_id>",
             registries=[rancher2.RegistryRegistryArgs(
                 address="test.io",
-                password="pass",
                 username="user2",
+                password="pass",
             )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Registries can be imported using the registry ID in the format `<namespace_id>.<project_id>.<registry_id>`
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/role_template.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/role_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,14 +457,15 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 cluster Role Template
         foo = rancher2.RoleTemplate("foo",
+            name="foo",
             context="cluster",
             default_role=True,
             description="Terraform role template acceptance test",
             rules=[rancher2.RoleTemplateRuleArgs(
                 api_groups=["*"],
                 resources=["secrets"],
                 verbs=["create"],
@@ -475,14 +476,15 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 project Role Template
         foo = rancher2.RoleTemplate("foo",
+            name="foo",
             context="project",
             default_role=True,
             description="Terraform role template acceptance test",
             rules=[rancher2.RoleTemplateRuleArgs(
                 api_groups=["*"],
                 resources=["secrets"],
                 verbs=["create"],
@@ -529,14 +531,15 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 cluster Role Template
         foo = rancher2.RoleTemplate("foo",
+            name="foo",
             context="cluster",
             default_role=True,
             description="Terraform role template acceptance test",
             rules=[rancher2.RoleTemplateRuleArgs(
                 api_groups=["*"],
                 resources=["secrets"],
                 verbs=["create"],
@@ -547,14 +550,15 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 project Role Template
         foo = rancher2.RoleTemplate("foo",
+            name="foo",
             context="project",
             default_role=True,
             description="Terraform role template acceptance test",
             rules=[rancher2.RoleTemplateRuleArgs(
                 api_groups=["*"],
                 resources=["secrets"],
                 verbs=["create"],
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/secret.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/secret.py`

 * *Files 18% similar despite different names*

```diff
@@ -265,14 +265,55 @@
         """
         Provides a Rancher v2 Secret resource. This can be used to create secrets for Rancher v2 environments and retrieve their information.
 
         Depending of the availability, there are 2 types of Rancher v2 secrets:
         - Project secret: Available to all namespaces in the `project_id`
         - Namespaced secret: Available to just `namespace_id` in the `project_id`
 
+        ## Example Usage
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_rancher2 as rancher2
+        import pulumi_std as std
+
+        # Create a new rancher2 Project Secret
+        foo = rancher2.Secret("foo",
+            name="foo",
+            description="Terraform secret foo",
+            project_id="<project_id>",
+            data={
+                "address": std.base64encode(input="test.io").result,
+                "username": std.base64encode(input="user2").result,
+                "password": std.base64encode(input="pass").result,
+            })
+        ```
+        <!--End PulumiCodeChooser -->
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_rancher2 as rancher2
+        import pulumi_std as std
+
+        # Create a new rancher2 Namespaced Secret
+        foo = rancher2.Secret("foo",
+            name="foo",
+            description="Terraform secret foo",
+            project_id="<project_id>",
+            namespace_id="<namespace_id>",
+            data={
+                "address": std.base64encode(input="test.io").result,
+                "username": std.base64encode(input="user2").result,
+                "password": std.base64encode(input="pass").result,
+            })
+        ```
+        <!--End PulumiCodeChooser -->
+
         ## Import
 
         Secrets can be imported using the secret ID in the format `<namespace_id>.<project_id>.<secret_id>`
 
         ```sh
         $ pulumi import rancher2:index/secret:Secret foo &lt;namespace_id&gt;.&lt;project_id&gt;.&lt;secret_id&gt;
         ```
@@ -297,14 +338,55 @@
         """
         Provides a Rancher v2 Secret resource. This can be used to create secrets for Rancher v2 environments and retrieve their information.
 
         Depending of the availability, there are 2 types of Rancher v2 secrets:
         - Project secret: Available to all namespaces in the `project_id`
         - Namespaced secret: Available to just `namespace_id` in the `project_id`
 
+        ## Example Usage
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_rancher2 as rancher2
+        import pulumi_std as std
+
+        # Create a new rancher2 Project Secret
+        foo = rancher2.Secret("foo",
+            name="foo",
+            description="Terraform secret foo",
+            project_id="<project_id>",
+            data={
+                "address": std.base64encode(input="test.io").result,
+                "username": std.base64encode(input="user2").result,
+                "password": std.base64encode(input="pass").result,
+            })
+        ```
+        <!--End PulumiCodeChooser -->
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_rancher2 as rancher2
+        import pulumi_std as std
+
+        # Create a new rancher2 Namespaced Secret
+        foo = rancher2.Secret("foo",
+            name="foo",
+            description="Terraform secret foo",
+            project_id="<project_id>",
+            namespace_id="<namespace_id>",
+            data={
+                "address": std.base64encode(input="test.io").result,
+                "username": std.base64encode(input="user2").result,
+                "password": std.base64encode(input="pass").result,
+            })
+        ```
+        <!--End PulumiCodeChooser -->
+
         ## Import
 
         Secrets can be imported using the secret ID in the format `<namespace_id>.<project_id>.<secret_id>`
 
         ```sh
         $ pulumi import rancher2:index/secret:Secret foo &lt;namespace_id&gt;.&lt;project_id&gt;.&lt;secret_id&gt;
         ```
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/secret_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/setting.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Setting
-        foo = rancher2.Setting("foo", value="<VALUE>")
+        foo = rancher2.Setting("foo",
+            name="foo",
+            value="<VALUE>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Setting can be imported using the Rancher setting ID.
 
@@ -215,15 +217,17 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 Setting
-        foo = rancher2.Setting("foo", value="<VALUE>")
+        foo = rancher2.Setting("foo",
+            name="foo",
+            value="<VALUE>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Setting can be imported using the Rancher setting ID.
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/storage_class_v2.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/token.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,29 +356,14 @@
 
         There are 2 kind of tokens:
         - no scoped: valid for global system.
         - scoped: valid for just a specific cluster (`cluster_id` should be provided).
 
         Tokens can't be updated once created. Any diff in token data will recreate the token. If any token expire, Rancher2 provider will generate a diff to regenerate it.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_rancher2 as rancher2
-
-        # Create a new rancher2 Token scoped
-        foo = rancher2.Token("foo",
-            cluster_id="<cluster-id>",
-            description="foo token",
-            ttl=1200)
-        ```
-        <!--End PulumiCodeChooser -->
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] annotations: (Computed) Annotations of the token (map)
         :param pulumi.Input[str] cluster_id: Cluster ID for scoped token (string)
         :param pulumi.Input[str] description: Token description (string)
         :param pulumi.Input[Mapping[str, Any]] labels: (Computed) Labels of the token (map)
         :param pulumi.Input[bool] renew: Renew expired or disabled token
@@ -397,29 +382,14 @@
 
         There are 2 kind of tokens:
         - no scoped: valid for global system.
         - scoped: valid for just a specific cluster (`cluster_id` should be provided).
 
         Tokens can't be updated once created. Any diff in token data will recreate the token. If any token expire, Rancher2 provider will generate a diff to regenerate it.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_rancher2 as rancher2
-
-        # Create a new rancher2 Token scoped
-        foo = rancher2.Token("foo",
-            cluster_id="<cluster-id>",
-            description="foo token",
-            ttl=1200)
-        ```
-        <!--End PulumiCodeChooser -->
-
         :param str resource_name: The name of the resource.
         :param TokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(TokenArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2/user.py` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -246,22 +246,24 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 User
-        foo_user = rancher2.User("fooUser",
+        foo = rancher2.User("foo",
+            name="Foo user",
             username="foo",
             password="changeme",
             enabled=True)
         # Create a new rancher2 global_role_binding for User
-        foo_global_role_binding = rancher2.GlobalRoleBinding("fooGlobalRoleBinding",
+        foo_global_role_binding = rancher2.GlobalRoleBinding("foo",
+            name="foo",
             global_role_id="user-base",
-            user_id=foo_user.id)
+            user_id=foo.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported using the Rancher User ID
 
@@ -292,22 +294,24 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rancher2 as rancher2
 
         # Create a new rancher2 User
-        foo_user = rancher2.User("fooUser",
+        foo = rancher2.User("foo",
+            name="Foo user",
             username="foo",
             password="changeme",
             enabled=True)
         # Create a new rancher2 global_role_binding for User
-        foo_global_role_binding = rancher2.GlobalRoleBinding("fooGlobalRoleBinding",
+        foo_global_role_binding = rancher2.GlobalRoleBinding("foo",
+            name="foo",
             global_role_id="user-base",
-            user_id=foo_user.id)
+            user_id=foo.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported using the Rancher User ID
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2.egg-info/PKG-INFO` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 6.2.0a1713337589
+Version: 6.2.0a1713561342
 Summary: A Pulumi package for creating and managing rancher2 resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi,rancher2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rancher2-6.2.0a1713337589/pulumi_rancher2.egg-info/SOURCES.txt` & `pulumi_rancher2-6.2.0a1713561342/pulumi_rancher2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-6.2.0a1713337589/pyproject.toml` & `pulumi_rancher2-6.2.0a1713561342/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rancher2"
   description = "A Pulumi package for creating and managing rancher2 resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rancher2"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "6.2.0a1713337589"
+  version = "6.2.0a1713561342"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rancher2"
 
 [build-system]
```

