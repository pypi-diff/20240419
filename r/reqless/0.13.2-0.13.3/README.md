# Comparing `tmp/reqless-0.13.2.tar.gz` & `tmp/reqless-0.13.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reqless-0.13.2.tar", last modified: Tue Apr  9 17:25:42 2024, max compression
+gzip compressed data, was "reqless-0.13.3.tar", last modified: Fri Apr 19 14:19:01 2024, max compression
```

## Comparing `reqless-0.13.2.tar` & `reqless-0.13.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.596715 reqless-0.13.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.576715 reqless-0.13.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.580715 reqless-0.13.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-09 17:24:38.000000 reqless-0.13.2/.github/workflows/main-branch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-09 17:24:38.000000 reqless-0.13.2/.github/workflows/other-branch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-09 17:24:38.000000 reqless-0.13.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 17:24:38.000000 reqless-0.13.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 17:24:38.000000 reqless-0.13.2/.gitmodules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.576715 reqless-0.13.2/.meta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.580715 reqless-0.13.2/.meta/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-09 17:25:39.000000 reqless-0.13.2/.meta/coverage/badge.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-09 17:25:39.000000 reqless-0.13.2/.meta/coverage/report.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-09 17:24:38.000000 reqless-0.13.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 17:24:38.000000 reqless-0.13.2/.safety-policy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 17:24:38.000000 reqless-0.13.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 17:24:38.000000 reqless-0.13.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-04-09 17:25:42.596715 reqless-0.13.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-04-09 17:24:38.000000 reqless-0.13.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 17:24:38.000000 reqless-0.13.2/Vagrantfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.580715 reqless-0.13.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3376 2024-04-09 17:24:38.000000 reqless-0.13.2/bin/reqless-py-worker
--rwxr-xr-x   0 runner    (1001) docker     (127)     5194 2024-04-09 17:24:38.000000 reqless-0.13.2/forgetful-bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-09 17:24:38.000000 reqless-0.13.2/provision.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-09 17:24:38.000000 reqless-0.13.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.580715 reqless-0.13.2/reqless/
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.584715 reqless-0.13.2/reqless/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_job_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_job_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_queue_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_queues.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_throttles.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16499 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.584715 reqless-0.13.2/reqless/lua/
--rw-r--r--   0 runner    (1001) docker     (127)    97685 2024-04-09 17:25:33.000000 reqless-0.13.2/reqless/lua/qless-lib.lua
--rw-r--r--   0 runner    (1001) docker     (127)    71833 2024-04-09 17:25:33.000000 reqless-0.13.2/reqless/lua/qless.lua
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/proctitle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.588715 reqless-0.13.2/reqless/qmore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/qmore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/qmore/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.588715 reqless-0.13.2/reqless/queue_resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/queue_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/queue_resolvers/transforming_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.588715 reqless-0.13.2/reqless/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/forking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/greenlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.592715 reqless-0.13.2/reqless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.592715 reqless-0.13.2/reqless_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/common.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_forking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_greenlet.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_job_processor_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_qmore_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14394 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15107 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_transforming_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_worker_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-09 17:25:15.000000 reqless-0.13.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:25:42.596715 reqless-0.13.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-09 17:24:38.000000 reqless-0.13.2/whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.253136 reqless-0.13.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.233136 reqless-0.13.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.237136 reqless-0.13.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-19 14:17:58.000000 reqless-0.13.3/.github/workflows/main-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-19 14:17:58.000000 reqless-0.13.3/.github/workflows/other-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-19 14:17:58.000000 reqless-0.13.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-19 14:17:58.000000 reqless-0.13.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 14:17:58.000000 reqless-0.13.3/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.233136 reqless-0.13.3/.meta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.237136 reqless-0.13.3/.meta/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-19 14:18:58.000000 reqless-0.13.3/.meta/coverage/badge.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-19 14:18:57.000000 reqless-0.13.3/.meta/coverage/report.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-19 14:17:58.000000 reqless-0.13.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 14:17:58.000000 reqless-0.13.3/.safety-policy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-19 14:17:58.000000 reqless-0.13.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 14:17:58.000000 reqless-0.13.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-04-19 14:19:01.253136 reqless-0.13.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-04-19 14:17:58.000000 reqless-0.13.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-19 14:17:58.000000 reqless-0.13.3/Vagrantfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.237136 reqless-0.13.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3376 2024-04-19 14:17:58.000000 reqless-0.13.3/bin/reqless-py-worker
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5194 2024-04-19 14:17:58.000000 reqless-0.13.3/forgetful-bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 14:17:58.000000 reqless-0.13.3/provision.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-19 14:17:58.000000 reqless-0.13.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.241136 reqless-0.13.3/reqless/
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.245136 reqless-0.13.3/reqless/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_job_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_queue_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_throttles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16598 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.245136 reqless-0.13.3/reqless/lua/
+-rw-r--r--   0 runner    (1001) docker     (127)    98606 2024-04-19 14:18:51.000000 reqless-0.13.3/reqless/lua/qless-lib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    72558 2024-04-19 14:18:51.000000 reqless-0.13.3/reqless/lua/qless.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/proctitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.245136 reqless-0.13.3/reqless/qmore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/qmore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/qmore/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.245136 reqless-0.13.3/reqless/queue_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/queue_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/queue_resolvers/transforming_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.249136 reqless-0.13.3/reqless/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/forking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/greenlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.253136 reqless-0.13.3/reqless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.249136 reqless-0.13.3/reqless_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_forking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_greenlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_job_processor_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_qmore_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14394 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15107 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_transforming_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_worker_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-19 14:18:33.000000 reqless-0.13.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:19:01.253136 reqless-0.13.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 14:17:58.000000 reqless-0.13.3/whitelist.txt
```

### Comparing `reqless-0.13.2/.github/workflows/main-branch.yaml` & `reqless-0.13.3/.github/workflows/main-branch.yaml`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/.github/workflows/other-branch.yaml` & `reqless-0.13.3/.github/workflows/other-branch.yaml`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/.github/workflows/release.yaml` & `reqless-0.13.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/.meta/coverage/badge.svg` & `reqless-0.13.3/.meta/coverage/badge.svg`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/.meta/coverage/report.txt` & `reqless-0.13.3/.meta/coverage/report.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 reqless/importer.py                                                                  26      0   100%
 reqless/job.py                                                                      280     15    95%
 reqless/listener.py                                                                  49      0   100%
 reqless/logger.py                                                                    13      0   100%
 reqless/proctitle.py                                                                  3      0   100%
 reqless/qmore/__init__.py                                                             0      0   100%
 reqless/qmore/client.py                                                              42      1    98%
-reqless/queue.py                                                                     89      0   100%
+reqless/queue.py                                                                     91      0   100%
 reqless/queue_resolvers/__init__.py                                                   4      0   100%
 reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py       50      0   100%
 reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py      61      0   100%
 reqless/queue_resolvers/transforming_queue_resolver.py                               13      0   100%
 reqless/throttle.py                                                                  29      0   100%
 reqless/util.py                                                                       7      0   100%
 reqless/workers/__init__.py                                                           2      0   100%
 reqless/workers/forking.py                                                           55      2    96%
 reqless/workers/greenlet.py                                                          50      0   100%
 reqless/workers/serial.py                                                            29      0   100%
 reqless/workers/util.py                                                              39      1    97%
 reqless/workers/worker.py                                                            78      3    96%
 -----------------------------------------------------------------------------------------------------
-TOTAL                                                                              1338     24    98%
+TOTAL                                                                              1340     24    98%
```

### Comparing `reqless-0.13.2/.pre-commit-config.yaml` & `reqless-0.13.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/LICENSE` & `reqless-0.13.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/Makefile` & `reqless-0.13.3/Makefile`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/PKG-INFO` & `reqless-0.13.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reqless
-Version: 0.13.2
+Version: 0.13.3
 Summary: Redis-based Queue Management
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/reqless-py
 Project-URL: Source, https://github.com/tdg5/reqless-py
 Project-URL: Tracker, https://github.com/tdg5/reqless-py/issues
 Keywords: job,qless,qmore,redis,reqless
@@ -20,15 +20,15 @@
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: decorator
 Requires-Dist: hiredis
 Requires-Dist: redis
 Requires-Dist: typing_extensions>=4.8.0
 Provides-Extra: dev
-Requires-Dist: black~=24.2.0; extra == "dev"
+Requires-Dist: black~=24.3; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
 Requires-Dist: flake8-pyproject~=1.2.3; extra == "dev"
 Requires-Dist: flake8~=7.0.0; extra == "dev"
 Requires-Dist: gevent~=24.2.1; extra == "dev"
 Requires-Dist: isort~=5.8.0; extra == "dev"
 Requires-Dist: mypy~=1.8.0; extra == "dev"
 Requires-Dist: pre-commit~=2.20.0; extra == "dev"
```

### Comparing `reqless-0.13.2/README.md` & `reqless-0.13.3/README.md`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/bin/reqless-py-worker` & `reqless-0.13.3/bin/reqless-py-worker`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/forgetful-bench.py` & `reqless-0.13.3/forgetful-bench.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/provision.sh` & `reqless-0.13.3/provision.sh`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/pyproject.toml` & `reqless-0.13.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 license = {text = "MIT"}
 name = "reqless"
 readme = "README.md"
 requires-python = ">3.9.0"
 
 [project.optional-dependencies]
 dev = [
-  "black~=24.2.0",
+  "black~=24.3",
   "build~=1.0.3",
   "flake8-pyproject~=1.2.3",
   "flake8~=7.0.0",
   "gevent~=24.2.1",
   "isort~=5.8.0",
   "mypy~=1.8.0",
   "pre-commit~=2.20.0",
```

### Comparing `reqless-0.13.2/reqless/__init__.py` & `reqless-0.13.3/reqless/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/abstract/__init__.py` & `reqless-0.13.3/reqless/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/abstract/abstract_client.py` & `reqless-0.13.3/reqless/abstract/abstract_client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/abstract/abstract_config.py` & `reqless-0.13.3/reqless/abstract/abstract_config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/abstract/abstract_job.py` & `reqless-0.13.3/reqless/abstract/abstract_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         pass
 
 
 class AbstractJob(AbstractBaseJob):
     @abstractmethod
     def complete(
         self,
-        nextq: Optional[str] = None,
+        next_queue: Optional[str] = None,
         delay: Optional[int] = None,
         depends: Optional[List[str]] = None,
     ) -> bool:  # pragma: no cover
         pass
 
     @property
     @abstractmethod
```

### Comparing `reqless-0.13.2/reqless/abstract/abstract_job_processor.py` & `reqless-0.13.3/reqless/abstract/abstract_job_processor.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/abstract/abstract_jobs.py` & `reqless-0.13.3/reqless/abstract/abstract_jobs.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/abstract/abstract_queue.py` & `reqless-0.13.3/reqless/abstract/abstract_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     @abstractmethod
     def pause(self) -> None:  # pragma: no cover
         pass
 
     @abstractmethod
     def peek(
-        self, count: Optional[int] = None
+        self, offset: Optional[int] = None, count: Optional[int] = None
     ) -> Union[AbstractJob, List[AbstractJob], None]:  # pragma: no cover
         pass
 
     @abstractmethod
     def pop(
         self, count: Optional[int] = None
     ) -> Union[AbstractJob, List[AbstractJob], None]:  # pragma: no cover
```

### Comparing `reqless-0.13.2/reqless/abstract/abstract_queue_jobs.py` & `reqless-0.13.3/reqless/abstract/abstract_queue_jobs.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/abstract/abstract_throttle.py` & `reqless-0.13.3/reqless/abstract/abstract_throttle.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/config.py` & `reqless-0.13.3/reqless/config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/importer.py` & `reqless-0.13.3/reqless/importer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/job.py` & `reqless-0.13.3/reqless/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -294,32 +294,37 @@
             "throttles",
             json.dumps(self.throttles or []),
         )
         return response
 
     def complete(
         self,
-        nextq: Optional[str] = None,
+        next_queue: Optional[str] = None,
         delay: Optional[int] = None,
         depends: Optional[List[str]] = None,
     ) -> bool:
         """Turn this job in as complete, optionally advancing it to another
         queue. Like ``Queue.put`` and ``move``, it accepts a delay, and
         dependencies"""
-        if nextq:
-            logger.info("Advancing %s to %s from %s", self.jid, nextq, self.queue_name)
+        if next_queue:
+            logger.info(
+                "Advancing %s to %s from %s",
+                self.jid,
+                next_queue,
+                self.queue_name,
+            )
             return (
                 self.client(
                     "complete",
                     self.jid,
                     self.client.worker_name,
                     self.queue_name,
                     self.data,
                     "next",
-                    nextq,
+                    next_queue,
                     "delay",
                     delay or 0,
                     "depends",
                     json.dumps(depends or []),
                 )
                 or False
             )
