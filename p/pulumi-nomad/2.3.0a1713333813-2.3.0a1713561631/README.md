# Comparing `tmp/pulumi_nomad-2.3.0a1713333813.tar.gz` & `tmp/pulumi_nomad-2.3.0a1713561631.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_nomad-2.3.0a1713333813.tar", last modified: Wed Apr 17 06:23:44 2024, max compression
+gzip compressed data, was "pulumi_nomad-2.3.0a1713561631.tar", last modified: Fri Apr 19 21:30:04 2024, max compression
```

## Comparing `pulumi_nomad-2.3.0a1713333813.tar` & `pulumi_nomad-2.3.0a1713561631.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:23:44.224483 pulumi_nomad-2.3.0a1713333813/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-17 06:23:44.224483 pulumi_nomad-2.3.0a1713333813/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:23:44.220483 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73944 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23832 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/acl_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/acl_binding_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/acl_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    29169 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/acl_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:23:44.224483 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    50670 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/csi_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    52609 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/csi_volume_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    52423 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/external_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_allocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_job_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_node_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_scaling_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_scaling_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_scheduler_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)    51951 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13234 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)   100555 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21549 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/quote_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/scheduler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    17156 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/sentinel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    57464 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:23:44.224483 pulumi_nomad-2.3.0a1713333813/pulumi_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-17 06:23:44.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-17 06:23:44.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:23:44.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 06:23:44.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 06:23:44.000000 pulumi_nomad-2.3.0a1713333813/pulumi_nomad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-17 06:23:36.000000 pulumi_nomad-2.3.0a1713333813/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:23:44.224483 pulumi_nomad-2.3.0a1713333813/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:04.172101 pulumi_nomad-2.3.0a1713561631/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-19 21:30:04.172101 pulumi_nomad-2.3.0a1713561631/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:04.168101 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73944 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23930 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16396 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_binding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29351 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:04.172101 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50670 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/csi_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52609 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/csi_volume_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52663 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/external_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_allocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_job_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_node_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scaling_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scaling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scheduler_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51951 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20817 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100555 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21549 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/quote_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/scheduler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17214 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/sentinel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11841 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57678 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:04.172101 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-19 21:30:04.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-19 21:30:04.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:30:04.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:30:04.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 21:30:04.000000 pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-19 21:29:57.000000 pulumi_nomad-2.3.0a1713561631/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:30:04.172101 pulumi_nomad-2.3.0a1713561631/setup.cfg
```

### Comparing `pulumi_nomad-2.3.0a1713333813/PKG-INFO` & `pulumi_nomad-2.3.0a1713561631/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_nomad
-Version: 2.3.0a1713333813
+Version: 2.3.0a1713561631
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi,nomad
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_nomad-2.3.0a1713333813/README.md` & `pulumi_nomad-2.3.0a1713561631/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/__init__.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/_inputs.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/_utilities.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/acl_auth_method.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_auth_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,16 @@
         Creating an ALC Auth Method:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
