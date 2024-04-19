# Comparing `tmp/synapseclient-4.1.1.tar.gz` & `tmp/synapseclient-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapseclient-4.1.1.tar", last modified: Thu Feb 29 02:59:24 2024, max compression
+gzip compressed data, was "synapseclient-4.2.0.tar", last modified: Fri Apr 19 00:44:54 2024, max compression
```

## Comparing `synapseclient-4.1.1.tar` & `synapseclient-4.2.0.tar`

### file list

```diff
@@ -1,112 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.232898 synapseclient-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-29 02:59:09.000000 synapseclient-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-02-29 02:59:24.232898 synapseclient-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-02-29 02:59:09.000000 synapseclient-4.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-29 02:59:09.000000 synapseclient-4.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-02-29 02:59:24.232898 synapseclient-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-29 02:59:09.000000 synapseclient-4.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.216898 synapseclient-4.1.1/synapseclient/
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/.synapseConfig
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63395 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.216898 synapseclient-4.1.1/synapseclient/api/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/api/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)   238435 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.216898 synapseclient-4.1.1/synapseclient/core/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19287 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.220898 synapseclient-4.1.1/synapseclient/core/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/constants/concrete_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/constants/config_file_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/constants/limits.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/constants/method_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.220898 synapseclient-4.1.1/synapseclient/core/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/credentials/cred_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/credentials/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/cumulative_transfer_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/dozer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/logging_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.220898 synapseclient-4.1.1/synapseclient/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/models/custom_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/models/dict_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/models/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.220898 synapseclient-4.1.1/synapseclient/core/multithread_download/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/multithread_download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15712 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/multithread_download/download_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/pool_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/remote_file_storage_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9591 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/sts_transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.220898 synapseclient-4.1.1/synapseclient/core/upload/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26031 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/upload/multipart_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/upload/upload_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    43085 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/core/version_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    34756 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.224898 synapseclient-4.1.1/synapseclient/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    37233 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    19090 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.224898 synapseclient-4.1.1/synapseclient/models/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/mixins/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/mixins/storable_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    20593 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.224898 synapseclient-4.1.1/synapseclient/models/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/access_control_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/activity_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/annotations_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/file_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/folder_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/project_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/storable_container_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/table_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/team_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/protocols/user_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.224898 synapseclient-4.1.1/synapseclient/models/services/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/services/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/services/storable_entity_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    29210 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    14031 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/models/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.224898 synapseclient-4.1.1/synapseclient/services/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28756 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/services/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/synapsePythonClient
--rw-r--r--   0 runner    (1001) docker     (127)    94445 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/team.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseclient/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.228898 synapseclient-4.1.1/synapseclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-02-29 02:59:24.000000 synapseclient-4.1.1/synapseclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-02-29 02:59:24.000000 synapseclient-4.1.1/synapseclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 02:59:24.000000 synapseclient-4.1.1/synapseclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-29 02:59:24.000000 synapseclient-4.1.1/synapseclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 02:59:15.000000 synapseclient-4.1.1/synapseclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-29 02:59:24.000000 synapseclient-4.1.1/synapseclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-29 02:59:24.000000 synapseclient-4.1.1/synapseclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 02:59:24.224898 synapseclient-4.1.1/synapseutils/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36429 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseutils/copy_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseutils/describe_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseutils/migrate_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseutils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53830 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseutils/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-02-29 02:59:09.000000 synapseclient-4.1.1/synapseutils/walk_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.906554 synapseclient-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 00:44:41.000000 synapseclient-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14561 2024-04-19 00:44:54.906554 synapseclient-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-19 00:44:41.000000 synapseclient-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 00:44:41.000000 synapseclient-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-19 00:44:54.906554 synapseclient-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-19 00:44:41.000000 synapseclient-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.886554 synapseclient-4.2.0/synapseclient/
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/.synapseConfig
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63395 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17293 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.890554 synapseclient-4.2.0/synapseclient/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/api/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/api/entity_bundle_services_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/api/entity_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/api/file_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)   254964 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.890554 synapseclient-4.2.0/synapseclient/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19498 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.890554 synapseclient-4.2.0/synapseclient/core/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/constants/concrete_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/constants/config_file_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/constants/limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/constants/method_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.894554 synapseclient-4.2.0/synapseclient/core/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/credentials/cred_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10919 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/credentials/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/cumulative_transfer_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/dozer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/logging_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.894554 synapseclient-4.2.0/synapseclient/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/models/custom_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/models/dict_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/models/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.894554 synapseclient-4.2.0/synapseclient/core/multithread_download/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/multithread_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15712 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/multithread_download/download_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/pool_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/remote_file_storage_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22468 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/sts_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.894554 synapseclient-4.2.0/synapseclient/core/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24662 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30626 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/multipart_upload_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/upload_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15164 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/upload_functions_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/upload/upload_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45377 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/core/version_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34756 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9581 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.894554 synapseclient-4.2.0/synapseclient/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51831 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseclient/models/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/mixins/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/mixins/storable_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseclient/models/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/access_control_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/activity_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/annotations_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/file_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/folder_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/project_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/storable_container_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/table_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/team_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/protocols/user_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseclient/models/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/services/storable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/services/storable_entity_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29342 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/models/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseclient/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28756 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/services/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-19 00:44:42.000000 synapseclient-4.2.0/synapseclient/synapsePythonClient
+-rw-r--r--   0 runner    (1001) docker     (127)    94315 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseclient/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14561 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:44:48.000000 synapseclient-4.2.0/synapseclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 00:44:54.000000 synapseclient-4.2.0/synapseclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:44:54.898554 synapseclient-4.2.0/synapseutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37471 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/copy_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/describe_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/migrate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-19 00:44:41.000000 synapseclient-4.2.0/synapseutils/walk_functions.py
```

### Comparing `synapseclient-4.1.1/PKG-INFO` & `synapseclient-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapseclient
-Version: 4.1.1
+Version: 4.2.0
 Summary: A client for Synapse, a collaborative, open-source research platform that allows teams to share data, track analyses, and collaborate.
 Home-page: https://www.synapse.org
 Author: The Synapse Engineering Team
 Author-email: platform@sagebase.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/Sage-Bionetworks/synapsePythonClient
 Project-URL: Tracker, https://github.com/Sage-Bionetworks/synapsePythonClient/issues
@@ -32,14 +32,20 @@
 Requires-Dist: requests<3.0,>=2.22.0
 Requires-Dist: urllib3<2,>=1.26.18
 Requires-Dist: deprecated<2.0,>=1.2.4
 Requires-Dist: opentelemetry-api~=1.21.0
 Requires-Dist: opentelemetry-sdk~=1.21.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-http~=1.21.0
 Requires-Dist: nest-asyncio~=1.6.0
+Requires-Dist: asyncio-atexit~=1.0.1
+Requires-Dist: httpx~=0.27.0
+Requires-Dist: tqdm<5.0,>=4.66.2
+Requires-Dist: loky~=3.0.0
+Requires-Dist: async-lru~=2.0.4
+Requires-Dist: psutil~=5.9.8
 Provides-Extra: dev
 Requires-Dist: pytest<7.0,>=6.0.0; extra == "dev"
 Requires-Dist: pytest-mock<4.0,>=3.0; extra == "dev"
 Requires-Dist: pytest-socket~=0.6.0; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.19; extra == "dev"
 Requires-Dist: flake8<4.0,>=3.7.0; extra == "dev"
 Requires-Dist: pytest-xdist[psutil]<3.0.0,>=2.2; extra == "dev"
```

### Comparing `synapseclient-4.1.1/README.md` & `synapseclient-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/setup.cfg` & `synapseclient-4.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,20 @@
 	requests>=2.22.0,<3.0
 	urllib3>=1.26.18,<2
 	deprecated>=1.2.4,<2.0
 	opentelemetry-api~=1.21.0
 	opentelemetry-sdk~=1.21.0
 	opentelemetry-exporter-otlp-proto-http~=1.21.0
 	nest-asyncio~=1.6.0
+	asyncio-atexit~=1.0.1
+	httpx~=0.27.0
+	tqdm>=4.66.2,<5.0
+	loky~=3.0.0
+	async-lru~=2.0.4
+	psutil~=5.9.8
 tests_require = 
 	pytest>=6.0.0,<7.0
 	pytest-mock>=3.0,<4.0
 	pytest-socket~=0.6.0
 	pytest-asyncio~=0.19
 	flake8>=3.7.0,<4.0
 	pytest-xdist[psutil]>=2.2,<3.0.0
```

### Comparing `synapseclient-4.1.1/setup.py` & `synapseclient-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/.synapseConfig` & `synapseclient-4.2.0/synapseclient/.synapseConfig`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/__init__.py` & `synapseclient-4.2.0/synapseclient/__init__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/__main__.py` & `synapseclient-4.2.0/synapseclient/__main__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/activity.py` & `synapseclient-4.2.0/synapseclient/activity.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/annotations.py` & `synapseclient-4.2.0/synapseclient/annotations.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/api/annotations.py` & `synapseclient-4.2.0/synapseclient/api/annotations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 """
 The purpose of this module is to provide any functions that are needed to interact with
 annotations that are not cleanly provided by the synapseclient library.
 """
+
 import json
 
 from dataclasses import asdict
 
 from typing import TYPE_CHECKING, Optional
-from synapseclient import Synapse
+
 from synapseclient.annotations import _convert_to_annotations_list
 
 if TYPE_CHECKING:
     from synapseclient.models import Annotations
+    from synapseclient import Synapse
 
 
 def set_annotations(
     annotations: "Annotations",
-    synapse_client: Optional[Synapse] = None,
+    synapse_client: Optional["Synapse"] = None,
 ):
     """Call to synapse and set the annotations for the given input.
 
     Arguments:
-        annotations: The annotations to set. This is expected to have the id, etag, and annotations filled in.
-        synapse_client: If not passed in or None this will use the last client from the `.login()` method.
+        annotations: The annotations to set. This is expected to have the id, etag,
+            and annotations filled in.
+        synapse_client: If not passed in or None this will use the last client from
+            the `.login()` method.
 
     Returns: The annotations set in Synapse.
     """
     annotations_dict = asdict(annotations)
 
-    synapse_annotations = _convert_to_annotations_list(annotations_dict["annotations"])
+    synapse_annotations = _convert_to_annotations_list(
+        annotations_dict["annotations"] or {}
+    )
+    from synapseclient import Synapse
 
     return Synapse.get_client(synapse_client=synapse_client).restPUT(
         f"/entity/{annotations.id}/annotations2",
         body=json.dumps(
             {
                 "id": annotations.id,
                 "etag": annotations.etag,
```

### Comparing `synapseclient-4.1.1/synapseclient/client.py` & `synapseclient-4.2.0/synapseclient/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 The `Synapse` object encapsulates a connection to the Synapse service and is used for building projects, uploading and
 retrieving data, and recording provenance of data analysis.
 """
+import asyncio
+import asyncio_atexit
 import collections
 import collections.abc
 import configparser
 import csv
 import numbers
 import threading
 import errno
@@ -23,17 +25,21 @@
 import time
 import typing
 import urllib.parse as urllib_urlparse
 import urllib.request as urllib_request
 import warnings
 import webbrowser
 import zipfile
+import httpx
 
 from deprecated import deprecated
 
+from concurrent.futures import ThreadPoolExecutor
+from loky import get_reusable_executor
+
 import synapseclient
 from .annotations import (
     from_synapse_annotations,
     to_synapse_annotations,
     Annotations,
     convert_old_annotation_json,
     check_annotations_changed,
@@ -86,47 +92,54 @@
 )
 from synapseclient.core.logging_setup import (
     DEFAULT_LOGGER_NAME,
     DEBUG_LOGGER_NAME,
     SILENT_LOGGER_NAME,
 )
 from synapseclient.core.version_check import version_check
-from synapseclient.core.pool_provider import DEFAULT_NUM_THREADS
+from synapseclient.core.pool_provider import DEFAULT_NUM_THREADS, get_executor
 from synapseclient.core.utils import (
     id_of,
     get_properties,
     MB,
     is_json,
     extract_synapse_id_from_query,
     find_data_file_handle,
     extract_zip_file_to_directory,
     is_integer,
     require_param,
 )
 from synapseclient.core.retry import (
     with_retry,
+    with_retry_time_based_async,
     DEFAULT_RETRY_STATUS_CODES,
     RETRYABLE_CONNECTION_ERRORS,
     RETRYABLE_CONNECTION_EXCEPTIONS,
 )
 from synapseclient.core import sts_transfer
-from synapseclient.core.upload.multipart_upload import (
-    multipart_upload_file,
-    multipart_upload_string,
+from synapseclient.core.upload.multipart_upload_async import (
+    multipart_upload_file_async,
+    multipart_upload_string_async,
 )
 from synapseclient.core.remote_file_storage_wrappers import S3ClientWrapper, SFTPWrapper
 from synapseclient.core.upload.upload_functions import (
     upload_file_handle,
+)
+from synapseclient.core.upload.upload_functions_async import (
+    upload_file_handle as upload_file_handle_async,
     upload_synapse_s3,
 )
 from synapseclient.core.dozer import doze
+from synapseclient.core.async_utils import wrap_async_to_sync
 
-from typing import Union, Dict, List, Optional, Tuple
+from typing import Any, Union, Dict, List, Optional, Tuple
 from synapseclient.core.models.permission import Permissions
 from opentelemetry import trace
+from opentelemetry.trace import SpanKind
+
 
 tracer = trace.get_tracer("synapseclient")
 
 PRODUCTION_ENDPOINTS = {
     "repoEndpoint": "https://repo-prod.prod.sagebase.org/repo/v1",
     "authEndpoint": "https://auth-prod.prod.sagebase.org/auth/v1",
     "fileHandleEndpoint": "https://file-prod.prod.sagebase.org/file/v1",
@@ -161,14 +174,20 @@
     "retry_exceptions": RETRYABLE_CONNECTION_EXCEPTIONS,
     "retries": 60,  # Retries for up to about 30 minutes
     "wait": 1,
     "max_wait": 30,
     "back_off": 2,
 }
 
+STANDARD_RETRY_ASYNC_PARAMS = {
+    "retry_status_codes": DEFAULT_RETRY_STATUS_CODES,
+    "retry_errors": RETRYABLE_CONNECTION_ERRORS,
+    "retry_exceptions": RETRYABLE_CONNECTION_EXCEPTIONS,
+}
+
 # Add additional mimetypes
 mimetypes.add_type("text/x-r", ".R", strict=False)
 mimetypes.add_type("text/x-r", ".r", strict=False)
 mimetypes.add_type("text/tab-separated-values", ".maf", strict=False)
 mimetypes.add_type("text/tab-separated-values", ".bed5", strict=False)
 mimetypes.add_type("text/tab-separated-values", ".bed", strict=False)
 mimetypes.add_type("text/tab-separated-values", ".vcf", strict=False)
@@ -233,27 +252,29 @@
             syn = synapseclient.login()
 
     """
 
     _synapse_client = None
 
     # TODO: add additional boolean for write to disk?
-    @tracer.start_as_current_span("Synapse::__init__")
     def __init__(
         self,
         repoEndpoint: str = None,
         authEndpoint: str = None,
         fileHandleEndpoint: str = None,
         portalEndpoint: str = None,
         debug: bool = None,
         skip_checks: bool = False,
         configPath: str = CONFIG_FILE,
         requests_session: requests.Session = None,
         cache_root_dir: str = None,
         silent: bool = None,
+        requests_session_async_synapse: httpx.AsyncClient = None,
+        requests_session_storage: httpx.Client = None,
+        asyncio_event_loop: asyncio.AbstractEventLoop = None,
     ) -> "Synapse":
         """
         Initialize Synapse object
 
         Arguments:
             repoEndpoint:       Location of Synapse repository.
             authEndpoint:       Location of authentication service.
@@ -262,20 +283,80 @@
             debug:              Print debugging messages if True.
             skip_checks:        Skip version and endpoint checks.
             configPath:         Path to config File with setting for Synapse.
             requests_session:   A custom [requests.Session object](https://requests.readthedocs.io/en/latest/user/advanced/) that this Synapse instance will use
                                 when making http requests.
             cache_root_dir:     Root directory for storing cache data.
             silent:             Suppresses message.
+            requests_session_async_synapse: The HTTPX Async client for interacting with
+                Synapse services.
+            requests_session_storage: The HTTPX client for interacting with
+                storage providers like AWS S3 and Google Cloud.
+            asyncio_event_loop: The event loop that is going to be used while executing
+                this code. This is optional and only used when you are manually
+                specifying an async HTTPX client.
 
         Raises:
             ValueError: Warn for non-boolean debug value.
         """
         self._requests_session = requests_session or requests.Session()
 
+        # `requests_session_async_synapse` and the thread pools are being stored in
+        # a dict based on the current running event loop. This is to ensure that the
+        # connection pooling is maintained within the same event loop. This is to
+        # prevent the connection pooling from being shared across different event loops.
+        if requests_session_async_synapse and asyncio_event_loop:
+            self._requests_session_async_synapse = {
+                asyncio_event_loop: requests_session_async_synapse
+            }
+        else:
+            self._requests_session_async_synapse = {}
+
+        span_dict: Dict[httpx.Request, trace.Span] = {}
+
+        def log_request(request: httpx.Request) -> None:
+            """
+            Log the HTTPX request to an otel span.
+
+            Arguments:
+                request: The HTTPX request object.
+            """
+            # Don't log the query string as it will contain tokens
+            url_without_query_string: httpx.URL = request.url.copy_with(query=None)
+            current_span = trace.get_current_span()
+            if current_span.is_recording():
+                span = tracer.start_span(
+                    f"{request.method} {url_without_query_string}", kind=SpanKind.CLIENT
+                )
+                span.set_attributes(
+                    {
+                        "url": str(url_without_query_string),
+                        "http.method": request.method,
+                    }
+                )
+                span_dict.update({request: span})
+
+        def log_response(response: httpx.Response) -> None:
+            """
+            Log the HTTPX response to an otel span.
+
+            Arguments:
+                response: The HTTPX response object.
+            """
+            span = span_dict.pop(response.request, None)
+            if span and span.is_recording():
+                span.set_attribute("http.response.status_code", response.status_code)
+                span.end()
+
+        event_hooks = {"request": [log_request], "response": [log_response]}
+        httpx_timeout = httpx.Timeout(70)
+        self._requests_session_storage = requests_session_storage or httpx.Client(
+            timeout=httpx_timeout, event_hooks=event_hooks
+        )
+
         cache_root_dir = (
             cache.CACHE_ROOT_DIR if cache_root_dir is None else cache_root_dir
         )
 
         config_debug = None
         # Check for a config file
         self.configPath = configPath
@@ -315,16 +396,176 @@
         self.table_query_backoff = 1.1
         self.table_query_max_sleep = 20
         self.table_query_timeout = 600  # in seconds
         self.multi_threaded = True  # if set to True, multi threaded download will be used for http and https URLs
 
         transfer_config = self._get_transfer_config()
         self.max_threads = transfer_config["max_threads"]
+        self._thread_executor = {}
+        self._process_executor = {}
+        self._md5_semaphore = {}
         self.use_boto_sts_transfers = transfer_config["use_boto_sts"]
 
