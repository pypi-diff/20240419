# Comparing `tmp/pulumi_materialize-0.1.8.tar.gz` & `tmp/pulumi_materialize-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_materialize-0.1.8.tar", last modified: Wed Mar 20 22:20:09 2024, max compression
+gzip compressed data, was "pulumi_materialize-0.1.9.tar", last modified: Fri Mar 29 16:44:52 2024, max compression
```

## Comparing `pulumi_materialize-0.1.8.tar` & `pulumi_materialize-0.1.9.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:20:09.864806 pulumi_materialize-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-20 22:20:09.864806 pulumi_materialize-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:20:09.864806 pulumi_materialize-0.1.8/pulumi_materialize/
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   208675 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/app_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    32086 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    30123 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/cluster_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:20:09.864806 pulumi_materialize-0.1.8/pulumi_materialize/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    38924 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/connection_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    25847 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/connection_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)    46174 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/connection_confluent_schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    54306 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/connection_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    47019 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/connection_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/connection_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    26451 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/connection_ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_cluster_replicas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_current_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_current_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_egress_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_materialized_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_scim_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_sinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_sso_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_system_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/get_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    15563 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_cluster_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17766 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20573 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_connection_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_database_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    18429 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    18124 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_schema_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17366 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_secret_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17346 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_system_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17558 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    20743 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_table_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_type_default_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/grant_view.py
--rw-r--r--   0 runner    (1001) docker     (127)    24878 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    28616 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/materialized_view.py
--rw-r--r--   0 runner    (1001) docker     (127)   239623 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/scim2_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    44082 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/sink_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    68779 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/source_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    38877 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/source_loadgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    36122 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/source_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    41674 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/source_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    37565 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/source_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/sso_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/sso_default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/sso_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/sso_role_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/system_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    27574 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:20:09.864806 pulumi_materialize-0.1.8/pulumi_materialize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/pulumi_materialize.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 22:20:09.864806 pulumi_materialize-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-20 22:20:09.000000 pulumi_materialize-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/pulumi_materialize/
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   208675 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/app_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32086 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30123 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/cluster_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/pulumi_materialize/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38924 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25847 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46174 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_confluent_schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54306 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47019 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49006 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28437 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/connection_ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_cluster_replicas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_current_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_current_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_egress_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_materialized_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_scim_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_scim_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_sso_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_system_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/get_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15563 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_cluster_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17766 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20573 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_connection_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15697 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_database_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18429 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18124 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_schema_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17366 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_secret_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17346 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_system_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17558 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20743 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_table_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_type_default_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/grant_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24878 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28616 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)   239623 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/role_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/scim2_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21139 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44082 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/sink_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68779 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/source_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38877 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/source_loadgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36122 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/source_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41674 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/source_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37565 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/source_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24196 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/sso_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/sso_default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/sso_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/sso_role_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/system_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27574 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/pulumi_materialize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 16:44:52.431204 pulumi_materialize-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-29 16:44:52.000000 pulumi_materialize-0.1.9/setup.py
```

### Comparing `pulumi_materialize-0.1.8/PKG-INFO` & `pulumi_materialize-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_materialize
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Pulumi package for creating and managing materialize cloud resources.
 Home-page: https://github.com/MaterializeInc/terraform-provider-materialize
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaterializeInc/terraform-provider-materialize
 Keywords: pulumi materialize category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_materialize-0.1.8/README.md` & `pulumi_materialize-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/__init__.py` & `pulumi_materialize-0.1.9/pulumi_materialize/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 from .grant_type_default_privilege import *
 from .grant_view import *
 from .index import *
 from .materialized_view import *
 from .provider import *
 from .region import *
 from .role import *
+from .role_parameter import *
 from .schema import *
 from .scim2_configuration import *
 from .secret import *
 from .sink_kafka import *
 from .source_kafka import *
 from .source_loadgen import *
 from .source_mysql import *
