# Comparing `tmp/pulumi_azuredevops-3.1.0a1713331204.tar.gz` & `tmp/pulumi_azuredevops-3.1.0a1713526847.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_azuredevops-3.1.0a1713331204.tar", last modified: Wed Apr 17 05:23:55 2024, max compression
+gzip compressed data, was "pulumi_azuredevops-3.1.0a1713526847.tar", last modified: Fri Apr 19 11:43:23 2024, max compression
```

## Comparing `pulumi_azuredevops-3.1.0a1713331204.tar` & `pulumi_azuredevops-3.1.0a1713526847.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:23:55.331519 pulumi_azuredevops-3.1.0a1713331204/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-17 05:23:55.331519 pulumi_azuredevops-3.1.0a1713331204/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:23:55.327519 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/
--rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   159174 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/area_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_auto_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18443 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_build_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_comment_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_merge_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_min_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17427 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_status_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    16941 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_work_item_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)    43565 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/build_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    29769 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/build_definition_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/build_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    30632 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/build_folder_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25884 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/check_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)    36499 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/check_branch_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    56723 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/check_business_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)    18894 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/check_exclusive_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/check_required_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:23:55.327519 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    34928 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/elastic_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/environment_resource_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_agent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_build_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_git_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_service_endpoint_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_serviceendpoint_azurecr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_serviceendpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_variable_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    42778 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/git_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/git_repository_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/git_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    29903 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/group_entitlement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    20785 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/iterative_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/library_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)   201840 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/pipeline_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    23748 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/project_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/project_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26547 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/project_pipeline_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    21960 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_author_email_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20904 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_case_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (127)    18085 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_check_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_file_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_max_file_size.py
--rw-r--r--   0 runner    (1001) docker     (127)    20181 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_max_path_length.py
--rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_reserved_names.py
--rw-r--r--   0 runner    (1001) docker     (127)    17417 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/resource_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    24222 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    27945 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    21045 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    30889 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_azure_ecr.py
--rw-r--r--   0 runner    (1001) docker     (127)    59232 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17330 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_bit_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    26408 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    20461 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    23957 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_generic_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_git_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    17902 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)    25409 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18291 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20052 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_service_fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_sonar_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_sonar_qube.py
--rw-r--r--   0 runner    (1001) docker     (127)    23003 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    25768 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_argocd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_externaltfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24637 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_gcp_terraform.py
--rw-r--r--   0 runner    (1001) docker     (127)    21103 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    23039 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_jenkins.py
--rw-r--r--   0 runner    (1001) docker     (127)    26010 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26086 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25758 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25472 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26764 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_maven.py
--rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    25867 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_nuget.py
--rw-r--r--   0 runner    (1001) docker     (127)    20117 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23357 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18015 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/servicehook_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30631 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/servicehook_storage_queue_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)    18578 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/tagging_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21904 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    18618 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/team_administrators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17671 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/team_members.py
--rw-r--r--   0 runner    (1001) docker     (127)    21781 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    24576 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/variable_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22441 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/variable_group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26033 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/work_item_query_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/workitem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:23:55.331519 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-17 05:23:55.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-17 05:23:55.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:23:55.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 05:23:55.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 05:23:55.000000 pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-17 05:23:47.000000 pulumi_azuredevops-3.1.0a1713331204/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:23:55.331519 pulumi_azuredevops-3.1.0a1713331204/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:43:23.383607 pulumi_azuredevops-3.1.0a1713526847/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-19 11:43:23.383607 pulumi_azuredevops-3.1.0a1713526847/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:43:23.379607 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/
+-rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   159174 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/area_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_auto_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18491 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_build_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_comment_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17011 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_merge_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_min_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17455 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_status_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_work_item_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43767 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29827 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_definition_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11051 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30526 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_folder_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25916 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36417 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_branch_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56641 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_business_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18832 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_exclusive_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21704 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_required_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:43:23.383607 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34954 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/elastic_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22334 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/environment_resource_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_agent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_git_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_service_endpoint_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_azurecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43100 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18769 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_repository_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29863 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group_entitlement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16280 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/iterative_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/library_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   201840 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22167 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/pipeline_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23820 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32578 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26527 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_pipeline_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31976 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15414 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21932 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_author_email_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_case_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18065 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_check_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22051 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_file_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_max_file_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_max_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17963 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_reserved_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/resource_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27935 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21019 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_ecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63452 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17308 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_bit_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26360 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23933 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_generic_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21318 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_git_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32619 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20032 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_service_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16955 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_sonar_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18689 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_sonar_qube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_argocd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_externaltfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24609 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_gcp_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21069 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23021 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25930 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26002 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25690 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25420 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26736 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_maven.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25853 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_nuget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20087 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23277 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18087 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/servicehook_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30769 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/servicehook_storage_queue_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/tagging_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21956 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18780 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17833 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21781 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24688 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22547 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/variable_group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26249 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/work_item_query_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25809 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/workitem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:43:23.383607 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-19 11:43:23.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-19 11:43:23.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:43:23.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 11:43:23.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-19 11:43:23.000000 pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-19 11:43:16.000000 pulumi_azuredevops-3.1.0a1713526847/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:43:23.383607 pulumi_azuredevops-3.1.0a1713526847/setup.cfg
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/PKG-INFO` & `pulumi_azuredevops-3.1.0a1713526847/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 3.1.0a1713331204
+Version: 3.1.0a1713526847
 Summary: A Pulumi package for creating and managing Azure DevOps.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi,azuredevops
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/README.md` & `pulumi_azuredevops-3.1.0a1713526847/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/__init__.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/_inputs.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/_utilities.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/area_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/area_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_project_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_root_permissions = azuredevops.AreaPermissions("example-root-permissions",
@@ -332,14 +333,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_project_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_root_permissions = azuredevops.AreaPermissions("example-root-permissions",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_auto_reviewers.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_auto_reviewers.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,25 +171,26 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_user = azuredevops.User("exampleUser",
+        example_user = azuredevops.User("example",
             principal_name="mail@email.com",
             account_license_type="basic")
-        example_branch_policy_auto_reviewers = azuredevops.BranchPolicyAutoReviewers("exampleBranchPolicyAutoReviewers",
-            project_id=example_project.id,
+        example_branch_policy_auto_reviewers = azuredevops.BranchPolicyAutoReviewers("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyAutoReviewersSettingsArgs(
                 auto_reviewer_ids=[example_user.id],
                 submitter_can_vote=False,
                 message="Auto reviewer",
                 path_filters=["*/src/*.ts"],
@@ -233,25 +234,26 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_user = azuredevops.User("exampleUser",
+        example_user = azuredevops.User("example",
             principal_name="mail@email.com",
             account_license_type="basic")
-        example_branch_policy_auto_reviewers = azuredevops.BranchPolicyAutoReviewers("exampleBranchPolicyAutoReviewers",
-            project_id=example_project.id,
+        example_branch_policy_auto_reviewers = azuredevops.BranchPolicyAutoReviewers("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyAutoReviewersSettingsArgs(
                 auto_reviewer_ids=[example_user.id],
                 submitter_can_vote=False,
                 message="Auto reviewer",
                 path_filters=["*/src/*.ts"],
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_build_validation.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_build_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,29 +171,31 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_build_definition = azuredevops.BuildDefinition("exampleBuildDefinition",
-            project_id=example_project.id,
+        example_build_definition = azuredevops.BuildDefinition("example",
+            project_id=example.id,
+            name="Example Build Definition",
             repository=azuredevops.BuildDefinitionRepositoryArgs(
                 repo_type="TfsGit",
                 repo_id=example_git.id,
                 yml_path="azure-pipelines.yml",
             ))
-        example_branch_policy_build_validation = azuredevops.BranchPolicyBuildValidation("exampleBranchPolicyBuildValidation",
-            project_id=example_project.id,
+        example_branch_policy_build_validation = azuredevops.BranchPolicyBuildValidation("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyBuildValidationSettingsArgs(
                 display_name="Example build validation policy",
                 build_definition_id=example_build_definition.id,
                 valid_duration=720,
                 filename_patterns=[
@@ -251,29 +253,31 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_build_definition = azuredevops.BuildDefinition("exampleBuildDefinition",
-            project_id=example_project.id,
+        example_build_definition = azuredevops.BuildDefinition("example",
+            project_id=example.id,
+            name="Example Build Definition",
             repository=azuredevops.BuildDefinitionRepositoryArgs(
                 repo_type="TfsGit",
                 repo_id=example_git.id,
                 yml_path="azure-pipelines.yml",
             ))
-        example_branch_policy_build_validation = azuredevops.BranchPolicyBuildValidation("exampleBranchPolicyBuildValidation",
-            project_id=example_project.id,
+        example_branch_policy_build_validation = azuredevops.BranchPolicyBuildValidation("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyBuildValidationSettingsArgs(
                 display_name="Example build validation policy",
                 build_definition_id=example_build_definition.id,
                 valid_duration=720,
                 filename_patterns=[
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_comment_resolution.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_comment_resolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,22 +171,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_branch_policy_comment_resolution = azuredevops.BranchPolicyCommentResolution("exampleBranchPolicyCommentResolution",
-            project_id=example_project.id,
+        example_branch_policy_comment_resolution = azuredevops.BranchPolicyCommentResolution("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyCommentResolutionSettingsArgs(
                 scopes=[
                     azuredevops.BranchPolicyCommentResolutionSettingsScopeArgs(
                         repository_id=example_git.id,
                         repository_ref=example_git.default_branch,
@@ -236,22 +237,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_branch_policy_comment_resolution = azuredevops.BranchPolicyCommentResolution("exampleBranchPolicyCommentResolution",
-            project_id=example_project.id,
+        example_branch_policy_comment_resolution = azuredevops.BranchPolicyCommentResolution("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyCommentResolutionSettingsArgs(
                 scopes=[
                     azuredevops.BranchPolicyCommentResolutionSettingsScopeArgs(
                         repository_id=example_git.id,
                         repository_ref=example_git.default_branch,
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_merge_types.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_merge_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,22 +171,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_branch_policy_merge_types = azuredevops.BranchPolicyMergeTypes("exampleBranchPolicyMergeTypes",
-            project_id=example_project.id,
+        example_branch_policy_merge_types = azuredevops.BranchPolicyMergeTypes("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyMergeTypesSettingsArgs(
                 allow_squash=True,
                 allow_rebase_and_fast_forward=True,
                 allow_basic_no_fast_forward=True,
                 allow_rebase_with_merge=True,
@@ -240,22 +241,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_branch_policy_merge_types = azuredevops.BranchPolicyMergeTypes("exampleBranchPolicyMergeTypes",
-            project_id=example_project.id,
+        example_branch_policy_merge_types = azuredevops.BranchPolicyMergeTypes("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyMergeTypesSettingsArgs(
                 allow_squash=True,
                 allow_rebase_and_fast_forward=True,
                 allow_basic_no_fast_forward=True,
                 allow_rebase_with_merge=True,
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_min_reviewers.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_min_reviewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,22 +171,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_branch_policy_min_reviewers = azuredevops.BranchPolicyMinReviewers("exampleBranchPolicyMinReviewers",
-            project_id=example_project.id,
+        example_branch_policy_min_reviewers = azuredevops.BranchPolicyMinReviewers("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyMinReviewersSettingsArgs(
                 reviewer_count=7,
                 submitter_can_vote=False,
                 last_pusher_cannot_approve=True,
                 allow_completion_with_rejects_or_waits=False,
@@ -242,22 +243,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_branch_policy_min_reviewers = azuredevops.BranchPolicyMinReviewers("exampleBranchPolicyMinReviewers",
-            project_id=example_project.id,
+        example_branch_policy_min_reviewers = azuredevops.BranchPolicyMinReviewers("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyMinReviewersSettingsArgs(
                 reviewer_count=7,
                 submitter_can_vote=False,
                 last_pusher_cannot_approve=True,
                 allow_completion_with_rejects_or_waits=False,
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_status_check.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_status_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,33 +171,35 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             features={
                 "testplans": "disabled",
                 "artifacts": "disabled",
             },
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_user = azuredevops.User("exampleUser",
+        example_user = azuredevops.User("example",
             principal_name="mail@email.com",
             account_license_type="basic")
-        example_branch_policy_status_check = azuredevops.BranchPolicyStatusCheck("exampleBranchPolicyStatusCheck",
-            project_id=example_project.id,
+        example_branch_policy_status_check = azuredevops.BranchPolicyStatusCheck("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyStatusCheckSettingsArgs(
                 name="Release",
                 author_id=example_user.id,
                 invalidate_on_update=True,
                 applicability="conditional",
@@ -247,33 +249,35 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             features={
                 "testplans": "disabled",
                 "artifacts": "disabled",
             },
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_user = azuredevops.User("exampleUser",
+        example_user = azuredevops.User("example",
             principal_name="mail@email.com",
             account_license_type="basic")
-        example_branch_policy_status_check = azuredevops.BranchPolicyStatusCheck("exampleBranchPolicyStatusCheck",
-            project_id=example_project.id,
+        example_branch_policy_status_check = azuredevops.BranchPolicyStatusCheck("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyStatusCheckSettingsArgs(
                 name="Release",
                 author_id=example_user.id,
                 invalidate_on_update=True,
                 applicability="conditional",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/branch_policy_work_item_linking.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/branch_policy_work_item_linking.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,22 +171,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_branch_policy_work_item_linking = azuredevops.BranchPolicyWorkItemLinking("exampleBranchPolicyWorkItemLinking",
-            project_id=example_project.id,
+        example_branch_policy_work_item_linking = azuredevops.BranchPolicyWorkItemLinking("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyWorkItemLinkingSettingsArgs(
                 scopes=[
                     azuredevops.BranchPolicyWorkItemLinkingSettingsScopeArgs(
                         repository_id=example_git.id,
                         repository_ref=example_git.default_branch,
@@ -236,22 +237,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_branch_policy_work_item_linking = azuredevops.BranchPolicyWorkItemLinking("exampleBranchPolicyWorkItemLinking",
-            project_id=example_project.id,
+        example_branch_policy_work_item_linking = azuredevops.BranchPolicyWorkItemLinking("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             settings=azuredevops.BranchPolicyWorkItemLinkingSettingsArgs(
                 scopes=[
                     azuredevops.BranchPolicyWorkItemLinkingSettingsScopeArgs(
                         repository_id=example_git.id,
                         repository_ref=example_git.default_branch,
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/build_definition.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -444,33 +444,37 @@
 
         ### Tfs
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_variable_group = azuredevops.VariableGroup("exampleVariableGroup",
-            project_id=example_project.id,
+        example_variable_group = azuredevops.VariableGroup("example",
+            project_id=example.id,
+            name="Example Pipeline Variables",
             description="Managed by Terraform",
             allow_access=True,
             variables=[azuredevops.VariableGroupVariableArgs(
                 name="FOO",
                 value="BAR",
             )])
-        example_build_definition = azuredevops.BuildDefinition("exampleBuildDefinition",
-            project_id=example_project.id,
+        example_build_definition = azuredevops.BuildDefinition("example",
+            project_id=example.id,
+            name="Example Build Definition",
             path="\\\\ExampleFolder",
             ci_trigger=azuredevops.BuildDefinitionCiTriggerArgs(
                 use_yaml=False,
             ),
             schedules=[azuredevops.BuildDefinitionScheduleArgs(
                 branch_filters=[azuredevops.BuildDefinitionScheduleBranchFilterArgs(
                     includes=["master"],
@@ -511,28 +515,30 @@
 
         ### GitHub Enterprise
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_service_endpoint_git_hub_enterprise = azuredevops.ServiceEndpointGitHubEnterprise("exampleServiceEndpointGitHubEnterprise",
-            project_id=example_project.id,
+        example_service_endpoint_git_hub_enterprise = azuredevops.ServiceEndpointGitHubEnterprise("example",
+            project_id=example.id,
             service_endpoint_name="Example GitHub Enterprise",
             url="https://github.contoso.com",
             description="Managed by Terraform",
             auth_personal=azuredevops.ServiceEndpointGitHubEnterpriseAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ))
-        example_build_definition = azuredevops.BuildDefinition("exampleBuildDefinition",
-            project_id=example_project.id,
+        example_build_definition = azuredevops.BuildDefinition("example",
+            project_id=example.id,
+            name="Example Build Definition",
             path="\\\\ExampleFolder",
             ci_trigger=azuredevops.BuildDefinitionCiTriggerArgs(
                 use_yaml=False,
             ),
             repository=azuredevops.BuildDefinitionRepositoryArgs(
                 repo_type="GitHubEnterprise",
                 repo_id="<GitHub Org>/<Repo Name>",
@@ -617,33 +623,37 @@
 
         ### Tfs
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_variable_group = azuredevops.VariableGroup("exampleVariableGroup",
-            project_id=example_project.id,
+        example_variable_group = azuredevops.VariableGroup("example",
+            project_id=example.id,
+            name="Example Pipeline Variables",
             description="Managed by Terraform",
             allow_access=True,
             variables=[azuredevops.VariableGroupVariableArgs(
                 name="FOO",
                 value="BAR",
             )])
-        example_build_definition = azuredevops.BuildDefinition("exampleBuildDefinition",
-            project_id=example_project.id,
+        example_build_definition = azuredevops.BuildDefinition("example",
+            project_id=example.id,
+            name="Example Build Definition",
             path="\\\\ExampleFolder",
             ci_trigger=azuredevops.BuildDefinitionCiTriggerArgs(
                 use_yaml=False,
             ),
             schedules=[azuredevops.BuildDefinitionScheduleArgs(
                 branch_filters=[azuredevops.BuildDefinitionScheduleBranchFilterArgs(
                     includes=["master"],
@@ -684,28 +694,30 @@
 
         ### GitHub Enterprise
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_service_endpoint_git_hub_enterprise = azuredevops.ServiceEndpointGitHubEnterprise("exampleServiceEndpointGitHubEnterprise",
-            project_id=example_project.id,
+        example_service_endpoint_git_hub_enterprise = azuredevops.ServiceEndpointGitHubEnterprise("example",
+            project_id=example.id,
             service_endpoint_name="Example GitHub Enterprise",
             url="https://github.contoso.com",
             description="Managed by Terraform",
             auth_personal=azuredevops.ServiceEndpointGitHubEnterpriseAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ))
-        example_build_definition = azuredevops.BuildDefinition("exampleBuildDefinition",
-            project_id=example_project.id,
+        example_build_definition = azuredevops.BuildDefinition("example",
+            project_id=example.id,
+            name="Example Build Definition",
             path="\\\\ExampleFolder",
             ci_trigger=azuredevops.BuildDefinitionCiTriggerArgs(
                 use_yaml=False,
             ),
             repository=azuredevops.BuildDefinitionRepositoryArgs(
                 repo_type="GitHubEnterprise",
                 repo_id="<GitHub Org>/<Repo Name>",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/build_definition_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_definition_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,40 +274,43 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_build_definition = azuredevops.BuildDefinition("exampleBuildDefinition",
-            project_id=example_project.id,
+        example_build_definition = azuredevops.BuildDefinition("example",
+            project_id=example.id,
+            name="Example Build Definition",
             path="\\\\ExampleFolder",
             ci_trigger=azuredevops.BuildDefinitionCiTriggerArgs(
                 use_yaml=True,
             ),
             repository=azuredevops.BuildDefinitionRepositoryArgs(
                 repo_type="TfsGit",
                 repo_id=example_git.id,
                 branch_name=example_git.default_branch,
                 yml_path="azure-pipelines.yml",
             ))
-        example_build_definition_permissions = azuredevops.BuildDefinitionPermissions("exampleBuildDefinitionPermissions",
-            project_id=example_project.id,
+        example_build_definition_permissions = azuredevops.BuildDefinitionPermissions("example",
+            project_id=example.id,
             principal=example_readers.id,
             build_definition_id=example_build_definition.id,
             permissions={
                 "ViewBuilds": "Allow",
                 "EditBuildQuality": "Deny",
                 "DeleteBuilds": "Deny",
                 "StopBuilds": "Allow",
@@ -367,40 +370,43 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_build_definition = azuredevops.BuildDefinition("exampleBuildDefinition",
-            project_id=example_project.id,
+        example_build_definition = azuredevops.BuildDefinition("example",
+            project_id=example.id,
+            name="Example Build Definition",
             path="\\\\ExampleFolder",
             ci_trigger=azuredevops.BuildDefinitionCiTriggerArgs(
                 use_yaml=True,
             ),
             repository=azuredevops.BuildDefinitionRepositoryArgs(
                 repo_type="TfsGit",
                 repo_id=example_git.id,
                 branch_name=example_git.default_branch,
                 yml_path="azure-pipelines.yml",
             ))
-        example_build_definition_permissions = azuredevops.BuildDefinitionPermissions("exampleBuildDefinitionPermissions",
-            project_id=example_project.id,
+        example_build_definition_permissions = azuredevops.BuildDefinitionPermissions("example",
+            project_id=example.id,
             principal=example_readers.id,
             build_definition_id=example_build_definition.id,
             permissions={
                 "ViewBuilds": "Allow",
                 "EditBuildQuality": "Deny",
                 "DeleteBuilds": "Deny",
                 "StopBuilds": "Allow",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/build_folder.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_folder.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,20 +136,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_build_folder = azuredevops.BuildFolder("exampleBuildFolder",
-            project_id=example_project.id,
+        example_build_folder = azuredevops.BuildFolder("example",
+            project_id=example.id,
             path="\\\\ExampleFolder",
             description="ExampleFolder description")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -183,20 +184,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_build_folder = azuredevops.BuildFolder("exampleBuildFolder",
-            project_id=example_project.id,
+        example_build_folder = azuredevops.BuildFolder("example",
+            project_id=example.id,
             path="\\\\ExampleFolder",
             description="ExampleFolder description")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/build_folder_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/build_folder_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,27 +276,28 @@
         ### Set specific folder permissions
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_build_folder = azuredevops.BuildFolder("exampleBuildFolder",
-            project_id=example_project.id,
+        example_build_folder = azuredevops.BuildFolder("example",
+            project_id=example.id,
             path="\\\\ExampleFolder",
             description="ExampleFolder description")
-        example_build_folder_permissions = azuredevops.BuildFolderPermissions("exampleBuildFolderPermissions",
-            project_id=example_project.id,
+        example_build_folder_permissions = azuredevops.BuildFolderPermissions("example",
+            project_id=example.id,
             path="\\\\ExampleFolder",
             principal=example_readers.id,
             permissions={
                 "ViewBuilds": "Allow",
                 "EditBuildQuality": "Allow",
                 "RetainIndefinitely": "Allow",
                 "DeleteBuilds": "Deny",
@@ -315,23 +316,24 @@
         <!--End PulumiCodeChooser -->
         ### Set root folder permissions
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_build_folder_permissions = azuredevops.BuildFolderPermissions("exampleBuildFolderPermissions",
-            project_id=example_project.id,
+        example_build_folder_permissions = azuredevops.BuildFolderPermissions("example",
+            project_id=example.id,
             path="\\\\",
             principal=example_readers.id,
             permissions={
                 "RetainIndefinitely": "Allow",
             })
         ```
         <!--End PulumiCodeChooser -->
@@ -390,27 +392,28 @@
         ### Set specific folder permissions
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_build_folder = azuredevops.BuildFolder("exampleBuildFolder",
-            project_id=example_project.id,
+        example_build_folder = azuredevops.BuildFolder("example",
+            project_id=example.id,
             path="\\\\ExampleFolder",
             description="ExampleFolder description")
-        example_build_folder_permissions = azuredevops.BuildFolderPermissions("exampleBuildFolderPermissions",
-            project_id=example_project.id,
+        example_build_folder_permissions = azuredevops.BuildFolderPermissions("example",
+            project_id=example.id,
             path="\\\\ExampleFolder",
             principal=example_readers.id,
             permissions={
                 "ViewBuilds": "Allow",
                 "EditBuildQuality": "Allow",
                 "RetainIndefinitely": "Allow",
                 "DeleteBuilds": "Deny",
@@ -429,23 +432,24 @@
         <!--End PulumiCodeChooser -->
         ### Set root folder permissions
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_build_folder_permissions = azuredevops.BuildFolderPermissions("exampleBuildFolderPermissions",
-            project_id=example_project.id,
+        example_build_folder_permissions = azuredevops.BuildFolderPermissions("example",
+            project_id=example.id,
             path="\\\\",
             principal=example_readers.id,
             permissions={
                 "RetainIndefinitely": "Allow",
             })
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/check_approval.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_approval.py`

 * *Files 5% similar despite different names*

```diff
@@ -317,19 +317,21 @@
         ### Protect an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_group = azuredevops.Group("exampleGroup", display_name="some-azdo-group")
-        example_check_approval = azuredevops.CheckApproval("exampleCheckApproval",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_group = azuredevops.Group("example", display_name="some-azdo-group")
+        example_check_approval = azuredevops.CheckApproval("example",
+            project_id=example.id,
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             requester_can_approve=True,
             approvers=[example_group.origin_id])
         ```
         <!--End PulumiCodeChooser -->
 
@@ -362,19 +364,21 @@
         ### Protect an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_group = azuredevops.Group("exampleGroup", display_name="some-azdo-group")
-        example_check_approval = azuredevops.CheckApproval("exampleCheckApproval",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_group = azuredevops.Group("example", display_name="some-azdo-group")
+        example_check_approval = azuredevops.CheckApproval("example",
+            project_id=example.id,
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             requester_can_approve=True,
             approvers=[example_group.origin_id])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/check_branch_control.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_branch_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -318,24 +318,24 @@
         ### Protect a service connection
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("exampleServiceEndpointGeneric",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
+            project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
-        example_check_branch_control = azuredevops.CheckBranchControl("exampleCheckBranchControl",
-            project_id=example_project.id,
+        example_check_branch_control = azuredevops.CheckBranchControl("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             allowed_branches="refs/heads/main, refs/heads/features/*",
             timeout=1440)
         ```
         <!--End PulumiCodeChooser -->
@@ -343,93 +343,97 @@
         ### Protect an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_check_branch_control = azuredevops.CheckBranchControl("exampleCheckBranchControl",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_check_branch_control = azuredevops.CheckBranchControl("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Protect an agent queue
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_pool = azuredevops.Pool("examplePool")
-        example_queue = azuredevops.Queue("exampleQueue",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_pool = azuredevops.Pool("example", name="example-pool")
+        example_queue = azuredevops.Queue("example",
+            project_id=example.id,
             agent_pool_id=example_pool.id)
-        example_check_branch_control = azuredevops.CheckBranchControl("exampleCheckBranchControl",
-            project_id=example_project.id,
+        example_check_branch_control = azuredevops.CheckBranchControl("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_queue.id,
             target_resource_type="queue",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Protect a repository
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Empty Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_check_branch_control = azuredevops.CheckBranchControl("exampleCheckBranchControl",
-            project_id=example_project.id,
+        example_check_branch_control = azuredevops.CheckBranchControl("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
-            target_resource_id=pulumi.Output.all(example_project.id, example_git.id).apply(lambda exampleProjectId, exampleGitId: f"{example_project_id}.{example_git_id}"),
+            target_resource_id=pulumi.Output.all(example.id, example_git.id).apply(lambda exampleId, exampleGitId: f"{example_id}.{example_git_id}"),
             target_resource_type="repository",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Protect a variable group
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_variable_group = azuredevops.VariableGroup("exampleVariableGroup",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_variable_group = azuredevops.VariableGroup("example",
+            project_id=example.id,
+            name="Example Variable Group",
             description="Example Variable Group Description",
             allow_access=True,
             variables=[
                 azuredevops.VariableGroupVariableArgs(
                     name="key1",
                     value="val1",
                 ),
                 azuredevops.VariableGroupVariableArgs(
                     name="key2",
                     secret_value="val2",
                     is_secret=True,
                 ),
             ])
-        example_check_branch_control = azuredevops.CheckBranchControl("exampleCheckBranchControl",
-            project_id=example_project.id,
+        example_check_branch_control = azuredevops.CheckBranchControl("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_variable_group.id,
             target_resource_type="variablegroup",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -466,24 +470,24 @@
         ### Protect a service connection
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("exampleServiceEndpointGeneric",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
+            project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
-        example_check_branch_control = azuredevops.CheckBranchControl("exampleCheckBranchControl",
-            project_id=example_project.id,
+        example_check_branch_control = azuredevops.CheckBranchControl("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             allowed_branches="refs/heads/main, refs/heads/features/*",
             timeout=1440)
         ```
         <!--End PulumiCodeChooser -->
@@ -491,93 +495,97 @@
         ### Protect an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_check_branch_control = azuredevops.CheckBranchControl("exampleCheckBranchControl",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_check_branch_control = azuredevops.CheckBranchControl("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Protect an agent queue
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_pool = azuredevops.Pool("examplePool")
-        example_queue = azuredevops.Queue("exampleQueue",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_pool = azuredevops.Pool("example", name="example-pool")
+        example_queue = azuredevops.Queue("example",
+            project_id=example.id,
             agent_pool_id=example_pool.id)
-        example_check_branch_control = azuredevops.CheckBranchControl("exampleCheckBranchControl",
-            project_id=example_project.id,
+        example_check_branch_control = azuredevops.CheckBranchControl("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_queue.id,
             target_resource_type="queue",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Protect a repository
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Empty Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_check_branch_control = azuredevops.CheckBranchControl("exampleCheckBranchControl",
-            project_id=example_project.id,
+        example_check_branch_control = azuredevops.CheckBranchControl("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
-            target_resource_id=pulumi.Output.all(example_project.id, example_git.id).apply(lambda exampleProjectId, exampleGitId: f"{example_project_id}.{example_git_id}"),
+            target_resource_id=pulumi.Output.all(example.id, example_git.id).apply(lambda exampleId, exampleGitId: f"{example_id}.{example_git_id}"),
             target_resource_type="repository",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Protect a variable group
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_variable_group = azuredevops.VariableGroup("exampleVariableGroup",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_variable_group = azuredevops.VariableGroup("example",
+            project_id=example.id,
+            name="Example Variable Group",
             description="Example Variable Group Description",
             allow_access=True,
             variables=[
                 azuredevops.VariableGroupVariableArgs(
                     name="key1",
                     value="val1",
                 ),
                 azuredevops.VariableGroupVariableArgs(
                     name="key2",
                     secret_value="val2",
                     is_secret=True,
                 ),
             ])
-        example_check_branch_control = azuredevops.CheckBranchControl("exampleCheckBranchControl",
-            project_id=example_project.id,
+        example_check_branch_control = azuredevops.CheckBranchControl("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_variable_group.id,
             target_resource_type="variablegroup",
             allowed_branches="refs/heads/main, refs/heads/features/*")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/check_business_hours.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_business_hours.py`

 * *Files 4% similar despite different names*

```diff
@@ -546,24 +546,24 @@
         ### Protect a service connection
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("exampleServiceEndpointGeneric",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
+            project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
-        example_check_business_hours = azuredevops.CheckBusinessHours("exampleCheckBusinessHours",
-            project_id=example_project.id,
+        example_check_business_hours = azuredevops.CheckBusinessHours("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
@@ -575,18 +575,20 @@
         ### Protect an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_check_business_hours = azuredevops.CheckBusinessHours("exampleCheckBusinessHours",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_check_business_hours = azuredevops.CheckBusinessHours("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
@@ -597,21 +599,21 @@
         ### Protect an agent queue
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_pool = azuredevops.Pool("examplePool")
-        example_queue = azuredevops.Queue("exampleQueue",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_pool = azuredevops.Pool("example", name="example-pool")
+        example_queue = azuredevops.Queue("example",
+            project_id=example.id,
             agent_pool_id=example_pool.id)
-        example_check_business_hours = azuredevops.CheckBusinessHours("exampleCheckBusinessHours",
-            project_id=example_project.id,
+        example_check_business_hours = azuredevops.CheckBusinessHours("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_queue.id,
             target_resource_type="queue",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
@@ -622,24 +624,25 @@
         ### Protect a repository
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Empty Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_check_business_hours = azuredevops.CheckBusinessHours("exampleCheckBusinessHours",
-            project_id=example_project.id,
+        example_check_business_hours = azuredevops.CheckBusinessHours("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
-            target_resource_id=pulumi.Output.all(example_project.id, example_git.id).apply(lambda exampleProjectId, exampleGitId: f"{example_project_id}.{example_git_id}"),
+            target_resource_id=pulumi.Output.all(example.id, example_git.id).apply(lambda exampleId, exampleGitId: f"{example_id}.{example_git_id}"),
             target_resource_type="repository",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True)
         ```
@@ -648,32 +651,33 @@
         ### Protect a variable group
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_variable_group = azuredevops.VariableGroup("exampleVariableGroup",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_variable_group = azuredevops.VariableGroup("example",
+            project_id=example.id,
+            name="Example Variable Group",
             description="Example Variable Group Description",
             allow_access=True,
             variables=[
                 azuredevops.VariableGroupVariableArgs(
                     name="key1",
                     value="val1",
                 ),
                 azuredevops.VariableGroupVariableArgs(
                     name="key2",
                     secret_value="val2",
                     is_secret=True,
                 ),
             ])
-        example_check_business_hours = azuredevops.CheckBusinessHours("exampleCheckBusinessHours",
-            project_id=example_project.id,
+        example_check_business_hours = azuredevops.CheckBusinessHours("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_variable_group.id,
             target_resource_type="variablegroup",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
@@ -865,24 +869,24 @@
         ### Protect a service connection
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("exampleServiceEndpointGeneric",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
+            project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
-        example_check_business_hours = azuredevops.CheckBusinessHours("exampleCheckBusinessHours",
-            project_id=example_project.id,
+        example_check_business_hours = azuredevops.CheckBusinessHours("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
@@ -894,18 +898,20 @@
         ### Protect an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_check_business_hours = azuredevops.CheckBusinessHours("exampleCheckBusinessHours",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_check_business_hours = azuredevops.CheckBusinessHours("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
@@ -916,21 +922,21 @@
         ### Protect an agent queue
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_pool = azuredevops.Pool("examplePool")
-        example_queue = azuredevops.Queue("exampleQueue",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_pool = azuredevops.Pool("example", name="example-pool")
+        example_queue = azuredevops.Queue("example",
+            project_id=example.id,
             agent_pool_id=example_pool.id)
-        example_check_business_hours = azuredevops.CheckBusinessHours("exampleCheckBusinessHours",
-            project_id=example_project.id,
+        example_check_business_hours = azuredevops.CheckBusinessHours("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_queue.id,
             target_resource_type="queue",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
@@ -941,24 +947,25 @@
         ### Protect a repository
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Empty Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_check_business_hours = azuredevops.CheckBusinessHours("exampleCheckBusinessHours",
-            project_id=example_project.id,
+        example_check_business_hours = azuredevops.CheckBusinessHours("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
-            target_resource_id=pulumi.Output.all(example_project.id, example_git.id).apply(lambda exampleProjectId, exampleGitId: f"{example_project_id}.{example_git_id}"),
+            target_resource_id=pulumi.Output.all(example.id, example_git.id).apply(lambda exampleId, exampleGitId: f"{example_id}.{example_git_id}"),
             target_resource_type="repository",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
             tuesday=True)
         ```
@@ -967,32 +974,33 @@
         ### Protect a variable group
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_variable_group = azuredevops.VariableGroup("exampleVariableGroup",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_variable_group = azuredevops.VariableGroup("example",
+            project_id=example.id,
+            name="Example Variable Group",
             description="Example Variable Group Description",
             allow_access=True,
             variables=[
                 azuredevops.VariableGroupVariableArgs(
                     name="key1",
                     value="val1",
                 ),
                 azuredevops.VariableGroupVariableArgs(
                     name="key2",
                     secret_value="val2",
                     is_secret=True,
                 ),
             ])
-        example_check_business_hours = azuredevops.CheckBusinessHours("exampleCheckBusinessHours",
-            project_id=example_project.id,
+        example_check_business_hours = azuredevops.CheckBusinessHours("example",
+            project_id=example.id,
             display_name="Managed by Terraform",
             target_resource_id=example_variable_group.id,
             target_resource_type="variablegroup",
             start_time="07:00",
             end_time="15:30",
             time_zone="UTC",
             monday=True,
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/check_exclusive_lock.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_exclusive_lock.py`

 * *Files 6% similar despite different names*

```diff
@@ -188,41 +188,43 @@
         ### Add Exclusive Lock to an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("exampleServiceEndpointGeneric",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
+            project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
-        example_check_exclusive_lock = azuredevops.CheckExclusiveLock("exampleCheckExclusiveLock",
-            project_id=example_project.id,
+        example_check_exclusive_lock = azuredevops.CheckExclusiveLock("example",
+            project_id=example.id,
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             timeout=43200)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Protect an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_check_exclusive_lock = azuredevops.CheckExclusiveLock("exampleCheckExclusiveLock",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_check_exclusive_lock = azuredevops.CheckExclusiveLock("example",
+            project_id=example.id,
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             timeout=43200)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -252,41 +254,43 @@
         ### Add Exclusive Lock to an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("exampleServiceEndpointGeneric",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
+            project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
-        example_check_exclusive_lock = azuredevops.CheckExclusiveLock("exampleCheckExclusiveLock",
-            project_id=example_project.id,
+        example_check_exclusive_lock = azuredevops.CheckExclusiveLock("example",
+            project_id=example.id,
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             timeout=43200)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Protect an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_check_exclusive_lock = azuredevops.CheckExclusiveLock("exampleCheckExclusiveLock",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_check_exclusive_lock = azuredevops.CheckExclusiveLock("example",
+            project_id=example.id,
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             timeout=43200)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/check_required_template.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/check_required_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,24 +187,24 @@
         ### Protect a service connection
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("exampleServiceEndpointGeneric",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
+            project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
-        example_check_required_template = azuredevops.CheckRequiredTemplate("exampleCheckRequiredTemplate",
-            project_id=example_project.id,
+        example_check_required_template = azuredevops.CheckRequiredTemplate("example",
+            project_id=example.id,
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             required_templates=[azuredevops.CheckRequiredTemplateRequiredTemplateArgs(
                 repository_type="azuregit",
                 repository_name="project/repository",
                 repository_ref="refs/heads/main",
                 template_path="template/path.yml",
@@ -215,18 +215,20 @@
         ### Protect an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_check_required_template = azuredevops.CheckRequiredTemplate("exampleCheckRequiredTemplate",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_check_required_template = azuredevops.CheckRequiredTemplate("example",
+            project_id=example.id,
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             required_templates=[
                 azuredevops.CheckRequiredTemplateRequiredTemplateArgs(
                     repository_name="project/repository",
                     repository_ref="refs/heads/main",
                     template_path="template/path.yml",
@@ -265,24 +267,24 @@
         ### Protect a service connection
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("exampleServiceEndpointGeneric",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
+            project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
-        example_check_required_template = azuredevops.CheckRequiredTemplate("exampleCheckRequiredTemplate",
-            project_id=example_project.id,
+        example_check_required_template = azuredevops.CheckRequiredTemplate("example",
+            project_id=example.id,
             target_resource_id=example_service_endpoint_generic.id,
             target_resource_type="endpoint",
             required_templates=[azuredevops.CheckRequiredTemplateRequiredTemplateArgs(
                 repository_type="azuregit",
                 repository_name="project/repository",
                 repository_ref="refs/heads/main",
                 template_path="template/path.yml",
@@ -293,18 +295,20 @@
         ### Protect an environment
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_check_required_template = azuredevops.CheckRequiredTemplate("exampleCheckRequiredTemplate",
-            project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_check_required_template = azuredevops.CheckRequiredTemplate("example",
+            project_id=example.id,
             target_resource_id=example_environment.id,
             target_resource_type="environment",
             required_templates=[
                 azuredevops.CheckRequiredTemplateRequiredTemplateArgs(
                     repository_name="project/repository",
                     repository_ref="refs/heads/main",
                     template_path="template/path.yml",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/config/__init__.pyi` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/config/vars.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/elastic_pool.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/elastic_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -430,34 +430,36 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example Azure Connection",
             description="Managed by Terraform",
             service_endpoint_authentication_scheme="ServicePrincipal",
             credentials=azuredevops.ServiceEndpointAzureRMCredentialsArgs(
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="00000000-0000-0000-0000-000000000000",
             ),
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Subscription Name")
-        example_elastic_pool = azuredevops.ElasticPool("exampleElasticPool",
+        example_elastic_pool = azuredevops.ElasticPool("example",
+            name="Example Elastic Pool",
             service_endpoint_id=example_service_endpoint_azure_rm.id,
-            service_endpoint_scope=example_project.id,
+            service_endpoint_scope=example.id,
             desired_idle=2,
             max_capacity=3,
             azure_resource_id="/subscriptions/<Subscription Id>/resourceGroups/<Resource Name>/providers/Microsoft.Compute/virtualMachineScaleSets/<VMSS Name>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
@@ -499,34 +501,36 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example Azure Connection",
             description="Managed by Terraform",
             service_endpoint_authentication_scheme="ServicePrincipal",
             credentials=azuredevops.ServiceEndpointAzureRMCredentialsArgs(
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="00000000-0000-0000-0000-000000000000",
             ),
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Subscription Name")
-        example_elastic_pool = azuredevops.ElasticPool("exampleElasticPool",
+        example_elastic_pool = azuredevops.ElasticPool("example",
+            name="Example Elastic Pool",
             service_endpoint_id=example_service_endpoint_azure_rm.id,
-            service_endpoint_scope=example_project.id,
+            service_endpoint_scope=example.id,
             desired_idle=2,
             max_capacity=3,
             azure_resource_id="/subscriptions/<Subscription Id>/resourceGroups/<Resource Name>/providers/Microsoft.Compute/virtualMachineScaleSets/<VMSS Name>")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/environment.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,20 +137,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Environments](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/environments?view=azure-devops-rest-7.0)
 
@@ -180,20 +183,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         * [Azure DevOps Service REST API 7.0 - Environments](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/environments?view=azure-devops-rest-7.0)
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/environment_resource_kubernetes.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/environment_resource_kubernetes.py`

 * *Files 4% similar despite different names*

```diff
@@ -266,37 +266,41 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_service_endpoint_kubernetes = azuredevops.ServiceEndpointKubernetes("exampleServiceEndpointKubernetes",
-            project_id=example_project.id,
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_service_endpoint_kubernetes = azuredevops.ServiceEndpointKubernetes("example",
+            project_id=example.id,
             service_endpoint_name="Example Kubernetes",
             apiserver_url="https://sample-kubernetes-cluster.hcp.westeurope.azmk8s.io",
             authorization_type="AzureSubscription",
             azure_subscriptions=[azuredevops.ServiceEndpointKubernetesAzureSubscriptionArgs(
                 subscription_id="00000000-0000-0000-0000-000000000000",
                 subscription_name="Example",
                 tenant_id="00000000-0000-0000-0000-000000000000",
                 resourcegroup_id="example-rg",
                 namespace="default",
                 cluster_name="example-aks",
             )])
-        example_environment_resource_kubernetes = azuredevops.EnvironmentResourceKubernetes("exampleEnvironmentResourceKubernetes",
-            project_id=example_project.id,
+        example_environment_resource_kubernetes = azuredevops.EnvironmentResourceKubernetes("example",
+            project_id=example.id,
             environment_id=example_environment.id,
             service_endpoint_id=example_service_endpoint_kubernetes.id,
+            name="Example",
             namespace="default",
             cluster_name="example-aks",
             tags=[
                 "tag1",
                 "tag2",
             ])
         ```
@@ -332,37 +336,41 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_environment = azuredevops.Environment("exampleEnvironment", project_id=example_project.id)
-        example_service_endpoint_kubernetes = azuredevops.ServiceEndpointKubernetes("exampleServiceEndpointKubernetes",
-            project_id=example_project.id,
+        example_environment = azuredevops.Environment("example",
+            project_id=example.id,
+            name="Example Environment")
+        example_service_endpoint_kubernetes = azuredevops.ServiceEndpointKubernetes("example",
+            project_id=example.id,
             service_endpoint_name="Example Kubernetes",
             apiserver_url="https://sample-kubernetes-cluster.hcp.westeurope.azmk8s.io",
             authorization_type="AzureSubscription",
             azure_subscriptions=[azuredevops.ServiceEndpointKubernetesAzureSubscriptionArgs(
                 subscription_id="00000000-0000-0000-0000-000000000000",
                 subscription_name="Example",
                 tenant_id="00000000-0000-0000-0000-000000000000",
                 resourcegroup_id="example-rg",
                 namespace="default",
                 cluster_name="example-aks",
             )])
-        example_environment_resource_kubernetes = azuredevops.EnvironmentResourceKubernetes("exampleEnvironmentResourceKubernetes",
-            project_id=example_project.id,
+        example_environment_resource_kubernetes = azuredevops.EnvironmentResourceKubernetes("example",
+            project_id=example.id,
             environment_id=example_environment.id,
             service_endpoint_id=example_service_endpoint_kubernetes.id,
+            name="Example",
             namespace="default",
             cluster_name="example-aks",
             tags=[
                 "tag1",
                 "tag2",
             ])
         ```
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_agent_queue.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_agent_queue.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,23 +89,24 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.Project("exampleProject",
+    example_project = azuredevops.Project("example",
+        name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
-    example_agent_queue = azuredevops.get_agent_queue_output(project_id=example_project.id,
+    example = azuredevops.get_agent_queue_output(project_id=example_project.id,
         name="Example Agent Queue")
-    pulumi.export("name", example_agent_queue.name)
-    pulumi.export("poolId", example_agent_queue.agent_pool_id)
+    pulumi.export("name", example.name)
+    pulumi.export("poolId", example.agent_pool_id)
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Agent Queues - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/queues/get?view=azure-devops-rest-7.0)
 
@@ -136,23 +137,24 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.Project("exampleProject",
+    example_project = azuredevops.Project("example",
+        name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
-    example_agent_queue = azuredevops.get_agent_queue_output(project_id=example_project.id,
+    example = azuredevops.get_agent_queue_output(project_id=example_project.id,
         name="Example Agent Queue")
-    pulumi.export("name", example_agent_queue.name)
-    pulumi.export("poolId", example_agent_queue.agent_pool_id)
+    pulumi.export("name", example.name)
+    pulumi.export("poolId", example.agent_pool_id)
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Agent Queues - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/queues/get?view=azure-devops-rest-7.0)
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_area.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,20 +124,21 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.Project("exampleProject",
+    example_project = azuredevops.Project("example",
+        name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
-    example_area = example_project.id.apply(lambda id: azuredevops.get_area_output(project_id=id,
+    example = example_project.id.apply(lambda id: azuredevops.get_area_output(project_id=id,
         path="/",
         fetch_children=False))
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
@@ -180,20 +181,21 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.Project("exampleProject",
+    example_project = azuredevops.Project("example",
+        name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
-    example_area = example_project.id.apply(lambda id: azuredevops.get_area_output(project_id=id,
+    example = example_project.id.apply(lambda id: azuredevops.get_area_output(project_id=id,
         path="/",
         fetch_children=False))
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_build_definition.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_build_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,18 +193,18 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.get_project(name="Example Project")
-    example_build_definition = azuredevops.get_build_definition(project_id=example_project.id,
+    example = azuredevops.get_project(name="Example Project")
+    example_get_build_definition = azuredevops.get_build_definition(project_id=example.id,
         name="existing")
-    pulumi.export("id", example_build_definition.id)
+    pulumi.export("id", example_get_build_definition.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of this Build Definition.
     :param str path: The path of the build definition. Default to `\\`.
     :param str project_id: The ID of the project.
@@ -243,18 +243,18 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.get_project(name="Example Project")
-    example_build_definition = azuredevops.get_build_definition(project_id=example_project.id,
+    example = azuredevops.get_project(name="Example Project")
+    example_get_build_definition = azuredevops.get_build_definition(project_id=example.id,
         name="existing")
-    pulumi.export("id", example_build_definition.id)
+    pulumi.export("id", example_get_build_definition.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of this Build Definition.
     :param str path: The path of the build definition. Default to `\\`.
     :param str project_id: The ID of the project.
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_client_config.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_client_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_git_repository.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_git_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
+    # Load a specific Git repository by name
     example_single_repo = azuredevops.get_git_repository(project_id=example.id,
         name="Example Repository")
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
@@ -208,14 +209,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
+    # Load a specific Git repository by name
     example_single_repo = azuredevops.get_git_repository(project_id=example.id,
         name="Example Repository")
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_group.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,22 +107,22 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.get_project(name="Example Project")
-    example_group = azuredevops.get_group(project_id=example_project.id,
+    example = azuredevops.get_project(name="Example Project")
+    example_get_group = azuredevops.get_group(project_id=example.id,
         name="Example Group")
-    pulumi.export("groupId", example_group.id)
-    pulumi.export("groupDescriptor", example_group.descriptor)
+    pulumi.export("groupId", example_get_group.id)
+    pulumi.export("groupDescriptor", example_get_group.descriptor)
     example_collection_group = azuredevops.get_group(name="Project Collection Administrators")
-    pulumi.export("collectionGroupId", example_group.id)
-    pulumi.export("collectionGroupDescriptor", example_group.descriptor)
+    pulumi.export("collectionGroupId", example_get_group.id)
+    pulumi.export("collectionGroupDescriptor", example_get_group.descriptor)
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Groups - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/groups/get?view=azure-devops-rest-7.0)
 
@@ -160,22 +160,22 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.get_project(name="Example Project")
-    example_group = azuredevops.get_group(project_id=example_project.id,
+    example = azuredevops.get_project(name="Example Project")
+    example_get_group = azuredevops.get_group(project_id=example.id,
         name="Example Group")
-    pulumi.export("groupId", example_group.id)
-    pulumi.export("groupDescriptor", example_group.descriptor)
+    pulumi.export("groupId", example_get_group.id)
+    pulumi.export("groupDescriptor", example_get_group.descriptor)
     example_collection_group = azuredevops.get_group(name="Project Collection Administrators")
-    pulumi.export("collectionGroupId", example_group.id)
-    pulumi.export("collectionGroupDescriptor", example_group.descriptor)
+    pulumi.export("collectionGroupId", example_get_group.id)
+    pulumi.export("collectionGroupDescriptor", example_get_group.descriptor)
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Groups - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/groups/get?view=azure-devops-rest-7.0)
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_groups.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_groups.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,15 +75,17 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
+    # load all existing groups inside an organization
     example_all_groups = azuredevops.get_groups()
+    # load all existing groups inside a specific project
     example_project_groups = azuredevops.get_groups(project_id=example.id)
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Groups - List](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/groups/list?view=azure-devops-rest-7.0)
@@ -112,15 +114,17 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
+    # load all existing groups inside an organization
     example_all_groups = azuredevops.get_groups()
+    # load all existing groups inside a specific project
     example_project_groups = azuredevops.get_groups(project_id=example.id)
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Groups - List](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/groups/list?view=azure-devops-rest-7.0)
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_iteration.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_iteration.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.Project("example",
+        name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
     example_root_iteration = azuredevops.get_iteration_output(project_id=example.id,
         path="/",
         fetch_children=True)
@@ -184,14 +185,15 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.Project("example",
+        name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
     example_root_iteration = azuredevops.get_iteration_output(project_id=example.id,
         path="/",
         fetch_children=True)
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_pool.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_pools.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_project.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_projects.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_repositories.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_repositories.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,16 +102,18 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
+    # Load all Git repositories of a project, which are accessible for the current user
     example_all_repos = azuredevops.get_repositories(project_id=example.id,
         include_hidden=True)
+    # Load a specific Git repository by name
     example_single_repo = azuredevops.get_repositories(project_id=example.id,
         name="Example Repository")
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
@@ -150,16 +152,18 @@
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_project(name="Example Project")
+    # Load all Git repositories of a project, which are accessible for the current user
     example_all_repos = azuredevops.get_repositories(project_id=example.id,
         include_hidden=True)
+    # Load a specific Git repository by name
     example_single_repo = azuredevops.get_repositories(project_id=example.id,
         name="Example Repository")
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_service_endpoint_azure_rm.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_service_endpoint_github.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_service_endpoint_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_serviceendpoint_azurecr.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_azurecr.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example = azuredevops.get_serviceendpoint_azurecr(project_id=azuredevops_project["example"]["id"],
+    example = azuredevops.get_serviceendpoint_azurecr(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example Azure Container Registry")
     pulumi.export("serviceEndpointId", example.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
@@ -279,15 +279,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example = azuredevops.get_serviceendpoint_azurecr(project_id=azuredevops_project["example"]["id"],
+    example = azuredevops.get_serviceendpoint_azurecr(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example Azure Container Registry")
     pulumi.export("serviceEndpointId", example.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_serviceendpoint_npm.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_npm.py`

 * *Files 7% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example = azuredevops.get_serviceendpoint_npm(project_id=azuredevops_project["example"]["id"],
+    example = azuredevops.get_serviceendpoint_npm(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example npm")
     pulumi.export("serviceEndpointId", example.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
@@ -162,15 +162,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example = azuredevops.get_serviceendpoint_npm(project_id=azuredevops_project["example"]["id"],
+    example = azuredevops.get_serviceendpoint_npm(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example npm")
     pulumi.export("serviceEndpointId", example.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example = azuredevops.get_serviceendpoint_sonarcloud(project_id=azuredevops_project["example"]["id"],
+    example = azuredevops.get_serviceendpoint_sonarcloud(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example Sonar Cloud")
     pulumi.export("serviceEndpointId", example.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
@@ -149,15 +149,15 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example = azuredevops.get_serviceendpoint_sonarcloud(project_id=azuredevops_project["example"]["id"],
+    example = azuredevops.get_serviceendpoint_sonarcloud(project_id=example_azuredevops_project["id"],
         service_endpoint_name="Example Sonar Cloud")
     pulumi.export("serviceEndpointId", example.id)
     ```
     <!--End PulumiCodeChooser -->
 
 
     :param str project_id: The ID of the project.
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_team.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_team.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,20 +129,21 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.Project("exampleProject",
+    example_project = azuredevops.Project("example",
+        name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
-    example_team = azuredevops.get_team_output(project_id=example_project.id,
+    example = azuredevops.get_team_output(project_id=example_project.id,
         name="Example Project Team")
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Teams - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get?view=azure-devops-rest-7.0)
@@ -185,20 +186,21 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.Project("exampleProject",
+    example_project = azuredevops.Project("example",
+        name="Example Project",
         work_item_template="Agile",
         version_control="Git",
         visibility="private",
         description="Managed by Terraform")
-    example_team = azuredevops.get_team_output(project_id=example_project.id,
+    example = azuredevops.get_team_output(project_id=example_project.id,
         name="Example Project Team")
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Teams - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get?view=azure-devops-rest-7.0)
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_teams.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_users.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_users.py`

 * *Files 21% similar despite different names*

```diff
@@ -117,59 +117,20 @@
               origin_id: Optional[str] = None,
               principal_name: Optional[str] = None,
               subject_types: Optional[Sequence[str]] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUsersResult:
     """
     Use this data source to access information about an existing users within Azure DevOps.
 
-    ## Example Usage
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_azuredevops as azuredevops
-
-    example = azuredevops.get_users(principal_name="contoso-user@contoso.onmicrosoft.com")
-    example_all_users = azuredevops.get_users(features=azuredevops.GetUsersFeaturesArgs(
-        concurrent_workers=10,
-    ))
-    example_all_from_origin = azuredevops.get_users(origin="aad")
-    example_all_from_subject_types = azuredevops.get_users(subject_types=[
-        "aad",
-        "msa",
-    ])
-    example_all_from_origin_id = azuredevops.get_users(origin="aad",
-        origin_id="00000000-0000-0000-0000-000000000000")
-    ```
-    <!--End PulumiCodeChooser -->
-
-    ## Relevant Links
-
-    - [Azure DevOps Service REST API 7.0 - Graph Users API](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/users?view=azure-devops-rest-7.0)
-
 
     :param pulumi.InputType['GetUsersFeaturesArgs'] features: A `features` block as defined below.
            
            DataSource without specifying any arguments will return all users inside an organization.
            
            List of possible subject types
-           
-           <!--Start PulumiCodeChooser -->
-           ```python
-           import pulumi
-           ```
-           <!--End PulumiCodeChooser -->
-           
-           List of possible origins
-           
-           <!--Start PulumiCodeChooser -->
-           ```python
-           import pulumi
-           ```
-           <!--End PulumiCodeChooser -->
     :param str origin: The type of source provider for the `origin_id` parameter (ex:AD, AAD, MSA) The supported origins are listed below.
     :param str origin_id: The unique identifier from the system of origin.
     :param str principal_name: The PrincipalName of this graph member from the source provider.
     :param Sequence[str] subject_types: A list of user subject subtypes to reduce the retrieved results, e.g. `msa`, `aad`, `svc` (service identity), `imp` (imported identity), etc. The supported subject types are listed below.
     """
     __args__ = dict()
     __args__['features'] = features
@@ -196,58 +157,19 @@
                      origin_id: Optional[pulumi.Input[Optional[str]]] = None,
                      principal_name: Optional[pulumi.Input[Optional[str]]] = None,
                      subject_types: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUsersResult]:
     """
     Use this data source to access information about an existing users within Azure DevOps.
 
-    ## Example Usage
-
-    <!--Start PulumiCodeChooser -->
-    ```python
-    import pulumi
-    import pulumi_azuredevops as azuredevops
-
-    example = azuredevops.get_users(principal_name="contoso-user@contoso.onmicrosoft.com")
-    example_all_users = azuredevops.get_users(features=azuredevops.GetUsersFeaturesArgs(
-        concurrent_workers=10,
-    ))
-    example_all_from_origin = azuredevops.get_users(origin="aad")
-    example_all_from_subject_types = azuredevops.get_users(subject_types=[
-        "aad",
-        "msa",
-    ])
-    example_all_from_origin_id = azuredevops.get_users(origin="aad",
-        origin_id="00000000-0000-0000-0000-000000000000")
-    ```
-    <!--End PulumiCodeChooser -->
-
-    ## Relevant Links
-
-    - [Azure DevOps Service REST API 7.0 - Graph Users API](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/users?view=azure-devops-rest-7.0)
-
 
     :param pulumi.InputType['GetUsersFeaturesArgs'] features: A `features` block as defined below.
            
            DataSource without specifying any arguments will return all users inside an organization.
            
            List of possible subject types
-           
-           <!--Start PulumiCodeChooser -->
-           ```python
-           import pulumi
-           ```
-           <!--End PulumiCodeChooser -->
-           
-           List of possible origins
-           
-           <!--Start PulumiCodeChooser -->
-           ```python
-           import pulumi
-           ```
-           <!--End PulumiCodeChooser -->
     :param str origin: The type of source provider for the `origin_id` parameter (ex:AD, AAD, MSA) The supported origins are listed below.
     :param str origin_id: The unique identifier from the system of origin.
     :param str principal_name: The PrincipalName of this graph member from the source provider.
     :param Sequence[str] subject_types: A list of user subject subtypes to reduce the retrieved results, e.g. `msa`, `aad`, `svc` (service identity), `imp` (imported identity), etc. The supported subject types are listed below.
     """
     ...
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/get_variable_group.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/get_variable_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,18 +125,18 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.get_project(name="Example Project")
-    example_variable_group = azuredevops.get_variable_group(project_id=example_project.id,
+    example = azuredevops.get_project(name="Example Project")
+    example_get_variable_group = azuredevops.get_variable_group(project_id=example.id,
         name="Example Variable Group")
-    pulumi.export("id", example_variable_group.id)
+    pulumi.export("id", example_get_variable_group.id)
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Variable Groups](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/variablegroups?view=azure-devops-rest-7.0)
 
@@ -172,18 +172,18 @@
     ## Example Usage
 
     <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
-    example_project = azuredevops.get_project(name="Example Project")
-    example_variable_group = azuredevops.get_variable_group(project_id=example_project.id,
+    example = azuredevops.get_project(name="Example Project")
+    example_get_variable_group = azuredevops.get_variable_group(project_id=example.id,
         name="Example Variable Group")
-    pulumi.export("id", example_variable_group.id)
+    pulumi.export("id", example_get_variable_group.id)
     ```
     <!--End PulumiCodeChooser -->
 
     ## Relevant Links
 
     - [Azure DevOps Service REST API 7.0 - Variable Groups](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/variablegroups?view=azure-devops-rest-7.0)
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/git.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/git_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,14 +334,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_permissions = azuredevops.GitPermissions("example-permissions",
@@ -362,22 +363,24 @@
         #### Example usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_group = azuredevops.get_group(name="Project Collection Administrators")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Empty Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
         example_permissions = azuredevops.GitPermissions("example-permissions",
             project_id=example_git.project_id,
             repository_id=example_git.id,
             principal=example_group.id,
@@ -397,21 +400,23 @@
         #### Example usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Empty Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
         example_group = azuredevops.get_group(name="Project Collection Administrators")
         example_permissions = azuredevops.GitPermissions("example-permissions",
             project_id=example_git.project_id,
             repository_id=example_git.id,
@@ -427,35 +432,37 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_project_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_project_contributors = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_contributors = azuredevops.get_group_output(project_id=example.id,
             name="Contributors")
-        example_project_administrators = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_administrators = azuredevops.get_group_output(project_id=example.id,
             name="Project administrators")
         example_permissions = azuredevops.GitPermissions("example-permissions",
-            project_id=example_project.id,
+            project_id=example.id,
             principal=example_project_readers.id,
             permissions={
                 "CreateRepository": "Deny",
                 "DeleteRepository": "Deny",
                 "RenameRepository": "NotSet",
             })
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="TestRepo",
             default_branch="refs/heads/master",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
         example_repo_permissions = azuredevops.GitPermissions("example-repo-permissions",
             project_id=example_git.project_id,
             repository_id=example_git.id,
@@ -545,14 +552,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_permissions = azuredevops.GitPermissions("example-permissions",
@@ -573,22 +581,24 @@
         #### Example usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_group = azuredevops.get_group(name="Project Collection Administrators")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Empty Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
         example_permissions = azuredevops.GitPermissions("example-permissions",
             project_id=example_git.project_id,
             repository_id=example_git.id,
             principal=example_group.id,
@@ -608,21 +618,23 @@
         #### Example usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Empty Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
         example_group = azuredevops.get_group(name="Project Collection Administrators")
         example_permissions = azuredevops.GitPermissions("example-permissions",
             project_id=example_git.project_id,
             repository_id=example_git.id,
@@ -638,35 +650,37 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_project_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_project_contributors = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_contributors = azuredevops.get_group_output(project_id=example.id,
             name="Contributors")
-        example_project_administrators = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_administrators = azuredevops.get_group_output(project_id=example.id,
             name="Project administrators")
         example_permissions = azuredevops.GitPermissions("example-permissions",
-            project_id=example_project.id,
+            project_id=example.id,
             principal=example_project_readers.id,
             permissions={
                 "CreateRepository": "Deny",
                 "DeleteRepository": "Deny",
                 "RenameRepository": "NotSet",
             })
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="TestRepo",
             default_branch="refs/heads/master",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
         example_repo_permissions = azuredevops.GitPermissions("example-repo-permissions",
             project_id=example_git.project_id,
             repository_id=example_git.id,
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/git_repository_branch.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_repository_branch.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,28 +219,32 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_git_repository_branch = azuredevops.GitRepositoryBranch("exampleGitRepositoryBranch",
+        example_git_repository_branch = azuredevops.GitRepositoryBranch("example",
             repository_id=example_git.id,
+            name="example-branch-name",
             ref_branch=example_git.default_branch)
-        example_from_commit_id = azuredevops.GitRepositoryBranch("exampleFromCommitId",
+        example_from_commit_id = azuredevops.GitRepositoryBranch("example_from_commit_id",
             repository_id=example_git.id,
+            name="example-from-commit-id",
             ref_commit_id=example_git_repository_branch.last_commit_id)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of the branch in short format not prefixed with `refs/heads/`.
@@ -261,28 +265,32 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_git_repository_branch = azuredevops.GitRepositoryBranch("exampleGitRepositoryBranch",
+        example_git_repository_branch = azuredevops.GitRepositoryBranch("example",
             repository_id=example_git.id,
+            name="example-branch-name",
             ref_branch=example_git.default_branch)
-        example_from_commit_id = azuredevops.GitRepositoryBranch("exampleFromCommitId",
+        example_from_commit_id = azuredevops.GitRepositoryBranch("example_from_commit_id",
             repository_id=example_git.id,
+            name="example-from-commit-id",
             ref_commit_id=example_git_repository_branch.last_commit_id)
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param GitRepositoryBranchArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/git_repository_file.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/git_repository_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,24 +238,26 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_git_repository_file = azuredevops.GitRepositoryFile("exampleGitRepositoryFile",
+        example_git_repository_file = azuredevops.GitRepositoryFile("example",
             repository_id=example_git.id,
             file=".gitignore",
             content="**/*.tfstate",
             branch="refs/heads/master",
             commit_message="First commit",
             overwrite_on_create=False)
         ```
@@ -301,24 +303,26 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Git Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_git_repository_file = azuredevops.GitRepositoryFile("exampleGitRepositoryFile",
+        example_git_repository_file = azuredevops.GitRepositoryFile("example",
             repository_id=example_git.id,
             file=".gitignore",
             content="**/*.tfstate",
             branch="refs/heads/master",
             commit_message="First commit",
             overwrite_on_create=False)
         ```
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/group.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,21 +333,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_contributors = azuredevops.get_group_output(project_id=example_project.id,
+        example_contributors = azuredevops.get_group_output(project_id=example.id,
             name="Contributors")
-        example_group = azuredevops.Group("exampleGroup",
-            scope=example_project.id,
+        example_group = azuredevops.Group("example",
+            scope=example.id,
             display_name="Example group",
             description="Example description",
             members=[
                 example_readers.descriptor,
                 example_contributors.descriptor,
             ])
         ```
@@ -390,21 +390,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example = azuredevops.Project("example", name="Example Project")
+        example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_contributors = azuredevops.get_group_output(project_id=example_project.id,
+        example_contributors = azuredevops.get_group_output(project_id=example.id,
             name="Contributors")
-        example_group = azuredevops.Group("exampleGroup",
-            scope=example_project.id,
+        example_group = azuredevops.Group("example",
+            scope=example.id,
             display_name="Example group",
             description="Example description",
             members=[
                 example_readers.descriptor,
                 example_contributors.descriptor,
             ])
         ```
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/group_entitlement.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group_entitlement.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/group_membership.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/group_membership.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,20 +152,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_user = azuredevops.User("exampleUser", principal_name="foo@contoso.com")
-        example_group = azuredevops.get_group_output(project_id=example_project.id,
+        example_project = azuredevops.Project("example", name="Example Project")
+        example_user = azuredevops.User("example", principal_name="foo@contoso.com")
+        example = azuredevops.get_group_output(project_id=example_project.id,
             name="Build Administrators")
-        example_group_membership = azuredevops.GroupMembership("exampleGroupMembership",
-            group=example_group.descriptor,
+        example_group_membership = azuredevops.GroupMembership("example",
+            group=example.descriptor,
             members=[example_user.descriptor])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Memberships](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/memberships?view=azure-devops-rest-7.0)
@@ -200,20 +200,20 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_user = azuredevops.User("exampleUser", principal_name="foo@contoso.com")
-        example_group = azuredevops.get_group_output(project_id=example_project.id,
+        example_project = azuredevops.Project("example", name="Example Project")
+        example_user = azuredevops.User("example", principal_name="foo@contoso.com")
+        example = azuredevops.get_group_output(project_id=example_project.id,
             name="Build Administrators")
-        example_group_membership = azuredevops.GroupMembership("exampleGroupMembership",
-            group=example_group.descriptor,
+        example_group_membership = azuredevops.GroupMembership("example",
+            group=example.descriptor,
             members=[example_user.descriptor])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Memberships](https://docs.microsoft.com/en-us/rest/api/azure/devops/graph/memberships?view=azure-devops-rest-7.0)
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/iterative_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/iterative_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_root_permissions = azuredevops.IterativePermissions("example-root-permissions",
@@ -314,14 +315,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_root_permissions = azuredevops.IterativePermissions("example-root-permissions",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/library_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/library_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
+            name="Testing",
             description="Testing-description",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
         tf_project_readers = azuredevops.get_group_output(project_id=project.id,
             name="Readers")
         permissions = azuredevops.LibraryPermissions("permissions",
@@ -278,14 +279,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
+            name="Testing",
             description="Testing-description",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
         tf_project_readers = azuredevops.get_group_output(project_id=project.id,
             name="Readers")
         permissions = azuredevops.LibraryPermissions("permissions",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/outputs.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/pipeline_authorization.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/pipeline_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,60 +194,65 @@
         ### Authorization for all pipelines
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_pool = azuredevops.Pool("examplePool",
+        example_pool = azuredevops.Pool("example",
+            name="Example Pool",
             auto_provision=False,
             auto_update=False)
-        example_queue = azuredevops.Queue("exampleQueue",
-            project_id=example_project.id,
+        example_queue = azuredevops.Queue("example",
+            project_id=example.id,
             agent_pool_id=example_pool.id)
-        example_pipeline_authorization = azuredevops.PipelineAuthorization("examplePipelineAuthorization",
-            project_id=example_project.id,
+        example_pipeline_authorization = azuredevops.PipelineAuthorization("example",
+            project_id=example.id,
             resource_id=example_queue.id,
             type="queue")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Authorization for specific pipeline
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example_project = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_pool = azuredevops.Pool("examplePool",
+        example_pool = azuredevops.Pool("example",
+            name="Example Pool",
             auto_provision=False,
             auto_update=False)
-        example_queue = azuredevops.Queue("exampleQueue",
+        example_queue = azuredevops.Queue("example",
             project_id=example_project.id,
             agent_pool_id=example_pool.id)
-        example_git_repository = azuredevops.get_git_repository_output(project_id=example_project.id,
+        example = azuredevops.get_git_repository_output(project_id=example_project.id,
             name="Example Project")
-        example_build_definition = azuredevops.BuildDefinition("exampleBuildDefinition",
+        example_build_definition = azuredevops.BuildDefinition("example",
             project_id=example_project.id,
+            name="Example Pipeline",
             repository=azuredevops.BuildDefinitionRepositoryArgs(
                 repo_type="TfsGit",
-                repo_id=example_git_repository.id,
+                repo_id=example.id,
                 yml_path="azure-pipelines.yml",
             ))
-        example_pipeline_authorization = azuredevops.PipelineAuthorization("examplePipelineAuthorization",
+        example_pipeline_authorization = azuredevops.PipelineAuthorization("example",
             project_id=example_project.id,
             resource_id=example_queue.id,
             type="queue",
             pipeline_id=example_build_definition.id)
         ```
         <!--End PulumiCodeChooser -->
 
@@ -285,60 +290,65 @@
         ### Authorization for all pipelines
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_pool = azuredevops.Pool("examplePool",
+        example_pool = azuredevops.Pool("example",
+            name="Example Pool",
             auto_provision=False,
             auto_update=False)
-        example_queue = azuredevops.Queue("exampleQueue",
-            project_id=example_project.id,
+        example_queue = azuredevops.Queue("example",
+            project_id=example.id,
             agent_pool_id=example_pool.id)
-        example_pipeline_authorization = azuredevops.PipelineAuthorization("examplePipelineAuthorization",
-            project_id=example_project.id,
+        example_pipeline_authorization = azuredevops.PipelineAuthorization("example",
+            project_id=example.id,
             resource_id=example_queue.id,
             type="queue")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Authorization for specific pipeline
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example_project = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_pool = azuredevops.Pool("examplePool",
+        example_pool = azuredevops.Pool("example",
+            name="Example Pool",
             auto_provision=False,
             auto_update=False)
-        example_queue = azuredevops.Queue("exampleQueue",
+        example_queue = azuredevops.Queue("example",
             project_id=example_project.id,
             agent_pool_id=example_pool.id)
-        example_git_repository = azuredevops.get_git_repository_output(project_id=example_project.id,
+        example = azuredevops.get_git_repository_output(project_id=example_project.id,
             name="Example Project")
-        example_build_definition = azuredevops.BuildDefinition("exampleBuildDefinition",
+        example_build_definition = azuredevops.BuildDefinition("example",
             project_id=example_project.id,
+            name="Example Pipeline",
             repository=azuredevops.BuildDefinitionRepositoryArgs(
                 repo_type="TfsGit",
-                repo_id=example_git_repository.id,
+                repo_id=example.id,
                 yml_path="azure-pipelines.yml",
             ))
-        example_pipeline_authorization = azuredevops.PipelineAuthorization("examplePipelineAuthorization",
+        example_pipeline_authorization = azuredevops.PipelineAuthorization("example",
             project_id=example_project.id,
             resource_id=example_queue.id,
             type="queue",
             pipeline_id=example_build_definition.id)
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/pool.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Pool("example",
+            name="Example-pool",
             auto_provision=False,
             auto_update=False)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
@@ -213,14 +214,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Pool("example",
+            name="Example-pool",
             auto_provision=False,
             auto_update=False)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/project.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,22 +278,23 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
+            visibility="private",
+            version_control="Git",
+            work_item_template="Agile",
             description="Managed by Terraform",
             features={
-                "artifacts": "disabled",
                 "testplans": "disabled",
-            },
-            version_control="Git",
-            visibility="private",
-            work_item_template="Agile")
+                "artifacts": "disabled",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Projects](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects?view=azure-devops-rest-7.0)
 
@@ -343,22 +344,23 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
+            visibility="private",
+            version_control="Git",
+            work_item_template="Agile",
             description="Managed by Terraform",
             features={
-                "artifacts": "disabled",
                 "testplans": "disabled",
-            },
-            version_control="Git",
-            visibility="private",
-            work_item_template="Agile")
+                "artifacts": "disabled",
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Projects](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects?view=azure-devops-rest-7.0)
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/project_features.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
         example_features = azuredevops.ProjectFeatures("example-features",
             project_id=example.id,
             features={
@@ -176,14 +177,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
         example_features = azuredevops.ProjectFeatures("example-features",
             project_id=example.id,
             features={
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/project_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_permission = azuredevops.ProjectPermissions("example-permission",
@@ -367,14 +368,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_permission = azuredevops.ProjectPermissions("example-permission",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/project_pipeline_settings.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/project_pipeline_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,21 +289,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_project_pipeline_settings = azuredevops.ProjectPipelineSettings("exampleProjectPipelineSettings",
-            project_id=example_project.id,
+        example_project_pipeline_settings = azuredevops.ProjectPipelineSettings("example",
+            project_id=example.id,
             enforce_job_scope=True,
             enforce_referenced_repo_scoped_token=False,
             enforce_settable_var=True,
             publish_pipeline_metadata=False,
             status_badges_are_private=True)
         ```
         <!--End PulumiCodeChooser -->
@@ -351,21 +352,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_project_pipeline_settings = azuredevops.ProjectPipelineSettings("exampleProjectPipelineSettings",
-            project_id=example_project.id,
+        example_project_pipeline_settings = azuredevops.ProjectPipelineSettings("example",
+            project_id=example.id,
             enforce_job_scope=True,
             enforce_referenced_repo_scoped_token=False,
             enforce_settable_var=True,
             publish_pipeline_metadata=False,
             status_badges_are_private=True)
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/provider.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/queue.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,37 +159,39 @@
         ### Creating a Queue from an organization-level pool
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_pool = azuredevops.get_pool(name="example-pool")
-        example_queue = azuredevops.Queue("exampleQueue",
+        example_project = azuredevops.Project("example", name="Example Project")
+        example = azuredevops.get_pool(name="example-pool")
+        example_queue = azuredevops.Queue("example",
             project_id=example_project.id,
-            agent_pool_id=example_pool.id)
+            agent_pool_id=example.id)
         # Grant access to queue to all pipelines in the project
-        example_resource_authorization = azuredevops.ResourceAuthorization("exampleResourceAuthorization",
+        example_resource_authorization = azuredevops.ResourceAuthorization("example",
             project_id=example_project.id,
             resource_id=example_queue.id,
             type="queue",
             authorized=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating a Queue at the project level (Organization-level permissions not required)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.get_project(name="Example Project")
-        example_queue = azuredevops.Queue("exampleQueue", project_id=example_project.id)
+        example = azuredevops.get_project(name="Example Project")
+        example_queue = azuredevops.Queue("example",
+            name="example-queue",
+            project_id=example.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Queues](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/queues?view=azure-devops-rest-7.0)
 
@@ -229,37 +231,39 @@
         ### Creating a Queue from an organization-level pool
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_pool = azuredevops.get_pool(name="example-pool")
-        example_queue = azuredevops.Queue("exampleQueue",
+        example_project = azuredevops.Project("example", name="Example Project")
+        example = azuredevops.get_pool(name="example-pool")
+        example_queue = azuredevops.Queue("example",
             project_id=example_project.id,
-            agent_pool_id=example_pool.id)
+            agent_pool_id=example.id)
         # Grant access to queue to all pipelines in the project
-        example_resource_authorization = azuredevops.ResourceAuthorization("exampleResourceAuthorization",
+        example_resource_authorization = azuredevops.ResourceAuthorization("example",
             project_id=example_project.id,
             resource_id=example_queue.id,
             type="queue",
             authorized=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ### Creating a Queue at the project level (Organization-level permissions not required)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.get_project(name="Example Project")
-        example_queue = azuredevops.Queue("exampleQueue", project_id=example_project.id)
+        example = azuredevops.get_project(name="Example Project")
+        example_queue = azuredevops.Queue("example",
+            name="example-queue",
+            project_id=example.id)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.0 - Agent Queues](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/queues?view=azure-devops-rest-7.0)
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_author_email_pattern.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_author_email_pattern.py`

 * *Files 8% similar despite different names*

```diff
@@ -206,26 +206,28 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_author_email_pattern = azuredevops.RepositoryPolicyAuthorEmailPattern("exampleRepositoryPolicyAuthorEmailPattern",
-            project_id=example_project.id,
+        example_repository_policy_author_email_pattern = azuredevops.RepositoryPolicyAuthorEmailPattern("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             author_email_patterns=[
                 "user1@test.com",
                 "user2@test.com",
             ],
             repository_ids=[example_git.id])
@@ -235,21 +237,22 @@
         ## Set project level repository policy
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_author_email_pattern = azuredevops.RepositoryPolicyAuthorEmailPattern("exampleRepositoryPolicyAuthorEmailPattern",
-            project_id=example_project.id,
+        example_repository_policy_author_email_pattern = azuredevops.RepositoryPolicyAuthorEmailPattern("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             author_email_patterns=[
                 "user1@test.com",
                 "user2@test.com",
             ])
         ```
@@ -288,26 +291,28 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_author_email_pattern = azuredevops.RepositoryPolicyAuthorEmailPattern("exampleRepositoryPolicyAuthorEmailPattern",
-            project_id=example_project.id,
+        example_repository_policy_author_email_pattern = azuredevops.RepositoryPolicyAuthorEmailPattern("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             author_email_patterns=[
                 "user1@test.com",
                 "user2@test.com",
             ],
             repository_ids=[example_git.id])
@@ -317,21 +322,22 @@
         ## Set project level repository policy
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_author_email_pattern = azuredevops.RepositoryPolicyAuthorEmailPattern("exampleRepositoryPolicyAuthorEmailPattern",
-            project_id=example_project.id,
+        example_repository_policy_author_email_pattern = azuredevops.RepositoryPolicyAuthorEmailPattern("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             author_email_patterns=[
                 "user1@test.com",
                 "user2@test.com",
             ])
         ```
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_case_enforcement.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_case_enforcement.py`

 * *Files 10% similar despite different names*

```diff
@@ -204,46 +204,49 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("exampleRepositoryPolicyCaseEnforcement",
-            project_id=example_project.id,
+        example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             enforce_consistent_case=True,
             repository_ids=[example_git.id])
         ```
         <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("exampleRepositoryPolicyCaseEnforcement",
-            project_id=example_project.id,
+        example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             enforce_consistent_case=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
@@ -280,46 +283,49 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("exampleRepositoryPolicyCaseEnforcement",
-            project_id=example_project.id,
+        example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             enforce_consistent_case=True,
             repository_ids=[example_git.id])
         ```
         <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("exampleRepositoryPolicyCaseEnforcement",
-            project_id=example_project.id,
+        example_repository_policy_case_enforcement = azuredevops.RepositoryPolicyCaseEnforcement("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             enforce_consistent_case=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_check_credentials.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_check_credentials.py`

 * *Files 5% similar despite different names*

```diff
@@ -172,45 +172,48 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("exampleRepositoryPolicyCheckCredentials",
-            project_id=example_project.id,
+        example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             repository_ids=[example_git.id])
         ```
         <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("exampleRepositoryPolicyCheckCredentials",
-            project_id=example_project.id,
+        example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("example",
+            project_id=example.id,
             enabled=True,
             blocking=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
@@ -245,45 +248,48 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("exampleRepositoryPolicyCheckCredentials",
-            project_id=example_project.id,
+        example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             repository_ids=[example_git.id])
         ```
         <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("exampleRepositoryPolicyCheckCredentials",
-            project_id=example_project.id,
+        example_repository_policy_check_credentials = azuredevops.RepositoryPolicyCheckCredentials("example",
+            project_id=example.id,
             enabled=True,
             blocking=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_file_path_pattern.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_file_path_pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,26 +202,28 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_file_path_pattern = azuredevops.RepositoryPolicyFilePathPattern("exampleRepositoryPolicyFilePathPattern",
-            project_id=example_project.id,
+        example_repository_policy_file_path_pattern = azuredevops.RepositoryPolicyFilePathPattern("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             filepath_patterns=[
                 "*.go",
                 "/home/test/*.ts",
             ],
             repository_ids=[example_git.id])
@@ -231,14 +233,15 @@
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
         examplep = azuredevops.RepositoryPolicyFilePathPattern("examplep",
             project_id=example.id,
             enabled=True,
@@ -282,26 +285,28 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_file_path_pattern = azuredevops.RepositoryPolicyFilePathPattern("exampleRepositoryPolicyFilePathPattern",
-            project_id=example_project.id,
+        example_repository_policy_file_path_pattern = azuredevops.RepositoryPolicyFilePathPattern("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             filepath_patterns=[
                 "*.go",
                 "/home/test/*.ts",
             ],
             repository_ids=[example_git.id])
@@ -311,14 +316,15 @@
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
         examplep = azuredevops.RepositoryPolicyFilePathPattern("examplep",
             project_id=example.id,
             enabled=True,
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_max_file_size.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_max_file_size.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,46 +204,49 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("exampleRepositoryPolicyMaxFileSize",
-            project_id=example_project.id,
+        example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             max_file_size=1,
             repository_ids=[example_git.id])
         ```
         <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("exampleRepositoryPolicyMaxFileSize",
-            project_id=example_project.id,
+        example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             max_file_size=1)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
@@ -280,46 +283,49 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("exampleRepositoryPolicyMaxFileSize",
-            project_id=example_project.id,
+        example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             max_file_size=1,
             repository_ids=[example_git.id])
         ```
         <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("exampleRepositoryPolicyMaxFileSize",
-            project_id=example_project.id,
+        example_repository_policy_max_file_size = azuredevops.RepositoryPolicyMaxFileSize("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             max_file_size=1)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_max_path_length.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_max_path_length.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,46 +204,49 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Sample Repo",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("exampleRepositoryPolicyMaxPathLength",
-            project_id=example_project.id,
+        example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             max_path_length=500,
             repository_ids=[example_git.id])
         ```
         <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("exampleRepositoryPolicyMaxPathLength",
-            project_id=example_project.id,
+        example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             max_path_length=1000)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
@@ -280,46 +283,49 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Sample Repo",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("exampleRepositoryPolicyMaxPathLength",
-            project_id=example_project.id,
+        example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             max_path_length=500,
             repository_ids=[example_git.id])
         ```
         <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("exampleRepositoryPolicyMaxPathLength",
-            project_id=example_project.id,
+        example_repository_policy_max_path_length = azuredevops.RepositoryPolicyMaxPathLength("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             max_path_length=1000)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/repository_policy_reserved_names.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/repository_policy_reserved_names.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,45 +172,48 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("exampleRepositoryPolicyReservedNames",
-            project_id=example_project.id,
+        example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             repository_ids=[example_git.id])
         ```
         <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("exampleRepositoryPolicyReservedNames",
-            project_id=example_project.id,
+        example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("example",
+            project_id=example.id,
             enabled=True,
             blocking=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
@@ -245,45 +248,48 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_git = azuredevops.Git("exampleGit",
-            project_id=example_project.id,
+        example_git = azuredevops.Git("example",
+            project_id=example.id,
+            name="Example Repository",
             initialization=azuredevops.GitInitializationArgs(
                 init_type="Clean",
             ))
-        example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("exampleRepositoryPolicyReservedNames",
-            project_id=example_project.id,
+        example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("example",
+            project_id=example.id,
             enabled=True,
             blocking=True,
             repository_ids=[example_git.id])
         ```
         <!--End PulumiCodeChooser -->
 
         # Set project level repository policy
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("exampleRepositoryPolicyReservedNames",
-            project_id=example_project.id,
+        example_repository_policy_reserved_names = azuredevops.RepositoryPolicyReservedNames("example",
+            project_id=example.id,
             enabled=True,
             blocking=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/resource_authorization.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/resource_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,27 +203,28 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_bit_bucket = azuredevops.ServiceEndpointBitBucket("exampleServiceEndpointBitBucket",
-            project_id=example_project.id,
+        example_service_endpoint_bit_bucket = azuredevops.ServiceEndpointBitBucket("example",
+            project_id=example.id,
             username="username",
             password="password",
             service_endpoint_name="example-bitbucket",
             description="Managed by Terraform")
-        example_resource_authorization = azuredevops.ResourceAuthorization("exampleResourceAuthorization",
-            project_id=example_project.id,
+        example_resource_authorization = azuredevops.ResourceAuthorization("example",
+            project_id=example.id,
             resource_id=example_service_endpoint_bit_bucket.id,
             authorized=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
@@ -251,27 +252,28 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_bit_bucket = azuredevops.ServiceEndpointBitBucket("exampleServiceEndpointBitBucket",
-            project_id=example_project.id,
+        example_service_endpoint_bit_bucket = azuredevops.ServiceEndpointBitBucket("example",
+            project_id=example.id,
             username="username",
             password="password",
             service_endpoint_name="example-bitbucket",
             description="Managed by Terraform")
-        example_resource_authorization = azuredevops.ResourceAuthorization("exampleResourceAuthorization",
-            project_id=example_project.id,
+        example_resource_authorization = azuredevops.ResourceAuthorization("example",
+            project_id=example.id,
             resource_id=example_service_endpoint_bit_bucket.id,
             authorized=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_artifactory.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_artifactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,21 +257,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_artifactory = azuredevops.ServiceEndpointArtifactory("exampleServiceEndpointArtifactory",
-            project_id=example_project.id,
+        example_service_endpoint_artifactory = azuredevops.ServiceEndpointArtifactory("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceEndpointArtifactoryAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -279,21 +280,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_artifactory = azuredevops.ServiceEndpointArtifactory("exampleServiceEndpointArtifactory",
-            project_id=example_project.id,
+        example_service_endpoint_artifactory = azuredevops.ServiceEndpointArtifactory("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceEndpointArtifactoryAuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
@@ -335,21 +337,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_artifactory = azuredevops.ServiceEndpointArtifactory("exampleServiceEndpointArtifactory",
-            project_id=example_project.id,
+        example_service_endpoint_artifactory = azuredevops.ServiceEndpointArtifactory("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceEndpointArtifactoryAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -357,21 +360,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_artifactory = azuredevops.ServiceEndpointArtifactory("exampleServiceEndpointArtifactory",
-            project_id=example_project.id,
+        example_service_endpoint_artifactory = azuredevops.ServiceEndpointArtifactory("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceEndpointArtifactoryAuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_aws.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,21 +349,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_aws = azuredevops.ServiceEndpointAws("exampleServiceEndpointAws",
-            project_id=example_project.id,
+        example_service_endpoint_aws = azuredevops.ServiceEndpointAws("example",
+            project_id=example.id,
             service_endpoint_name="Example AWS",
             access_key_id="00000000-0000-0000-0000-000000000000",
             secret_access_key="accesskey",
             description="Managed by AzureDevOps")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -403,21 +404,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_aws = azuredevops.ServiceEndpointAws("exampleServiceEndpointAws",
-            project_id=example_project.id,
+        example_service_endpoint_aws = azuredevops.ServiceEndpointAws("example",
+            project_id=example.id,
             service_endpoint_name="Example AWS",
             access_key_id="00000000-0000-0000-0000-000000000000",
             secret_access_key="accesskey",
             description="Managed by AzureDevOps")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_azure_dev_ops.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_dev_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,21 +253,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_azure_dev_ops = azuredevops.ServiceEndpointAzureDevOps("exampleServiceEndpointAzureDevOps",
-            project_id=example_project.id,
+        example_service_endpoint_azure_dev_ops = azuredevops.ServiceEndpointAzureDevOps("example",
+            project_id=example.id,
             service_endpoint_name="Example Azure DevOps",
             org_url="https://dev.azure.com/testorganization",
             release_api_url="https://vsrm.dev.azure.com/testorganization",
             personal_access_token="0000000000000000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
@@ -308,21 +309,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_azure_dev_ops = azuredevops.ServiceEndpointAzureDevOps("exampleServiceEndpointAzureDevOps",
-            project_id=example_project.id,
+        example_service_endpoint_azure_dev_ops = azuredevops.ServiceEndpointAzureDevOps("example",
+            project_id=example.id,
             service_endpoint_name="Example Azure DevOps",
             org_url="https://dev.azure.com/testorganization",
             release_api_url="https://vsrm.dev.azure.com/testorganization",
             personal_access_token="0000000000000000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_azure_ecr.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_ecr.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,22 +377,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
         # azure container registry service connection
-        example_service_endpoint_azure_ecr = azuredevops.ServiceEndpointAzureEcr("exampleServiceEndpointAzureEcr",
-            project_id=example_project.id,
+        example_service_endpoint_azure_ecr = azuredevops.ServiceEndpointAzureEcr("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureCR",
             resource_group="example-rg",
             azurecr_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurecr_name="ExampleAcr",
             azurecr_subscription_id="00000000-0000-0000-0000-000000000000",
             azurecr_subscription_name="subscription name")
         ```
@@ -433,22 +434,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
         # azure container registry service connection
-        example_service_endpoint_azure_ecr = azuredevops.ServiceEndpointAzureEcr("exampleServiceEndpointAzureEcr",
-            project_id=example_project.id,
+        example_service_endpoint_azure_ecr = azuredevops.ServiceEndpointAzureEcr("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureCR",
             resource_group="example-rg",
             azurecr_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurecr_name="ExampleAcr",
             azurecr_subscription_id="00000000-0000-0000-0000-000000000000",
             azurecr_subscription_name="subscription name")
         ```
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_azure_rm.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_azure_rm.py`

 * *Files 6% similar despite different names*

```diff
@@ -564,21 +564,22 @@
         ### Service Principal Manual AzureRM Service Endpoint (Subscription Scoped)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             description="Managed by Terraform",
             service_endpoint_authentication_scheme="ServicePrincipal",
             credentials=azuredevops.ServiceEndpointAzureRMCredentialsArgs(
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
@@ -591,21 +592,22 @@
         ### Service Principal Manual AzureRM Service Endpoint (ManagementGroup Scoped)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             description="Managed by Terraform",
             service_endpoint_authentication_scheme="ServicePrincipal",
             credentials=azuredevops.ServiceEndpointAzureRMCredentialsArgs(
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
@@ -618,41 +620,86 @@
         ### Service Principal Automatic AzureRM Service Endpoint
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="ServicePrincipal",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
         <!--End PulumiCodeChooser -->
 
+        ### Workload Identity Federation Manual AzureRM Service Endpoint (Subscription Scoped)
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_azure as azure
+        import pulumi_azuredevops as azuredevops
+
+        service_connection_name = "example-federated-sc"
+        example = azuredevops.Project("example",
+            name="Example Project",
+            visibility="private",
+            version_control="Git",
+            work_item_template="Agile",
+            description="Managed by Terraform")
+        identity = azure.core.ResourceGroup("identity",
+            name="identity",
+            location="UK South")
+        example_user_assigned_identity = azure.authorization.UserAssignedIdentity("example",
+            location=identity.location,
+            name="example-identity",
+            resource_group_name="azurerm_resource_group.identity.name")
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
+            service_endpoint_name=service_connection_name,
+            description="Managed by Terraform",
+            service_endpoint_authentication_scheme="WorkloadIdentityFederation",
+            credentials=azuredevops.ServiceEndpointAzureRMCredentialsArgs(
+                serviceprincipalid=example_user_assigned_identity.client_id,
+            ),
+            azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
+            azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
+            azurerm_subscription_name="Example Subscription Name")
+        example_federated_identity_credential = azure.armmsi.FederatedIdentityCredential("example",
+            name="example-federated-credential",
+            resource_group_name=identity.name,
+            parent_id=example_user_assigned_identity.id,
+            audience="api://AzureADTokenExchange",
+            issuer=example_service_endpoint_azure_rm.workload_identity_federation_issuer,
+            subject=example_service_endpoint_azure_rm.workload_identity_federation_subject)
+        ```
+        <!--End PulumiCodeChooser -->
+
         ### Workload Identity Federation Automatic AzureRM Service Endpoint
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="WorkloadIdentityFederation",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
         <!--End PulumiCodeChooser -->
@@ -660,20 +707,21 @@
         ### Managed Identity AzureRM Service Endpoint
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="ManagedServiceIdentity",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
         <!--End PulumiCodeChooser -->
@@ -730,21 +778,22 @@
         ### Service Principal Manual AzureRM Service Endpoint (Subscription Scoped)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             description="Managed by Terraform",
             service_endpoint_authentication_scheme="ServicePrincipal",
             credentials=azuredevops.ServiceEndpointAzureRMCredentialsArgs(
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
@@ -757,21 +806,22 @@
         ### Service Principal Manual AzureRM Service Endpoint (ManagementGroup Scoped)
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             description="Managed by Terraform",
             service_endpoint_authentication_scheme="ServicePrincipal",
             credentials=azuredevops.ServiceEndpointAzureRMCredentialsArgs(
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
@@ -784,41 +834,86 @@
         ### Service Principal Automatic AzureRM Service Endpoint
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="ServicePrincipal",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
         <!--End PulumiCodeChooser -->
 
+        ### Workload Identity Federation Manual AzureRM Service Endpoint (Subscription Scoped)
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_azure as azure
+        import pulumi_azuredevops as azuredevops
+
+        service_connection_name = "example-federated-sc"
+        example = azuredevops.Project("example",
+            name="Example Project",
+            visibility="private",
+            version_control="Git",
+            work_item_template="Agile",
+            description="Managed by Terraform")
+        identity = azure.core.ResourceGroup("identity",
+            name="identity",
+            location="UK South")
+        example_user_assigned_identity = azure.authorization.UserAssignedIdentity("example",
+            location=identity.location,
+            name="example-identity",
+            resource_group_name="azurerm_resource_group.identity.name")
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
+            service_endpoint_name=service_connection_name,
+            description="Managed by Terraform",
+            service_endpoint_authentication_scheme="WorkloadIdentityFederation",
+            credentials=azuredevops.ServiceEndpointAzureRMCredentialsArgs(
+                serviceprincipalid=example_user_assigned_identity.client_id,
+            ),
+            azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
+            azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
+            azurerm_subscription_name="Example Subscription Name")
+        example_federated_identity_credential = azure.armmsi.FederatedIdentityCredential("example",
+            name="example-federated-credential",
+            resource_group_name=identity.name,
+            parent_id=example_user_assigned_identity.id,
+            audience="api://AzureADTokenExchange",
+            issuer=example_service_endpoint_azure_rm.workload_identity_federation_issuer,
+            subject=example_service_endpoint_azure_rm.workload_identity_federation_subject)
+        ```
+        <!--End PulumiCodeChooser -->
+
         ### Workload Identity Federation Automatic AzureRM Service Endpoint
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="WorkloadIdentityFederation",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
         <!--End PulumiCodeChooser -->
@@ -826,20 +921,21 @@
         ### Managed Identity AzureRM Service Endpoint
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             service_endpoint_authentication_scheme="ManagedServiceIdentity",
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_bit_bucket.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_bit_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,21 +217,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_bit_bucket = azuredevops.ServiceEndpointBitBucket("exampleServiceEndpointBitBucket",
-            project_id=example_project.id,
+        example_service_endpoint_bit_bucket = azuredevops.ServiceEndpointBitBucket("example",
+            project_id=example.id,
             username="username",
             password="password",
             service_endpoint_name="Example Bitbucket",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -266,21 +267,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_bit_bucket = azuredevops.ServiceEndpointBitBucket("exampleServiceEndpointBitBucket",
-            project_id=example_project.id,
+        example_service_endpoint_bit_bucket = azuredevops.ServiceEndpointBitBucket("example",
+            project_id=example.id,
             username="username",
             password="password",
             service_endpoint_name="Example Bitbucket",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_docker_registry.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_docker_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,30 +316,31 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
         # dockerhub registry service connection
-        example_service_endpoint_docker_registry = azuredevops.ServiceEndpointDockerRegistry("exampleServiceEndpointDockerRegistry",
-            project_id=example_project.id,
+        example_service_endpoint_docker_registry = azuredevops.ServiceEndpointDockerRegistry("example",
+            project_id=example.id,
             service_endpoint_name="Example Docker Hub",
             docker_username="example",
             docker_email="email@example.com",
             docker_password="12345",
             registry_type="DockerHub")
         # other docker registry service connection
         example_other = azuredevops.ServiceEndpointDockerRegistry("example-other",
-            project_id=example_project.id,
+            project_id=example.id,
             service_endpoint_name="Example Docker Registry",
             docker_registry="https://sample.azurecr.io/v1",
             docker_username="sample",
             docker_password="12345",
             registry_type="Others")
         ```
         <!--End PulumiCodeChooser -->
@@ -379,30 +380,31 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
         # dockerhub registry service connection
-        example_service_endpoint_docker_registry = azuredevops.ServiceEndpointDockerRegistry("exampleServiceEndpointDockerRegistry",
-            project_id=example_project.id,
+        example_service_endpoint_docker_registry = azuredevops.ServiceEndpointDockerRegistry("example",
+            project_id=example.id,
             service_endpoint_name="Example Docker Hub",
             docker_username="example",
             docker_email="email@example.com",
             docker_password="12345",
             registry_type="DockerHub")
         # other docker registry service connection
         example_other = azuredevops.ServiceEndpointDockerRegistry("example-other",
-            project_id=example_project.id,
+            project_id=example.id,
             service_endpoint_name="Example Docker Registry",
             docker_registry="https://sample.azurecr.io/v1",
             docker_username="sample",
             docker_password="12345",
             registry_type="Others")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_generic.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,21 +252,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("exampleServiceEndpointGeneric",
-            project_id=example_project.id,
+        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
+            project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
@@ -306,21 +307,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("exampleServiceEndpointGeneric",
-            project_id=example_project.id,
+        example_service_endpoint_generic = azuredevops.ServiceEndpointGeneric("example",
+            project_id=example.id,
             server_url="https://some-server.example.com",
             username="username",
             password="password",
             service_endpoint_name="Example Generic",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_generic_git.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_generic_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,21 +293,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_generic_git = azuredevops.ServiceEndpointGenericGit("exampleServiceEndpointGenericGit",
-            project_id=example_project.id,
+        example_service_endpoint_generic_git = azuredevops.ServiceEndpointGenericGit("example",
+            project_id=example.id,
             repository_url="https://dev.azure.com/org/project/_git/repository",
             username="username",
             password="password",
             service_endpoint_name="Example Generic Git",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
@@ -350,21 +351,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_generic_git = azuredevops.ServiceEndpointGenericGit("exampleServiceEndpointGenericGit",
-            project_id=example_project.id,
+        example_service_endpoint_generic_git = azuredevops.ServiceEndpointGenericGit("example",
+            project_id=example.id,
             repository_url="https://dev.azure.com/org/project/_git/repository",
             username="username",
             password="password",
             service_endpoint_name="Example Generic Git",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_git_hub.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_git_hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,59 +213,62 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("exampleServiceEndpointGitHub",
-            project_id=example_project.id,
+        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
+            project_id=example.id,
             service_endpoint_name="Example GitHub Personal Access Token",
             auth_personal=azuredevops.ServiceEndpointGitHubAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("exampleServiceEndpointGitHub",
-            project_id=example_project.id,
+        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
+            project_id=example.id,
             service_endpoint_name="Example GitHub",
             auth_oauth=azuredevops.ServiceEndpointGitHubAuthOauthArgs(
                 oauth_configuration_id="00000000-0000-0000-0000-000000000000",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("exampleServiceEndpointGitHub",
-            project_id=example_project.id,
+        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
+            project_id=example.id,
             service_endpoint_name="Example GitHub Apps: Azure Pipelines",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
@@ -297,59 +300,62 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("exampleServiceEndpointGitHub",
-            project_id=example_project.id,
+        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
+            project_id=example.id,
             service_endpoint_name="Example GitHub Personal Access Token",
             auth_personal=azuredevops.ServiceEndpointGitHubAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("exampleServiceEndpointGitHub",
-            project_id=example_project.id,
+        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
+            project_id=example.id,
             service_endpoint_name="Example GitHub",
             auth_oauth=azuredevops.ServiceEndpointGitHubAuthOauthArgs(
                 oauth_configuration_id="00000000-0000-0000-0000-000000000000",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("exampleServiceEndpointGitHub",
-            project_id=example_project.id,
+        example_service_endpoint_git_hub = azuredevops.ServiceEndpointGitHub("example",
+            project_id=example.id,
             service_endpoint_name="Example GitHub Apps: Azure Pipelines",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,21 +211,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_git_hub_enterprise = azuredevops.ServiceEndpointGitHubEnterprise("exampleServiceEndpointGitHubEnterprise",
-            project_id=example_project.id,
+        example_service_endpoint_git_hub_enterprise = azuredevops.ServiceEndpointGitHubEnterprise("example",
+            project_id=example.id,
             service_endpoint_name="Example GitHub Enterprise",
             url="https://github.contoso.com",
             description="Managed by Terraform",
             auth_personal=azuredevops.ServiceEndpointGitHubEnterpriseAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ))
         ```
@@ -261,21 +262,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_git_hub_enterprise = azuredevops.ServiceEndpointGitHubEnterprise("exampleServiceEndpointGitHubEnterprise",
-            project_id=example_project.id,
+        example_service_endpoint_git_hub_enterprise = azuredevops.ServiceEndpointGitHubEnterprise("example",
+            project_id=example.id,
             service_endpoint_name="Example GitHub Enterprise",
             url="https://github.contoso.com",
             description="Managed by Terraform",
             auth_personal=azuredevops.ServiceEndpointGitHubEnterpriseAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ))
         ```
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_kubernetes.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_kubernetes.py`

 * *Files 14% similar despite different names*

```diff
@@ -311,14 +311,86 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  service_account: Optional[pulumi.Input[pulumi.InputType['ServiceEndpointKubernetesServiceAccountArgs']]] = None,
                  service_endpoint_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Kubernetes service endpoint within Azure DevOps.
 
+        ## Example Usage
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_azuredevops as azuredevops
+
+        example = azuredevops.Project("example",
+            name="Example Project",
+            visibility="private",
+            version_control="Git",
+            work_item_template="Agile",
+            description="Managed by Terraform")
+        example_azure = azuredevops.ServiceEndpointKubernetes("example-azure",
+            project_id=example.id,
+            service_endpoint_name="Example Kubernetes",
+            apiserver_url="https://sample-kubernetes-cluster.hcp.westeurope.azmk8s.io",
+            authorization_type="AzureSubscription",
+            azure_subscriptions=[azuredevops.ServiceEndpointKubernetesAzureSubscriptionArgs(
+                subscription_id="00000000-0000-0000-0000-000000000000",
+                subscription_name="Example",
+                tenant_id="00000000-0000-0000-0000-000000000000",
+                resourcegroup_id="example-rg",
+                namespace="default",
+                cluster_name="example-aks",
+            )])
+        example_kubeconfig = azuredevops.ServiceEndpointKubernetes("example-kubeconfig",
+            project_id=example.id,
+            service_endpoint_name="Example Kubernetes",
+            apiserver_url="https://sample-kubernetes-cluster.hcp.westeurope.azmk8s.io",
+            authorization_type="Kubeconfig",
+            kubeconfig=azuredevops.ServiceEndpointKubernetesKubeconfigArgs(
+                kube_config=\"\"\"                              apiVersion: v1
+                                      clusters:
+                                      - cluster:
+                                          certificate-authority: fake-ca-file
+                                          server: https://1.2.3.4
+                                        name: development
+                                      contexts:
+                                      - context:
+                                          cluster: development
+                                          namespace: frontend
+                                          user: developer
+                                        name: dev-frontend
+                                      current-context: dev-frontend
+                                      kind: Config
+                                      preferences: {}
+                                      users:
+                                      - name: developer
+                                        user:
+                                          client-certificate: fake-cert-file
+                                          client-key: fake-key-file
+        \"\"\",
+                accept_untrusted_certs=True,
+                cluster_context="dev-frontend",
+            ))
+        example_service_account = azuredevops.ServiceEndpointKubernetes("example-service-account",
+            project_id=example.id,
+            service_endpoint_name="Example Kubernetes",
+            apiserver_url="https://sample-kubernetes-cluster.hcp.westeurope.azmk8s.io",
+            authorization_type="ServiceAccount",
+            service_account=azuredevops.ServiceEndpointKubernetesServiceAccountArgs(
+                token="000000000000000000000000",
+                ca_cert="0000000000000000000000000000000",
+            ))
+        ```
+        <!--End PulumiCodeChooser -->
+
+        ## Relevant Links
+
+        - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
+
         ## Import
 
         Azure DevOps Service Endpoint Kubernetes can be imported using **projectID/serviceEndpointID** or **projectName/serviceEndpointID**
 
         ```sh
         $ pulumi import azuredevops:index/serviceEndpointKubernetes:ServiceEndpointKubernetes example 00000000-0000-0000-0000-000000000000/00000000-0000-0000-0000-000000000000
         ```
@@ -338,14 +410,86 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceEndpointKubernetesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Kubernetes service endpoint within Azure DevOps.
 
+        ## Example Usage
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_azuredevops as azuredevops
+
+        example = azuredevops.Project("example",
+            name="Example Project",
+            visibility="private",
+            version_control="Git",
+            work_item_template="Agile",
+            description="Managed by Terraform")
+        example_azure = azuredevops.ServiceEndpointKubernetes("example-azure",
+            project_id=example.id,
+            service_endpoint_name="Example Kubernetes",
+            apiserver_url="https://sample-kubernetes-cluster.hcp.westeurope.azmk8s.io",
+            authorization_type="AzureSubscription",
+            azure_subscriptions=[azuredevops.ServiceEndpointKubernetesAzureSubscriptionArgs(
+                subscription_id="00000000-0000-0000-0000-000000000000",
+                subscription_name="Example",
+                tenant_id="00000000-0000-0000-0000-000000000000",
+                resourcegroup_id="example-rg",
+                namespace="default",
+                cluster_name="example-aks",
+            )])
+        example_kubeconfig = azuredevops.ServiceEndpointKubernetes("example-kubeconfig",
+            project_id=example.id,
+            service_endpoint_name="Example Kubernetes",
+            apiserver_url="https://sample-kubernetes-cluster.hcp.westeurope.azmk8s.io",
+            authorization_type="Kubeconfig",
+            kubeconfig=azuredevops.ServiceEndpointKubernetesKubeconfigArgs(
+                kube_config=\"\"\"                              apiVersion: v1
+                                      clusters:
+                                      - cluster:
+                                          certificate-authority: fake-ca-file
+                                          server: https://1.2.3.4
+                                        name: development
+                                      contexts:
+                                      - context:
+                                          cluster: development
+                                          namespace: frontend
+                                          user: developer
+                                        name: dev-frontend
+                                      current-context: dev-frontend
+                                      kind: Config
+                                      preferences: {}
+                                      users:
+                                      - name: developer
+                                        user:
+                                          client-certificate: fake-cert-file
+                                          client-key: fake-key-file
+        \"\"\",
+                accept_untrusted_certs=True,
+                cluster_context="dev-frontend",
+            ))
+        example_service_account = azuredevops.ServiceEndpointKubernetes("example-service-account",
+            project_id=example.id,
+            service_endpoint_name="Example Kubernetes",
+            apiserver_url="https://sample-kubernetes-cluster.hcp.westeurope.azmk8s.io",
+            authorization_type="ServiceAccount",
+            service_account=azuredevops.ServiceEndpointKubernetesServiceAccountArgs(
+                token="000000000000000000000000",
+                ca_cert="0000000000000000000000000000000",
+            ))
+        ```
+        <!--End PulumiCodeChooser -->
+
+        ## Relevant Links
+
+        - [Azure DevOps Service REST API 7.0 - Endpoints](https://docs.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints?view=azure-devops-rest-7.0)
+
         ## Import
 
         Azure DevOps Service Endpoint Kubernetes can be imported using **projectID/serviceEndpointID** or **projectName/serviceEndpointID**
 
         ```sh
         $ pulumi import azuredevops:index/serviceEndpointKubernetes:ServiceEndpointKubernetes example 00000000-0000-0000-0000-000000000000/00000000-0000-0000-0000-000000000000
         ```
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_npm.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_npm.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,21 +225,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_npm = azuredevops.ServiceEndpointNpm("exampleServiceEndpointNpm",
-            project_id=example_project.id,
+        example_service_endpoint_npm = azuredevops.ServiceEndpointNpm("example",
+            project_id=example.id,
             service_endpoint_name="Example npm",
             url="https://registry.npmjs.org",
             access_token="00000000-0000-0000-0000-000000000000",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -277,21 +278,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_npm = azuredevops.ServiceEndpointNpm("exampleServiceEndpointNpm",
-            project_id=example_project.id,
+        example_service_endpoint_npm = azuredevops.ServiceEndpointNpm("example",
+            project_id=example.id,
             service_endpoint_name="Example npm",
             url="https://registry.npmjs.org",
             access_token="00000000-0000-0000-0000-000000000000",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_pipeline.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,21 +219,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_pipeline = azuredevops.ServiceEndpointPipeline("exampleServiceEndpointPipeline",
-            project_id=example_project.id,
+        example_service_endpoint_pipeline = azuredevops.ServiceEndpointPipeline("example",
+            project_id=example.id,
             service_endpoint_name="Example Pipeline Runner",
             organization_name="Organization Name",
             auth_personal=azuredevops.ServiceEndpointPipelineAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
             description="Managed by Terraform")
         ```
@@ -270,21 +271,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_pipeline = azuredevops.ServiceEndpointPipeline("exampleServiceEndpointPipeline",
-            project_id=example_project.id,
+        example_service_endpoint_pipeline = azuredevops.ServiceEndpointPipeline("example",
+            project_id=example.id,
             service_endpoint_name="Example Pipeline Runner",
             organization_name="Organization Name",
             auth_personal=azuredevops.ServiceEndpointPipelineAuthPersonalArgs(
                 personal_access_token="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
             description="Managed by Terraform")
         ```
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_service_fabric.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_service_fabric.py`

 * *Files 10% similar despite different names*

```diff
@@ -257,49 +257,23 @@
                  service_endpoint_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Service Fabric service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        ### Client Certificate Authentication
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import base64
-        import pulumi_azuredevops as azuredevops
-
-        example_project = azuredevops.Project("exampleProject",
-            visibility="private",
-            version_control="Git",
-            work_item_template="Agile",
-            description="Managed by Terraform")
-        example_service_endpoint_service_fabric = azuredevops.ServiceEndpointServiceFabric("exampleServiceEndpointServiceFabric",
-            project_id=example_project.id,
-            service_endpoint_name="Example Service Fabric",
-            description="Managed by Terraform",
-            cluster_endpoint="tcp://test",
-            certificate=azuredevops.ServiceEndpointServiceFabricCertificateArgs(
-                server_certificate_lookup="Thumbprint",
-                server_certificate_thumbprint="0000000000000000000000000000000000000000",
-                client_certificate=(lambda path: base64.b64encode(open(path).read().encode()).decode())("certificate.pfx"),
-                client_certificate_password="password",
-            ))
-        ```
-        <!--End PulumiCodeChooser -->
-
         ### Azure Active Directory Authentication
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
+            name="Sample Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
         test = azuredevops.ServiceEndpointServiceFabric("test",
             project_id=project.id,
             service_endpoint_name="Sample Service Fabric",
             description="Managed by Terraform",
@@ -317,14 +291,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
+            name="Sample Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
         test = azuredevops.ServiceEndpointServiceFabric("test",
             project_id=project.id,
             service_endpoint_name="Sample Service Fabric",
             description="Managed by Terraform",
@@ -361,49 +336,23 @@
                  args: ServiceEndpointServiceFabricArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Service Fabric service endpoint within Azure DevOps.
 
         ## Example Usage
 
-        ### Client Certificate Authentication
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import base64
-        import pulumi_azuredevops as azuredevops
-
-        example_project = azuredevops.Project("exampleProject",
-            visibility="private",
-            version_control="Git",
-            work_item_template="Agile",
-            description="Managed by Terraform")
-        example_service_endpoint_service_fabric = azuredevops.ServiceEndpointServiceFabric("exampleServiceEndpointServiceFabric",
-            project_id=example_project.id,
-            service_endpoint_name="Example Service Fabric",
-            description="Managed by Terraform",
-            cluster_endpoint="tcp://test",
-            certificate=azuredevops.ServiceEndpointServiceFabricCertificateArgs(
-                server_certificate_lookup="Thumbprint",
-                server_certificate_thumbprint="0000000000000000000000000000000000000000",
-                client_certificate=(lambda path: base64.b64encode(open(path).read().encode()).decode())("certificate.pfx"),
-                client_certificate_password="password",
-            ))
-        ```
-        <!--End PulumiCodeChooser -->
-
         ### Azure Active Directory Authentication
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
+            name="Sample Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
         test = azuredevops.ServiceEndpointServiceFabric("test",
             project_id=project.id,
             service_endpoint_name="Sample Service Fabric",
             description="Managed by Terraform",
@@ -421,14 +370,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
+            name="Sample Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
         test = azuredevops.ServiceEndpointServiceFabric("test",
             project_id=project.id,
             service_endpoint_name="Sample Service Fabric",
             description="Managed by Terraform",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_sonar_cloud.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_sonar_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,21 +193,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_sonar_cloud = azuredevops.ServiceEndpointSonarCloud("exampleServiceEndpointSonarCloud",
-            project_id=example_project.id,
+        example_service_endpoint_sonar_cloud = azuredevops.ServiceEndpointSonarCloud("example",
+            project_id=example.id,
             service_endpoint_name="Example SonarCloud",
             token="0000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
@@ -243,21 +244,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_sonar_cloud = azuredevops.ServiceEndpointSonarCloud("exampleServiceEndpointSonarCloud",
-            project_id=example_project.id,
+        example_service_endpoint_sonar_cloud = azuredevops.ServiceEndpointSonarCloud("example",
+            project_id=example.id,
             service_endpoint_name="Example SonarCloud",
             token="0000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_sonar_qube.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_sonar_qube.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,21 +225,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_sonar_qube = azuredevops.ServiceEndpointSonarQube("exampleServiceEndpointSonarQube",
-            project_id=example_project.id,
+        example_service_endpoint_sonar_qube = azuredevops.ServiceEndpointSonarQube("example",
+            project_id=example.id,
             service_endpoint_name="Example SonarQube",
             url="https://sonarqube.my.com",
             token="0000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -277,21 +278,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_sonar_qube = azuredevops.ServiceEndpointSonarQube("exampleServiceEndpointSonarQube",
-            project_id=example_project.id,
+        example_service_endpoint_sonar_qube = azuredevops.ServiceEndpointSonarQube("example",
+            project_id=example.id,
             service_endpoint_name="Example SonarQube",
             url="https://sonarqube.my.com",
             token="0000000000000000000000000000000000000000",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/service_endpoint_ssh.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/service_endpoint_ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,21 +316,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_ssh = azuredevops.ServiceEndpointSsh("exampleServiceEndpointSsh",
-            project_id=example_project.id,
+        example_service_endpoint_ssh = azuredevops.ServiceEndpointSsh("example",
+            project_id=example.id,
             service_endpoint_name="Example SSH",
             host="1.2.3.4",
             username="username",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -370,21 +371,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_service_endpoint_ssh = azuredevops.ServiceEndpointSsh("exampleServiceEndpointSsh",
-            project_id=example_project.id,
+        example_service_endpoint_ssh = azuredevops.ServiceEndpointSsh("example",
+            project_id=example.id,
             service_endpoint_name="Example SSH",
             host="1.2.3.4",
             username="username",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_argocd.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_argocd.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,20 +269,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_serviceendpoint_argocd = azuredevops.ServiceendpointArgocd("exampleServiceendpointArgocd",
-            project_id=example_project.id,
+        example_serviceendpoint_argocd = azuredevops.ServiceendpointArgocd("example",
+            project_id=example.id,
             service_endpoint_name="Example ArgoCD",
             description="Managed by Terraform",
             url="https://argocd.my.com",
             authentication_token=azuredevops.ServiceendpointArgocdAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -290,21 +291,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_argocd = azuredevops.ServiceendpointArgocd("exampleServiceendpointArgocd",
-            project_id=example_project.id,
+        example_serviceendpoint_argocd = azuredevops.ServiceendpointArgocd("example",
+            project_id=example.id,
             service_endpoint_name="Example ArgoCD",
             description="Managed by Terraform",
             url="https://argocd.my.com",
             authentication_basic=azuredevops.ServiceendpointArgocdAuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
@@ -347,20 +349,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
-        example_serviceendpoint_argocd = azuredevops.ServiceendpointArgocd("exampleServiceendpointArgocd",
-            project_id=example_project.id,
+        example_serviceendpoint_argocd = azuredevops.ServiceendpointArgocd("example",
+            project_id=example.id,
             service_endpoint_name="Example ArgoCD",
             description="Managed by Terraform",
             url="https://argocd.my.com",
             authentication_token=azuredevops.ServiceendpointArgocdAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -368,21 +371,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_argocd = azuredevops.ServiceendpointArgocd("exampleServiceendpointArgocd",
-            project_id=example_project.id,
+        example_serviceendpoint_argocd = azuredevops.ServiceendpointArgocd("example",
+            project_id=example.id,
             service_endpoint_name="Example ArgoCD",
             description="Managed by Terraform",
             url="https://argocd.my.com",
             authentication_basic=azuredevops.ServiceendpointArgocdAuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_externaltfs.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_externaltfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_gcp_terraform.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_gcp_terraform.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,21 +313,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_gcp_terraform = azuredevops.ServiceendpointGcpTerraform("exampleServiceendpointGcpTerraform",
-            project_id=example_project.id,
+        example_serviceendpoint_gcp_terraform = azuredevops.ServiceendpointGcpTerraform("example",
+            project_id=example.id,
             token_uri="https://oauth2.example.com/token",
             client_email="gcp-sa-example@example.iam.gserviceaccount.com",
             private_key="0000000000000000000000000000000000000",
             service_endpoint_name="Example GCP Terraform extension",
             gcp_project_id="Example GCP Project",
             description="Managed by Terraform")
         ```
@@ -365,21 +366,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_gcp_terraform = azuredevops.ServiceendpointGcpTerraform("exampleServiceendpointGcpTerraform",
-            project_id=example_project.id,
+        example_serviceendpoint_gcp_terraform = azuredevops.ServiceendpointGcpTerraform("example",
+            project_id=example.id,
             token_uri="https://oauth2.example.com/token",
             client_email="gcp-sa-example@example.iam.gserviceaccount.com",
             private_key="0000000000000000000000000000000000000",
             service_endpoint_name="Example GCP Terraform extension",
             gcp_project_id="Example GCP Project",
             description="Managed by Terraform")
         ```
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_incomingwebhook.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_incomingwebhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,21 +251,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_incomingwebhook = azuredevops.ServiceendpointIncomingwebhook("exampleServiceendpointIncomingwebhook",
-            project_id=example_project.id,
+        example_serviceendpoint_incomingwebhook = azuredevops.ServiceendpointIncomingwebhook("example",
+            project_id=example.id,
             webhook_name="example_webhook",
             secret="secret",
             http_header="X-Hub-Signature",
             service_endpoint_name="Example IncomingWebhook",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
@@ -298,21 +299,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_incomingwebhook = azuredevops.ServiceendpointIncomingwebhook("exampleServiceendpointIncomingwebhook",
-            project_id=example_project.id,
+        example_serviceendpoint_incomingwebhook = azuredevops.ServiceendpointIncomingwebhook("example",
+            project_id=example.id,
             webhook_name="example_webhook",
             secret="secret",
             http_header="X-Hub-Signature",
             service_endpoint_name="Example IncomingWebhook",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_jenkins.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jenkins.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,21 +282,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jenkins = azuredevops.ServiceendpointJenkins("exampleServiceendpointJenkins",
-            project_id=example_project.id,
+        example_serviceendpoint_jenkins = azuredevops.ServiceendpointJenkins("example",
+            project_id=example.id,
             service_endpoint_name="jenkins-example",
             description="Service Endpoint for 'Jenkins' (Managed by Terraform)",
             url="https://example.com",
             accept_untrusted_certs=False,
             username="username",
             password="password")
         ```
@@ -331,21 +332,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jenkins = azuredevops.ServiceendpointJenkins("exampleServiceendpointJenkins",
-            project_id=example_project.id,
+        example_serviceendpoint_jenkins = azuredevops.ServiceendpointJenkins("example",
+            project_id=example.id,
             service_endpoint_name="jenkins-example",
             description="Service Endpoint for 'Jenkins' (Managed by Terraform)",
             url="https://example.com",
             accept_untrusted_certs=False,
             username="username",
             password="password")
         ```
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,21 +271,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_artifactory_v2 = azuredevops.ServiceendpointJfrogArtifactoryV2("exampleServiceendpointJfrogArtifactoryV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_artifactory_v2 = azuredevops.ServiceendpointJfrogArtifactoryV2("example",
+            project_id=example.id,
             service_endpoint_name="Example JFrog Artifactory V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogArtifactoryV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -293,21 +294,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_artifactory_v2 = azuredevops.ServiceendpointJfrogArtifactoryV2("exampleServiceendpointJfrogArtifactoryV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_artifactory_v2 = azuredevops.ServiceendpointJfrogArtifactoryV2("example",
+            project_id=example.id,
             service_endpoint_name="Example JFrog Artifactory V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogArtifactoryV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
@@ -352,21 +354,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_artifactory_v2 = azuredevops.ServiceendpointJfrogArtifactoryV2("exampleServiceendpointJfrogArtifactoryV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_artifactory_v2 = azuredevops.ServiceendpointJfrogArtifactoryV2("example",
+            project_id=example.id,
             service_endpoint_name="Example JFrog Artifactory V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogArtifactoryV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -374,21 +377,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_artifactory_v2 = azuredevops.ServiceendpointJfrogArtifactoryV2("exampleServiceendpointJfrogArtifactoryV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_artifactory_v2 = azuredevops.ServiceendpointJfrogArtifactoryV2("example",
+            project_id=example.id,
             service_endpoint_name="Example JFrog Artifactory V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogArtifactoryV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,21 +271,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_distribution_v2 = azuredevops.ServiceendpointJfrogDistributionV2("exampleServiceendpointJfrogDistributionV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_distribution_v2 = azuredevops.ServiceendpointJfrogDistributionV2("example",
+            project_id=example.id,
             service_endpoint_name="Example JFrog Distribution V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogDistributionV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -293,21 +294,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_distribution_v2 = azuredevops.ServiceendpointJfrogDistributionV2("exampleServiceendpointJfrogDistributionV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_distribution_v2 = azuredevops.ServiceendpointJfrogDistributionV2("example",
+            project_id=example.id,
             service_endpoint_name="Example JFrog Distribution V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogDistributionV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
@@ -352,21 +354,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_distribution_v2 = azuredevops.ServiceendpointJfrogDistributionV2("exampleServiceendpointJfrogDistributionV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_distribution_v2 = azuredevops.ServiceendpointJfrogDistributionV2("example",
+            project_id=example.id,
             service_endpoint_name="Example JFrog Distribution V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogDistributionV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -374,21 +377,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_distribution_v2 = azuredevops.ServiceendpointJfrogDistributionV2("exampleServiceendpointJfrogDistributionV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_distribution_v2 = azuredevops.ServiceendpointJfrogDistributionV2("example",
+            project_id=example.id,
             service_endpoint_name="Example JFrog Distribution V2",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogDistributionV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,21 +271,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_platform_v2 = azuredevops.ServiceendpointJfrogPlatformV2("exampleServiceendpointJfrogPlatformV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_platform_v2 = azuredevops.ServiceendpointJfrogPlatformV2("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogPlatformV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -293,21 +294,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_platform_v2 = azuredevops.ServiceendpointJfrogPlatformV2("exampleServiceendpointJfrogPlatformV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_platform_v2 = azuredevops.ServiceendpointJfrogPlatformV2("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogPlatformV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
@@ -352,21 +354,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_platform_v2 = azuredevops.ServiceendpointJfrogPlatformV2("exampleServiceendpointJfrogPlatformV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_platform_v2 = azuredevops.ServiceendpointJfrogPlatformV2("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogPlatformV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -374,21 +377,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_platform_v2 = azuredevops.ServiceendpointJfrogPlatformV2("exampleServiceendpointJfrogPlatformV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_platform_v2 = azuredevops.ServiceendpointJfrogPlatformV2("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogPlatformV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,21 +271,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_xray_v2 = azuredevops.ServiceendpointJfrogXrayV2("exampleServiceendpointJfrogXrayV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_xray_v2 = azuredevops.ServiceendpointJfrogXrayV2("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogXrayV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -293,21 +294,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_xray_v2 = azuredevops.ServiceendpointJfrogXrayV2("exampleServiceendpointJfrogXrayV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_xray_v2 = azuredevops.ServiceendpointJfrogXrayV2("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogXrayV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
@@ -352,21 +354,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_xray_v2 = azuredevops.ServiceendpointJfrogXrayV2("exampleServiceendpointJfrogXrayV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_xray_v2 = azuredevops.ServiceendpointJfrogXrayV2("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_token=azuredevops.ServiceendpointJfrogXrayV2AuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
         ```
@@ -374,21 +377,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_jfrog_xray_v2 = azuredevops.ServiceendpointJfrogXrayV2("exampleServiceendpointJfrogXrayV2",
-            project_id=example_project.id,
+        example_serviceendpoint_jfrog_xray_v2 = azuredevops.ServiceendpointJfrogXrayV2("example",
+            project_id=example.id,
             service_endpoint_name="Example Artifactory",
             description="Managed by Terraform",
             url="https://artifactory.my.com",
             authentication_basic=azuredevops.ServiceendpointJfrogXrayV2AuthenticationBasicArgs(
                 username="username",
                 password="password",
             ))
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_maven.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_maven.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,21 +285,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_maven = azuredevops.ServiceendpointMaven("exampleServiceendpointMaven",
-            project_id=example_project.id,
+        example_serviceendpoint_maven = azuredevops.ServiceendpointMaven("example",
+            project_id=example.id,
             service_endpoint_name="maven-example",
             description="Service Endpoint for 'Maven' (Managed by Terraform)",
             url="https://example.com",
             repository_id="example",
             authentication_token=azuredevops.ServiceendpointMavenAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
@@ -309,21 +310,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_maven = azuredevops.ServiceendpointMaven("exampleServiceendpointMaven",
-            project_id=example_project.id,
+        example_serviceendpoint_maven = azuredevops.ServiceendpointMaven("example",
+            project_id=example.id,
             service_endpoint_name="maven-example",
             description="Service Endpoint for 'Maven' (Managed by Terraform)",
             url="https://example.com",
             repository_id="example",
             authentication_basic=azuredevops.ServiceendpointMavenAuthenticationBasicArgs(
                 username="username",
                 password="password",
@@ -360,21 +362,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_maven = azuredevops.ServiceendpointMaven("exampleServiceendpointMaven",
-            project_id=example_project.id,
+        example_serviceendpoint_maven = azuredevops.ServiceendpointMaven("example",
+            project_id=example.id,
             service_endpoint_name="maven-example",
             description="Service Endpoint for 'Maven' (Managed by Terraform)",
             url="https://example.com",
             repository_id="example",
             authentication_token=azuredevops.ServiceendpointMavenAuthenticationTokenArgs(
                 token="0000000000000000000000000000000000000000",
             ))
@@ -384,21 +387,22 @@
         Alternatively a username and password may be used.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_maven = azuredevops.ServiceendpointMaven("exampleServiceendpointMaven",
-            project_id=example_project.id,
+        example_serviceendpoint_maven = azuredevops.ServiceendpointMaven("example",
+            project_id=example.id,
             service_endpoint_name="maven-example",
             description="Service Endpoint for 'Maven' (Managed by Terraform)",
             url="https://example.com",
             repository_id="example",
             authentication_basic=azuredevops.ServiceendpointMavenAuthenticationBasicArgs(
                 username="username",
                 password="password",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_nexus.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_nexus.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,21 +250,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_nexus = azuredevops.ServiceendpointNexus("exampleServiceendpointNexus",
-            project_id=example_project.id,
+        example_serviceendpoint_nexus = azuredevops.ServiceendpointNexus("example",
+            project_id=example.id,
             service_endpoint_name="nexus-example",
             description="Service Endpoint for 'Nexus IQ' (Managed by Terraform)",
             url="https://example.com",
             username="username",
             password="password")
         ```
         <!--End PulumiCodeChooser -->
@@ -298,21 +299,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_nexus = azuredevops.ServiceendpointNexus("exampleServiceendpointNexus",
-            project_id=example_project.id,
+        example_serviceendpoint_nexus = azuredevops.ServiceendpointNexus("example",
+            project_id=example.id,
             service_endpoint_name="nexus-example",
             description="Service Endpoint for 'Nexus IQ' (Managed by Terraform)",
             url="https://example.com",
             username="username",
             password="password")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_nuget.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_nuget.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,21 +325,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_nuget = azuredevops.ServiceendpointNuget("exampleServiceendpointNuget",
-            project_id=example_project.id,
+        example_serviceendpoint_nuget = azuredevops.ServiceendpointNuget("example",
+            project_id=example.id,
             api_key="apikey",
             service_endpoint_name="Example NuGet",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
@@ -378,21 +379,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_nuget = azuredevops.ServiceendpointNuget("exampleServiceendpointNuget",
-            project_id=example_project.id,
+        example_serviceendpoint_nuget = azuredevops.ServiceendpointNuget("example",
+            project_id=example.id,
             api_key="apikey",
             service_endpoint_name="Example NuGet",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_octopusdeploy.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_octopusdeploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,21 +250,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_octopusdeploy = azuredevops.ServiceendpointOctopusdeploy("exampleServiceendpointOctopusdeploy",
-            project_id=example_project.id,
+        example_serviceendpoint_octopusdeploy = azuredevops.ServiceendpointOctopusdeploy("example",
+            project_id=example.id,
             url="https://octopus.com",
             api_key="000000000000000000000000000000000000",
             service_endpoint_name="Example Octopus Deploy",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
 
@@ -300,21 +301,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             visibility="private",
             version_control="Git",
             work_item_template="Agile",
             description="Managed by Terraform")
-        example_serviceendpoint_octopusdeploy = azuredevops.ServiceendpointOctopusdeploy("exampleServiceendpointOctopusdeploy",
-            project_id=example_project.id,
+        example_serviceendpoint_octopusdeploy = azuredevops.ServiceendpointOctopusdeploy("example",
+            project_id=example.id,
             url="https://octopus.com",
             api_key="000000000000000000000000000000000000",
             service_endpoint_name="Example Octopus Deploy",
             description="Managed by Terraform")
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/serviceendpoint_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/serviceendpoint_permissions.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,40 +240,41 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_root_permissions = azuredevops.ServiceendpointPermissions("example-root-permissions",
-            project_id=example_project.id,
+            project_id=example.id,
             principal=example_readers.id,
             permissions={
                 "Use": "allow",
                 "Administer": "allow",
                 "Create": "allow",
                 "ViewAuthorization": "allow",
                 "ViewEndpoint": "allow",
             })
-        example_service_endpoint_docker_registry = azuredevops.ServiceEndpointDockerRegistry("exampleServiceEndpointDockerRegistry",
-            project_id=example_project.id,
+        example_service_endpoint_docker_registry = azuredevops.ServiceEndpointDockerRegistry("example",
+            project_id=example.id,
             service_endpoint_name="Example Docker Hub",
             docker_username="username",
             docker_email="email@example.com",
             docker_password="password",
             registry_type="DockerHub")
         example_permissions = azuredevops.ServiceendpointPermissions("example-permissions",
-            project_id=example_project.id,
+            project_id=example.id,
             principal=example_readers.id,
             serviceendpoint_id=example_service_endpoint_docker_registry.id,
             permissions={
                 "Use": "allow",
                 "Administer": "deny",
                 "Create": "deny",
                 "ViewAuthorization": "allow",
@@ -329,40 +330,41 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_root_permissions = azuredevops.ServiceendpointPermissions("example-root-permissions",
-            project_id=example_project.id,
+            project_id=example.id,
             principal=example_readers.id,
             permissions={
                 "Use": "allow",
                 "Administer": "allow",
                 "Create": "allow",
                 "ViewAuthorization": "allow",
                 "ViewEndpoint": "allow",
             })
-        example_service_endpoint_docker_registry = azuredevops.ServiceEndpointDockerRegistry("exampleServiceEndpointDockerRegistry",
-            project_id=example_project.id,
+        example_service_endpoint_docker_registry = azuredevops.ServiceEndpointDockerRegistry("example",
+            project_id=example.id,
             service_endpoint_name="Example Docker Hub",
             docker_username="username",
             docker_email="email@example.com",
             docker_password="password",
             registry_type="DockerHub")
         example_permissions = azuredevops.ServiceendpointPermissions("example-permissions",
-            project_id=example_project.id,
+            project_id=example.id,
             principal=example_readers.id,
             serviceendpoint_id=example_service_endpoint_docker_registry.id,
             permissions={
                 "Use": "allow",
                 "Administer": "deny",
                 "Create": "deny",
                 "ViewAuthorization": "allow",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/servicehook_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/servicehook_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_permissions = azuredevops.ServicehookPermissions("example-permissions",
@@ -269,14 +270,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_permissions = azuredevops.ServicehookPermissions("example-permissions",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/servicehook_storage_queue_pipelines.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/servicehook_storage_queue_pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,24 +310,29 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azure as azure
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_resource_group = azure.core.ResourceGroup("exampleResourceGroup", location="West Europe")
-        example_account = azure.storage.Account("exampleAccount",
+        example = azuredevops.Project("example", name="example-project")
+        example_resource_group = azure.core.ResourceGroup("example",
+            name="example-resources",
+            location="West Europe")
+        example_account = azure.storage.Account("example",
+            name="servicehookexamplestacc",
             resource_group_name=example_resource_group.name,
             location=example_resource_group.location,
             account_tier="Standard",
             account_replication_type="LRS")
-        example_queue = azure.storage.Queue("exampleQueue", storage_account_name=example_account.name)
-        example_servicehook_storage_queue_pipelines = azuredevops.ServicehookStorageQueuePipelines("exampleServicehookStorageQueuePipelines",
-            project_id=example_project.id,
+        example_queue = azure.storage.Queue("example",
+            name="examplequeue",
+            storage_account_name=example_account.name)
+        example_servicehook_storage_queue_pipelines = azuredevops.ServicehookStorageQueuePipelines("example",
+            project_id=example.id,
             account_name=example_account.name,
             account_key=example_account.primary_access_key,
             queue_name=example_queue.name,
             visi_timeout=30,
             run_state_changed_event=azuredevops.ServicehookStorageQueuePipelinesRunStateChangedEventArgs(
                 run_state_filter="Completed",
                 run_result_filter="Succeeded",
@@ -339,18 +344,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.ServicehookStorageQueuePipelines("example",
-            project_id=azuredevops_project["example"]["id"],
-            account_name=azurerm_storage_account["example"]["name"],
-            account_key=azurerm_storage_account["example"]["primary_access_key"],
-            queue_name=azurerm_storage_queue["example"]["name"],
+            project_id=example_azuredevops_project["id"],
+            account_name=example_azurerm_storage_account["name"],
+            account_key=example_azurerm_storage_account["primaryAccessKey"],
+            queue_name=example_azurerm_storage_queue["name"],
             visi_timeout=30,
             run_state_changed_event=azuredevops.ServicehookStorageQueuePipelinesRunStateChangedEventArgs())
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
@@ -386,24 +391,29 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azure as azure
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject")
-        example_resource_group = azure.core.ResourceGroup("exampleResourceGroup", location="West Europe")
-        example_account = azure.storage.Account("exampleAccount",
+        example = azuredevops.Project("example", name="example-project")
+        example_resource_group = azure.core.ResourceGroup("example",
+            name="example-resources",
+            location="West Europe")
+        example_account = azure.storage.Account("example",
+            name="servicehookexamplestacc",
             resource_group_name=example_resource_group.name,
             location=example_resource_group.location,
             account_tier="Standard",
             account_replication_type="LRS")
-        example_queue = azure.storage.Queue("exampleQueue", storage_account_name=example_account.name)
-        example_servicehook_storage_queue_pipelines = azuredevops.ServicehookStorageQueuePipelines("exampleServicehookStorageQueuePipelines",
-            project_id=example_project.id,
+        example_queue = azure.storage.Queue("example",
+            name="examplequeue",
+            storage_account_name=example_account.name)
+        example_servicehook_storage_queue_pipelines = azuredevops.ServicehookStorageQueuePipelines("example",
+            project_id=example.id,
             account_name=example_account.name,
             account_key=example_account.primary_access_key,
             queue_name=example_queue.name,
             visi_timeout=30,
             run_state_changed_event=azuredevops.ServicehookStorageQueuePipelinesRunStateChangedEventArgs(
                 run_state_filter="Completed",
                 run_result_filter="Succeeded",
@@ -415,18 +425,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.ServicehookStorageQueuePipelines("example",
-            project_id=azuredevops_project["example"]["id"],
-            account_name=azurerm_storage_account["example"]["name"],
-            account_key=azurerm_storage_account["example"]["primary_access_key"],
-            queue_name=azurerm_storage_queue["example"]["name"],
+            project_id=example_azuredevops_project["id"],
+            account_name=example_azurerm_storage_account["name"],
+            account_key=example_azurerm_storage_account["primaryAccessKey"],
+            queue_name=example_azurerm_storage_queue["name"],
             visi_timeout=30,
             run_state_changed_event=azuredevops.ServicehookStorageQueuePipelinesRunStateChangedEventArgs())
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/tagging_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/tagging_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_permissions = azuredevops.TaggingPermissions("example-permissions",
@@ -269,14 +270,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_permissions = azuredevops.TaggingPermissions("example-permissions",
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/team.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,25 +259,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_project_contributors = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_contributors = azuredevops.get_group_output(project_id=example.id,
             name="Contributors")
-        example_project_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_team = azuredevops.Team("exampleTeam",
-            project_id=example_project.id,
+        example_team = azuredevops.Team("example",
+            project_id=example.id,
+            name="Example Team",
             administrators=[example_project_contributors.descriptor],
             members=[example_project_readers.descriptor])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
 
@@ -325,25 +327,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_project_contributors = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_contributors = azuredevops.get_group_output(project_id=example.id,
             name="Contributors")
-        example_project_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_team = azuredevops.Team("exampleTeam",
-            project_id=example_project.id,
+        example_team = azuredevops.Team("example",
+            project_id=example.id,
+            name="Example Team",
             administrators=[example_project_contributors.descriptor],
             members=[example_project_readers.descriptor])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Relevant Links
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/team_administrators.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team_administrators.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,22 +196,25 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_project_contributors = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_contributors = azuredevops.get_group_output(project_id=example.id,
             name="Contributors")
-        example_team = azuredevops.Team("exampleTeam", project_id=example_project.id)
+        example_team = azuredevops.Team("example",
+            project_id=example.id,
+            name=example.name.apply(lambda name: f"{name} Team 2"))
         example_team_administrators = azuredevops.TeamAdministrators("example-team-administrators",
             project_id=example_team.project_id,
             team_id=example_team.id,
             mode="overwrite",
             administrators=[example_project_contributors.descriptor])
         ```
         <!--End PulumiCodeChooser -->
@@ -254,22 +257,25 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_project_contributors = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_contributors = azuredevops.get_group_output(project_id=example.id,
             name="Contributors")
-        example_team = azuredevops.Team("exampleTeam", project_id=example_project.id)
+        example_team = azuredevops.Team("example",
+            project_id=example.id,
+            name=example.name.apply(lambda name: f"{name} Team 2"))
         example_team_administrators = azuredevops.TeamAdministrators("example-team-administrators",
             project_id=example_team.project_id,
             team_id=example_team.id,
             mode="overwrite",
             administrators=[example_project_contributors.descriptor])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/team_members.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/team_members.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,22 +196,25 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_project_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_team = azuredevops.Team("exampleTeam", project_id=example_project.id)
+        example_team = azuredevops.Team("example",
+            project_id=example.id,
+            name=example.name.apply(lambda name: f"{name} Team 2"))
         example_team_members = azuredevops.TeamMembers("example-team-members",
             project_id=example_team.project_id,
             team_id=example_team.id,
             mode="overwrite",
             members=[example_project_readers.descriptor])
         ```
         <!--End PulumiCodeChooser -->
@@ -254,22 +257,25 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_project_readers = azuredevops.get_group_output(project_id=example_project.id,
+        example_project_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
-        example_team = azuredevops.Team("exampleTeam", project_id=example_project.id)
+        example_team = azuredevops.Team("example",
+            project_id=example.id,
+            name=example.name.apply(lambda name: f"{name} Team 2"))
         example_team_members = azuredevops.TeamMembers("example-team-members",
             project_id=example_team.project_id,
             team_id=example_team.id,
             mode="overwrite",
             members=[example_project_readers.descriptor])
         ```
         <!--End PulumiCodeChooser -->
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/user.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/variable_group.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/variable_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -235,21 +235,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_variable_group = azuredevops.VariableGroup("exampleVariableGroup",
-            project_id=example_project.id,
+        example_variable_group = azuredevops.VariableGroup("example",
+            project_id=example.id,
+            name="Example Variable Group",
             description="Example Variable Group Description",
             allow_access=True,
             variables=[
                 azuredevops.VariableGroupVariableArgs(
                     name="key1",
                     value="val1",
                 ),
@@ -265,32 +267,34 @@
         ### With AzureRM Key Vault
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             description="Managed by Terraform",
             credentials=azuredevops.ServiceEndpointAzureRMCredentialsArgs(
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
-        example_variable_group = azuredevops.VariableGroup("exampleVariableGroup",
-            project_id=example_project.id,
+        example_variable_group = azuredevops.VariableGroup("example",
+            project_id=example.id,
+            name="Example Variable Group",
             description="Example Variable Group Description",
             allow_access=True,
             key_vault=azuredevops.VariableGroupKeyVaultArgs(
                 name="example-kv",
                 service_endpoint_id=example_service_endpoint_azure_rm.id,
             ),
             variables=[
@@ -355,21 +359,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_variable_group = azuredevops.VariableGroup("exampleVariableGroup",
-            project_id=example_project.id,
+        example_variable_group = azuredevops.VariableGroup("example",
+            project_id=example.id,
+            name="Example Variable Group",
             description="Example Variable Group Description",
             allow_access=True,
             variables=[
                 azuredevops.VariableGroupVariableArgs(
                     name="key1",
                     value="val1",
                 ),
@@ -385,32 +391,34 @@
         ### With AzureRM Key Vault
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("exampleServiceEndpointAzureRM",
-            project_id=example_project.id,
+        example_service_endpoint_azure_rm = azuredevops.ServiceEndpointAzureRM("example",
+            project_id=example.id,
             service_endpoint_name="Example AzureRM",
             description="Managed by Terraform",
             credentials=azuredevops.ServiceEndpointAzureRMCredentialsArgs(
                 serviceprincipalid="00000000-0000-0000-0000-000000000000",
                 serviceprincipalkey="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             ),
             azurerm_spn_tenantid="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_id="00000000-0000-0000-0000-000000000000",
             azurerm_subscription_name="Example Subscription Name")
-        example_variable_group = azuredevops.VariableGroup("exampleVariableGroup",
-            project_id=example_project.id,
+        example_variable_group = azuredevops.VariableGroup("example",
+            project_id=example.id,
+            name="Example Variable Group",
             description="Example Variable Group Description",
             allow_access=True,
             key_vault=azuredevops.VariableGroupKeyVaultArgs(
                 name="example-kv",
                 service_endpoint_id=example_service_endpoint_azure_rm.id,
             ),
             variables=[
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/variable_group_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/variable_group_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,20 +237,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
+            name="Testing",
             description="Testing-description",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
         example = azuredevops.VariableGroup("example",
             project_id=project.id,
+            name="test",
             description="Test Description",
             allow_access=True,
             variables=[azuredevops.VariableGroupVariableArgs(
                 name="key1",
                 value="val1",
             )])
         tf_project_readers = azuredevops.get_group_output(project_id=project.id,
@@ -319,20 +321,22 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         project = azuredevops.Project("project",
+            name="Testing",
             description="Testing-description",
             visibility="private",
             version_control="Git",
             work_item_template="Agile")
         example = azuredevops.VariableGroup("example",
             project_id=project.id,
+            name="test",
             description="Test Description",
             allow_access=True,
             variables=[azuredevops.VariableGroupVariableArgs(
                 name="key1",
                 value="val1",
             )])
         tf_project_readers = azuredevops.get_group_output(project_id=project.id,
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/work_item_query_permissions.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/work_item_query_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         project_wiq_root_permissions = azuredevops.WorkItemQueryPermissions("project-wiq-root-permissions",
@@ -272,14 +273,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_permissions = azuredevops.WorkItemQueryPermissions("example-permissions",
@@ -298,14 +300,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_contributors = azuredevops.get_group_output(project_id=example.id,
@@ -381,14 +384,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         project_wiq_root_permissions = azuredevops.WorkItemQueryPermissions("project-wiq-root-permissions",
@@ -412,14 +416,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_permissions = azuredevops.WorkItemQueryPermissions("example-permissions",
@@ -438,14 +443,15 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
         example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
         example_readers = azuredevops.get_group_output(project_id=example.id,
             name="Readers")
         example_contributors = azuredevops.get_group_output(project_id=example.id,
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops/workitem.py` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops/workitem.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,42 +302,44 @@
         ### Basic usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_workitem = azuredevops.Workitem("exampleWorkitem",
-            project_id=example_project.id,
+        example_workitem = azuredevops.Workitem("example",
+            project_id=example_azuredevops_project["id"],
             title="Example Work Item",
             type="Issue",
             state="Active",
             tags=["Tag"])
         ```
         <!--End PulumiCodeChooser -->
 
         ### With custom fields
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_workitem = azuredevops.Workitem("exampleWorkitem",
-            project_id=example_project.id,
+        example_workitem = azuredevops.Workitem("example",
+            project_id=example_azuredevops_project["id"],
             title="Example Work Item",
             type="Issue",
             state="Active",
             tags=["Tag"],
             custom_fields={
                 "example": "example",
             })
@@ -373,42 +375,44 @@
         ### Basic usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_workitem = azuredevops.Workitem("exampleWorkitem",
-            project_id=example_project.id,
+        example_workitem = azuredevops.Workitem("example",
+            project_id=example_azuredevops_project["id"],
             title="Example Work Item",
             type="Issue",
             state="Active",
             tags=["Tag"])
         ```
         <!--End PulumiCodeChooser -->
 
         ### With custom fields
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
-        example_project = azuredevops.Project("exampleProject",
+        example = azuredevops.Project("example",
+            name="Example Project",
             work_item_template="Agile",
             version_control="Git",
             visibility="private",
             description="Managed by Terraform")
-        example_workitem = azuredevops.Workitem("exampleWorkitem",
-            project_id=example_project.id,
+        example_workitem = azuredevops.Workitem("example",
+            project_id=example_azuredevops_project["id"],
             title="Example Work Item",
             type="Issue",
             state="Active",
             tags=["Tag"],
             custom_fields={
                 "example": "example",
             })
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops.egg-info/PKG-INFO` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 3.1.0a1713331204
+Version: 3.1.0a1713526847
 Summary: A Pulumi package for creating and managing Azure DevOps.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi,azuredevops
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pulumi_azuredevops.egg-info/SOURCES.txt` & `pulumi_azuredevops-3.1.0a1713526847/pulumi_azuredevops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1713331204/pyproject.toml` & `pulumi_azuredevops-3.1.0a1713526847/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_azuredevops"
   description = "A Pulumi package for creating and managing Azure DevOps."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "azuredevops"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.1.0a1713331204"
+  version = "3.1.0a1713526847"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-azuredevops"
 
 [build-system]
```

