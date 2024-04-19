# Comparing `tmp/gitlabform-3.9.4.tar.gz` & `tmp/gitlabform-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabform-3.9.4.tar", last modified: Mon Apr 15 15:17:15 2024, max compression
+gzip compressed data, was "gitlabform-3.9.5.tar", last modified: Fri Apr 19 16:07:33 2024, max compression
```

## Comparing `gitlabform-3.9.4.tar` & `gitlabform-3.9.5.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.370504 gitlabform-3.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-15 15:17:10.000000 gitlabform-3.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-15 15:17:15.370504 gitlabform-3.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-15 15:17:10.000000 gitlabform-3.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.346504 gitlabform-3.9.4/gitlabform/
--rw-r--r--   0 runner    (1001) docker     (127)    23871 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.346504 gitlabform-3.9.4/gitlabform/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/configuration/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.350504 gitlabform-3.9.4/gitlabform/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/branches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/commits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/group_badges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/group_ldap_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/group_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/members.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/merge_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/project_badges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/project_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/project_merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/project_protected_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     8115 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/gitlab/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.350504 gitlabform-3.9.4/gitlabform/lists/
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/lists/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/lists/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/lists/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.354504 gitlabform-3.9.4/gitlabform/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/defining_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.354504 gitlabform-3.9.4/gitlabform/processors/group/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/group_badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/group_ldap_links_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/group_members_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/group_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/group/group_variables_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/multiple_entities_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.358504 gitlabform-3.9.4/gitlabform/processors/project/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/branches_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/deploy_keys_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/files_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/hooks_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/integrations_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/members_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/merge_requests_approval_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/project_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/project_push_rules_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/project_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/resource_groups_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/schedules_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/tags_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/project/variables_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.358504 gitlabform-3.9.4/gitlabform/processors/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/shared/protected_environments_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/single_entity_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.358504 gitlabform-3.9.4/gitlabform/processors/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/util/branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/processors/util/difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 15:17:10.000000 gitlabform-3.9.4/gitlabform/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.366504 gitlabform-3.9.4/gitlabform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 15:17:15.000000 gitlabform-3.9.4/gitlabform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 15:17:15.370504 gitlabform-3.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-15 15:17:10.000000 gitlabform-3.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.358504 gitlabform-3.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.358504 gitlabform-3.9.4/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.362504 gitlabform-3.9.4/tests/acceptance/standard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2738 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_archive_project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5971 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_badges.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3293 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_branches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8047 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_deploy_keys.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_deploy_keys_all_projects.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10859 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_files.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_files_all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1951 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_files_protected.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3059 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_files_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4136 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_badges.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4129 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_members_case_insensitive.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_members_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9639 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_members_users.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      882 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5622 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_inheritance_break.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10353 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2324 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_members.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_members_add_group.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2253 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_members_enforce.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2205 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_project_group_members_case_insensitive.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1391 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_project_members_case_insensitve.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_resource_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2180 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_running.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10507 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_schedules.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      871 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_token_from_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16845 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_transfer_project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5559 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/acceptance/standard/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.366504 gitlabform-3.9.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.366504 gitlabform-3.9.4/tests/unit/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3042 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_case_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_skip_groups_skip_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/configuration/test_yaml_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:15.366504 gitlabform-3.9.4/tests/unit/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/processors/test_abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/processors/test_branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/processors/test_difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/test_access_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/test_non_empty_configs_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-15 15:17:10.000000 gitlabform-3.9.4/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.539098 gitlabform-3.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-19 16:07:30.000000 gitlabform-3.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-19 16:07:33.539098 gitlabform-3.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-19 16:07:30.000000 gitlabform-3.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.519098 gitlabform-3.9.5/gitlabform/
+-rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.523098 gitlabform-3.9.5/gitlabform/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.527098 gitlabform-3.9.5/gitlabform/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/commits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/group_badges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/group_ldap_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/merge_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/project_badges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/project_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/project_merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/project_protected_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8115 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/python_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.527098 gitlabform-3.9.5/gitlabform/lists/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/lists/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/lists/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/lists/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.527098 gitlabform-3.9.5/gitlabform/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/defining_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.527098 gitlabform-3.9.5/gitlabform/processors/group/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/group_badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/group_ldap_links_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/group_members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/group_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/group_variables_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/multiple_entities_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.531098 gitlabform-3.9.5/gitlabform/processors/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/branches_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/deploy_keys_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/files_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/hooks_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/integrations_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/merge_requests_approval_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/project_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/project_push_rules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/project_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/resource_groups_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/schedules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/tags_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/variables_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.531098 gitlabform-3.9.5/gitlabform/processors/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/shared/protected_environments_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/single_entity_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.531098 gitlabform-3.9.5/gitlabform/processors/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/util/branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/util/difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.539098 gitlabform-3.9.5/gitlabform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 16:07:33.543098 gitlabform-3.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-19 16:07:30.000000 gitlabform-3.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.531098 gitlabform-3.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.531098 gitlabform-3.9.5/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.535098 gitlabform-3.9.5/tests/acceptance/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2738 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_archive_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5971 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_badges.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3293 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_branches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8047 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_deploy_keys.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_deploy_keys_all_projects.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10859 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_files_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1951 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_files_protected.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3059 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_files_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4136 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_badges.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4129 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_members_case_insensitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_members_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9639 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_members_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      882 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5622 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_inheritance_break.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10353 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2324 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_members.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_members_add_group.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2253 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_members_enforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2205 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_project_group_members_case_insensitive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1391 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_project_members_case_insensitve.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_resource_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2834 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_running.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14216 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_schedules.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      871 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_token_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_transfer_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5559 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.539098 gitlabform-3.9.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.539098 gitlabform-3.9.5/tests/unit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3042 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_case_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_skip_groups_skip_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_yaml_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.539098 gitlabform-3.9.5/tests/unit/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/processors/test_abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/processors/test_branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/processors/test_difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/test_access_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/test_non_empty_configs_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/test_utils.py
```

### Comparing `gitlabform-3.9.4/LICENSE` & `gitlabform-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/PKG-INFO` & `gitlabform-3.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.9.4
+Version: 3.9.5
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.9.4 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.9.5 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