@@ -354,14 +355,22 @@
   "fqn": "pulumi_materialize",
   "classes": {
    "materialize:index/role:Role": "Role"
   }
  },
  {
   "pkg": "materialize",
+  "mod": "index/roleParameter",
+  "fqn": "pulumi_materialize",
+  "classes": {
+   "materialize:index/roleParameter:RoleParameter": "RoleParameter"
+  }
+ },
+ {
+  "pkg": "materialize",
   "mod": "index/sCIM2Configuration",
   "fqn": "pulumi_materialize",
   "classes": {
    "materialize:index/sCIM2Configuration:SCIM2Configuration": "SCIM2Configuration"
   }
  },
  {
```

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/_inputs.py` & `pulumi_materialize-0.1.9/pulumi_materialize/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/_utilities.py` & `pulumi_materialize-0.1.9/pulumi_materialize/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/app_password.py` & `pulumi_materialize-0.1.9/pulumi_materialize/app_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/cluster.py` & `pulumi_materialize-0.1.9/pulumi_materialize/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/cluster_replica.py` & `pulumi_materialize-0.1.9/pulumi_materialize/cluster_replica.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/config/vars.py` & `pulumi_materialize-0.1.9/pulumi_materialize/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/connection_aws.py` & `pulumi_materialize-0.1.9/pulumi_materialize/connection_aws.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/connection_aws_privatelink.py` & `pulumi_materialize-0.1.9/pulumi_materialize/connection_aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/connection_confluent_schema_registry.py` & `pulumi_materialize-0.1.9/pulumi_materialize/connection_confluent_schema_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/connection_kafka.py` & `pulumi_materialize-0.1.9/pulumi_materialize/connection_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/connection_mysql.py` & `pulumi_materialize-0.1.9/pulumi_materialize/connection_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/connection_postgres.py` & `pulumi_materialize-0.1.9/pulumi_materialize/connection_postgres.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/connection_ssh_tunnel.py` & `pulumi_materialize-0.1.9/pulumi_materialize/connection_ssh_tunnel.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,28 @@
                  port: pulumi.Input[int],
                  user: pulumi.Input[str],
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
-                 schema_name: Optional[pulumi.Input[str]] = None):
+                 schema_name: Optional[pulumi.Input[str]] = None,
+                 validate: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ConnectionSshTunnel resource.
         :param pulumi.Input[str] host: The host of the SSH tunnel.
         :param pulumi.Input[int] port: The port of the SSH tunnel.
         :param pulumi.Input[str] user: The user of the SSH tunnel.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the connection database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input[str] name: The identifier for the connection.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the connection schema in Materialize. Defaults to `public`.
+        :param pulumi.Input[bool] validate: **Private Preview** If the connection should wait for validation.
         """
         pulumi.set(__self__, "host", host)
         pulumi.set(__self__, "port", port)
         pulumi.set(__self__, "user", user)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if database_name is not None:
@@ -46,14 +48,16 @@
             pulumi.set(__self__, "name", name)
         if ownership_role is not None:
             pulumi.set(__self__, "ownership_role", ownership_role)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
+        if validate is not None:
+            pulumi.set(__self__, "validate", validate)
 
     @property
     @pulumi.getter
     def host(self) -> pulumi.Input[str]:
         """
         The host of the SSH tunnel.
         """
@@ -155,14 +159,26 @@
         """
         return pulumi.get(self, "schema_name")
 
     @schema_name.setter
     def schema_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "schema_name", value)
 
+    @property
+    @pulumi.getter
+    def validate(self) -> Optional[pulumi.Input[bool]]:
+        """
+        **Private Preview** If the connection should wait for validation.
+        """
+        return pulumi.get(self, "validate")
+
+    @validate.setter
+    def validate(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "validate", value)
+
 
 @pulumi.input_type
 class _ConnectionSshTunnelState:
     def __init__(__self__, *,
                  comment: Optional[pulumi.Input[str]] = None,
                  database_name: Optional[pulumi.Input[str]] = None,
                  host: Optional[pulumi.Input[str]] = None,
@@ -170,29 +186,31 @@
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  public_key1: Optional[pulumi.Input[str]] = None,
                  public_key2: Optional[pulumi.Input[str]] = None,
                  qualified_sql_name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
-                 user: Optional[pulumi.Input[str]] = None):
+                 user: Optional[pulumi.Input[str]] = None,
+                 validate: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering ConnectionSshTunnel resources.
         :param pulumi.Input[str] comment: **Public Preview** Comment on an object in the database.
         :param pulumi.Input[str] database_name: The identifier for the connection database in Materialize. Defaults to `MZ_DATABASE` environment variable if set or `materialize` if environment variable is not set.
         :param pulumi.Input[str] host: The host of the SSH tunnel.
         :param pulumi.Input[str] name: The identifier for the connection.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[int] port: The port of the SSH tunnel.
         :param pulumi.Input[str] public_key1: The first public key associated with the SSH tunnel.
         :param pulumi.Input[str] public_key2: The second public key associated with the SSH tunnel.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the connection.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the connection schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] user: The user of the SSH tunnel.
+        :param pulumi.Input[bool] validate: **Private Preview** If the connection should wait for validation.
         """
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if database_name is not None:
             pulumi.set(__self__, "database_name", database_name)
         if host is not None:
             pulumi.set(__self__, "host", host)
@@ -210,14 +228,16 @@
             pulumi.set(__self__, "qualified_sql_name", qualified_sql_name)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if schema_name is not None:
             pulumi.set(__self__, "schema_name", schema_name)
         if user is not None:
             pulumi.set(__self__, "user", user)
+        if validate is not None:
+            pulumi.set(__self__, "validate", validate)
 
     @property
     @pulumi.getter
     def comment(self) -> Optional[pulumi.Input[str]]:
         """
         **Public Preview** Comment on an object in the database.
         """
@@ -355,14 +375,26 @@
         """
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user", value)
 
+    @property
+    @pulumi.getter
+    def validate(self) -> Optional[pulumi.Input[bool]]:
+        """
+        **Private Preview** If the connection should wait for validation.
+        """
+        return pulumi.get(self, "validate")
+
+    @validate.setter
+    def validate(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "validate", value)
+
 
 class ConnectionSshTunnel(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  comment: Optional[pulumi.Input[str]] = None,
@@ -370,14 +402,15 @@
                  host: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None,
+                 validate: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         An SSH tunnel connection establishes a link to an SSH bastion server.
 
         ## Example Usage
 
         ```python
@@ -409,14 +442,15 @@
         :param pulumi.Input[str] host: The host of the SSH tunnel.
         :param pulumi.Input[str] name: The identifier for the connection.
         :param pulumi.Input[str] ownership_role: The owernship role of the object.
         :param pulumi.Input[int] port: The port of the SSH tunnel.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the connection schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] user: The user of the SSH tunnel.
