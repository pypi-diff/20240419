# Comparing `tmp/cosmotech-run-orchestrator-1.2.2.tar.gz` & `tmp/cosmotech_run_orchestrator-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmotech-run-orchestrator-1.2.2.tar", last modified: Fri Mar 15 15:51:27 2024, max compression
+gzip compressed data, was "cosmotech_run_orchestrator-1.2.3.tar", last modified: Fri Apr 19 14:05:54 2024, max compression
```

## Comparing `cosmotech-run-orchestrator-1.2.2.tar` & `cosmotech_run_orchestrator-1.2.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.403575 cosmotech-run-orchestrator-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-15 15:51:27.403575 cosmotech-run-orchestrator-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.391575 cosmotech-run-orchestrator-1.2.2/cosmotech/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.391575 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.395575 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/download_cloud_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15242 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/legacy_json_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/parameters_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/run_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/runner_data_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/templates_listing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.395575 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/command_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.395575 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/schema/run_template_json_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.395575 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/templates/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/templates/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.395575 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.391575 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator_plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.395575 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator_plugins/csm-orc/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator_plugins/csm-orc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.399575 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator_plugins/csm-orc/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator_plugins/csm-orc/templates/download_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator_plugins/csm-orc/templates/download_run_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator_plugins/csm-orc/templates/run_step.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.399575 cosmotech-run-orchestrator-1.2.2/cosmotech_run_orchestrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-15 15:51:27.000000 cosmotech-run-orchestrator-1.2.2/cosmotech_run_orchestrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-15 15:51:27.000000 cosmotech-run-orchestrator-1.2.2/cosmotech_run_orchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 15:51:27.000000 cosmotech-run-orchestrator-1.2.2/cosmotech_run_orchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-15 15:51:27.000000 cosmotech-run-orchestrator-1.2.2/cosmotech_run_orchestrator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 15:51:27.000000 cosmotech-run-orchestrator-1.2.2/cosmotech_run_orchestrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-15 15:51:27.000000 cosmotech-run-orchestrator-1.2.2/cosmotech_run_orchestrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-15 15:51:27.000000 cosmotech-run-orchestrator-1.2.2/cosmotech_run_orchestrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/requirements.doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 15:51:27.403575 cosmotech-run-orchestrator-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.399575 cosmotech-run-orchestrator-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/tests/test_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-15 15:51:23.000000 cosmotech-run-orchestrator-1.2.2/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.016782 cosmotech_run_orchestrator-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-19 14:05:54.016782 cosmotech_run_orchestrator-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.004782 cosmotech_run_orchestrator-1.2.3/cosmotech/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.008782 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.008782 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/download_cloud_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15242 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/legacy_json_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/parameters_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/runner_data_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/templates_listing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.008782 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/command_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.008782 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/schema/run_template_json_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.012781 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/templates/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/templates/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.012781 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.004782 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.012781 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator_plugins/csm-orc/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator_plugins/csm-orc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.012781 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator_plugins/csm-orc/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator_plugins/csm-orc/templates/download_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator_plugins/csm-orc/templates/download_run_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator_plugins/csm-orc/templates/run_step.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.016782 cosmotech_run_orchestrator-1.2.3/cosmotech_run_orchestrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-19 14:05:53.000000 cosmotech_run_orchestrator-1.2.3/cosmotech_run_orchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-19 14:05:54.000000 cosmotech_run_orchestrator-1.2.3/cosmotech_run_orchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:05:53.000000 cosmotech_run_orchestrator-1.2.3/cosmotech_run_orchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 14:05:53.000000 cosmotech_run_orchestrator-1.2.3/cosmotech_run_orchestrator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:05:53.000000 cosmotech_run_orchestrator-1.2.3/cosmotech_run_orchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-19 14:05:53.000000 cosmotech_run_orchestrator-1.2.3/cosmotech_run_orchestrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 14:05:53.000000 cosmotech_run_orchestrator-1.2.3/cosmotech_run_orchestrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/requirements.doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:05:54.016782 cosmotech_run_orchestrator-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:05:54.016782 cosmotech_run_orchestrator-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/tests/test_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-19 14:05:48.000000 cosmotech_run_orchestrator-1.2.3/tests/test_template.py
```

### Comparing `cosmotech-run-orchestrator-1.2.2/LICENSE` & `cosmotech_run_orchestrator-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/PKG-INFO` & `cosmotech_run_orchestrator-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: cosmotech-run-orchestrator
-Version: 1.2.2
+Version: 1.2.3
 Summary: Orchestration suite for Cosmotech Run Templates
 Author-email: Cosmo Tech <platform@cosmotech.com>
 Project-URL: Homepage, https://www.cosmotech.com
 Project-URL: Source, https://github.com/Cosmo-Tech/run-orchestrator
 Project-URL: Documentation, https://cosmo-tech.github.io/run-orchestrator/
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cosmotech-acceleration-library==0.5.2
-Requires-Dist: cosmotech-api==3.1.1
+Requires-Dist: cosmotech-acceleration-library~=0.5.3
+Requires-Dist: cosmotech-api~=3.1.1
 Requires-Dist: flowpipe==1.0.0
 Requires-Dist: jsonschema==4.21.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: click==8.1.7
 Requires-Dist: rich-click==1.7.3
 Requires-Dist: click-log==0.4.0
 Requires-Dist: rich==13.7.0