### Comparing `gitlabform-3.9.4/README.md` & `gitlabform-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/__init__.py` & `gitlabform-3.9.5/gitlabform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,27 +49,28 @@
 class GitLabForm:
     def __init__(
         self,
         include_archived_projects=True,
         target=None,
         config_string=None,
         noop=False,
+        output_file=None,
     ):
         if target and config_string:
             # this mode is basically only for testing
 
             self.target = target
             self.config_string = config_string
             self.verbose = True
             self.debug = True
             self.strict = True
             self.start_from = 1
             self.start_from_group = 1
             self.noop = noop
-            self.output_file = None
+            self.output_file = output_file
             self.skip_version_check = True
             self.include_archived_projects = include_archived_projects
             self.just_show_version = False
             self.terminate_after_error = True
             self.only_sections = "all"
 
             self._configure_output(tests=True)
```

### Comparing `gitlabform-3.9.4/gitlabform/configuration/common.py` & `gitlabform-3.9.5/gitlabform/configuration/common.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/configuration/core.py` & `gitlabform-3.9.5/gitlabform/configuration/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/configuration/groups.py` & `gitlabform-3.9.5/gitlabform/configuration/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/configuration/projects.py` & `gitlabform-3.9.5/gitlabform/configuration/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/configuration/transform.py` & `gitlabform-3.9.5/gitlabform/configuration/transform.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/__init__.py` & `gitlabform-3.9.5/gitlabform/gitlab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,20 @@
 from gitlabform.gitlab.project_deploy_keys import GitLabProjectDeployKeys
 from gitlabform.gitlab.project_protected_environments import (
     GitLabProjectProtectedEnvironments,
 )
 from gitlabform.gitlab.project_merge_requests_approvals import (
     GitLabProjectMergeRequestsApprovals,
 )
+from gitlabform.gitlab.python_gitlab import PythonGitlab
 from gitlabform.gitlab.variables import GitLabVariables
 from gitlabform.gitlab.repositories import GitLabRepositories
 from gitlabform.gitlab.resource_groups import GitLabResourceGroups
-from gitlabform.gitlab.schedules import GitLabPipelineSchedules
 from gitlabform.gitlab.integrations import GitLabIntegrations
 from gitlabform.gitlab.users import GitLabUsers
-from gitlab import Gitlab
 
 
 @enum.unique
 class AccessLevel(enum.IntEnum):
     NO_ACCESS = 0
     MINIMAL = 5  # introduced in GitLab 13.5
     GUEST = 10
@@ -61,15 +60,14 @@
     GitLabIntegrations,
     GitLabGroupLDAPLinks,
     GitLabGroupBadges,
     GitLabGroupVariables,
     GitLabPipelines,
     GitLabMembers,
     GitLabUsers,
-    GitLabPipelineSchedules,
     GitLabProjectBadges,
     GitLabProjectDeployKeys,
     GitLabProjectProtectedEnvironments,
     GitLabProjectMergeRequestsApprovals,
     GitLabVariables,
 ):
     pass
@@ -79,15 +77,15 @@
     def __init__(self, gitlabform: GitLab):
         url = gitlabform.url
         token = gitlabform.token
         ssl_verify = gitlabform.ssl_verify
         timeout = gitlabform.timeout
         session = gitlabform.session
 