+        :param pulumi.Input[bool] validate: **Private Preview** If the connection should wait for validation.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ConnectionSshTunnelArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -467,14 +501,15 @@
                  host: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ownership_role: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  schema_name: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None,
+                 validate: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -491,14 +526,15 @@
                 raise TypeError("Missing required property 'port'")
             __props__.__dict__["port"] = port
             __props__.__dict__["region"] = region
             __props__.__dict__["schema_name"] = schema_name
             if user is None and not opts.urn:
                 raise TypeError("Missing required property 'user'")
             __props__.__dict__["user"] = user
+            __props__.__dict__["validate"] = validate
             __props__.__dict__["public_key1"] = None
             __props__.__dict__["public_key2"] = None
             __props__.__dict__["qualified_sql_name"] = None
         super(ConnectionSshTunnel, __self__).__init__(
             'materialize:index/connectionSshTunnel:ConnectionSshTunnel',
             resource_name,
             __props__,
@@ -515,15 +551,16 @@
             ownership_role: Optional[pulumi.Input[str]] = None,
             port: Optional[pulumi.Input[int]] = None,
             public_key1: Optional[pulumi.Input[str]] = None,
             public_key2: Optional[pulumi.Input[str]] = None,
             qualified_sql_name: Optional[pulumi.Input[str]] = None,
             region: Optional[pulumi.Input[str]] = None,
             schema_name: Optional[pulumi.Input[str]] = None,
-            user: Optional[pulumi.Input[str]] = None) -> 'ConnectionSshTunnel':
+            user: Optional[pulumi.Input[str]] = None,
+            validate: Optional[pulumi.Input[bool]] = None) -> 'ConnectionSshTunnel':
         """
         Get an existing ConnectionSshTunnel resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -535,14 +572,15 @@
         :param pulumi.Input[int] port: The port of the SSH tunnel.
         :param pulumi.Input[str] public_key1: The first public key associated with the SSH tunnel.
         :param pulumi.Input[str] public_key2: The second public key associated with the SSH tunnel.
         :param pulumi.Input[str] qualified_sql_name: The fully qualified name of the connection.
         :param pulumi.Input[str] region: The region to use for the resource connection. If not set, the default region is used.
         :param pulumi.Input[str] schema_name: The identifier for the connection schema in Materialize. Defaults to `public`.
         :param pulumi.Input[str] user: The user of the SSH tunnel.
+        :param pulumi.Input[bool] validate: **Private Preview** If the connection should wait for validation.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ConnectionSshTunnelState.__new__(_ConnectionSshTunnelState)
 
         __props__.__dict__["comment"] = comment
         __props__.__dict__["database_name"] = database_name
@@ -552,14 +590,15 @@
         __props__.__dict__["port"] = port
         __props__.__dict__["public_key1"] = public_key1
         __props__.__dict__["public_key2"] = public_key2
         __props__.__dict__["qualified_sql_name"] = qualified_sql_name
         __props__.__dict__["region"] = region
         __props__.__dict__["schema_name"] = schema_name
         __props__.__dict__["user"] = user
+        __props__.__dict__["validate"] = validate
         return ConnectionSshTunnel(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
         """
         **Public Preview** Comment on an object in the database.
@@ -650,7 +689,15 @@
     @pulumi.getter
     def user(self) -> pulumi.Output[str]:
         """
         The user of the SSH tunnel.
         """
         return pulumi.get(self, "user")
 