```

### Comparing `reqless-0.13.2/reqless/listener.py` & `reqless-0.13.3/reqless/listener.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/lua/qless-lib.lua` & `reqless-0.13.3/reqless/lua/qless-lib.lua`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
--- Current SHA: 09dc4ef4bb3cf089ef285d0a92a51b9af398ca03
+-- Current SHA: 62857f66dee92b76fc8b0e12ca6d588feba2d225
 -- This is a generated file
 -------------------------------------------------------------------------------
 -- Forward declarations to make everything happy
 -------------------------------------------------------------------------------
 local Qless = {
   ns = 'ql:'
 }
@@ -36,15 +36,15 @@
 QlessRecurringJob.__index = QlessRecurringJob
 
 -- Config forward declaration
 Qless.config = {}
 
 -- Extend a table. This comes up quite frequently
 local function table_extend(self, other)
-  for i, v in ipairs(other) do
+  for _, v in ipairs(other) do
     table.insert(self, v)
   end
 end
 
 -- This is essentially the same as redis' publish, but it prefixes the channel
 -- with the Qless namespace
 function Qless.publish(channel, message)
@@ -159,15 +159,15 @@
       total = redis.call('llen', 'ql:f:' .. group),
       jobs  = redis.call('lrange', 'ql:f:' .. group, start, start + limit - 1)
     }
   else
     -- Otherwise, we should just list all the known failure groups we have
     local response = {}
     local groups = redis.call('smembers', 'ql:failures')
-    for index, group in ipairs(groups) do
+    for _, group in ipairs(groups) do
       response[group] = redis.call('llen', 'ql:f:' .. group)
     end
     return response
   end
 end
 
 -- Jobs(now, 'complete', [offset, [count]])
@@ -257,18 +257,18 @@
       return redis.call('zrem', 'ql:tracked', jid)
     else
       error('Track(): Unknown action "' .. command .. '"')
     end
   else
     local response = {
       jobs = {},
-      expired = {}
+      expired = {},
     }
     local jids = redis.call('zrange', 'ql:tracked', 0, -1)
-    for index, jid in ipairs(jids) do
+    for _, jid in ipairs(jids) do
       local data = Qless.job(jid):data()
       if data then
         table.insert(response.jobs, data)
       else
         table.insert(response.expired, jid)
       end
     end
@@ -307,18 +307,18 @@
     local jid  = assert(arg[1], 'Tag(): Arg "jid" missing')
     local tags = redis.call('hget', QlessJob.ns .. jid, 'tags')
     -- If the job has been canceled / deleted, then return false
     if tags then
       -- Decode the json blob, convert to dictionary
       tags = cjson.decode(tags)
       local _tags = {}
-      for i,v in ipairs(tags) do _tags[v] = true end
+      for _, v in ipairs(tags) do _tags[v] = true end
 
       -- Otherwise, add the job to the sorted set with that tags
-      for i=2,#arg do
+      for i=2, #arg do
         local tag = arg[i]
         if _tags[tag] == nil then
           _tags[tag] = true
           table.insert(tags, tag)
         end
         Qless.job(jid):insert_tag(now, tag)
       end
@@ -332,25 +332,29 @@
     local jid  = assert(arg[1], 'Tag(): Arg "jid" missing')
     local tags = redis.call('hget', QlessJob.ns .. jid, 'tags')
     -- If the job has been canceled / deleted, then return false
     if tags then
       -- Decode the json blob, convert to dictionary
       tags = cjson.decode(tags)
       local _tags = {}
-      for i,v in ipairs(tags) do _tags[v] = true end
+      for _, v in ipairs(tags) do _tags[v] = true end
 
       -- Otherwise, remove the job from the sorted set with that tags
-      for i=2,#arg do
+      for i=2, #arg do
         local tag = arg[i]
         _tags[tag] = nil
         Qless.job(jid):remove_tag(tag)
       end
 
       local results = {}
-      for i,tag in ipairs(tags) do if _tags[tag] then table.insert(results, tag) end end
+      for _, tag in ipairs(tags) do
+        if _tags[tag] then
+          table.insert(results, tag)
+        end
+      end
 
       redis.call('hset', QlessJob.ns .. jid, 'tags', cjson.encode(results))
       return results
     else
       error('Tag(): Job ' .. jid .. ' does not exist')
     end
   elseif command == 'get' then
@@ -383,15 +387,15 @@
   for _, jid in ipairs(arg) do
     dependents[jid] = redis.call(
       'smembers', QlessJob.ns .. jid .. '-dependents') or {}
   end
 
   -- Now, we'll loop through every jid we intend to cancel, and we'll go
   -- make sure that this operation will be ok
-  for i, jid in ipairs(arg) do
+  for _, jid in ipairs(arg) do
     for j, dep in ipairs(dependents[jid]) do
       if dependents[dep] == nil then
         error('Cancel(): ' .. jid .. ' is a dependency of ' .. dep ..
            ' but is not mentioned to be canceled')
       end
     end
   end
@@ -428,15 +432,15 @@
 
       local job = Qless.job(jid)
 
       job:throttles_release(now)
 
       -- We should probably go through all our dependencies and remove
       -- ourselves from the list of dependents
-      for i, j in ipairs(redis.call(
+      for _, j in ipairs(redis.call(
         'smembers', QlessJob.ns .. jid .. '-dependencies')) do
         redis.call('srem', QlessJob.ns .. j .. '-dependents', jid)
       end
 
       -- If we're in the failed state, remove all of our data
       if state == 'failed' then
         failure = cjson.decode(failure)
@@ -538,42 +542,39 @@
 
   -- Return nil if we haven't found it
   if not job[1] then
     return nil
   end
 
   local data = {
-    jid              = job[1],
-    klass            = job[2],
-    state            = job[3],
-    queue            = job[4],
-    worker           = job[5] or '',
-    tracked          = redis.call(
-      'zscore', 'ql:tracked', self.jid) ~= false,
-    priority     = tonumber(job[6]),
-    expires      = tonumber(job[7]) or 0,
-    retries      = tonumber(job[8]),
-    remaining    = math.floor(tonumber(job[9])),
-    data         = job[10],
-    tags         = cjson.decode(job[11]),
-    history      = self:history(),
-    failure      = cjson.decode(job[12] or '{}'),
-    throttles    = cjson.decode(job[13] or '[]'),
+    jid = job[1],
+    klass = job[2],
+    state = job[3],
+    queue = job[4],
+    worker = job[5] or '',
+    tracked = redis.call('zscore', 'ql:tracked', self.jid) ~= false,
+    priority = tonumber(job[6]),
+    expires = tonumber(job[7]) or 0,
+    retries = tonumber(job[8]),
+    remaining = math.floor(tonumber(job[9])),
+    data = job[10],
+    tags = cjson.decode(job[11]),
+    history = self:history(),
+    failure = cjson.decode(job[12] or '{}'),
+    throttles = cjson.decode(job[13] or '[]'),
     spawned_from_jid = job[14],
-    dependents   = redis.call(
-      'smembers', QlessJob.ns .. self.jid .. '-dependents'),
-    dependencies = redis.call(
-      'smembers', QlessJob.ns .. self.jid .. '-dependencies')
+    dependents = redis.call('smembers', QlessJob.ns .. self.jid .. '-dependents'),
+    dependencies = redis.call('smembers', QlessJob.ns .. self.jid .. '-dependencies'),
   }
 
   if #arg > 0 then
     -- This section could probably be optimized, but I wanted the interface
     -- in place first
     local response = {}
-    for index, key in ipairs(arg) do
+    for _, key in ipairs(arg) do
       table.insert(response, data[key])
     end
     return response
   else
     return data
   end
 end
@@ -586,37 +587,37 @@
 -- The variable-length arguments may be pairs of the form:
 --
 --      ('next'   , queue) : The queue to advance it to next
 --      ('delay'  , delay) : The delay for the next queue
 --      ('depends',        : Json of jobs it depends on in the new queue
 --          '["jid1", "jid2", ...]')
 ---
-function QlessJob:complete(now, worker, queue, raw_data, ...)
+function QlessJob:complete(now, worker, queue_name, raw_data, ...)
   assert(worker, 'Complete(): Arg "worker" missing')
-  assert(queue , 'Complete(): Arg "queue" missing')
+  assert(queue_name , 'Complete(): Arg "queue_name" missing')
   local data = assert(cjson.decode(raw_data),
     'Complete(): Arg "data" missing or not JSON: ' .. tostring(raw_data))
 
   -- Read in all the optional parameters
   local options = {}
   for i = 1, #arg, 2 do options[arg[i]] = arg[i + 1] end
 
   -- Sanity check on optional args
-  local nextq   = options['next']
-  local delay   = assert(tonumber(options['delay'] or 0))
+  local next_queue_name = options['next']
+  local delay = assert(tonumber(options['delay'] or 0))
   local depends = assert(cjson.decode(options['depends'] or '[]'),
     'Complete(): Arg "depends" not JSON: ' .. tostring(options['depends']))
 
-  -- Depends doesn't make sense without nextq
-  if options['delay'] and nextq == nil then
+  -- Depends doesn't make sense without next_queue_name
+  if options['delay'] and next_queue_name == nil then
     error('Complete(): "delay" cannot be used without a "next".')
   end
 
-  -- Depends doesn't make sense without nextq
-  if options['depends'] and nextq == nil then
+  -- Depends doesn't make sense without next_queue_name
+  if options['depends'] and next_queue_name == nil then
     error('Complete(): "depends" cannot be used without a "next".')
   end
 
   -- The bin is midnight of the provided day
   -- 24 * 60 * 60 = 86400
   local bin = now - (now % 86400)
 
@@ -628,15 +629,15 @@
   if lastworker == false then
     error('Complete(): Job does not exist')
   elseif (state ~= 'running') then
     error('Complete(): Job is not currently running: ' .. state)
   elseif lastworker ~= worker then
     error('Complete(): Job has been handed out to another worker: ' ..
       tostring(lastworker))
-  elseif queue ~= current_queue then
+  elseif queue_name ~= current_queue then
     error('Complete(): Job running in another queue: ' ..
       tostring(current_queue))
   end
 
   -- Now we can assume that the worker does own the job. We need to
   --    1) Remove the job from the 'locks' from the old queue
   --    2) Enqueue it in the next stage if necessary
@@ -646,103 +647,103 @@
   self:history(now, 'done')
 
   if raw_data then
     redis.call('hset', QlessJob.ns .. self.jid, 'data', raw_data)
   end
 
   -- Remove the job from the previous queue
-  local queue_obj = Qless.queue(queue)
-  queue_obj:remove_job(self.jid)
+  local queue = Qless.queue(queue_name)
+  queue:remove_job(self.jid)
 
   self:throttles_release(now)
 
   ----------------------------------------------------------
   -- This is the massive stats update that we have to do
   ----------------------------------------------------------
   -- This is how long we've been waiting to get popped
   -- local waiting = math.floor(now) - history[#history]['popped']
   local time = tonumber(
     redis.call('hget', QlessJob.ns .. self.jid, 'time') or now)
   local waiting = now - time
-  queue_obj:stat(now, 'run', waiting)
+  queue:stat(now, 'run', waiting)
   redis.call('hset', QlessJob.ns .. self.jid,
     'time', string.format("%.20f", now))
 
   -- Remove this job from the jobs that the worker that was running it has
   redis.call('zrem', 'ql:w:' .. worker .. ':jobs', self.jid)
 
   if redis.call('zscore', 'ql:tracked', self.jid) ~= false then
     Qless.publish('completed', self.jid)
   end
 
-  if nextq then
-    queue_obj = Qless.queue(nextq)
+  if next_queue_name then
+    local next_queue = Qless.queue(next_queue_name)
     -- Send a message out to log
     Qless.publish('log', cjson.encode({
-      jid   = self.jid,
+      jid = self.jid,
       event = 'advanced',
-      queue = queue,
-      to    = nextq
+      queue = queue_name,
+      to = next_queue_name,
     }))
 
     -- Enqueue the job
-    self:history(now, 'put', {q = nextq})
+    self:history(now, 'put', {q = next_queue_name})
 
     -- We're going to make sure that this queue is in the
     -- set of known queues
-    if redis.call('zscore', 'ql:queues', nextq) == false then
-      redis.call('zadd', 'ql:queues', now, nextq)
+    if redis.call('zscore', 'ql:queues', next_queue_name) == false then
+      redis.call('zadd', 'ql:queues', now, next_queue_name)
     end
 
     redis.call('hmset', QlessJob.ns .. self.jid,
       'state', 'waiting',
       'worker', '',
       'failure', '{}',
-      'queue', nextq,
+      'queue', next_queue_name,
       'expires', 0,
       'remaining', tonumber(retries))
 
     if (delay > 0) and (#depends == 0) then
-      queue_obj.scheduled.add(now + delay, self.jid)
+      next_queue.scheduled.add(now + delay, self.jid)
       return 'scheduled'
     else
       -- These are the jids we legitimately have to wait on
       local count = 0
-      for i, j in ipairs(depends) do
+      for _, j in ipairs(depends) do
         -- Make sure it's something other than 'nil' or complete.
         local state = redis.call('hget', QlessJob.ns .. j, 'state')
         if (state and state ~= 'complete') then
           count = count + 1
           redis.call(
             'sadd', QlessJob.ns .. j .. '-dependents',self.jid)
           redis.call(
             'sadd', QlessJob.ns .. self.jid .. '-dependencies', j)
         end
       end
       if count > 0 then
-        queue_obj.depends.add(now, self.jid)
+        next_queue.depends.add(now, self.jid)
         redis.call('hset', QlessJob.ns .. self.jid, 'state', 'depends')
         if delay > 0 then
           -- We've already put it in 'depends'. Now, we must just save the data
           -- for when it's scheduled
-          queue_obj.depends.add(now, self.jid)
+          next_queue.depends.add(now, self.jid)
           redis.call('hset', QlessJob.ns .. self.jid, 'scheduled', now + delay)
         end
         return 'depends'
       else
-        queue_obj.work.add(now, priority, self.jid)
+        next_queue.work.add(now, priority, self.jid)
         return 'waiting'
       end
     end
   else
     -- Send a message out to log
     Qless.publish('log', cjson.encode({
-      jid   = self.jid,
+      jid = self.jid,
       event = 'completed',
-      queue = queue
+      queue = queue_name,
     }))
 
     redis.call('hmset', QlessJob.ns .. self.jid,
       'state', 'complete',
       'worker', '',
       'failure', '{}',
       'queue', '',
@@ -759,46 +760,46 @@
 
     -- Schedule this job for destructination eventually
     redis.call('zadd', 'ql:completed', now, self.jid)
 
     -- Now look at the expired job data. First, based on the current time
     local jids = redis.call('zrangebyscore', 'ql:completed', 0, now - time)
     -- Any jobs that need to be expired... delete
-    for index, jid in ipairs(jids) do
+    for _, jid in ipairs(jids) do
       Qless.job(jid):delete()
     end
 
     -- And now remove those from the queued-for-cleanup queue
     redis.call('zremrangebyscore', 'ql:completed', 0, now - time)
 
     -- Now take the all by the most recent 'count' ids
     jids = redis.call('zrange', 'ql:completed', 0, (-1-count))
-    for index, jid in ipairs(jids) do
+    for _, jid in ipairs(jids) do
       Qless.job(jid):delete()
     end
     redis.call('zremrangebyrank', 'ql:completed', 0, (-1-count))
 
     -- Alright, if this has any dependents, then we should go ahead
     -- and unstick those guys.
-    for i, j in ipairs(redis.call(
+    for _, j in ipairs(redis.call(
       'smembers', QlessJob.ns .. self.jid .. '-dependents')) do
       redis.call('srem', QlessJob.ns .. j .. '-dependencies', self.jid)
       if redis.call(
         'scard', QlessJob.ns .. j .. '-dependencies') == 0 then
-        local q, p, scheduled = unpack(
+        local other_queue_name, priority, scheduled = unpack(
           redis.call('hmget', QlessJob.ns .. j, 'queue', 'priority', 'scheduled'))
-        if q then
-          local queue = Qless.queue(q)
-          queue.depends.remove(j)
+        if other_queue_name then
+          local other_queue = Qless.queue(other_queue_name)
+          other_queue.depends.remove(j)
           if scheduled then
-            queue.scheduled.add(scheduled, j)
+            other_queue.scheduled.add(scheduled, j)
             redis.call('hset', QlessJob.ns .. j, 'state', 'scheduled')
             redis.call('hdel', QlessJob.ns .. j, 'scheduled')
           else
-            queue.work.add(now, p, j)
+            other_queue.work.add(now, priority, j)
             redis.call('hset', QlessJob.ns .. j, 'state', 'waiting')
           end
         end
       end
     end
 
     -- Delete our dependents key
@@ -844,33 +845,33 @@
   local bin = now - (now % 86400)
 
   if data then
     data = cjson.decode(data)
   end
 
   -- First things first, we should get the history
-  local queue, state, oldworker = unpack(redis.call(
+  local queue_name, state, oldworker = unpack(redis.call(
     'hmget', QlessJob.ns .. self.jid, 'queue', 'state', 'worker'))
 
   -- If the job has been completed, we cannot fail it
   if not state then
     error('Fail(): Job does not exist')
   elseif state ~= 'running' then
     error('Fail(): Job not currently running: ' .. state)
   elseif worker ~= oldworker then
     error('Fail(): Job running with another worker: ' .. oldworker)
   end
 
   -- Send out a log message
   Qless.publish('log', cjson.encode({
-    jid     = self.jid,
-    event   = 'failed',
-    worker  = worker,
-    group   = group,
-    message = message
+    jid = self.jid,
+    event = 'failed',
+    worker = worker,
+    group = group,
+    message = message,
   }))
 
   if redis.call('zscore', 'ql:tracked', self.jid) ~= false then
     Qless.publish('failed', self.jid)
   end
 
   -- Remove this job from the jobs that the worker that was running it has
@@ -878,21 +879,21 @@
 
   -- Now, take the element of the history for which our provided worker is
   -- the worker, and update 'failed'
   self:history(now, 'failed', {worker = worker, group = group})
 
   -- Increment the number of failures for that queue for the
   -- given day.
-  redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue, 'failures', 1)
-  redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue, 'failed'  , 1)
+  redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue_name, 'failures', 1)
+  redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue_name, 'failed'  , 1)
 
   -- Now remove the instance from the schedule, and work queues for the
   -- queue it's in
-  local queue_obj = Qless.queue(queue)
-  queue_obj:remove_job(self.jid)
+  local queue = Qless.queue(queue_name)
+  queue:remove_job(self.jid)
 
   -- The reason that this appears here is that the above will fail if the
   -- job doesn't exist
   if data then
     redis.call('hset', QlessJob.ns .. self.jid, 'data', cjson.encode(data))
   end
 
@@ -916,15 +917,15 @@
 
   -- Here is where we'd increment stats about the particular stage
   -- and possibly the workers
 
   return self.jid
 end
 
--- retry(now, queue, worker, [delay, [group, [message]]])
+-- retry(now, queue_name, worker, [delay, [group, [message]]])
 -- ------------------------------------------
 -- This script accepts jid, queue, worker and delay for retrying a job. This
 -- is similar in functionality to `put`, except that this counts against the
 -- retries a job has for a stage.
 --
 -- Throws an exception if:
 --      - the worker is not the worker with a lock on the job
@@ -933,22 +934,22 @@
 -- Otherwise, it returns the number of retries remaining. If the allowed
 -- retries have been exhausted, then it is automatically failed, and a negative
 -- number is returned.
 --
 -- If a group and message is provided, then if the retries are exhausted, then
 -- the provided group and message will be used in place of the default
 -- messaging about retries in the particular queue being exhausted
-function QlessJob:retry(now, queue, worker, delay, group, message)
-  assert(queue , 'Retry(): Arg "queue" missing')
+function QlessJob:retry(now, queue_name, worker, delay, group, message)
+  assert(queue_name , 'Retry(): Arg "queue_name" missing')
   assert(worker, 'Retry(): Arg "worker" missing')
   delay = assert(tonumber(delay or 0),
     'Retry(): Arg "delay" not a number: ' .. tostring(delay))
 
   -- Let's see what the old priority, and tags were
-  local oldqueue, state, retries, oldworker, priority, failure = unpack(
+  local old_queue_name, state, retries, oldworker, priority, failure = unpack(
     redis.call('hmget', QlessJob.ns .. self.jid, 'queue', 'state',
       'retries', 'worker', 'priority', 'failure'))
 
   -- If this isn't the worker that owns
   if oldworker == false then
     error('Retry(): Job does not exist')
   elseif state ~= 'running' then
@@ -961,26 +962,26 @@
   -- have exhausted their retries, then we should mark them as
   -- failed.
   local remaining = tonumber(redis.call(
     'hincrby', QlessJob.ns .. self.jid, 'remaining', -1))
   redis.call('hdel', QlessJob.ns .. self.jid, 'grace')
 
   -- Remove it from the locks key of the old queue
-  Qless.queue(oldqueue).locks.remove(self.jid)
+  Qless.queue(old_queue_name).locks.remove(self.jid)
 
   -- Release the throttle for the job
   self:throttles_release(now)
 
   -- Remove this job from the worker that was previously working it
   redis.call('zrem', 'ql:w:' .. worker .. ':jobs', self.jid)
 
   if remaining < 0 then
     -- Now remove the instance from the schedule, and work queues for the
     -- queue it's in
-    local group = group or 'failed-retries-' .. queue
+    local group = group or 'failed-retries-' .. queue_name
     self:history(now, 'failed', {['group'] = group})
 
     redis.call('hmset', QlessJob.ns .. self.jid, 'state', 'failed',
       'worker', '',
       'expires', '')
     -- If the failure has not already been set, then set it
     if group ~= nil and message ~= nil then
@@ -993,36 +994,36 @@
         })
       )
     else
       redis.call('hset', QlessJob.ns .. self.jid,
       'failure', cjson.encode({
         ['group']   = group,
         ['message'] =
-          'Job exhausted retries in queue "' .. oldqueue .. '"',
+          'Job exhausted retries in queue "' .. old_queue_name .. '"',
         ['when']    = now,
         ['worker']  = unpack(self:data('worker'))
       }))
     end
 
     -- Add this type of failure to the list of failures
     redis.call('sadd', 'ql:failures', group)
     -- And add this particular instance to the failed types
     redis.call('lpush', 'ql:f:' .. group, self.jid)
     -- Increment the count of the failed jobs
     local bin = now - (now % 86400)
-    redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue, 'failures', 1)
-    redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue, 'failed'  , 1)
+    redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue_name, 'failures', 1)
+    redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue_name, 'failed'  , 1)
   else
     -- Put it in the queue again with a delay. Like put()
-    local queue_obj = Qless.queue(queue)
+    local queue = Qless.queue(queue_name)
     if delay > 0 then
-      queue_obj.scheduled.add(now + delay, self.jid)
+      queue.scheduled.add(now + delay, self.jid)
       redis.call('hset', QlessJob.ns .. self.jid, 'state', 'scheduled')
     else
-      queue_obj.work.add(now, priority, self.jid)
+      queue.work.add(now, priority, self.jid)
       redis.call('hset', QlessJob.ns .. self.jid, 'state', 'waiting')
     end
 
     -- If a group and a message was provided, then we should save it
     if group ~= nil and message ~= nil then
       redis.call('hset', QlessJob.ns .. self.jid,
         'failure', cjson.encode({
@@ -1055,53 +1056,53 @@
   if state ~= 'depends' then
     error('Depends(): Job ' .. self.jid ..
       ' not in the depends state: ' .. tostring(state))
   end
 
   if command == 'on' then
     -- These are the jids we legitimately have to wait on
-    for i, j in ipairs(arg) do
+    for _, j in ipairs(arg) do
       -- Make sure it's something other than 'nil' or complete.
       local state = redis.call('hget', QlessJob.ns .. j, 'state')
       if (state and state ~= 'complete') then
         redis.call(
           'sadd', QlessJob.ns .. j .. '-dependents'  , self.jid)
         redis.call(
           'sadd', QlessJob.ns .. self.jid .. '-dependencies', j)
       end
     end
     return true
   elseif command == 'off' then
     if arg[1] == 'all' then
-      for i, j in ipairs(redis.call(
+      for _, j in ipairs(redis.call(
         'smembers', QlessJob.ns .. self.jid .. '-dependencies')) do
         redis.call('srem', QlessJob.ns .. j .. '-dependents', self.jid)
       end
       redis.call('del', QlessJob.ns .. self.jid .. '-dependencies')
-      local q, p = unpack(redis.call(
+      local queue_name, priority = unpack(redis.call(
         'hmget', QlessJob.ns .. self.jid, 'queue', 'priority'))
-      if q then
-        local queue_obj = Qless.queue(q)
-        queue_obj.depends.remove(self.jid)
-        queue_obj.work.add(now, p, self.jid)
+      if queue_name then
+        local queue = Qless.queue(queue_name)
+        queue.depends.remove(self.jid)
+        queue.work.add(now, priority, self.jid)
         redis.call('hset', QlessJob.ns .. self.jid, 'state', 'waiting')
       end
     else
-      for i, j in ipairs(arg) do
+      for _, j in ipairs(arg) do
         redis.call('srem', QlessJob.ns .. j .. '-dependents', self.jid)
         redis.call(
           'srem', QlessJob.ns .. self.jid .. '-dependencies', j)
         if redis.call('scard',
           QlessJob.ns .. self.jid .. '-dependencies') == 0 then
-          local q, p = unpack(redis.call(
+          local queue_name, priority = unpack(redis.call(
             'hmget', QlessJob.ns .. self.jid, 'queue', 'priority'))
-          if q then
-            local queue_obj = Qless.queue(q)
-            queue_obj.depends.remove(self.jid)
-            queue_obj.work.add(now, p, self.jid)
+          if queue_name then
+            local queue = Qless.queue(queue_name)
+            queue.depends.remove(self.jid)
+            queue.work.add(now, priority, self.jid)
             redis.call('hset',
               QlessJob.ns .. self.jid, 'state', 'waiting')
           end
         end
       end
     end
     return true
@@ -1119,17 +1120,17 @@
 --      - the job's not running
 function QlessJob:heartbeat(now, worker, data)
   assert(worker, 'Heatbeat(): Arg "worker" missing')
 
   -- We should find the heartbeat interval for this queue
   -- heartbeat. First, though, we need to find the queue
   -- this particular job is in
-  local queue = redis.call('hget', QlessJob.ns .. self.jid, 'queue') or ''
+  local queue_name = redis.call('hget', QlessJob.ns .. self.jid, 'queue') or ''
   local expires = now + tonumber(
-    Qless.config.get(queue .. '-heartbeat') or
+    Qless.config.get(queue_name .. '-heartbeat') or
     Qless.config.get('heartbeat', 60))
 
   if data then
     data = cjson.decode(data)
   end
 
   -- First, let's see if the worker still owns this job, and there is a
@@ -1173,29 +1174,29 @@
 -- exception
 function QlessJob:priority(priority)
   priority = assert(tonumber(priority),
     'Priority(): Arg "priority" missing or not a number: ' ..
     tostring(priority))
 
   -- Get the queue the job is currently in, if any
-  local queue = redis.call('hget', QlessJob.ns .. self.jid, 'queue')
+  local queue_name = redis.call('hget', QlessJob.ns .. self.jid, 'queue')
 
-  if queue == nil then
+  if queue_name == nil then
     -- If the job doesn't exist, throw an error
     error('Priority(): Job ' .. self.jid .. ' does not exist')
-  elseif queue == '' then
+  elseif queue_name == '' then
     -- Just adjust the priority
     redis.call('hset', QlessJob.ns .. self.jid, 'priority', priority)
     return priority
   else
     -- Adjust the priority and see if it's a candidate for updating
     -- its priority in the queue it's currently in
-    local queue_obj = Qless.queue(queue)
-    if queue_obj.work.score(self.jid) then
-      queue_obj.work.add(0, priority, self.jid)
+    local queue = Qless.queue(queue_name)
+    if queue.work.score(self.jid) then
+      queue.work.add(0, priority, self.jid)
     end
     redis.call('hset', QlessJob.ns .. self.jid, 'priority', priority)
     return priority
   end
 end
 
 -- Update the jobs' attributes with the provided dictionary
@@ -1225,17 +1226,17 @@
     -- Release acquired throttles
     self:throttles_release(now)
 
     queue.work.add(now, math.huge, self.jid)
     redis.call('hmset', QlessJob.ns .. self.jid,
       'state', 'stalled', 'expires', 0)
     local encoded = cjson.encode({
-      jid    = self.jid,
-      event  = 'lock_lost',
-      worker = worker
+      jid = self.jid,
+      event = 'lock_lost',
+      worker = worker,
     })
     Qless.publish('w:' .. worker, encoded)
     Qless.publish('log', encoded)
     return queue_name
   end
 end
 
@@ -1246,15 +1247,15 @@
 
 -- Get or append to history
 function QlessJob:history(now, what, item)
   -- First, check if there's an old-style history, and update it if there is
   local history = redis.call('hget', QlessJob.ns .. self.jid, 'history')
   if history then
     history = cjson.decode(history)
-    for i, value in ipairs(history) do
+    for _, value in ipairs(history) do
       redis.call('rpush', QlessJob.ns .. self.jid .. '-history',
         cjson.encode({math.floor(value.put), 'put', {q = value.q}}))
 
       -- If there's any popped time
       if value.popped then
         redis.call('rpush', QlessJob.ns .. self.jid .. '-history',
           cjson.encode({math.floor(value.popped), 'popped',
@@ -1279,15 +1280,15 @@
     redis.call('hdel', QlessJob.ns .. self.jid, 'history')
   end
 
   -- Now to the meat of the function
   if what == nil then
     -- Get the history
     local response = {}
-    for i, value in ipairs(redis.call('lrange',
+    for _, value in ipairs(redis.call('lrange',
       QlessJob.ns .. self.jid .. '-history', 0, -1)) do
       value = cjson.decode(value)
       local dict = value[3] or {}
       dict['when'] = value[1]
       dict['what'] = value[2]
       table.insert(response, dict)
     end
@@ -1363,15 +1364,15 @@
 -- Completely removes all the data
 -- associated with this job, use
 -- with care.
 function QlessJob:delete()
   local tags = redis.call('hget', QlessJob.ns .. self.jid, 'tags') or '[]'
   tags = cjson.decode(tags)
   -- remove the jid from each tag
-  for i, tag in ipairs(tags) do
+  for _, tag in ipairs(tags) do
     self:remove_tag(tag)
   end
   -- Delete the job's data
   redis.call('del', QlessJob.ns .. self.jid)
   -- Delete the job's history
   redis.call('del', QlessJob.ns .. self.jid .. '-history')
   -- Delete any notion of dependencies it has
@@ -1418,24 +1419,19 @@
   assert(name, 'Queue(): no queue name provided')
   local queue = {}
   setmetatable(queue, QlessQueue)
   queue.name = name
 
   -- Access to our work
   queue.work = {
-    peek = function(count)
-      if count == 0 then
+    peek = function(offset, count)
+      if count <= 0 then
         return {}
       end
-      local jids = {}
-      for index, jid in ipairs(redis.call(
-        'zrevrange', queue:prefix('work'), 0, count - 1)) do
-        table.insert(jids, jid)
-      end
-      return jids
+      return redis.call('zrevrange', queue:prefix('work'), offset, offset + count - 1)
     end, remove = function(...)
       if #arg > 0 then
         return redis.call('zrem', queue:prefix('work'), unpack(arg))
       end
     end, add = function(now, priority, jid)
       return redis.call('zadd',
         queue:prefix('work'), priority - (now / 10000000000), jid)
@@ -1490,16 +1486,16 @@
   }
 
 
   -- Access to the queue level throttled jobs.
   queue.throttled = {
     length = function()
       return (redis.call('zcard', queue:prefix('throttled')) or 0)
-    end, peek = function(now, min, max)
-      return redis.call('zrange', queue:prefix('throttled'), min, max)
+    end, peek = function(now, offset, count)
+      return redis.call('zrange', queue:prefix('throttled'), offset, offset + count - 1)
     end, add = function(...)
       if #arg > 0 then
         redis.call('zadd', queue:prefix('throttled'), unpack(arg))
       end
     end, remove = function(...)
       if #arg > 0 then
         return redis.call('zrem', queue:prefix('throttled'), unpack(arg))
@@ -1550,17 +1546,17 @@
   }
   return queue
 end
 
 -- Return the prefix for this particular queue
 function QlessQueue:prefix(group)
   if group then
-    return QlessQueue.ns..self.name..'-'..group
+    return QlessQueue.ns .. self.name .. '-' .. group
   else
-    return QlessQueue.ns..self.name
+    return QlessQueue.ns .. self.name
   end
 end
 
 -- Stats(now, date)
 -- ---------------------
 -- Return the current statistics for a given queue on a given date. The
 -- results are returned are a JSON blob:
@@ -1590,15 +1586,15 @@
 -- The histogram's data points are at the second resolution for the first
 -- minute, the minute resolution for the first hour, the 15-minute resolution
 -- for the first day, the hour resolution for the first 3 days, and then at
 -- the day resolution from there on out. The `histogram` key is a list of
 -- those values.
 function QlessQueue:stats(now, date)
   date = assert(tonumber(date),
-    'Stats(): Arg "date" missing or not a number: '.. (date or 'nil'))
+    'Stats(): Arg "date" missing or not a number: ' .. (date or 'nil'))
 
   -- The bin is midnight of the provided day
   -- 24 * 60 * 60 = 86400
   local bin = date - (date % 86400)
 
   -- This a table of all the keys we want to use in order to produce a histogram
   local histokeys = {
@@ -1630,15 +1626,15 @@
         results.std = math.sqrt(vk / (count - 1))
       else
         results.std = 0
       end
     end
 
     local histogram = redis.call('hmget', key, unpack(histokeys))
-    for i=1,#histokeys do
+    for i=1, #histokeys do
       table.insert(results.histogram, tonumber(histogram[i]) or 0)
     end
     return results
   end
 
   local retries, failed, failures = unpack(redis.call('hmget', 'ql:s:stats:' .. bin .. ':' .. self.name, 'retries', 'failed', 'failures'))
   return {
@@ -1650,39 +1646,61 @@
   }
 end
 
 -- Peek
 -------
 -- Examine the next jobs that would be popped from the queue without actually
 -- popping them.
-function QlessQueue:peek(now, count)
+function QlessQueue:peek(now, offset, count)
+  offset = assert(tonumber(offset),
+    'Peek(): Arg "offset" missing or not a number: ' .. tostring(offset))
+
   count = assert(tonumber(count),
     'Peek(): Arg "count" missing or not a number: ' .. tostring(count))
 
+  if count <= 0 then
+    return {}
+  end
+
+  local count_with_offset = offset + count
+
   -- These are the ids that we're going to return. We'll begin with any jobs
   -- that have lost their locks
-  local jids = self.locks.expired(now, 0, count)
+  local jids = self.locks.expired(now, 0, count_with_offset)
+
+  -- Since we can't just peek the range we want, we have to consider all offset
+  -- + count jobs before we can take the relevant range.
+  local remaining_capacity = count_with_offset - #jids
 
   -- If we still need jobs in order to meet demand, then we should
   -- look for all the recurring jobs that need jobs run
-  self:check_recurring(now, count - #jids)
+  self:check_recurring(now, remaining_capacity)
 
   -- Now we've checked __all__ the locks for this queue the could
   -- have expired, and are no more than the number requested. If
   -- we still need values in order to meet the demand, then we
   -- should check if any scheduled items, and if so, we should
   -- insert them to ensure correctness when pulling off the next
   -- unit of work.
-  self:check_scheduled(now, count - #jids)
+  self:check_scheduled(now, remaining_capacity)
 
-  -- With these in place, we can expand this list of jids based on the work
-  -- queue itself and the priorities therein
-  table_extend(jids, self.work.peek(count - #jids))
+  if offset > #jids then
+    -- Offset takes us past the expired jids, so just return straight from the
+    -- work queue
+    return self.work.peek(offset - #jids, count)
+  else
+    -- Return a mix of expired jids and prioritized items from the work queue
+    table_extend(jids, self.work.peek(0, remaining_capacity))
 
-  return jids
+    if #jids < offset then
+      return {}
+    end
+
+    return {unpack(jids, offset + 1, count_with_offset)}
+  end
 end
 
 -- Return true if this queue is paused
 function QlessQueue:paused()
   return redis.call('sismember', 'ql:paused_queues', self.name) == 1
 end
 
@@ -1716,15 +1734,15 @@
 
   -- Make sure we this worker to the list of seen workers
   redis.call('zadd', 'ql:workers', now, worker)
 
   local dead_jids = self:invalidate_locks(now, count) or {}
   local popped = {}
 
-  for index, jid in ipairs(dead_jids) do
+  for _, jid in ipairs(dead_jids) do
     local success = self:pop_job(now, worker, Qless.job(jid))
     -- only track jid if a job was popped and it's not a phantom jid
     if success then
       table.insert(popped, jid)
     end
   end
 
@@ -1756,23 +1774,23 @@
     Qless.config.get('max-pop-retry', 1)
   )
 
   -- Keep trying to fulfill fulfill jobs from the work queue until we reach
   -- the desired count or exhaust our retry limit
   while #popped < count and pop_retry_limit > 0 do
 
-    local jids = self.work.peek(count - #popped) or {}
+    local jids = self.work.peek(0, count - #popped) or {}
 
     -- If there is nothing in the work queue, then no need to keep looping
     if #jids == 0 then
       break
     end
 
 
-    for index, jid in ipairs(jids) do
+    for _, jid in ipairs(jids) do
       local job = Qless.job(jid)
       if job:throttles_acquire(now) then
         local success = self:pop_job(now, worker, job)
         -- only track jid if a job was popped and it's not a phantom jid
         if success then
           table.insert(popped, jid)
         end
@@ -1966,16 +1984,16 @@
 
   -- If this item was previously in another queue, then we should remove it from there
   -- and remove the associated throttle
   if oldqueue then
     local queue_obj = Qless.queue(oldqueue)
     queue_obj:remove_job(jid)
     local old_qid = QlessQueue.ns .. oldqueue
-    for index, tname in ipairs(throttles) do
-      if tname == old_qid then
+    for index, throttle_name in ipairs(throttles) do
+      if throttle_name == old_qid then
         table.remove(throttles, index)
       end
     end
   end
 
   -- If this had previously been given out to a worker, make sure to remove it
   -- from that worker's jobs
@@ -1998,15 +2016,15 @@
   -- If the job was previously in the 'completed' state, then we should
   -- remove it from being enqueued for destructination
   if state == 'complete' then
     redis.call('zrem', 'ql:completed', jid)
   end
 
   -- Add this job to the list of jobs tagged with whatever tags were supplied
-  for i, tag in ipairs(tags) do
+  for _, tag in ipairs(tags) do
     Qless.job(jid):insert_tag(now, tag)
   end
 
   -- If we're in the failed state, remove all of our data
   if state == 'failed' then
     failure = cjson.decode(failure)
     -- We need to make this remove it from the failed queues
@@ -2041,15 +2059,15 @@
     'throttles', cjson.encode(throttles)
   }
 
   -- First, let's save its data
   redis.call('hmset', QlessJob.ns .. jid, unpack(data))
 
   -- These are the jids we legitimately have to wait on
-  for i, j in ipairs(depends) do
+  for _, j in ipairs(depends) do
     -- Make sure it's something other than 'nil' or complete.
     local state = redis.call('hget', QlessJob.ns .. j, 'state')
     if (state and state ~= 'complete') then
       redis.call('sadd', QlessJob.ns .. j .. '-dependents'  , jid)
       redis.call('sadd', QlessJob.ns .. jid .. '-dependencies', j)
     end
   end
@@ -2103,15 +2121,15 @@
     'Unfail(): Arg "count" not a number: ' .. tostring(count))
 
   -- Get up to that many jobs, and we'll put them in the appropriate queue
   local jids = redis.call('lrange', 'ql:f:' .. group, -count, -1)
 
   -- And now set each job's state, and put it into the appropriate queue
   local toinsert = {}
-  for index, jid in ipairs(jids) do
+  for _, jid in ipairs(jids) do
     local job = Qless.job(jid)
     local data = job:data()
     job:history(now, 'put', {q = self.name})
     redis.call('hmset', QlessJob.ns .. data.jid,
       'state'    , 'waiting',
       'worker'   , '',
       'expires'  , 0,
@@ -2178,16 +2196,16 @@
     local throttles = options['throttles'] or {}
 
     -- If it has previously been in another queue, then we should remove
     -- some information about it
     if old_queue then
       Qless.queue(old_queue).recurring.remove(jid)
 
-      for index, tname in ipairs(throttles) do
-        if tname == old_queue then
+      for index, throttle_name in ipairs(throttles) do
+        if throttle_name == old_queue then
           table.remove(throttles, index)
         end
       end
     end
 
     -- insert default queue throttle
     table.insert(throttles, QlessQueue.ns .. self.name)
@@ -2238,19 +2256,22 @@
   self.throttled.remove(jid)
   self.depends.remove(jid)
   self.scheduled.remove(jid)
 end
 
 -- Instantiate any recurring jobs that are ready
 function QlessQueue:check_recurring(now, count)
+  if count <= 0 then
+    return
+  end
   -- This is how many jobs we've moved so far
   local moved = 0
   -- These are the recurring jobs that need work
   local r = self.recurring.peek(now, 0, count)
-  for index, jid in ipairs(r) do
+  for _, jid in ipairs(r) do
     -- For each of the jids that need jobs scheduled, first
     -- get the last time each of them was run, and then increment
     -- it by its interval. While this time is less than now,
     -- we need to keep putting jobs on the queue
     local r = redis.call('hmget', 'ql:r:' .. jid, 'klass', 'data', 'priority',
         'tags', 'retries', 'interval', 'backlog', 'throttles')
     local klass, data, priority, tags, retries, interval, backlog, throttles = unpack(
@@ -2280,15 +2301,15 @@
       local count = redis.call('hincrby', 'ql:r:' .. jid, 'count', 1)
       moved = moved + 1
 
       local child_jid = jid .. '-' .. count
 
       -- Add this job to the list of jobs tagged with whatever tags were
       -- supplied
-      for i, tag in ipairs(_tags) do
+      for _, tag in ipairs(_tags) do
         Qless.job(child_jid):insert_tag(now, tag)
       end
 
       -- First, let's save its data
       redis.call('hmset', QlessJob.ns .. child_jid,
         'jid'      , child_jid,
         'klass'    , klass,
@@ -2318,18 +2339,21 @@
   end
 end
 
 -- Check for any jobs that have been scheduled, and shovel them onto
 -- the work queue. Returns nothing, but afterwards, up to `count`
 -- scheduled jobs will be moved into the work queue
 function QlessQueue:check_scheduled(now, count)
+  if count <= 0 then
+    return
+  end
   -- zadd is a list of arguments that we'll be able to use to
   -- insert into the work queue
   local scheduled = self.scheduled.ready(now, 0, count)
-  for index, jid in ipairs(scheduled) do
+  for _, jid in ipairs(scheduled) do
     -- With these in hand, we'll have to go out and find the
     -- priorities of these jobs, and then we'll insert them
     -- into the work queue and then when that's complete, we'll
     -- remove them from the scheduled queue
     local priority = tonumber(
       redis.call('hget', QlessJob.ns .. jid, 'priority') or 0)
     self.work.add(now, priority, jid)
@@ -2343,15 +2367,15 @@
 
 -- Check for and invalidate any locks that have been lost. Returns the
 -- list of jids that have been invalidated
 function QlessQueue:invalidate_locks(now, count)
   local jids = {}
   -- Iterate through all the expired locks and add them to the list
   -- of keys that we'll return
-  for index, jid in ipairs(self.locks.expired(now, 0, count)) do
+  for _, jid in ipairs(self.locks.expired(now, 0, count)) do
     -- Remove this job from the jobs that the worker that was running it
     -- has
     local worker, failure = unpack(
       redis.call('hmget', QlessJob.ns .. jid, 'worker', 'failure'))
     redis.call('zrem', 'ql:w:' .. worker .. ':jobs', jid)
 
     -- We'll provide a grace period after jobs time out for them to give
@@ -2385,15 +2409,15 @@
       redis.call('hset', QlessJob.ns .. jid, 'grace', 1)
 
       -- Send a message to let the worker know that its lost its lock on
       -- the job
       local encoded = cjson.encode({
         jid    = jid,
         event  = 'lock_lost',
-        worker = worker
+        worker = worker,
       })
       Qless.publish('w:' .. worker, encoded)
       Qless.publish('log', encoded)
       self.locks.add(now + grace_period, jid)
 
       -- If we got any expired locks, then we should increment the
       -- number of retries for this stage for this bin. The bin is
@@ -2508,30 +2532,30 @@
       depends   = queue.depends.length(),
       recurring = queue.recurring.length(),
       paused    = queue:paused()
     }
   else
     local queues = redis.call('zrange', 'ql:queues', 0, -1)
     local response = {}
-    for index, qname in ipairs(queues) do
+    for _, qname in ipairs(queues) do
       table.insert(response, QlessQueue.counts(now, qname))
     end
     return response
   end
 end
 -- Get all the attributes of this particular job
 function QlessRecurringJob:data()
   local job = redis.call(
     'hmget', 'ql:r:' .. self.jid, 'jid', 'klass', 'state', 'queue',
     'priority', 'interval', 'retries', 'count', 'data', 'tags', 'backlog', 'throttles')
-  
+
   if not job[1] then
     return nil
   end
-  
+
   return {
     jid          = job[1],
     klass        = job[2],
     state        = job[3],
     queue        = job[4],
     priority     = tonumber(job[5]),
     interval     = tonumber(job[6]),
@@ -2547,15 +2571,15 @@
 -- Update the recurring job data. Key can be:
 --      - priority
 --      - interval
 --      - retries
 --      - data
 --      - klass
 --      - queue
---      - backlog 
+--      - backlog
 function QlessRecurringJob:update(now, ...)
   local options = {}
   -- Make sure that the job exists
   if redis.call('exists', 'ql:r:' .. self.jid) ~= 0 then
     for i = 1, #arg, 2 do
       local key = arg[i]
       local value = arg[i+1]
@@ -2579,16 +2603,16 @@
         local old_queue_name = redis.call('hget', 'ql:r:' .. self.jid, 'queue')
         local queue_obj = Qless.queue(old_queue_name)
         local score = queue_obj.recurring.score(self.jid)
 
         -- Detach from the old queue
         queue_obj.recurring.remove(self.jid)
         local throttles = cjson.decode(redis.call('hget', 'ql:r:' .. self.jid, 'throttles') or '{}')
-        for index, tname in ipairs(throttles) do
-          if tname == QlessQueue.ns .. old_queue_name then
+        for index, throttle_name in ipairs(throttles) do
+          if throttle_name == QlessQueue.ns .. old_queue_name then
             table.remove(throttles, index)
           end
         end
 
 
         -- Attach to the new queue
         table.insert(throttles, QlessQueue.ns .. value)
@@ -2621,19 +2645,19 @@
 function QlessRecurringJob:tag(...)
   local tags = redis.call('hget', 'ql:r:' .. self.jid, 'tags')
   -- If the job has been canceled / deleted, then return false
   if tags then
     -- Decode the json blob, convert to dictionary
     tags = cjson.decode(tags)
     local _tags = {}
-    for i,v in ipairs(tags) do _tags[v] = true end
-    
+    for _, v in ipairs(tags) do _tags[v] = true end
+
     -- Otherwise, add the job to the sorted set with that tags
-    for i=1,#arg do if _tags[arg[i]] == nil then table.insert(tags, arg[i]) end end
-    
+    for i=1, #arg do if _tags[arg[i]] == nil then table.insert(tags, arg[i]) end end
+
     tags = cjson.encode(tags)
     redis.call('hset', 'ql:r:' .. self.jid, 'tags', tags)
     return tags
   else
     error('Tag(): Job ' .. self.jid .. ' does not exist')
   end
 end
@@ -2642,22 +2666,22 @@
 function QlessRecurringJob:untag(...)
   -- Get the existing tags
   local tags = redis.call('hget', 'ql:r:' .. self.jid, 'tags')
   -- If the job has been canceled / deleted, then return false
   if tags then
     -- Decode the json blob, convert to dictionary
     tags = cjson.decode(tags)
-    local _tags    = {}
+    local _tags = {}
     -- Make a hash
-    for i,v in ipairs(tags) do _tags[v] = true end
+    for _, v in ipairs(tags) do _tags[v] = true end
     -- Delete these from the hash
-    for i = 1,#arg do _tags[arg[i]] = nil end
+    for i = 1, #arg do _tags[arg[i]] = nil end
     -- Back into a list
     local results = {}
-    for i, tag in ipairs(tags) do if _tags[tag] then table.insert(results, tag) end end
+    for _, tag in ipairs(tags) do if _tags[tag] then table.insert(results, tag) end end
     -- json encode them, set, and return
     tags = cjson.encode(results)
     redis.call('hset', 'ql:r:' .. self.jid, 'tags', tags)
     return tags
   else
     error('Untag(): Job ' .. self.jid .. ' does not exist')
   end
@@ -2681,28 +2705,28 @@
 function QlessWorker.deregister(...)
   redis.call('zrem', 'ql:workers', unpack(arg))
 end
 
 -- Provide data about all the workers, or if a specific worker is provided,
 -- then which jobs that worker is responsible for. If no worker is provided,
 -- expect a response of the form:
--- 
+--
 --  [
 --      # This is sorted by the recency of activity from that worker
 --      {
 --          'name'   : 'hostname1-pid1',
 --          'jobs'   : 20,
 --          'stalled': 0
 --      }, {
 --          ...
 --      }
 --  ]
--- 
+--
 -- If a worker id is provided, then expect a response of the form:
--- 
+--
 --  {
 --      'jobs': [
 --          jid1,
 --          jid2,
 --          ...
 --      ], 'stalled': [
 --          jid1,
@@ -2713,30 +2737,30 @@
 function QlessWorker.counts(now, worker)
   -- Clean up all the workers' job lists if they're too old. This is
   -- determined by the `max-worker-age` configuration, defaulting to the
   -- last day. Seems like a 'reasonable' default
   local interval = tonumber(Qless.config.get('max-worker-age', 86400))
 
   local workers  = redis.call('zrangebyscore', 'ql:workers', 0, now - interval)
-  for index, worker in ipairs(workers) do
+  for _, worker in ipairs(workers) do
     redis.call('del', 'ql:w:' .. worker .. ':jobs')
   end
 
   -- And now remove them from the list of known workers
   redis.call('zremrangebyscore', 'ql:workers', 0, now - interval)
 
   if worker then
     return {
       jobs    = redis.call('zrevrangebyscore', 'ql:w:' .. worker .. ':jobs', now + 8640000, now),
       stalled = redis.call('zrevrangebyscore', 'ql:w:' .. worker .. ':jobs', now, 0)
     }
   else
     local response = {}
     local workers = redis.call('zrevrange', 'ql:workers', 0, -1)
-    for index, worker in ipairs(workers) do
+    for _, worker in ipairs(workers) do
       table.insert(response, {
         name    = worker,
         jobs    = redis.call('zcount', 'ql:w:' .. worker .. ':jobs', now, now + 8640000),
         stalled = redis.call('zcount', 'ql:w:' .. worker .. ':jobs', 0, now)
       })
     end
     return response
```