-        self._gitlab: Gitlab = Gitlab(
+        self._gitlab: PythonGitlab = PythonGitlab(
             url,
             token,
             ssl_verify=ssl_verify,
             api_version="4",
             session=session,
             retry_transient_errors=True,
             timeout=timeout,
```

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/branches.py` & `gitlabform-3.9.5/gitlabform/gitlab/branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/commits.py` & `gitlabform-3.9.5/gitlabform/gitlab/commits.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/core.py` & `gitlabform-3.9.5/gitlabform/gitlab/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/group_badges.py` & `gitlabform-3.9.5/gitlabform/gitlab/group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/group_ldap_links.py` & `gitlabform-3.9.5/gitlabform/gitlab/group_ldap_links.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/group_variables.py` & `gitlabform-3.9.5/gitlabform/gitlab/group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/groups.py` & `gitlabform-3.9.5/gitlabform/gitlab/groups.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,35 +26,14 @@
             for group in groups:
                 if group["full_path"].lower() == some_string.lower():
                     return group
             raise NotFoundException(
                 f"Group/subgroup with path '{some_string}' not found."
             )
 
-    def create_group(self, name, path, parent_id=None, visibility="private"):
-        data = {
-            "name": name,
-            "path": path,
-            "visibility": visibility,
-        }
-        if parent_id is not None:
-            data["parent_id"] = parent_id
-        return self._make_requests_to_api(
-            "groups", data=data, method="POST", expected_codes=201
-        )
-
-    def delete_group(self, group_name):
-        # 404 means that the group does not exist anymore, so let's accept it for idempotency
-        return self._make_requests_to_api(
-            "groups/%s",
-            group_name,
-            method="DELETE",
-            expected_codes=[200, 202, 204, 404],
-        )
-
     def get_group(self, name):
         return self._make_requests_to_api("groups/%s", name)
 
     def get_groups(self):
         """
         :return: sorted list of groups
         """
@@ -131,34 +110,7 @@
         #     'setting1': value1,
         #     'setting2': value2,
         # }
         # ..as documented at: https://docs.gitlab.com/ee/api/groups.html#update-group
         self._make_requests_to_api(
             "groups/%s", project_and_group_name, "PUT", group_settings
         )
-
-    def add_share_to_group(
-        self, group, share_with_group_name, group_access, expires_at=None
-    ):
-        share_with_group_id = self.get_group_id_case_insensitive(share_with_group_name)
-        data = {"group_id": share_with_group_id, "expires_at": expires_at}
-        if group_access is not None:
-            data["group_access"] = group_access
-
-        return self._make_requests_to_api(
-            "groups/%s/share",
-            group,
-            method="POST",
-            data=data,
-            expected_codes=[200, 201],
-        )
-
-    def remove_share_from_group(self, group, share_with_group_name):
-        share_with_group_id = self.get_group_id_case_insensitive(share_with_group_name)
-
-        # 404 means that the user is already removed, so let's accept it for idempotency
-        return self._make_requests_to_api(
-            "groups/%s/share/%s",
-            (group, share_with_group_id),
-            method="DELETE",
-            expected_codes=[204, 404],
-        )
```

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/integrations.py` & `gitlabform-3.9.5/gitlabform/gitlab/integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/merge_requests.py` & `gitlabform-3.9.5/gitlabform/gitlab/merge_requests.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/pipelines.py` & `gitlabform-3.9.5/gitlabform/gitlab/pipelines.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/project_badges.py` & `gitlabform-3.9.5/gitlabform/gitlab/project_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/project_deploy_keys.py` & `gitlabform-3.9.5/gitlabform/gitlab/project_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/project_merge_requests_approvals.py` & `gitlabform-3.9.5/gitlabform/gitlab/project_merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/project_protected_environments.py` & `gitlabform-3.9.5/gitlabform/gitlab/project_protected_environments.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/projects.py` & `gitlabform-3.9.5/gitlabform/gitlab/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/repositories.py` & `gitlabform-3.9.5/gitlabform/gitlab/repositories.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/resource_groups.py` & `gitlabform-3.9.5/gitlabform/gitlab/resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/users.py` & `gitlabform-3.9.5/gitlabform/gitlab/users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/gitlab/variables.py` & `gitlabform-3.9.5/gitlabform/gitlab/variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/lists/__init__.py` & `gitlabform-3.9.5/gitlabform/lists/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/lists/filter.py` & `gitlabform-3.9.5/gitlabform/lists/filter.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/lists/groups.py` & `gitlabform-3.9.5/gitlabform/lists/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/lists/projects.py` & `gitlabform-3.9.5/gitlabform/lists/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/output.py` & `gitlabform-3.9.5/gitlabform/output.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/__init__.py` & `gitlabform-3.9.5/gitlabform/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/abstract_processor.py` & `gitlabform-3.9.5/gitlabform/processors/abstract_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from abc import ABC, abstractmethod
 from logging import debug
 from typing import Callable, Union
 
 import requests
 from cli_ui import debug as verbose
 
-from gitlabform.gitlab import GitLab
-from gitlab import Gitlab
+from gitlabform.gitlab import GitLab, PythonGitlab
 from gitlabform.gitlab import GitlabWrapper
 from gitlabform.output import EffectiveConfigurationFile
 from gitlabform.processors.util.decorators import configuration_to_safe_dict
 
 
 class AbstractProcessor(ABC):
     def __init__(self, configuration_name: str, gitlab: GitLab):
@@ -18,15 +17,15 @@
         self.gitlab = gitlab
         self.custom_diff_analyzers: dict[
             str,
             Callable[
                 [str, list[dict[str, Union[str, int]]], list[dict[str, int]]], bool
             ],
         ] = {}
-        self.gl: Gitlab = GitlabWrapper(self.gitlab)._gitlab
+        self.gl: PythonGitlab = GitlabWrapper(self.gitlab).get_gitlab()
 
     @configuration_to_safe_dict
     def process(
         self,
         project_or_project_and_group: str,
         configuration,
         dry_run: bool,
@@ -47,26 +46,26 @@
                 )
                 return
 
             if dry_run:
                 verbose(
                     f"Processing section '{self.configuration_name}' in dry-run mode."
                 )
+                project_transfer_source = ""
                 try:
                     project_transfer_source = configuration["project"]["transfer_from"]
                     verbose(
                         f"""Project {project_or_project_and_group} is configured to be transferred, 
                         diffing config from transfer source project {project_transfer_source}."""
                     )
-                    project_or_project_and_group = project_transfer_source
                 except KeyError:
                     pass
 
                 self._print_diff(
-                    project_or_project_and_group,
+                    project_transfer_source or project_or_project_and_group,
                     configuration.get(self.configuration_name),
                 )
             else:
                 verbose(f"Processing section '{self.configuration_name}'")
                 if self._can_proceed(project_or_project_and_group, configuration):
                     self._process_configuration_with_retries(
                         project_or_project_and_group, configuration
```

### Comparing `gitlabform-3.9.4/gitlabform/processors/defining_keys.py` & `gitlabform-3.9.5/gitlabform/processors/defining_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/group/__init__.py` & `gitlabform-3.9.5/gitlabform/processors/group/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/group/group_badges_processor.py` & `gitlabform-3.9.5/gitlabform/processors/group/group_badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/group/group_ldap_links_processor.py` & `gitlabform-3.9.5/gitlabform/processors/group/group_ldap_links_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/group/group_members_processor.py` & `gitlabform-3.9.5/gitlabform/processors/group/group_members_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from logging import debug
+from logging import debug, warning
 from typing import Dict, Tuple
 
 from cli_ui import fatal
 
 from gitlabform.constants import EXIT_INVALID_INPUT
 from gitlabform.gitlab import GitLab, AccessLevel
 from gitlabform.processors.abstract_processor import AbstractProcessor
+from gitlab.v4.objects import Group, GroupMember
+from gitlab import GitlabDeleteError
 
 
 class GroupMembersProcessor(AbstractProcessor):
     def __init__(self, gitlab: GitLab):
         super().__init__("group_members", gitlab)
 
-    def _process_configuration(self, group: str, configuration: dict):
+    def _process_configuration(self, group_name: str, configuration: dict):
         keep_bots = configuration.get("group_members|keep_bots", False)
 
         enforce_group_members = configuration.get("group_members|enforce", False)
 
         (
             groups_to_set_by_group_path,
             users_to_set_by_username,
@@ -30,18 +32,23 @@
             fatal(
                 "Group members configuration section has to contain"
                 " some 'users' or 'groups' defined as Owners,"
                 " if you want to enforce them (GitLab requires it).",
                 exit_code=EXIT_INVALID_INPUT,
             )
 
+        group = self.gl.get_group_by_name(group_name)
+
         self._process_groups(group, groups_to_set_by_group_path, enforce_group_members)
 
         self._process_users(
-            group, users_to_set_by_username, enforce_group_members, keep_bots
+            users_to_set_by_username,
+            enforce_group_members,
+            keep_bots,
+            group,
         )
 
     @staticmethod
     def _get_groups_and_users_to_set(configuration: dict) -> Tuple[dict, dict]:
         groups_to_set_by_group_path = configuration.get("group_members|groups", {})
 
         users_to_set_by_username = configuration.get("group_members", {})
@@ -56,36 +63,36 @@
                 users_to_set_by_username.pop("users", None)
                 users_to_set_by_username.pop("groups", None)
                 users_to_set_by_username.pop("keep_bots", None)
 
         return groups_to_set_by_group_path, users_to_set_by_username
 
     def _process_groups(
-        self, group: str, groups_to_set_by_group_path: dict, enforce_group_members: bool
+        self,
+        group_being_processed: Group,
+        groups_to_share_with_by_path: dict,
+        enforce_group_members: bool,
     ):
-        # group users before by group name
-        groups_before = self.gitlab.get_group_case_insensitive(group)[
-            "shared_with_groups"
-        ]
-        debug("Group shared with BEFORE: %s", groups_before)
+        shared_with_groups_before = group_being_processed.shared_with_groups
+        debug("Group shared with BEFORE: %s", shared_with_groups_before)
 
         groups_before_by_group_path = dict()
-        for share_details in groups_before:
-            groups_before_by_group_path[share_details["group_full_path"]] = (
-                share_details
+        for shared_with_group in shared_with_groups_before:
+            groups_before_by_group_path[shared_with_group["group_full_path"]] = (
+                shared_with_group
             )
 
-        for share_with_group_path in groups_to_set_by_group_path:
-            group_access_to_set = groups_to_set_by_group_path[share_with_group_path][
+        for share_with_group_path in groups_to_share_with_by_path:
+            group_access_to_set = groups_to_share_with_by_path[share_with_group_path][
                 "group_access"
             ]
 
             expires_at_to_set = (
-                groups_to_set_by_group_path[share_with_group_path]["expires_at"]
-                if "expires_at" in groups_to_set_by_group_path[share_with_group_path]
+                groups_to_share_with_by_path[share_with_group_path]["expires_at"]
+                if "expires_at" in groups_to_share_with_by_path[share_with_group_path]
                 else None
             )
 
             if share_with_group_path in groups_before_by_group_path:
                 group_access_before = groups_before_by_group_path[
                     share_with_group_path
                 ]["group_access_level"]
@@ -102,59 +109,72 @@
                         share_with_group_path,
                     )
                 else:
                     debug(
                         "Re-adding group '%s' to change their access level or expires at.",
                         share_with_group_path,
                     )
+                    share_with_group_id = groups_before_by_group_path[
+                        share_with_group_path
+                    ]["group_id"]
                     # we will remove the group first and then re-add them,
                     # to ensure that the group has the expected access level
-                    self.gitlab.remove_share_from_group(group, share_with_group_path)
-                    self.gitlab.add_share_to_group(
-                        group,
-                        share_with_group_path,
-                        group_access_to_set,
-                        expires_at_to_set,
+                    self._unshare(group_being_processed, share_with_group_id)
+
+                    group_being_processed.share(
+                        share_with_group_id, group_access_to_set, expires_at_to_set
                     )
 
             else:
                 debug(
                     "Adding group '%s' who previously was not a member.",
                     share_with_group_path,
                 )
-                self.gitlab.add_share_to_group(
-                    group, share_with_group_path, group_access_to_set, expires_at_to_set
+
+                share_with_group_id = self.gl.get_group_id(share_with_group_path)
+                group_being_processed.share(
+                    share_with_group_id, group_access_to_set, expires_at_to_set
                 )
 
         if enforce_group_members:
             # remove groups not configured explicitly
             groups_not_configured = set(groups_before_by_group_path) - set(
-                groups_to_set_by_group_path
+                groups_to_share_with_by_path
             )
             for group_path in groups_not_configured:
                 debug(
                     "Removing group '%s' who is not configured to be a member.",
                     group_path,
                 )
-                self.gitlab.remove_share_from_group(group, group_path)
+                share_with_group_id = self.gl.get_group_id(group_path)
+                self._unshare(group_being_processed, share_with_group_id)
         else:
             debug("Not enforcing group members.")
 
-        debug("Group shared with AFTER: %s", self.gitlab.get_group_members(group))
+        debug("Group shared with AFTER: %s", group_being_processed.members.list())
+
+    @staticmethod
+    def _unshare(group_being_processed, share_with_group_id):
+        try:
+            group_being_processed.unshare(share_with_group_id)
+        except GitlabDeleteError:
+            debug("Group could not be unshared, likely was never shared to begin with")
+            pass
 
     def _process_users(
         self,
-        group: str,
         users_to_set_by_username: dict,
         enforce_group_members: bool,
         keep_bots: bool,
+        group: Group,
     ):
         # group users before by username
         # (note: we DON'T get inherited users as we don't manage them at this level anyway)
-        users_before = self.gitlab.get_group_members(group, with_inherited=False)
+        users_before = self.get_group_members(group)
+
         debug("Group members BEFORE: %s", users_before.keys())
 
         if users_to_set_by_username:
             # group users to set by access level
             users_to_set_by_access_level: Dict[int, list] = dict()
             for user in users_to_set_by_username:
                 access_level = users_to_set_by_username[user]["access_level"]
@@ -174,50 +194,51 @@
                     expires_at_to_set = (
                         users_to_set_by_username[user]["expires_at"]
                         if "expires_at" in users_to_set_by_username[user]
                         else None
                     )
 
                     common_username = user.lower()
+                    user_id = self.gl.get_user_id(user)
+
                     if common_username in users_before:
-                        access_level_before = users_before[common_username][
-                            "access_level"
-                        ]
-                        expires_at_before = users_before[common_username]["expires_at"]
+                        group_member: GroupMember = group.members.get(user_id)
+
+                        access_level_before = users_before[common_username].access_level
+                        expires_at_before = users_before[common_username].expires_at
 
                         if (
                             access_level_before == access_level_to_set
                             and expires_at_before == expires_at_to_set
                         ):
                             debug(
                                 "Nothing to change for user '%s' - same config now as to set.",
                                 common_username,
                             )
                         else:
                             debug(
                                 "Editing user '%s' membership to change their access level or expires at.",
                                 common_username,
                             )
-                            self.gitlab.edit_member_of_group(
-                                group,
-                                common_username,
-                                access_level_to_set,
-                                expires_at_to_set,
-                            )
+
+                            group_member.access_level = access_level_to_set
+                            group_member.expires_at = expires_at_to_set
+                            group_member.save()
 
                     else:
                         debug(
                             "Adding user '%s' who previously was not a member.",
                             common_username,
                         )
-                        self.gitlab.add_member_to_group(
-                            group,
-                            common_username,
-                            access_level_to_set,
-                            expires_at_to_set,
+                        group.members.create(
+                            {
+                                "user_id": user_id,
+                                "access_level": access_level_to_set,
+                                "expires_at": expires_at_to_set,
+                            }
                         )
 
         if enforce_group_members:
             # remove users not configured explicitly
             # note: only direct members are removed - inherited are left
             users_not_configured = set(users_before.keys()) - set(
                 [username.lower() for username in users_to_set_by_username.keys()]
@@ -225,12 +246,25 @@
             for user in users_not_configured:
                 if keep_bots and self.gitlab.get_user_by_name(user)["bot"]:
                     debug(
                         f"Will not remove bot user '{user}' as the 'keep_bots' option is true."
                     )
                     continue
                 debug("Removing user '%s' who is not configured to be a member.", user)
-                self.gitlab.remove_member_from_group(group, user)
+                user_id = self.gl.get_user_id(user)
+                try:
+                    group.members.delete(user_id)
+                except GitlabDeleteError as error:
+                    warning(f"Member could not be deleted: ", error)
+                    pass
         else:
             debug("Not enforcing group members.")
 
-        debug("Group members AFTER: %s", self.gitlab.get_group_members(group))
+        debug("Group members AFTER: %s", group.members.list())
+
+    @staticmethod
+    def get_group_members(group) -> dict:
+        members = group.members.list()
+        users = {}
+        for member in members:
+            users[member.username.lower()] = member
+        return users
```

### Comparing `gitlabform-3.9.4/gitlabform/processors/group/group_variables_processor.py` & `gitlabform-3.9.5/gitlabform/processors/group/group_variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/multiple_entities_processor.py` & `gitlabform-3.9.5/gitlabform/processors/multiple_entities_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/__init__.py` & `gitlabform-3.9.5/gitlabform/processors/project/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/badges_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/branches_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/branches_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/deploy_keys_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/deploy_keys_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/files_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/files_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/hooks_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/hooks_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/integrations_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/integrations_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/members_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/members_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/merge_requests_approval_rules.py` & `gitlabform-3.9.5/gitlabform/processors/project/merge_requests_approval_rules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/merge_requests_approvals.py` & `gitlabform-3.9.5/gitlabform/processors/project/merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/project_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/project_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/resource_groups_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/resource_groups_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/tags_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/tags_processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 
 
 class TagsProcessor(AbstractProcessor):
     def __init__(self, gitlab: GitLab, strict: bool):
         super().__init__("tags", gitlab)
         self.strict = strict
 
-    def _get_user_by_username(self, username):
-        user = self.gl.users.list(username=username)
-        if len(user) == 0:
-            raise GitlabGetError(
-                "No users found when searching for username '%s'" % username, 404
-            )
-        return user[0]
-
     def _process_configuration(self, project_and_group: str, configuration: dict):
         project = self.gl.projects.get(id=project_and_group, lazy=True)
 
         for tag in sorted(configuration["tags"]):
             try:
                 if configuration["tags"][tag]["protected"]:
                     allowed_to_create = []
@@ -39,20 +31,24 @@
 
                         for config in requested_configuration:
                             if "access_level" in config:
                                 access_levels.add(config["access_level"])
                             elif "user_id" in config:
                                 user_ids.add(config["user_id"])
                             elif "user" in config:
-                                gitlab_user = self._get_user_by_username(config["user"])
+                                gitlab_user = self.gl.get_user_by_username(
+                                    config["user"]
+                                )
                                 user_ids.add(gitlab_user.get_id())
                             elif "group_id" in config:
                                 group_ids.add(config["group_id"])
                             elif "group" in config:
-                                gitlab_group = self.gl.groups.get(config["group"])
+                                gitlab_group = self.gl.get_group_by_groupname(
+                                    config["group"]
+                                )
                                 group_ids.add(gitlab_group.get_id())
 
                         for val in access_levels:
                             allowed_to_create.append({"access_level": val})
 
                         for val in user_ids:
                             allowed_to_create.append({"user_id": val})
```

### Comparing `gitlabform-3.9.4/gitlabform/processors/project/variables_processor.py` & `gitlabform-3.9.5/gitlabform/processors/project/variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/shared/protected_environments_processor.py` & `gitlabform-3.9.5/gitlabform/processors/shared/protected_environments_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/single_entity_processor.py` & `gitlabform-3.9.5/gitlabform/processors/single_entity_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/util/branch_protector.py` & `gitlabform-3.9.5/gitlabform/processors/util/branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/util/decorators.py` & `gitlabform-3.9.5/gitlabform/processors/util/decorators.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform/processors/util/difference_logger.py` & `gitlabform-3.9.5/gitlabform/processors/util/difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/gitlabform.egg-info/PKG-INFO` & `gitlabform-3.9.5/gitlabform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.9.4
+Version: 3.9.5
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.9.4 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.9.5 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

### Comparing `gitlabform-3.9.4/gitlabform.egg-info/SOURCES.txt` & `gitlabform-3.9.5/gitlabform.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 gitlabform/gitlab/merge_requests.py
 gitlabform/gitlab/pipelines.py
 gitlabform/gitlab/project_badges.py
 gitlabform/gitlab/project_deploy_keys.py
 gitlabform/gitlab/project_merge_requests_approvals.py
 gitlabform/gitlab/project_protected_environments.py
 gitlabform/gitlab/projects.py
+gitlabform/gitlab/python_gitlab.py
 gitlabform/gitlab/repositories.py
 gitlabform/gitlab/resource_groups.py
-gitlabform/gitlab/schedules.py
 gitlabform/gitlab/users.py
 gitlabform/gitlab/variables.py
 gitlabform/lists/__init__.py
 gitlabform/lists/filter.py
 gitlabform/lists/groups.py
 gitlabform/lists/projects.py
 gitlabform/processors/__init__.py
```

### Comparing `gitlabform-3.9.4/setup.py` & `gitlabform-3.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/__init__.py` & `gitlabform-3.9.5/tests/acceptance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,17 @@
     )
 
 
 def randomize_case(input: str) -> str:
     return "".join(random.choice((str.upper, str.lower))(char) for char in input)
 
 
-def run_gitlabform(config, target, include_archived_projects=True, noop=False):
+def run_gitlabform(
+    config, target, include_archived_projects=True, noop=False, output_file=None
+):
     # f-strings with """ used as configs have the disadvantage of having indentation in them - let's remove it here
     config = textwrap.dedent(config)
 
     # we don't want to repeat ourselves in the tests, so prefix the configs with this mandatory part here
     config = CONFIG + config
 
     # allow passing in gitlab RESTObjects. assume full path string otherwise
@@ -261,9 +263,10 @@
         target = target.path_with_namespace
 
     gf = GitLabForm(
         include_archived_projects=include_archived_projects,
         config_string=config,
         target=target,
         noop=noop,
+        output_file=output_file,
     )
     gf.run()
```

### Comparing `gitlabform-3.9.4/tests/acceptance/conftest.py` & `gitlabform-3.9.5/tests/acceptance/conftest.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_archive_project.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_archive_project.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_badges.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_branches.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_deploy_keys.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_deploy_keys_all_projects.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_deploy_keys_all_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_files.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_files.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_files_all.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_files_all.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_files_protected.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_files_protected.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_files_templates.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_files_templates.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_group_badges.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_group_members_case_insensitive.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_group_members_case_insensitive.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_group_members_groups.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_group_members_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_group_members_users.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_group_members_users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_group_settings.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_group_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_group_variables.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_hooks.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_hooks.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_inheritance_break.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_inheritance_break.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_integrations.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_members.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_members_add_group.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_members_add_group.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_members_enforce.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_members_enforce.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_project_group_members_case_insensitive.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_project_group_members_case_insensitive.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_project_members_case_insensitve.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_project_members_case_insensitve.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_project_settings.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_project_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_resource_groups.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_running.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_running.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pytest
 from tests.acceptance import (
     run_gitlabform,
 )
+from pathlib import Path
+from ruamel.yaml import YAML
 
 
 class TestRunning:
     # noinspection PyPep8Naming
     def test__ALL(self, gl, project, other_project):
         config = f"""
         projects_and_groups:
@@ -18,14 +20,34 @@
 
         project = gl.projects.get(project.id)
         assert project.request_access_enabled is True
 
         other_project = gl.projects.get(other_project.id)
         assert other_project.request_access_enabled is True
 
+    def test__ALL_output_file(self, gl, project, other_project):
+        config = f"""
+        projects_and_groups:
+          '*':
+            project_settings:
+              request_access_enabled: true
+        """
+
+        run_gitlabform(config, "ALL", output_file="output.yml")
+
+        project = gl.projects.get(project.id)
+        assert project.request_access_enabled is True
+
+        other_project = gl.projects.get(other_project.id)
+        assert other_project.request_access_enabled is True
+
+        path = Path("output.yml")
+        yaml = YAML(typ="safe")
+        assert yaml.load(path)
+
     # noinspection PyPep8Naming
     def test__ALL_dry_run(self, gl, project, other_project):
         config = f"""
         projects_and_groups:
           '*':
             project_settings:
               request_access_enabled: false
```

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_schedules.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_schedules.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import logging
 import pytest
 
-
 from tests.acceptance import run_gitlabform
 
 
 @pytest.fixture(scope="class")
 def schedules(project):
     another_branch = "scheduled/new-feature"
     project.branches.create({"branch": another_branch, "ref": "main"})
@@ -129,14 +129,18 @@
         assert variables[0]["value"] == "value123"
 
         assert variables[1]["variable_type"] == "file"
         assert variables[1]["key"] == "var2"
         assert variables[1]["value"] == "value987"
 
     def test__update_existing_schedule(self, project, schedules):
+        existing_schedule = self.__find_pipeline_schedule_by_description_and_get_first(
+            project, "Existing schedule"
+        )
+
         edit_schedule = f"""
         projects_and_groups:
           {project.path_with_namespace}:
             schedules:
               "Existing schedule":
                 ref: scheduled/new-feature
                 cron: "0 */4 * * *"
@@ -146,15 +150,114 @@
 
         run_gitlabform(edit_schedule, project)
 
         schedule = self.__find_pipeline_schedule_by_description_and_get_first(
             project, "Existing schedule"
         )
         assert schedule is not None
-        assert schedule.description == "Existing schedule"
+
+        # Verify it updated the schedule rather than creating/deleting
+        assert schedule.id == existing_schedule.id
+        assert schedule.description == existing_schedule.description
+
+        # Verify updates to schedule
+        assert schedule.ref == "scheduled/new-feature"
+        assert schedule.cron == "0 */4 * * *"
+        assert schedule.cron_timezone == "Stockholm"
+        assert schedule.active is False
+
+    def test__existing_schedule_is_not_modified_when_no_changes_made(
+        self, project_for_function, caplog
+    ):
+        caplog.set_level(logging.DEBUG)
+        existing_schedule = project_for_function.pipelineschedules.create(
+            {
+                "description": "Existing schedule",
+                "ref": "main",
+                "cron": "0 * * * *",
+                "active": True,
+            }
+        )
+
+        edit_schedule = f"""
+        projects_and_groups:
+          {project_for_function.path_with_namespace}:
+            schedules:
+              "Existing schedule":
+                ref: {existing_schedule.ref}
+                cron:  {existing_schedule.cron}
+                active: {existing_schedule.active}
+        """
+        run_gitlabform(edit_schedule, project_for_function)
+
+        schedule = self.__find_pipeline_schedule_by_description_and_get_first(
+            project_for_function, "Existing schedule"
+        )
+        assert schedule is not None
+
+        # Verify it updated the schedule rather than creating/deleting
+        assert schedule.id == existing_schedule.id
+        assert schedule.description == existing_schedule.description
+
+        # Verify schedule
+        assert schedule.ref == "main"
+        assert schedule.cron == "0 * * * *"
+        assert schedule.active is True
+
+        # Verify logged out "No update"; from which we can infer no API actions invoked
+        assert (
+            "No update required for pipeline schedule 'Existing schedule'"
+            in caplog.text
+        )
+
+    def test__update_existing_schedule_with_variables(self, project_for_function):
+        existing_schedule = project_for_function.pipelineschedules.create(
+            {
+                "description": "Existing schedule with vars",
+                "ref": "main",
+                "cron": "0 * * * *",
+            }
+        )
+        existing_schedule.variables.create(
+            {"key": "existing_var", "value": "test_value"}
+        )
+        assert existing_schedule is not None
+
+        edit_schedule = f"""
+        projects_and_groups:
+          {project_for_function.path_with_namespace}:
+            schedules:
+              "Existing schedule with vars":
+                ref: scheduled/new-feature
+                cron: "0 */4 * * *"
+                cron_timezone: "Stockholm"
+                active: false
+                variables:
+                    existing_var:
+                        value: new_value
+        """
+
+        run_gitlabform(edit_schedule, project_for_function)
+
+        schedule = self.__find_pipeline_schedule_by_description_and_get_first(
+            project_for_function, "Existing schedule with vars"
+        )
+        assert schedule is not None
+
+        # Verify it updated the schedule rather than creating/deleting
+        assert schedule.id == existing_schedule.id
+        assert schedule.description == existing_schedule.description
+
+        # Verify updates to schedule
+        variables = schedule.attributes["variables"]
+        assert len(variables) == 1
+        variable = variables[0]
+        assert variable.get("key") == "existing_var"
+        assert variable.get("value") == "new_value"
+
         assert schedule.ref == "scheduled/new-feature"
         assert schedule.cron == "0 */4 * * *"
         assert schedule.cron_timezone == "Stockholm"
         assert schedule.active is False
 
     def test__replace_existing_schedules(self, project, schedules):
         replace_schedules = f"""
```

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_tags.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_tags.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_token_from_config.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_token_from_config.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_transfer_project.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_transfer_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,17 @@
           {project_new_path_with_namespace}:
             project:
               transfer_from: {project_for_function.path_with_namespace}
             project_settings:
               description: test
         """
 
-        run_gitlabform(config, project_new_path_with_namespace, noop=True)
+        run_gitlabform(
+            config, project_new_path_with_namespace, noop=True, output_file="output.yml"
+        )
         projects_in_destination_after_transfer = other_group.projects.list()
 
         assert len(projects_in_destination_after_transfer) == len(
             projects_in_destination_before_transfer
         )
 
     def test__transfer_between_two_root_groups(
```

### Comparing `gitlabform-3.9.4/tests/acceptance/standard/test_variables.py` & `gitlabform-3.9.5/tests/acceptance/standard/test_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/configuration/test_case_sensitivity.py` & `gitlabform-3.9.5/tests/unit/configuration/test_case_sensitivity.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_projects_and_groups.py` & `gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_subgroups.py` & `gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/configuration/test_inheritance_break_validation.py` & `gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_validation.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/configuration/test_projects_and_groups.py` & `gitlabform-3.9.5/tests/unit/configuration/test_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/configuration/test_skip_groups_skip_projects.py` & `gitlabform-3.9.5/tests/unit/configuration/test_skip_groups_skip_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/configuration/test_subgroups.py` & `gitlabform-3.9.5/tests/unit/configuration/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/configuration/test_yaml_version.py` & `gitlabform-3.9.5/tests/unit/configuration/test_yaml_version.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/processors/test_abstract_processor.py` & `gitlabform-3.9.5/tests/unit/processors/test_abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/processors/test_branch_protector.py` & `gitlabform-3.9.5/tests/unit/processors/test_branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/processors/test_difference_logger.py` & `gitlabform-3.9.5/tests/unit/processors/test_difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/test_access_levels.py` & `gitlabform-3.9.5/tests/unit/test_access_levels.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/test_non_empty_configs_provider.py` & `gitlabform-3.9.5/tests/unit/test_non_empty_configs_provider.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.4/tests/unit/test_utils.py` & `gitlabform-3.9.5/tests/unit/test_utils.py`

 * *Files identical despite different names*