+    @property
+    @pulumi.getter
+    def validate(self) -> pulumi.Output[Optional[bool]]:
+        """
+        **Private Preview** If the connection should wait for validation.
+        """
+        return pulumi.get(self, "validate")
+
```

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/database.py` & `pulumi_materialize-0.1.9/pulumi_materialize/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_cluster_replicas.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_cluster_replicas.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_clusters.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_connections.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_connections.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_current_cluster.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_current_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_current_database.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_current_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_databases.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_egress_ips.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_egress_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_indexes.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_indexes.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_materialized_views.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_materialized_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_roles.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_schemas.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_schemas.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_scim_configs.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_scim_configs.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_scim_groups.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_scim_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_secrets.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_sinks.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_sinks.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_sources.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_sources.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_sso_config.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_sso_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_system_parameters.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_system_parameters.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_tables.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_types.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/get_views.py` & `pulumi_materialize-0.1.9/pulumi_materialize/get_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_cluster.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_cluster_default_privilege.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_cluster_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_connection.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_connection_default_privilege.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_connection_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_database.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_database_default_privilege.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_database_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_materialized_view.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_materialized_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_role.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_schema.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_schema_default_privilege.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_schema_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_secret.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_secret_default_privilege.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_secret_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_source.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_system_privilege.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_system_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_table.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_table.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_table_default_privilege.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_table_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_type.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_type_default_privilege.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_type_default_privilege.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/grant_view.py` & `pulumi_materialize-0.1.9/pulumi_materialize/grant_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/index.py` & `pulumi_materialize-0.1.9/pulumi_materialize/index.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/materialized_view.py` & `pulumi_materialize-0.1.9/pulumi_materialize/materialized_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/outputs.py` & `pulumi_materialize-0.1.9/pulumi_materialize/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/provider.py` & `pulumi_materialize-0.1.9/pulumi_materialize/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/region.py` & `pulumi_materialize-0.1.9/pulumi_materialize/region.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/role.py` & `pulumi_materialize-0.1.9/pulumi_materialize/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/schema.py` & `pulumi_materialize-0.1.9/pulumi_materialize/schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/scim2_configuration.py` & `pulumi_materialize-0.1.9/pulumi_materialize/scim2_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/secret.py` & `pulumi_materialize-0.1.9/pulumi_materialize/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/sink_kafka.py` & `pulumi_materialize-0.1.9/pulumi_materialize/sink_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/source_kafka.py` & `pulumi_materialize-0.1.9/pulumi_materialize/source_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/source_loadgen.py` & `pulumi_materialize-0.1.9/pulumi_materialize/source_loadgen.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/source_mysql.py` & `pulumi_materialize-0.1.9/pulumi_materialize/source_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/source_postgres.py` & `pulumi_materialize-0.1.9/pulumi_materialize/source_postgres.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/source_webhook.py` & `pulumi_materialize-0.1.9/pulumi_materialize/source_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/sso_config.py` & `pulumi_materialize-0.1.9/pulumi_materialize/sso_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/sso_default_roles.py` & `pulumi_materialize-0.1.9/pulumi_materialize/sso_default_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/sso_domain.py` & `pulumi_materialize-0.1.9/pulumi_materialize/sso_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/sso_role_group_mapping.py` & `pulumi_materialize-0.1.9/pulumi_materialize/sso_role_group_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/system_parameter.py` & `pulumi_materialize-0.1.9/pulumi_materialize/system_parameter.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/table.py` & `pulumi_materialize-0.1.9/pulumi_materialize/table.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/type.py` & `pulumi_materialize-0.1.9/pulumi_materialize/type.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/user.py` & `pulumi_materialize-0.1.9/pulumi_materialize/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize/view.py` & `pulumi_materialize-0.1.9/pulumi_materialize/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize.egg-info/PKG-INFO` & `pulumi_materialize-0.1.9/pulumi_materialize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-materialize
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Pulumi package for creating and managing materialize cloud resources.
 Home-page: https://github.com/MaterializeInc/terraform-provider-materialize
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaterializeInc/terraform-provider-materialize
 Keywords: pulumi materialize category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_materialize-0.1.8/pulumi_materialize.egg-info/SOURCES.txt` & `pulumi_materialize-0.1.9/pulumi_materialize.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 pulumi_materialize/materialized_view.py
 pulumi_materialize/outputs.py
 pulumi_materialize/provider.py
 pulumi_materialize/pulumi-plugin.json
 pulumi_materialize/py.typed
 pulumi_materialize/region.py
 pulumi_materialize/role.py
+pulumi_materialize/role_parameter.py
 pulumi_materialize/schema.py
 pulumi_materialize/scim2_configuration.py
 pulumi_materialize/secret.py
 pulumi_materialize/sink_kafka.py
 pulumi_materialize/source_kafka.py
 pulumi_materialize/source_loadgen.py
 pulumi_materialize/source_mysql.py
```

### Comparing `pulumi_materialize-0.1.8/setup.py` & `pulumi_materialize-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "materialize Pulumi Package - Development Version"
```