### Comparing `reqless-0.13.2/reqless/lua/qless.lua` & `reqless-0.13.3/reqless/lua/qless.lua`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
--- Current SHA: 09dc4ef4bb3cf089ef285d0a92a51b9af398ca03
+-- Current SHA: 62857f66dee92b76fc8b0e12ca6d588feba2d225
 -- This is a generated file
 local Qless = {
   ns = 'ql:'
 }
 
 local QlessQueue = {
   ns = Qless.ns .. 'q:'
@@ -26,15 +26,15 @@
 
 local QlessRecurringJob = {}
 QlessRecurringJob.__index = QlessRecurringJob
 
 Qless.config = {}
 
 local function table_extend(self, other)
-  for i, v in ipairs(other) do
+  for _, v in ipairs(other) do
     table.insert(self, v)
   end
 end
 
 function Qless.publish(channel, message)
   redis.call('publish', Qless.ns .. channel, message)
 end
@@ -111,15 +111,15 @@
     return {
       total = redis.call('llen', 'ql:f:' .. group),
       jobs  = redis.call('lrange', 'ql:f:' .. group, start, start + limit - 1)
     }
   else
     local response = {}
     local groups = redis.call('smembers', 'ql:failures')
-    for index, group in ipairs(groups) do
+    for _, group in ipairs(groups) do
       response[group] = redis.call('llen', 'ql:f:' .. group)
     end
     return response
   end
 end
 
 function Qless.jobs(now, state, ...)
@@ -170,18 +170,18 @@
       return redis.call('zrem', 'ql:tracked', jid)
     else
       error('Track(): Unknown action "' .. command .. '"')
     end
   else
     local response = {
       jobs = {},
-      expired = {}
+      expired = {},
     }
     local jids = redis.call('zrange', 'ql:tracked', 0, -1)
-    for index, jid in ipairs(jids) do
+    for _, jid in ipairs(jids) do
       local data = Qless.job(jid):data()
       if data then
         table.insert(response.jobs, data)
       else
         table.insert(response.expired, jid)
       end
     end
@@ -195,17 +195,17 @@
 
   if command == 'add' then
     local jid  = assert(arg[1], 'Tag(): Arg "jid" missing')
     local tags = redis.call('hget', QlessJob.ns .. jid, 'tags')
     if tags then
       tags = cjson.decode(tags)
       local _tags = {}
-      for i,v in ipairs(tags) do _tags[v] = true end
+      for _, v in ipairs(tags) do _tags[v] = true end
 
-      for i=2,#arg do
+      for i=2, #arg do
         local tag = arg[i]
         if _tags[tag] == nil then
           _tags[tag] = true
           table.insert(tags, tag)
         end
         Qless.job(jid):insert_tag(now, tag)
       end
@@ -217,24 +217,28 @@
     end
   elseif command == 'remove' then
     local jid  = assert(arg[1], 'Tag(): Arg "jid" missing')
     local tags = redis.call('hget', QlessJob.ns .. jid, 'tags')
     if tags then
       tags = cjson.decode(tags)
       local _tags = {}
-      for i,v in ipairs(tags) do _tags[v] = true end
+      for _, v in ipairs(tags) do _tags[v] = true end
 
-      for i=2,#arg do
+      for i=2, #arg do
         local tag = arg[i]
         _tags[tag] = nil
         Qless.job(jid):remove_tag(tag)
       end
 
       local results = {}
-      for i,tag in ipairs(tags) do if _tags[tag] then table.insert(results, tag) end end
+      for _, tag in ipairs(tags) do
+        if _tags[tag] then
+          table.insert(results, tag)
+        end
+      end
 
       redis.call('hset', QlessJob.ns .. jid, 'tags', cjson.encode(results))
       return results
     else
       error('Tag(): Job ' .. jid .. ' does not exist')
     end
   elseif command == 'get' then
@@ -259,15 +263,15 @@
 function Qless.cancel(now, ...)
   local dependents = {}
   for _, jid in ipairs(arg) do
     dependents[jid] = redis.call(
       'smembers', QlessJob.ns .. jid .. '-dependents') or {}
   end
 
-  for i, jid in ipairs(arg) do
+  for _, jid in ipairs(arg) do
     for j, dep in ipairs(dependents[jid]) do
       if dependents[dep] == nil then
         error('Cancel(): ' .. jid .. ' is a dependency of ' .. dep ..
            ' but is not mentioned to be canceled')
       end
     end
   end
@@ -295,15 +299,15 @@
         queue:remove_job(jid)
       end
 
       local job = Qless.job(jid)
 
       job:throttles_release(now)
 
-      for i, j in ipairs(redis.call(
+      for _, j in ipairs(redis.call(
         'smembers', QlessJob.ns .. jid .. '-dependencies')) do
         redis.call('srem', QlessJob.ns .. j .. '-dependents', jid)
       end
 
       if state == 'failed' then
         failure = cjson.decode(failure)
         redis.call('lrem', 'ql:f:' .. failure.group, 0, jid)
@@ -381,67 +385,64 @@
       'tags', 'failure', 'throttles', 'spawned_from_jid')
 
   if not job[1] then
     return nil
   end
 
   local data = {
-    jid              = job[1],
-    klass            = job[2],
-    state            = job[3],
-    queue            = job[4],
-    worker           = job[5] or '',
-    tracked          = redis.call(
-      'zscore', 'ql:tracked', self.jid) ~= false,
-    priority     = tonumber(job[6]),
-    expires      = tonumber(job[7]) or 0,
-    retries      = tonumber(job[8]),
-    remaining    = math.floor(tonumber(job[9])),
-    data         = job[10],
-    tags         = cjson.decode(job[11]),
-    history      = self:history(),
-    failure      = cjson.decode(job[12] or '{}'),
-    throttles    = cjson.decode(job[13] or '[]'),
+    jid = job[1],
+    klass = job[2],
+    state = job[3],
+    queue = job[4],
+    worker = job[5] or '',
+    tracked = redis.call('zscore', 'ql:tracked', self.jid) ~= false,
+    priority = tonumber(job[6]),
+    expires = tonumber(job[7]) or 0,
+    retries = tonumber(job[8]),
+    remaining = math.floor(tonumber(job[9])),
+    data = job[10],
+    tags = cjson.decode(job[11]),
+    history = self:history(),
+    failure = cjson.decode(job[12] or '{}'),
+    throttles = cjson.decode(job[13] or '[]'),
     spawned_from_jid = job[14],
-    dependents   = redis.call(
-      'smembers', QlessJob.ns .. self.jid .. '-dependents'),
-    dependencies = redis.call(
-      'smembers', QlessJob.ns .. self.jid .. '-dependencies')
+    dependents = redis.call('smembers', QlessJob.ns .. self.jid .. '-dependents'),
+    dependencies = redis.call('smembers', QlessJob.ns .. self.jid .. '-dependencies'),
   }
 
   if #arg > 0 then
     local response = {}
-    for index, key in ipairs(arg) do
+    for _, key in ipairs(arg) do
       table.insert(response, data[key])
     end
     return response
   else
     return data
   end
 end
 
-function QlessJob:complete(now, worker, queue, raw_data, ...)
+function QlessJob:complete(now, worker, queue_name, raw_data, ...)
   assert(worker, 'Complete(): Arg "worker" missing')
-  assert(queue , 'Complete(): Arg "queue" missing')
+  assert(queue_name , 'Complete(): Arg "queue_name" missing')
   local data = assert(cjson.decode(raw_data),
     'Complete(): Arg "data" missing or not JSON: ' .. tostring(raw_data))
 
   local options = {}
   for i = 1, #arg, 2 do options[arg[i]] = arg[i + 1] end
 
-  local nextq   = options['next']
-  local delay   = assert(tonumber(options['delay'] or 0))
+  local next_queue_name = options['next']
+  local delay = assert(tonumber(options['delay'] or 0))
   local depends = assert(cjson.decode(options['depends'] or '[]'),
     'Complete(): Arg "depends" not JSON: ' .. tostring(options['depends']))
 
-  if options['delay'] and nextq == nil then
+  if options['delay'] and next_queue_name == nil then
     error('Complete(): "delay" cannot be used without a "next".')
   end
 
-  if options['depends'] and nextq == nil then
+  if options['depends'] and next_queue_name == nil then
     error('Complete(): "depends" cannot be used without a "next".')
   end
 
   local bin = now - (now % 86400)
 
   local lastworker, state, priority, retries, current_queue = unpack(
     redis.call('hmget', QlessJob.ns .. self.jid, 'worker', 'state',
@@ -450,99 +451,99 @@
   if lastworker == false then
     error('Complete(): Job does not exist')
   elseif (state ~= 'running') then
     error('Complete(): Job is not currently running: ' .. state)
   elseif lastworker ~= worker then
     error('Complete(): Job has been handed out to another worker: ' ..
       tostring(lastworker))
-  elseif queue ~= current_queue then
+  elseif queue_name ~= current_queue then
     error('Complete(): Job running in another queue: ' ..
       tostring(current_queue))
   end
 
   self:history(now, 'done')
 
   if raw_data then
     redis.call('hset', QlessJob.ns .. self.jid, 'data', raw_data)
   end
 
-  local queue_obj = Qless.queue(queue)
-  queue_obj:remove_job(self.jid)
+  local queue = Qless.queue(queue_name)
+  queue:remove_job(self.jid)
 
   self:throttles_release(now)
 
   local time = tonumber(
     redis.call('hget', QlessJob.ns .. self.jid, 'time') or now)
   local waiting = now - time
-  queue_obj:stat(now, 'run', waiting)
+  queue:stat(now, 'run', waiting)
   redis.call('hset', QlessJob.ns .. self.jid,
     'time', string.format("%.20f", now))
 
   redis.call('zrem', 'ql:w:' .. worker .. ':jobs', self.jid)
 
   if redis.call('zscore', 'ql:tracked', self.jid) ~= false then
     Qless.publish('completed', self.jid)
   end
 
-  if nextq then
-    queue_obj = Qless.queue(nextq)
+  if next_queue_name then
+    local next_queue = Qless.queue(next_queue_name)
     Qless.publish('log', cjson.encode({
-      jid   = self.jid,
+      jid = self.jid,
       event = 'advanced',
-      queue = queue,
-      to    = nextq
+      queue = queue_name,
+      to = next_queue_name,
     }))
 
-    self:history(now, 'put', {q = nextq})
+    self:history(now, 'put', {q = next_queue_name})
 
-    if redis.call('zscore', 'ql:queues', nextq) == false then
-      redis.call('zadd', 'ql:queues', now, nextq)
+    if redis.call('zscore', 'ql:queues', next_queue_name) == false then
+      redis.call('zadd', 'ql:queues', now, next_queue_name)
     end
 
     redis.call('hmset', QlessJob.ns .. self.jid,
       'state', 'waiting',
       'worker', '',
       'failure', '{}',
-      'queue', nextq,
+      'queue', next_queue_name,
       'expires', 0,
       'remaining', tonumber(retries))
 
     if (delay > 0) and (#depends == 0) then
-      queue_obj.scheduled.add(now + delay, self.jid)
+      next_queue.scheduled.add(now + delay, self.jid)
       return 'scheduled'
     else
       local count = 0
-      for i, j in ipairs(depends) do
+      for _, j in ipairs(depends) do
         local state = redis.call('hget', QlessJob.ns .. j, 'state')
         if (state and state ~= 'complete') then
           count = count + 1
           redis.call(
             'sadd', QlessJob.ns .. j .. '-dependents',self.jid)
           redis.call(
             'sadd', QlessJob.ns .. self.jid .. '-dependencies', j)
         end
       end
       if count > 0 then
-        queue_obj.depends.add(now, self.jid)
+        next_queue.depends.add(now, self.jid)
         redis.call('hset', QlessJob.ns .. self.jid, 'state', 'depends')
         if delay > 0 then
-          queue_obj.depends.add(now, self.jid)
+          next_queue.depends.add(now, self.jid)
           redis.call('hset', QlessJob.ns .. self.jid, 'scheduled', now + delay)
         end
         return 'depends'
       else
-        queue_obj.work.add(now, priority, self.jid)
+        next_queue.work.add(now, priority, self.jid)
         return 'waiting'
       end
     end
   else
     Qless.publish('log', cjson.encode({
-      jid   = self.jid,
+      jid = self.jid,
       event = 'completed',
-      queue = queue
+      queue = queue_name,
     }))
 
     redis.call('hmset', QlessJob.ns .. self.jid,
       'state', 'complete',
       'worker', '',
       'failure', '{}',
       'queue', '',
@@ -554,42 +555,42 @@
 
     count = tonumber(count or 50000)
     time  = tonumber(time  or 7 * 24 * 60 * 60)
 
     redis.call('zadd', 'ql:completed', now, self.jid)
 
     local jids = redis.call('zrangebyscore', 'ql:completed', 0, now - time)
-    for index, jid in ipairs(jids) do
+    for _, jid in ipairs(jids) do
       Qless.job(jid):delete()
     end
 
     redis.call('zremrangebyscore', 'ql:completed', 0, now - time)
 
     jids = redis.call('zrange', 'ql:completed', 0, (-1-count))
-    for index, jid in ipairs(jids) do
+    for _, jid in ipairs(jids) do
       Qless.job(jid):delete()
     end
     redis.call('zremrangebyrank', 'ql:completed', 0, (-1-count))
 
-    for i, j in ipairs(redis.call(
+    for _, j in ipairs(redis.call(
       'smembers', QlessJob.ns .. self.jid .. '-dependents')) do
       redis.call('srem', QlessJob.ns .. j .. '-dependencies', self.jid)
       if redis.call(
         'scard', QlessJob.ns .. j .. '-dependencies') == 0 then
-        local q, p, scheduled = unpack(
+        local other_queue_name, priority, scheduled = unpack(
           redis.call('hmget', QlessJob.ns .. j, 'queue', 'priority', 'scheduled'))
-        if q then
-          local queue = Qless.queue(q)
-          queue.depends.remove(j)
+        if other_queue_name then
+          local other_queue = Qless.queue(other_queue_name)
+          other_queue.depends.remove(j)
           if scheduled then
-            queue.scheduled.add(scheduled, j)
+            other_queue.scheduled.add(scheduled, j)
             redis.call('hset', QlessJob.ns .. j, 'state', 'scheduled')
             redis.call('hdel', QlessJob.ns .. j, 'scheduled')
           else
-            queue.work.add(now, p, j)
+            other_queue.work.add(now, priority, j)
             redis.call('hset', QlessJob.ns .. j, 'state', 'waiting')
           end
         end
       end
     end
 
     redis.call('del', QlessJob.ns .. self.jid .. '-dependents')
@@ -605,46 +606,46 @@
 
   local bin = now - (now % 86400)
 
   if data then
     data = cjson.decode(data)
   end
 
-  local queue, state, oldworker = unpack(redis.call(
+  local queue_name, state, oldworker = unpack(redis.call(
     'hmget', QlessJob.ns .. self.jid, 'queue', 'state', 'worker'))
 
   if not state then
     error('Fail(): Job does not exist')
   elseif state ~= 'running' then
     error('Fail(): Job not currently running: ' .. state)
   elseif worker ~= oldworker then
     error('Fail(): Job running with another worker: ' .. oldworker)
   end
 
   Qless.publish('log', cjson.encode({
-    jid     = self.jid,
-    event   = 'failed',
-    worker  = worker,
-    group   = group,
-    message = message
+    jid = self.jid,
+    event = 'failed',
+    worker = worker,
+    group = group,
+    message = message,
   }))
 
   if redis.call('zscore', 'ql:tracked', self.jid) ~= false then
     Qless.publish('failed', self.jid)
   end
 
   redis.call('zrem', 'ql:w:' .. worker .. ':jobs', self.jid)
 
   self:history(now, 'failed', {worker = worker, group = group})
 
-  redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue, 'failures', 1)
-  redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue, 'failed'  , 1)
+  redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue_name, 'failures', 1)
+  redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue_name, 'failed'  , 1)
 
-  local queue_obj = Qless.queue(queue)
-  queue_obj:remove_job(self.jid)
+  local queue = Qless.queue(queue_name)
+  queue:remove_job(self.jid)
 
   if data then
     redis.call('hset', QlessJob.ns .. self.jid, 'data', cjson.encode(data))
   end
 
   redis.call('hmset', QlessJob.ns .. self.jid,
     'state', 'failed',
@@ -662,21 +663,21 @@
   redis.call('sadd', 'ql:failures', group)
   redis.call('lpush', 'ql:f:' .. group, self.jid)
 
 
   return self.jid
 end
 
-function QlessJob:retry(now, queue, worker, delay, group, message)
-  assert(queue , 'Retry(): Arg "queue" missing')
+function QlessJob:retry(now, queue_name, worker, delay, group, message)
+  assert(queue_name , 'Retry(): Arg "queue_name" missing')
   assert(worker, 'Retry(): Arg "worker" missing')
   delay = assert(tonumber(delay or 0),
     'Retry(): Arg "delay" not a number: ' .. tostring(delay))
 
-  local oldqueue, state, retries, oldworker, priority, failure = unpack(
+  local old_queue_name, state, retries, oldworker, priority, failure = unpack(
     redis.call('hmget', QlessJob.ns .. self.jid, 'queue', 'state',
       'retries', 'worker', 'priority', 'failure'))
 
   if oldworker == false then
     error('Retry(): Job does not exist')
   elseif state ~= 'running' then
     error('Retry(): Job is not currently running: ' .. state)
@@ -684,22 +685,22 @@
     error('Retry(): Job has been given to another worker: ' .. oldworker)
   end
 
   local remaining = tonumber(redis.call(
     'hincrby', QlessJob.ns .. self.jid, 'remaining', -1))
   redis.call('hdel', QlessJob.ns .. self.jid, 'grace')
 
-  Qless.queue(oldqueue).locks.remove(self.jid)
+  Qless.queue(old_queue_name).locks.remove(self.jid)
 
   self:throttles_release(now)
 
   redis.call('zrem', 'ql:w:' .. worker .. ':jobs', self.jid)
 
   if remaining < 0 then
-    local group = group or 'failed-retries-' .. queue
+    local group = group or 'failed-retries-' .. queue_name
     self:history(now, 'failed', {['group'] = group})
 
     redis.call('hmset', QlessJob.ns .. self.jid, 'state', 'failed',
       'worker', '',
       'expires', '')
     if group ~= nil and message ~= nil then
       redis.call('hset', QlessJob.ns .. self.jid,
@@ -711,32 +712,32 @@
         })
       )
     else
       redis.call('hset', QlessJob.ns .. self.jid,
       'failure', cjson.encode({
         ['group']   = group,
         ['message'] =
-          'Job exhausted retries in queue "' .. oldqueue .. '"',
+          'Job exhausted retries in queue "' .. old_queue_name .. '"',
         ['when']    = now,
         ['worker']  = unpack(self:data('worker'))
       }))
     end
 
     redis.call('sadd', 'ql:failures', group)
     redis.call('lpush', 'ql:f:' .. group, self.jid)
     local bin = now - (now % 86400)
-    redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue, 'failures', 1)
-    redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue, 'failed'  , 1)
+    redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue_name, 'failures', 1)
+    redis.call('hincrby', 'ql:s:stats:' .. bin .. ':' .. queue_name, 'failed'  , 1)
   else
-    local queue_obj = Qless.queue(queue)
+    local queue = Qless.queue(queue_name)
     if delay > 0 then
-      queue_obj.scheduled.add(now + delay, self.jid)
+      queue.scheduled.add(now + delay, self.jid)
       redis.call('hset', QlessJob.ns .. self.jid, 'state', 'scheduled')
     else
-      queue_obj.work.add(now, priority, self.jid)
+      queue.work.add(now, priority, self.jid)
       redis.call('hset', QlessJob.ns .. self.jid, 'state', 'waiting')
     end
 
     if group ~= nil and message ~= nil then
       redis.call('hset', QlessJob.ns .. self.jid,
         'failure', cjson.encode({
           ['group']   = group,
@@ -756,52 +757,52 @@
   local state = redis.call('hget', QlessJob.ns .. self.jid, 'state')
   if state ~= 'depends' then
     error('Depends(): Job ' .. self.jid ..
       ' not in the depends state: ' .. tostring(state))
   end
 
   if command == 'on' then
-    for i, j in ipairs(arg) do
+    for _, j in ipairs(arg) do
       local state = redis.call('hget', QlessJob.ns .. j, 'state')
       if (state and state ~= 'complete') then
         redis.call(
           'sadd', QlessJob.ns .. j .. '-dependents'  , self.jid)
         redis.call(
           'sadd', QlessJob.ns .. self.jid .. '-dependencies', j)
       end
     end
     return true
   elseif command == 'off' then
     if arg[1] == 'all' then
-      for i, j in ipairs(redis.call(
+      for _, j in ipairs(redis.call(
         'smembers', QlessJob.ns .. self.jid .. '-dependencies')) do
         redis.call('srem', QlessJob.ns .. j .. '-dependents', self.jid)
       end
       redis.call('del', QlessJob.ns .. self.jid .. '-dependencies')
-      local q, p = unpack(redis.call(
+      local queue_name, priority = unpack(redis.call(
         'hmget', QlessJob.ns .. self.jid, 'queue', 'priority'))
-      if q then
-        local queue_obj = Qless.queue(q)
-        queue_obj.depends.remove(self.jid)
-        queue_obj.work.add(now, p, self.jid)
+      if queue_name then
+        local queue = Qless.queue(queue_name)
+        queue.depends.remove(self.jid)
+        queue.work.add(now, priority, self.jid)
         redis.call('hset', QlessJob.ns .. self.jid, 'state', 'waiting')
       end
     else
-      for i, j in ipairs(arg) do
+      for _, j in ipairs(arg) do
         redis.call('srem', QlessJob.ns .. j .. '-dependents', self.jid)
         redis.call(
           'srem', QlessJob.ns .. self.jid .. '-dependencies', j)
         if redis.call('scard',
           QlessJob.ns .. self.jid .. '-dependencies') == 0 then
-          local q, p = unpack(redis.call(
+          local queue_name, priority = unpack(redis.call(
             'hmget', QlessJob.ns .. self.jid, 'queue', 'priority'))
-          if q then
-            local queue_obj = Qless.queue(q)
-            queue_obj.depends.remove(self.jid)
-            queue_obj.work.add(now, p, self.jid)
+          if queue_name then
+            local queue = Qless.queue(queue_name)
+            queue.depends.remove(self.jid)
+            queue.work.add(now, priority, self.jid)
             redis.call('hset',
               QlessJob.ns .. self.jid, 'state', 'waiting')
           end
         end
       end
     end
     return true
@@ -809,17 +810,17 @@
     error('Depends(): Argument "command" must be "on" or "off"')
   end
 end
 
 function QlessJob:heartbeat(now, worker, data)
   assert(worker, 'Heatbeat(): Arg "worker" missing')
 
-  local queue = redis.call('hget', QlessJob.ns .. self.jid, 'queue') or ''
+  local queue_name = redis.call('hget', QlessJob.ns .. self.jid, 'queue') or ''
   local expires = now + tonumber(
-    Qless.config.get(queue .. '-heartbeat') or
+    Qless.config.get(queue_name .. '-heartbeat') or
     Qless.config.get('heartbeat', 60))
 
   if data then
     data = cjson.decode(data)
   end
 
   local job_worker, state = unpack(
@@ -849,25 +850,25 @@
 end
 
 function QlessJob:priority(priority)
   priority = assert(tonumber(priority),
     'Priority(): Arg "priority" missing or not a number: ' ..
     tostring(priority))
 
-  local queue = redis.call('hget', QlessJob.ns .. self.jid, 'queue')
+  local queue_name = redis.call('hget', QlessJob.ns .. self.jid, 'queue')
 
-  if queue == nil then
+  if queue_name == nil then
     error('Priority(): Job ' .. self.jid .. ' does not exist')
-  elseif queue == '' then
+  elseif queue_name == '' then
     redis.call('hset', QlessJob.ns .. self.jid, 'priority', priority)
     return priority
   else
-    local queue_obj = Qless.queue(queue)
-    if queue_obj.work.score(self.jid) then
-      queue_obj.work.add(0, priority, self.jid)
+    local queue = Qless.queue(queue_name)
+    if queue.work.score(self.jid) then
+      queue.work.add(0, priority, self.jid)
     end
     redis.call('hset', QlessJob.ns .. self.jid, 'priority', priority)
     return priority
   end
 end
 
 function QlessJob:update(data)
@@ -893,17 +894,17 @@
 
     self:throttles_release(now)
 
     queue.work.add(now, math.huge, self.jid)
     redis.call('hmset', QlessJob.ns .. self.jid,
       'state', 'stalled', 'expires', 0)
     local encoded = cjson.encode({
-      jid    = self.jid,
-      event  = 'lock_lost',
-      worker = worker
+      jid = self.jid,
+      event = 'lock_lost',
+      worker = worker,
     })
     Qless.publish('w:' .. worker, encoded)
     Qless.publish('log', encoded)
     return queue_name
   end
 end
 
@@ -911,15 +912,15 @@
   return redis.call('exists', QlessJob.ns .. self.jid) == 1
 end
 
 function QlessJob:history(now, what, item)
   local history = redis.call('hget', QlessJob.ns .. self.jid, 'history')
   if history then
     history = cjson.decode(history)
-    for i, value in ipairs(history) do
+    for _, value in ipairs(history) do
       redis.call('rpush', QlessJob.ns .. self.jid .. '-history',
         cjson.encode({math.floor(value.put), 'put', {q = value.q}}))
 
       if value.popped then
         redis.call('rpush', QlessJob.ns .. self.jid .. '-history',
           cjson.encode({math.floor(value.popped), 'popped',
             {worker = value.worker}}))
@@ -938,15 +939,15 @@
       end
     end
     redis.call('hdel', QlessJob.ns .. self.jid, 'history')
   end
 
   if what == nil then
     local response = {}
-    for i, value in ipairs(redis.call('lrange',
+    for _, value in ipairs(redis.call('lrange',
       QlessJob.ns .. self.jid .. '-history', 0, -1)) do
       value = cjson.decode(value)
       local dict = value[3] or {}
       dict['when'] = value[1]
       dict['what'] = value[2]
       table.insert(response, dict)
     end
@@ -1013,15 +1014,15 @@
 
   return self._throttles
 end
 
 function QlessJob:delete()
   local tags = redis.call('hget', QlessJob.ns .. self.jid, 'tags') or '[]'
   tags = cjson.decode(tags)
-  for i, tag in ipairs(tags) do
+  for _, tag in ipairs(tags) do
     self:remove_tag(tag)
   end
   redis.call('del', QlessJob.ns .. self.jid)
   redis.call('del', QlessJob.ns .. self.jid .. '-history')
   redis.call('del', QlessJob.ns .. self.jid .. '-dependencies')
 end
 
@@ -1046,24 +1047,19 @@
 function Qless.queue(name)
   assert(name, 'Queue(): no queue name provided')
   local queue = {}
   setmetatable(queue, QlessQueue)
   queue.name = name
 
   queue.work = {
-    peek = function(count)
-      if count == 0 then
+    peek = function(offset, count)
+      if count <= 0 then
         return {}
       end
-      local jids = {}
-      for index, jid in ipairs(redis.call(
-        'zrevrange', queue:prefix('work'), 0, count - 1)) do
-        table.insert(jids, jid)
-      end
-      return jids
+      return redis.call('zrevrange', queue:prefix('work'), offset, offset + count - 1)
     end, remove = function(...)
       if #arg > 0 then
         return redis.call('zrem', queue:prefix('work'), unpack(arg))
       end
     end, add = function(now, priority, jid)
       return redis.call('zadd',
         queue:prefix('work'), priority - (now / 10000000000), jid)
@@ -1113,16 +1109,16 @@
     end
   }
 
 
   queue.throttled = {
     length = function()
       return (redis.call('zcard', queue:prefix('throttled')) or 0)
-    end, peek = function(now, min, max)
-      return redis.call('zrange', queue:prefix('throttled'), min, max)
+    end, peek = function(now, offset, count)
+      return redis.call('zrange', queue:prefix('throttled'), offset, offset + count - 1)
     end, add = function(...)
       if #arg > 0 then
         redis.call('zadd', queue:prefix('throttled'), unpack(arg))
       end
     end, remove = function(...)
       if #arg > 0 then
         return redis.call('zrem', queue:prefix('throttled'), unpack(arg))
@@ -1170,23 +1166,23 @@
     end
   }
   return queue
 end
 
 function QlessQueue:prefix(group)
   if group then
-    return QlessQueue.ns..self.name..'-'..group
+    return QlessQueue.ns .. self.name .. '-' .. group
   else
-    return QlessQueue.ns..self.name
+    return QlessQueue.ns .. self.name
   end
 end
 
 function QlessQueue:stats(now, date)
   date = assert(tonumber(date),
-    'Stats(): Arg "date" missing or not a number: '.. (date or 'nil'))
+    'Stats(): Arg "date" missing or not a number: ' .. (date or 'nil'))
 
   local bin = date - (date % 86400)
 
   local histokeys = {
     's0','s1','s2','s3','s4','s5','s6','s7','s8','s9','s10','s11','s12','s13','s14','s15','s16','s17','s18','s19','s20','s21','s22','s23','s24','s25','s26','s27','s28','s29','s30','s31','s32','s33','s34','s35','s36','s37','s38','s39','s40','s41','s42','s43','s44','s45','s46','s47','s48','s49','s50','s51','s52','s53','s54','s55','s56','s57','s58','s59',
     'm1','m2','m3','m4','m5','m6','m7','m8','m9','m10','m11','m12','m13','m14','m15','m16','m17','m18','m19','m20','m21','m22','m23','m24','m25','m26','m27','m28','m29','m30','m31','m32','m33','m34','m35','m36','m37','m38','m39','m40','m41','m42','m43','m44','m45','m46','m47','m48','m49','m50','m51','m52','m53','m54','m55','m56','m57','m58','m59',
     'h1','h2','h3','h4','h5','h6','h7','h8','h9','h10','h11','h12','h13','h14','h15','h16','h17','h18','h19','h20','h21','h22','h23',
@@ -1214,15 +1210,15 @@
         results.std = math.sqrt(vk / (count - 1))
       else
         results.std = 0
       end
     end
 
     local histogram = redis.call('hmget', key, unpack(histokeys))
-    for i=1,#histokeys do
+    for i=1, #histokeys do
       table.insert(results.histogram, tonumber(histogram[i]) or 0)
     end
     return results
   end
 
   local retries, failed, failures = unpack(redis.call('hmget', 'ql:s:stats:' .. bin .. ':' .. self.name, 'retries', 'failed', 'failures'))
   return {
@@ -1230,27 +1226,46 @@
     failed   = tonumber(failed   or 0),
     failures = tonumber(failures or 0),
     wait     = mkstats('wait', bin, self.name),
     run      = mkstats('run' , bin, self.name)
   }
 end
 
-function QlessQueue:peek(now, count)
+function QlessQueue:peek(now, offset, count)
+  offset = assert(tonumber(offset),
+    'Peek(): Arg "offset" missing or not a number: ' .. tostring(offset))
+
   count = assert(tonumber(count),
     'Peek(): Arg "count" missing or not a number: ' .. tostring(count))
 
-  local jids = self.locks.expired(now, 0, count)
+  if count <= 0 then
+    return {}
+  end
+
+  local count_with_offset = offset + count
 
-  self:check_recurring(now, count - #jids)
+  local jids = self.locks.expired(now, 0, count_with_offset)
 
-  self:check_scheduled(now, count - #jids)
+  local remaining_capacity = count_with_offset - #jids
 
-  table_extend(jids, self.work.peek(count - #jids))
+  self:check_recurring(now, remaining_capacity)
 
-  return jids
+  self:check_scheduled(now, remaining_capacity)
+
+  if offset > #jids then
+    return self.work.peek(offset - #jids, count)
+  else
+    table_extend(jids, self.work.peek(0, remaining_capacity))
+
+    if #jids < offset then
+      return {}
+    end
+
+    return {unpack(jids, offset + 1, count_with_offset)}
+  end
 end
 
 function QlessQueue:paused()
   return redis.call('sismember', 'ql:paused_queues', self.name) == 1
 end
 
 function QlessQueue.pause(now, ...)
@@ -1271,15 +1286,15 @@
   end
 
   redis.call('zadd', 'ql:workers', now, worker)
 
   local dead_jids = self:invalidate_locks(now, count) or {}
   local popped = {}
 
-  for index, jid in ipairs(dead_jids) do
+  for _, jid in ipairs(dead_jids) do
     local success = self:pop_job(now, worker, Qless.job(jid))
     if success then
       table.insert(popped, jid)
     end
   end
 
   if not Qless.throttle(QlessQueue.ns .. self.name):available() then
@@ -1295,22 +1310,22 @@
   local pop_retry_limit = tonumber(
     Qless.config.get(self.name .. '-max-pop-retry') or
     Qless.config.get('max-pop-retry', 1)
   )
 
   while #popped < count and pop_retry_limit > 0 do
 
-    local jids = self.work.peek(count - #popped) or {}
+    local jids = self.work.peek(0, count - #popped) or {}
 
     if #jids == 0 then
       break
     end
 
 
-    for index, jid in ipairs(jids) do
+    for _, jid in ipairs(jids) do
       local job = Qless.job(jid)
       if job:throttles_acquire(now) then
         local success = self:pop_job(now, worker, job)
         if success then
           table.insert(popped, jid)
         end
       else
@@ -1462,16 +1477,16 @@
 
   job:history(now, 'put', {q = self.name})
 
   if oldqueue then
     local queue_obj = Qless.queue(oldqueue)
     queue_obj:remove_job(jid)
     local old_qid = QlessQueue.ns .. oldqueue
-    for index, tname in ipairs(throttles) do
-      if tname == old_qid then
+    for index, throttle_name in ipairs(throttles) do
+      if throttle_name == old_qid then
         table.remove(throttles, index)
       end
     end
   end
 
   if oldworker and oldworker ~= '' then
     redis.call('zrem', 'ql:w:' .. oldworker .. ':jobs', jid)
@@ -1486,15 +1501,15 @@
     end
   end
 
   if state == 'complete' then
     redis.call('zrem', 'ql:completed', jid)
   end
 
-  for i, tag in ipairs(tags) do
+  for _, tag in ipairs(tags) do
     Qless.job(jid):insert_tag(now, tag)
   end
 
   if state == 'failed' then
     failure = cjson.decode(failure)
     redis.call('lrem', 'ql:f:' .. failure.group, 0, jid)
     if redis.call('llen', 'ql:f:' .. failure.group) == 0 then
@@ -1520,15 +1535,15 @@
     'remaining', retries,
     'time'     , string.format("%.20f", now),
     'throttles', cjson.encode(throttles)
   }
 
   redis.call('hmset', QlessJob.ns .. jid, unpack(data))
 
-  for i, j in ipairs(depends) do
+  for _, j in ipairs(depends) do
     local state = redis.call('hget', QlessJob.ns .. j, 'state')
     if (state and state ~= 'complete') then
       redis.call('sadd', QlessJob.ns .. j .. '-dependents'  , jid)
       redis.call('sadd', QlessJob.ns .. jid .. '-dependencies', j)
     end
   end
 
@@ -1568,15 +1583,15 @@
   assert(group, 'Unfail(): Arg "group" missing')
   count = assert(tonumber(count or 25),
     'Unfail(): Arg "count" not a number: ' .. tostring(count))
 
   local jids = redis.call('lrange', 'ql:f:' .. group, -count, -1)
 
   local toinsert = {}
-  for index, jid in ipairs(jids) do
+  for _, jid in ipairs(jids) do
     local job = Qless.job(jid)
     local data = job:data()
     job:history(now, 'put', {q = self.name})
     redis.call('hmset', QlessJob.ns .. data.jid,
       'state'    , 'waiting',
       'worker'   , '',
       'expires'  , 0,
@@ -1634,16 +1649,16 @@
     count = count or 0
 
     local throttles = options['throttles'] or {}
 
     if old_queue then
       Qless.queue(old_queue).recurring.remove(jid)
 
-      for index, tname in ipairs(throttles) do
-        if tname == old_queue then
+      for index, throttle_name in ipairs(throttles) do
+        if throttle_name == old_queue then
           table.remove(throttles, index)
         end
       end
     end
 
     table.insert(throttles, QlessQueue.ns .. self.name)
 
@@ -1682,17 +1697,20 @@
   self.locks.remove(jid)
   self.throttled.remove(jid)
   self.depends.remove(jid)
   self.scheduled.remove(jid)
 end
 
 function QlessQueue:check_recurring(now, count)
+  if count <= 0 then
+    return
+  end
   local moved = 0
   local r = self.recurring.peek(now, 0, count)
-  for index, jid in ipairs(r) do
+  for _, jid in ipairs(r) do
     local r = redis.call('hmget', 'ql:r:' .. jid, 'klass', 'data', 'priority',
         'tags', 'retries', 'interval', 'backlog', 'throttles')
     local klass, data, priority, tags, retries, interval, backlog, throttles = unpack(
       redis.call('hmget', 'ql:r:' .. jid, 'klass', 'data', 'priority',
         'tags', 'retries', 'interval', 'backlog', 'throttles'))
     local _tags = cjson.decode(tags)
     local score = math.floor(tonumber(self.recurring.score(jid)))
@@ -1710,15 +1728,15 @@
 
     while (score <= now) and (moved < count) do
       local count = redis.call('hincrby', 'ql:r:' .. jid, 'count', 1)
       moved = moved + 1
 
       local child_jid = jid .. '-' .. count
 
-      for i, tag in ipairs(_tags) do
+      for _, tag in ipairs(_tags) do
         Qless.job(child_jid):insert_tag(now, tag)
       end
 
       redis.call('hmset', QlessJob.ns .. child_jid,
         'jid'      , child_jid,
         'klass'    , klass,
         'data'     , data,
@@ -1741,28 +1759,31 @@
       score = score + interval
       self.recurring.add(score, jid)
     end
   end
 end
 
 function QlessQueue:check_scheduled(now, count)
+  if count <= 0 then
+    return
+  end
   local scheduled = self.scheduled.ready(now, 0, count)
-  for index, jid in ipairs(scheduled) do
+  for _, jid in ipairs(scheduled) do
     local priority = tonumber(
       redis.call('hget', QlessJob.ns .. jid, 'priority') or 0)
     self.work.add(now, priority, jid)
     self.scheduled.remove(jid)
 
     redis.call('hset', QlessJob.ns .. jid, 'state', 'waiting')
   end
 end
 
 function QlessQueue:invalidate_locks(now, count)
   local jids = {}
-  for index, jid in ipairs(self.locks.expired(now, 0, count)) do
+  for _, jid in ipairs(self.locks.expired(now, 0, count)) do
     local worker, failure = unpack(
       redis.call('hmget', QlessJob.ns .. jid, 'worker', 'failure'))
     redis.call('zrem', 'ql:w:' .. worker .. ':jobs', jid)
 
     local grace_period = tonumber(Qless.config.get('grace-period'))
 
     local courtesy_sent = tonumber(
@@ -1782,15 +1803,15 @@
       end
       Qless.job(jid):history(now, 'timed-out')
       redis.call('hset', QlessJob.ns .. jid, 'grace', 1)
 
       local encoded = cjson.encode({
         jid    = jid,
         event  = 'lock_lost',
-        worker = worker
+        worker = worker,
       })
       Qless.publish('w:' .. worker, encoded)
       Qless.publish('log', encoded)
       self.locks.add(now + grace_period, jid)
 
       local bin = now - (now % 86400)
       redis.call('hincrby',
@@ -1876,29 +1897,29 @@
       depends   = queue.depends.length(),
       recurring = queue.recurring.length(),
       paused    = queue:paused()
     }
   else
     local queues = redis.call('zrange', 'ql:queues', 0, -1)
     local response = {}
-    for index, qname in ipairs(queues) do
+    for _, qname in ipairs(queues) do
       table.insert(response, QlessQueue.counts(now, qname))
     end
     return response
   end
 end
 function QlessRecurringJob:data()
   local job = redis.call(
     'hmget', 'ql:r:' .. self.jid, 'jid', 'klass', 'state', 'queue',
     'priority', 'interval', 'retries', 'count', 'data', 'tags', 'backlog', 'throttles')
-  
+
   if not job[1] then
     return nil
   end
-  
+
   return {
     jid          = job[1],
     klass        = job[2],
     state        = job[3],
     queue        = job[4],
     priority     = tonumber(job[5]),
     interval     = tonumber(job[6]),
@@ -1934,16 +1955,16 @@
       elseif key == 'queue' then
         local old_queue_name = redis.call('hget', 'ql:r:' .. self.jid, 'queue')
         local queue_obj = Qless.queue(old_queue_name)
         local score = queue_obj.recurring.score(self.jid)
 
         queue_obj.recurring.remove(self.jid)
         local throttles = cjson.decode(redis.call('hget', 'ql:r:' .. self.jid, 'throttles') or '{}')
-        for index, tname in ipairs(throttles) do
-          if tname == QlessQueue.ns .. old_queue_name then
+        for index, throttle_name in ipairs(throttles) do
+          if throttle_name == QlessQueue.ns .. old_queue_name then
             table.remove(throttles, index)
           end
         end
 
 
         table.insert(throttles, QlessQueue.ns .. value)
         redis.call('hset', 'ql:r:' .. self.jid, 'throttles', cjson.encode(throttles))
@@ -1971,35 +1992,35 @@
 end
 
 function QlessRecurringJob:tag(...)
   local tags = redis.call('hget', 'ql:r:' .. self.jid, 'tags')
   if tags then
     tags = cjson.decode(tags)
     local _tags = {}
-    for i,v in ipairs(tags) do _tags[v] = true end
-    
-    for i=1,#arg do if _tags[arg[i]] == nil then table.insert(tags, arg[i]) end end
-    
+    for _, v in ipairs(tags) do _tags[v] = true end
+
+    for i=1, #arg do if _tags[arg[i]] == nil then table.insert(tags, arg[i]) end end
+
     tags = cjson.encode(tags)
     redis.call('hset', 'ql:r:' .. self.jid, 'tags', tags)
     return tags
   else
     error('Tag(): Job ' .. self.jid .. ' does not exist')
   end
 end
 
 function QlessRecurringJob:untag(...)
   local tags = redis.call('hget', 'ql:r:' .. self.jid, 'tags')
   if tags then
     tags = cjson.decode(tags)
-    local _tags    = {}
-    for i,v in ipairs(tags) do _tags[v] = true end
-    for i = 1,#arg do _tags[arg[i]] = nil end
+    local _tags = {}
+    for _, v in ipairs(tags) do _tags[v] = true end
+    for i = 1, #arg do _tags[arg[i]] = nil end
     local results = {}
-    for i, tag in ipairs(tags) do if _tags[tag] then table.insert(results, tag) end end
+    for _, tag in ipairs(tags) do if _tags[tag] then table.insert(results, tag) end end
     tags = cjson.encode(results)
     redis.call('hset', 'ql:r:' .. self.jid, 'tags', tags)
     return tags
   else
     error('Untag(): Job ' .. self.jid .. ' does not exist')
   end
 end
@@ -2018,29 +2039,29 @@
   redis.call('zrem', 'ql:workers', unpack(arg))
 end
 
 function QlessWorker.counts(now, worker)
   local interval = tonumber(Qless.config.get('max-worker-age', 86400))
 
   local workers  = redis.call('zrangebyscore', 'ql:workers', 0, now - interval)
-  for index, worker in ipairs(workers) do
+  for _, worker in ipairs(workers) do
     redis.call('del', 'ql:w:' .. worker .. ':jobs')
   end
 
   redis.call('zremrangebyscore', 'ql:workers', 0, now - interval)
 
   if worker then
     return {
       jobs    = redis.call('zrevrangebyscore', 'ql:w:' .. worker .. ':jobs', now + 8640000, now),
       stalled = redis.call('zrevrangebyscore', 'ql:w:' .. worker .. ':jobs', now, 0)
     }
   else
     local response = {}
     local workers = redis.call('zrevrange', 'ql:workers', 0, -1)
-    for index, worker in ipairs(workers) do
+    for _, worker in ipairs(workers) do
       table.insert(response, {
         name    = worker,
         jobs    = redis.call('zcount', 'ql:w:' .. worker .. ':jobs', now, now + 8640000),
         stalled = redis.call('zcount', 'ql:w:' .. worker .. ':jobs', 0, now)
       })
     end
     return response
@@ -2130,15 +2151,15 @@
     return nil
   end
   return cjson.encode(data)
 end
 
 function QlessAPI.multiget(now, ...)
   local results = {}
-  for i, jid in ipairs(arg) do
+  for _, jid in ipairs(arg) do
     table.insert(results, Qless.job(jid):data())
   end
   return cjson.encode(results)
 end
 
 QlessAPI['config.get'] = function(now, key)
   if not key then
@@ -2217,27 +2238,27 @@
   end
 
   local job = Qless.job(jid)
   assert(job:exists(), 'Log(): Job ' .. jid .. ' does not exist')
   job:history(now, message, data)
 end
 
-QlessAPI.peek = function(now, queue, count)
-  local jids = Qless.queue(queue):peek(now, count)
+QlessAPI.peek = function(now, queue, offset, count)
+  local jids = Qless.queue(queue):peek(now, offset, count)
   local response = {}
-  for i, jid in ipairs(jids) do
+  for _, jid in ipairs(jids) do
     table.insert(response, Qless.job(jid):data())
   end
   return cjson.encode(response)
 end
 
 QlessAPI.pop = function(now, queue, worker, count)
   local jids = Qless.queue(queue):pop(now, worker, count)
   local response = {}
-  for i, jid in ipairs(jids) do
+  for _, jid in ipairs(jids) do
     table.insert(response, Qless.job(jid):data())
   end
   return cjson.encode(response)
 end
 
 QlessAPI.pause = function(now, ...)
   return QlessQueue.pause(now, unpack(arg))
```

### Comparing `reqless-0.13.2/reqless/profile.py` & `reqless-0.13.3/reqless/profile.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/qmore/client.py` & `reqless-0.13.3/reqless/qmore/client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/queue.py` & `reqless-0.13.3/reqless/queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -227,21 +227,23 @@
             )
         ]
         if count is None:
             return (len(results) and results[0]) or None
         return results
 
     def peek(
-        self, count: Optional[int] = None
+        self, offset: Optional[int] = None, count: Optional[int] = None
     ) -> Union[AbstractJob, List[AbstractJob], None]:
         """Similar to the pop command, except that it merely peeks at the next
         items"""
+        _offset = offset or 0
+        _count = count or 1
         results: List[AbstractJob] = [
             Job(self.client, **rec)
-            for rec in json.loads(self.client("peek", self.name, count or 1))
+            for rec in json.loads(self.client("peek", self.name, _offset, _count))
         ]
         if count is None:
             return (len(results) and results[0]) or None
         return results
 
     def stats(self, date: Optional[str] = None) -> Dict:
         """Return the current statistics for a given queue on a given date.
```

### Comparing `reqless-0.13.2/reqless/queue_resolvers/__init__.py` & `reqless-0.13.3/reqless/queue_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py` & `reqless-0.13.3/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py` & `reqless-0.13.3/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/queue_resolvers/transforming_queue_resolver.py` & `reqless-0.13.3/reqless/queue_resolvers/transforming_queue_resolver.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/throttle.py` & `reqless-0.13.3/reqless/throttle.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/workers/forking.py` & `reqless-0.13.3/reqless/workers/forking.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/workers/greenlet.py` & `reqless-0.13.3/reqless/workers/greenlet.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/workers/serial.py` & `reqless-0.13.3/reqless/workers/serial.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/workers/util.py` & `reqless-0.13.3/reqless/workers/util.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless/workers/worker.py` & `reqless-0.13.3/reqless/workers/worker.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless.egg-info/PKG-INFO` & `reqless-0.13.3/reqless.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reqless
-Version: 0.13.2
+Version: 0.13.3
 Summary: Redis-based Queue Management
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/reqless-py
 Project-URL: Source, https://github.com/tdg5/reqless-py
 Project-URL: Tracker, https://github.com/tdg5/reqless-py/issues
 Keywords: job,qless,qmore,redis,reqless
@@ -20,15 +20,15 @@
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: decorator
 Requires-Dist: hiredis
 Requires-Dist: redis
 Requires-Dist: typing_extensions>=4.8.0
 Provides-Extra: dev
-Requires-Dist: black~=24.2.0; extra == "dev"
+Requires-Dist: black~=24.3; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
 Requires-Dist: flake8-pyproject~=1.2.3; extra == "dev"
 Requires-Dist: flake8~=7.0.0; extra == "dev"
 Requires-Dist: gevent~=24.2.1; extra == "dev"
 Requires-Dist: isort~=5.8.0; extra == "dev"
 Requires-Dist: mypy~=1.8.0; extra == "dev"
 Requires-Dist: pre-commit~=2.20.0; extra == "dev"
```

### Comparing `reqless-0.13.2/reqless.egg-info/SOURCES.txt` & `reqless-0.13.3/reqless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/common.py` & `reqless-0.13.3/reqless_test/common.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_client.py` & `reqless-0.13.3/reqless_test/test_client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_config.py` & `reqless-0.13.3/reqless_test/test_config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_events.py` & `reqless-0.13.3/reqless_test/test_events.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_forking.py` & `reqless-0.13.3/reqless_test/test_forking.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_greenlet.py` & `reqless-0.13.3/reqless_test/test_greenlet.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_importer.py` & `reqless-0.13.3/reqless_test/test_importer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_job.py` & `reqless-0.13.3/reqless_test/test_job.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_job_processor_api.py` & `reqless-0.13.3/reqless_test/test_job_processor_api.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_listener.py` & `reqless-0.13.3/reqless_test/test_listener.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_qmore_client.py` & `reqless-0.13.3/reqless_test/test_qmore_client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py` & `reqless-0.13.3/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py` & `reqless-0.13.3/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_queue.py` & `reqless-0.13.3/reqless_test/test_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,34 +55,34 @@
     def test_attribute_error(self) -> None:
         """Raises an attribute error if there is no attribute"""
         self.assertRaises(
             AttributeError,
             lambda: self.client.queues["foo"].foo,  # type: ignore[attr-defined]
         )
 
-    def test_multipop(self) -> None:
+    def test_pop_many(self) -> None:
         """Exposes multi-pop"""
         self.client.queues["foo"].put("reqless_test.common.NoopJob", "{}")
         self.client.queues["foo"].put("reqless_test.common.NoopJob", "{}")
         jobs = self.client.queues["foo"].pop(10)
         assert isinstance(jobs, List)
         self.assertEqual(len(jobs), 2)
 
     def test_peek(self) -> None:
         """Exposes queue peeking"""
         self.client.queues["foo"].put("reqless_test.common.NoopJob", "{}", jid="jid")
         job = self.client.queues["foo"].peek()
         assert job is not None and not isinstance(job, List)
         self.assertEqual(job.jid, "jid")
 
-    def test_multipeek(self) -> None:
+    def test_peek_many(self) -> None:
         """Exposes multi-peek"""
         self.client.queues["foo"].put("reqless_test.common.NoopJob", "{}")
         self.client.queues["foo"].put("reqless_test.common.NoopJob", "{}")
-        jobs = self.client.queues["foo"].peek(10)
+        jobs = self.client.queues["foo"].peek(count=10)
         assert isinstance(jobs, List)
         self.assertEqual(len(jobs), 2)
 
     def test_stats(self) -> None:
         """Exposes stats"""
         self.client.queues["foo"].stats()
```

### Comparing `reqless-0.13.2/reqless_test/test_serial.py` & `reqless-0.13.3/reqless_test/test_serial.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_transforming_queue_resolver.py` & `reqless-0.13.3/reqless_test/test_transforming_queue_resolver.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_worker.py` & `reqless-0.13.3/reqless_test/test_worker.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/reqless_test/test_worker_util.py` & `reqless-0.13.3/reqless_test/test_worker_util.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.2/requirements.txt` & `reqless-0.13.3/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 async-timeout==4.0.3
-black==24.2.0
+black==24.4.0
 build==1.0.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 charset-normalizer==3.3.2
 click==8.1.7
 coverage==7.4.4
```