-        my_nomad_acl_auth_method = nomad.AclAuthMethod("myNomadAclAuthMethod",
+        my_nomad_acl_auth_method = nomad.AclAuthMethod("my_nomad_acl_auth_method",
+            name="my-nomad-acl-auth-method",
             type="OIDC",
             token_locality="global",
             max_token_ttl="10m0s",
             token_name_format="${auth_method_type}-${value.user}",
             default=True,
             config=nomad.AclAuthMethodConfigArgs(
                 oidc_discovery_url="https://uk.auth0.com/",
@@ -360,15 +361,16 @@
         Creating an ALC Auth Method:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
-        my_nomad_acl_auth_method = nomad.AclAuthMethod("myNomadAclAuthMethod",
+        my_nomad_acl_auth_method = nomad.AclAuthMethod("my_nomad_acl_auth_method",
+            name="my-nomad-acl-auth-method",
             type="OIDC",
             token_locality="global",
             max_token_ttl="10m0s",
             token_name_format="${auth_method_type}-${value.user}",
             default=True,
             config=nomad.AclAuthMethodConfigArgs(
                 oidc_discovery_url="https://uk.auth0.com/",
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/acl_binding_rule.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_binding_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/acl_policy.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,46 +169,14 @@
                  job_acl: Optional[pulumi.Input[pulumi.InputType['AclPolicyJobAclArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  rules_hcl: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages an ACL policy registered in Nomad.
 
-        ## Example Usage
-
-        Registering a policy from a HCL file:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_nomad as nomad
-
-        dev = nomad.AclPolicy("dev",
-            description="Submit jobs to the dev environment.",
-            rules_hcl=(lambda path: open(path).read())(f"{path['module']}/dev.hcl"))
-        ```
-        <!--End PulumiCodeChooser -->
-
-        Registering a policy from inline HCL:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_nomad as nomad
-
-        dev = nomad.AclPolicy("dev",
-            description="Submit jobs to the dev environment.",
-            rules_hcl=\"\"\"namespace "dev" {
-          policy = "write"
-        }
-
-        \"\"\")
-        ```
-        <!--End PulumiCodeChooser -->
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: `(string: "")` - A description of the policy.
         :param pulumi.Input[pulumi.InputType['AclPolicyJobAclArgs']] job_acl: `(``JobACL``: <optional>)` - Options for assigning the ACL rules to a job, group, or task.
         :param pulumi.Input[str] name: `(string: <required>)` - A unique name for the policy.
         :param pulumi.Input[str] rules_hcl: `(string: <required>)` - The contents of the policy to register,
                as HCL or JSON.
@@ -218,46 +186,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: AclPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages an ACL policy registered in Nomad.
 
-        ## Example Usage
-
-        Registering a policy from a HCL file:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_nomad as nomad
-
-        dev = nomad.AclPolicy("dev",
-            description="Submit jobs to the dev environment.",
-            rules_hcl=(lambda path: open(path).read())(f"{path['module']}/dev.hcl"))
-        ```
-        <!--End PulumiCodeChooser -->
-
-        Registering a policy from inline HCL:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_nomad as nomad
-
-        dev = nomad.AclPolicy("dev",
-            description="Submit jobs to the dev environment.",
-            rules_hcl=\"\"\"namespace "dev" {
-          policy = "write"
-        }
-
-        \"\"\")
-        ```
-        <!--End PulumiCodeChooser -->
-
         :param str resource_name: The name of the resource.
         :param AclPolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(AclPolicyArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/acl_role.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/acl_token.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/acl_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,47 +353,51 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dakota = nomad.AclToken("dakota",
+            name="Dakota",
+            type="client",
             policies=[
                 "dev",
                 "qa",
-            ],
-            type="client")
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         Creating a global token that will be replicated to all regions:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dakota = nomad.AclToken("dakota",
-            global_=True,
+            name="Dakota",
+            type="client",
             policies=[
                 "dev",
                 "qa",
             ],
-            type="client")
+            global_=True)
         ```
         <!--End PulumiCodeChooser -->
 
         Creating a token with full access to the cluster:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
-        iman = nomad.AclToken("iman", type="management")
+        iman = nomad.AclToken("iman",
+            name="Iman",
+            type="management")
         ```
         <!--End PulumiCodeChooser -->
 
         Accessing the token:
 
         <!--Start PulumiCodeChooser -->
         ```python
@@ -440,47 +444,51 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dakota = nomad.AclToken("dakota",
+            name="Dakota",
+            type="client",
             policies=[
                 "dev",
                 "qa",
-            ],
-            type="client")
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         Creating a global token that will be replicated to all regions:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dakota = nomad.AclToken("dakota",
-            global_=True,
+            name="Dakota",
+            type="client",
             policies=[
                 "dev",
                 "qa",
             ],
-            type="client")
+            global_=True)
         ```
         <!--End PulumiCodeChooser -->
 
         Creating a token with full access to the cluster:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
-        iman = nomad.AclToken("iman", type="management")
+        iman = nomad.AclToken("iman",
+            name="Iman",
+            type="management")
         ```
         <!--End PulumiCodeChooser -->
 
         Accessing the token:
 
         <!--Start PulumiCodeChooser -->
         ```python
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/config/__init__.pyi` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/config/outputs.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/config/vars.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/csi_volume.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/csi_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/csi_volume_registration.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/csi_volume_registration.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/external_volume.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/external_volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -644,20 +644,22 @@
         Creating a volume:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
+        # It can sometimes be helpful to wait for a particular plugin to be available
         ebs = nomad.get_plugin(plugin_id="aws-ebs0",
             wait_for_healthy=True)
-        mysql_volume = nomad.ExternalVolume("mysqlVolume",
+        mysql_volume = nomad.ExternalVolume("mysql_volume",
             type="csi",
             plugin_id="aws-ebs0",
             volume_id="mysql_volume",
+            name="mysql_volume",
             capacity_min="10GiB",
             capacity_max="20GiB",
             capabilities=[nomad.ExternalVolumeCapabilityArgs(
                 access_mode="single-node-writer",
                 attachment_mode="file-system",
             )],
             mount_options=nomad.ExternalVolumeMountOptionsArgs(
@@ -713,20 +715,22 @@
         Creating a volume:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
+        # It can sometimes be helpful to wait for a particular plugin to be available
         ebs = nomad.get_plugin(plugin_id="aws-ebs0",
             wait_for_healthy=True)
-        mysql_volume = nomad.ExternalVolume("mysqlVolume",
+        mysql_volume = nomad.ExternalVolume("mysql_volume",
             type="csi",
             plugin_id="aws-ebs0",
             volume_id="mysql_volume",
+            name="mysql_volume",
             capacity_min="10GiB",
             capacity_max="20GiB",
             capabilities=[nomad.ExternalVolumeCapabilityArgs(
                 access_mode="single-node-writer",
                 attachment_mode="file-system",
             )],
             mount_options=nomad.ExternalVolumeMountOptionsArgs(
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_policies.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_policy.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_role.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_roles.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_token.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_acl_tokens.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_acl_tokens.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_allocations.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_allocations.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_datacenters.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_datacenters.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
-    datacenters = nomad.get_datacenters(ignore_down_nodes=True,
-        prefix="prod")
+    datacenters = nomad.get_datacenters(prefix="prod",
+        ignore_down_nodes=True)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param bool ignore_down_nodes: `(bool: false)`: An optional flag that, if set to `true` will ignore down nodes when compiling the list of datacenters.
     :param str prefix: `(string)`: An optional string to filter datacenters based on name prefix. If not provided, all datacenters are returned.
     """
@@ -119,16 +119,16 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_nomad as nomad
 
-    datacenters = nomad.get_datacenters(ignore_down_nodes=True,
-        prefix="prod")
+    datacenters = nomad.get_datacenters(prefix="prod",
+        ignore_down_nodes=True)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param bool ignore_down_nodes: `(bool: false)`: An optional flag that, if set to `true` will ignore down nodes when compiling the list of datacenters.
     :param str prefix: `(string)`: An optional string to filter datacenters based on name prefix. If not provided, all datacenters are returned.
     """
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_deployments.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_job.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_job_parser.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_job_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -82,26 +82,14 @@
 
 def get_job_parser(canonicalize: Optional[bool] = None,
                    hcl: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetJobParserResult:
     """
     Parse a HCL jobspec and produce the equivalent JSON encoded job.
 
-    ## Example Usage
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_nomad as nomad
-
-    my_job = nomad.get_job_parser(hcl=(lambda path: open(path).read())(f"{path['module']}/jobspec.hcl"),
-        canonicalize=False)
-    ```
-    <!--End PulumiCodeChooser -->
-
 
     :param bool canonicalize: `(boolean: true)` - flag to enable setting any unset fields to their default values.
     :param str hcl: `(string)` - the HCL definition of the job.
     """
     __args__ = dict()
     __args__['canonicalize'] = canonicalize
     __args__['hcl'] = hcl
@@ -118,24 +106,12 @@
 @_utilities.lift_output_func(get_job_parser)
 def get_job_parser_output(canonicalize: Optional[pulumi.Input[Optional[bool]]] = None,
                           hcl: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetJobParserResult]:
     """
     Parse a HCL jobspec and produce the equivalent JSON encoded job.
 
-    ## Example Usage
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_nomad as nomad
-
-    my_job = nomad.get_job_parser(hcl=(lambda path: open(path).read())(f"{path['module']}/jobspec.hcl"),
-        canonicalize=False)
-    ```
-    <!--End PulumiCodeChooser -->
-
 
     :param bool canonicalize: `(boolean: true)` - flag to enable setting any unset fields to their default values.
     :param str hcl: `(string)` - the HCL definition of the job.
     """
     ...
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_namespace.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_namespaces.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_namespaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     import pulumi
     import pulumi_nomad as nomad
 
     namespaces = nomad.get_namespaces()
     namespace = []
     for range in [{"value": i} for i in range(0, len(namespaces.namespaces))]:
         namespace.append(nomad.AclPolicy(f"namespace-{range['value']}",
+            name=f"namespace-{namespaces[range['value']]}",
             description=f"Write to the namespace {namespaces[range['value']]}",
             rules_hcl=f\"\"\"namespace "{namespaces[range["value"]]}" {{
       policy = "write"
     }}
     \"\"\"))
     ```
     <!--End PulumiCodeChooser -->
@@ -100,14 +101,15 @@
     import pulumi
     import pulumi_nomad as nomad
 
     namespaces = nomad.get_namespaces()
     namespace = []
     for range in [{"value": i} for i in range(0, len(namespaces.namespaces))]:
         namespace.append(nomad.AclPolicy(f"namespace-{range['value']}",
+            name=f"namespace-{namespaces[range['value']]}",
             description=f"Write to the namespace {namespaces[range['value']]}",
             rules_hcl=f\"\"\"namespace "{namespaces[range["value"]]}" {{
       policy = "write"
     }}
     \"\"\"))
     ```
     <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_node_pool.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_node_pools.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_node_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_plugin.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_plugins.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_plugins.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_scaling_policies.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scaling_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_scaling_policy.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scaling_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_scheduler_policy.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_scheduler_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_variable.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/get_volumes.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/get_volumes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/job.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/namespace.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,40 +251,43 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dev = nomad.Namespace("dev",
+            name="dev",
             description="Shared development environment.",
+            quota="dev",
             meta={
-                "foo": "bar",
                 "owner": "John Doe",
-            },
-            quota="dev")
+                "foo": "bar",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         Registering a namespace with a quota:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
-        web_team = nomad.QuoteSpecification("webTeam",
+        web_team = nomad.QuoteSpecification("web_team",
+            name="web-team",
             description="web team quota",
             limits=[nomad.QuoteSpecificationLimitArgs(
                 region="global",
                 region_limit=nomad.QuoteSpecificationLimitRegionLimitArgs(
                     cpu=1000,
                     memory_mb=256,
                 ),
             )])
         web = nomad.Namespace("web",
+            name="web",
             description="Web team production environment.",
             quota=web_team.name)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -316,40 +319,43 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dev = nomad.Namespace("dev",
+            name="dev",
             description="Shared development environment.",
+            quota="dev",
             meta={
-                "foo": "bar",
                 "owner": "John Doe",
-            },
-            quota="dev")
+                "foo": "bar",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         Registering a namespace with a quota:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
-        web_team = nomad.QuoteSpecification("webTeam",
+        web_team = nomad.QuoteSpecification("web_team",
+            name="web-team",
             description="web team quota",
             limits=[nomad.QuoteSpecificationLimitArgs(
                 region="global",
                 region_limit=nomad.QuoteSpecificationLimitRegionLimitArgs(
                     cpu=1000,
                     memory_mb=256,
                 ),
             )])
         web = nomad.Namespace("web",
+            name="web",
             description="Web team production environment.",
             quota=web_team.name)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param NamespaceArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/node_pool.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/node_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dev = nomad.NodePool("dev",
+            name="dev",
             description="Nodes for the development environment.",
             meta={
                 "department": "Engineering",
                 "env": "dev",
             })
         ```
         <!--End PulumiCodeChooser -->
@@ -215,14 +216,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         dev = nomad.NodePool("dev",
+            name="dev",
             description="Nodes for the development environment.",
             meta={
                 "department": "Engineering",
                 "env": "dev",
             })
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/outputs.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/provider.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/quote_specification.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/quote_specification.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,16 @@
         Registering a quota specification:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
-        prod_api = nomad.QuoteSpecification("prodApi",
+        prod_api = nomad.QuoteSpecification("prod_api",
+            name="prod-api",
             description="Production instances of backend API servers",
             limits=[nomad.QuoteSpecificationLimitArgs(
                 region="global",
                 region_limit=nomad.QuoteSpecificationLimitRegionLimitArgs(
                     cpu=2400,
                     memory_mb=1200,
                 ),
@@ -182,15 +183,16 @@
         Registering a quota specification:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
-        prod_api = nomad.QuoteSpecification("prodApi",
+        prod_api = nomad.QuoteSpecification("prod_api",
+            name="prod-api",
             description="Production instances of backend API servers",
             limits=[nomad.QuoteSpecificationLimitArgs(
                 region="global",
                 region_limit=nomad.QuoteSpecificationLimitRegionLimitArgs(
                     cpu=2400,
                     memory_mb=1200,
                 ),
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/scheduler_config.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/scheduler_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,22 +146,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         config = nomad.SchedulerConfig("config",
+            scheduler_algorithm="spread",
             memory_oversubscription_enabled=True,
             preemption_config={
+                "system_scheduler_enabled": True,
                 "batch_scheduler_enabled": True,
                 "service_scheduler_enabled": True,
                 "sysbatch_scheduler_enabled": True,
-                "system_scheduler_enabled": True,
-            },
-            scheduler_algorithm="spread")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] memory_oversubscription_enabled: `(bool: false)` - When `true`, tasks may exceed their reserved memory limit.
         :param pulumi.Input[Mapping[str, pulumi.Input[bool]]] preemption_config: `(map[string]bool)` - Options to enable preemption for various schedulers.
@@ -187,22 +187,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         config = nomad.SchedulerConfig("config",
+            scheduler_algorithm="spread",
             memory_oversubscription_enabled=True,
             preemption_config={
+                "system_scheduler_enabled": True,
                 "batch_scheduler_enabled": True,
                 "service_scheduler_enabled": True,
                 "sysbatch_scheduler_enabled": True,
-                "system_scheduler_enabled": True,
-            },
-            scheduler_algorithm="spread")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SchedulerConfigArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/sentinel_policy.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/sentinel_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,29 +221,29 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         exec_only = nomad.SentinelPolicy("exec-only",
+            name="exec-only",
             description="Only allow jobs that are based on an exec driver.",
-            enforcement_level="soft-mandatory",
             policy=\"\"\"main = rule { all_drivers_exec }
 
         # all_drivers_exec checks that all the drivers in use are exec
         all_drivers_exec = rule {
             all job.task_groups as tg {
                 all tg.tasks as task {
                     task.driver is "exec"
                 }
             }
         }
-
         \"\"\",
-            scope="submit-job")
+            scope="submit-job",
+            enforcement_level="soft-mandatory")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: `(string: "")` - A description of the policy.
                
@@ -271,29 +271,29 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         exec_only = nomad.SentinelPolicy("exec-only",
+            name="exec-only",
             description="Only allow jobs that are based on an exec driver.",
-            enforcement_level="soft-mandatory",
             policy=\"\"\"main = rule { all_drivers_exec }
 
         # all_drivers_exec checks that all the drivers in use are exec
         all_drivers_exec = rule {
             all job.task_groups as tg {
                 all tg.tasks as task {
                     task.driver is "exec"
                 }
             }
         }
-
         \"\"\",
-            scope="submit-job")
+            scope="submit-job",
+            enforcement_level="soft-mandatory")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SentinelPolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/variable.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,32 +137,34 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         example = nomad.Variable("example",
+            path="some/path/of/your/choosing",
             items={
                 "example_key": "example_value",
-            },
-            path="some/path/of/your/choosing")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         Creating a variable in a custom namespace:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
-        example_namespace = nomad.Namespace("exampleNamespace", description="Example namespace.")
-        example_variable = nomad.Variable("exampleVariable",
+        example = nomad.Namespace("example",
+            name="example",
+            description="Example namespace.")
+        example_variable = nomad.Variable("example",
             path="some/path/of/your/choosing",
-            namespace=example_namespace.name,
+            namespace=example.name,
             items={
                 "example_key": "example_value",
             })
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
@@ -184,32 +186,34 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
         example = nomad.Variable("example",
+            path="some/path/of/your/choosing",
             items={
                 "example_key": "example_value",
-            },
-            path="some/path/of/your/choosing")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         Creating a variable in a custom namespace:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
-        example_namespace = nomad.Namespace("exampleNamespace", description="Example namespace.")
-        example_variable = nomad.Variable("exampleVariable",
+        example = nomad.Namespace("example",
+            name="example",
+            description="Example namespace.")
+        example_variable = nomad.Variable("example",
             path="some/path/of/your/choosing",
-            namespace=example_namespace.name,
+            namespace=example.name,
             items={
                 "example_key": "example_value",
             })
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad/volume.py` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,21 +721,23 @@
         Registering a volume:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
+        # It can sometimes be helpful to wait for a particular plugin to be available
         ebs = nomad.get_plugin(plugin_id="aws-ebs0",
             wait_for_healthy=True)
-        mysql_volume = nomad.Volume("mysqlVolume",
+        mysql_volume = nomad.Volume("mysql_volume",
             type="csi",
             plugin_id="aws-ebs0",
             volume_id="mysql_volume",
-            external_id=module["hashistack"]["ebs_test_volume_id"],
+            name="mysql_volume",
+            external_id=hashistack["ebsTestVolumeId"],
             capabilities=[nomad.VolumeCapabilityArgs(
                 access_mode="single-node-writer",
                 attachment_mode="file-system",
             )],
             mount_options=nomad.VolumeMountOptionsArgs(
                 fs_type="ext4",
             ),
@@ -795,21 +797,23 @@
         Registering a volume:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_nomad as nomad
 
+        # It can sometimes be helpful to wait for a particular plugin to be available
         ebs = nomad.get_plugin(plugin_id="aws-ebs0",
             wait_for_healthy=True)
-        mysql_volume = nomad.Volume("mysqlVolume",
+        mysql_volume = nomad.Volume("mysql_volume",
             type="csi",
             plugin_id="aws-ebs0",
             volume_id="mysql_volume",
-            external_id=module["hashistack"]["ebs_test_volume_id"],
+            name="mysql_volume",
+            external_id=hashistack["ebsTestVolumeId"],
             capabilities=[nomad.VolumeCapabilityArgs(
                 access_mode="single-node-writer",
                 attachment_mode="file-system",
             )],
             mount_options=nomad.VolumeMountOptionsArgs(
                 fs_type="ext4",
             ),
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad.egg-info/PKG-INFO` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_nomad
-Version: 2.3.0a1713333813
+Version: 2.3.0a1713561631
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi,nomad
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_nomad-2.3.0a1713333813/pulumi_nomad.egg-info/SOURCES.txt` & `pulumi_nomad-2.3.0a1713561631/pulumi_nomad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-2.3.0a1713333813/pyproject.toml` & `pulumi_nomad-2.3.0a1713561631/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_nomad"
   description = "A Pulumi package for creating and managing nomad cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "nomad"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.3.0a1713333813"
+  version = "2.3.0a1713561631"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-nomad"
 
 [build-system]
```