```

### Comparing `cosmotech-run-orchestrator-1.2.2/README.md` & `cosmotech_run_orchestrator-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/download_cloud_steps.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/download_cloud_steps.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/entrypoint.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/entrypoint.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/legacy_json_generator.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/legacy_json_generator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/main.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/main.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/parameters_generation.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/parameters_generation.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/run.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/run.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/run_step.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/run_step.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/runner_data_downloader.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/runner_data_downloader.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/console_scripts/templates_listing.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/console_scripts/templates_listing.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/command_template.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/command_template.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/environment.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/environment.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/orchestrator.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/orchestrator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/runner.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/runner.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/core/step.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/core/step.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/schema/run_template_json_schema.json` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/schema/run_template_json_schema.json`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/templates/library.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/templates/library.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/templates/plugin.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/templates/plugin.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/api.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/api.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/click.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/click.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/decorators.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/json.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/logger.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/logger.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator/utils/singleton.py` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator_plugins/csm-orc/templates/download_data.json` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator_plugins/csm-orc/templates/download_data.json`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator_plugins/csm-orc/templates/download_run_data.json` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator_plugins/csm-orc/templates/download_run_data.json`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech/orchestrator_plugins/csm-orc/templates/run_step.json` & `cosmotech_run_orchestrator-1.2.3/cosmotech/orchestrator_plugins/csm-orc/templates/run_step.json`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech_run_orchestrator.egg-info/PKG-INFO` & `cosmotech_run_orchestrator-1.2.3/cosmotech_run_orchestrator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: cosmotech-run-orchestrator
-Version: 1.2.2
+Version: 1.2.3
 Summary: Orchestration suite for Cosmotech Run Templates
 Author-email: Cosmo Tech <platform@cosmotech.com>
 Project-URL: Homepage, https://www.cosmotech.com
 Project-URL: Source, https://github.com/Cosmo-Tech/run-orchestrator
 Project-URL: Documentation, https://cosmo-tech.github.io/run-orchestrator/
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cosmotech-acceleration-library==0.5.2
-Requires-Dist: cosmotech-api==3.1.1
+Requires-Dist: cosmotech-acceleration-library~=0.5.3
+Requires-Dist: cosmotech-api~=3.1.1
 Requires-Dist: flowpipe==1.0.0
 Requires-Dist: jsonschema==4.21.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: click==8.1.7
 Requires-Dist: rich-click==1.7.3
 Requires-Dist: click-log==0.4.0
 Requires-Dist: rich==13.7.0
```

### Comparing `cosmotech-run-orchestrator-1.2.2/cosmotech_run_orchestrator.egg-info/SOURCES.txt` & `cosmotech_run_orchestrator-1.2.3/cosmotech_run_orchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/pyproject.toml` & `cosmotech_run_orchestrator-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/tests/test_environment.py` & `cosmotech_run_orchestrator-1.2.3/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/tests/test_orchestrator.py` & `cosmotech_run_orchestrator-1.2.3/tests/test_orchestrator.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/tests/test_step.py` & `cosmotech_run_orchestrator-1.2.3/tests/test_step.py`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.2.2/tests/test_template.py` & `cosmotech_run_orchestrator-1.2.3/tests/test_template.py`

 * *Files identical despite different names*

