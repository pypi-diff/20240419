# Comparing `tmp/domino-py-0.9.1.tar.gz` & `tmp/domino_py-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.9.1.tar", last modified: Fri Feb 23 17:15:50 2024, max compression
+gzip compressed data, was "domino_py-0.9.2.tar", last modified: Fri Apr 19 19:05:41 2024, max compression
```

## Comparing `domino-py-0.9.1.tar` & `domino_py-0.9.2.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.171075 domino-py-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-02-23 17:15:34.000000 domino-py-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24428 2024-02-23 17:15:50.171075 domino-py-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9253 2024-02-23 17:15:34.000000 domino-py-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-23 17:15:34.000000 domino-py-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 17:15:50.171075 domino-py-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.155076 domino-py-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.155076 domino-py-0.9.1/src/domino/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.155076 domino-py-0.9.1/src/domino/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/actions/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.159076 domino-py-0.9.1/src/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.159076 domino-py-0.9.1/src/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/cli/utils/config-domino-local.toml
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/cli/utils/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    40723 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.159076 domino-py-0.9.1/src/domino/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/client/github_rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.159076 domino-py-0.9.1/src/domino/client/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/client/legacy/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/client/legacy/s3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/client/local_files_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.159076 domino-py-0.9.1/src/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.163076 domino-py-0.9.1/src/domino/custom_operators/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/deprecated/base_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/deprecated/external_python_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/docker_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    26228 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.163076 domino-py-0.9.1/src/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/sidecar/fuse.conf
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/sidecar/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/sidecar/rclone.conf
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/sidecar/sidecar_lifecycle.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/custom_operators/worker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.163076 domino-py-0.9.1/src/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.163076 domino-py-0.9.1/src/domino/models/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/models/output_modifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.163076 domino-py-0.9.1/src/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/schemas/deploy_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/schemas/display_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.163076 domino-py-0.9.1/src/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/scripts/build_docker_images_pieces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.167075 domino-py-0.9.1/src/domino/scripts/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/scripts/deprecated/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/scripts/deprecated/deprecated_piece_dry_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/scripts/deprecated/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/scripts/deprecated/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/scripts/deprecated/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/scripts/run_piece_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.167075 domino-py-0.9.1/src/domino/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/storage/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.167075 domino-py-0.9.1/src/domino/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/testing/dry_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/testing/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/testing/http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.167075 domino-py-0.9.1/src/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/utils/piece_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-23 17:15:34.000000 domino-py-0.9.1/src/domino/utils/workflow_shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 17:15:50.167075 domino-py-0.9.1/src/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24428 2024-02-23 17:15:50.000000 domino-py-0.9.1/src/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-02-23 17:15:50.000000 domino-py-0.9.1/src/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 17:15:50.000000 domino-py-0.9.1/src/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-23 17:15:50.000000 domino-py-0.9.1/src/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-23 17:15:50.000000 domino-py-0.9.1/src/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-23 17:15:50.000000 domino-py-0.9.1/src/domino_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.299061 domino_py-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-19 19:05:27.000000 domino_py-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-19 19:05:41.299061 domino_py-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-19 19:05:27.000000 domino_py-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-19 19:05:27.000000 domino_py-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:05:41.303061 domino_py-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.283062 domino_py-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/actions/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/config-domino-local.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40723 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/github_rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.287062 domino_py-0.9.2/src/domino/client/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/legacy/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/legacy/s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/client/local_files_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/custom_operators/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/deprecated/base_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/deprecated/external_python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/docker_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26228 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/fuse.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/rclone.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/sidecar/sidecar_lifecycle.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/custom_operators/worker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/models/output_modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.291061 domino_py-0.9.2/src/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/deploy_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/display_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.295061 domino_py-0.9.2/src/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/build_docker_images_pieces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.295061 domino_py-0.9.2/src/domino/scripts/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/deprecated/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/deprecated/deprecated_piece_dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/deprecated/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/deprecated/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/deprecated/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/scripts/run_piece_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.295061 domino_py-0.9.2/src/domino/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/storage/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.295061 domino_py-0.9.2/src/domino/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/testing/dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/testing/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/testing/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.295061 domino_py-0.9.2/src/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/utils/piece_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 19:05:27.000000 domino_py-0.9.2/src/domino/utils/workflow_shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:05:41.299061 domino_py-0.9.2/src/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 19:05:41.000000 domino_py-0.9.2/src/domino_py.egg-info/top_level.txt
```

### Comparing `domino-py-0.9.1/LICENSE` & `domino_py-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/PKG-INFO` & `domino_py-0.9.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python package for Domino.
 Author-email: Luiz Tauffer <luiz@taufferconsulting.com>, Vinicius Vaz <vinicius@taufferconsulting.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -274,15 +274,15 @@
     <img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86">
   </a>
 </p>
 
 
 <br>
 