+    def _get_requests_session_async_synapse(
+        self, asyncio_event_loop: asyncio.AbstractEventLoop
+    ) -> httpx.AsyncClient:
+        """
+        httpx.AsyncClient can only use connection pooling within the same event loop.
+        As a result an `atexit` handler is used to close the connection when the event
+        loop is closed. It will also delete the attribute from the object to prevent
+        it from being reused in the future.
+
+        Further documentation can be found here:
+        <https://github.com/encode/httpx/discussions/2959>
+
+
+        As a result of this issue: It is recommended to use the same event loop for all
+        requests. This means to enter into an event loop before making any requests.
+
+        This is expected to be called from within an AsyncIO loop.
+        """
+        if (
+            hasattr(self, "_requests_session_async_synapse")
+            and asyncio_event_loop in self._requests_session_async_synapse
+            and self._requests_session_async_synapse[asyncio_event_loop] is not None
+        ):
+            return self._requests_session_async_synapse[asyncio_event_loop]
+
+        async def close_connection() -> None:
+            """Close connection when event loop exits"""
+            await self._requests_session_async_synapse[asyncio_event_loop].aclose()
+            del self._requests_session_async_synapse[asyncio_event_loop]
+
+        httpx_timeout = httpx.Timeout(70)
+        span_dict: Dict[httpx.Request, trace.Span] = {}
+
+        async def log_request(request: httpx.Request) -> None:
+            """
+            Log the HTTPX request to an otel span.
+
+            Arguments:
+                request: The HTTPX request object.
+            """
+            current_span = trace.get_current_span()
+            if current_span.is_recording():
+                span = tracer.start_span(
+                    f"{request.method} {request.url}", kind=SpanKind.CLIENT
+                )
+                span.set_attributes(
+                    {"url": str(request.url), "http.method": request.method}
+                )
+                self._attach_rest_data_to_otel(
+                    request.method, str(request.url), request.content, span
+                )
+                span_dict.update({request: span})
+
+        async def log_response(response: httpx.Response) -> None:
+            """
+            Log the HTTPX response to an otel span.
+
+            Arguments:
+                response: The HTTPX response object.
+            """
+            span = span_dict.pop(response.request, None)
+            if span and span.is_recording():
+                span.set_attribute("http.response.status_code", response.status_code)
+                span.end()
+
+        event_hooks = {"request": [log_request], "response": [log_response]}
+        self._requests_session_async_synapse.update(
+            {
+                asyncio_event_loop: httpx.AsyncClient(
+                    limits=httpx.Limits(max_connections=25),
+                    timeout=httpx_timeout,
+                    event_hooks=event_hooks,
+                )
+            }
+        )
+
+        asyncio_atexit.register(close_connection)
+        return self._requests_session_async_synapse[asyncio_event_loop]
+
+    def _get_thread_pool_executor(
+        self, asyncio_event_loop: asyncio.AbstractEventLoop
+    ) -> ThreadPoolExecutor:
+        """
+        Retrieve the thread pool executor for the Synapse client. Or create a new one if
+        it does not exist. This executor is used for concurrent uploads of data to
+        storage providers like AWS S3 and Google Cloud Storage.
+
+        This is expected to be called from within an AsyncIO loop.
+        """
+        if (
+            hasattr(self, "_thread_executor")
+            and asyncio_event_loop in self._thread_executor
+            and self._thread_executor[asyncio_event_loop] is not None
+        ):
+            return self._thread_executor[asyncio_event_loop]
+
+        def close_pool() -> None:
+            """Close pool when event loop exits"""
+            self._thread_executor[asyncio_event_loop].shutdown(wait=True)
+            del self._thread_executor[asyncio_event_loop]
+
+        self._thread_executor.update(
+            {asyncio_event_loop: get_executor(thread_count=self.max_threads)}
+        )
+
+        asyncio_atexit.register(close_pool)
+        return self._thread_executor[asyncio_event_loop]
+
+    def _get_process_pool_executor(self, asyncio_event_loop: asyncio.AbstractEventLoop):
+        """
+        Retrieve the process pool executor for the Synapse client. Or create a new one
+        if it does not exist. This executor is used for parallel processing of data.
+
+        This is expected to be called from within an AsyncIO loop.
+
+        Note: Within Windows a ProcessPoolExecutor requires that the initial entry point
+        into the code be within a `if __name__ == "__main__":` block. This is not
+        possible within the current codebase as it would require everyone using this
+        library to have this as their entry point. As a result, the ProcessPoolExecutor
+        will not work within Windows.
+
+        To get around this Windows limitation this is using this package:
+        https://github.com/joblib/loky
+        """
+        if (
+            hasattr(self, "_process_executor")
+            and asyncio_event_loop in self._process_executor
+            and self._process_executor[asyncio_event_loop] is not None
+        ):
+            return self._process_executor[asyncio_event_loop]
+
+        self._process_executor.update({asyncio_event_loop: get_reusable_executor(1)})
+
+        return self._process_executor[asyncio_event_loop]
+
+    def _get_md5_semaphore(
+        self, asyncio_event_loop: asyncio.AbstractEventLoop
+    ) -> asyncio.Semaphore:
+        """
+        Retrieve the semaphore for the Synapse client. Or create a new one if it does not
+        exist. This semaphore is used to ensure that only one process is calculating the
+        MD5 hash at a time. This is to prevent the custom process pool executor from
+        thrashing or handling the waiting. We should let asyncio handle the waiting.
+
+        This is expected to be called from within an AsyncIO loop.
+        """
+        if (
+            hasattr(self, "_md5_semaphore")
+            and asyncio_event_loop in self._md5_semaphore
+            and self._md5_semaphore[asyncio_event_loop] is not None
+        ):
+            return self._md5_semaphore[asyncio_event_loop]
+
+        self._md5_semaphore.update({asyncio_event_loop: asyncio.Semaphore(1)})
+
+        return self._md5_semaphore[asyncio_event_loop]
+
     # initialize logging
     def _init_logger(self):
         """
         Initialize logging
         """
         logger_name = (
             SILENT_LOGGER_NAME
@@ -376,15 +617,14 @@
         self._max_threads = min(max(value, 1), MAX_THREADS_CAP)
 
     @property
     def username(self) -> Union[str, None]:
         # for backwards compatability when username was a part of the Synapse object and not in credentials
         return self.credentials.username if self.credentials is not None else None
 
-    @tracer.start_as_current_span("Synapse::getConfigFile")
     @functools.lru_cache()
     def getConfigFile(self, configPath: str) -> configparser.RawConfigParser:
         """
         Retrieves the client configuration information.
 
         Arguments:
             configPath:  Path to configuration file on local file system
@@ -398,15 +638,14 @@
             config.read(configPath)  # Does not fail if the file does not exist
             return config
         except configparser.Error as ex:
             raise ValueError(
                 "Error parsing Synapse config file: {}".format(configPath)
             ) from ex
 
-    @tracer.start_as_current_span("Synapse::setEndpoints")
     def setEndpoints(
         self,
         repoEndpoint: str = None,
         authEndpoint: str = None,
         fileHandleEndpoint: str = None,
         portalEndpoint: str = None,
         skip_checks: bool = False,
@@ -458,15 +697,14 @@
                     endpoints[point] = response.headers["location"]
 
         self.repoEndpoint = endpoints["repoEndpoint"]
         self.authEndpoint = endpoints["authEndpoint"]
         self.fileHandleEndpoint = endpoints["fileHandleEndpoint"]
         self.portalEndpoint = endpoints["portalEndpoint"]
 
-    @tracer.start_as_current_span("Synapse::login")
     def login(
         self,
         email: str = None,
         silent: bool = False,
         authToken: str = None,
         cache_client: bool = True,
     ) -> None:
@@ -618,15 +856,14 @@
                             f"Invalid transfer.use_boto_sts config setting {v}"
                         )
 
                     transfer_config["use_boto_sts"] = "true" == lower_v
 
         return transfer_config
 
-    @tracer.start_as_current_span("Synapse::_is_logged_in")
     def _is_logged_in(self) -> bool:
         """
         Test whether the user is logged in to Synapse.
 
         Returns:
             Boolean value indicating current user's login status
         """
@@ -865,15 +1102,14 @@
         try:
             response = self.restGET(f"/user/{userid}/bundle?mask={mask}")
         except SynapseHTTPError as ex:
             if ex.response.status_code == 404:
                 return None
         return response
 
-    @tracer.start_as_current_span("Synapse::is_certified")
     def is_certified(self, user: typing.Union[str, int]) -> bool:
         """Determines whether a Synapse user is a certified user.
 
         Arguments:
             user: Synapse username or Id
 
         Returns:
@@ -890,15 +1126,14 @@
             return certification_status["passed"]
         except SynapseHTTPError as ex:
             if ex.response.status_code == 404:
                 # user hasn't taken the quiz
                 return False
             raise
 
-    @tracer.start_as_current_span("Synapse::is_synapse_id")
     def is_synapse_id(self, syn_id: str) -> bool:
         """Checks if given synID is valid (attached to actual entity?)
 
         Arguments:
             syn_id: A Synapse ID
 
         Returns:
@@ -941,15 +1176,14 @@
         if subpageId is None:
             webbrowser.open("%s#!Synapse:%s" % (self.portalEndpoint, synId))
         else:
             webbrowser.open(
                 "%s#!Wiki:%s/ENTITY/%s" % (self.portalEndpoint, synId, subpageId)
             )
 
-    @tracer.start_as_current_span("Synapse::printEntity")
     def printEntity(self, entity, ensure_ascii=True) -> None:
         """
         Pretty prints an Entity.
 
         Arguments:
             entity: The entity to be printed.
             ensure_ascii: If True, escapes all non-ASCII characters
@@ -1017,15 +1251,14 @@
         service = service_cls(self)
         return service
 
     ############################################################
     #                   Get / Store methods                    #
     ############################################################
 
-    @tracer.start_as_current_span("Synapse::get")
     def get(self, entity, **kwargs):
         """
         Gets a Synapse entity from the repository service.
 
         Arguments:
             entity:           A Synapse ID (e.g. syn123 or syn123.1, with .1 denoting version), a Synapse Entity object,
                               a plain dictionary in which 'id' maps to a Synapse ID or a local file that is stored in
@@ -1040,14 +1273,16 @@
                                 Defaults to False.
             ifcollision:      Determines how to handle file collisions.
                                 May be "overwrite.local", "keep.local", or "keep.both".
                                 Defaults to "keep.both".
             limitSearch:      A Synanpse ID used to limit the search in Synapse if entity is specified as a local
                                 file.  That is, if the file is stored in multiple locations in Synapse only the ones
                                 in the specified folder/project will be returned.
+            md5: The MD5 checksum for the file, if known. Otherwise if the file is a
+                local file, it will be calculated automatically.
 
         Returns:
             A new Synapse Entity object of the appropriate type.
 
         Example: Using this function
             Download file into cache
 
@@ -1064,15 +1299,17 @@
             Determine the provenance of a locally stored file as indicated in Synapse
 
                 entity = syn.get('/path/to/file.txt', limitSearch='syn12312')
                 print(syn.getProvenance(entity))
         """
         # If entity is a local file determine the corresponding synapse entity
         if isinstance(entity, str) and os.path.isfile(entity):
-            bundle = self._getFromFile(entity, kwargs.pop("limitSearch", None))
+            bundle = self._getFromFile(
+                entity, kwargs.pop("limitSearch", None), md5=kwargs.get("md5", None)
+            )
             kwargs["downloadFile"] = False
             kwargs["path"] = entity
 
         elif isinstance(entity, str) and not utils.is_synapse_id_str(entity):
             raise SynapseFileNotFoundError(
                 (
                     "The parameter %s is neither a local file path "
@@ -1133,32 +1370,36 @@
                 'the file name. Click "Request Access", and then review and fulfill the file '
                 "download requirement(s).\n"
             )
             if downloadFile and bundle.get("entityType") not in ("project", "folder"):
                 raise SynapseUnmetAccessRestrictions(warning_message)
             warnings.warn(warning_message)
 
-    @tracer.start_as_current_span("Synapse::_getFromFile")
-    def _getFromFile(self, filepath: str, limitSearch: str = None) -> Dict[str, dict]:
+    def _getFromFile(
+        self, filepath: str, limitSearch: str = None, md5: str = None
+    ) -> Dict[str, dict]:
         """
         Gets a Synapse entityBundle based on the md5 of a local file.
         See [get][synapseclient.Synapse.get].
 
         Arguments:
             filepath:    The path to local file
             limitSearch: Limits the places in Synapse where the file is searched for.
+            md5: The MD5 checksum for the file, if known. Otherwise if the file is a
+                local file, it will be calculated automatically.
+
 
         Raises:
             SynapseFileNotFoundError: If the file is not in Synapse.
 
         Returns:
             A Synapse entityBundle
         """
         results = self.restGET(
-            "/entity/md5/%s" % utils.md5_for_file(filepath).hexdigest()
+            "/entity/md5/%s" % (md5 or utils.md5_for_file(filepath).hexdigest())
         )["results"]
         if limitSearch is not None:
             # Go through and find the path of every entity found
             paths = [self.restGET("/entity/%s/path" % ent["id"]) for ent in results]
             # Filter out all entities whose path does not contain limitSearch
             results = [
                 ent
@@ -1182,15 +1423,14 @@
         entity = results[0]
 
         bundle = self._getEntityBundle(entity, version=entity["versionNumber"])
         self.cache.add(bundle["entity"]["dataFileHandleId"], filepath)
 
         return bundle
 
-    @tracer.start_as_current_span("Synapse::move")
     def move(self, entity, new_parent):
         """
         Move a Synapse entity to a new container.
 
         Arguments:
             entity:     A Synapse ID, a Synapse Entity object, or a local file that is stored in Synapse
             new_parent: The new parent container (Folder or Project) to which the entity should be moved.
@@ -1321,15 +1561,14 @@
         download_dir = os.path.expandvars(os.path.expanduser(downloadLocation))
         if os.path.isfile(download_dir):
             raise ValueError(
                 "Parameter 'downloadLocation' should be a directory, not a file."
             )
         return download_dir
 
-    @tracer.start_as_current_span("Synapse::_download_file_entity")
     def _download_file_entity(
         self,
         downloadLocation: str,
         entity: Entity,
         ifcollision: str,
         submission: str,
     ) -> None:
@@ -1472,29 +1711,29 @@
             else:
                 raise ValueError(
                     'Invalid parameter: "%s" is not a valid value '
                     'for "ifcollision"' % ifcollision
                 )
         return downloadPath
 
-    @tracer.start_as_current_span("Synapse::store")
     def store(
         self,
         obj,
         *,
         createOrUpdate=True,
         forceVersion=True,
         versionLabel=None,
         isRestricted=False,
         activity=None,
         used=None,
         executed=None,
         activityName=None,
         activityDescription=None,
         set_annotations=True,
+        async_file_handle_upload: bool = True,
     ):
         """
         Creates a new Entity or updates an existing Entity, uploading any files in the process.
 
         Arguments:
             obj: A Synapse Entity, Evaluation, or Wiki
             used: The Entity, Synapse ID, or URL used to create the object (can also be a list of these)
@@ -1509,14 +1748,19 @@
                             has changed.
             versionLabel: Arbitrary string used to label the version.
             isRestricted: If set to true, an email will be sent to the Synapse access control team to start the
                             process of adding terms-of-use or review board approval for this entity.
                             You will be contacted with regards to the specific data being restricted and the
                             requirements of access.
             set_annotations: If True, set the annotations on the entity. If False, do not set the annotations.
+            async_file_handle_upload: Temporary feature flag that will be removed at an
+                unannounced later date. This is used during the Synapse Utils
+                syncToSynapse to disable the async file handle upload. The is because
+                the multi-threaded logic in the syncToSynapse is not compatible with
+                the async file handle upload.
 
         Returns:
             A Synapse Entity, Evaluation, or Wiki
 
         Example: Using this function
             Creating a new Project:
 
@@ -1667,26 +1911,46 @@
                 if not parent_id_for_upload and bundle and bundle.get("entity", None):
                     parent_id_for_upload = bundle["entity"]["parentId"]
 
                 if not parent_id_for_upload:
                     raise SynapseMalformedEntityError(
                         "Entities of type File must have a parentId."
                     )
-                fileHandle = upload_file_handle(
-                    self,
-                    parent_id_for_upload,
-                    local_state["path"]
-                    if (synapseStore or local_state_fh.get("externalURL") is None)
-                    else local_state_fh.get("externalURL"),
-                    synapseStore=synapseStore,
-                    md5=local_file_md5_hex or local_state_fh.get("contentMd5"),
-                    file_size=local_state_fh.get("contentSize"),
-                    mimetype=local_state_fh.get("contentType"),
-                    max_threads=self.max_threads,
-                )
+
+                if async_file_handle_upload:
+                    fileHandle = wrap_async_to_sync(
+                        upload_file_handle_async(
+                            self,
+                            parent_id_for_upload,
+                            local_state["path"]
+                            if (
+                                synapseStore
+                                or local_state_fh.get("externalURL") is None
+                            )
+                            else local_state_fh.get("externalURL"),
+                            synapse_store=synapseStore,
+                            md5=local_file_md5_hex or local_state_fh.get("contentMd5"),
+                            file_size=local_state_fh.get("contentSize"),
+                            mimetype=local_state_fh.get("contentType"),
+                        ),
+                        self,
+                    )
+                else:
+                    fileHandle = upload_file_handle(
+                        self,
+                        parent_id_for_upload,
+                        local_state["path"]
+                        if (synapseStore or local_state_fh.get("externalURL") is None)
+                        else local_state_fh.get("externalURL"),
+                        synapseStore=synapseStore,
+                        md5=local_file_md5_hex or local_state_fh.get("contentMd5"),
+                        file_size=local_state_fh.get("contentSize"),
+                        mimetype=local_state_fh.get("contentType"),
+                        max_threads=self.max_threads,
+                    )
                 properties["dataFileHandleId"] = fileHandle["id"]
                 local_state["_file_handle"] = fileHandle
 
             elif "dataFileHandleId" not in properties:
                 # Handle the case where the Entity lacks an ID
                 # But becomes an update() due to conflict
                 properties["dataFileHandleId"] = bundle["entity"]["dataFileHandleId"]
@@ -1825,15 +2089,14 @@
             {
                 "synapse.id": return_data.get("id", ""),
                 "synapse.concrete_type": entity.get("concreteType", ""),
             }
         )
         return return_data
 
-    @tracer.start_as_current_span("Synapse::_createAccessRequirementIfNone")
     def _createAccessRequirementIfNone(self, entity: Union[Entity, str]) -> None:
         """
         Checks to see if the given entity has access requirements. If not, then one is added
 
         Arguments:
             entity: A Synapse ID or a Synapse Entity object
         """
@@ -1921,15 +2184,14 @@
             uri = f"/entity/{id_of(entity)}/version/{int(version):d}/bundle2"
         else:
             uri = f"/entity/{id_of(entity)}/bundle2"
         bundle = self.restPOST(uri, body=json.dumps(requestedObjects))
 
         return bundle
 
-    @tracer.start_as_current_span("Synapse::delete")
     def delete(
         self,
         obj,
         version=None,
     ):
         """
         Removes an object from Synapse.
@@ -1973,15 +2235,14 @@
         """
         if user_id not in self._user_name_cache:
             self._user_name_cache[user_id] = utils.extract_user_name(
                 self.getUserProfile(user_id)
             )
         return self._user_name_cache[user_id]
 
-    @tracer.start_as_current_span("Synapse::_list")
     def _list(
         self,
         parent: str,
         recursive: bool = False,
         long_format: bool = False,
         show_modified: bool = False,
         indent: float = 0,
@@ -2072,16 +2333,19 @@
                         automatically.
             file_type: The MIME type the file, if known. Otherwise if the file is a local file, it will be calculated
                         automatically.
 
         Returns:
             A dict of a new FileHandle as a dict that represents the uploaded file
         """
-        return upload_file_handle(
-            self, parent, path, synapseStore, md5, file_size, mimetype
+        return wrap_async_to_sync(
+            upload_file_handle_async(
+                self, parent, path, synapseStore, md5, file_size, mimetype
+            ),
+            self,
         )
 
     ############################################################
     #                  Download List                           #
     ############################################################
     def clear_download_list(self):
         """Clear all files from download list"""
@@ -2133,15 +2397,14 @@
                 "isFirstLineHeader": header,
             },
         }
         return self._waitForAsync(
             uri="/download/list/manifest/async", request=request_body
         )
 
-    @tracer.start_as_current_span("Synapse::get_download_list_manifest")
     def get_download_list_manifest(self):
         """Get the path of the download list manifest file
 
         Returns:
             Path of download list manifest file
         """
         manifest = self._generate_manifest_from_download_list()
@@ -2159,15 +2422,14 @@
             expected_md5=file_result["fileHandle"].get("contentMd5"),
         )
         trace.get_current_span().set_attributes(
             {"synapse.file_handle_id": file_result["fileHandleId"]}
         )
         return downloaded_path
 
-    @tracer.start_as_current_span("Synapse::get_download_list")
     def get_download_list(self, downloadLocation: str = None) -> str:
         """Download all files from your Synapse download list
 
         Arguments:
             downloadLocation: Directory to download files to.
 
         Returns:
@@ -2246,15 +2508,14 @@
         # See [PLFM-1874](https://sagebionetworks.jira.com/browse/PLFM-1874) for more details.
         if version:
             uri = f"/entity/{id_of(entity)}/version/{str(version)}/annotations2"
         else:
             uri = f"/entity/{id_of(entity)}/annotations2"
         return self.restGET(uri)
 
-    @tracer.start_as_current_span("Synapse::get_annotations")
     def get_annotations(
         self, entity: typing.Union[str, Entity], version: typing.Union[str, int] = None
     ) -> Annotations:
         """
         Retrieve annotations for an Entity from the Synapse Repository as a Python dict.
 
         Note that collapsing annotations from the native Synapse format to a Python dict may involve some loss of
@@ -2265,15 +2526,14 @@
             version: The version of the Entity to retrieve.
 
         Returns:
             A [synapseclient.annotations.Annotations][] object, a dict that also has id and etag attributes
         """
         return from_synapse_annotations(self._getRawAnnotations(entity, version))
 
-    @tracer.start_as_current_span("Synapse::set_annotations")
     def set_annotations(self, annotations: Annotations):
         """
         Store annotations for an Entity in the Synapse Repository.
 
         Arguments:
             annotations: A [synapseclient.annotations.Annotations][] of annotation names and values,
                             with the id and etag attribute set
@@ -2358,38 +2618,36 @@
         Yields:
             An iterator that shows all the children of the container.
 
         Also see:
 
         - [synapseutils.walk][]
         """
-        with tracer.start_as_current_span("Synapse::getChildren"):
-            parentId = id_of(parent) if parent is not None else None
+        parentId = id_of(parent) if parent is not None else None
 
-            trace.get_current_span().set_attributes({"synapse.parent_id": parentId})
-            entityChildrenRequest = {
-                "parentId": parentId,
-                "includeTypes": includeTypes,
-                "sortBy": sortBy,
-                "sortDirection": sortDirection,
-                "nextPageToken": None,
-            }
-            entityChildrenResponse = {"nextPageToken": "first"}
-            while entityChildrenResponse.get("nextPageToken") is not None:
-                entityChildrenResponse = self.restPOST(
-                    "/entity/children", body=json.dumps(entityChildrenRequest)
-                )
-                for child in entityChildrenResponse["page"]:
-                    yield child
-                if entityChildrenResponse.get("nextPageToken") is not None:
-                    entityChildrenRequest["nextPageToken"] = entityChildrenResponse[
-                        "nextPageToken"
-                    ]
+        trace.get_current_span().set_attributes({"synapse.parent_id": parentId})
+        entityChildrenRequest = {
+            "parentId": parentId,
+            "includeTypes": includeTypes,
+            "sortBy": sortBy,
+            "sortDirection": sortDirection,
+            "nextPageToken": None,
+        }
+        entityChildrenResponse = {"nextPageToken": "first"}
+        while entityChildrenResponse.get("nextPageToken") is not None:
+            entityChildrenResponse = self.restPOST(
+                "/entity/children", body=json.dumps(entityChildrenRequest)
+            )
+            for child in entityChildrenResponse["page"]:
+                yield child
+            if entityChildrenResponse.get("nextPageToken") is not None:
+                entityChildrenRequest["nextPageToken"] = entityChildrenResponse[
+                    "nextPageToken"
+                ]
 
-    @tracer.start_as_current_span("Synapse::md5Query")
     def md5Query(self, md5):
         """
         Find the Entities which have attached file(s) which have the given MD5 hash.
 
         Arguments:
             md5: The MD5 to query for (hexadecimal string)
 
@@ -2509,15 +2767,14 @@
             supplementalMessage = (
                 "Please be more specific" if totalResults > 1 else "No matches"
             )
             raise SynapseError(
                 "Unknown Synapse user (%s).  %s." % (principalId, supplementalMessage)
             )
 
-    @tracer.start_as_current_span("Synapse::get_acl")
     def get_acl(
         self,
         entity: Union[Entity, Evaluation, str, collections.abc.Mapping],
         principal_id: str = None,
     ) -> typing.List[str]:
         """
         Get the [ACL](https://rest-docs.synapse.org/rest/org/
@@ -2568,15 +2825,14 @@
                 )
             ):
                 effective_permission_set = effective_permission_set.union(
                     permissions["accessType"]
                 )
         return list(effective_permission_set)
 
-    @tracer.start_as_current_span("Synapse::getPermissions")
     @deprecated(
         version="4.0.0",
         reason="deprecated and replaced with synapseclient.Synapse.get_acl",
     )
     def getPermissions(
         self,
         entity: Union[Entity, Evaluation, str, collections.abc.Mapping],
@@ -2597,15 +2853,14 @@
                 ['READ', 'UPDATE', 'CREATE', 'DELETE', 'DOWNLOAD', 'MODERATE',
                 'CHANGE_PERMISSIONS', 'CHANGE_SETTINGS']
                 or an empty array
         """
 
         return self.get_acl(entity=entity, principal_id=principal_id)
 
-    @tracer.start_as_current_span("Synapse::get_permissions")
     def get_permissions(
         self, entity: Union[Entity, Evaluation, str, collections.abc.Mapping]
     ) -> Permissions:
         """
         Get the [permissions](https://rest-docs.synapse.org/rest/org/
         sagebionetworks/repo/model/auth/UserEntityPermissions.html)
         that the caller has on an Entity.
@@ -2635,15 +2890,14 @@
 
         trace.get_current_span().set_attributes({"synapse.id": entity_id})
 
         url = f"/entity/{entity_id}/permissions"
         data = self.restGET(url)
         return Permissions.from_dict(data)
 
-    @tracer.start_as_current_span("Synapse::setPermissions")
     def setPermissions(
         self,
         entity,
         principalId=None,
         accessType=["READ", "DOWNLOAD"],
         modify_benefactor=False,
         warn_if_inherits=True,
@@ -2723,15 +2977,14 @@
         return self._storeACL(entity, acl)
 
     ############################################################
     #                        Provenance                        #
     ############################################################
 
     # TODO: rename these to Activity
-    @tracer.start_as_current_span("Synapse::getProvenance")
     def getProvenance(
         self,
         entity: typing.Union[str, collections.abc.Mapping, numbers.Number],
         version: int = None,
     ) -> Activity:
         """
         Retrieve provenance information for a Synapse Entity.
@@ -2754,15 +3007,14 @@
             uri = "/entity/%s/version/%d/generatedBy" % (entity_id, version)
         else:
             uri = "/entity/%s/generatedBy" % entity_id
 
         trace.get_current_span().set_attributes({"synapse.id": entity_id})
         return Activity(data=self.restGET(uri))
 
-    @tracer.start_as_current_span("Synapse::setProvenance")
     def setProvenance(
         self,
         entity: typing.Union[str, collections.abc.Mapping, numbers.Number],
         activity: Activity,
     ) -> Activity:
         """
         Stores a record of the code and data used to derive a Synapse entity.
@@ -2781,15 +3033,14 @@
         # assert that an entity is generated by an activity
         uri = "/entity/%s/generatedBy?generatedBy=%s" % (entity_id, activity["id"])
         activity = Activity(data=self.restPUT(uri))
 
         trace.get_current_span().set_attributes({"synapse.id": entity_id})
         return activity
 
-    @tracer.start_as_current_span("Synapse::deleteProvenance")
     def deleteProvenance(
         self,
         entity: typing.Union[str, collections.abc.Mapping, numbers.Number],
     ) -> None:
         """
         Removes provenance information from an Entity and deletes the associated Activity.
 
@@ -2824,15 +3075,14 @@
             # We're updating provenance
             uri = "/activity/%s" % activity["id"]
             activity = Activity(data=self.restPUT(uri, json.dumps(activity)))
         else:
             activity = self.restPOST("/activity", body=json.dumps(activity))
         return activity
 
-    @tracer.start_as_current_span("Synapse::updateActivity")
     def updateActivity(self, activity) -> Activity:
         """
         Modifies an existing Activity.
 
         Arguments:
             activity: The Activity to be updated.
 
@@ -2928,15 +3178,14 @@
         # some exceptions caught during download indicate non-recoverable situations that
         # will not be remedied by a repeated download attempt.
         return not (
             (isinstance(ex, OSError) and ex.errno == errno.ENOSPC)
             or isinstance(ex, SynapseMd5MismatchError)  # out of disk space
         )
 
-    @tracer.start_as_current_span("Synapse::_downloadFileHandle")
     def _downloadFileHandle(
         self,
         fileHandleId: str,
         objectId: str,
         objectType: str,
         destination: str,
         retries: int = 5,
@@ -3050,15 +3299,14 @@
                     retries -= 1
                 if retries <= 0:
                     # Re-raise exception
                     raise
 
         raise Exception("should not reach this line")
 
-    @tracer.start_as_current_span("Synapse::_download_from_url_multi_threaded")
     def _download_from_url_multi_threaded(
         self,
         file_handle_id: str,
         object_id: str,
         object_type: str,
         destination: str,
         *,
@@ -3126,15 +3374,14 @@
         Returns:
             A boolean value indicating whether the given uri is hosted at the configured Synapse repo endpoint
         """
         uri_domain = urllib_urlparse.urlparse(uri).netloc
         synapse_repo_domain = urllib_urlparse.urlparse(self.repoEndpoint).netloc
         return uri_domain.lower() == synapse_repo_domain.lower()
 
-    @tracer.start_as_current_span("Synapse::_download_from_URL")
     def _download_from_URL(
         self,
         url: str,
         destination: str,
         fileHandleId: Optional[str] = None,
         expected_md5: Optional[str] = None,
     ) -> str:
@@ -3339,15 +3586,14 @@
                 " {expected_md5}".format(
                     filename=destination, md5=actual_md5, expected_md5=expected_md5
                 )
             )
 
         return destination
 
-    @tracer.start_as_current_span("Synapse::_createExternalFileHandle")
     def _createExternalFileHandle(
         self,
         externalURL: str,
         mimetype: str = None,
         md5: str = None,
         fileSize: int = None,
     ) -> Dict[str, Union[str, int]]:
@@ -3376,15 +3622,14 @@
             (mimetype, enc) = mimetypes.guess_type(externalURL, strict=False)
         if mimetype is not None:
             fileHandle["contentType"] = mimetype
         return self.restPOST(
             "/externalFileHandle", json.dumps(fileHandle), self.fileHandleEndpoint
         )
 
-    @tracer.start_as_current_span("Synapse::_createExternalObjectStoreFileHandle")
     def _createExternalObjectStoreFileHandle(
         self,
         s3_file_key,
         file_path: str,
         storage_location_id: int,
         mimetype: str = None,
         md5: str = None,
@@ -3414,15 +3659,14 @@
             "contentType": mimetype,
         }
 
         return self.restPOST(
             "/externalFileHandle", json.dumps(file_handle), self.fileHandleEndpoint
         )
 
-    @tracer.start_as_current_span("Synapse::create_external_s3_file_handle")
     def create_external_s3_file_handle(
         self,
         bucket_name,
         s3_file_key,
         file_path,
         *,
         parent=None,
@@ -3475,15 +3719,14 @@
 
         return self.restPOST(
             "/externalFileHandle/s3",
             json.dumps(file_handle),
             endpoint=self.fileHandleEndpoint,
         )
 
-    @tracer.start_as_current_span("Synapse::_get_file_handle_as_creator")
     def _get_file_handle_as_creator(
         self, fileHandle: Dict[str, Union[str, int]]
     ) -> Dict[str, Union[str, int]]:
         """
         Retrieve a fileHandle from the fileHandle service.
         Note: You must be the creator of the filehandle to use this method. Otherwise, an 403-Forbidden error will be raised.
 
@@ -3492,15 +3735,14 @@
 
         Returns:
             A fileHandle retrieved from the fileHandle service.
         """
         uri = "/fileHandle/%s" % (id_of(fileHandle),)
         return self.restGET(uri, endpoint=self.fileHandleEndpoint)
 
-    @tracer.start_as_current_span("Synapse::_deleteFileHandle")
     def _deleteFileHandle(self, fileHandle: Dict[str, Union[str, int]]) -> None:
         """
         Delete the given file handle.
 
         Note: Only the user that created the FileHandle can delete it. Also, a FileHandle cannot be deleted if it is
         associated with a FileEntity or WikiPage.
 
@@ -3511,22 +3753,20 @@
         self.restDELETE(uri, endpoint=self.fileHandleEndpoint)
         return fileHandle
 
     ############################################################
     #                    SFTP                                  #
     ############################################################
 
-    @tracer.start_as_current_span("Synapse::_getDefaultUploadDestination")
     def _getDefaultUploadDestination(self, parent_entity):
         return self.restGET(
             "/entity/%s/uploadDestination" % id_of(parent_entity),
             endpoint=self.fileHandleEndpoint,
         )
 
-    @tracer.start_as_current_span("Synapse::_getUserCredentials")
     def _getUserCredentials(
         self, url: str, username: str = None, password: str = None
     ) -> Tuple[str, str]:
         """
         Get user credentials for a specified URL by either looking in the configFile or querying the user.
 
         Arguments:
@@ -3557,15 +3797,14 @@
             password = getpass.getpass("Password for %s:" % baseURL)
         return username, password
 
     ############################################
     # Project/Folder storage location settings #
     ############################################
 
-    @tracer.start_as_current_span("Synapse::createStorageLocationSetting")
     def createStorageLocationSetting(self, storage_type, **kwargs):
         """
         Creates an IMMUTABLE storage location based on the specified type.
 
         For each storage_type, the following kwargs should be specified:
 
         **ExternalObjectStorage**: (S3-like (e.g. AWS S3 or Openstack) bucket not accessed by Synapse)
@@ -3614,29 +3853,27 @@
             + "LocationSetting"
             + ("s" if storage_type == "ProxyStorage" else "")
         )
         kwargs["uploadType"] = upload_type_dict[storage_type]
 
         return self.restPOST("/storageLocation", body=json.dumps(kwargs))
 
-    @tracer.start_as_current_span("Synapse::getMyStorageLocationSetting")
     def getMyStorageLocationSetting(self, storage_location_id):
         """
         Get a StorageLocationSetting by its id.
 
         Arguments:
             storage_location_id: id of the StorageLocationSetting to retrieve.
                                     The corresponding StorageLocationSetting must have been created by this user.
 
         Returns:
             A dict describing the StorageLocationSetting retrieved by its id
         """
         return self.restGET("/storageLocation/%s" % storage_location_id)
 
-    @tracer.start_as_current_span("Synapse::setStorageLocation")
     def setStorageLocation(self, entity, storage_location_id):
         """
         Sets the storage location for a Project or Folder
 
         Arguments:
             entity: A Project or Folder to which the StorageLocationSetting is set
             storage_location_id: A StorageLocation id or a list of StorageLocation ids. Pass in None for the default
@@ -3666,15 +3903,14 @@
                 "projectId": id_of(entity),
             }
 
             return self.restPOST(
                 "/projectSettings", body=json.dumps(project_destination)
             )
 
-    @tracer.start_as_current_span("Synapse::getProjectSetting")
     def getProjectSetting(self, project, setting_type):
         """
         Gets the ProjectSetting for a project.
 
         Arguments:
             project: Project entity or its id as a string
             setting_type: Type of setting. Choose from:
@@ -3694,15 +3930,14 @@
                 projectId=id_of(project), type=setting_type
             )
         )
         return (
             response if response else None
         )  # if no project setting, a empty string is returned as the response
 
-    @tracer.start_as_current_span("Synapse::get_sts_storage_token")
     def get_sts_storage_token(
         self, entity, permission, *, output_format="json", min_remaining_life=None
     ):
         """Get STS credentials for the given entity_id and permission, outputting it in the given format
 
         Arguments:
             entity: The entity or entity id whose credentials are being returned
@@ -3727,15 +3962,14 @@
             self,
             id_of(entity),
             permission,
             output_format=output_format,
             min_remaining_life=min_remaining_life,
         )
 
-    @tracer.start_as_current_span("Synapse::create_s3_storage_location")
     def create_s3_storage_location(
         self,
         *,
         parent=None,
         folder_name=None,
         folder=None,
         bucket_name=None,
@@ -3802,15 +4036,14 @@
 
         return folder, storage_location_setting, project_setting
 
     ############################################################
     #                   CRUD for Evaluations                   #
     ############################################################
 
-    @tracer.start_as_current_span("Synapse::getEvaluation")
     def getEvaluation(self, id):
         """
         Gets an Evaluation object from Synapse.
 
         Arguments:
             id: The ID of the [synapseclient.evaluation.Evaluation][] to return.
 
@@ -3824,29 +4057,27 @@
         """
 
         evaluation_id = id_of(id)
         uri = Evaluation.getURI(evaluation_id)
         return Evaluation(**self.restGET(uri))
 
     # TODO: Should this be combined with getEvaluation?
-    @tracer.start_as_current_span("Synapse::getEvaluationByName")
     def getEvaluationByName(self, name):
         """
         Gets an Evaluation object from Synapse.
 
         Arguments:
             Name: The name of the [synapseclient.evaluation.Evaluation][] to return.
 
         Returns:
             An [synapseclient.evaluation.Evaluation][] object
         """
         uri = Evaluation.getByNameURI(name)
         return Evaluation(**self.restGET(uri))
 
-    @tracer.start_as_current_span("Synapse::getEvaluationByContentSource")
     def getEvaluationByContentSource(self, entity):
         """
         Returns a generator over evaluations that derive their content from the given entity
 
         Arguments:
             entity: The [synapseclient.entity.Project][] whose Evaluations are to be fetched.
 
@@ -3856,29 +4087,27 @@
 
         entityId = id_of(entity)
         url = "/entity/%s/evaluation" % entityId
 
         for result in self._GET_paginated(url):
             yield Evaluation(**result)
 
-    @tracer.start_as_current_span("Synapse::_findTeam")
     def _findTeam(self, name: str) -> typing.Iterator[Team]:
         """
         Retrieve a Teams matching the supplied name fragment
 
         Arguments:
             name: A team name
 
         Yields:
             A generator that yields objects of type [Team][synapseclient.team.Team]
         """
         for result in self._GET_paginated("/teams?fragment=%s" % name):
             yield Team(**result)
 
-    @tracer.start_as_current_span("Synapse::_find_teams_for_principal")
     def _find_teams_for_principal(self, principal_id: str) -> typing.Iterator[Team]:
         """
         Retrieve a list of teams for the matching principal ID. If the principalId that is passed in is a team itself,
         or not found, this will return a generator that yields no results.
 
         Arguments:
             principal_id: Identifier of a user or group.
@@ -3906,87 +4135,80 @@
             icon: The FileHandleID of the icon to be used for the team.
             canPublicJoin: Whether the team can be joined by anyone. Defaults to False.
             canRequestMembership: Whether the team can request membership. Defaults to True.
 
         Returns:
             An object of type [synapseclient.team.Team][]
         """
-        with tracer.start_as_current_span("Synapse::create_team"):
-            request_body = {
-                "name": name,
-                "description": description,
-                "icon": icon,
-                "canPublicJoin": can_public_join,
-                "canRequestMembership": can_request_membership,
-            }
-            return Team(
-                **self.restPOST(
-                    "/team",
-                    json.dumps(request_body),
-                )
+        request_body = {
+            "name": name,
+            "description": description,
+            "icon": icon,
+            "canPublicJoin": can_public_join,
+            "canRequestMembership": can_request_membership,
+        }
+        return Team(
+            **self.restPOST(
+                "/team",
+                json.dumps(request_body),
             )
+        )
 
     def delete_team(self, id: int) -> None:
         """
         Deletes a team.
 
         Arguments:
             id: The ID of the team to delete.
 
         """
-        with tracer.start_as_current_span("Synapse::delete_team"):
-            return self.restDELETE(f"/team/{id}")
+        return self.restDELETE(f"/team/{id}")
 
     def getTeam(self, id: Union[int, str]) -> Team:
         """
         Finds a team with a given ID or name.
 
         Arguments:
             id: The ID or name of the team or a Team object to retrieve.
 
         Returns:
             An object of type [synapseclient.team.Team][]
         """
         # Retrieves team id
-        with tracer.start_as_current_span("Synapse::getTeam"):
-            teamid = id_of(id)
-            try:
-                int(teamid)
-            except (TypeError, ValueError):
-                if isinstance(id, str):
-                    for team in self._findTeam(id):
-                        if team.name == id:
-                            teamid = team.id
-                            break
-                    else:
-                        raise ValueError('Can\'t find team "{}"'.format(teamid))
+        teamid = id_of(id)
+        try:
+            int(teamid)
+        except (TypeError, ValueError):
+            if isinstance(id, str):
+                for team in self._findTeam(id):
+                    if team.name == id:
+                        teamid = team.id
+                        break
                 else:
                     raise ValueError('Can\'t find team "{}"'.format(teamid))
-            return Team(**self.restGET("/team/%s" % teamid))
+            else:
+                raise ValueError('Can\'t find team "{}"'.format(teamid))
+        return Team(**self.restGET("/team/%s" % teamid))
 
     def getTeamMembers(
         self, team: Union[Team, int, str]
     ) -> typing.Generator[TeamMember, None, None]:
         """
         Lists the members of the given team.
 
         Arguments:
             team: A [synapseclient.team.Team][] object or a team's ID.
 
         Yields:
             A generator over [synapseclient.team.TeamMember][] objects.
 
         """
-        with tracer.start_as_current_span("Synapse::getTeamMembers"):
-            for result in self._GET_paginated(
-                "/teamMembers/{id}".format(id=id_of(team))
-            ):
-                yield TeamMember(**result)
+        for result in self._GET_paginated("/teamMembers/{id}".format(id=id_of(team))):
+            yield TeamMember(**result)
 
-    @tracer.start_as_current_span("Synapse::_get_docker_digest")
     def _get_docker_digest(
         self, entity: Union[Entity, str], docker_tag: str = "latest"
     ) -> str:
         """
         Get matching Docker sha-digest of a DockerRepository given a Docker tag
 
         Arguments:
@@ -4020,21 +4242,19 @@
 
         Arguments:
             team: A [synapseclient.team.Team][] object or a team's ID.
 
         Yields:
             Generator of MembershipRequest dictionaries
         """
-        with tracer.start_as_current_span("Synapse::get_team_open_invitations"):
-            teamid = id_of(team)
-            request = "/team/{team}/openInvitation".format(team=teamid)
-            open_requests = self._GET_paginated(request)
-            return open_requests
+        teamid = id_of(team)
+        request = "/team/{team}/openInvitation".format(team=teamid)
+        open_requests = self._GET_paginated(request)
+        return open_requests
 
-    @tracer.start_as_current_span("Synapse::get_membership_status")
     def get_membership_status(self, userid, team):
         """Retrieve a user's Team Membership Status bundle.
         <https://rest-docs.synapse.org/rest/GET/team/id/member/principalId/membershipStatus.html>
 
         Arguments:
             user: Synapse user ID
             team: A [synapseclient.team.Team][] object or a team's ID.
@@ -4045,26 +4265,24 @@
         teamid = id_of(team)
         request = "/team/{team}/member/{user}/membershipStatus".format(
             team=teamid, user=userid
         )
         membership_status = self.restGET(request)
         return membership_status
 
-    @tracer.start_as_current_span("Synapse::_delete_membership_invitation")
     def _delete_membership_invitation(self, invitationid: str) -> None:
         """
         Delete an invitation Note: The client must be an administrator of the
         Team referenced by the invitation or the invitee to make this request.
 
         Arguments:
             invitationid: Open invitation id
         """
         self.restDELETE("/membershipInvitation/{id}".format(id=invitationid))
 
-    @tracer.start_as_current_span("Synapse::send_membership_invitation")
     def send_membership_invitation(
         self, teamId, inviteeId=None, inviteeEmail=None, message=None
     ):
         """Create a membership invitation and send an email notification
         to the invitee.
 
         Arguments:
@@ -4107,67 +4325,65 @@
             inviteeEmail: Email of user
             message: Additional message for the user getting invited to the team.
             force: If an open invitation exists for the invitee, the old invite will be cancelled.
 
         Returns:
             MembershipInvitation or None if user is already a member
         """
-        with tracer.start_as_current_span("Synapse::invite_to_team"):
-            # Throw error if both user and email is specified and if both not
-            # specified
-            id_email_specified = inviteeEmail is not None and user is not None
-            id_email_notspecified = inviteeEmail is None and user is None
-            if id_email_specified or id_email_notspecified:
-                raise ValueError("Must specify either 'user' or 'inviteeEmail'")
-
-            teamid = id_of(team)
-            is_member = False
-            open_invitations = self.get_team_open_invitations(teamid)
-
-            if user is not None:
-                inviteeId = self.getUserProfile(user)["ownerId"]
-                membership_status = self.get_membership_status(inviteeId, teamid)
-                is_member = membership_status["isMember"]
-                open_invites_to_user = [
-                    invitation
-                    for invitation in open_invitations
-                    if invitation.get("inviteeId") == inviteeId
-                ]
-            else:
-                inviteeId = None
-                open_invites_to_user = [
-                    invitation
-                    for invitation in open_invitations
-                    if invitation.get("inviteeEmail") == inviteeEmail
-                ]
-            # Only invite if the invitee is not a member and
-            # if invitee doesn't have an open invitation unless force=True
-            if not is_member and (not open_invites_to_user or force):
-                # Delete all old invitations
-                for invite in open_invites_to_user:
-                    self._delete_membership_invitation(invite["id"])
-                return self.send_membership_invitation(
-                    teamid,
-                    inviteeId=inviteeId,
-                    inviteeEmail=inviteeEmail,
-                    message=message,
-                )
-            if is_member:
-                not_sent_reason = "invitee is already a member"
-            else:
-                not_sent_reason = (
-                    "invitee already has an open invitation "
-                    "Set force=True to send new invite."
-                )
+        # Throw error if both user and email is specified and if both not
+        # specified
+        id_email_specified = inviteeEmail is not None and user is not None
+        id_email_notspecified = inviteeEmail is None and user is None
+        if id_email_specified or id_email_notspecified:
+            raise ValueError("Must specify either 'user' or 'inviteeEmail'")
 
-            self.logger.warning("No invitation sent: {}".format(not_sent_reason))
-            # Return None if no invite is sent.
-            return None
+        teamid = id_of(team)
+        is_member = False
+        open_invitations = self.get_team_open_invitations(teamid)
+
+        if user is not None:
+            inviteeId = self.getUserProfile(user)["ownerId"]
+            membership_status = self.get_membership_status(inviteeId, teamid)
+            is_member = membership_status["isMember"]
+            open_invites_to_user = [
+                invitation
+                for invitation in open_invitations
+                if invitation.get("inviteeId") == inviteeId
+            ]
+        else:
+            inviteeId = None
+            open_invites_to_user = [
+                invitation
+                for invitation in open_invitations
+                if invitation.get("inviteeEmail") == inviteeEmail
+            ]
+        # Only invite if the invitee is not a member and
+        # if invitee doesn't have an open invitation unless force=True
+        if not is_member and (not open_invites_to_user or force):
+            # Delete all old invitations
+            for invite in open_invites_to_user:
+                self._delete_membership_invitation(invite["id"])
+            return self.send_membership_invitation(
+                teamid,
+                inviteeId=inviteeId,
+                inviteeEmail=inviteeEmail,
+                message=message,
+            )
+        if is_member:
+            not_sent_reason = "invitee is already a member"
+        else:
+            not_sent_reason = (
+                "invitee already has an open invitation "
+                "Set force=True to send new invite."
+            )
+
+        self.logger.warning("No invitation sent: {}".format(not_sent_reason))
+        # Return None if no invite is sent.
+        return None
 
-    @tracer.start_as_current_span("Synapse::submit")
     def submit(
         self,
         evaluation,
         entity,
         name=None,
         team=None,
         silent=False,
@@ -4268,26 +4484,24 @@
             if not (isinstance(evaluation, Evaluation)):
                 evaluation = self.getEvaluation(evaluation_id)
             if "submissionReceiptMessage" in evaluation:
                 self.logger.info(evaluation["submissionReceiptMessage"])
 
         return Submission(**submitted)
 
-    @tracer.start_as_current_span("Synapse::_submit")
     def _submit(self, submission, entity_etag, eligibility_hash):
         require_param(submission, "submission")
         require_param(entity_etag, "entity_etag")
         # URI requires the etag of the entity and, in the case of a team submission, requires an eligibilityStateHash
         uri = "/evaluation/submission?etag=%s" % entity_etag
         if eligibility_hash:
             uri += "&submissionEligibilityHash={0}".format(eligibility_hash)
         submitted = self.restPOST(uri, json.dumps(submission))
         return submitted
 
-    @tracer.start_as_current_span("Synapse::_get_contributors")
     def _get_contributors(self, evaluation_id, team):
         if not evaluation_id or not team:
             return None, None
 
         team_id = id_of(team)
         # see <https://rest-docs.synapse.org/rest/GET/evaluation/evalId/team/id/submissionEligibility.html>
         eligibility = self.restGET(
@@ -4314,15 +4528,14 @@
         contributors = [
             {"principalId": member["principalId"]}
             for member in eligibility["membersEligibility"]
             if member["isEligible"] and not member["hasConflictingSubmission"]
         ]
         return contributors, eligibility["eligibilityStateHash"]
 
-    @tracer.start_as_current_span("Synapse::_allowParticipation")
     def _allowParticipation(
         self,
         evaluation: Union[Evaluation, str],
         user: str,
         rights: list = ["READ", "PARTICIPATE", "SUBMIT", "UPDATE_SUBMISSION"],
     ) -> Dict[str, Union[str, list]]:
         """
@@ -4369,15 +4582,14 @@
             userId = self._getUserbyPrincipalIdOrName(user)
 
         if not isinstance(evaluation, Evaluation):
             evaluation = self.getEvaluation(id_of(evaluation))
 
         self.setPermissions(evaluation, userId, accessType=rights, overwrite=False)
 
-    @tracer.start_as_current_span("Synapse::getSubmissions")
     def getSubmissions(self, evaluation, status=None, myOwn=False, limit=20, offset=0):
         """
         Arguments:
             evaluation: Evaluation to get submissions from.
             status: Optionally filter submissions for a specific status.
                     One of:
 
@@ -4419,15 +4631,14 @@
 
         if status is not None:
             uri += "?status=%s" % status
 
         for result in self._GET_paginated(uri, limit=limit, offset=offset):
             yield Submission(**result)
 
-    @tracer.start_as_current_span("Synapse::_getSubmissionBundles")
     def _getSubmissionBundles(
         self,
         evaluation: Union[Evaluation, str],
         status: str = None,
         myOwn: bool = False,
         limit: int = 20,
         offset: int = 0,
@@ -4469,15 +4680,14 @@
             "" if myOwn else "/all",
         )
         if status is not None:
             url += "?status=%s" % status
 
         return self._GET_paginated(url, limit=limit, offset=offset)
 
-    @tracer.start_as_current_span("Synapse::getSubmissionBundles")
     def getSubmissionBundles(
         self, evaluation, status=None, myOwn=False, limit=20, offset=0
     ):
         """
         Retrieve submission bundles (submission and submissions status) for an evaluation queue, optionally filtered by
         submission status and/or owner.
 
@@ -4519,15 +4729,14 @@
             evaluation, status=status, myOwn=myOwn, limit=limit, offset=offset
         ):
             yield (
                 Submission(**bundle["submission"]),
                 SubmissionStatus(**bundle["submissionStatus"]),
             )
 
-    @tracer.start_as_current_span("Synapse::_GET_paginated")
     def _GET_paginated(self, uri: str, limit: int = 20, offset: int = 0):
         """
         Get paginated results
 
         Arguments:
             uri:     A URI that returns paginated results
             limit:   How many records should be returned per request
@@ -4546,15 +4755,14 @@
             results = page["results"] if "results" in page else page["children"]
             prev_num_results = len(results)
 
             for result in results:
                 offset += 1
                 yield result
 
-    @tracer.start_as_current_span("Synapse::_POST_paginated")
     def _POST_paginated(self, uri: str, body, **kwargs):
         """
         Get paginated results
 
         Arguments:
             uri:     A URI that returns paginated results
             body:    POST request payload
@@ -4569,15 +4777,14 @@
             response = self.restPOST(uri, body=json.dumps(body), **kwargs)
             next_page_token = response.get("nextPageToken")
             for item in response["page"]:
                 yield item
             if next_page_token is None:
                 break
 
-    @tracer.start_as_current_span("Synapse::getSubmission")
     def getSubmission(self, id, **kwargs):
         """
         Gets a [synapseclient.evaluation.Submission][] object by its id.
 
         Arguments:
             id: The id of the submission to retrieve
 
@@ -4615,15 +4822,14 @@
                 **kwargs,
             )
             submission.entity = related
             submission.filePath = related.get("path", None)
 
         return submission
 
-    @tracer.start_as_current_span("Synapse::getSubmissionStatus")
     def getSubmissionStatus(self, submission):
         """
         Downloads the status of a Submission.
 
         Arguments:
             submission: The submission to lookup
 
@@ -4636,15 +4842,14 @@
         val = self.restGET(uri)
         return SubmissionStatus(**val)
 
     ############################################################
     #                      CRUD for Wikis                      #
     ############################################################
 
-    @tracer.start_as_current_span("Synapse::getWiki")
     def getWiki(self, owner, subpageId=None, version=None):
         """
         Get a [synapseclient.wiki.Wiki][] object from Synapse. Uses wiki2 API which supports versioning.
 
         Arguments:
             owner: The entity to which the Wiki is attached
             subpageId: The id of the specific sub-page or None to get the root Wiki page
@@ -4684,30 +4889,28 @@
                 markdown = f.read().decode("utf-8")
 
         wiki.markdown = markdown
         wiki.markdown_path = path
 
         return wiki
 
-    @tracer.start_as_current_span("Synapse::getWikiHeaders")
     def getWikiHeaders(self, owner):
         """
         Retrieves the headers of all Wikis belonging to the owner (the entity to which the Wiki is attached).
 
         Arguments:
             owner: An Entity
 
         Returns:
             A list of Objects with three fields: id, title and parentId.
         """
 
         uri = "/entity/%s/wikiheadertree" % id_of(owner)
         return [DictObject(**header) for header in self._GET_paginated(uri)]
 
-    @tracer.start_as_current_span("Synapse::_storeWiki")
     def _storeWiki(self, wiki: Wiki, createOrUpdate: bool) -> Wiki:
         """
         Stores or updates the given Wiki.
 
         Arguments:
             wiki:           A Wiki object
             createOrUpdate: Indicates whether the method should automatically perform an update if the 'obj'
@@ -4719,15 +4922,17 @@
         # Make sure the file handle field is a list
         if "attachmentFileHandleIds" not in wiki:
             wiki["attachmentFileHandleIds"] = []
 
         # Convert all attachments into file handles
         if wiki.get("attachments") is not None:
             for attachment in wiki["attachments"]:
-                fileHandle = upload_synapse_s3(self, attachment)
+                fileHandle = wrap_async_to_sync(
+                    upload_synapse_s3(self, attachment), self
+                )
                 wiki["attachmentFileHandleIds"].append(fileHandle["id"])
             del wiki["attachments"]
 
         # Perform an update if the Wiki has an ID
         if "id" in wiki:
             updated_wiki = Wiki(
                 owner=wiki.ownerId, **self.restPUT(wiki.putURI(), wiki.json())
@@ -4759,15 +4964,14 @@
                         owner=wiki.ownerId,
                         **self.restPUT(existing_wiki.putURI(), existing_wiki.json()),
                     )
                 else:
                     raise
         return updated_wiki
 
-    @tracer.start_as_current_span("Synapse::getWikiAttachments")
     def getWikiAttachments(self, wiki):
         """
         Retrieve the attachments to a wiki page.
 
         Arguments:
             wiki: The Wiki object for which the attachments are to be returned.
 
@@ -4779,15 +4983,14 @@
         file_handles = list(WikiAttachment(**fh) for fh in results["list"])
         return file_handles
 
     ############################################################
     #                      Tables                              #
     ############################################################
 
-    @tracer.start_as_current_span("Synapse::_waitForAsync")
     def _waitForAsync(self, uri, request, endpoint=None):
         if endpoint is None:
             endpoint = self.repoEndpoint
         async_job_id = self.restPOST(
             uri + "/start", body=json.dumps(request), endpoint=endpoint
         )
 
@@ -4830,15 +5033,14 @@
                 + result.get("errorDetails", None),
                 asynchronousJobStatus=result,
             )
         if progressed:
             self._print_transfer_progress(total, total, message, isBytes=False)
         return result
 
-    @tracer.start_as_current_span("Synapse::getColumn")
     def getColumn(self, id):
         """
         Gets a Column object from Synapse by ID.
 
         See: [synapseclient.table.Column][]
 
         Arguments:
@@ -4851,15 +5053,14 @@
         Example: Using this function
             Getting a column
 
                 column = syn.getColumn(123)
         """
         return Column(**self.restGET(Column.getURI(id)))
 
-    @tracer.start_as_current_span("Synapse::getColumns")
     def getColumns(self, x, limit=100, offset=0):
         """
         Get the columns defined in Synapse either (1) corresponding to a set of column headers, (2) those for a given
         schema, or (3) those whose names start with a given prefix.
 
         Arguments:
             x: A list of column headers, a Table Entity object (Schema/EntityViewSchema), a Table's Synapse ID, or a
@@ -4889,15 +5090,14 @@
         elif isinstance(x, str):
             uri = "/column?prefix=" + x
             for result in self._GET_paginated(uri, limit=limit, offset=offset):
                 yield Column(**result)
         else:
             ValueError("Can't get columns for a %s" % type(x))
 
-    @tracer.start_as_current_span("Synapse::create_snapshot_version")
     def create_snapshot_version(
         self,
         table: typing.Union[
             EntityViewSchema, Schema, str, SubmissionViewSchema, Dataset
         ],
         comment: str = None,
         label: str = None,
@@ -4940,15 +5140,14 @@
                 "This function only accepts Synapse ids of Tables or Views"
             )
 
         # for consistency we return nothing if wait=False since we can't
         # supply the snapshot version on an async table update without waiting
         return result["snapshotVersionNumber"] if wait else None
 
-    @tracer.start_as_current_span("Synapse::_create_table_snapshot")
     def _create_table_snapshot(
         self,
         table: typing.Union[Schema, str],
         comment: str = None,
         label: str = None,
         activity: typing.Union[Activity, str] = None,
     ) -> dict:
@@ -4983,15 +5182,14 @@
             key: value for key, value in snapshot_body.items() if value is not None
         }
         snapshot = self.restPOST(
             "/entity/{}/table/snapshot".format(id_of(table)), body=json.dumps(new_body)
         )
         return snapshot
 
-    @tracer.start_as_current_span("Synapse::_async_table_update")
     def _async_table_update(
         self,
         table: typing.Union[EntityViewSchema, Schema, str, SubmissionViewSchema],
         changes: typing.List[dict] = [],
         create_snapshot: bool = False,
         comment: str = None,
         label: str = None,
@@ -5035,15 +5233,14 @@
         else:
             result = self.restPOST(
                 "{}/start".format(uri), body=json.dumps(table_update_body)
             )
 
         return result
 
-    @tracer.start_as_current_span("Synapse::getTableColumns")
     def getTableColumns(self, table):
         """
         Retrieve the column models used in the given table schema.
 
         Arguments:
             table: The schema of the Table whose columns are to be retrieved
 
@@ -5052,15 +5249,14 @@
         """
         uri = "/entity/{id}/column".format(id=id_of(table))
         # The returned object type for this service, PaginatedColumnModels, is a misnomer.
         # This service always returns the full list of results so the pagination does not not actually matter.
         for result in self.restGET(uri)["results"]:
             yield Column(**result)
 
-    @tracer.start_as_current_span("Synapse::tableQuery")
     def tableQuery(self, query: str, resultsAs: str = "csv", **kwargs):
         """
         Query a Synapse Table.
 
         You can receive query results either as a generator over rows or as a CSV file. For smallish tables, either
         method will work equally well. Use of a "rowset" generator allows rows to be processed one at a time and
         processing may be stopped before downloading the entire table.
@@ -5101,15 +5297,14 @@
                 kwargs.pop("isConsistent")
             return CsvFileTable.from_table_query(self, query, **kwargs)
         else:
             raise ValueError(
                 "Unknown return type requested from tableQuery: " + str(resultsAs)
             )
 
-    @tracer.start_as_current_span("Synapse::_queryTable")
     def _queryTable(
         self,
         query: str,
         limit: int = None,
         offset: int = None,
         isConsistent: bool = True,
         partMask=None,
@@ -5153,30 +5348,28 @@
 
         uri = "/entity/{id}/table/query/async".format(
             id=extract_synapse_id_from_query(query)
         )
 
         return self._waitForAsync(uri=uri, request=query_bundle_request)
 
-    @tracer.start_as_current_span("Synapse::_queryTableNext")
     def _queryTableNext(self, nextPageToken: str, tableId: str) -> TableQueryResult:
         """
         Retrieve following pages if the result contains a *nextPageToken*
 
         Arguments:
             nextPageToken: Forward this token to get the next page of results.
             tableId:       The Synapse ID of the table
 
         Returns:
             The following page of results as a QueryResultBundle
         """
         uri = "/entity/{id}/table/query/nextPage/async".format(id=tableId)
         return self._waitForAsync(uri=uri, request=nextPageToken)
 
-    @tracer.start_as_current_span("Synapse::_uploadCsv")
     def _uploadCsv(
         self,
         filepath: str,
         schema: Union[Entity, str],
         updateEtag: str = None,
         quoteCharacter: str = '"',
         escapeCharacter: str = "\\",
@@ -5201,15 +5394,17 @@
             linesToSkip:     The number of lines to skip from the start of the file.
                              The default value of 0 will be used if this is not provided by the caller.
 
         Returns:
             [UploadToTableResult](https://rest-docs.synapse.org/rest/org/sagebionetworks/repo/model/table/UploadToTableResult.html)
         """
 
-        fileHandleId = multipart_upload_file(self, filepath, content_type="text/csv")
+        fileHandleId = wrap_async_to_sync(
+            multipart_upload_file_async(self, filepath, content_type="text/csv"), self
+        )
 
         uploadRequest = {
             "concreteType": "org.sagebionetworks.repo.model.table.UploadToTableRequest",
             "csvTableDescriptor": {
                 "isFirstLineHeader": header,
                 "quoteCharacter": quoteCharacter,
                 "escapeCharacter": escapeCharacter,
@@ -5225,15 +5420,14 @@
             uploadRequest["updateEtag"] = updateEtag
 
         response = self._async_table_update(schema, changes=[uploadRequest], wait=True)
         self._check_table_transaction_response(response)
 
         return response
 
-    @tracer.start_as_current_span("Synapse::_check_table_transaction_response")
     def _check_table_transaction_response(self, response):
         for result in response["results"]:
             result_type = result["concreteType"]
 
             if result_type in {
                 concrete_types.ROW_REFERENCE_SET_RESULTS,
                 concrete_types.TABLE_SCHEMA_CHANGE_RESPONSE,
@@ -5264,15 +5458,14 @@
             else:
                 warnings.warn(
                     "Unexpected result from a table transaction of type [%s]."
                     " Please check the result to make sure it is correct. %s"
                     % (result_type, result)
                 )
 
-    @tracer.start_as_current_span("Synapse::_queryTableCsv")
     def _queryTableCsv(
         self,
         query: str,
         quoteCharacter: str = '"',
         escapeCharacter: str = "\\",
         lineEnd: str = os.linesep,
         separator: str = ",",
@@ -5349,15 +5542,14 @@
             "TableEntity",
             os.path.join(download_dir, filename),
         )
 
         return download_from_table_result, path
 
     # This is redundant with syn.store(Column(...)) and will be removed unless people prefer this method.
-    @tracer.start_as_current_span("Synapse::createColumn")
     def createColumn(
         self,
         name,
         columnType,
         maximumSize=None,
         defaultValue=None,
         enumValues=None,
@@ -5367,15 +5559,14 @@
             columnType=columnType,
             maximumSize=maximumSize,
             defaultValue=defaultValue,
             enumValue=enumValues,
         )
         return Column(**self.restPOST("/column", json.dumps(columnModel)))
 
-    @tracer.start_as_current_span("Synapse::createColumns")
     def createColumns(self, columns: typing.List[Column]) -> typing.List[Column]:
         """
         Creates a batch of [synapseclient.table.Column][]'s within a single request.
 
         Arguments:
             columns: A list of [synapseclient.table.Column][]'s
 
@@ -5385,15 +5576,14 @@
         request_body = {
             "concreteType": "org.sagebionetworks.repo.model.ListWrapper",
             "list": list(columns),
         }
         response = self.restPOST("/column/batch", json.dumps(request_body))
         return [Column(**col) for col in response["list"]]
 
-    @tracer.start_as_current_span("Synapse::_getColumnByName")
     def _getColumnByName(self, schema: Schema, column_name: str) -> Column:
         """
         Given a schema and a column name, get the corresponding [Column][synapseclient.table.Column] object.
 
         Arguments:
             schema: The Schema is an [Entity][synapseclient.entity.Entity] that defines a set of columns in a table.
             column_name: The column name
@@ -5402,15 +5592,14 @@
             A Column object
         """
         for column in self.getColumns(schema):
             if column.name == column_name:
                 return column
         return None
 
-    @tracer.start_as_current_span("Synapse::downloadTableColumns")
     def downloadTableColumns(self, table, columns, downloadLocation=None, **kwargs):
         """
         Bulk download of table-associated files.
 
         Arguments:
             table: Table query result
             columns: A list of column names as strings
@@ -5543,15 +5732,14 @@
                 and fha["fileHandleId"] not in permanent_failures.keys()
             ]
 
         # TODO if there are files we still haven't downloaded
 
         return file_handle_to_path_map
 
-    @tracer.start_as_current_span("Synapse::_build_table_download_file_handle_list")
     def _build_table_download_file_handle_list(self, table, columns, downloadLocation):
         # ------------------------------------------------------------
         # build list of file handles to download
         # ------------------------------------------------------------
         cols_not_found = [
             c for c in columns if c not in [h.name for h in table.headers]
         ]
@@ -5585,23 +5773,21 @@
                             )
                         )
                     seen_file_handle_ids.add(file_handle_id)
                 else:
                     warnings.warn("Weird file handle: %s" % file_handle_id)
         return file_handle_associations, file_handle_to_path_map
 
-    @tracer.start_as_current_span("Synapse::_get_default_view_columns")
     def _get_default_view_columns(self, view_type, view_type_mask=None):
         """Get default view columns"""
         uri = f"/column/tableview/defaults?viewEntityType={view_type}"
         if view_type_mask:
             uri += f"&viewTypeMask={view_type_mask}"
         return [Column(**col) for col in self.restGET(uri)["list"]]
 
-    @tracer.start_as_current_span("Synapse::_get_annotation_view_columns")
     def _get_annotation_view_columns(
         self, scope_ids: list, view_type: str, view_type_mask: str = None
     ) -> list:
         """
         Get all the columns of a submission of entity view based on existing annotations
 
         Arguments:
@@ -5634,15 +5820,14 @@
                 break
         return columns
 
     ############################################################
     #              CRUD for Entities (properties)              #
     ############################################################
 
-    @tracer.start_as_current_span("Synapse::_getEntity")
     def _getEntity(
         self, entity: Union[str, dict, Entity], version: int = None
     ) -> Dict[str, Union[str, bool]]:
         """
         Get an entity from Synapse.
 
         Arguments:
@@ -5654,29 +5839,27 @@
         """
 
         uri = "/entity/" + id_of(entity)
         if version:
             uri += "/version/%d" % version
         return self.restGET(uri)
 
-    @tracer.start_as_current_span("Synapse::_createEntity")
     def _createEntity(self, entity: Union[dict, Entity]) -> Dict[str, Union[str, bool]]:
         """
         Create a new entity in Synapse.
 
         Arguments:
             entity: A dictionary representing an Entity or a Synapse Entity object
 
         Returns:
             A dictionary containing an Entity's properties
         """
 
         return self.restPOST(uri="/entity", body=json.dumps(get_properties(entity)))
 
-    @tracer.start_as_current_span("Synapse::_updateEntity")
     def _updateEntity(
         self,
         entity: Union[dict, Entity],
         incrementVersion: bool = True,
         versionLabel: str = None,
     ) -> Dict[str, Union[str, bool]]:
         """
@@ -5703,15 +5886,14 @@
 
             if incrementVersion:
                 entity["versionLabel"] = versionLabel
                 params["newVersion"] = "true"
 
         return self.restPUT(uri, body=json.dumps(get_properties(entity)), params=params)
 
-    @tracer.start_as_current_span("Synapse::findEntityId")
     def findEntityId(self, name, parent=None):
         """
         Find an Entity given its name and parent.
 
         Arguments:
             name: Name of the entity to find
             parent: An Entity object or the Id of an entity as a string. Omit if searching for a Project by name
@@ -5734,15 +5916,14 @@
             ):  # a 404 error is raised if the entity does not exist
                 return None
             raise
 
     ############################################################
     #                       Send Message                       #
     ############################################################
-    @tracer.start_as_current_span("Synapse::sendMessage")
     def sendMessage(
         self, userIds, messageSubject, messageBody, contentType="text/plain"
     ):
         """
         send a message via Synapse.
 
         Arguments:
@@ -5752,16 +5933,17 @@
             contentType: optional contentType of message body (default="text/plain")
                             Should be one of "text/plain" or "text/html"
 
         Returns:
             The metadata of the created message
         """
 
-        fileHandleId = multipart_upload_string(
-            self, messageBody, content_type=contentType
+        fileHandleId = wrap_async_to_sync(
+            multipart_upload_string_async(self, messageBody, content_type=contentType),
+            self,
         )
         message = dict(
             recipients=userIds, subject=messageSubject, fileHandleId=fileHandleId
         )
         return self.restPOST(uri="/message", body=json.dumps(message))
 
     ############################################################
@@ -5792,14 +5974,85 @@
             if response.status_code in (401, 403) and not self.credentials:
                 raise SynapseAuthenticationError(
                     "You are not logged in and do not have access to a requested resource."
                 ) from ex
 
             raise
 
+    def _handle_httpx_synapse_http_error(self, response: httpx.Response) -> None:
+        """Raise errors as appropriate for the HTTPX library returned Synapse http
+        status codes
+
+        Arguments:
+            response: The HTTPX response object
+        """
+
+        try:
+            exceptions._raise_for_status_httpx(
+                response=response, verbose=self.debug, logger=self.logger
+            )
+        except exceptions.SynapseHTTPError as ex:
+            # if we get a unauthenticated or forbidden error and the user is not logged in
+            # then we raise it as an authentication error.
+            # we can't know for certain that logging in to their particular account will grant them
+            # access to this resource but more than likely it's the cause of this error.
+            if response.status_code in (401, 403) and not self.credentials:
+                raise SynapseAuthenticationError(
+                    "You are not logged in and do not have access to a requested resource."
+                ) from ex
+
+            raise
+
+    def _attach_rest_data_to_otel(
+        self,
+        method: str,
+        uri: str,
+        data: typing.Union[str, bytes],
+        current_span: trace.Span,
+    ) -> None:
+        """Handle attaching a few piece of data from the REST call into the OTEL span.
+        This is used for easier tracking of data that is being sent out of this service.
+
+        Arguments:
+            method: The HTTP method used in the REST call.
+            uri: The URI of the REST call.
+            data: The data being sent in the REST call.
+        """
+        current_span.set_attributes({"url": uri, "http.method": method.upper()})
+        if current_span.is_recording() and data:
+            try:
+                if isinstance(data, str):
+                    data_to_parse = data
+                elif isinstance(data, bytes):
+                    data_to_parse = data.decode("utf-8")
+                else:
+                    return
+                data_dict = json.loads(data_to_parse)
+
+                if "parentId" in data_dict:
+                    current_span.set_attribute(
+                        "synapse.parent_id", data_dict["parentId"]
+                    )
+                if "id" in data_dict:
+                    current_span.set_attribute("synapse.id", data_dict["id"])
+                if "concreteType" in data_dict:
+                    current_span.set_attribute(
+                        "synapse.concrete_type", data_dict["concreteType"]
+                    )
+                if "entityName" in data_dict:
+                    current_span.set_attribute(
+                        "synapse.entity_name", data_dict["entityName"]
+                    )
+                elif "name" in data_dict:
+                    current_span.set_attribute("synapse.name", data_dict["name"])
+            except Exception as ex:
+                self.logger.debug(
+                    "Failed to parse data for OTEL span in _rest_call", ex
+                )
+
     def _rest_call(
         self,
         method,
         uri,
         data,
         endpoint,
         headers,
@@ -5830,30 +6083,36 @@
         )
 
         retryPolicy = self._build_retry_policy(retryPolicy)
         requests_session = requests_session or self._requests_session
 
         auth = kwargs.pop("auth", self.credentials)
         requests_method_fn = getattr(requests_session, method)
+        current_span = trace.get_current_span()
+        if current_span.is_recording():
+            current_span = tracer.start_span(
+                f"{method.upper()} {uri}", kind=SpanKind.CLIENT
+            )
+            self._attach_rest_data_to_otel(method, uri, data, current_span)
         response = with_retry(
             lambda: requests_method_fn(
                 uri,
                 data=data,
                 headers=headers,
                 auth=auth,
                 **kwargs,
             ),
             verbose=self.debug,
             **retryPolicy,
         )
-
+        if current_span.is_recording():
+            current_span.end()
         self._handle_synapse_http_error(response)
         return response
 
-    @tracer.start_as_current_span("Synapse::restGET")
     def restGET(
         self,
         uri,
         endpoint=None,
         headers=None,
         retryPolicy={},
         requests_session=None,
@@ -5868,21 +6127,19 @@
             headers: Dictionary of headers to use rather than the API-key-signed default set of headers
             requests_session: An external [requests.Session object](https://requests.readthedocs.io/en/latest/user/advanced/) to use when making this specific call
             kwargs: Any other arguments taken by a [request](http://docs.python-requests.org/en/latest/) method
 
         Returns:
             JSON encoding of response
         """
-        trace.get_current_span().set_attributes({"url.path": uri})
         response = self._rest_call(
             "get", uri, None, endpoint, headers, retryPolicy, requests_session, **kwargs
         )
         return self._return_rest_body(response)
 
-    @tracer.start_as_current_span("Synapse::restPOST")
     def restPOST(
         self,
         uri,
         body,
         endpoint=None,
         headers=None,
         retryPolicy={},
@@ -5899,28 +6156,26 @@
             headers: Dictionary of headers to use rather than the API-key-signed default set of headers
             requests_session: An external [requests.Session object](https://requests.readthedocs.io/en/latest/user/advanced/) to use when making this specific call
             kwargs: Any other arguments taken by a [request](http://docs.python-requests.org/en/latest/) method
 
         Returns:
             JSON encoding of response
         """
-        trace.get_current_span().set_attributes({"url.path": uri})
         response = self._rest_call(
             "post",
             uri,
             body,
             endpoint,
             headers,
             retryPolicy,
             requests_session,
             **kwargs,
         )
         return self._return_rest_body(response)
 
-    @tracer.start_as_current_span("Synapse::restPUT")
     def restPUT(
         self,
         uri,
         body=None,
         endpoint=None,
         headers=None,
         retryPolicy={},
@@ -5937,28 +6192,26 @@
             headers: Dictionary of headers to use rather than the API-key-signed default set of headers
             requests_session: An external [requests.Session object](https://requests.readthedocs.io/en/latest/user/advanced/) to use when making this specific call
             kwargs: Any other arguments taken by a [request](http://docs.python-requests.org/en/latest/) method
 
         Returns
             JSON encoding of response
         """
-        trace.get_current_span().set_attributes({"url.path": uri})
         response = self._rest_call(
             "put",
             uri,
             body,
             endpoint,
             headers,
             retryPolicy,
             requests_session,
             **kwargs,
         )
         return self._return_rest_body(response)
 
-    @tracer.start_as_current_span("Synapse::restDELETE")
     def restDELETE(
         self,
         uri,
         endpoint=None,
         headers=None,
         retryPolicy={},
         requests_session=None,
@@ -5971,27 +6224,28 @@
             uri: URI of resource to be deleted
             endpoint: Server endpoint, defaults to self.repoEndpoint
             headers: Dictionary of headers to use rather than the API-key-signed default set of headers
             requests_session: An external [requests.Session object](https://requests.readthedocs.io/en/latest/user/advanced/) to use when making this specific call
             kwargs: Any other arguments taken by a [request](http://docs.python-requests.org/en/latest/) method
 
         """
-        trace.get_current_span().set_attributes({"url.path": uri})
         self._rest_call(
             "delete",
             uri,
             None,
             endpoint,
             headers,
             retryPolicy,
             requests_session,
             **kwargs,
         )
 
-    def _build_uri_and_headers(self, uri, endpoint=None, headers=None):
+    def _build_uri_and_headers(
+        self, uri: str, endpoint: str = None, headers: Dict[str, str] = None
+    ) -> Tuple[str, Dict[str, str]]:
         """Returns a tuple of the URI and headers to request with."""
 
         if endpoint is None:
             endpoint = self.repoEndpoint
 
         trace.get_current_span().set_attributes({"server.address": endpoint})
 
@@ -6008,15 +6262,252 @@
     def _build_retry_policy(self, retryPolicy={}):
         """Returns a retry policy to be passed onto _with_retry."""
 
         defaults = dict(STANDARD_RETRY_PARAMS)
         defaults.update(retryPolicy)
         return defaults
 
-    def _return_rest_body(self, response):
+    def _build_retry_policy_async(
+        self, retry_policy: Dict[str, Any] = {}
+    ) -> Dict[str, Any]:
+        """Returns a retry policy to be passed onto with_retry_time_based_async."""
+
+        defaults = dict(STANDARD_RETRY_ASYNC_PARAMS)
+        defaults.update(retry_policy)
+        return defaults
+
+    def _return_rest_body(self, response) -> Union[Dict[str, Any], str]:
         """Returns either a dictionary or a string depending on the 'content-type' of the response."""
         trace.get_current_span().set_attributes(
             {"http.response.status_code": response.status_code}
         )
         if is_json(response.headers.get("content-type", None)):
             return response.json()
         return response.text
+
+    async def _rest_call_async(
+        self,
+        method: str,
+        uri: str,
+        data: Any,
+        endpoint: str,
+        headers: Dict[str, str],
+        retry_policy: Dict[str, Any],
+        requests_session_async_synapse: httpx.AsyncClient,
+        **kwargs,
+    ) -> Union[httpx.Response, None]:
+        """
+        Sends an HTTP request to the Synapse server.
+
+        Arguments:
+            method: The method to implement Create, Read, Update, Delete operations.
+                Should be post, get, put, delete.
+            uri: URI on which the method is performed.
+            data: The payload to be delivered.
+            endpoint: Server endpoint, defaults to self.repoEndpoint
+            headers: Dictionary of headers to use.
+            retry_policy: A retry policy that matches the arguments of
+                [synapseclient.core.retry.with_retry_time_based_async][].
+            requests_session_async_synapse: The async client to use when making this
+                specific call.
+            kwargs: Any other arguments taken by a
+                [request](https://www.python-httpx.org/api/) method
+
+        Returns:
+            JSON encoding of response
+        """
+        uri, headers = self._build_uri_and_headers(
+            uri, endpoint=endpoint, headers=headers
+        )
+
+        retry_policy = self._build_retry_policy_async(retry_policy)
+        requests_session = (
+            requests_session_async_synapse
+            or self._get_requests_session_async_synapse(
+                asyncio_event_loop=asyncio.get_running_loop()
+            )
+        )
+
+        auth = kwargs.pop("auth", self.credentials)
+        requests_method_fn = getattr(requests_session, method)
+        if data:
+            response = await with_retry_time_based_async(
+                lambda: requests_method_fn(
+                    uri,
+                    content=data,
+                    headers=headers,
+                    auth=auth,
+                    **kwargs,
+                ),
+                verbose=self.debug,
+                **retry_policy,
+            )
+        else:
+            response = await with_retry_time_based_async(
+                lambda: requests_method_fn(
+                    uri,
+                    headers=headers,
+                    auth=auth,
+                    **kwargs,
+                ),
+                verbose=self.debug,
+                **retry_policy,
+            )
+
+        self._handle_httpx_synapse_http_error(response)
+
+        return response
+
+    async def rest_get_async(
+        self,
+        uri: str,
+        endpoint: str = None,
+        headers: httpx.Headers = None,
+        retry_policy: Dict[str, Any] = {},
+        requests_session_async_synapse: httpx.AsyncClient = None,
+        **kwargs,
+    ) -> Union[Dict[str, Any], str, None]:
+        """
+        Sends an HTTP GET request to the Synapse server.
+
+        Arguments:
+            uri: URI on which get is performed
+            endpoint: Server endpoint, defaults to self.repoEndpoint
+            headers: Dictionary of headers to use.
+            retry_policy: A retry policy that matches the arguments of
+                [synapseclient.core.retry.with_retry_time_based_async][].
+            requests_session_async_synapse: The async client to use when making this
+                specific call.
+            kwargs: Any other arguments taken by a
+                [request](https://www.python-httpx.org/api/) method
+
+        Returns:
+            JSON encoding of response
+        """
+        try:
+            response = await self._rest_call_async(
+                "get",
+                uri,
+                None,
+                endpoint,
+                headers,
+                retry_policy,
+                requests_session_async_synapse,
+                **kwargs,
+            )
+            return self._return_rest_body(response)
+        except Exception:
+            self.logger.exception("Error in rest_get_async")
+
+    async def rest_post_async(
+        self,
+        uri: str,
+        body: Any = None,
+        endpoint: str = None,
+        headers: httpx.Headers = None,
+        retry_policy: Dict[str, Any] = {},
+        requests_session_async_synapse: httpx.AsyncClient = None,
+        **kwargs,
+    ) -> Union[Dict[str, Any], str]:
+        """
+        Sends an HTTP POST request to the Synapse server.
+
+        Arguments:
+            uri: URI on which get is performed
+            body: The payload to be delivered
+            endpoint: Server endpoint, defaults to self.repoEndpoint
+            headers: Dictionary of headers to use.
+            retry_policy: A retry policy that matches the arguments of
+                [synapseclient.core.retry.with_retry_time_based_async][].
+            requests_session_async_synapse: The async client to use when making this
+                specific call.
+            kwargs: Any other arguments taken by a
+                [request](https://www.python-httpx.org/api/) method
+
+        Returns:
+            JSON encoding of response
+        """
+        response = await self._rest_call_async(
+            "post",
+            uri,
+            body,
+            endpoint,
+            headers,
+            retry_policy,
+            requests_session_async_synapse,
+            **kwargs,
+        )
+        return self._return_rest_body(response)
+
+    async def rest_put_async(
+        self,
+        uri: str,
+        body: Any = None,
+        endpoint: str = None,
+        headers: httpx.Headers = None,
+        retry_policy: Dict[str, Any] = {},
+        requests_session_async_synapse: httpx.AsyncClient = None,
+        **kwargs,
+    ) -> Union[Dict[str, Any], str]:
+        """
+        Sends an HTTP PUT request to the Synapse server.
+
+        Arguments:
+            uri: URI on which get is performed
+            body: The payload to be delivered.
+            endpoint: Server endpoint, defaults to self.repoEndpoint
+            headers: Dictionary of headers to use.
+            retry_policy: A retry policy that matches the arguments of
+                [synapseclient.core.retry.with_retry_time_based_async][].
+            requests_session_async_synapse: The async client to use when making this
+                specific call.
+            kwargs: Any other arguments taken by a
+                [request](https://www.python-httpx.org/api/) method
+
+        Returns
+            JSON encoding of response
+        """
+        response = await self._rest_call_async(
+            "put",
+            uri,
+            body,
+            endpoint,
+            headers,
+            retry_policy,
+            requests_session_async_synapse,
+            **kwargs,
+        )
+        return self._return_rest_body(response)
+
+    async def rest_delete_async(
+        self,
+        uri: str,
+        endpoint: str = None,
+        headers: httpx.Headers = None,
+        retry_policy: Dict[str, Any] = {},
+        requests_session_async_synapse: httpx.AsyncClient = None,
+        **kwargs,
+    ) -> None:
+        """
+        Sends an HTTP DELETE request to the Synapse server.
+
+        Arguments:
+            uri: URI of resource to be deleted
+            endpoint: Server endpoint, defaults to self.repoEndpoint
+            headers: Dictionary of headers to use.
+            retry_policy: A retry policy that matches the arguments of
+                [synapseclient.core.retry.with_retry_time_based_async][].
+            requests_session_async_synapse: The async client to use when making this
+                specific call
+            kwargs: Any other arguments taken by a [request](https://www.python-httpx.org/api/) method
+
+        """
+        await self._rest_call_async(
+            "delete",
+            uri,
+            None,
+            endpoint,
+            headers,
+            retry_policy,
+            requests_session_async_synapse,
+            **kwargs,
+        )
```

### Comparing `synapseclient-4.1.1/synapseclient/core/async_utils.py` & `synapseclient-4.2.0/synapseclient/core/async_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """This utility class is to hold any utilities that are needed for async operations."""
 
 import asyncio
 import functools
-from typing import Callable, Union
+from typing import Any, Callable, Coroutine, Union, TYPE_CHECKING
 
 import nest_asyncio
 from opentelemetry import trace
 
+if TYPE_CHECKING:
+    from synapseclient import Synapse
+
 tracer = trace.get_tracer("synapseclient")
 
 
 def otel_trace_method(method_to_trace_name: Union[Callable[..., str], None] = None):
     """
     Decorator to trace a method with OpenTelemetry in an async environment. This function
     is specifically written to be used on a method within a class.
@@ -39,17 +42,21 @@
         async def otel_trace_method_wrapper(self, *arg, **kwargs) -> None:
             """Wrapper for the function to be traced."""
             trace_name = (
                 method_to_trace_name(self, *arg, **kwargs)
                 if method_to_trace_name
                 else None
             )
-            with tracer.start_as_current_span(
-                trace_name or f"Synaspse::{func.__name__}"
-            ):
+            current_span = trace.get_current_span()
+            if current_span.is_recording():
+                with tracer.start_as_current_span(
+                    trace_name or f"Synaspse::{func.__name__}"
+                ):
+                    return await func(self, *arg, **kwargs)
+            else:
                 return await func(self, *arg, **kwargs)
 
         return otel_trace_method_wrapper
 
     return decorator
 
 
@@ -66,14 +73,36 @@
             else:
                 return self.fn(cls, *args, **kwds)
 
         functools.update_wrapper(f, self.fn)
         return f
 
 
+def wrap_async_to_sync(coroutine: Coroutine[Any, Any, Any], syn: "Synapse") -> Any:
+    """Wrap an async function to be called in a sync context."""
+    loop = None
+    try:
+        try:
+            loop = asyncio.get_running_loop()
+        except RuntimeError:
+            pass
+
+        if loop:
+            nest_asyncio.apply(loop=loop)
+            return loop.run_until_complete(coroutine)
+        else:
+            return asyncio.run(coroutine)
+
+    except Exception as ex:
+        syn.logger.exception(
+            f"Error occurred while running {coroutine} in a sync context."
+        )
+        raise ex
+
+
 # Adapted from
 # https://github.com/keflavich/astroquery/blob/30deafc3aa057916bcdca70733cba748f1b36b64/astroquery/utils/process_asyncs.py#L11
 def async_to_sync(cls):
     """
     Convert all name_of_thing_async methods to name_of_thing methods
 
     (see
@@ -88,21 +117,37 @@
         def newmethod(self, *args, **kwargs):
             """The new method that will replace the non-async method."""
 
             async def wrapper(*args, **kwargs):
                 """Wrapper for the function to be called in an async context."""
                 return await getattr(self, async_method_name)(*args, **kwargs)
 
+            loop = None
             try:
-                loop = asyncio.get_running_loop()
-            except RuntimeError:
-                return asyncio.run(wrapper(*args, **kwargs))
-            else:
-                nest_asyncio.apply(loop=loop)
-                return loop.run_until_complete(wrapper(*args, **kwargs))
+                try:
+                    loop = asyncio.get_running_loop()
+                except RuntimeError:
+                    pass
+
+                if loop:
+                    nest_asyncio.apply(loop=loop)
+                    return loop.run_until_complete(wrapper(*args, **kwargs))
+                else:
+                    return asyncio.run(wrapper(*args, **kwargs))
+
+            except Exception as ex:
+                from synapseclient import Synapse
+
+                synapse_client = Synapse.get_client(
+                    getattr(kwargs, "synapse_client", None)
+                )
+                synapse_client.logger.exception(
+                    f"Error occurred while running {async_method_name} on {self.__class__}."
+                )
+                raise ex
 
         return newmethod
 
     methods = cls.__dict__.keys()
 
     methods_to_update = []
     for k in methods:
```

### Comparing `synapseclient-4.1.1/synapseclient/core/cache.py` & `synapseclient-4.2.0/synapseclient/core/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,24 +149,28 @@
         """
         Retrieve the `modified_time` from the `cache_map_entry`. This needed to be
         backwards-compatible any cache entries that do not have the new JSON structure
         for data. That means that if the cache_map_entry has a `modified_time` key,
         then it is a new entry and we can return the value. If it does not, then it
         is an old entry and we should return the `cache_map_entry` itself.
 
+        The caveat is that `cache_map_entry` needs to be a string to return the value
+        otherwise it will return None.
+
         Arguments:
             cache_map_entry: The entry from the cache map
 
         Returns:
             The modified time if it exists, otherwise the cache_map_entry
         """
         if cache_map_entry is not None and "modified_time" in cache_map_entry:
             return cache_map_entry.get("modified_time", None)
-        else:
+        elif cache_map_entry is not None and isinstance(cache_map_entry, str):
             return cache_map_entry
+        return None
 
     def _get_cache_content_md5(
         self, cache_map_entry: typing.Union[str, dict, None]
     ) -> typing.Union[str, None]:
         """
         Retrieve the `content_md5` from the cache_map_entry.
```

### Comparing `synapseclient-4.1.1/synapseclient/core/constants/concrete_types.py` & `synapseclient-4.2.0/synapseclient/core/constants/concrete_types.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/credentials/cred_data.py` & `synapseclient-4.2.0/synapseclient/core/credentials/cred_data.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/credentials/credential_provider.py` & `synapseclient-4.2.0/synapseclient/core/credentials/credential_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
 This module contains classes that are responsible for retrieving synapse authentication
 information (e.g. authToken) from a source (e.g. login args, config file).
 """
+
 import abc
 import os
 from typing import Union, Dict, Tuple, TYPE_CHECKING
 
 from synapseclient.core.credentials.cred_data import (
     SynapseAuthTokenCredentials,
     SynapseCredentials,
 )
 from synapseclient.core.exceptions import SynapseAuthenticationError
-from opentelemetry import trace
 
 if TYPE_CHECKING:
     from synapseclient import Synapse
 
-tracer = trace.get_tracer("synapseclient")
-
 
 class SynapseCredentialsProvider(metaclass=abc.ABCMeta):
     """
     A credential provider is responsible for retrieving synapse authentication
     information (e.g. authToken) from a source (e.g. login args, config file),
     and use them to return a
     [SynapseCredentials][synapseclient.core.credentials.cred_data.SynapseCredentials]
@@ -221,15 +219,14 @@
             ([SynapseCredentialsProvider][synapseclient.core.credentials.credential_provider.SynapseCredentialsProvider])
             credential providers
     """
 
     def __init__(self, cred_providers) -> None:
         self.cred_providers = list(cred_providers)
 
-    @tracer.start_as_current_span("SynapseCredentialsProviderChain::get_credentials")
     def get_credentials(
         self, syn: "Synapse", user_login_args: Dict[str, str]
     ) -> Union[SynapseCredentials, None]:
         """
         Iterates its list of
         [SynapseCredentialsProvider][synapseclient.core.credentials.credential_provider.SynapseCredentialsProvider]
         and returns the first non-None
```

### Comparing `synapseclient-4.1.1/synapseclient/core/cumulative_transfer_progress.py` & `synapseclient-4.2.0/synapseclient/core/cumulative_transfer_progress.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/dozer.py` & `synapseclient-4.2.0/synapseclient/core/dozer.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/lock.py` & `synapseclient-4.2.0/synapseclient/core/lock.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/logging_setup.py` & `synapseclient-4.2.0/synapseclient/core/logging_setup.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/models/custom_json.py` & `synapseclient-4.2.0/synapseclient/core/models/custom_json.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/models/dict_object.py` & `synapseclient-4.2.0/synapseclient/core/models/dict_object.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/models/permission.py` & `synapseclient-4.2.0/synapseclient/core/models/permission.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/multithread_download/download_threads.py` & `synapseclient-4.2.0/synapseclient/core/multithread_download/download_threads.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/pool_provider.py` & `synapseclient-4.2.0/synapseclient/core/pool_provider.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/remote_file_storage_wrappers.py` & `synapseclient-4.2.0/synapseclient/core/remote_file_storage_wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from contextlib import contextmanager
+"""Wrappers for remote file storage clients like S3 and SFTP."""
+
 import os
-import time
 import typing
-import multiprocessing
 import urllib.parse as urllib_parse
+from contextlib import contextmanager
+
+from tqdm import tqdm
 
-from synapseclient.core.retry import with_retry
 from synapseclient.core.cumulative_transfer_progress import printTransferProgress
+from synapseclient.core.retry import with_retry
 from synapseclient.core.utils import attempt_import
 
 
 class S3ClientWrapper:
     """
     Wrapper class for S3 client.
     """
@@ -31,47 +33,36 @@
             "\n\nLibraries required for client authenticated S3 access are not installed!\n"
             "The Synapse client uses boto3 in order to access S3-like storage "
             "locations.\n",
         )
 
     @staticmethod
     def _create_progress_callback_func(
-        file_size: int, filename: str, prefix: str = None
+        progress_bar: tqdm,
     ) -> callable:
         """
         Creates a progress callback function for tracking the progress of a file transfer.
 
         Arguments:
             file_size: The total size of the file being transferred.
             filename: The name of the file being transferred.
             prefix: A prefix to display before the progress bar. Defaults to None.
 
         Returns:
             progress_callback: The progress callback function.
         """
-        bytes_transferred = multiprocessing.Value("d", 0)
-        t0 = time.time()
 
-        def progress_callback(bytes: int) -> None:
+        def progress_callback(transferred_bytes: int) -> None:
             """
             Update the progress of a transfer.
 
             Arguments:
                 bytes: The number of bytes transferred.
             """
-            with bytes_transferred.get_lock():
-                bytes_transferred.value += bytes
-                printTransferProgress(
-                    bytes_transferred.value,
-                    file_size,
-                    prefix=prefix,
-                    postfix=filename,
-                    dt=time.time() - t0,
-                    previouslyTransferred=0,
-                )
+            progress_bar.update(transferred_bytes)
 
         return progress_callback
 
     @staticmethod
     def download_file(
         bucket: str,
         endpoint_url: str,
@@ -108,67 +99,76 @@
         Raises:
             ValueError: If the key does not exist in the bucket.
             botocore.exceptions.ClientError: If there is an error with the S3 client.
         """
 
         S3ClientWrapper._attempt_import_boto3()
 
-        import botocore
         import boto3.s3.transfer
+        import botocore
 
         transfer_config = boto3.s3.transfer.TransferConfig(
             **(transfer_config_kwargs or {})
         )
 
         session_args = credentials if credentials else {"profile_name": profile_name}
         boto_session = boto3.session.Session(**session_args)
         s3 = boto_session.resource("s3", endpoint_url=endpoint_url)
 
         try:
             s3_obj = s3.Object(bucket, remote_file_key)
 
             progress_callback = None
+            progress_bar = None
             if show_progress:
                 s3_obj.load()
                 file_size = s3_obj.content_length
                 filename = os.path.basename(download_file_path)
+                progress_bar = tqdm(
+                    total=file_size,
+                    desc="Downloading",
+                    unit="B",
+                    unit_scale=True,
+                    postfix=filename,
+                    smoothing=0,
+                )
                 progress_callback = S3ClientWrapper._create_progress_callback_func(
-                    file_size,
-                    filename,
-                    prefix="Downloading",
+                    progress_bar
                 )
 
             s3_obj.download_file(
                 download_file_path,
                 Callback=progress_callback,
                 Config=transfer_config,
             )
+            if progress_bar:
+                progress_bar.close()
 
-            # why return what we were passed...?
             return download_file_path
 
         except botocore.exceptions.ClientError as e:
             if e.response["Error"]["Code"] == "404":
                 raise ValueError(
                     "The key:%s does not exist in bucket:%s.", remote_file_key, bucket
                 )
             else:
                 raise
 
     @staticmethod
     def upload_file(
         bucket: str,
-        endpoint_url: str,
+        endpoint_url: typing.Optional[str],
         remote_file_key: str,
         upload_file_path: str,
         *,
         profile_name: str = None,
         credentials: typing.Dict[str, str] = None,
         show_progress: bool = True,
         transfer_config_kwargs: dict = None,
+        storage_str: str = None,
     ) -> str:
         """
         Upload a file to s3 using boto3.
 
         Arguments:
             bucket: name of bucket to upload to
             endpoint_url: a boto3 compatible endpoint url
@@ -206,29 +206,40 @@
         )
 
         session_args = credentials if credentials else {"profile_name": profile_name}
         boto_session = boto3.session.Session(**session_args)
         s3 = boto_session.resource("s3", endpoint_url=endpoint_url)
 
         progress_callback = None
+        progress_bar = None
         if show_progress:
             file_size = os.stat(upload_file_path).st_size
             filename = os.path.basename(upload_file_path)
+            progress_bar = tqdm(
+                total=file_size,
+                desc=storage_str,
+                unit="B",
+                unit_scale=True,
+                postfix=filename,
+                smoothing=0,
+            )
             progress_callback = S3ClientWrapper._create_progress_callback_func(
-                file_size, filename, prefix="Uploading"
+                progress_bar
             )
 
         # automatically determines whether to perform multi-part upload
         s3.Bucket(bucket).upload_file(
             upload_file_path,
             remote_file_key,
             Callback=progress_callback,
             Config=transfer_config,
             ExtraArgs={"ACL": "bucket-owner-full-control"},
         )
+        if progress_bar:
+            progress_bar.close()
         return upload_file_path
 
 
 class SFTPWrapper:
     @staticmethod
     def _attempt_import_sftp():
         """
@@ -257,37 +268,54 @@
                     "This method only supports sftp URLs of the form sftp://..."
                 )
             )
         return parsedURL
 
     @staticmethod
     def upload_file(
-        filepath: str, url: str, username: str = None, password: str = None
+        filepath: str,
+        url: str,
+        username: str = None,
+        password: str = None,
+        storage_str: str = None,
     ) -> str:
         """
         Performs upload of a local file to an sftp server.
 
         Arguments:
             filepath: The path to the file to be uploaded.
             url: URL where file will be deposited. Should include path and protocol. e.g.
                         sftp://sftp.example.com/path/to/file/store
             username: The username for authentication. Defaults to None.
             password: The password for authentication. Defaults to None.
 
         Returns:
             The URL of the uploaded file.
         """
+        progress_bar = tqdm(
+            desc=storage_str,
+            unit="B",
+            unit_scale=True,
+            smoothing=0,
+            postfix=filepath,
+        )
+
+        def progress_callback(*args, **kwargs) -> None:
+            if not progress_bar.total:
+                progress_bar.total = args[1]
+            progress_bar.update(args[0] - progress_bar.n)
+
         parsedURL = SFTPWrapper._parse_for_sftp(url)
         with _retry_pysftp_connection(
             parsedURL.hostname, username=username, password=password
         ) as sftp:
             sftp.makedirs(parsedURL.path)
             with sftp.cd(parsedURL.path):
-                sftp.put(filepath, preserve_mtime=True, callback=printTransferProgress)
-
+                sftp.put(filepath, preserve_mtime=True, callback=progress_callback)
+        progress_bar.close()
         path = urllib_parse.quote(parsedURL.path + "/" + os.path.split(filepath)[-1])
         parsedURL = parsedURL._replace(path=path)
         return urllib_parse.urlunparse(parsedURL)
 
     @staticmethod
     def download_file(
         url: str,
```

### Comparing `synapseclient-4.1.1/synapseclient/core/sts_transfer.py` & `synapseclient-4.2.0/synapseclient/core/sts_transfer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import collections
 import collections.abc
 import datetime
 import importlib
 import os
 import threading
 import platform
-
+from typing import TYPE_CHECKING
 from synapseclient.core.utils import iso_to_datetime, snake_case
 
+if TYPE_CHECKING:
+    from synapseclient import Synapse
+
 try:
     boto3 = importlib.import_module("boto3")
 except ImportError:
     # boto is not a requirement to load this module,
     # we are able to optionally use functionality if it's available
     boto3 = None
 
@@ -235,15 +238,15 @@
 
     Arguments:
         syn:       A [Synapse][synapseclient.Synapse] object
         entity_id: The ID of synapse entity whose storage location we want to check for sts access
         location:  A storage location ID or a dictionary representing the location UploadDestination
 
     Returns:
-        True if STS if enabled for the location, False otherwise
+        True if STS is enabled for the location, False otherwise
     """
     if not location:
         return False
 
     if isinstance(location, collections.abc.Mapping):
         # looks like this is already an upload destination dict
         destination = location
@@ -252,7 +255,40 @@
         # otherwise treat it as a storage location id,
         destination = syn.restGET(
             f"/entity/{entity_id}/uploadDestination/{location}",
             endpoint=syn.fileHandleEndpoint,
         )
 
     return destination.get("stsEnabled", False)
+
+
+async def is_storage_location_sts_enabled_async(
+    syn: "Synapse", entity_id: str, location: str
+) -> bool:
+    """
+    Returns whether the given storage location is enabled for STS.
+
+    Arguments:
+        syn:       A [Synapse][synapseclient.Synapse] object
+        entity_id: The ID of synapse entity whose storage location we want to check for sts access
+        location:  A storage location ID or a dictionary representing the location UploadDestination
+
+    Returns:
+        True if STS is enabled for the location, False otherwise
+    """
+    if not location:
+        return False
+
+    if isinstance(location, collections.abc.Mapping):
+        # looks like this is already an upload destination dict
+        destination = location
+
+    else:
+        # Lazy import to avoid circular imports
+        from synapseclient.api.entity_services import get_upload_destination_location
+
+        # otherwise treat it as a storage location id,
+        destination = await get_upload_destination_location(
+            entity_id=entity_id, location=location, synapse_client=syn
+        )
+
+    return destination.get("stsEnabled", False)
```

### Comparing `synapseclient-4.1.1/synapseclient/core/upload/__init__.py` & `synapseclient-4.2.0/synapseclient/core/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/core/upload/multipart_upload.py` & `synapseclient-4.2.0/synapseclient/core/upload/multipart_upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,46 @@
 Synapse's [Multipart File Upload API](https://rest-docs.synapse.org/rest/index.html#org.sagebionetworks.file.controller.UploadController), which provides a
 robust means of uploading large files (into the 10s of GiB). End users should not need to call any of the methods under
 [UploadAttempt][synapseclient.core.upload.multipart_upload.UploadAttempt] directly.
 
 """
 
 import concurrent.futures
-from contextlib import contextmanager
 import json
-import math
 import mimetypes
 import os
-import re
-import typing
-import requests
 import threading
 import time
+import typing
+from contextlib import contextmanager
 from typing import List, Mapping
 
-from synapseclient.core.retry import with_retry
+import requests
+from opentelemetry import context, trace
+from opentelemetry.context import Context
+
 from synapseclient.core import pool_provider
 from synapseclient.core.constants import concrete_types
 from synapseclient.core.exceptions import (
-    _raise_for_status,  # why is is this a single underscore
+    _raise_for_status,
+)  # why is is this a single underscore
+from synapseclient.core.exceptions import (
     SynapseHTTPError,
     SynapseUploadAbortedException,
     SynapseUploadFailedException,
 )
-from synapseclient.core.utils import md5_fn, md5_for_file, MB, Spinner
-from opentelemetry import trace, context
-from opentelemetry.context import Context
+from synapseclient.core.retry import with_retry
+from synapseclient.core.upload.upload_utils import (
+    copy_md5_fn,
+    copy_part_request_body_provider_fn,
+    get_data_chunk,
+    get_file_chunk,
+    get_part_size,
+)
+from synapseclient.core.utils import MB, Spinner, md5_fn, md5_for_file
 
 # AWS limits
 MAX_NUMBER_OF_PARTS = 10000
 MIN_PART_SIZE = 5 * MB
 
 # ancient tribal knowledge
 DEFAULT_PART_SIZE = 8 * MB
@@ -300,15 +308,14 @@
 
             # remove so future batch pre_signed url fetches will exclude this part
             with self._lock:
                 del self._pre_signed_part_urls[part_number]
 
             return part_number, part_size
 
-    @tracer.start_as_current_span("UploadAttempt::_upload_parts")
     def _upload_parts(self, part_count, remaining_part_numbers):
         trace.get_current_span().set_attributes({"thread.id": threading.get_ident()})
         time_upload_started = time.time()
         completed_part_count = part_count - len(remaining_part_numbers)
         file_size = self._upload_request_payload.get("fileSizeBytes")
 
         if not self._is_copy():
@@ -368,15 +375,14 @@
                 # upload attempt running
                 concurrent.futures.wait(futures)
 
                 if isinstance(cause, KeyboardInterrupt):
                     raise SynapseUploadAbortedException("User interrupted upload")
                 raise SynapseUploadFailedException("Part upload failed") from cause
 
-    @tracer.start_as_current_span("UploadAttempt::_complete_upload")
     def _complete_upload(self):
         upload_status_response = self._syn.restPUT(
             "/file/multipart/{upload_id}/complete".format(
                 upload_id=self._upload_id,
             ),
             requests_session=self._get_thread_session(),
             endpoint=self._syn.fileHandleEndpoint,
@@ -408,37 +414,14 @@
             if remaining_part_numbers:
                 self._upload_parts(part_count, remaining_part_numbers)
             upload_status_response = self._complete_upload()
 
         return upload_status_response
 
 
-def _get_file_chunk(file_path, part_number, chunk_size):
-    """Read the nth chunk from the file."""
-    with open(file_path, "rb") as f:
-        f.seek((part_number - 1) * chunk_size)
-        return f.read(chunk_size)
-
-
-def _get_data_chunk(data, part_number, chunk_size):
-    """Return the nth chunk of a buffer."""
-    return data[(part_number - 1) * chunk_size : part_number * chunk_size]
-
-
-def _get_part_size(part_size, file_size):
-    part_size = part_size or DEFAULT_PART_SIZE
-
-    # can't exceed the maximum allowed num parts
-    part_size = max(
-        part_size, MIN_PART_SIZE, int(math.ceil(file_size / MAX_NUMBER_OF_PARTS))
-    )
-    return part_size
-
-
-@tracer.start_as_current_span("multipart_upload::multipart_upload_file")
 def multipart_upload_file(
     syn,
     file_path: str,
     dest_file_name: str = None,
     content_type: str = None,
     part_size: int = None,
     storage_location_id: str = None,
@@ -491,42 +474,46 @@
     if content_type is None:
         mime_type, _ = mimetypes.guess_type(file_path, strict=False)
         content_type = mime_type or "application/octet-stream"
 
     callback_func = Spinner().print_tick if not syn.silent else None
     md5_hex = md5 or md5_for_file(file_path, callback=callback_func).hexdigest()
 
-    part_size = _get_part_size(part_size, file_size)
+    part_size = get_part_size(
+        part_size or DEFAULT_PART_SIZE,
+        file_size,
+        MIN_PART_SIZE,
+        MAX_NUMBER_OF_PARTS,
+    )
 
     upload_request = {
         "concreteType": concrete_types.MULTIPART_UPLOAD_REQUEST,
         "contentType": content_type,
         "contentMD5Hex": md5_hex,
         "fileName": dest_file_name,
         "fileSizeBytes": file_size,
         "generatePreview": preview,
         "partSizeBytes": part_size,
         "storageLocationId": storage_location_id,
     }
 
     def part_fn(part_number):
-        return _get_file_chunk(file_path, part_number, part_size)
+        return get_file_chunk(file_path, part_number, part_size)
 
     return _multipart_upload(
         syn,
         dest_file_name,
         upload_request,
         part_fn,
         md5_fn,
         force_restart=force_restart,
         max_threads=max_threads,
     )
 
 
-@tracer.start_as_current_span("multipart_upload::multipart_upload_string")
 def multipart_upload_string(
     syn,
     text: str,
     dest_file_name: str = None,
     part_size: int = None,
     content_type: str = None,
     storage_location_id: str = None,
@@ -563,43 +550,52 @@
 
     if not dest_file_name:
         dest_file_name = "message.txt"
 
     if not content_type:
         content_type = "text/plain; charset=utf-8"
 
-    part_size = _get_part_size(part_size, file_size)
+    part_size = get_part_size(
+        part_size or DEFAULT_PART_SIZE,
+        file_size,
+        MIN_PART_SIZE,
+        MAX_NUMBER_OF_PARTS,
+    )
 
     upload_request = {
         "concreteType": concrete_types.MULTIPART_UPLOAD_REQUEST,
         "contentType": content_type,
         "contentMD5Hex": md5_hex,
         "fileName": dest_file_name,
         "fileSizeBytes": file_size,
         "generatePreview": preview,
         "partSizeBytes": part_size,
         "storageLocationId": storage_location_id,
     }
 
     def part_fn(part_number):
-        return _get_data_chunk(data, part_number, part_size)
+        return get_data_chunk(data, part_number, part_size)
 
-    part_size = _get_part_size(part_size, file_size)
+    part_size = get_part_size(
+        part_size or DEFAULT_PART_SIZE,
+        file_size,
+        MIN_PART_SIZE,
+        MAX_NUMBER_OF_PARTS,
+    )
     return _multipart_upload(
         syn,
         dest_file_name,
         upload_request,
         part_fn,
         md5_fn,
         force_restart=force_restart,
         max_threads=max_threads,
     )
 
 
-@tracer.start_as_current_span("multipart_upload::multipart_copy")
 def multipart_copy(
     syn,
     source_file_handle_association,
     dest_file_name: str = None,
     part_size: int = None,
     storage_location_id: str = None,
     preview: bool = True,
@@ -635,39 +631,20 @@
         "fileName": dest_file_name,
         "generatePreview": preview,
         "partSizeBytes": part_size,
         "sourceFileHandleAssociation": source_file_handle_association,
         "storageLocationId": storage_location_id,
     }
 
-    def part_request_body_provider_fn(part_num):
-        # for an upload copy there are no bytes
-        return None
-
-    def md5_fn(_, response):
-        # for a multipart copy we use the md5 returned by the UploadPartCopy command
-        # when we add the part to the Synapse upload
-
-        # we extract the md5 from the <ETag> element in the response.
-        # use lookahead and lookbehind to find the opening and closing ETag elements but
-        # do not include those in the match, thus the entire matched string (group 0) will be
-        # what was between those elements.
-        md5_hex = re.search(
-            "(?<=<ETag>).*?(?=<\\/ETag>)", (response.content.decode("utf-8"))
-        ).group(0)
-
-        # remove quotes found in the ETag to get at the normalized ETag
-        return md5_hex.replace("&quot;", "").replace('"', "")
-
     return _multipart_upload(
         syn,
         dest_file_name,
         upload_request,
-        part_request_body_provider_fn,
-        md5_fn,
+        copy_part_request_body_provider_fn,
+        copy_md5_fn,
         force_restart=force_restart,
         max_threads=max_threads,
     )
 
 
 def _multipart_upload(
     syn,
```

### Comparing `synapseclient-4.1.1/synapseclient/core/upload/upload_functions.py` & `synapseclient-4.2.0/synapseclient/core/upload/upload_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,22 @@
 from synapseclient.core.exceptions import SynapseMd5MismatchError
 from synapseclient.core import utils
 from opentelemetry import trace
 
 if TYPE_CHECKING:
     from synapseclient import Synapse
 
-tracer = trace.get_tracer("synapseclient")
-
 
 def log_upload_message(syn: "Synapse", message: str) -> None:
     # if this upload is in the context of a larger, multi threaded sync upload as indicated by a cumulative progress
     # then we don't print the individual upload messages to the console since they wouldn't be properly interleaved.
     if not cumulative_transfer_progress.is_active():
         syn.logger.info(message)
 
 
-@tracer.start_as_current_span("upload_functions::upload_file_handle")
 def upload_file_handle(
     syn: "Synapse",
     parent_entity: Union[str, collections.abc.Mapping, numbers.Number],
     path: str,
     synapseStore: bool = True,
     md5: str = None,
     file_size: int = None,
```

### Comparing `synapseclient-4.1.1/synapseclient/core/utils.py` & `synapseclient-4.2.0/synapseclient/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Utility functions useful in the implementation and testing of the Synapse client.
 """
 
+import asyncio
 import base64
 import cgi
 import collections.abc
 import datetime
 import errno
+import gc
 import hashlib
 import importlib
 import inspect
 import numbers
 import os
 import platform
 import random
@@ -19,23 +21,23 @@
 import tempfile
 import threading
 import typing
 import urllib.parse as urllib_parse
 import uuid
 import warnings
 import zipfile
-from dataclasses import asdict
+from dataclasses import asdict, is_dataclass
 from typing import TYPE_CHECKING, Callable, TypeVar
 
 import requests
 from opentelemetry import context, trace
 from opentelemetry.context import Context
 
 if TYPE_CHECKING:
-    from synapseclient.models import Folder, Project
+    from synapseclient.models import File, Folder, Project
 
 R = TypeVar("R")
 
 UNIX_EPOCH = datetime.datetime(1970, 1, 1, 0, 0, tzinfo=datetime.timezone.utc)
 ISO_FORMAT = "%Y-%m-%dT%H:%M:%S.000Z"
 ISO_FORMAT_MICROS = "%Y-%m-%dT%H:%M:%S.%fZ"
 GB = 2**30
@@ -61,27 +63,85 @@
                     Defaults to 2 MB
         callback: The callback function that help us show loading spinner on terminal.
                     Defaults to None
 
     Returns:
         The MD5 Checksum
     """
-
+    loop_iteration = 0
     md5 = hashlib.new("md5", usedforsecurity=False)
     with open(filename, "rb") as f:
         while True:
+            loop_iteration += 1
             if callback:
                 callback()
             data = f.read(block_size)
             if not data:
                 break
             md5.update(data)
+            del data
+            # Garbage collect every 100 iterations
+            if loop_iteration % 100 == 0:
+                gc.collect()
     return md5
 
 
+def md5_for_file_hex(
+    filename: str, block_size: int = 2 * MB, callback: typing.Callable = None
+) -> str:
+    """
+    Calculates the MD5 of the given file.
+    See source <http://stackoverflow.com/questions/1131220/get-md5-hash-of-a-files-without-open-it-in-python>.
+
+    Arguments:
+        filename: The file to read in
+        block_size: How much of the file to read in at once (bytes).
+                    Defaults to 2 MB
+        callback: The callback function that help us show loading spinner on terminal.
+                    Defaults to None
+
+    Returns:
+        The MD5 Checksum
+    """
+
+    return md5_for_file(filename, block_size, callback).hexdigest()
+
+
+async def md5_for_file_multiprocessing(
+    filename: str,
+    process_pool_executor,
+    md5_semaphore: asyncio.Semaphore,
+    block_size: int = 2 * MB,
+) -> str:
+    """
+    Calculates the MD5 of the given file.
+    See source <http://stackoverflow.com/questions/1131220/get-md5-hash-of-a-files-without-open-it-in-python>.
+
+    Arguments:
+        filename: The file to read in
+        process_pool_executor: The process pool executor to use for the calculation.
+        md5_semaphore: The semaphore to use for waiting to calculate.
+        block_size: How much of the file to read in at once (bytes).
+                    Defaults to 2 MB.
+
+    Returns:
+        The MD5 Checksum
+    """
+    async with md5_semaphore:
+        with tracer.start_as_current_span("Utils::md5_for_file_multiprocessing"):
+            future = process_pool_executor.submit(
+                md5_for_file_hex, filename, block_size
+            )
+            while not future.done():
+                await asyncio.sleep(0)
+            result = future.result()
+            return result
+
+
+@tracer.start_as_current_span("Utils::md5_fn")
 def md5_fn(part, _) -> str:
     """Calculate the MD5 of a file-like object.
 
     Arguments:
         part: A file-like object to read from.
 
     Returns:
@@ -929,15 +989,15 @@
     nbytes = humanizeBytes(transferred) if isBytes else transferred
     if toBeTransferred > 0:
         outOf = "/%s" % (humanizeBytes(toBeTransferred) if isBytes else toBeTransferred)
         percentage = "%4.2f%%" % (progress * 100)
     else:
         outOf = ""
         percentage = ""
-    text = "\r%s [%s]%s   %s%s %s %s %s    " % (
+    text = "\r%s [%s]%s   %s%s %s %s %s    \n" % (
         prefix,
         "#" * block + "-" * (barLength - block),
         percentage,
         nbytes,
         outOf,
         rate,
         postfix,
@@ -1335,15 +1395,15 @@
     if incoming_object:
         for key in list(incoming_object.keys()):
             if incoming_object[key] is None:
                 del incoming_object[key]
 
 
 def merge_dataclass_entities(
-    source: typing.Union["Project", "Folder"],
+    source: typing.Union["Project", "Folder", "File"],
     destination: typing.Union["Project", "Folder"],
 ) -> typing.Union["Project", "Folder"]:
     """
     Utility function to merge two dataclass entities together. This is used when we are
     upserting an entity from the Synapse service with the requested changes.
 
     Arguments:
@@ -1356,20 +1416,27 @@
     # Convert dataclasses to dictionaries
     destination_dict = asdict(destination)
     source_dict = asdict(source)
     modified_items = {}
 
     # Update destination_dict with source_dict, keeping destination's values in case of conflicts
     for key, value in source_dict.items():
-        if key not in destination_dict or destination_dict[key] is None:
+        if is_dataclass(getattr(source, key)):
+            if hasattr(destination, key):
+                setattr(destination, key, getattr(source, key))
+            else:
+                modified_items[key] = merge_dataclass_entities(
+                    getattr(source, key), destination=getattr(destination, key)
+                )
+        elif key not in destination_dict or destination_dict[key] is None:
             modified_items[key] = value
         elif key == "annotations":
             modified_items[key] = {
                 **(value or {}),
                 **destination_dict[key],
             }
 
     # Update destination's fields with the merged dictionary
     for key, value in modified_items.items():
         setattr(destination, key, value)
-    destination._last_persistent_instance = source._last_persistent_instance
+
     return destination
```

### Comparing `synapseclient-4.1.1/synapseclient/core/version_check.py` & `synapseclient-4.2.0/synapseclient/core/version_check.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/entity.py` & `synapseclient-4.2.0/synapseclient/entity.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/evaluation.py` & `synapseclient-4.2.0/synapseclient/evaluation.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/__init__.py` & `synapseclient-4.2.0/synapseclient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/activity.py` & `synapseclient-4.2.0/synapseclient/models/activity.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/annotations.py` & `synapseclient-4.2.0/synapseclient/models/annotations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import asyncio
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import date, datetime
 from typing import Dict, List, Optional, Union
 
-from opentelemetry import context, trace
+from opentelemetry import context
 
 from synapseclient import Synapse
 from synapseclient.annotations import ANNO_TYPE_TO_FUNC
 from synapseclient.api import set_annotations
-from synapseclient.core.async_utils import async_to_sync, otel_trace_method
+from synapseclient.core.async_utils import async_to_sync
 from synapseclient.core.utils import run_and_attach_otel_context
 from synapseclient.models.protocols.annotations_protocol import (
     AnnotationsSynchronousProtocol,
 )
 
-tracer = trace.get_tracer("synapseclient")
-
 
 @dataclass()
 @async_to_sync
 class Annotations(AnnotationsSynchronousProtocol):
     """Annotations that can be applied to a number of Synapse resources to provide
     additional information.
 
@@ -44,15 +42,15 @@
                 List[float],
                 List[int],
                 List[date],
                 List[datetime],
             ],
         ],
         None,
-    ]
+    ] = field(default_factory=dict)
     """Additional metadata associated with the object. The key is the name of your
     desired annotations. The value is an object containing a list of string values
     (use empty list to represent no values for key) and the value type associated with
     all values in the list.
     """
 
     id: Optional[str] = None
@@ -60,17 +58,14 @@
     a member variable on another class."""
 
     etag: Optional[str] = None
     """ Etag of the object to which this annotation belongs. To update an AnnotationV2,
     this field must match the current etag on the object. Not required if being used as
     a member variable on another class."""
 
-    @otel_trace_method(
-        method_to_trace_name=lambda self, **kwargs: f"Annotation_store: {self.id}"
-    )
     async def store_async(
         self,
         synapse_client: Optional[Synapse] = None,
     ) -> "Annotations":
         """Storing annotations to synapse.
 
         Arguments:
@@ -144,8 +139,8 @@
                 conversion_func = ANNO_TYPE_TO_FUNC[dict_to_convert[key]["type"]]
                 annotations[key] = [
                     conversion_func(v) for v in dict_to_convert[key]["value"]
                 ]
             else:
                 annotations[key] = dict_to_convert[key]
 
-        return annotations if annotations else None
+        return annotations
```

### Comparing `synapseclient-4.1.1/synapseclient/models/file.py` & `synapseclient-4.2.0/synapseclient/models/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,50 @@
+"""Script to work with Synapse files."""
+
+# pylint: disable=protected-access
 import asyncio
 import dataclasses
+import os
 from copy import deepcopy
 from dataclasses import dataclass, field
 from datetime import date, datetime
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
-from opentelemetry import context, trace
+from opentelemetry import context
 
 from synapseclient import Synapse
+from synapseclient.core import utils
 from synapseclient.core.async_utils import async_to_sync, otel_trace_method
-from synapseclient.core.exceptions import SynapseError
+from synapseclient.core.exceptions import (
+    SynapseError,
+    SynapseMalformedEntityError,
+    SynapseFileNotFoundError,
+)
+from synapseclient.core.upload.upload_functions_async import upload_file_handle
 from synapseclient.core.utils import (
     delete_none_keys,
     guess_file_name,
+    merge_dataclass_entities,
     run_and_attach_otel_context,
 )
 from synapseclient.entity import File as Synapse_File
 from synapseclient.models import Activity, Annotations
 from synapseclient.models.mixins.access_control import AccessControllable
 from synapseclient.models.protocols.file_protocol import FileSynchronousProtocol
+from synapseclient.models.services.search import get_id
+from synapseclient.models.services.storable_entity import store_entity
 from synapseclient.models.services.storable_entity_components import (
     store_entity_components,
 )
 from synapseutils.copy_functions import changeFileMetaData, copy
 
 if TYPE_CHECKING:
     from synapseclient.models import Folder, Project
 
 
-tracer = trace.get_tracer("synapseclient")
-
-
 @dataclass()
 class FileHandle:
     """A file handle is a pointer to a file stored in a specific location.
 
     Attributes:
         id: The ID of this FileHandle. All references to this FileHandle will use this
             ID. Synapse will generate this ID when the FileHandle is created.
@@ -119,175 +129,211 @@
 
     is_preview: Optional[bool] = None
     """Whether or not this is a preview of another file."""
 
     external_url: Optional[str] = None
     """The URL of the file if it is stored externally."""
 
+    def fill_from_dict(
+        self, synapse_instance: Dict[str, Union[bool, str, int]]
+    ) -> "FileHandle":
+        """
+        Converts a response from the REST API into this dataclass.
+
+        Arguments:
+            synapse_instance: The response from the REST API.
+            set_annotations: Whether to set the annotations from the response.
+
+        Returns:
+            The File object.
+        """
+        file_handle = self or FileHandle()
+        file_handle.id = synapse_instance.get("id", None)
+        file_handle.etag = synapse_instance.get("etag", None)
+        file_handle.created_by = synapse_instance.get("createdBy", None)
+        file_handle.created_on = synapse_instance.get("createdOn", None)
+        file_handle.modified_on = synapse_instance.get("modifiedOn", None)
+        file_handle.concrete_type = synapse_instance.get("concreteType", None)
+        file_handle.content_type = synapse_instance.get("contentType", None)
+        file_handle.content_md5 = synapse_instance.get("contentMd5", None)
+        file_handle.file_name = synapse_instance.get("fileName", None)
+        file_handle.storage_location_id = synapse_instance.get(
+            "storageLocationId", None
+        )
+        file_handle.content_size = synapse_instance.get("contentSize", None)
+        file_handle.status = synapse_instance.get("status", None)
+        file_handle.bucket_name = synapse_instance.get("bucketName", None)
+        file_handle.key = synapse_instance.get("key", None)
+        file_handle.preview_id = synapse_instance.get("previewId", None)
+        file_handle.is_preview = synapse_instance.get("isPreview", None)
+        file_handle.external_url = synapse_instance.get("externalURL", None)
+
+        return self
+
 
 @dataclass()
 @async_to_sync
 class File(FileSynchronousProtocol, AccessControllable):
     """A file within Synapse.
 
     Attributes:
         id: The unique immutable ID for this file. A new ID will be generated for new
             Files. Once issued, this ID is guaranteed to never change or be re-issued.
         name: The name of this entity. Must be 256 characters or less. Names may only
             contain: letters, numbers, spaces, underscores, hyphens, periods, plus
             signs, apostrophes, and parentheses. If not specified, the name will be
             derived from the file name.
         path: The path to the file on disk.
-        content_type: Used to manually specify Content-type header, for example
-            'application/png' or 'application/json; charset=UTF-8'. If not specified,
-            the content type will be derived from the file extension.
-
-
-            (Create Only)
-            This can be specified only during the initial store of this file.
-            In order to change this after the File has been created use
-            [synapseclient.models.File.change_metadata][].
         description: The description of this file. Must be 1000 characters or less.
-        etag: (Read Only) Synapse employs an Optimistic Concurrency Control (OCC) scheme
-            to handle concurrent updates. Since the E-Tag changes every time an entity
-            is updated it is used to detect when a client's current representation of an
-            entity is out-of-date.
-        created_on: (Read Only) The date this entity was created.
-        modified_on: (Read Only) The date this entity was last modified.
-        created_by: (Read Only) The ID of the user that created this entity.
-        modified_by: (Read Only) The ID of the user that last modified this entity.
         parent_id: The ID of the Entity that is the parent of this Entity. Setting this
             to a new value and storing it will move this File under the new parent.
-        version_number: (Read Only) The version number issued to this version on the
-            object.
-        version_label: The version label for this entity
+        version_label: The version label for this entity. Updates to the entity will
+            increment the version number.
         version_comment: The version comment for this entity
-        is_latest_version: (Read Only) If this is the latest version of the object.
         data_file_handle_id: ID of the file associated with this entity. You may define
             an existing data_file_handle_id to use the existing data_file_handle_id. The
             creator of the file must also be the owner of the data_file_handle_id to
             have permission to store the file.
-        file_handle: (Read Only) The file handle associated with this entity.
+        external_url: The external URL of this file. If this is set AND `synapse_store`
+            is False, only a reference to this URL and the file metadata will be stored
+            in Synapse. The file itself will not be uploaded. If this attribute is set
+            it will override the `path`.
         activity: The Activity model represents the main record of Provenance in
             Synapse. It is analygous to the Activity defined in the
             [W3C Specification](https://www.w3.org/TR/prov-n/) on Provenance.
         annotations: Additional metadata associated with the folder. The key is the name
             of your desired annotations. The value is an object containing a list of
             values (use empty list to represent no values for key) and the value type
             associated with all values in the list. To remove all annotations set this
-            to an empty dict `{}`.
+            to an empty dict `{}` or None and store the entity.
+
+    Attributes:
+        content_type: (New Upload Only)
+            Used to manually specify Content-type header, for example
+            'application/png' or 'application/json; charset=UTF-8'. If not specified,
+            the content type will be derived from the file extension.
+
+
+            This can be specified only during the initial store of this file or any time
+            there is a new file to upload.
+            In order to change this after the File has been created use
+            [synapseclient.models.File.change_metadata][].
+        content_size: (New Upload Only)
+            The size of the file in bytes. This can be specified only during the initial
+            creation of the File. This is also only applicable to files not uploaded to
+            Synapse. ie: `synapse_store` is False.
+
+    Attributes:
+        content_md5: (Store only) The MD5 of the file is known. If not supplied this
+            will be computed in the client is possible. If supplied for a file entity
+            already stored in Synapse it will be calculated again to check if a new
+            upload needs to occur. This will not be filled in during a read for data. It
+            is only used during a store operation. To retrieve the md5 of the file after
+            read from synapse use the `.file_handle.content_md5` attribute.
         create_or_update: (Store only)
             Indicates whether the method should automatically perform an
-            update if the 'obj' conflicts with an existing Synapse object.
+            update if the `file` conflicts with an existing Synapse object.
         force_version: (Store only)
-            Indicates whether the method should increment the version of the
-            object even if nothing has changed. An update to the MD5 of the file will
-            force a version update regardless of this flag.
+            Indicates whether the method should increment the version of the object if
+            something within the entity has changed. For example updating the
+            description or annotations. You may set this to False and an update to the
+            entity will not increment the version.
+
+            Updating the `version_label` attribute will also cause a version update
+            regardless  of this flag.
+
+            An update to the MD5 of the file will force a version update regardless of
+            this  flag.
         is_restricted: (Store only)
             If set to true, an email will be sent to the Synapse access control
             team to start the process of adding terms-of-use or review board approval
             for this entity. You will be contacted with regards to the specific data
             being restricted and the requirements of access.
+
+            This may be used only by an administrator of the specified file.
+
         synapse_store: (Store only)
             Whether the File should be uploaded or if false: only the path should
             be stored when [synapseclient.models.File.store][] is called.
+
+    Attributes:
         download_file: (Get only) If True the file will be downloaded.
         download_location: (Get only) The location to download the file to.
         if_collision: (Get only)
             Determines how to handle file collisions. Defaults to "keep.both". May be:
 
             - `overwrite.local`
             - `keep.local`
             - `keep.both`
         synapse_container_limit: (Get only)
             A Synanpse ID used to limit the search in Synapse if
             file is specified as a local file. That is, if the file is stored in
             multiple locations in Synapse only the ones in the specified folder/project
             will be returned.
+
+    Attributes:
+        etag: (Read Only) Synapse employs an Optimistic Concurrency Control (OCC) scheme
+            to handle concurrent updates. Since the E-Tag changes every time an entity
+            is updated it is used to detect when a client's current representation of an
+            entity is out-of-date.
+        created_on: (Read Only) The date this entity was created.
+        modified_on: (Read Only) The date this entity was last modified.
+        created_by: (Read Only) The ID of the user that created this entity.
+        modified_by: (Read Only) The ID of the user that last modified this entity.
+        version_number: (Read Only) The version number issued to this version on the
+            object.
+        is_latest_version: (Read Only) If this is the latest version of the object.
+        file_handle: (Read Only) The file handle associated with this entity.
     """
 
     id: Optional[str] = None
     """The unique immutable ID for this file. A new ID will be generated for new Files.
     Once issued, this ID is guaranteed to never change or be re-issued."""
 
     name: Optional[str] = None
     """
     The name of this entity. Must be 256 characters or less.
     Names may only contain: letters, numbers, spaces, underscores, hyphens, periods,
     plus signs, apostrophes, and parentheses. If not specified, the name will be
     derived from the file name.
     """
 
-    path: Optional[str] = None
+    path: Optional[str] = field(default=None, compare=False)
     """The path to the file on disk."""
 
-    content_type: Optional[str] = None
-    """
-    Used to manually specify Content-type header, for example 'application/png'
-    or 'application/json; charset=UTF-8'. If not specified, the content type will be
-    derived from the file extension.
-
-
-    (Create Only)
-    This can be specified only during the initial store of this file. In order to change
-    this after the File has been created use
-    [synapseclient.models.File.change_metadata][].
-    """
-
     description: Optional[str] = None
     """The description of this file. Must be 1000 characters or less."""
 
-    etag: Optional[str] = None
-    """
-    (Read Only)
-    Synapse employs an Optimistic Concurrency Control (OCC) scheme to handle
-    concurrent updates. Since the E-Tag changes every time an entity is updated it is
-    used to detect when a client's current representation of an entity is out-of-date.
-    """
-
-    created_on: Optional[str] = None
-    """(Read Only) The date this entity was created."""
-
-    modified_on: Optional[str] = None
-    """(Read Only) The date this entity was last modified."""
-
-    created_by: Optional[str] = None
-    """(Read Only) The ID of the user that created this entity."""
-
-    modified_by: Optional[str] = None
-    """(Read Only) The ID of the user that last modified this entity."""
-
     parent_id: Optional[str] = None
     """The ID of the Entity that is the parent of this Entity. Setting this to a new
     value and storing it will move this File under the new parent."""
 
-    version_number: Optional[int] = None
-    """(Read Only) The version number issued to this version on the object."""
-
     version_label: Optional[str] = None
-    """The version label for this entity"""
+    """The version label for this entity. Updates to the entity will increment the
+    version number."""
 
     version_comment: Optional[str] = None
-    """The version comment for this entity"""
-
-    is_latest_version: Optional[bool] = False
-    """(Read Only) If this is the latest version of the object."""
+    """The version comment for this entity."""
 
     data_file_handle_id: Optional[str] = None
     """
-    ID of the file associated with this entity. You may define an existing
+    ID of the file handle associated with this entity. You may define an existing
     data_file_handle_id to use the existing data_file_handle_id. The creator of the
     file must also be the owner of the data_file_handle_id to have permission to
     store the file.
     """
 
-    file_handle: Optional[FileHandle] = None
-    """(Read Only) The file handle associated with this entity."""
+    external_url: Optional[str] = field(default=None, compare=False)
+    """
+    The external URL of this file. If this is set AND `synapse_store` is False, only
+    a reference to this URL and the file metadata will be stored in Synapse. The file
+    itself will not be uploaded. If this attribute is set it will override the `path`.
+    """
 
-    activity: Optional[Activity] = None
+    activity: Optional[Activity] = field(default=None, compare=False)
     """The Activity model represents the main record of Provenance in Synapse.  It is
     analygous to the Activity defined in the
     [W3C Specification](https://www.w3.org/TR/prov-n/) on Provenance."""
 
     annotations: Optional[
         Dict[
             str,
@@ -296,118 +342,205 @@
                 List[bool],
                 List[float],
                 List[int],
                 List[date],
                 List[datetime],
             ],
         ]
-    ] = None
+    ] = field(default_factory=dict, compare=False)
     """Additional metadata associated with the folder. The key is the name of your
     desired annotations. The value is an object containing a list of values
     (use empty list to represent no values for key) and the value type associated with
     all values in the list. To remove all annotations set this to an empty dict `{}`."""
 
-    create_or_update: bool = field(default=True, repr=False)
+    content_type: Optional[str] = None
+    """
+    (New Upload Only)
+    Used to manually specify Content-type header, for example 'application/png'
+    or 'application/json; charset=UTF-8'. If not specified, the content type will be
+    derived from the file extension.
+
+    This can be specified only during the initial store of this file. In order to change
+    this after the File has been created use
+    [synapseclient.models.File.change_metadata][].
+    """
+
+    content_size: Optional[int] = None
+    """
+    (New Upload Only)
+    The size of the file in bytes. This can be specified only during the initial
+    creation of the File. This is also only applicable to files not uploaded to Synapse.
+    ie: `synapse_store` is False.
+    """
+
+    content_md5: Optional[str] = field(default=None, compare=False)
+    """
+    (Store only)
+    The MD5 of the file is known. If not supplied this will be computed in the client
+    is possible. If supplied for a file entity already stored in Synapse it will be
+    calculated again to check if a new upload needs to occur. This will not be filled
+    in during a read for data. It is only used during a store operation. To retrieve
+    the md5 of the file after read from synapse use the `.file_handle.content_md5`
+    attribute.
+    """
+
+    create_or_update: bool = field(default=True, repr=False, compare=False)
     """
     (Store only)
 
     Indicates whether the method should automatically perform an update if the file
     conflicts with an existing Synapse object.
     """
 
-    force_version: bool = field(default=True, repr=False)
+    force_version: bool = field(default=True, repr=False, compare=False)
     """
     (Store only)
 
-    Indicates whether the method should increment the version of the object even if
-    nothing has changed. An update to the MD5 of the file will force a version update
-    regardless of this flag.
+    Indicates whether the method should increment the version of the object if something
+    within the entity has changed. For example updating the description or annotations.
+    You may set this to False and an update to the entity will not increment the
+    version.
+
+    Updating the `version_label` attribute will also cause a version update regardless
+    of this flag.
+
+    An update to the MD5 of the file will force a version update regardless of this
+    flag.
     """
 
     is_restricted: bool = field(default=False, repr=False)
     """
     (Store only)
 
     If set to true, an email will be sent to the Synapse access control team to start
     the process of adding terms-of-use or review board approval for this entity.
     You will be contacted with regards to the specific data being restricted and the
     requirements of access.
+
+    This may be used only by an administrator of the specified file.
     """
 
     synapse_store: bool = field(default=True, repr=False)
     """
     (Store only)
 
     Whether the File should be uploaded or if false: only the path should be stored when
     [synapseclient.models.File.store][] is called.
     """
 
-    download_file: bool = field(default=True, repr=False)
+    download_file: bool = field(default=True, repr=False, compare=False)
     """
     (Get only)
 
     If True the file will be downloaded."""
 
-    download_location: str = field(default=None, repr=False)
+    download_location: str = field(default=None, repr=False, compare=False)
     """
     (Get only)
 
     The location to download the file to."""
 
-    if_collision: str = field(default="keep.both", repr=False)
+    if_collision: str = field(default="keep.both", repr=False, compare=False)
     """
     (Get only)
 
     Determines how to handle file collisions. Defaults to "keep.both".
             May be
 
             - `overwrite.local`
             - `keep.local`
             - `keep.both`
     """
 
-    synapse_container_limit: Optional[str] = field(default=None, repr=False)
+    synapse_container_limit: Optional[str] = field(
+        default=None, repr=False, compare=False
+    )
     """A Synanpse ID used to limit the search in Synapse if file is specified as a local
     file. That is, if the file is stored in multiple locations in Synapse only the
     ones in the specified folder/project will be returned."""
 
+    etag: Optional[str] = field(default=None, compare=False)
+    """
+    (Read Only)
+    Synapse employs an Optimistic Concurrency Control (OCC) scheme to handle
+    concurrent updates. Since the E-Tag changes every time an entity is updated it is
+    used to detect when a client's current representation of an entity is out-of-date.
+    """
+
+    created_on: Optional[str] = field(default=None, compare=False)
+    """(Read Only) The date this entity was created."""
+
+    modified_on: Optional[str] = field(default=None, compare=False)
+    """(Read Only) The date this entity was last modified."""
+
+    created_by: Optional[str] = field(default=None, compare=False)
+    """(Read Only) The ID of the user that created this entity."""
+
+    modified_by: Optional[str] = field(default=None, compare=False)
+    """(Read Only) The ID of the user that last modified this entity."""
+
+    version_number: Optional[int] = field(default=None, compare=False)
+    """(Read Only) The version number issued to this version on the object."""
+
+    is_latest_version: Optional[bool] = field(default=None, compare=False)
+    """(Read Only) If this is the latest version of the object."""
+
+    file_handle: Optional[FileHandle] = field(default=None, compare=False)
+    """(Read Only) The file handle associated with this entity."""
+
     _last_persistent_instance: Optional["File"] = field(
         default=None, repr=False, compare=False
     )
     """The last persistent instance of this object. This is used to determine if the
     object has been changed and needs to be updated in Synapse."""
 
+    @property
+    def has_changed(self) -> bool:
+        """Determines if the object has been changed and needs to be updated in Synapse."""
+        return (
+            not self._last_persistent_instance or self._last_persistent_instance != self
+        )
+
     def _set_last_persistent_instance(self) -> None:
         """Stash the last time this object interacted with Synapse. This is used to
         determine if the object has been changed and needs to be updated in Synapse."""
         del self._last_persistent_instance
         self._last_persistent_instance = dataclasses.replace(self)
         self._last_persistent_instance.activity = (
             dataclasses.replace(self.activity) if self.activity else None
         )
         self._last_persistent_instance.annotations = (
-            deepcopy(self.annotations) if self.annotations else None
+            deepcopy(self.annotations) if self.annotations else {}
         )
 
+    def _fill_from_file_handle(self) -> None:
+        """Fill the file object from the file handle."""
+        if self.file_handle:
+            self.data_file_handle_id = self.file_handle.id
+            self.content_type = self.file_handle.content_type
+            self.content_size = self.file_handle.content_size
+            self.external_url = self.file_handle.external_url
+
     def fill_from_dict(
-        self, synapse_file: Union[Synapse_File, Dict], set_annotations: bool = True
+        self,
+        synapse_file: Union[Synapse_File, Dict[str, Union[bool, str, int]]],
+        set_annotations: bool = True,
     ) -> "File":
         """
         Converts a response from the REST API into this dataclass.
 
         Arguments:
             synapse_file: The response from the REST API.
             set_annotations: Whether to set the annotations from the response.
 
         Returns:
             The File object.
         """
         self.id = synapse_file.get("id", None)
         self.name = synapse_file.get("name", None)
-        self.path = synapse_file.get("path", None)
         self.description = synapse_file.get("description", None)
         self.etag = synapse_file.get("etag", None)
         self.created_on = synapse_file.get("createdOn", None)
         self.modified_on = synapse_file.get("modifiedOn", None)
         self.created_by = synapse_file.get("createdBy", None)
         self.modified_by = synapse_file.get("modifiedBy", None)
         self.parent_id = synapse_file.get("parentId", None)
@@ -415,42 +548,97 @@
         self.version_label = synapse_file.get("versionLabel", None)
         self.version_comment = synapse_file.get("versionComment", None)
         self.is_latest_version = synapse_file.get("isLatestVersion", False)
         self.data_file_handle_id = synapse_file.get("dataFileHandleId", None)
         synapse_file_handle = synapse_file.get("_file_handle", None)
         if synapse_file_handle:
             file_handle = self.file_handle or FileHandle()
-            self.file_handle = file_handle
-            file_handle.id = synapse_file_handle.get("id", None)
-            file_handle.etag = synapse_file_handle.get("etag", None)
-            file_handle.created_by = synapse_file_handle.get("createdBy", None)
-            file_handle.created_on = synapse_file_handle.get("createdOn", None)
-            file_handle.modified_on = synapse_file_handle.get("modifiedOn", None)
-            file_handle.concrete_type = synapse_file_handle.get("concreteType", None)
-            self.content_type = synapse_file_handle.get("contentType", None)
-            file_handle.content_type = synapse_file_handle.get("contentType", None)
-            file_handle.content_md5 = synapse_file_handle.get("contentMd5", None)
-            file_handle.file_name = synapse_file_handle.get("fileName", None)
-            file_handle.storage_location_id = synapse_file_handle.get(
-                "storageLocationId", None
-            )
-            file_handle.content_size = synapse_file_handle.get("contentSize", None)
-            file_handle.status = synapse_file_handle.get("status", None)
-            file_handle.bucket_name = synapse_file_handle.get("bucketName", None)
-            file_handle.key = synapse_file_handle.get("key", None)
-            file_handle.preview_id = synapse_file_handle.get("previewId", None)
-            file_handle.is_preview = synapse_file_handle.get("isPreview", None)
-            file_handle.external_url = synapse_file_handle.get("externalURL", None)
+            self.file_handle = file_handle.fill_from_dict(
+                synapse_instance=synapse_file_handle
+            )
+            self._fill_from_file_handle()
 
         if set_annotations:
             self.annotations = Annotations.from_dict(
-                synapse_file.get("annotations", None)
+                synapse_file.get("annotations", {})
             )
         return self
 
+    def _cannot_store(self) -> bool:
+        """Determines based on some guard conditions if we are unable to continue with
+        a store operation."""
+        return (
+            not (
+                self.id is not None
+                and (self.path is not None or self.data_file_handle_id is not None)
+            )
+            and not (self.path is not None and self.parent_id is not None)
+            and not (
+                self.parent_id is not None and self.data_file_handle_id is not None
+            )
+        )
+
+    async def _load_local_md5(self, syn: "Synapse") -> None:
+        """Load the MD5 of the file if it's a local file and we have not already loaded
+        it."""
+        if not self.content_md5 and self.path and os.path.isfile(self.path):
+            self.content_md5 = await utils.md5_for_file_multiprocessing(
+                filename=self.path,
+                process_pool_executor=syn._get_process_pool_executor(
+                    asyncio_event_loop=asyncio.get_running_loop()
+                ),
+                md5_semaphore=syn._get_md5_semaphore(
+                    asyncio_event_loop=asyncio.get_running_loop()
+                ),
+            )
+
+    async def _find_existing_file(
+        self, synapse_client: Optional[Synapse] = None
+    ) -> Union["File", None]:
+        """Determines if the file already exists in Synapse. If it does it will return
+        the file object, otherwise it will return None. This is used to determine if the
+        file should be updated or created."""
+
+        async def get_file(existing_id: str) -> "File":
+            """Small wrapper to retrieve a file instance without raising an error if it
+            does not exist.
+
+            Arguments:
+                existing_id: The ID of the file to retrieve.
+
+            Returns:
+                The file object if it exists, otherwise None.
+            """
+            try:
+                file_copy = File(
+                    id=existing_id,
+                    download_file=False,
+                    version_number=self.version_number,
+                    synapse_container_limit=self.synapse_container_limit,
+                    parent_id=self.parent_id,
+                )
+                return await file_copy.get_async(synapse_client=synapse_client)
+            except SynapseFileNotFoundError:
+                return None
+
+        if (
+            self.create_or_update
+            and not self._last_persistent_instance
+            and (
+                existing_file_id := await get_id(
+                    entity=self,
+                    failure_strategy=None,
+                    synapse_client=synapse_client,
+                )
+            )
+            and (existing_file := await get_file(existing_file_id))
+        ):
+            return existing_file
+        return None
+
     @otel_trace_method(
         method_to_trace_name=lambda self, **kwargs: f"File_Store: {self.path if self.path else self.id}"
     )
     async def store_async(
         self,
         parent: Optional[Union["Folder", "Project"]] = None,
         synapse_client: Optional[Synapse] = None,
@@ -464,113 +652,130 @@
             `synapse_store` to False.
         - Change the name of a file in Synapse by setting the `name` attribute of the
             File object. Also see the [synapseclient.models.File.change_metadata][]
             method for changing the name of the downloaded file.
         - Moving a file to a new parent by setting the `parent_id` attribute of the
             File object.
 
+        If no Name is specified this will be derived from the file name. This is the
+        reccommended way to store a file in Synapse.
+
+        Please note:
+        The file, as it appears on disk, will be the file that is downloaded from
+        Synapse. The name of the actual File is different from the name of the File
+        Entity in Synapse. It is generally not reccommended to specify a different
+        name for the Entity and the file as it will cause confusion and potential
+        conflicts later on.
+
         Arguments:
             parent: The parent folder or project to store the file in. May also be
                 specified in the File object. If both are provided the parent passed
                 into `store` will take precedence.
             synapse_client: If not passed in or None this will use the last client from
                 the `.login()` method.
 
         Returns:
             The file object.
 
+        Raises:
+            ValueError: If the file does not have an ID and a path, or a path and a
+                parent ID, or a data file handle ID and a parent ID.
 
         Example: Using this function
             File with the ID `syn123` at path `path/to/file.txt`:
 
                 file_instance = await File(id="syn123", path="path/to/file.txt").store_async()
 
             File at the path `path/to/file.txt` and a parent folder with the ID `syn456`:
 
                 file_instance = await File(path="path/to/file.txt", parent_id="syn456").store_async()
 
             File at the path `path/to/file.txt` and a parent folder with the ID `syn456`:
 
                 file_instance = await File(path="path/to/file.txt").store_async(parent=Folder(id="syn456"))
 
+            File with a parent and existing file handle (This allows multiple entities to reference the underlying file):
+
+                file_instance = await File(data_file_handle_id="123", parent_id="syn456").store_async()
+
             Rename a file (Does not update the file on disk or the name of the downloaded file):
 
                 file_instance = await File(id="syn123", download_file=False).get_async()
                 print(file_instance.name)  ## prints, e.g., "my_file.txt"
                 await file_instance.change_metadata_async(name="my_new_name_file.txt")
 
-            Rename a file, and the name of the file as downloaded (Does not update the file on disk):
+            Rename a file, and the name of the file as downloaded
+                (Does not update the file on disk). Is is reccommended that `name` and
+                `download_as` match to prevent confusion later on:
 
                 file_instance = await File(id="syn123", download_file=False).get_async()
                 print(file_instance.name)  ## prints, e.g., "my_file.txt"
                 await file_instance.change_metadata_async(name="my_new_name_file.txt", download_as="my_new_name_file.txt")
 
         """
-        if not (
-            self.id is not None
-            and (self.path is not None or self.data_file_handle_id is not None)
-        ) and not (
-            self.path is not None
-            and (parent.id if parent else self.parent_id) is not None
-        ):
+        self.parent_id = parent.id if parent else self.parent_id
+        if self._cannot_store():
             raise ValueError(
                 "The file must have an (ID with a (path or `data_file_handle_id`)), or a "
-                "(path with a (`parent_id` or parent with an id)) to store."
+                "(path with a (`parent_id` or parent with an id)), or a "
+                "(data_file_handle_id with a (`parent_id` or parent with an id)) to store."
             )
+        self.name = self.name or (guess_file_name(self.path) if self.path else None)
+        client = Synapse.get_client(synapse_client=synapse_client)
 
-        loop = asyncio.get_event_loop()
-        synapse_file = Synapse_File(
-            id=self.id,
-            path=self.path,
-            description=self.description,
-            etag=self.etag,
-            name=self.name or (guess_file_name(self.path) if self.path else None),
-            parent=parent.id if parent else self.parent_id,
-            contentType=self.content_type,
-            dataFileHandleId=self.data_file_handle_id,
-            synapseStore=self.synapse_store,
-            modifiedOn=self.modified_on,
-            versionLabel=self.version_label,
-            versionNumber=self.version_number,
-            versionComment=self.version_comment,
-        )
-        delete_none_keys(synapse_file)
-        current_context = context.get_current()
-        entity = await loop.run_in_executor(
-            None,
-            lambda: run_and_attach_otel_context(
-                lambda: Synapse.get_client(synapse_client=synapse_client).store(
-                    obj=synapse_file,
-                    createOrUpdate=self.create_or_update,
-                    forceVersion=self.force_version,
-                    isRestricted=self.is_restricted,
-                    set_annotations=False,
-                ),
-                current_context,
-            ),
-        )
+        if existing_file := await self._find_existing_file(synapse_client=client):
+            merge_dataclass_entities(source=existing_file, destination=self)
+
+        if self.path:
+            self.path = os.path.expanduser(self.path)
+            await self._upload_file(synapse_client=client)
+        elif self.data_file_handle_id:
+            self.path = client.cache.get(file_handle_id=self.data_file_handle_id)
+
+        if self.has_changed:
+            synapse_file = Synapse_File(
+                id=self.id,
+                path=self.path,
+                description=self.description,
+                etag=self.etag,
+                name=self.name,
+                parent=parent.id if parent else self.parent_id,
+                contentType=self.content_type,
+                contentSize=self.content_size,
+                dataFileHandleId=self.data_file_handle_id,
+                synapseStore=self.synapse_store,
+                modifiedOn=self.modified_on,
+                versionLabel=self.version_label,
+                versionNumber=self.version_number,
+                versionComment=self.version_comment,
+            )
+            delete_none_keys(synapse_file)
 
-        self.fill_from_dict(synapse_file=entity, set_annotations=False)
+            entity = await store_entity(
+                resource=self, entity=synapse_file, synapse_client=client
+            )
+
+            self.fill_from_dict(synapse_file=entity, set_annotations=False)
 
         re_read_required = await store_entity_components(
-            root_resource=self, synapse_client=synapse_client
+            root_resource=self, synapse_client=client
         )
         if re_read_required:
             before_download_file = self.download_file
             self.download_file = False
             await self.get_async(
-                synapse_client=synapse_client,
+                synapse_client=client,
             )
             self.download_file = before_download_file
 
         self._set_last_persistent_instance()
 
-        Synapse.get_client(synapse_client=synapse_client).logger.debug(
-            f"Stored File {self.name}, id: {self.id}: {self.path}"
-        )
+        client.logger.debug(f"Stored File {self.name}, id: {self.id}: {self.path}")
+        # Clear the content_md5 so that it is recalculated if the file is updated
+        self.content_md5 = None
         return self
 
     @otel_trace_method(
         method_to_trace_name=lambda self, **kwargs: f"File_Change_Metadata: {self.id}"
     )
     async def change_metadata_async(
         self,
@@ -591,15 +796,16 @@
             synapse_client: If not passed in or None this will use the last client from
                 the `.login()` method.
 
         Returns:
             The file object.
 
         Example: Using this function
-            Can be used to change the filename, the filename when the file is downloaded, or the file content-type without downloading:
+            Can be used to change the filename, the filename when the file is
+            downloaded, or the file content-type without downloading:
 
                 file_entity = await File(id="syn123", download_file=False).get_async()
                 print(os.path.basename(file_entity.path))  ## prints, e.g., "my_file.txt"
                 file_entity = await file_entity.change_metadata_async(name="my_new_name_file.txt", download_as="my_new_downloadAs_name_file.txt", content_type="text/plain")
                 print(os.path.basename(file_entity.path))  ## prints, "my_new_downloadAs_name_file.txt"
                 print(file_entity.name) ## prints, "my_new_name_file.txt"
 
@@ -680,34 +886,45 @@
 
             Assuming you have a file at the path "path/to/file.txt":
 
                 file_instance = await File(path="path/to/file.txt").get_async()
         """
         if not self.id and not self.path:
             raise ValueError("The file must have an ID or path to get.")
+        syn = Synapse.get_client(synapse_client=synapse_client)
 
         loop = asyncio.get_event_loop()
         current_context = context.get_current()
+        await self._load_local_md5(syn)
+
         entity = await loop.run_in_executor(
             None,
             lambda: run_and_attach_otel_context(
-                lambda: Synapse.get_client(synapse_client=synapse_client).get(
+                lambda: syn.get(
                     entity=self.id or self.path,
                     version=self.version_number,
                     ifcollision=self.if_collision,
-                    limitSearch=self.synapse_container_limit,
+                    limitSearch=self.synapse_container_limit or self.parent_id,
                     downloadFile=self.download_file,
                     downloadLocation=self.download_location,
+                    md5=self.content_md5,
                 ),
                 current_context,
             ),
         )
 
         self.fill_from_dict(synapse_file=entity, set_annotations=True)
 
+        if (
+            not self.path
+            and self.data_file_handle_id
+            and (cached_path := syn.cache.get(file_handle_id=self.data_file_handle_id))
+        ):
+            self.path = cached_path
+
         if include_activity:
             self.activity = await Activity.from_parent_async(
                 parent=self, synapse_client=synapse_client
             )
 
         self._set_last_persistent_instance()
         Synapse.get_client(synapse_client=synapse_client).logger.debug(
@@ -896,7 +1113,137 @@
             synapse_client=synapse_client
         )
         file_copy.download_file = True
         Synapse.get_client(synapse_client=synapse_client).logger.debug(
             f"Copied from file {self.id} to {parent_id} with new id of {file_copy.id}"
         )
         return file_copy
+
+    async def _needs_upload(self, syn: Synapse) -> bool:
+        """
+        Determines if a file needs to be uploaded to Synapse. The following conditions
+        apply:
+
+        - The file exists and is an ExternalFileHandle and the url has changed
+        - The file exists and is a local file and the MD5 has changed
+        - The file is not present in Synapse
+
+        If the file is already specifying a data_file_handle_id then it is assumed that
+        the file is already uploaded to Synapse. It does not need to be uploaded and
+        the only thing that will occur is the File metadata will be added to Synapse
+        outside of this upload process.
+
+        Arguments:
+            syn: If not passed in or None this will use the last client from
+                the `.login()` method.
+
+        Returns:
+            True if the file needs to be uploaded, otherwise False.
+        """
+        needs_upload = False
+        # Check if the file should be uploaded
+        if self._last_persistent_instance is not None:
+            if (
+                self.file_handle
+                and self.file_handle.concrete_type
+                == "org.sagebionetworks.repo.model.file.ExternalFileHandle"
+            ):
+                # switching away from ExternalFileHandle or the url was updated
+                needs_upload = self.synapse_store or (
+                    self.file_handle.external_url != self.external_url
+                )
+            else:
+                # Check if we need to upload a new version of an existing
+                # file. If the file referred to by entity['path'] has been
+                # modified, we want to upload the new version.
+                # If synapeStore is false then we must upload a ExternalFileHandle
+                needs_upload = (
+                    not self.synapse_store
+                    or not self.file_handle
+                    or not (
+                        exists_in_cache := syn.cache.contains(
+                            self.file_handle.id, self.path
+                        )
+                    )
+                )
+
+                md5_stored_in_synapse = (
+                    self.file_handle.content_md5 if self.file_handle else None
+                )
+
+                # Check if we got an MD5 checksum from Synapse and compare it to the local file
+                if (
+                    self.synapse_store
+                    and needs_upload
+                    and os.path.isfile(self.path)
+                    and md5_stored_in_synapse
+                ):
+                    await self._load_local_md5(syn)
+                    if md5_stored_in_synapse == (
+                        local_file_md5_hex := self.content_md5
+                    ):
+                        needs_upload = False
+
+                    # If we had a cache miss, but already uploaded to Synapse we
+                    # can add the file to the cache.
+                    if (
+                        not exists_in_cache
+                        and self.file_handle
+                        and self.file_handle.id
+                        and local_file_md5_hex
+                    ):
+                        syn.cache.add(
+                            file_handle_id=self.file_handle.id,
+                            path=self.path,
+                            md5=local_file_md5_hex,
+                        )
+        elif self.data_file_handle_id is not None:
+            needs_upload = False
+        else:
+            needs_upload = True
+        return needs_upload
+
+    async def _upload_file(
+        self,
+        synapse_client: Optional[Synapse] = None,
+    ) -> "File":
+        """The upload process for a file. This will upload the file to Synapse if it
+        needs to be uploaded. If the file does not need to be uploaded the file
+        metadata will be added to Synapse outside of this upload process.
+
+        Arguments:
+            synapse_client: If not passed in or None this will use the last client from
+                the `.login()` method.
+
+        Returns:
+            The file object.
+        """
+        syn = Synapse.get_client(synapse_client=synapse_client)
+
+        needs_upload = await self._needs_upload(syn=syn)
+
+        if needs_upload:
+            parent_id_for_upload = self.parent_id
+
+            if not parent_id_for_upload:
+                raise SynapseMalformedEntityError(
+                    "Entities of type File must have a parentId."
+                )
+
+            updated_file_handle = await upload_file_handle(
+                syn=syn,
+                parent_entity_id=parent_id_for_upload,
+                path=(
+                    self.path
+                    if (self.synapse_store or self.external_url is None)
+                    else self.external_url
+                ),
+                synapse_store=self.synapse_store,
+                md5=self.content_md5,
+                file_size=self.content_size,
+                mimetype=self.content_type,
+            )
+
+            self.file_handle = FileHandle().fill_from_dict(updated_file_handle)
+            self._fill_from_file_handle()
+
+        return self
```

### Comparing `synapseclient-4.1.1/synapseclient/models/folder.py` & `synapseclient-4.2.0/synapseclient/models/folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,14 @@
     store_entity_components,
 )
 from synapseutils import copy
 
 if TYPE_CHECKING:
     from synapseclient.models import Project
 
-tracer = trace.get_tracer("synapseclient")
-
 
 @dataclass()
 @async_to_sync
 class Folder(FolderSynchronousProtocol, AccessControllable, StorableContainer):
     """Folder is a hierarchical container for organizing data in Synapse.
 
     Attributes:
@@ -54,16 +52,16 @@
         created_by: (Read Only) The ID of the user that created this entity.
         modified_by: (Read Only) The ID of the user that last modified this entity.
         files: Files that exist within this folder.
         folders: Folders that exist within this folder.
         annotations: Additional metadata associated with the folder. The key is the name
             of your desired annotations. The value is an object containing a list of
             values (use empty list to represent no values for key) and the value type
-            associated with all values in the list.  To remove all annotations set this
-            to an empty dict `{}`.
+            associated with all values in the list. To remove all annotations set this
+            to an empty dict `{}` or None and store the entity.
         create_or_update: (Store only) Indicates whether the method should
             automatically perform an update if the resource conflicts with an existing
             Synapse object. When True this means that any changes to the resource will
             be non-destructive.
 
             This boolean is ignored if you've already stored or retrieved the resource
             from Synapse for this instance at least once. Any changes to the resource
@@ -120,19 +118,20 @@
                 List[bool],
                 List[float],
                 List[int],
                 List[date],
                 List[datetime],
             ],
         ]
-    ] = field(default=None, compare=False)
+    ] = field(default_factory=dict, compare=False)
     """Additional metadata associated with the folder. The key is the name of your
     desired annotations. The value is an object containing a list of values
     (use empty list to represent no values for key) and the value type associated with
-    all values in the list. To remove all annotations set this to an empty dict `{}`."""
+    all values in the list. To remove all annotations set this to an empty dict `{}`
+    or None and store the entity."""
 
     is_restricted: bool = field(default=False, repr=False)
     """
     (Store only)
 
     If set to true, an email will be sent to the Synapse access control team to start
     the process of adding terms-of-use or review board approval for this entity.
@@ -169,15 +168,15 @@
 
     def _set_last_persistent_instance(self) -> None:
         """Stash the last time this object interacted with Synapse. This is used to
         determine if the object has been changed and needs to be updated in Synapse."""
         del self._last_persistent_instance
         self._last_persistent_instance = replace(self)
         self._last_persistent_instance.annotations = (
-            deepcopy(self.annotations) if self.annotations else None
+            deepcopy(self.annotations) if self.annotations else {}
         )
 
     def fill_from_dict(
         self, synapse_folder: Synapse_Folder, set_annotations: bool = True
     ) -> "Folder":
         """
         Converts a response from the REST API into this dataclass.
@@ -252,15 +251,20 @@
                 existing_folder_id := await get_id(
                     entity=self, failure_strategy=None, synapse_client=synapse_client
                 )
             )
             and (existing_folder := await Folder(id=existing_folder_id).get_async())
         ):
             merge_dataclass_entities(source=existing_folder, destination=self)
-
+        trace.get_current_span().set_attributes(
+            {
+                "synapse.name": self.name or "",
+                "synapse.id": self.id or "",
+            }
+        )
         if self.has_changed:
             loop = asyncio.get_event_loop()
             synapse_folder = Synapse_Folder(
                 id=self.id,
                 name=self.name,
                 parent=parent_id,
                 etag=self.etag,
```

### Comparing `synapseclient-4.1.1/synapseclient/models/mixins/access_control.py` & `synapseclient-4.2.0/synapseclient/models/mixins/access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import asyncio
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
-from opentelemetry import context, trace
+from opentelemetry import context
 
 from synapseclient import Synapse
 from synapseclient.core.async_utils import async_to_sync
 from synapseclient.core.utils import run_and_attach_otel_context
 from synapseclient.models.protocols.access_control_protocol import (
     AccessControllableSynchronousProtocol,
 )
 
-tracer = trace.get_tracer("synapseclient")
-
 if TYPE_CHECKING:
     from synapseclient.core.models.permission import Permissions
 
 
 @async_to_sync
 class AccessControllable(AccessControllableSynchronousProtocol):
     """
```

### Comparing `synapseclient-4.1.1/synapseclient/models/mixins/storable_container.py` & `synapseclient-4.2.0/synapseclient/models/mixins/storable_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Mixin for objects that can have Folders and Files stored in them."""
 
 import asyncio
 import os
 from typing import TYPE_CHECKING, List, Optional, Union
 
-from opentelemetry import context, trace
+from opentelemetry import context
 from typing_extensions import Self
 
 from synapseclient import Synapse
 from synapseclient.core.async_utils import async_to_sync, otel_trace_method
 from synapseclient.core.constants.concrete_types import FILE_ENTITY, FOLDER_ENTITY
 from synapseclient.core.constants.method_flags import COLLISION_OVERWRITE_LOCAL
 from synapseclient.core.exceptions import SynapseError
@@ -20,16 +20,14 @@
     FailureStrategy,
     wrap_coroutine,
 )
 
 if TYPE_CHECKING:
     from synapseclient.models import File, Folder
 
-tracer = trace.get_tracer("synapseclient")
-
 
 @async_to_sync
 class StorableContainer(StorableContainerSynchronousProtocol):
     """
     Mixin for objects that can have Folders and Files stored in them.
 
     In order to use this mixin, the class must have the following attributes:
```

### Comparing `synapseclient-4.1.1/synapseclient/models/project.py` & `synapseclient-4.2.0/synapseclient/models/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 from synapseclient.models.services.search import get_id
 from synapseclient.models.services.storable_entity_components import (
     FailureStrategy,
     store_entity_components,
 )
 from synapseutils.copy_functions import copy
 
-tracer = trace.get_tracer("synapseclient")
-
 
 @dataclass()
 @async_to_sync
 class Project(ProjectSynchronousProtocol, AccessControllable, StorableContainer):
     """A Project is a top-level container for organizing data in Synapse.
 
     Attributes:
@@ -50,16 +48,16 @@
         modified_by: The ID of the user that last modified this entity.
         alias: The project alias for use in friendly project urls.
         files: Any files that are at the root directory of the project.
         folders: Any folders that are at the root directory of the project.
         annotations: Additional metadata associated with the folder. The key is the name
             of your desired annotations. The value is an object containing a list of
             values (use empty list to represent no values for key) and the value type
-            associated with all values in the list.  To remove all annotations set this
-            to an empty dict `{}`.
+            associated with all values in the list. To remove all annotations set this
+            to an empty dict `{}` or None and store the entity.
         create_or_update: (Store only) Indicates whether the method should
             automatically perform an update if the resource conflicts with an existing
             Synapse object. When True this means that any changes to the resource will
             be non-destructive.
 
             This boolean is ignored if you've already stored or retrieved the resource
             from Synapse for this instance at least once. Any changes to the resource
@@ -153,19 +151,20 @@
                 List[bool],
                 List[float],
                 List[int],
                 List[date],
                 List[datetime],
             ],
         ]
-    ] = field(default=None, compare=False)
+    ] = field(default_factory=dict, compare=False)
     """Additional metadata associated with the folder. The key is the name of your
     desired annotations. The value is an object containing a list of values
     (use empty list to represent no values for key) and the value type associated with
-    all values in the list. To remove all annotations set this to an empty dict `{}`."""
+    all values in the list. To remove all annotations set this to an empty dict `{}`
+    or None and store the entity."""
 
     create_or_update: bool = field(default=True, repr=False)
     """
     (Store only)
 
     Indicates whether the method should automatically perform an update if the resource
     conflicts with an existing Synapse object. When True this means that any changes
@@ -196,15 +195,15 @@
 
     def _set_last_persistent_instance(self) -> None:
         """Stash the last time this object interacted with Synapse. This is used to
         determine if the object has been changed and needs to be updated in Synapse."""
         del self._last_persistent_instance
         self._last_persistent_instance = replace(self)
         self._last_persistent_instance.annotations = (
-            deepcopy(self.annotations) if self.annotations else None
+            deepcopy(self.annotations) if self.annotations else {}
         )
 
     def fill_from_dict(
         self,
         synapse_project: Union[Synapse_Project, Dict],
         set_annotations: bool = True,
     ) -> "Project":
@@ -225,15 +224,15 @@
         self.modified_on = synapse_project.get("modifiedOn", None)
         self.created_by = synapse_project.get("createdBy", None)
         self.modified_by = synapse_project.get("modifiedBy", None)
         self.alias = synapse_project.get("alias", None)
         self.parent_id = synapse_project.get("parentId", None)
         if set_annotations:
             self.annotations = Annotations.from_dict(
-                synapse_project.get("annotations", None)
+                synapse_project.get("annotations", {})
             )
         return self
 
     @otel_trace_method(
         method_to_trace_name=lambda self, **kwargs: f"Project_Store: ID: {self.id}, Name: {self.name}"
     )
     async def store_async(
@@ -287,15 +286,20 @@
             and (
                 existing_project := await Project(id=existing_project_id).get_async(
                     synapse_client=synapse_client
                 )
             )
         ):
             merge_dataclass_entities(source=existing_project, destination=self)
-
+        trace.get_current_span().set_attributes(
+            {
+                "synapse.name": self.name or "",
+                "synapse.id": self.id or "",
+            }
+        )
         if self.has_changed:
             loop = asyncio.get_event_loop()
             synapse_project = Synapse_Project(
                 id=self.id,
                 etag=self.etag,
                 name=self.name,
                 description=self.description,
```

### Comparing `synapseclient-4.1.1/synapseclient/models/protocols/access_control_protocol.py` & `synapseclient-4.2.0/synapseclient/models/protocols/access_control_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/protocols/activity_protocol.py` & `synapseclient-4.2.0/synapseclient/models/protocols/activity_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/protocols/annotations_protocol.py` & `synapseclient-4.2.0/synapseclient/models/protocols/annotations_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/protocols/file_protocol.py` & `synapseclient-4.2.0/synapseclient/models/protocols/file_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/protocols/folder_protocol.py` & `synapseclient-4.2.0/synapseclient/models/protocols/folder_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/protocols/project_protocol.py` & `synapseclient-4.2.0/synapseclient/models/protocols/project_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/protocols/storable_container_protocol.py` & `synapseclient-4.2.0/synapseclient/models/protocols/storable_container_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/protocols/table_protocol.py` & `synapseclient-4.2.0/synapseclient/models/protocols/table_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/protocols/team_protocol.py` & `synapseclient-4.2.0/synapseclient/models/protocols/team_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/protocols/user_protocol.py` & `synapseclient-4.2.0/synapseclient/models/protocols/user_protocol.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/models/services/search.py` & `synapseclient-4.2.0/synapseclient/models/services/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Functional interface for searching for entities in Synapse."""
 
 import asyncio
 from typing import Union
 
-from opentelemetry import trace, context
+from opentelemetry import context
 
 from typing import Optional, TYPE_CHECKING
 
 
 from synapseclient import Synapse
 from synapseclient.core.utils import (
     run_and_attach_otel_context,
@@ -16,21 +16,19 @@
     FailureStrategy,
 )
 from synapseclient.core.exceptions import (
     SynapseNotFoundError,
 )
 
 if TYPE_CHECKING:
-    from synapseclient.models import Folder, Project
-
-tracer = trace.get_tracer("synapseclient")
+    from synapseclient.models import Folder, Project, File
 
 
 async def get_id(
-    entity: Union["Project", "Folder"],
+    entity: Union["Project", "Folder", "File"],
     failure_strategy: Optional[FailureStrategy] = FailureStrategy.RAISE_EXCEPTION,
     synapse_client: Optional[Synapse] = None,
 ) -> Union[str, None]:
     """
     Get the ID of the entity from either the ID field or the name/parent of the entity.
     This is a wrapper for the [synapseclient.Synapse.findEntityId][] method that is
     used in order to search by name/parent.
```

### Comparing `synapseclient-4.1.1/synapseclient/models/services/storable_entity_components.py` & `synapseclient-4.2.0/synapseclient/models/services/storable_entity_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     last_persistent_instance = (
         root_resource._last_persistent_instance
         if hasattr(root_resource, "_last_persistent_instance")
         else None
     )
     if (
         hasattr(root_resource, "annotations")
-        and root_resource.annotations is not None
+        and (root_resource.annotations or last_persistent_instance)
         and (
             last_persistent_instance is None
             or last_persistent_instance.annotations != root_resource.annotations
         )
     ):
         result = await Annotations(
             id=root_resource.id,
```

### Comparing `synapseclient-4.1.1/synapseclient/models/table.py` & `synapseclient-4.2.0/synapseclient/models/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import os
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import date, datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from opentelemetry import context, trace
 
 from synapseclient import Column as Synapse_Column
@@ -22,16 +22,14 @@
 from synapseclient.models.services.storable_entity_components import (
     store_entity_components,
 )
 from synapseclient.table import CsvFileTable as Synapse_CsvFileTable
 from synapseclient.table import TableQueryResult as Synaspe_TableQueryResult
 from synapseclient.table import delete_rows
 
-tracer = trace.get_tracer("synapseclient")
-
 
 # TODO: Have a plug-and-play interface to plugin different dataframes,
 # or perhaps stream a CSV back when querying for data and uploading data
 
 
 class FacetType(str, Enum):
     """Set to one of the enumerated values to indicate a column should be treated as
@@ -372,18 +370,19 @@
         version_number: The version number issued to this version on the object.
         version_label: The version label for this table
         version_comment: The version comment for this table
         is_latest_version: If this is the latest version of the object.
         is_search_enabled: When creating or updating a table or view specifies if full
             text search should be enabled. Note that enabling full text search might
             slow down the indexing of the table or view.
-        annotations: Additional metadata associated with the table. The key is the
-            name of your desired annotations. The value is an object containing a list
-            of values (use empty list to represent no values for key) and the value
-            type associated with all values in the list.
+        annotations: Additional metadata associated with the table. The key is the name
+            of your desired annotations. The value is an object containing a list of
+            values (use empty list to represent no values for key) and the value type
+            associated with all values in the list. To remove all annotations set this
+            to an empty dict `{}` or None and store the entity.
 
     """
 
     id: Optional[str] = None
     """The unique immutable ID for this table. A new ID will be generated for new
     Tables. Once issued, this ID is guaranteed to never change or be re-issued"""
 
@@ -450,19 +449,20 @@
                 List[bool],
                 List[float],
                 List[int],
                 List[date],
                 List[datetime],
             ],
         ]
-    ] = None
+    ] = field(default_factory=dict)
     """Additional metadata associated with the table. The key is the name of your
     desired annotations. The value is an object containing a list of values
     (use empty list to represent no values for key) and the value type associated with
-    all values in the list. To remove all annotations set this to an empty dict `{}`."""
+    all values in the list. To remove all annotations set this to an empty dict `{}`
+    or None and store the entity."""
 
     def fill_from_dict(
         self, synapse_table: Synapse_Table, set_annotations: bool = True
     ) -> "Table":
         """Converts the data coming from the Synapse API into this datamodel.
 
         :param synapse_table: The data coming from the Synapse API
@@ -484,15 +484,15 @@
         self.is_search_enabled = synapse_table.get("isSearchEnabled", False)
         self.columns = [
             Column(id=columnId, name=None, column_type=None)
             for columnId in synapse_table.get("columnIds", [])
         ]
         if set_annotations:
             self.annotations = Annotations.from_dict(
-                synapse_table.get("annotations", None)
+                synapse_table.get("annotations", {})
             )
         return self
 
     @otel_trace_method(
         method_to_trace_name=lambda _, **kwargs: f"Store_rows_by_csv: {kwargs.get('csv_path', None)}"
     )
     async def store_rows_from_csv_async(
@@ -599,15 +599,20 @@
                 print("I hit an exception")
 
         synapse_schema = Synapse_Schema(
             name=self.name,
             columns=self.columns,
             parent=self.parent_id,
         )
-
+        trace.get_current_span().set_attributes(
+            {
+                "synapse.name": self.name or "",
+                "synapse.id": self.id or "",
+            }
+        )
         loop = asyncio.get_event_loop()
         current_context = context.get_current()
         entity = await loop.run_in_executor(
             None,
             lambda: run_and_attach_otel_context(
                 lambda: Synapse.get_client(synapse_client=synapse_client).store(
                     obj=synapse_schema
@@ -697,26 +702,23 @@
             result_format: The format of the results. Defaults to CsvResultFormat().
             synapse_client: If not passed in or None this will use the last client
                 from the `.login()` method.
 
         Returns:
             The results of the query.
         """
-        with tracer.start_as_current_span("Table_query"):
-            loop = asyncio.get_event_loop()
-            current_context = context.get_current()
-
-            # TODO: Future Idea - We stream back a CSV, and let those reading this to handle the CSV however they want
-            results = await loop.run_in_executor(
-                None,
-                lambda: run_and_attach_otel_context(
-                    lambda: Synapse.get_client(
-                        synapse_client=synapse_client
-                    ).tableQuery(
-                        query=query,
-                        **result_format.to_dict(),
-                    ),
-                    current_context,
+        loop = asyncio.get_event_loop()
+        current_context = context.get_current()
+
+        # TODO: Future Idea - We stream back a CSV, and let those reading this to handle the CSV however they want
+        results = await loop.run_in_executor(
+            None,
+            lambda: run_and_attach_otel_context(
+                lambda: Synapse.get_client(synapse_client=synapse_client).tableQuery(
+                    query=query,
+                    **result_format.to_dict(),
                 ),
-            )
-            print(results)
-            return results
+                current_context,
+            ),
+        )
+        print(results)
+        return results
```

### Comparing `synapseclient-4.1.1/synapseclient/models/team.py` & `synapseclient-4.2.0/synapseclient/models/team.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from synapseclient.core.async_utils import async_to_sync, otel_trace_method
 from synapseclient.core.utils import run_and_attach_otel_context
 from synapseclient.models.protocols.team_protocol import TeamSynchronousProtocol
 from synapseclient.models.user import UserGroupHeader
 from synapseclient.team import Team as Synapse_Team
 from synapseclient.team import TeamMember as Synapse_TeamMember
 
-tracer = trace.get_tracer("synapseclient")
-
 
 @dataclass
 class TeamMember:
     """
     Contains information about a user's membership in a Team.
     In practice the constructor is not called directly by the client.
 
@@ -151,14 +149,20 @@
                 from the `.login()` method.
 
         Returns:
             Team: The Team object.
         """
         loop = asyncio.get_event_loop()
         current_context = context.get_current()
+        trace.get_current_span().set_attributes(
+            {
+                "synapse.name": self.name or "",
+                "synapse.id": self.id or "",
+            }
+        )
         team = await loop.run_in_executor(
             None,
             lambda: run_and_attach_otel_context(
                 lambda: Synapse.get_client(synapse_client=synapse_client).create_team(
                     name=self.name,
                     description=self.description,
                     icon=self.icon,
```

### Comparing `synapseclient-4.1.1/synapseclient/models/user.py` & `synapseclient-4.2.0/synapseclient/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import asyncio
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Union
 
-from opentelemetry import context, trace
+from opentelemetry import context
 
 from synapseclient import Synapse
 from synapseclient.core.async_utils import async_to_sync, otel_trace_method
 from synapseclient.core.utils import run_and_attach_otel_context
 from synapseclient.models.protocols.user_protocol import UserProfileSynchronousProtocol
 from synapseclient.team import UserGroupHeader as Synapse_UserGroupHeader
 from synapseclient.team import UserProfile as Synapse_UserProfile
 
-tracer = trace.get_tracer("synapseclient")
-
 
 @dataclass
 class UserGroupHeader:
     """
     Select metadata about a Synapse principal.
     In practice the constructor is not called directly by the client.
```

### Comparing `synapseclient-4.1.1/synapseclient/services/json_schema.py` & `synapseclient-4.2.0/synapseclient/services/json_schema.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/table.py` & `synapseclient-4.2.0/synapseclient/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,16 @@
 
 from synapseclient.core.utils import id_of, itersubclasses, from_unix_epoch_time
 from synapseclient.core.exceptions import SynapseError
 from synapseclient.core.models.dict_object import DictObject
 from .entity import Entity, entity_type_to_class, Folder, Project
 from .evaluation import Evaluation
 from synapseclient.core.constants import concrete_types
-from opentelemetry import trace
 
 
-tracer = trace.get_tracer("synapseclient")
-
 aggregate_pattern = re.compile(r"(count|max|min|avg|sum)\((.+)\)")
 
 # default is STRING, only need to put the non-STRING keys in here
 PANDAS_TABLE_TYPE = {
     "floating": "DOUBLE",
     "decimal": "DOUBLE",
     "integer": "INTEGER",
@@ -489,15 +486,14 @@
     delete_row_csv_filepath = _create_row_delete_csv(row_id_vers_list)
     try:
         syn._uploadCsv(delete_row_csv_filepath, schema)
     finally:
         os.remove(delete_row_csv_filepath)
 
 
-@tracer.start_as_current_span("Synapse::delete_rows")
 def delete_rows(
     syn,
     table_id: str,
     row_id_vers_list: List[Tuple[int, int]],
 ):
     """
     Deletes rows from a synapse table
```

### Comparing `synapseclient-4.1.1/synapseclient/team.py` & `synapseclient-4.2.0/synapseclient/team.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient/wiki.py` & `synapseclient-4.2.0/synapseclient/wiki.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseclient.egg-info/PKG-INFO` & `synapseclient-4.2.0/synapseclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapseclient
-Version: 4.1.1
+Version: 4.2.0
 Summary: A client for Synapse, a collaborative, open-source research platform that allows teams to share data, track analyses, and collaborate.
 Home-page: https://www.synapse.org
 Author: The Synapse Engineering Team
 Author-email: platform@sagebase.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/Sage-Bionetworks/synapsePythonClient
 Project-URL: Tracker, https://github.com/Sage-Bionetworks/synapsePythonClient/issues
@@ -32,14 +32,20 @@
 Requires-Dist: requests<3.0,>=2.22.0
 Requires-Dist: urllib3<2,>=1.26.18
 Requires-Dist: deprecated<2.0,>=1.2.4
 Requires-Dist: opentelemetry-api~=1.21.0
 Requires-Dist: opentelemetry-sdk~=1.21.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-http~=1.21.0
 Requires-Dist: nest-asyncio~=1.6.0
+Requires-Dist: asyncio-atexit~=1.0.1
+Requires-Dist: httpx~=0.27.0
+Requires-Dist: tqdm<5.0,>=4.66.2
+Requires-Dist: loky~=3.0.0
+Requires-Dist: async-lru~=2.0.4
+Requires-Dist: psutil~=5.9.8
 Provides-Extra: dev
 Requires-Dist: pytest<7.0,>=6.0.0; extra == "dev"
 Requires-Dist: pytest-mock<4.0,>=3.0; extra == "dev"
 Requires-Dist: pytest-socket~=0.6.0; extra == "dev"
 Requires-Dist: pytest-asyncio~=0.19; extra == "dev"
 Requires-Dist: flake8<4.0,>=3.7.0; extra == "dev"
 Requires-Dist: pytest-xdist[psutil]<3.0.0,>=2.2; extra == "dev"
```

### Comparing `synapseclient-4.1.1/synapseclient.egg-info/SOURCES.txt` & `synapseclient-4.2.0/synapseclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 synapseclient.egg-info/dependency_links.txt
 synapseclient.egg-info/entry_points.txt
 synapseclient.egg-info/not-zip-safe
 synapseclient.egg-info/requires.txt
 synapseclient.egg-info/top_level.txt
 synapseclient/api/__init__.py
 synapseclient/api/annotations.py
+synapseclient/api/entity_bundle_services_v2.py
+synapseclient/api/entity_services.py
+synapseclient/api/file_services.py
 synapseclient/core/__init__.py
 synapseclient/core/async_utils.py
 synapseclient/core/cache.py
 synapseclient/core/config.py
 synapseclient/core/cumulative_transfer_progress.py
 synapseclient/core/dozer.py
 synapseclient/core/exceptions.py
@@ -51,15 +54,18 @@
 synapseclient/core/models/custom_json.py
 synapseclient/core/models/dict_object.py
 synapseclient/core/models/permission.py
 synapseclient/core/multithread_download/__init__.py
 synapseclient/core/multithread_download/download_threads.py
 synapseclient/core/upload/__init__.py
 synapseclient/core/upload/multipart_upload.py
+synapseclient/core/upload/multipart_upload_async.py
 synapseclient/core/upload/upload_functions.py
+synapseclient/core/upload/upload_functions_async.py
+synapseclient/core/upload/upload_utils.py
 synapseclient/models/__init__.py
 synapseclient/models/activity.py
 synapseclient/models/annotations.py
 synapseclient/models/evaluation.py
 synapseclient/models/file.py
 synapseclient/models/folder.py
 synapseclient/models/project.py
@@ -79,14 +85,15 @@
 synapseclient/models/protocols/project_protocol.py
 synapseclient/models/protocols/storable_container_protocol.py
 synapseclient/models/protocols/table_protocol.py
 synapseclient/models/protocols/team_protocol.py
 synapseclient/models/protocols/user_protocol.py
 synapseclient/models/services/__init__.py
 synapseclient/models/services/search.py
+synapseclient/models/services/storable_entity.py
 synapseclient/models/services/storable_entity_components.py
 synapseclient/services/__init__.py
 synapseclient/services/json_schema.py
 synapseutils/__init__.py
 synapseutils/copy_functions.py
 synapseutils/describe_functions.py
 synapseutils/migrate_functions.py
```

### Comparing `synapseclient-4.1.1/synapseclient.egg-info/requires.txt` & `synapseclient-4.2.0/synapseclient.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 requests<3.0,>=2.22.0
 urllib3<2,>=1.26.18
 deprecated<2.0,>=1.2.4
 opentelemetry-api~=1.21.0
 opentelemetry-sdk~=1.21.0
 opentelemetry-exporter-otlp-proto-http~=1.21.0
 nest-asyncio~=1.6.0
+asyncio-atexit~=1.0.1
+httpx~=0.27.0
+tqdm<5.0,>=4.66.2
+loky~=3.0.0
+async-lru~=2.0.4
+psutil~=5.9.8
 
 [boto3]
 boto3<2.0,>=1.7.0
 
 [dev]
 pytest<7.0,>=6.0.0
 pytest-mock<4.0,>=3.0
```

### Comparing `synapseclient-4.1.1/synapseutils/__init__.py` & `synapseclient-4.2.0/synapseutils/__init__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseutils/copy_functions.py` & `synapseclient-4.2.0/synapseutils/copy_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,15 +256,45 @@
                         the object even if nothing has changed. Defaults to True.
         name: Specify filename to change the filename of the file.
 
     Returns:
         Synapse Entity
 
     Example: Using this function
-        Can be used to change the filename, the filename when the file is downloaded, or the file content-type without downloading:
+        Updating all file 'downloadAs' names within a folder to match the name of the
+        entity.
+
+            import synapseclient
+            import synapseutils
+
+
+            syn = synapseclient.Synapse()
+            syn.login()
+
+            MY_FOLDER_TO_UPDATE_ALL_FILES_IN = "syn123"
+
+            for files_to_update in syn.getChildren(
+                parent=MY_FOLDER_TO_UPDATE_ALL_FILES_IN, includeTypes=["file"]
+            ):
+                file_to_check = syn.get(files_to_update["id"], downloadFile=False)
+                if file_to_check.name != file_to_check["_file_handle"]["fileName"]:
+                    print(
+                        f"Updating downloadAs for {file_to_check['_file_handle']['fileName']} to {file_to_check.name}"
+                    )
+
+                    synapseutils.changeFileMetaData(
+                        syn=syn,
+                        entity=file_to_check.id,
+                        downloadAs=file_to_check.name,
+                        forceVersion=False,
+                    )
+
+
+        Can be used to change the filename, the filename when the file is downloaded,
+        or the file content-type without downloading:
 
             file_entity = syn.get(synid)
             print(os.path.basename(file_entity.path))  ## prints, e.g., "my_file.txt"
             file_entity = synapseutils.changeFileMetaData(syn=syn, entity=file_entity, downloadAs="my_new_downloadAs_name_file.txt", name="my_new_name_file.txt")
             print(os.path.basename(file_entity.path))  ## prints, "my_new_downloadAs_name_file.txt"
             print(file_entity.name) ## prints, "my_new_name_file.txt"
     """
```

### Comparing `synapseclient-4.1.1/synapseutils/describe_functions.py` & `synapseclient-4.2.0/synapseutils/describe_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseutils/migrate_functions.py` & `synapseclient-4.2.0/synapseutils/migrate_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseutils/monitor.py` & `synapseclient-4.2.0/synapseutils/monitor.py`

 * *Files identical despite different names*

### Comparing `synapseclient-4.1.1/synapseutils/sync.py` & `synapseclient-4.2.0/synapseutils/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 )
 from synapseclient.core.multithread_download.download_threads import (
     shared_executor as download_shared_executor,
 )
 from synapseclient.core.upload.multipart_upload import (
     shared_executor as upload_shared_executor,
 )
-from opentelemetry import trace, context
+from opentelemetry import context, trace
 from opentelemetry.context import Context
 
 
 REQUIRED_FIELDS = ["path", "parent"]
 FILE_CONSTRUCTOR_FIELDS = ["name", "id", "synapseStore", "contentType"]
 STORE_FUNCTION_FIELDS = ["activityName", "activityDescription", "forceVersion"]
 PROVENANCE_FIELDS = ["used", "executed"]
@@ -59,16 +59,14 @@
 ]
 ARRAY_BRACKET_PATTERN = re.compile(r"^\[.*\]$")
 SINGLE_OPEN_BRACKET_PATTERN = re.compile(r"^\[")
 SINGLE_CLOSING_BRACKET_PATTERN = re.compile(r"\]$")
 # https://stackoverflow.com/questions/18893390/splitting-on-comma-outside-quotes
 COMMAS_OUTSIDE_DOUBLE_QUOTES_PATTERN = re.compile(r",(?=(?:[^\"]*\"[^\"]*\")*[^\"]*$)")
 
-tracer = trace.get_tracer("synapseclient")
-
 
 @contextmanager
 def _sync_executor(syn):
     """Use this context manager to run some sync code with an executor that will
     be created and then shutdown once the context completes."""
     if syn.max_threads < 2 or config.single_threaded:
         executor = SingleThreadExecutor()
@@ -77,15 +75,14 @@
 
     try:
         yield executor
     finally:
         executor.shutdown()
 
 
-@tracer.start_as_current_span("sync::syncFromSynapse")
 def syncFromSynapse(
     syn,
     entity,
     path=None,
     ifcollision="overwrite.local",
     allFiles=None,
     followLink=False,
@@ -545,17 +542,17 @@
     Files will be uploaded concurrently and in an order that honors any
     interdependent provenance.
 
     """
 
     def __init__(
         self,
-        syn,
+        syn: Synapse,
         executor: concurrent.futures.Executor,
-        max_concurrent_file_transfers=None,
+        max_concurrent_file_transfers: int = None,
     ):
         """
         Arguments:
             syn: A synapse client
             executor: An ExecutorService in which concurrent file downloads
                       can be scheduled
         """
@@ -625,15 +622,14 @@
                 future.cancel()
 
         # if we are aborted by definition one of the futures should have an
         # exception.
         # if somehow not from None fuctions fine
         raise ValueError("Sync aborted due to upload failure") from exception
 
-    @tracer.start_as_current_span("sync::_SyncUploader::upload")
     def upload(self, items: typing.Iterable[_SyncUploadItem]):
         progress = CumulativeTransferProgress("Uploaded")
 
         # flag to set in a child in an upload thread if an error occurs to signal
         # to the entrant thread to stop processing.
         abort_event = threading.Event()
 
@@ -741,15 +737,19 @@
             with upload_shared_executor(self._executor):
                 # we configure an upload thread local shared executor so that any
                 # multipart uploads that result from this upload will share the
                 # executor of this sync rather than creating their own threadpool.
 
                 with progress.accumulate_progress():
                     entity = self._syn.store(
-                        item.entity, used=used, executed=executed, **item.store_kwargs
+                        item.entity,
+                        used=used,
+                        executed=executed,
+                        **item.store_kwargs,
+                        async_file_handle_upload=False,
                     )
 
                 with dependency_condition:
                     finished_items[item.entity.path] = entity
                     try:
                         pending_provenance.finished(item.entity.path)
 
@@ -1070,15 +1070,14 @@
             f'\nThe specified path "{f}" is either not a file path or does not exist.',
             file=sys.stderr,
         )
         raise IOError("The path %s is not a file or does not exist" % f)
     return path_normalized
 
 
-@tracer.start_as_current_span("sync::readManifestFile")
 def readManifestFile(syn, manifestFile):
     """Verifies a file manifest and returns a reordered dataframe ready for upload.
 
     [Read more about the manifest file format](../../explanations/manifest_tsv/)
 
     Arguments:
         syn: A Synapse object with user's login, e.g. syn = synapseclient.login()
@@ -1161,15 +1160,14 @@
                 "\n%s in the parent column is is not a Folder or Project\n" % synId
             )
             raise SynapseHTTPError
     sys.stdout.write("OK\n")
     return df
 
 
-@tracer.start_as_current_span("sync::syncToSynapse")
 def syncToSynapse(
     syn, manifestFile, dryRun=False, sendMessages=True, retries=MAX_RETRIES
 ) -> None:
     """Synchronizes files specified in the manifest file to Synapse.
 
     Given a file describing all of the uploads, this uploads the content to Synapse and
     optionally notifies you via Synapse messagging (email) at specific intervals, on
@@ -1392,15 +1390,14 @@
                 raise ValueError(
                     "File {} is empty, empty files cannot be uploaded to Synapse".format(
                         file_name
                     )
                 )
 
 
-@tracer.start_as_current_span("sync::generate_sync_manifest")
 def generate_sync_manifest(syn, directory_path, parent_id, manifest_path) -> None:
     """Generate manifest for [syncToSynapse][synapseutils.sync.syncToSynapse] from a local directory.
 
     [Read more about the manifest file format](../../explanations/manifest_tsv/)
 
     Arguments:
         syn: A Synapse object with user's login, e.g. syn = synapseclient.login()
```

### Comparing `synapseclient-4.1.1/synapseutils/walk_functions.py` & `synapseclient-4.2.0/synapseutils/walk_functions.py`

 * *Files identical despite different names*