-![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/gif-example.gif)
+![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/intro/gif-example.gif)
 
 # Table of contents
 - [About](#about)
 - [Quick start](#quick-start)
 - [GUI](#gui)
 - [Pieces](#pieces)
 - [REST](#rest)
@@ -315,15 +315,15 @@
 - :wheel_of_dharma: scalable, Kubernetes-native platform
 - :battery: powered by Apache Airflow for top-tier workflows scheduling and monitoring
 
 <br>
 
 # Quick start
 
-Check out the quick start guide in the [documentation](https://domino-workflows.io/docs/quickstart).
+Check out the quick start guide in the [documentation](https://docs.domino-workflows.io/quickstart).
 
 The Domino Python package can be installed via pip. We reccommend you install Domino in a separate Python environment.
 
 ```bash
 pip install domino-py[cli]
 ```
 
@@ -332,88 +332,88 @@
 ```bash
 domino platform run-compose
 ```
 
 After all processes started successfully, navigate to `localhost:3000` to access the Domino frontend service. <br>
 Obs.: the first time you run the platform, it may take a few minutes to download the Docker images.
 
-Running the Domino platform locally with Docker compose is useful for development and testing purposes. For production environments, we recommend you deploy Domino and Airflow to a Kubernetes cluster. For other deployment modes, check out the instructions in the [documentation](https://domino-workflows.io/docs/category/run-domino).
+Running the Domino platform locally with Docker compose is useful for development and testing purposes. For production environments, we recommend you deploy Domino and Airflow to a Kubernetes cluster. For other deployment modes, check out the instructions in the [documentation](https://docs.domino-workflows.io/category/run-domino).
 
 <br>
 
 # GUI
-The Domino frontend service is a React application that provides the GUI for easily creating, editing and monitoring Workflows. Check out the [GUI documentation](https://domino-workflows.io/docs/domino_components/domino_components_gui) for more details.
+The Domino frontend service is a React application that provides the GUI for easily creating, editing and monitoring Workflows. Check out the [GUI documentation](https://docs.domino-workflows.io/domino_components/domino_components_gui) for more details.
 
 <details>
   <summary>
     <strong>Access authentication</strong>
   </summary>
   Sign up and login to use the Domino platform. <br></br>
 
-  ![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/1_sign_up.gif)
+  ![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/signin.gif)
 
 </details>
 
 <details>
   <summary>
-    <strong>Create Workspaces</strong>
+    <strong>Select or Create Workspaces</strong>
   </summary>
-  Create new Workspaces and add your github access token. <br></br>
+  Select an existing or create a new Workspace. <br></br>
 
-  ![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/2_create_workspace_and_token.gif)
+  ![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/select-workspace.png)
 
 </details>
 
 <details>
   <summary>
     <strong>Install Pieces repositories</strong>
   </summary>
   Install bundles of Pieces to your Domino Workspaces direclty from Github repositories, and use them in your Workflows. <br></br>
 
-  ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/6_install_pieces.gif)
+  ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/pieces/install_repository.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Create Workflows</strong>
   </summary>
   Create Workflows by dragging and dropping Pieces to the canvas, and connecting them. <br></br>
 
-  ![create-workflow](https://github.com/Tauffer-Consulting/domino/assets/54302847/34d619fa-4b6c-4761-8b24-3ca829cfc28c)
+  ![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/create_workflow.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Edit Pieces</strong>
   </summary>
   Edit Pieces by changing their input. Outputs from upstream Pieces are automatically available as inputs for downstream Pieces. Pieces can pass forward any type of data, from simple strings to heavy files, all automatically handled by Domino shared storage system. <br></br>
 
-  ![edit pieces](https://github.com/Tauffer-Consulting/domino/assets/54302847/d453ac81-5485-4159-b2f3-bf57eb969906)
+  ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/edit_pieces.gif)
 
 </details>
 
 <details>
   <summary>
-    <strong>Schedule Workflows</strong>
+    <strong>Configure Workflows</strong>
   </summary>
-  Schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
+  Configure and schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
 
-  ![schedule workflows](https://github.com/Tauffer-Consulting/domino/assets/54302847/e881d225-e8e0-4344-bc3f-c170cb820274)
+  ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/workflow_settings.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Monitor Workflows</strong>
   </summary>
   Monitor Workflows in real time, including the status of each Piece, the logs and results of each run. <br></br>
 
-  ![run-pieces7](https://github.com/Tauffer-Consulting/domino/assets/54302847/fb5a30c5-0314-4271-bb46-81a159ab2696)
+  ![run-pieces7](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/monitoring_workflow.gif)
 
 </details>
 
 <br>
 
 # Pieces
 Pieces are the secret sauce of Domino, they are functional units that can be distributed and reused in multiple Workflows. Domino Pieces are special because they:
@@ -430,25 +430,25 @@
 
 1. write your Python function as a Piece <br>
 2. define the data types, dependencies, metadata and tests <br>
 3. publish in a git repository (public or private)
 
 The [Pieces repository template](https://github.com/Tauffer-Consulting/domino_pieces_repository_template) provides the basic structure, example files and automatic actions for a seamless Pieces creation experience.
 
-Read more in the [Pieces documentation](https://domino-workflows.io/docs/pieces).
+Read more in the [Pieces documentation](https://docs.domino-workflows.io/pieces).
 
 
 <br>
 
 # REST
 The Backend service is a REST API that controls a running Apache Airflow instance. It is responsible for:
 
 - executing operations requested by the frontend service
 - interacting with the Airflow instance, including triggering, creating, editing and deleting Workflows (DAGs)
 - interacting with the Domino Database
 
-The REST service is written in Python, using the FastAPI framework. Read more about it in the [REST documentation](https://domino-py.readthedocs.io/en/latest/pages/rest.html).
+The REST service is written in Python, using the FastAPI framework. Read more about it in the [REST documentation](https://docs.domino-workflows.io/domino_components/domino_components_rest).
 
 <br>
 
 # Credits
 Domino is developed and maintained by [Tauffer Consulting](https://www.taufferconsulting.com/).
```

### Comparing `domino-py-0.9.1/README.md` & `domino_py-0.9.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     <img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86">
   </a>
 </p>
 
 
 <br>
 
-![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/gif-example.gif)
+![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/intro/gif-example.gif)
 
 # Table of contents
 - [About](#about)
 - [Quick start](#quick-start)
 - [GUI](#gui)
 - [Pieces](#pieces)
 - [REST](#rest)
@@ -63,15 +63,15 @@
 - :wheel_of_dharma: scalable, Kubernetes-native platform
 - :battery: powered by Apache Airflow for top-tier workflows scheduling and monitoring
 
 <br>
 
 # Quick start
 
-Check out the quick start guide in the [documentation](https://domino-workflows.io/docs/quickstart).
+Check out the quick start guide in the [documentation](https://docs.domino-workflows.io/quickstart).
 
 The Domino Python package can be installed via pip. We reccommend you install Domino in a separate Python environment.
 
 ```bash
 pip install domino-py[cli]
 ```
 
@@ -80,88 +80,88 @@
 ```bash
 domino platform run-compose
 ```
 
 After all processes started successfully, navigate to `localhost:3000` to access the Domino frontend service. <br>
 Obs.: the first time you run the platform, it may take a few minutes to download the Docker images.
 
-Running the Domino platform locally with Docker compose is useful for development and testing purposes. For production environments, we recommend you deploy Domino and Airflow to a Kubernetes cluster. For other deployment modes, check out the instructions in the [documentation](https://domino-workflows.io/docs/category/run-domino).
+Running the Domino platform locally with Docker compose is useful for development and testing purposes. For production environments, we recommend you deploy Domino and Airflow to a Kubernetes cluster. For other deployment modes, check out the instructions in the [documentation](https://docs.domino-workflows.io/category/run-domino).
 
 <br>
 
 # GUI
-The Domino frontend service is a React application that provides the GUI for easily creating, editing and monitoring Workflows. Check out the [GUI documentation](https://domino-workflows.io/docs/domino_components/domino_components_gui) for more details.
+The Domino frontend service is a React application that provides the GUI for easily creating, editing and monitoring Workflows. Check out the [GUI documentation](https://docs.domino-workflows.io/domino_components/domino_components_gui) for more details.
 
 <details>
   <summary>
     <strong>Access authentication</strong>
   </summary>
   Sign up and login to use the Domino platform. <br></br>
 
-  ![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/1_sign_up.gif)
+  ![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/signin.gif)
 
 </details>
 
 <details>
   <summary>
-    <strong>Create Workspaces</strong>
+    <strong>Select or Create Workspaces</strong>
   </summary>
-  Create new Workspaces and add your github access token. <br></br>
+  Select an existing or create a new Workspace. <br></br>
 
-  ![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/2_create_workspace_and_token.gif)
+  ![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/select-workspace.png)
 
 </details>
 
 <details>
   <summary>
     <strong>Install Pieces repositories</strong>
   </summary>
   Install bundles of Pieces to your Domino Workspaces direclty from Github repositories, and use them in your Workflows. <br></br>
 
-  ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/6_install_pieces.gif)
+  ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/pieces/install_repository.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Create Workflows</strong>
   </summary>
   Create Workflows by dragging and dropping Pieces to the canvas, and connecting them. <br></br>
 
-  ![create-workflow](https://github.com/Tauffer-Consulting/domino/assets/54302847/34d619fa-4b6c-4761-8b24-3ca829cfc28c)
+  ![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/create_workflow.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Edit Pieces</strong>
   </summary>
   Edit Pieces by changing their input. Outputs from upstream Pieces are automatically available as inputs for downstream Pieces. Pieces can pass forward any type of data, from simple strings to heavy files, all automatically handled by Domino shared storage system. <br></br>
 
-  ![edit pieces](https://github.com/Tauffer-Consulting/domino/assets/54302847/d453ac81-5485-4159-b2f3-bf57eb969906)
+  ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/edit_pieces.gif)
 
 </details>
 
 <details>
   <summary>
-    <strong>Schedule Workflows</strong>
+    <strong>Configure Workflows</strong>
   </summary>
-  Schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
+  Configure and schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
 
-  ![schedule workflows](https://github.com/Tauffer-Consulting/domino/assets/54302847/e881d225-e8e0-4344-bc3f-c170cb820274)
+  ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/workflow_settings.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Monitor Workflows</strong>
   </summary>
   Monitor Workflows in real time, including the status of each Piece, the logs and results of each run. <br></br>
 
-  ![run-pieces7](https://github.com/Tauffer-Consulting/domino/assets/54302847/fb5a30c5-0314-4271-bb46-81a159ab2696)
+  ![run-pieces7](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/monitoring_workflow.gif)
 
 </details>
 
 <br>
 
 # Pieces
 Pieces are the secret sauce of Domino, they are functional units that can be distributed and reused in multiple Workflows. Domino Pieces are special because they:
@@ -178,25 +178,25 @@
 
 1. write your Python function as a Piece <br>
 2. define the data types, dependencies, metadata and tests <br>
 3. publish in a git repository (public or private)
 
 The [Pieces repository template](https://github.com/Tauffer-Consulting/domino_pieces_repository_template) provides the basic structure, example files and automatic actions for a seamless Pieces creation experience.
 
-Read more in the [Pieces documentation](https://domino-workflows.io/docs/pieces).
+Read more in the [Pieces documentation](https://docs.domino-workflows.io/pieces).
 
 
 <br>
 
 # REST
 The Backend service is a REST API that controls a running Apache Airflow instance. It is responsible for:
 
 - executing operations requested by the frontend service
 - interacting with the Airflow instance, including triggering, creating, editing and deleting Workflows (DAGs)
 - interacting with the Domino Database
 
-The REST service is written in Python, using the FastAPI framework. Read more about it in the [REST documentation](https://domino-py.readthedocs.io/en/latest/pages/rest.html).
+The REST service is written in Python, using the FastAPI framework. Read more about it in the [REST documentation](https://docs.domino-workflows.io/domino_components/domino_components_rest).
 
 <br>
 
 # Credits
 Domino is developed and maintained by [Tauffer Consulting](https://www.taufferconsulting.com/).
```

#### html2text {}

```diff
@@ -3,18 +3,18 @@
                  _[_D_o_c_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_d_o_m_i_n_o_-
   _p_y_?_c_o_l_o_r_=_%_2_3_1_B_A_3_3_1_&_l_a_b_e_l_=_P_y_P_I_&_l_o_g_o_=_p_y_t_h_o_n_&_l_o_g_o_C_o_l_o_r_=_%_2_3_F_7_F_9_9_1_%_2_0_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/_a_r_t_i_f_a_c_t_h_u_b_._i_o_/_b_a_d_g_e_/_r_e_p_o_s_i_t_o_r_y_/_d_o_m_i_n_o_]
             _[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_T_a_u_f_f_e_r_-_C_o_n_s_u_l_t_i_n_g_/_d_o_m_i_n_o_/_g_r_a_p_h_/
         _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_W_T_J_P_H_7_F_S_N_J_]_[_D_O_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
         _v_1_?_l_a_b_e_l_=_S_p_o_n_s_o_r_&_m_e_s_s_a_g_e_=_%_E_2_%_9_D_%_A_4_&_l_o_g_o_=_G_i_t_H_u_b_&_c_o_l_o_r_=_%_2_3_f_e_8_e_8_6_]
 
-![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
-main/media/gif-example.gif) # Table of contents - [About](#about) - [Quick
-start](#quick-start) - [GUI](#gui) - [Pieces](#pieces) - [REST](#rest) -
-[Credits](#credits)
+![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino-
+docs/main/static/img/intro/gif-example.gif) # Table of contents - [About]
+(#about) - [Quick start](#quick-start) - [GUI](#gui) - [Pieces](#pieces) -
+[REST](#rest) - [Credits](#credits)
 # About **Domino is an open source workflow management platform**, with: - :
 desktop_computer: an intuitive [Graphical User Interface](#gui) that
 facilitates creating, editing and monitoring any type of Workflow, from data
 processing to machine learning - :package: a standard way of writing and
 publishing functional [Pieces](#pieces), which follows good practices for data
 modeling, documentation and distribution - :gear: a [REST API](#rest) that
 controls a running Apache Airflow instance Creating Workflows in the GUI is as
@@ -36,58 +36,59 @@
 chart_with_upwards_trend: experience a cleaner and more intuitive GUI for
 viewing Workflows results, including logs and richer reports with images and
 tables - :minidisc: shared storage for tasks in the same workflow - :
 arrows_counterclockwise: use gitSync to sync DAGs from files stored in a Git
 repository - :wheel_of_dharma: scalable, Kubernetes-native platform - :battery:
 powered by Apache Airflow for top-tier workflows scheduling and monitoring
 # Quick start Check out the quick start guide in the [documentation](https://
-domino-workflows.io/docs/quickstart). The Domino Python package can be
+docs.domino-workflows.io/quickstart). The Domino Python package can be
 installed via pip. We reccommend you install Domino in a separate Python
 environment. ```bash pip install domino-py[cli] ``` You can then use Domino
 command line interface to easily run the Domino platform locally (requires
 [Docker Compose V2](https://docs.docker.com/compose/)). Go to a new, empty
 directory and run the following command: ```bash domino platform run-compose
 ``` After all processes started successfully, navigate to `localhost:3000` to
 access the Domino frontend service.
 Obs.: the first time you run the platform, it may take a few minutes to
 download the Docker images. Running the Domino platform locally with Docker
 compose is useful for development and testing purposes. For production
 environments, we recommend you deploy Domino and Airflow to a Kubernetes
 cluster. For other deployment modes, check out the instructions in the
-[documentation](https://domino-workflows.io/docs/category/run-domino).
+[documentation](https://docs.domino-workflows.io/category/run-domino).
 # GUI The Domino frontend service is a React application that provides the GUI
 for easily creating, editing and monitoring Workflows. Check out the [GUI
-documentation](https://domino-workflows.io/docs/domino_components/
+documentation](https://docs.domino-workflows.io/domino_components/
 domino_components_gui) for more details. AAcccceessss aauutthheennttiiccaattiioonn Sign up and
 login to use the Domino platform.
 ![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/
-domino/main/docs/source/_static/media/1_sign_up.gif) CCrreeaattee WWoorrkkssppaacceess Create
-new Workspaces and add your github access token.
+domino-docs/main/static/img/quickstart/signin.gif) SSeelleecctt oorr CCrreeaattee WWoorrkkssppaacceess
+Select an existing or create a new Workspace.
 ![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/
-domino/main/docs/source/_static/media/2_create_workspace_and_token.gif) IInnssttaallll
-PPiieecceess rreeppoossiittoorriieess Install bundles of Pieces to your Domino Workspaces
-direclty from Github repositories, and use them in your Workflows.
-![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
-main/docs/source/_static/media/6_install_pieces.gif) CCrreeaattee WWoorrkkfflloowwss Create
+domino-docs/main/static/img/quickstart/select-workspace.png) IInnssttaallll PPiieecceess
+rreeppoossiittoorriieess Install bundles of Pieces to your Domino Workspaces direclty from
+Github repositories, and use them in your Workflows.
+![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino-
+docs/main/static/img/pieces/install_repository.gif) CCrreeaattee WWoorrkkfflloowwss Create
 Workflows by dragging and dropping Pieces to the canvas, and connecting them.
-![create-workflow](https://github.com/Tauffer-Consulting/domino/assets/
-54302847/34d619fa-4b6c-4761-8b24-3ca829cfc28c) EEddiitt PPiieecceess Edit Pieces by
+![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino-
+docs/main/static/img/quickstart/create_workflow.gif) EEddiitt PPiieecceess Edit Pieces by
 changing their input. Outputs from upstream Pieces are automatically available
 as inputs for downstream Pieces. Pieces can pass forward any type of data, from
 simple strings to heavy files, all automatically handled by Domino shared
 storage system.
-![edit pieces](https://github.com/Tauffer-Consulting/domino/assets/54302847/
-d453ac81-5485-4159-b2f3-bf57eb969906) SScchheedduullee WWoorrkkfflloowwss Schedule Workflows to
-run periodically, at a specific date/time, or trigger them manually.
-![schedule workflows](https://github.com/Tauffer-Consulting/domino/assets/
-54302847/e881d225-e8e0-4344-bc3f-c170cb820274) MMoonniittoorr WWoorrkkfflloowwss Monitor
-Workflows in real time, including the status of each Piece, the logs and
-results of each run.
-![run-pieces7](https://github.com/Tauffer-Consulting/domino/assets/54302847/
-fb5a30c5-0314-4271-bb46-81a159ab2696)
+![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino-
+docs/main/static/img/quickstart/edit_pieces.gif) CCoonnffiigguurree WWoorrkkfflloowwss Configure
+and schedule Workflows to run periodically, at a specific date/time, or trigger
+them manually.
+![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino-docs/main/static/img/quickstart/workflow_settings.gif) MMoonniittoorr WWoorrkkfflloowwss
+Monitor Workflows in real time, including the status of each Piece, the logs
+and results of each run.
+![run-pieces7](https://raw.githubusercontent.com/Tauffer-Consulting/domino-
+docs/main/static/img/quickstart/monitoring_workflow.gif)
 # Pieces Pieces are the secret sauce of Domino, they are functional units that
 can be distributed and reused in multiple Workflows. Domino Pieces are special
 because they: - :snake: can execute anything written in Python, heavy-weight
 (e.g. Machine Learning) as well as light-weight (e.g. sending emails) tasks - :
 traffic_light: have well defined data models for inputs, outputs and secrets -
 :package: run in self-contained and isolated execution environments (Docker
 containers) - :gear: are immutable, guaranteeing reproducibility of your
@@ -97,17 +98,17 @@
 incorporated in any workflow It is very easy to create and share your own
 Pieces: 1. write your Python function as a Piece
 2. define the data types, dependencies, metadata and tests
 3. publish in a git repository (public or private) The [Pieces repository
 template](https://github.com/Tauffer-Consulting/
 domino_pieces_repository_template) provides the basic structure, example files
 and automatic actions for a seamless Pieces creation experience. Read more in
-the [Pieces documentation](https://domino-workflows.io/docs/pieces).
+the [Pieces documentation](https://docs.domino-workflows.io/pieces).
 # REST The Backend service is a REST API that controls a running Apache Airflow
 instance. It is responsible for: - executing operations requested by the
 frontend service - interacting with the Airflow instance, including triggering,
 creating, editing and deleting Workflows (DAGs) - interacting with the Domino
 Database The REST service is written in Python, using the FastAPI framework.
-Read more about it in the [REST documentation](https://domino-
-py.readthedocs.io/en/latest/pages/rest.html).
+Read more about it in the [REST documentation](https://docs.domino-
+workflows.io/domino_components/domino_components_rest).
 # Credits Domino is developed and maintained by [Tauffer Consulting](https://
 www.taufferconsulting.com/).
```

### Comparing `domino-py-0.9.1/pyproject.toml` & `domino_py-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/actions/github_actions.py` & `domino_py-0.9.2/src/domino/actions/github_actions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/base_piece.py` & `domino_py-0.9.2/src/domino/base_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/cli/cli.py` & `domino_py-0.9.2/src/domino/cli/cli.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/cli/utils/config-domino-local.toml` & `domino_py-0.9.2/src/domino/cli/utils/config-domino-local.toml`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/cli/utils/docker-compose.yaml` & `domino_py-0.9.2/src/domino/cli/utils/docker-compose.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
         condition: service_started
     environment:
       - DOMINO_DEPLOY_MODE=local-compose
       - API_URL=http://localhost:8000
 
   # Domino Docker proxy
   docker-proxy:
-    image: bobrik/socat
+    image: alpine/socat
     container_name: domino-docker-proxy
     command: "TCP4-LISTEN:2375,fork,reuseaddr UNIX-CONNECT:/var/run/docker.sock"
     ports:
       - "2376:2375"
     volumes:
       - /var/run/docker.sock:/var/run/docker.sock
```

### Comparing `domino-py-0.9.1/src/domino/cli/utils/pieces_repository.py` & `domino_py-0.9.2/src/domino/cli/utils/pieces_repository.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/cli/utils/platform.py` & `domino_py-0.9.2/src/domino/cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/client/domino_backend_client.py` & `domino_py-0.9.2/src/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/client/github_rest_client.py` & `domino_py-0.9.2/src/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/client/legacy/fs_client.py` & `domino_py-0.9.2/src/domino/client/legacy/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/client/legacy/s3_client.py` & `domino_py-0.9.2/src/domino/client/legacy/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/client/local_files_client.py` & `domino_py-0.9.2/src/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/custom_operators/deprecated/base_operator.py` & `domino_py-0.9.2/src/domino/custom_operators/deprecated/base_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/custom_operators/deprecated/external_python_operator.py` & `domino_py-0.9.2/src/domino/custom_operators/deprecated/external_python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/custom_operators/docker_operator.py` & `domino_py-0.9.2/src/domino/custom_operators/docker_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/custom_operators/k8s_operator.py` & `domino_py-0.9.2/src/domino/custom_operators/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/custom_operators/python_operator.py` & `domino_py-0.9.2/src/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/custom_operators/sidecar/logger.py` & `domino_py-0.9.2/src/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/custom_operators/sidecar/mount.py` & `domino_py-0.9.2/src/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/custom_operators/worker_operator.py` & `domino_py-0.9.2/src/domino/custom_operators/worker_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/exceptions/exceptions.py` & `domino_py-0.9.2/src/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/logger.py` & `domino_py-0.9.2/src/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/models/output_modifier.py` & `domino_py-0.9.2/src/domino/models/output_modifier.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/schemas/piece_metadata.py` & `domino_py-0.9.2/src/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/schemas/shared_storage.py` & `domino_py-0.9.2/src/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/scripts/build_docker_images_pieces.py` & `domino_py-0.9.2/src/domino/scripts/build_docker_images_pieces.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/scripts/deprecated/create_docker_compose_file.py` & `domino_py-0.9.2/src/domino/scripts/deprecated/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/scripts/deprecated/deprecated_piece_dry_run.py` & `domino_py-0.9.2/src/domino/scripts/deprecated/deprecated_piece_dry_run.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/scripts/deprecated/docker_compose_constants.py` & `domino_py-0.9.2/src/domino/scripts/deprecated/docker_compose_constants.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/scripts/deprecated/docker_compose_scripts.py` & `domino_py-0.9.2/src/domino/scripts/deprecated/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/scripts/deprecated/run_piece_bash.py` & `domino_py-0.9.2/src/domino/scripts/deprecated/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/scripts/load_piece.py` & `domino_py-0.9.2/src/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/scripts/run_piece_docker.py` & `domino_py-0.9.2/src/domino/scripts/run_piece_docker.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/storage/s3.py` & `domino_py-0.9.2/src/domino/storage/s3.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/task.py` & `domino_py-0.9.2/src/domino/task.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/testing/dry_run.py` & `domino_py-0.9.2/src/domino/testing/dry_run.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/testing/http_client.py` & `domino_py-0.9.2/src/domino/testing/http_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino/utils/piece_generator.py` & `domino_py-0.9.2/src/domino/utils/piece_generator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino_py.egg-info/PKG-INFO` & `domino_py-0.9.2/src/domino_py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python package for Domino.
 Author-email: Luiz Tauffer <luiz@taufferconsulting.com>, Vinicius Vaz <vinicius@taufferconsulting.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -274,15 +274,15 @@
     <img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86">
   </a>
 </p>
 
 
 <br>
 
-![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/gif-example.gif)
+![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/intro/gif-example.gif)
 
 # Table of contents
 - [About](#about)
 - [Quick start](#quick-start)
 - [GUI](#gui)
 - [Pieces](#pieces)
 - [REST](#rest)
@@ -315,15 +315,15 @@
 - :wheel_of_dharma: scalable, Kubernetes-native platform
 - :battery: powered by Apache Airflow for top-tier workflows scheduling and monitoring
 
 <br>
 
 # Quick start
 
-Check out the quick start guide in the [documentation](https://domino-workflows.io/docs/quickstart).
+Check out the quick start guide in the [documentation](https://docs.domino-workflows.io/quickstart).
 
 The Domino Python package can be installed via pip. We reccommend you install Domino in a separate Python environment.
 
 ```bash
 pip install domino-py[cli]
 ```
 
@@ -332,88 +332,88 @@
 ```bash
 domino platform run-compose
 ```
 
 After all processes started successfully, navigate to `localhost:3000` to access the Domino frontend service. <br>
 Obs.: the first time you run the platform, it may take a few minutes to download the Docker images.
 
-Running the Domino platform locally with Docker compose is useful for development and testing purposes. For production environments, we recommend you deploy Domino and Airflow to a Kubernetes cluster. For other deployment modes, check out the instructions in the [documentation](https://domino-workflows.io/docs/category/run-domino).
+Running the Domino platform locally with Docker compose is useful for development and testing purposes. For production environments, we recommend you deploy Domino and Airflow to a Kubernetes cluster. For other deployment modes, check out the instructions in the [documentation](https://docs.domino-workflows.io/category/run-domino).
 
 <br>
 
 # GUI
-The Domino frontend service is a React application that provides the GUI for easily creating, editing and monitoring Workflows. Check out the [GUI documentation](https://domino-workflows.io/docs/domino_components/domino_components_gui) for more details.
+The Domino frontend service is a React application that provides the GUI for easily creating, editing and monitoring Workflows. Check out the [GUI documentation](https://docs.domino-workflows.io/domino_components/domino_components_gui) for more details.
 
 <details>
   <summary>
     <strong>Access authentication</strong>
   </summary>
   Sign up and login to use the Domino platform. <br></br>
 
-  ![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/1_sign_up.gif)
+  ![signup and login](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/signin.gif)
 
 </details>
 
 <details>
   <summary>
-    <strong>Create Workspaces</strong>
+    <strong>Select or Create Workspaces</strong>
   </summary>
-  Create new Workspaces and add your github access token. <br></br>
+  Select an existing or create a new Workspace. <br></br>
 
-  ![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/2_create_workspace_and_token.gif)
+  ![create workspace](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/select-workspace.png)
 
 </details>
 
 <details>
   <summary>
     <strong>Install Pieces repositories</strong>
   </summary>
   Install bundles of Pieces to your Domino Workspaces direclty from Github repositories, and use them in your Workflows. <br></br>
 
-  ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/6_install_pieces.gif)
+  ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/pieces/install_repository.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Create Workflows</strong>
   </summary>
   Create Workflows by dragging and dropping Pieces to the canvas, and connecting them. <br></br>
 
-  ![create-workflow](https://github.com/Tauffer-Consulting/domino/assets/54302847/34d619fa-4b6c-4761-8b24-3ca829cfc28c)
+  ![create-workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/create_workflow.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Edit Pieces</strong>
   </summary>
   Edit Pieces by changing their input. Outputs from upstream Pieces are automatically available as inputs for downstream Pieces. Pieces can pass forward any type of data, from simple strings to heavy files, all automatically handled by Domino shared storage system. <br></br>
 
-  ![edit pieces](https://github.com/Tauffer-Consulting/domino/assets/54302847/d453ac81-5485-4159-b2f3-bf57eb969906)
+  ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/edit_pieces.gif)
 
 </details>
 
 <details>
   <summary>
-    <strong>Schedule Workflows</strong>
+    <strong>Configure Workflows</strong>
   </summary>
-  Schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
+  Configure and schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
 
-  ![schedule workflows](https://github.com/Tauffer-Consulting/domino/assets/54302847/e881d225-e8e0-4344-bc3f-c170cb820274)
+  ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/workflow_settings.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Monitor Workflows</strong>
   </summary>
   Monitor Workflows in real time, including the status of each Piece, the logs and results of each run. <br></br>
 
-  ![run-pieces7](https://github.com/Tauffer-Consulting/domino/assets/54302847/fb5a30c5-0314-4271-bb46-81a159ab2696)
+  ![run-pieces7](https://raw.githubusercontent.com/Tauffer-Consulting/domino-docs/main/static/img/quickstart/monitoring_workflow.gif)
 
 </details>
 
 <br>
 
 # Pieces
 Pieces are the secret sauce of Domino, they are functional units that can be distributed and reused in multiple Workflows. Domino Pieces are special because they:
@@ -430,25 +430,25 @@
 
 1. write your Python function as a Piece <br>
 2. define the data types, dependencies, metadata and tests <br>
 3. publish in a git repository (public or private)
 
 The [Pieces repository template](https://github.com/Tauffer-Consulting/domino_pieces_repository_template) provides the basic structure, example files and automatic actions for a seamless Pieces creation experience.
 
-Read more in the [Pieces documentation](https://domino-workflows.io/docs/pieces).
+Read more in the [Pieces documentation](https://docs.domino-workflows.io/pieces).
 
 
 <br>
 
 # REST
 The Backend service is a REST API that controls a running Apache Airflow instance. It is responsible for:
 
 - executing operations requested by the frontend service
 - interacting with the Airflow instance, including triggering, creating, editing and deleting Workflows (DAGs)
 - interacting with the Domino Database
 
-The REST service is written in Python, using the FastAPI framework. Read more about it in the [REST documentation](https://domino-py.readthedocs.io/en/latest/pages/rest.html).
+The REST service is written in Python, using the FastAPI framework. Read more about it in the [REST documentation](https://docs.domino-workflows.io/domino_components/domino_components_rest).
 
 <br>
 
 # Credits
 Domino is developed and maintained by [Tauffer Consulting](https://www.taufferconsulting.com/).
```

### Comparing `domino-py-0.9.1/src/domino_py.egg-info/SOURCES.txt` & `domino_py-0.9.2/src/domino_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domino-py-0.9.1/src/domino_py.egg-info/requires.txt` & `domino_py-0.9.2/src/domino_py.egg-info/requires.txt`

 * *Files identical despite different names*

