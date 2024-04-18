# Comparing `tmp/newrelic-9.8.0.tar.gz` & `tmp/newrelic-9.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic-9.8.0.tar", last modified: Wed Mar 27 23:08:43 2024, max compression
+gzip compressed data, was "newrelic-9.9.0.tar", last modified: Thu Apr 18 22:50:51 2024, max compression
```

## Comparing `newrelic-9.8.0.tar` & `newrelic-9.9.0.tar`

### file list

```diff
@@ -1,1364 +1,1368 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.611113 newrelic-9.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.407110 newrelic-9.8.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-27 23:08:38.000000 newrelic-9.8.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-27 23:08:38.000000 newrelic-9.8.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.407110 newrelic-9.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.411110 newrelic-9.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/ISSUE_TEMPLATE/troubleshooting.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.411110 newrelic-9.8.0/.github/containers/
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/containers/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/containers/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     1528 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/containers/install-python.sh
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/containers/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.411110 newrelic-9.8.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1268 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/scripts/retry.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.411110 newrelic-9.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/workflows/build-ci-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/workflows/deploy-python.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1186 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/workflows/get-envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/workflows/mega-linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)    29683 2024-03-27 23:08:38.000000 newrelic-9.8.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-27 23:08:38.000000 newrelic-9.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-27 23:08:38.000000 newrelic-9.8.0/.mega-linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-03-27 23:08:38.000000 newrelic-9.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-27 23:08:38.000000 newrelic-9.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-27 23:08:38.000000 newrelic-9.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-03-27 23:08:43.611113 newrelic-9.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-03-27 23:08:38.000000 newrelic-9.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-27 23:08:38.000000 newrelic-9.8.0/ROADMAP.md
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-27 23:08:38.000000 newrelic-9.8.0/THIRD_PARTY_NOTICES.md
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-27 23:08:38.000000 newrelic-9.8.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.411110 newrelic-9.8.0/newrelic/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.415110 newrelic-9.8.0/newrelic/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/debug_console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/generate_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/license_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/local_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/network_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/record_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/run_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/server_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/admin/validate_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.423110 newrelic-9.8.0/newrelic/api/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/application.py
--rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/asgi_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/background_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/cat_header_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/database_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/datastore_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/error_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/external_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/function_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/function_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/generator_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/graphql_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/html_insertion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/in_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/memcache_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/message_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/message_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/ml_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/object_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/out_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/post_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/pre_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/profile_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/solr_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/supportability.py
--rw-r--r--   0 runner    (1001) docker     (127)    26851 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/time_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    79389 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/transaction_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/web_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    25224 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/api/wsgi_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.423110 newrelic-9.8.0/newrelic/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/bootstrap/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.423110 newrelic-9.8.0/newrelic/common/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/_monotonic.c
--rw-r--r--   0 runner    (1001) docker     (127)    21725 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/agent_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/async_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/async_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    64813 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/certs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/coroutine.py
--rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/encoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/log_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/object_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/object_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/package_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/streaming_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13872 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/common/utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)   160561 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.431110 newrelic-9.8.0/newrelic/core/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/_thread_utilization.c
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/adaptive_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    32825 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    22340 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/agent_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/agent_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)    74275 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    45825 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/custom_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/database_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    29349 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/datastore_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/error_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/error_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/external_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/function_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/graphql_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/graphql_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/infinite_tracing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/infinite_tracing_v3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/infinite_tracing_v4_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/internal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/log_event_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/loop_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/memcache_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/message_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/node_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/otlp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16490 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/profile_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/root_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/rules_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/solr_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/stack_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    75777 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/stats_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/string_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/thread_utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15461 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/trace_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/core/transaction_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.431110 newrelic-9.8.0/newrelic/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.431110 newrelic-9.8.0/newrelic/extras/framework_django/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/extras/framework_django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.431110 newrelic-9.8.0/newrelic/extras/framework_django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/extras/framework_django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/extras/framework_django/templatetags/newrelic_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.451111 newrelic-9.8.0/newrelic/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_asgiref.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_cheroot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_cherrypy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_daphne.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_flup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_gevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_hypercorn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_meinheld.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_paste.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_uvicorn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_waitress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/adapter_wsgiref.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/application_celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/application_gearman.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/component_cornice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/component_djangorestframework.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/component_flask_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/component_graphqlserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/component_piston.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/component_sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/component_tastypie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/coroutines_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/coroutines_gevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_cx_oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_dbapi2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_ibm_db_dbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_oursql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_psycopg2cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_psycopg2ct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_pymssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_pymysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_pyodbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/database_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_aioredis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_aredis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_bmemcached.py
--rw-r--r--   0 runner    (1001) docker     (127)    21862 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18601 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_firestore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_pyelasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_pylibmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_pymemcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_pymongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_pysolr.py
--rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_solrpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/datastore_umemcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    33551 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_botocore.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_facepy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_feedparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_httplib2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_pywapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_thrift.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_urllib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_urllib2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/external_xmlrpclib.py
--rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_ariadne.py
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_bottle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_cherrypy.py
--rw-r--r--   0 runner    (1001) docker     (127)    42156 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_django_py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    15352 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_graphene.py
--rw-r--r--   0 runner    (1001) docker     (127)    18198 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_graphql_py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_pylons.py
--rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_strawberry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_web2py.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/framework_webpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/logger_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/logger_loguru.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/logger_structlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/memcache_memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/messagebroker_confluentkafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/messagebroker_kafkapython.py
--rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/messagebroker_pika.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/middleware_flask_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/middleware_weberror.py
--rw-r--r--   0 runner    (1001) docker     (127)    35117 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/mlmodel_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    41623 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/mlmodel_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/mlmodel_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/template_genshi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/template_jinja2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/hooks/template_mako.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.451111 newrelic-9.8.0/newrelic/network/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/network/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/network/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/newrelic.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.451111 newrelic-9.8.0/newrelic/packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/asgiref_compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.451111 newrelic-9.8.0/newrelic/packages/isort/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.455111 newrelic-9.8.0/newrelic/packages/isort/stdlibs/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/all.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/py2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/py27.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/py311.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/py36.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/py37.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/isort/stdlibs/py39.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.455111 newrelic-9.8.0/newrelic/packages/opentelemetry_proto/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/opentelemetry_proto/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/opentelemetry_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/opentelemetry_proto/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/opentelemetry_proto/logs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/opentelemetry_proto/metrics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/opentelemetry_proto/resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34549 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/six.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.455111 newrelic-9.8.0/newrelic/packages/urllib3/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    39128 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.459111 newrelic-9.8.0/newrelic/packages/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.459111 newrelic-9.8.0/newrelic/packages/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (127)    17055 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    34416 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.459111 newrelic-9.8.0/newrelic/packages/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.459111 newrelic-9.8.0/newrelic/packages/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)    34665 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/packages/six.py
--rw-r--r--   0 runner    (1001) docker     (127)    19786 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    30761 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.463111 newrelic-9.8.0/newrelic/packages/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    22003 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/urllib3/util/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.463111 newrelic-9.8.0/newrelic/packages/wrapt/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/wrapt/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/wrapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/wrapt/__wrapt__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96990 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/wrapt/_wrappers.c
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/wrapt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/wrapt/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/wrapt/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/wrapt/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/wrapt/weakrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/packages/wrapt/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.463111 newrelic-9.8.0/newrelic/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/samplers/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/samplers/data_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/samplers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/samplers/gc_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-27 23:08:38.000000 newrelic-9.8.0/newrelic/samplers/memory_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-27 23:08:43.000000 newrelic-9.8.0/newrelic/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.611113 newrelic-9.8.0/newrelic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-03-27 23:08:43.000000 newrelic-9.8.0/newrelic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    61517 2024-03-27 23:08:43.000000 newrelic-9.8.0/newrelic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 23:08:43.000000 newrelic-9.8.0/newrelic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-27 23:08:43.000000 newrelic-9.8.0/newrelic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 23:08:43.000000 newrelic-9.8.0/newrelic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-27 23:08:43.000000 newrelic-9.8.0/newrelic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-27 23:08:43.000000 newrelic-9.8.0/newrelic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-27 23:08:38.000000 newrelic-9.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.463111 newrelic-9.8.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/scripts/newrelic-admin
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-27 23:08:43.611113 newrelic-9.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-03-27 23:08:38.000000 newrelic-9.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.403110 newrelic-9.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.463111 newrelic-9.8.0/tests/adapter_asgiref/
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_asgiref/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_asgiref/test_context_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.467111 newrelic-9.8.0/tests/adapter_cheroot/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_cheroot/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_cheroot/test_wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.467111 newrelic-9.8.0/tests/adapter_daphne/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_daphne/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_daphne/test_daphne.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.467111 newrelic-9.8.0/tests/adapter_gevent/
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gevent/_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gevent/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gevent/test_patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gevent/test_pywsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.467111 newrelic-9.8.0/tests/adapter_gunicorn/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gunicorn/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gunicorn/asgi_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gunicorn/async_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gunicorn/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gunicorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gunicorn/test_aiohttp_app_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gunicorn/test_asgi_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gunicorn/test_gaiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_gunicorn/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.467111 newrelic-9.8.0/tests/adapter_hypercorn/
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_hypercorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_hypercorn/test_hypercorn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.467111 newrelic-9.8.0/tests/adapter_uvicorn/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_uvicorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_uvicorn/test_uvicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.467111 newrelic-9.8.0/tests/adapter_waitress/
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_waitress/_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_waitress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/adapter_waitress/test_wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.479111 newrelic-9.8.0/tests/agent_features/
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/_test_async_coroutine_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/_test_async_coroutine_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/_test_async_generator_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/_test_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_apdex_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    32375 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_asgi_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_asgi_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_asgi_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_asgi_w3c_trace_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_async_context_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_async_generator_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_async_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_async_wrapper_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    35683 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_attributes_in_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_background_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    34468 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_browser_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_collector_payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_coroutine_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_coroutine_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_custom_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_custom_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_datastore_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_dead_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_dimensional_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_error_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_error_group_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_event_loop_wait_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_exception_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_function_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    29623 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_high_security_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_ignore_expected_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_llm_token_count_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_log_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_logs_in_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_metric_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_ml_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_notice_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_priority_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_profile_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_record_llm_feedback_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_serverless_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_span_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_stack_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_supportability_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_synthetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_time_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_transaction_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_transaction_trace_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_w3c_trace_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_web_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_features/test_wsgi_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.479111 newrelic-9.8.0/tests/agent_streaming/
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_streaming/_test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_streaming/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17363 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_streaming/test_infinite_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_streaming/test_span_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_streaming/test_stream_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_streaming/test_streaming_rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.487111 newrelic-9.8.0/tests/agent_unittests/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/_test_import_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_agent_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)    20250 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_agent_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_check_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_connect_response_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_distributed_tracing_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_encoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_full_uri_payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)    32348 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_harvest_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    21008 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_import_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_infinite_trace_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_package_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_region_aware_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_sampler_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_serverless_mode_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_trace_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_utilization_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/agent_unittests/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.487111 newrelic-9.8.0/tests/application_celery/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/application_celery/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/application_celery/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/application_celery/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/application_celery/test_celery_max_tasks_per_child.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.487111 newrelic-9.8.0/tests/application_gearman/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/application_gearman/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/application_gearman/test_gearman.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.487111 newrelic-9.8.0/tests/component_djangorestframework/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_djangorestframework/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_djangorestframework/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_djangorestframework/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_djangorestframework/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_djangorestframework/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_djangorestframework/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.487111 newrelic-9.8.0/tests/component_flask_rest/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_flask_rest/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_flask_rest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_flask_rest/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.487111 newrelic-9.8.0/tests/component_graphqlserver/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_graphqlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_graphqlserver/_target_schema_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_graphqlserver/_test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_graphqlserver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_graphqlserver/test_graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.491111 newrelic-9.8.0/tests/component_tastypie/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_tastypie/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_tastypie/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_tastypie/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_tastypie/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_tastypie/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_tastypie/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/component_tastypie/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.491111 newrelic-9.8.0/tests/coroutines_asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/coroutines_asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/coroutines_asyncio/test_context_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.495112 newrelic-9.8.0/tests/cross_agent/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.495112 newrelic-9.8.0/tests/cross_agent/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/attribute_configuration.json
--rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/cat_map.json
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/collector_hostname.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.495112 newrelic-9.8.0/tests/cross_agent/fixtures/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/datastores/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/datastores/datastore_instances.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.495112 newrelic-9.8.0/tests/cross_agent/fixtures/distributed_tracing/
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/distributed_tracing/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    48250 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json
--rw-r--r--   0 runner    (1001) docker     (127)    58950 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/distributed_tracing/trace_context.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.499112 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/cases.json
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-0.9.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/empty.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/heroku.txt
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/invalid-length.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-lxc-container.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-no-container.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.10-no-container.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.503112 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/cases.json
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-20.10.16.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-24.0.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-too-long.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/empty.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-characters.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-length.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/labels.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.507112 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_auth.json
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/batch_get.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/batch_submit.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudformation_create.json
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudwatch_logs.json
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/codecommit.json
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cognito_sync.json
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis.json
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_analytics.json
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_apache.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_invoke.json
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/lex_appointment.json
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/lex_book_car.json
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/s3_put.json
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/scheduled_event.json
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/ses.json
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/smarthome_discovery.json
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/smarthome_turn_off.json
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/sns.json
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/sqs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.523112 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.query.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.explain.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.query.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.523112 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_1logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_2core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17027 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38341 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/malformed_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.527112 newrelic-9.8.0/tests/cross_agent/fixtures/proc_meminfo/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_meminfo/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_meminfo/malformed_file.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rules.json
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_cookie.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.531112 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/empty_head
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html
--rwxr-xr-x   0 runner    (1001) docker     (127)      852 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html
--rwxr-xr-x   0 runner    (1001) docker     (127)      958 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.539112 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.539112 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.543112 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/sql_parsing.json
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/transaction_segment_terms.json
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/url_clean.json
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/url_domain_extraction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.543112 newrelic-9.8.0/tests/cross_agent/fixtures/utilization/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/utilization/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/utilization/boot_id.json
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/utilization/utilization_json.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.543112 newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_agent_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_aws_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_azure_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_boot_id_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_cat_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_collector_hostname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_datastore_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_docker_container_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_docker_container_id_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_gcp_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_labels_and_rollups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_lambda_event_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_pcf_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_sql_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_transaction_segment_terms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_utilization_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/cross_agent/test_w3c_trace_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.543112 newrelic-9.8.0/tests/datastore_aioredis/
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aioredis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aioredis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aioredis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aioredis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aioredis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aioredis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aioredis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aioredis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aioredis/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aioredis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.547112 newrelic-9.8.0/tests/datastore_aredis/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aredis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aredis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aredis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aredis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aredis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aredis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aredis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aredis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_aredis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.547112 newrelic-9.8.0/tests/datastore_asyncpg/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_asyncpg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_asyncpg/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_asyncpg/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.547112 newrelic-9.8.0/tests/datastore_bmemcached/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_bmemcached/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_bmemcached/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.547112 newrelic-9.8.0/tests/datastore_elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_elasticsearch/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_elasticsearch/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_elasticsearch/test_database_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_elasticsearch/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_elasticsearch/test_instrumented_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_elasticsearch/test_mget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_elasticsearch/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_elasticsearch/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_elasticsearch/test_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.551113 newrelic-9.8.0/tests/datastore_firestore/
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_async_batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_async_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_async_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_async_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_async_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_firestore/test_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.551113 newrelic-9.8.0/tests/datastore_memcache/
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_memcache/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_memcache/test_all_methods_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_memcache/test_memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_memcache/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_memcache/test_span_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.551113 newrelic-9.8.0/tests/datastore_mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_mysql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_mysql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.551113 newrelic-9.8.0/tests/datastore_postgresql/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_postgresql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_postgresql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.555112 newrelic-9.8.0/tests/datastore_psycopg2/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_as_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_database_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_explain_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_forward_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_rollback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_slow_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.555112 newrelic-9.8.0/tests/datastore_psycopg2cffi/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2cffi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2cffi/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_psycopg2cffi/test_explain_plans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.555112 newrelic-9.8.0/tests/datastore_pylibmc/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pylibmc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pylibmc/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.555112 newrelic-9.8.0/tests/datastore_pymemcache/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pymemcache/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pymemcache/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.555112 newrelic-9.8.0/tests/datastore_pymongo/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pymongo/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pymongo/test_pymongo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.555112 newrelic-9.8.0/tests/datastore_pymssql/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pymssql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pymssql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.555112 newrelic-9.8.0/tests/datastore_pymysql/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pymysql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pymysql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.555112 newrelic-9.8.0/tests/datastore_pyodbc/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pyodbc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pyodbc/test_pyodbc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.559113 newrelic-9.8.0/tests/datastore_pysolr/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pysolr/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_pysolr/test_solr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.559113 newrelic-9.8.0/tests/datastore_redis/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_rb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_redis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.559113 newrelic-9.8.0/tests/datastore_rediscluster/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_rediscluster/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_rediscluster/test_uninstrumented_rediscluster_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.559113 newrelic-9.8.0/tests/datastore_solrpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_solrpy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_solrpy/test_solr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.559113 newrelic-9.8.0/tests/datastore_sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_sqlite/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_sqlite/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/datastore_sqlite/test_obfuscation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.563113 newrelic-9.8.0/tests/external_botocore/
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/_mock_bedrock_encoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   331596 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/_mock_external_bedrock_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    55154 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/_test_bedrock_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/_test_bedrock_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    36253 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/test_bedrock_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/test_bedrock_chat_completion_via_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    17666 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/test_bedrock_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/test_boto3_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/test_boto3_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/test_boto3_sns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/test_botocore_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/test_botocore_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/test_botocore_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_botocore/test_botocore_sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.563113 newrelic-9.8.0/tests/external_feedparser/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_feedparser/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_feedparser/packages.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_feedparser/test_feedparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.563113 newrelic-9.8.0/tests/external_http/
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_http/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_http/test_http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.563113 newrelic-9.8.0/tests/external_httplib/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_httplib/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_httplib/test_httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_httplib/test_urllib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_httplib/test_urllib2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.567113 newrelic-9.8.0/tests/external_httplib2/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_httplib2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_httplib2/test_httplib2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.567113 newrelic-9.8.0/tests/external_httpx/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_httpx/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_httpx/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.567113 newrelic-9.8.0/tests/external_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_requests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_requests/test_span_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.567113 newrelic-9.8.0/tests/external_urllib3/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_urllib3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9361 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/external_urllib3/test_urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.567113 newrelic-9.8.0/tests/framework_aiohttp/
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_aiohttp/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_aiohttp/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_aiohttp/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_aiohttp/test_client_async_await.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_aiohttp/test_client_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_aiohttp/test_externals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_aiohttp/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_aiohttp/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_aiohttp/test_server_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_aiohttp/test_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.567113 newrelic-9.8.0/tests/framework_ariadne/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_ariadne/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_ariadne/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_ariadne/_target_schema_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_ariadne/_target_schema_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_ariadne/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_ariadne/schema.graphql
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_ariadne/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.571113 newrelic-9.8.0/tests/framework_bottle/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_bottle/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_bottle/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_bottle/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.571113 newrelic-9.8.0/tests/framework_cherrypy/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_cherrypy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_cherrypy/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_cherrypy/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_cherrypy/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_cherrypy/test_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.571113 newrelic-9.8.0/tests/framework_django/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.571113 newrelic-9.8.0/tests/framework_django/dummy_app/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/dummy_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.571113 newrelic-9.8.0/tests/framework_django/dummy_app/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/dummy_app/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/dummy_app/templatetags/custom_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.571113 newrelic-9.8.0/tests/framework_django/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/templates/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/templates/render_exception.html
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/templates/results.html
--rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/test_asgi_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_django/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.575113 newrelic-9.8.0/tests/framework_falcon/
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_falcon/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_falcon/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_falcon/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.575113 newrelic-9.8.0/tests/framework_fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_fastapi/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_fastapi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_fastapi/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.575113 newrelic-9.8.0/tests/framework_flask/
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/_test_application_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/_test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/_test_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/_test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/_test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/_test_user_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/_test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/_test_views_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/test_user_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_flask/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.579113 newrelic-9.8.0/tests/framework_graphene/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphene/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphene/_target_schema_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphene/_target_schema_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphene/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphene/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.579113 newrelic-9.8.0/tests/framework_graphql/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphql/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphql/_target_schema_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphql/_target_schema_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    21392 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphql/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_graphql/test_application_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.579113 newrelic-9.8.0/tests/framework_grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_grpc/_test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_grpc/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.579113 newrelic-9.8.0/tests/framework_grpc/sample_application/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_grpc/sample_application/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_grpc/sample_application/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_grpc/sample_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_grpc/sample_application/sample_application.proto
--rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_grpc/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_grpc/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_grpc/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_grpc/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.579113 newrelic-9.8.0/tests/framework_pyramid/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_pyramid/_test_append_slash_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_pyramid/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_pyramid/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_pyramid/test_append_slash_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_pyramid/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_pyramid/test_cornice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.583113 newrelic-9.8.0/tests/framework_sanic/
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_sanic/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_sanic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_sanic/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_sanic/test_cross_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.583113 newrelic-9.8.0/tests/framework_starlette/
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_starlette/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_starlette/_test_bg_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_starlette/_test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_starlette/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_starlette/test_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_starlette/test_bg_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.583113 newrelic-9.8.0/tests/framework_strawberry/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_strawberry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_strawberry/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_strawberry/_target_schema_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_strawberry/_target_schema_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_strawberry/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_strawberry/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.583113 newrelic-9.8.0/tests/framework_tornado/
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_tornado/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_tornado/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_tornado/test_custom_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_tornado/test_externals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_tornado/test_inbound_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/framework_tornado/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.587113 newrelic-9.8.0/tests/logger_logging/
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_logging/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_logging/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_logging/test_local_decorating.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_logging/test_log_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_logging/test_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_logging/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_logging/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.587113 newrelic-9.8.0/tests/logger_loguru/
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_loguru/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_loguru/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_loguru/test_local_decorating.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_loguru/test_log_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_loguru/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_loguru/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.587113 newrelic-9.8.0/tests/logger_structlog/
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_structlog/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_structlog/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_structlog/test_local_decorating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_structlog/test_log_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/logger_structlog/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.587113 newrelic-9.8.0/tests/messagebroker_confluentkafka/
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_confluentkafka/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_confluentkafka/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_confluentkafka/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_confluentkafka/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.587113 newrelic-9.8.0/tests/messagebroker_kafkapython/
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_kafkapython/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_kafkapython/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_kafkapython/test_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_kafkapython/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_kafkapython/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.587113 newrelic-9.8.0/tests/messagebroker_pika/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/minversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/test_memory_leak.py
--rw-r--r--   0 runner    (1001) docker     (127)    17001 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/test_pika_async_connection_consume.py
--rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/test_pika_blocking_connection_consume.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13879 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/test_pika_produce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/messagebroker_pika/test_pika_supportability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.591113 newrelic-9.8.0/tests/mlmodel_langchain/
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_langchain/_mock_external_openai_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_langchain/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_langchain/hello.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_langchain/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    53134 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_langchain/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16873 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_langchain/test_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_langchain/test_vectorstore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.591113 newrelic-9.8.0/tests/mlmodel_openai/
--rw-r--r--   0 runner    (1001) docker     (127)    55141 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/_mock_external_openai_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16470 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    23598 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    18518 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_error_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    28847 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_stream_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_stream_error_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    17666 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_stream_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)    19096 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_embeddings_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    15585 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_embeddings_error_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_embeddings_stream_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_openai/test_embeddings_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.599113 newrelic-9.8.0/tests/mlmodel_sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_calibration_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_cluster_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_compose_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_covariance_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_cross_decomposition_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_discriminant_analysis_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_dummy_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_ensemble_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_feature_selection_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_gaussian_process_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_inference_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_kernel_ridge_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_linear_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_metric_scorers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_mixture_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_ml_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_model_selection_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_multiclass_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_multioutput_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_naive_bayes_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_neighbors_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_neural_network_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_pipeline_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    26289 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_prediction_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_semi_supervised_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_svm_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/mlmodel_sklearn/test_tree_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.599113 newrelic-9.8.0/tests/template_genshi/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/template_genshi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/template_genshi/test_genshi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.599113 newrelic-9.8.0/tests/template_jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/template_jinja2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/template_jinja2/test_jinja2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.599113 newrelic-9.8.0/tests/template_mako/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/template_mako/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/template_mako/test_mako.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.599113 newrelic-9.8.0/tests/testing_support/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/asgi_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/db_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/external_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.599113 newrelic-9.8.0/tests/testing_support/fixture/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/fixture/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    52405 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/ml_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/mock_external_grpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/mock_external_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/mock_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/sample_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/sample_asgi_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 23:08:43.611113 newrelic-9.8.0/tests/testing_support/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_apdex_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_application_error_event_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_application_error_trace_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_application_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_browser_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_cross_process_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_custom_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_custom_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_custom_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_database_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_database_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_database_trace_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_datastore_trace_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_dimensional_metric_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_dimensional_metrics_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_distributed_trace_accepted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_distributed_tracing_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_error_event_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_error_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_error_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_error_trace_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_external_node_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_function_called.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_internal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_log_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_log_event_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_log_event_count_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_log_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_log_events_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_messagebroker_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_metric_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_ml_event_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_ml_event_count_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_ml_event_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_ml_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_ml_events_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_non_transaction_error_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_outbound_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_serverless_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_serverless_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_serverless_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_slow_sql_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_span_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_sql_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_synthetics_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_synthetics_transaction_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_time_metrics_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_transaction_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_transaction_error_event_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_transaction_error_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_transaction_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_transaction_event_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_transaction_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_transaction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_transaction_slow_sql_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_transaction_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_tt_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_tt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-03-27 23:08:38.000000 newrelic-9.8.0/tests/testing_support/validators/validate_tt_segment_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    26359 2024-03-27 23:08:38.000000 newrelic-9.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.735916 newrelic-9.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.535914 newrelic-9.9.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-18 22:50:46.000000 newrelic-9.9.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-18 22:50:46.000000 newrelic-9.9.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.535914 newrelic-9.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.535914 newrelic-9.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/ISSUE_TEMPLATE/troubleshooting.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.535914 newrelic-9.9.0/.github/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/containers/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/containers/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1528 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/containers/install-python.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/containers/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.535914 newrelic-9.9.0/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1268 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/scripts/retry.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.539914 newrelic-9.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/workflows/build-ci-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/workflows/deploy-python.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1186 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/workflows/get-envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/workflows/mega-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    31311 2024-04-18 22:50:46.000000 newrelic-9.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 22:50:46.000000 newrelic-9.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 22:50:46.000000 newrelic-9.9.0/.mega-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-04-18 22:50:46.000000 newrelic-9.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-18 22:50:46.000000 newrelic-9.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-18 22:50:46.000000 newrelic-9.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-04-18 22:50:51.735916 newrelic-9.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-04-18 22:50:46.000000 newrelic-9.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-18 22:50:46.000000 newrelic-9.9.0/ROADMAP.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-18 22:50:46.000000 newrelic-9.9.0/THIRD_PARTY_NOTICES.md
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-18 22:50:46.000000 newrelic-9.9.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.539914 newrelic-9.9.0/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.543914 newrelic-9.9.0/newrelic/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/debug_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/generate_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/license_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/network_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/record_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/run_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/server_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/admin/validate_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.547914 newrelic-9.9.0/newrelic/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/asgi_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/background_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/cat_header_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/database_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/datastore_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/error_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/external_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/function_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/function_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/generator_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/graphql_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/html_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/in_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/memcache_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/message_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/message_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/ml_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/object_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/out_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/post_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/pre_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/profile_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/solr_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/supportability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26851 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/time_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79389 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/transaction_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/web_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25224 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/api/wsgi_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.547914 newrelic-9.9.0/newrelic/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/bootstrap/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.551914 newrelic-9.9.0/newrelic/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/_monotonic.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21725 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/agent_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/async_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64813 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20660 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/encoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/log_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/object_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/object_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/package_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/streaming_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13872 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/common/utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)   161325 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.555914 newrelic-9.9.0/newrelic/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/_thread_utilization.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/adaptive_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32825 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22340 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/agent_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/agent_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74275 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46085 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/database_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29349 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/datastore_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/error_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/error_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/external_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/function_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/graphql_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/graphql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/infinite_tracing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/infinite_tracing_v3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/infinite_tracing_v4_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/internal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/log_event_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/loop_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/memcache_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/message_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/node_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/otlp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16490 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/profile_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/root_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/rules_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/solr_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/stack_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75777 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/stats_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/string_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/thread_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15461 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/trace_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/core/transaction_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.555914 newrelic-9.9.0/newrelic/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.555914 newrelic-9.9.0/newrelic/extras/framework_django/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/extras/framework_django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.559914 newrelic-9.9.0/newrelic/extras/framework_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/extras/framework_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/extras/framework_django/templatetags/newrelic_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.571914 newrelic-9.9.0/newrelic/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_asgiref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_cheroot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_cherrypy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_daphne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_flup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_gevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_hypercorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_meinheld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_paste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_uvicorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_waitress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/adapter_wsgiref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/application_celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/application_gearman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_cornice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_djangorestframework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_flask_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_graphqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_piston.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/component_tastypie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/coroutines_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/coroutines_gevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_cx_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_ibm_db_dbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_oursql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_psycopg2cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_psycopg2ct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_pymssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_pymysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_pyodbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/database_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_aioredis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_aredis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_bmemcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21862 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18601 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_firestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_pyelasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_pylibmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_pymemcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_pysolr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_solrpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/datastore_umemcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33824 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_botocore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_facepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_feedparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_pywapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_thrift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_urllib2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/external_xmlrpclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_bottle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_cherrypy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42156 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_django_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15352 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_graphene.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18198 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_graphql_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_pylons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_web2py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/framework_webpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/logger_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/logger_loguru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/logger_structlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/memcache_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/messagebroker_confluentkafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/messagebroker_kafkapython.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/messagebroker_pika.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/middleware_flask_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/middleware_weberror.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35454 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/mlmodel_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41623 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/mlmodel_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/mlmodel_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/template_genshi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/template_jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/hooks/template_mako.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.575914 newrelic-9.9.0/newrelic/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/network/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/network/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/newrelic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.575914 newrelic-9.9.0/newrelic/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/asgiref_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.575914 newrelic-9.9.0/newrelic/packages/isort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.575914 newrelic-9.9.0/newrelic/packages/isort/stdlibs/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py27.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py311.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/isort/stdlibs/py39.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.575914 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/logs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16736 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/metrics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/opentelemetry_proto/resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34549 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/six.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.579914 newrelic-9.9.0/newrelic/packages/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40285 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.579914 newrelic-9.9.0/newrelic/packages/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.579914 newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17632 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17055 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34431 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.579914 newrelic-9.9.0/newrelic/packages/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.579914 newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34665 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19990 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30761 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.583914 newrelic-9.9.0/newrelic/packages/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22013 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17165 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/urllib3/util/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.583914 newrelic-9.9.0/newrelic/packages/wrapt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/__wrapt__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96990 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/_wrappers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/weakrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/packages/wrapt/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/newrelic/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/data_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/gc_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-18 22:50:46.000000 newrelic-9.9.0/newrelic/samplers/memory_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.735916 newrelic-9.9.0/newrelic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    61751 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-18 22:50:51.000000 newrelic-9.9.0/newrelic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-18 22:50:46.000000 newrelic-9.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/scripts/newrelic-admin
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-18 22:50:51.735916 newrelic-9.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-04-18 22:50:46.000000 newrelic-9.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.531914 newrelic-9.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_asgiref/
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_asgiref/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_asgiref/test_context_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_cheroot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_cheroot/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_cheroot/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_daphne/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_daphne/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_daphne/test_daphne.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_gevent/
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gevent/_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gevent/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gevent/test_patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gevent/test_pywsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/asgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/async_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/test_aiohttp_app_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/test_asgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/test_gaiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_gunicorn/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_hypercorn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_hypercorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_hypercorn/test_hypercorn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.587914 newrelic-9.9.0/tests/adapter_uvicorn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_uvicorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_uvicorn/test_uvicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.591915 newrelic-9.9.0/tests/adapter_waitress/
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_waitress/_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_waitress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/adapter_waitress/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.599915 newrelic-9.9.0/tests/agent_features/
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/_test_async_coroutine_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/_test_async_coroutine_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/_test_async_generator_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/_test_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_apdex_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32398 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_asgi_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_asgi_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_asgi_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_asgi_w3c_trace_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_async_context_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_async_generator_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_async_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_async_wrapper_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35683 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_attributes_in_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_background_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34491 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_browser_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_collector_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_coroutine_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_coroutine_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_custom_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_custom_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_datastore_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_dead_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_dimensional_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_error_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_error_group_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_event_loop_wait_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_exception_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_function_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29688 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_high_security_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_ignore_expected_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_llm_token_count_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_log_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_logs_in_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_metric_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_ml_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_notice_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_priority_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_profile_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_record_llm_feedback_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_serverless_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24641 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_stack_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_supportability_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_synthetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_time_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_transaction_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_transaction_trace_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_w3c_trace_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_web_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_features/test_wsgi_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.599915 newrelic-9.9.0/tests/agent_streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/_test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17363 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/test_infinite_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/test_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/test_stream_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_streaming/test_streaming_rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.603915 newrelic-9.9.0/tests/agent_unittests/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/_test_import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_agent_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20250 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_agent_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_check_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_connect_response_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_distributed_tracing_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_encoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_full_uri_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32348 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_harvest_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21008 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_infinite_trace_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_package_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_region_aware_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_sampler_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_serverless_mode_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_trace_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_utilization_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/agent_unittests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.607915 newrelic-9.9.0/tests/application_celery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/test_max_tasks_per_child.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_celery/test_task_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.607915 newrelic-9.9.0/tests/application_gearman/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_gearman/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/application_gearman/test_gearman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.607915 newrelic-9.9.0/tests/component_djangorestframework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_djangorestframework/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.607915 newrelic-9.9.0/tests/component_flask_rest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_flask_rest/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_flask_rest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_flask_rest/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.607915 newrelic-9.9.0/tests/component_graphqlserver/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_graphqlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_graphqlserver/_target_schema_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_graphqlserver/_test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_graphqlserver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_graphqlserver/test_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.611915 newrelic-9.9.0/tests/component_tastypie/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/component_tastypie/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.611915 newrelic-9.9.0/tests/coroutines_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/coroutines_asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/coroutines_asyncio/test_context_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.615915 newrelic-9.9.0/tests/cross_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.615915 newrelic-9.9.0/tests/cross_agent/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/attribute_configuration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/cat_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/collector_hostname.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.615915 newrelic-9.9.0/tests/cross_agent/fixtures/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/datastores/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/datastores/datastore_instances.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.615915 newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    48250 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json
+-rw-r--r--   0 runner    (1001) docker     (127)    58950 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/trace_context.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.619915 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/cases.json
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-0.9.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/heroku.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/invalid-length.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-lxc-container.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-no-container.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.10-no-container.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.619915 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/cases.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-20.10.16.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-24.0.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-too-long.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-characters.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-length.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/labels.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.627915 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_auth.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/batch_get.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/batch_submit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudformation_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudwatch_logs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/codecommit.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cognito_sync.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_analytics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_apache.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_invoke.json
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/lex_appointment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/lex_book_car.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_put.json
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/scheduled_event.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/ses.json
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/smarthome_discovery.json
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/smarthome_turn_off.json
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/sns.json
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/sqs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.643915 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.query.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.query.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.643915 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_1logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_2core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17027 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38341 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/malformed_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.643915 newrelic-9.9.0/tests/cross_agent/fixtures/proc_meminfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_meminfo/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_meminfo/malformed_file.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rules.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_cookie.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.651915 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/empty_head
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)      852 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)      958 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.659915 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.659915 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.659915 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/sql_parsing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/transaction_segment_terms.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/url_clean.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/url_domain_extraction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.659915 newrelic-9.9.0/tests/cross_agent/fixtures/utilization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization/boot_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization/utilization_json.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.663915 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_agent_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_aws_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_azure_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_boot_id_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_cat_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_collector_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_datastore_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_docker_container_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_docker_container_id_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_gcp_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_labels_and_rollups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_lambda_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_pcf_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_sql_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_transaction_segment_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_utilization_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/cross_agent/test_w3c_trace_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.663915 newrelic-9.9.0/tests/datastore_aioredis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aioredis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.663915 newrelic-9.9.0/tests/datastore_aredis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_aredis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.667915 newrelic-9.9.0/tests/datastore_asyncpg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_asyncpg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_asyncpg/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_asyncpg/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.667915 newrelic-9.9.0/tests/datastore_bmemcached/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_bmemcached/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_bmemcached/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.667915 newrelic-9.9.0/tests/datastore_elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_database_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_instrumented_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_mget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_elasticsearch/test_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.671915 newrelic-9.9.0/tests/datastore_firestore/
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_async_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_firestore/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.671915 newrelic-9.9.0/tests/datastore_memcache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_memcache/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_memcache/test_all_methods_wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_memcache/test_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_memcache/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_memcache/test_span_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.671915 newrelic-9.9.0/tests/datastore_mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_mysql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_mysql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.671915 newrelic-9.9.0/tests/datastore_postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_postgresql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_postgresql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_psycopg2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_as_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_database_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_explain_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_forward_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_rollback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_slow_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_psycopg2cffi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2cffi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2cffi/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_psycopg2cffi/test_explain_plans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pylibmc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pylibmc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pylibmc/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pymemcache/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymemcache/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymemcache/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pymongo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymongo/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymongo/test_pymongo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pymssql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymssql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymssql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pymysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymysql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pymysql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pyodbc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pyodbc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pyodbc/test_pyodbc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.675915 newrelic-9.9.0/tests/datastore_pysolr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pysolr/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_pysolr/test_solr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.679915 newrelic-9.9.0/tests/datastore_redis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_rb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_redis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.679915 newrelic-9.9.0/tests/datastore_rediscluster/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_rediscluster/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_rediscluster/test_uninstrumented_rediscluster_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.679915 newrelic-9.9.0/tests/datastore_solrpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_solrpy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_solrpy/test_solr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.679915 newrelic-9.9.0/tests/datastore_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_sqlite/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_sqlite/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/datastore_sqlite/test_obfuscation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_botocore/
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/_mock_bedrock_encoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   331596 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/_mock_external_bedrock_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55152 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/_test_bedrock_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/_test_bedrock_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36309 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_bedrock_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_bedrock_chat_completion_via_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_bedrock_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_boto3_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_boto3_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_boto3_sns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_botocore_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_botocore_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_botocore_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_botocore/test_botocore_sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_feedparser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_feedparser/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_feedparser/packages.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_feedparser/test_feedparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_http/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_http/test_http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_httplib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib/test_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib/test_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib/test_urllib2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_httplib2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httplib2/test_httplib2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.683915 newrelic-9.9.0/tests/external_httpx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httpx/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_httpx/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.687915 newrelic-9.9.0/tests/external_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_requests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_requests/test_span_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.687915 newrelic-9.9.0/tests/external_urllib3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_urllib3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9361 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/external_urllib3/test_urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.687915 newrelic-9.9.0/tests/framework_aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_client_async_await.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_client_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_externals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_server_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_aiohttp/test_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.687915 newrelic-9.9.0/tests/framework_ariadne/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/_target_schema_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/_target_schema_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/schema.graphql
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_ariadne/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.687915 newrelic-9.9.0/tests/framework_bottle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_bottle/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_bottle/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_bottle/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_cherrypy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_cherrypy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_cherrypy/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_cherrypy/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_cherrypy/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_cherrypy/test_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_django/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_django/dummy_app/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/dummy_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_django/dummy_app/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/dummy_app/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/dummy_app/templatetags/custom_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_django/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/templates/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/templates/render_exception.html
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/templates/results.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22716 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/test_asgi_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_django/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.691915 newrelic-9.9.0/tests/framework_falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_falcon/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_falcon/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_falcon/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.695915 newrelic-9.9.0/tests/framework_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_fastapi/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_fastapi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_fastapi/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.695915 newrelic-9.9.0/tests/framework_flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_application_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_user_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/_test_views_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_user_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_flask/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.695915 newrelic-9.9.0/tests/framework_graphene/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/_target_schema_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/_target_schema_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphene/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.699915 newrelic-9.9.0/tests/framework_graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/_target_schema_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/_target_schema_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21392 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_graphql/test_application_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.699915 newrelic-9.9.0/tests/framework_grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/_test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.699915 newrelic-9.9.0/tests/framework_grpc/sample_application/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/sample_application/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/sample_application/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/sample_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/sample_application/sample_application.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_grpc/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.699915 newrelic-9.9.0/tests/framework_pyramid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/_test_append_slash_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/test_append_slash_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_pyramid/test_cornice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.703915 newrelic-9.9.0/tests/framework_sanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_sanic/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_sanic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_sanic/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_sanic/test_cross_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.703915 newrelic-9.9.0/tests/framework_starlette/
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/_test_bg_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/_test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_starlette/test_bg_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.703915 newrelic-9.9.0/tests/framework_strawberry/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/_target_schema_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/_target_schema_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_strawberry/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.703915 newrelic-9.9.0/tests/framework_tornado/
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/test_custom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/test_externals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/test_inbound_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/framework_tornado/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.707915 newrelic-9.9.0/tests/logger_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_local_decorating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_log_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_logging/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.707915 newrelic-9.9.0/tests/logger_loguru/
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/test_local_decorating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/test_log_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_loguru/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.707915 newrelic-9.9.0/tests/logger_structlog/
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_structlog/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_structlog/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_structlog/test_local_decorating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_structlog/test_log_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/logger_structlog/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.707915 newrelic-9.9.0/tests/messagebroker_confluentkafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_confluentkafka/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_confluentkafka/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_confluentkafka/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_confluentkafka/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.711915 newrelic-9.9.0/tests/messagebroker_kafkapython/
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_kafkapython/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_kafkapython/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_kafkapython/test_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_kafkapython/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_kafkapython/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.711915 newrelic-9.9.0/tests/messagebroker_pika/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/minversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_memory_leak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_pika_async_connection_consume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13879 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_pika_produce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/messagebroker_pika/test_pika_supportability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.711915 newrelic-9.9.0/tests/mlmodel_langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/_mock_external_openai_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/hello.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53177 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16916 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/test_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17598 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_langchain/test_vectorstore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.715915 newrelic-9.9.0/tests/mlmodel_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)    55141 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/_mock_external_openai_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23654 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18574 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_error_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17200 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28903 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_error_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19152 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15641 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_error_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_stream_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.719915 newrelic-9.9.0/tests/mlmodel_sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_calibration_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_cluster_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_compose_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_covariance_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_cross_decomposition_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_discriminant_analysis_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_dummy_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13450 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_ensemble_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_feature_selection_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_gaussian_process_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12412 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_inference_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_kernel_ridge_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_linear_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_metric_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_mixture_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_ml_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_model_selection_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_multiclass_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_multioutput_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_naive_bayes_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_neighbors_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_neural_network_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_pipeline_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26289 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_prediction_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_semi_supervised_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_svm_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/mlmodel_sklearn/test_tree_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.719915 newrelic-9.9.0/tests/template_genshi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_genshi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_genshi/test_genshi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.719915 newrelic-9.9.0/tests/template_jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_jinja2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_jinja2/test_jinja2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.719915 newrelic-9.9.0/tests/template_mako/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_mako/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/template_mako/test_mako.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.723915 newrelic-9.9.0/tests/testing_support/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/asgi_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9612 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/db_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/external_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.723915 newrelic-9.9.0/tests/testing_support/fixture/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/fixture/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50802 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/ml_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/mock_external_grpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/mock_external_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/mock_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/sample_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/sample_asgi_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:50:51.735916 newrelic-9.9.0/tests/testing_support/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_apdex_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_application_error_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_application_error_trace_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_application_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_browser_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_cross_process_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_custom_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_custom_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_custom_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_database_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_database_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_database_trace_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_datastore_trace_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_dimensional_metric_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_dimensional_metrics_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_distributed_trace_accepted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_distributed_tracing_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_event_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_external_node_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_function_called.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_internal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_log_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_log_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_log_event_count_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_log_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_log_events_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_messagebroker_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_metric_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_count_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_ml_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_ml_events_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_non_transaction_error_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_outbound_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_serverless_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_serverless_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_serverless_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_slow_sql_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_sql_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_synthetics_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_synthetics_transaction_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_time_metrics_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_error_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_error_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_event_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_slow_sql_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_transaction_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_tt_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_tt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-18 22:50:46.000000 newrelic-9.9.0/tests/testing_support/validators/validate_tt_segment_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26571 2024-04-18 22:50:46.000000 newrelic-9.9.0/tox.ini
```

### Comparing `newrelic-9.8.0/.devcontainer/Dockerfile` & `newrelic-9.9.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.devcontainer/devcontainer.json` & `newrelic-9.9.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `newrelic-9.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/ISSUE_TEMPLATE/config.yml` & `newrelic-9.9.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `newrelic-9.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/containers/Dockerfile` & `newrelic-9.9.0/.github/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/containers/Makefile` & `newrelic-9.9.0/.github/containers/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,19 @@
 
 # Run a specific tag as a container.
 # Usage: make run.<tag>
 # Defaults to run.local, but can instead be run.latest or any other tag.
 .PHONY: run.%
 run.%:
 # Build image if local was specified, else pull latest
-	@if [[ "$*" = "local" ]]; then cd ${MAKEFILE_DIR} && $(MAKE) build; else docker pull ${IMAGE_NAME}:$*; fi
+	@if [[ "$*" = "local" ]]; then \
+		cd ${MAKEFILE_DIR} && $(MAKE) build; \
+	else \
+		docker pull --platform=${PLATFORM} ${IMAGE_NAME}:$*; \
+	fi
 	@docker run --rm -it \
 		--platform=${PLATFORM} \
 		--mount type=bind,source="${REPO_ROOT}",target=/home/github/python-agent \
 		--workdir=/home/github/python-agent \
 		--add-host=host.docker.internal:host-gateway \
 		-e NEW_RELIC_HOST="${NEW_RELIC_HOST}" \
 		-e NEW_RELIC_LICENSE_KEY="${NEW_RELIC_LICENSE_KEY}" \
```

### Comparing `newrelic-9.8.0/.github/containers/install-python.sh` & `newrelic-9.9.0/.github/containers/install-python.sh`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/dependabot.yml` & `newrelic-9.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/mergify.yml` & `newrelic-9.9.0/.github/mergify.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/pull_request_template.md` & `newrelic-9.9.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/scripts/retry.sh` & `newrelic-9.9.0/.github/scripts/retry.sh`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/stale.yml` & `newrelic-9.9.0/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/workflows/build-ci-image.yml` & `newrelic-9.9.0/.github/workflows/build-ci-image.yml`

 * *Files 9% similar despite different names*

```diff
@@ -22,47 +22,47 @@
   cancel-in-progress: true
 
 jobs:
   build:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
         with:
           persist-credentials: false
           fetch-depth: 0
 
       - name: Set up Docker Buildx
         id: buildx
-        uses: docker/setup-buildx-action@v2
+        uses: docker/setup-buildx-action@d70bba72b1f3fd22344832f00baa16ece964efeb # 3.3.0
 
       - name: Generate Docker Metadata (Tags and Labels)
         id: meta
-        uses: docker/metadata-action@v4
+        uses: docker/metadata-action@8e5442c4ef9f78752691e2d8f8d19755c6f78e81 # 5.5.1
         with:
           images: ghcr.io/${{ github.repository }}-ci
           flavor: |
             prefix=
             suffix=
             latest=false
           tags: |
             type=raw,value=latest,enable={{is_default_branch}}
             type=schedule,pattern={{date 'YYYY-MM-DD'}}
             type=sha,format=short,prefix=sha-
             type=sha,format=long,prefix=sha-
 
       - name: Login to GitHub Container Registry
         if: github.event_name != 'pull_request'
-        uses: docker/login-action@v2
+        uses: docker/login-action@e92390c5fb421da1463c202d546fed0ec5c39f20 # 3.1.0
         with:
           registry: ghcr.io
           username: ${{ github.repository_owner }}
           password: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Build and Publish Image
-        uses: docker/build-push-action@v3
+        uses: docker/build-push-action@2cdde995de11925a030ce8070c3d77a52ffcf1c0 # 5.3.0
         with:
           push: ${{ github.event_name != 'pull_request' }}
           context: .github/containers
           platforms: ${{ (format('refs/heads/{0}', github.event.repository.default_branch) == github.ref) && 'linux/amd64,linux/arm64' || 'linux/amd64' }}
           tags: ${{ steps.meta.outputs.tags }}
           labels: ${{ steps.meta.outputs.labels }}
```

### Comparing `newrelic-9.8.0/.github/workflows/deploy-python.yml` & `newrelic-9.9.0/.github/workflows/deploy-python.yml`

 * *Files 15% similar despite different names*

```diff
@@ -36,72 +36,72 @@
           - cp310-musllinux
           - cp311-manylinux
           - cp311-musllinux
           - cp312-manylinux
           - cp312-musllinux
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
         with:
           persist-credentials: false
           fetch-depth: 0
 
       - name: Setup QEMU
-        uses: docker/setup-qemu-action@v3
+        uses: docker/setup-qemu-action@68827325e0b33c7199eb31dd4e31fbe9023e06e3 # 3.0.0
 
       - name: Build Wheels
-        uses: pypa/cibuildwheel@v2.16.2
+        uses: pypa/cibuildwheel@8d945475ac4b1aac4ae08b2fd27db9917158b6ce # 2.17.0
         env:
           CIBW_PLATFORM: linux
           CIBW_BUILD: "${{ matrix.wheel }}*"
           CIBW_ARCHS_LINUX: x86_64 aarch64
           CIBW_ENVIRONMENT: "LD_LIBRARY_PATH=/opt/rh/devtoolset-8/root/usr/lib64:/opt/rh/devtoolset-8/root/usr/lib:/opt/rh/devtoolset-8/root/usr/lib64/dyninst:/opt/rh/devtoolset-8/root/usr/lib/dyninst:/usr/local/lib64:/usr/local/lib"
           CIBW_TEST_REQUIRES: pytest
           CIBW_TEST_COMMAND: "PYTHONPATH={project}/tests pytest {project}/tests/agent_unittests -vx"
 
       - name: Upload Artifacts
-        uses: actions/upload-artifact@v4.0.0
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: ${{ github.job }}-${{ matrix.wheel }}
           path: ./wheelhouse/*.whl
           retention-days: 1
 
   build-linux-py2:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
         with:
           persist-credentials: false
           fetch-depth: 0
 
       - name: Setup QEMU
-        uses: docker/setup-qemu-action@v3
+        uses: docker/setup-qemu-action@68827325e0b33c7199eb31dd4e31fbe9023e06e3 # 3.0.0
 
       - name: Build Wheels
-        uses: pypa/cibuildwheel@v1.12.0
+        uses: pypa/cibuildwheel@bf3a5590c9aeb9a7e4ff4025ef7400e0c6ad1248 # 1.12.0  (Last release to support Python 2)
         env:
           CIBW_PLATFORM: linux
           CIBW_BUILD: cp27-manylinux_x86_64
           CIBW_ARCHS_LINUX: x86_64
           CIBW_ENVIRONMENT: "LD_LIBRARY_PATH=/opt/rh/devtoolset-8/root/usr/lib64:/opt/rh/devtoolset-8/root/usr/lib:/opt/rh/devtoolset-8/root/usr/lib64/dyninst:/opt/rh/devtoolset-8/root/usr/lib/dyninst:/usr/local/lib64:/usr/local/lib"
           CIBW_TEST_REQUIRES: pytest==4.6.11
           CIBW_TEST_COMMAND: "PYTHONPATH={project}/tests pytest {project}/tests/agent_unittests -vx"
 
       - name: Upload Artifacts
-        uses: actions/upload-artifact@v4.0.0
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: ${{ github.job }}
           path: ./wheelhouse/*.whl
           retention-days: 1
 
   build-sdist:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
         with:
           persist-credentials: false
           fetch-depth: 0
 
       - name: Install Dependencies
         run: |
           pip install -U pip
@@ -114,15 +114,15 @@
       - name: Prepare MD5 Hash File
         run: |
           tarball="$(python setup.py --fullname).tar.gz"
           md5_file=${tarball}.md5
           openssl md5 -binary dist/${tarball} | xxd -p | tr -d '\n' > dist/${md5_file}
 
       - name: Upload Artifacts
-        uses: actions/upload-artifact@v4.0.0
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: ${{ github.job }}-sdist
           path: |
             ./dist/*.tar.gz
             ./dist/*.tar.gz.md5
           retention-days: 1
 
@@ -131,31 +131,31 @@
 
     needs:
       - build-linux-py3
       - build-linux-py2
       - build-sdist
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
         with:
           persist-credentials: false
           fetch-depth: 0
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # 5.1.0
         with:
           python-version: "3.x"
           architecture: x64
 
       - name: Install Dependencies
         run: |
           pip install -U pip
           pip install -U wheel setuptools twine
 
       - name: Download Artifacts
-        uses: actions/download-artifact@v4.1.0
+        uses: actions/download-artifact@c850b930e6ba138125429b7e5c93fc707a7f8427 # 4.1.4
         with:
           path: ./artifacts/
 
       - name: Unpack Artifacts
         run: |
           mkdir -p dist/
           mv artifacts/**/*{.whl,.tar.gz,.tar.gz.md5} dist/
```

### Comparing `newrelic-9.8.0/.github/workflows/get-envs.py` & `newrelic-9.9.0/.github/workflows/get-envs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.github/workflows/mega-linter.yml` & `newrelic-9.9.0/.github/workflows/mega-linter.yml`

 * *Files 6% similar despite different names*

```diff
@@ -21,48 +21,48 @@
 jobs:
   build:
     name: Mega-Linter
     runs-on: ubuntu-latest
     steps:
       # Git Checkout
       - name: Checkout Code
-        uses: actions/checkout@v4
+        uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
         with:
           token: ${{ secrets.PAT || secrets.GITHUB_TOKEN }}
           fetch-depth: 0
 
       # Mega-Linter
       - name: Mega-Linter
         id: ml
         # You can override Mega-Linter flavor used to have faster performances
         # More info at https://oxsecurity.github.io/megalinter/flavors/
-        uses: oxsecurity/megalinter/flavors/python@v6
+        uses: oxsecurity/megalinter/flavors/python@a7a0163b6c8ff7474a283d99a706e27483ddd80f # 7.10.0
         env:
           # All available variables are described in documentation
           # https://oxsecurity.github.io/megalinter/configuration/
           VALIDATE_ALL_CODEBASE: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }} # Validates all source when push on main, else just the git diff with main. Set 'true' if you always want to lint all sources
           DEFAULT_BRANCH: ${{ github.event_name == 'pull_request' && github.base_ref || 'main' }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           # ADD YOUR CUSTOM ENV VARIABLES HERE TO OVERRIDE VALUES OF .mega-linter.yml AT THE ROOT OF YOUR REPOSITORY
 
       # Upload Mega-Linter artifacts
       - name: Archive production artifacts
         if: ${{ success() }} || ${{ failure() }}
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: Mega-Linter reports
           path: |
             megalinter-reports
             mega-linter.log
 
       # Create pull request if applicable (for now works only on PR from same repository, not from forks)
       - name: Create Pull Request with applied fixes
         id: cpr
         if: steps.ml.outputs.has_updated_sources == 1 && (env.APPLY_FIXES_EVENT == 'all' || env.APPLY_FIXES_EVENT == github.event_name) && env.APPLY_FIXES_MODE == 'pull_request' && (github.event_name == 'push' || github.event.pull_request.head.repo.full_name == github.repository) && !contains(github.event.head_commit.message, 'skip fix')
-        uses: peter-evans/create-pull-request@v3
+        uses: peter-evans/create-pull-request@c55203cfde3e5c11a452d352b4393e68b85b4533 # 6.0.3
         with:
           token: ${{ secrets.PAT || secrets.GITHUB_TOKEN }}
           commit-message: "[Mega-Linter] Apply linters automatic fixes"
           title: "[Mega-Linter] Apply linters automatic fixes"
           labels: bot
       - name: Create PR output
         if: steps.ml.outputs.has_updated_sources == 1 && (env.APPLY_FIXES_EVENT == 'all' || env.APPLY_FIXES_EVENT == github.event_name) && env.APPLY_FIXES_MODE == 'pull_request' && (github.event_name == 'push' || github.event.pull_request.head.repo.full_name == github.repository) && !contains(github.event.head_commit.message, 'skip fix')
@@ -72,11 +72,11 @@
 
       # Push new commit if applicable (for now works only on PR from same repository, not from forks)
       - name: Prepare commit
         if: steps.ml.outputs.has_updated_sources == 1 && (env.APPLY_FIXES_EVENT == 'all' || env.APPLY_FIXES_EVENT == github.event_name) && env.APPLY_FIXES_MODE == 'commit' && github.ref != 'refs/heads/main' && (github.event_name == 'push' || github.event.pull_request.head.repo.full_name == github.repository) && !contains(github.event.head_commit.message, 'skip fix')
         run: sudo chown -Rc $UID .git/
       - name: Commit and push applied linter fixes
         if: steps.ml.outputs.has_updated_sources == 1 && (env.APPLY_FIXES_EVENT == 'all' || env.APPLY_FIXES_EVENT == github.event_name) && env.APPLY_FIXES_MODE == 'commit' && github.ref != 'refs/heads/main' && (github.event_name == 'push' || github.event.pull_request.head.repo.full_name == github.repository) && !contains(github.event.head_commit.message, 'skip fix')
-        uses: stefanzweifel/git-auto-commit-action@v4
+        uses: stefanzweifel/git-auto-commit-action@8621497c8c39c72f3e2a999a26b4ca1b5058a842 # 5.0.1
         with:
           branch: ${{ github.event.pull_request.head.ref || github.head_ref || github.ref }}
           commit_message: "[Mega-Linter] Apply linters fixes"
```

### Comparing `newrelic-9.8.0/.github/workflows/tests.yml` & `newrelic-9.9.0/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -32,14 +32,15 @@
   # Aggregate job that provides a single check for all tests passing
   tests:
     runs-on: ubuntu-20.04
     needs:
       - python
       - elasticsearchserver07
       - elasticsearchserver08
+      - firestore
       - grpc
       - kafka
       - memcached
       - mongodb
       - mssql
       - mysql
       - postgres
@@ -56,37 +57,38 @@
   coverage:
     if: success() || failure() # Does not run on cancelled workflows
     runs-on: ubuntu-20.04
     needs:
       - tests
 
     steps:
-      - uses: actions/checkout@v4
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
+      - uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # 5.1.0
         with:
           python-version: "3.10"
           architecture: x64
 
       - name: Download Coverage Artifacts
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@c850b930e6ba138125429b7e5c93fc707a7f8427 # 4.1.4
         with:
           path: ./
 
       - name: Combine Coverage
         run: |
           pip install coverage
           find . -name ".coverage.*" -exec mv {} ./ \;
           coverage combine
           coverage xml
 
       - name: Upload Coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@84508663e988701840491b86de86b666e8a86bed # 4.3.0
         with:
           files: coverage.xml
           fail_ci_if_error: true
+          token: ${{ secrets.CODECOV_TOKEN }}
 
   # Tests
   python:
     env:
       TOTAL_GROUPS: 20
 
     strategy:
@@ -119,15 +121,15 @@
     runs-on: ubuntu-20.04
     container:
       image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -146,15 +148,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   grpc:
     env:
@@ -168,15 +170,15 @@
     runs-on: ubuntu-20.04
     container:
       image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -195,15 +197,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }}
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   postgres:
     env:
@@ -232,15 +234,15 @@
         options: >-
           --health-cmd pg_isready
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -259,15 +261,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   mssql:
     env:
@@ -299,15 +301,15 @@
         options: >-
           --health-cmd "/opt/mssql-tools/bin/sqlcmd -U SA -P $MSSQL_SA_PASSWORD -Q 'SELECT 1'"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -326,15 +328,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   mysql:
     env:
@@ -366,15 +368,15 @@
         options: >-
           --health-cmd "mysqladmin ping -h localhost"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -393,15 +395,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   rediscluster:
     env:
@@ -469,15 +471,15 @@
 
       cluster-setup:
         image: hmstepanek/redis-cluster:1.0.0
         options: >-
           --add-host=host.docker.internal:host-gateway
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -496,15 +498,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   redis:
     env:
@@ -531,15 +533,15 @@
         options: >-
           --health-cmd "redis-cli ping"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -558,15 +560,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   solr:
     env:
@@ -595,15 +597,15 @@
         options: >-
           --health-cmd "curl localhost:8983/solr/collection/admin/ping | grep OK"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -622,15 +624,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   memcached:
     env:
@@ -657,15 +659,15 @@
         options: >-
           --health-cmd "timeout 5 bash -c 'cat < /dev/null > /dev/udp/127.0.0.1/11211'"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -684,15 +686,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   rabbitmq:
     env:
@@ -720,15 +722,15 @@
         options: >-
           --health-cmd "rabbitmq-diagnostics status"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -747,15 +749,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   kafka:
     env:
@@ -794,15 +796,15 @@
           KAFKA_CFG_AUTO_CREATE_TOPICS_ENABLE: true
           KAFKA_CFG_LISTENERS: L1://:8082,L2://:8083,L3://:8080
           KAFKA_CFG_ADVERTISED_LISTENERS: L1://host.docker.internal:8082,L2://host.docker.internal:8083,L3://kafka:8080
           KAFKA_CFG_LISTENER_SECURITY_PROTOCOL_MAP: L1:PLAINTEXT,L2:PLAINTEXT,L3:PLAINTEXT
           KAFKA_CFG_INTER_BROKER_LISTENER_NAME: L3
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -821,15 +823,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   mongodb:
     env:
@@ -856,15 +858,15 @@
         options: >-
           --health-cmd "echo 'db.runCommand(\"ping\").ok' | mongo localhost:27017/test --quiet || exit 1"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -883,15 +885,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   elasticsearchserver07:
     env:
@@ -920,15 +922,15 @@
         options: >-
           --health-cmd "curl --silent --fail localhost:9200/_cluster/health || exit 1"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -947,15 +949,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   elasticsearchserver08:
     env:
@@ -985,15 +987,15 @@
         options: >-
           --health-cmd "curl --silent --fail localhost:9200/_cluster/health || exit 1"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -1012,15 +1014,15 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
   firestore:
     env:
@@ -1054,15 +1056,15 @@
         # This is a very hacky solution. GitHub Actions doesn't provide APIs for setting commands on services, but allows adding arbitrary options.
         # --entrypoint won't work as it only accepts an executable and not the [] syntax.
         # Instead, we specify the image again the command afterwards like a call to docker create. The result is a few environment variables
         # and the original command being appended to our hijacked docker create command. We can avoid any issues by adding || to prevent that
         # from every being executed as bash commands.
 
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11 # 4.1.1
 
       - name: Fetch git tags
         run: |
           git config --global --add safe.directory "$GITHUB_WORKSPACE"
           git fetch --tags origin
 
       - name: Configure pip cache
@@ -1081,12 +1083,12 @@
         run: |
           tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
         env:
           TOX_PARALLEL_NO_SPINNER: 1
           PY_COLORS: 0
 
       - name: Upload Coverage Artifacts
-        uses: actions/upload-artifact@v4
+        uses: actions/upload-artifact@5d5d22a31266ced268874388b861e4b58bb5c2f3 # 4.3.1
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
```

### Comparing `newrelic-9.8.0/.gitignore` & `newrelic-9.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/.mega-linter.yml` & `newrelic-9.9.0/.mega-linter.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/CONTRIBUTING.rst` & `newrelic-9.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/LICENSE` & `newrelic-9.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/PKG-INFO` & `newrelic-9.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic
-Version: 9.8.0
+Version: 9.9.0
 Summary: New Relic Python Agent
 Home-page: https://docs.newrelic.com/docs/apm/agents/python-agent/
 Author: New Relic
 Author-email: support@newrelic.com
 Maintainer: New Relic
 Maintainer-email: support@newrelic.com
 License: Apache-2.0
```

### Comparing `newrelic-9.8.0/README.rst` & `newrelic-9.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/ROADMAP.md` & `newrelic-9.9.0/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/THIRD_PARTY_NOTICES.md` & `newrelic-9.9.0/THIRD_PARTY_NOTICES.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/codecov.yml` & `newrelic-9.9.0/codecov.yml`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/__init__.py` & `newrelic-9.9.0/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/__init__.py` & `newrelic-9.9.0/newrelic/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/__main__.py` & `newrelic-9.9.0/newrelic/admin/__main__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/debug_console.py` & `newrelic-9.9.0/newrelic/admin/debug_console.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/generate_config.py` & `newrelic-9.9.0/newrelic/admin/generate_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/license_key.py` & `newrelic-9.9.0/newrelic/admin/license_key.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/local_config.py` & `newrelic-9.9.0/newrelic/admin/local_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/network_config.py` & `newrelic-9.9.0/newrelic/admin/network_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/record_deploy.py` & `newrelic-9.9.0/newrelic/admin/record_deploy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/run_program.py` & `newrelic-9.9.0/newrelic/admin/run_program.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/run_python.py` & `newrelic-9.9.0/newrelic/admin/run_python.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/server_config.py` & `newrelic-9.9.0/newrelic/admin/server_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/admin/validate_config.py` & `newrelic-9.9.0/newrelic/admin/validate_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/agent.py` & `newrelic-9.9.0/newrelic/agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/__init__.py` & `newrelic-9.9.0/newrelic/api/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/application.py` & `newrelic-9.9.0/newrelic/api/application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/asgi_application.py` & `newrelic-9.9.0/newrelic/api/asgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/background_task.py` & `newrelic-9.9.0/newrelic/api/background_task.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/cat_header_mixin.py` & `newrelic-9.9.0/newrelic/api/cat_header_mixin.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/database_trace.py` & `newrelic-9.9.0/newrelic/api/database_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/datastore_trace.py` & `newrelic-9.9.0/newrelic/api/datastore_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/error_trace.py` & `newrelic-9.9.0/newrelic/api/error_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/exceptions.py` & `newrelic-9.9.0/newrelic/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/external_trace.py` & `newrelic-9.9.0/newrelic/api/external_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/function_profile.py` & `newrelic-9.9.0/newrelic/api/function_profile.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/function_trace.py` & `newrelic-9.9.0/newrelic/api/function_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/generator_trace.py` & `newrelic-9.9.0/newrelic/api/generator_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/graphql_trace.py` & `newrelic-9.9.0/newrelic/api/graphql_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/html_insertion.py` & `newrelic-9.9.0/newrelic/api/html_insertion.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/import_hook.py` & `newrelic-9.9.0/newrelic/api/import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/in_function.py` & `newrelic-9.9.0/newrelic/api/in_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/lambda_handler.py` & `newrelic-9.9.0/newrelic/api/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/log.py` & `newrelic-9.9.0/newrelic/api/log.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/memcache_trace.py` & `newrelic-9.9.0/newrelic/api/memcache_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/message_trace.py` & `newrelic-9.9.0/newrelic/api/message_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/message_transaction.py` & `newrelic-9.9.0/newrelic/api/message_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/ml_model.py` & `newrelic-9.9.0/newrelic/api/ml_model.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/object_wrapper.py` & `newrelic-9.9.0/newrelic/api/object_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/out_function.py` & `newrelic-9.9.0/newrelic/api/out_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/post_function.py` & `newrelic-9.9.0/newrelic/api/post_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/pre_function.py` & `newrelic-9.9.0/newrelic/api/pre_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/profile_trace.py` & `newrelic-9.9.0/newrelic/api/profile_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/settings.py` & `newrelic-9.9.0/newrelic/api/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/solr_trace.py` & `newrelic-9.9.0/newrelic/api/solr_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/supportability.py` & `newrelic-9.9.0/newrelic/api/supportability.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/time_trace.py` & `newrelic-9.9.0/newrelic/api/time_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/transaction.py` & `newrelic-9.9.0/newrelic/api/transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/transaction_name.py` & `newrelic-9.9.0/newrelic/api/transaction_name.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/web_transaction.py` & `newrelic-9.9.0/newrelic/api/web_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/api/wsgi_application.py` & `newrelic-9.9.0/newrelic/api/wsgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/bootstrap/__init__.py` & `newrelic-9.9.0/newrelic/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/bootstrap/sitecustomize.py` & `newrelic-9.9.0/newrelic/bootstrap/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/__init__.py` & `newrelic-9.9.0/newrelic/common/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/_monotonic.c` & `newrelic-9.9.0/newrelic/common/_monotonic.c`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/agent_http.py` & `newrelic-9.9.0/newrelic/common/agent_http.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/async_proxy.py` & `newrelic-9.9.0/newrelic/common/async_proxy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/async_wrapper.py` & `newrelic-9.9.0/newrelic/common/async_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/cacert.pem` & `newrelic-9.9.0/newrelic/common/cacert.pem`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/certs.py` & `newrelic-9.9.0/newrelic/common/certs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/coroutine.py` & `newrelic-9.9.0/newrelic/common/coroutine.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/encoding_utils.py` & `newrelic-9.9.0/newrelic/common/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/log_file.py` & `newrelic-9.9.0/newrelic/common/log_file.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/metric_utils.py` & `newrelic-9.9.0/newrelic/common/metric_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/object_names.py` & `newrelic-9.9.0/newrelic/common/object_names.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/object_wrapper.py` & `newrelic-9.9.0/newrelic/common/object_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/package_version_utils.py` & `newrelic-9.9.0/newrelic/common/package_version_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/signature.py` & `newrelic-9.9.0/newrelic/common/signature.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/stopwatch.py` & `newrelic-9.9.0/newrelic/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/streaming_utils.py` & `newrelic-9.9.0/newrelic/common/streaming_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/system_info.py` & `newrelic-9.9.0/newrelic/common/system_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/common/utilization.py` & `newrelic-9.9.0/newrelic/common/utilization.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/config.py` & `newrelic-9.9.0/newrelic/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,15 @@
     _process_setting(section, "compressed_content_encoding", "get", _map_compressed_content_encoding)
     _process_setting(section, "attributes.enabled", "getboolean", None)
     _process_setting(section, "attributes.exclude", "get", _map_inc_excl_attributes)
     _process_setting(section, "attributes.include", "get", _map_inc_excl_attributes)
     _process_setting(section, "transaction_name.naming_scheme", "get", None)
     _process_setting(section, "gc_runtime_metrics.enabled", "getboolean", None)
     _process_setting(section, "gc_runtime_metrics.top_object_count_limit", "getint", None)
+    _process_setting(section, "memory_runtime_pid_metrics.enabled", "getboolean", None)
     _process_setting(section, "thread_profiler.enabled", "getboolean", None)
     _process_setting(section, "transaction_tracer.enabled", "getboolean", None)
     _process_setting(
         section,
         "transaction_tracer.transaction_threshold",
         "get",
         _map_transaction_threshold,
@@ -2248,14 +2249,26 @@
     _process_module_definition(
         "langchain_community.vectorstores.documentdb",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
+        "langchain_community.vectorstores.duckdb",
+        "newrelic.hooks.mlmodel_langchain",
+        "instrument_langchain_vectorstore_similarity_search",
+    )
+
+    _process_module_definition(
+        "langchain_community.vectorstores.ecloud_vector_search",
+        "newrelic.hooks.mlmodel_langchain",
+        "instrument_langchain_vectorstore_similarity_search",
+    )
+
+    _process_module_definition(
         "langchain_community.vectorstores.elastic_vector_search",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
         "langchain_community.vectorstores.elasticsearch",
@@ -2296,14 +2309,20 @@
     _process_module_definition(
         "langchain_community.vectorstores.infinispanvs",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
+        "langchain_community.vectorstores.inmemory",
+        "newrelic.hooks.mlmodel_langchain",
+        "instrument_langchain_vectorstore_similarity_search",
+    )
+
+    _process_module_definition(
         "langchain_community.vectorstores.kdbai",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
         "langchain_community.vectorstores.kinetica",
@@ -2386,14 +2405,20 @@
     _process_module_definition(
         "langchain_community.vectorstores.opensearch_vector_search",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
+        "langchain_community.vectorstores.pathway",
+        "newrelic.hooks.mlmodel_langchain",
+        "instrument_langchain_vectorstore_similarity_search",
+    )
+
+    _process_module_definition(
         "langchain_community.vectorstores.pgembedding",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
         "langchain_community.vectorstores.pgvecto_rs",
@@ -2530,14 +2555,20 @@
     _process_module_definition(
         "langchain_community.vectorstores.vald",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
+        "langchain_community.vectorstores.vdms",
+        "newrelic.hooks.mlmodel_langchain",
+        "instrument_langchain_vectorstore_similarity_search",
+    )
+
+    _process_module_definition(
         "langchain_community.vectorstores.vearch",
         "newrelic.hooks.mlmodel_langchain",
         "instrument_langchain_vectorstore_similarity_search",
     )
 
     _process_module_definition(
         "langchain_community.vectorstores.vectara",
@@ -4328,27 +4359,17 @@
     _process_module_definition(
         "celery.concurrency.prefork",
         "newrelic.hooks.application_celery",
         "instrument_celery_worker",
     )
 
     _process_module_definition(
-        "celery.execute.trace",
-        "newrelic.hooks.application_celery",
-        "instrument_celery_execute_trace",
-    )
-    _process_module_definition(
-        "celery.task.trace",
-        "newrelic.hooks.application_celery",
-        "instrument_celery_execute_trace",
-    )
-    _process_module_definition(
-        "celery.app.trace",
+        "celery.app.base",
         "newrelic.hooks.application_celery",
-        "instrument_celery_execute_trace",
+        "instrument_celery_app_base",
     )
     _process_module_definition("billiard.pool", "newrelic.hooks.application_celery", "instrument_billiard_pool")
 
     _process_module_definition("flup.server.cgi", "newrelic.hooks.adapter_flup", "instrument_flup_server_cgi")
     _process_module_definition(
         "flup.server.ajp_base",
         "newrelic.hooks.adapter_flup",
```

### Comparing `newrelic-9.8.0/newrelic/console.py` & `newrelic-9.9.0/newrelic/console.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/__init__.py` & `newrelic-9.9.0/newrelic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/_thread_utilization.c` & `newrelic-9.9.0/newrelic/core/_thread_utilization.c`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/adaptive_sampler.py` & `newrelic-9.9.0/newrelic/core/adaptive_sampler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/agent.py` & `newrelic-9.9.0/newrelic/core/agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/agent_protocol.py` & `newrelic-9.9.0/newrelic/core/agent_protocol.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/agent_streaming.py` & `newrelic-9.9.0/newrelic/core/agent_streaming.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/application.py` & `newrelic-9.9.0/newrelic/core/application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/attribute.py` & `newrelic-9.9.0/newrelic/core/attribute.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/attribute_filter.py` & `newrelic-9.9.0/newrelic/core/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/code_level_metrics.py` & `newrelic-9.9.0/newrelic/core/code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/config.py` & `newrelic-9.9.0/newrelic/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,18 @@
     pass
 
 
 class GCRuntimeMetricsSettings(Settings):
     enabled = False
 
 
+class MemoryRuntimeMetricsSettings(Settings):
+    pass
+
+
 class MachineLearningSettings(Settings):
     pass
 
 
 class MachineLearningInferenceEventsValueSettings(Settings):
     pass
 
@@ -442,14 +446,15 @@
 _settings.distributed_tracing = DistributedTracingSettings()
 _settings.error_collector = ErrorCollectorSettings()
 _settings.error_collector.attributes = ErrorCollectorAttributesSettings()
 _settings.event_harvest_config = EventHarvestConfigSettings()
 _settings.event_harvest_config.harvest_limits = EventHarvestConfigHarvestLimitSettings()
 _settings.event_loop_visibility = EventLoopVisibilitySettings()
 _settings.gc_runtime_metrics = GCRuntimeMetricsSettings()
+_settings.memory_runtime_pid_metrics = MemoryRuntimeMetricsSettings()
 _settings.heroku = HerokuSettings()
 _settings.infinite_tracing = InfiniteTracingSettings()
 _settings.instrumentation = InstrumentationSettings()
 _settings.instrumentation.graphql = InstrumentationGraphQLSettings()
 _settings.message_tracer = MessageTracerSettings()
 _settings.process_host = ProcessHostSettings()
 _settings.rum = RumSettings()
@@ -736,14 +741,18 @@
 
 _settings.thread_profiler.enabled = True
 _settings.cross_application_tracer.enabled = False
 
 _settings.gc_runtime_metrics.enabled = False
 _settings.gc_runtime_metrics.top_object_count_limit = 5
 
+_settings.memory_runtime_pid_metrics.enabled = _environ_as_bool(
+    "NEW_RELIC_MEMORY_RUNTIME_PID_METRICS_ENABLED", default=True
+)
+
 _settings.transaction_events.enabled = True
 _settings.transaction_events.attributes.enabled = True
 _settings.transaction_events.attributes.exclude = []
 _settings.transaction_events.attributes.include = []
 
 _settings.custom_insights_events.enabled = True
 _settings.custom_insights_events.max_attribute_value = _environ_as_int(
```

### Comparing `newrelic-9.8.0/newrelic/core/context.py` & `newrelic-9.9.0/newrelic/core/context.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/custom_event.py` & `newrelic-9.9.0/newrelic/core/custom_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/data_collector.py` & `newrelic-9.9.0/newrelic/core/data_collector.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/database_node.py` & `newrelic-9.9.0/newrelic/core/database_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/database_utils.py` & `newrelic-9.9.0/newrelic/core/database_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/datastore_node.py` & `newrelic-9.9.0/newrelic/core/datastore_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/environment.py` & `newrelic-9.9.0/newrelic/core/environment.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/error_collector.py` & `newrelic-9.9.0/newrelic/core/error_collector.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/error_node.py` & `newrelic-9.9.0/newrelic/core/error_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/external_node.py` & `newrelic-9.9.0/newrelic/core/external_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/function_node.py` & `newrelic-9.9.0/newrelic/core/function_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/graphql_node.py` & `newrelic-9.9.0/newrelic/core/graphql_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/graphql_utils.py` & `newrelic-9.9.0/newrelic/core/graphql_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/infinite_tracing_pb2.py` & `newrelic-9.9.0/newrelic/core/infinite_tracing_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/infinite_tracing_v3_pb2.py` & `newrelic-9.9.0/newrelic/core/infinite_tracing_v3_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/infinite_tracing_v4_pb2.py` & `newrelic-9.9.0/newrelic/core/infinite_tracing_v4_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/internal_metrics.py` & `newrelic-9.9.0/newrelic/core/internal_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/log_event_node.py` & `newrelic-9.9.0/newrelic/core/log_event_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/loop_node.py` & `newrelic-9.9.0/newrelic/core/loop_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/memcache_node.py` & `newrelic-9.9.0/newrelic/core/memcache_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/message_node.py` & `newrelic-9.9.0/newrelic/core/message_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/metric.py` & `newrelic-9.9.0/newrelic/core/metric.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/node_mixin.py` & `newrelic-9.9.0/newrelic/core/node_mixin.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/otlp_utils.py` & `newrelic-9.9.0/newrelic/core/otlp_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/profile_sessions.py` & `newrelic-9.9.0/newrelic/core/profile_sessions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/root_node.py` & `newrelic-9.9.0/newrelic/core/root_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/rules_engine.py` & `newrelic-9.9.0/newrelic/core/rules_engine.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/solr_node.py` & `newrelic-9.9.0/newrelic/core/solr_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/stack_trace.py` & `newrelic-9.9.0/newrelic/core/stack_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/stats_engine.py` & `newrelic-9.9.0/newrelic/core/stats_engine.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/string_table.py` & `newrelic-9.9.0/newrelic/core/string_table.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/thread_utilization.py` & `newrelic-9.9.0/newrelic/core/thread_utilization.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/trace_cache.py` & `newrelic-9.9.0/newrelic/core/trace_cache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/trace_node.py` & `newrelic-9.9.0/newrelic/core/trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/core/transaction_node.py` & `newrelic-9.9.0/newrelic/core/transaction_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/extras/__init__.py` & `newrelic-9.9.0/newrelic/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/extras/framework_django/__init__.py` & `newrelic-9.9.0/newrelic/extras/framework_django/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/extras/framework_django/templatetags/__init__.py` & `newrelic-9.9.0/newrelic/extras/framework_django/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/extras/framework_django/templatetags/newrelic_tags.py` & `newrelic-9.9.0/newrelic/extras/framework_django/templatetags/newrelic_tags.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/__init__.py` & `newrelic-9.9.0/newrelic/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_asgiref.py` & `newrelic-9.9.0/newrelic/hooks/adapter_asgiref.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_cheroot.py` & `newrelic-9.9.0/newrelic/hooks/adapter_cheroot.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_cherrypy.py` & `newrelic-9.9.0/newrelic/hooks/adapter_cherrypy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_daphne.py` & `newrelic-9.9.0/newrelic/hooks/adapter_daphne.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_flup.py` & `newrelic-9.9.0/newrelic/hooks/adapter_flup.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_gevent.py` & `newrelic-9.9.0/newrelic/hooks/adapter_gevent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_gunicorn.py` & `newrelic-9.9.0/newrelic/hooks/adapter_gunicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_hypercorn.py` & `newrelic-9.9.0/newrelic/hooks/adapter_hypercorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_meinheld.py` & `newrelic-9.9.0/newrelic/hooks/adapter_meinheld.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_paste.py` & `newrelic-9.9.0/newrelic/hooks/adapter_paste.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_uvicorn.py` & `newrelic-9.9.0/newrelic/hooks/adapter_uvicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_waitress.py` & `newrelic-9.9.0/newrelic/hooks/adapter_waitress.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/adapter_wsgiref.py` & `newrelic-9.9.0/newrelic/hooks/adapter_wsgiref.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/application_celery.py` & `newrelic-9.9.0/newrelic/hooks/application_celery.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,54 +21,56 @@
 """
 
 import functools
 
 from newrelic.api.application import application_instance
 from newrelic.api.background_task import BackgroundTask
 from newrelic.api.function_trace import FunctionTrace
+from newrelic.api.message_trace import MessageTrace
 from newrelic.api.pre_function import wrap_pre_function
-from newrelic.common.object_names import callable_name
-from newrelic.common.object_wrapper import FunctionWrapper
 from newrelic.api.transaction import current_transaction
+from newrelic.common.object_wrapper import FunctionWrapper, wrap_function_wrapper
 from newrelic.core.agent import shutdown_agent
 
+UNKNOWN_TASK_NAME = "<Unknown Task>"
+MAPPING_TASK_NAMES = {"celery.starmap", "celery.map"}
 
-def CeleryTaskWrapper(wrapped, application=None, name=None):
 
-    def wrapper(wrapped, instance, args, kwargs):
-        transaction = current_transaction(active_only=False)
+def task_name(*args, **kwargs):
+    # Grab the current task, which can be located in either place
+    if args:
+        task = args[0]
+    elif "task" in kwargs:
+        task = kwargs["task"]
+    else:
+        return UNKNOWN_TASK_NAME  # Failsafe
+
+    # Task can be either a task instance or a signature, which subclasses dict, or an actual dict in some cases.
+    task_name = getattr(task, "name", None) or task.get("task", UNKNOWN_TASK_NAME)
+
+    # Under mapping tasks, the root task name isn't descriptive enough so we append the
+    # subtask name to differentiate between different mapping tasks
+    if task_name in MAPPING_TASK_NAMES:
+        try:
+            subtask = kwargs["task"]["task"]
+            task_name = "/".join((task_name, subtask))
+        except Exception:
+            pass
 
-        if callable(name):
-            # Start Hotfix v2.2.1.
-            # if instance and inspect.ismethod(wrapped):
-            #     _name = name(instance, *args, **kwargs)
-            # else:
-            #     _name = name(*args, **kwargs)
+    return task_name
 
-            if instance is not None:
-                _name = name(instance, *args, **kwargs)
-            else:
-                _name = name(*args, **kwargs)
-            # End Hotfix v2.2.1.
 
-        elif name is None:
-            _name = callable_name(wrapped)
+def CeleryTaskWrapper(wrapped):
+    def wrapper(wrapped, instance, args, kwargs):
+        transaction = current_transaction(active_only=False)
 
+        if instance is not None:
+            _name = task_name(instance, *args, **kwargs)
         else:
-            _name = name
-
-        # Helper for obtaining the appropriate application object. If
-        # has an activate() method assume it is a valid application
-        # object. Don't check by type so se can easily mock it for
-        # testing if need be.
-
-        def _application():
-            if hasattr(application, 'activate'):
-                return application
-            return application_instance(application)
+            _name = task_name(*args, **kwargs)
 
         # A Celery Task can be called either outside of a transaction, or
         # within the context of an existing transaction. There are 3
         # possibilities we need to handle:
         #
         #   1. In an inactive transaction
         #
@@ -83,111 +85,134 @@
         #
         #   3. Outside of a transaction
         #
         #      This is the typical case for a celery Task. Since it's not
         #      running inside of an existing transaction, we want to create
         #      a new background transaction for it.
 
-        if transaction and (transaction.ignore_transaction or
-                transaction.stopped):
+        if transaction and (transaction.ignore_transaction or transaction.stopped):
             return wrapped(*args, **kwargs)
 
         elif transaction:
             with FunctionTrace(_name, source=instance):
                 return wrapped(*args, **kwargs)
 
         else:
-            with BackgroundTask(_application(), _name, 'Celery', source=instance):
+            with BackgroundTask(application_instance(), _name, "Celery", source=instance) as transaction:
+                # Attempt to grab distributed tracing headers
+                try:
+                    # Headers on earlier versions of Celery may end up as attributes
+                    # on the request context instead of as custom headers. Handler this
+                    # by defaulting to using vars() if headers is not available
+                    request = instance.request
+                    headers = getattr(request, "headers", None) or vars(request)
+
+                    settings = transaction.settings
+                    if headers is not None and settings is not None:
+                        if settings.distributed_tracing.enabled:
+                            transaction.accept_distributed_trace_headers(headers, transport_type="AMQP")
+                        elif transaction.settings.cross_application_tracer.enabled:
+                            transaction._process_incoming_cat_headers(
+                                headers.get(MessageTrace.cat_id_key, None),
+                                headers.get(MessageTrace.cat_transaction_key, None),
+                            )
+                except Exception:
+                    pass
+
                 return wrapped(*args, **kwargs)
 
     # Celery tasks that inherit from celery.app.task must implement a run()
     # method.
     # ref: (http://docs.celeryproject.org/en/2.5/reference/
     #                            celery.app.task.html#celery.app.task.BaseTask)
     # Celery task's __call__ method then calls the run() method to execute the
     # task. But celery does a micro-optimization where if the __call__ method
     # was not overridden by an inherited task, then it will directly execute
     # the run() method without going through the __call__ method. Our
     # instrumentation via FunctionWrapper() relies on __call__ being called which
     # in turn executes the wrapper() function defined above. Since the micro
     # optimization bypasses __call__ method it breaks our instrumentation of
-    # celery. To circumvent this problem, we added a run() attribute to our
+    # celery.
+    #
+    # For versions of celery 2.5.3 to 2.5.5+
+    # Celery has included a monkey-patching provision which did not perform this
+    # optimization on functions that were monkey-patched. Unfortunately, our
+    # wrappers are too transparent for celery to detect that they've even been
+    # monky-patched. To circumvent this, we set the __module__ of our wrapped task
+    # to this file which causes celery to properly detect that it has been patched.
+    #
+    # For versions of celery 2.5.3 to 2.5.5
+    # To circumvent this problem, we added a run() attribute to our
     # FunctionWrapper which points to our __call__ method. This causes Celery
     # to execute our __call__ method which in turn applies the wrapper
     # correctly before executing the task.
-    #
-    # This is only a problem in Celery versions 2.5.3 to 2.5.5. The later
-    # versions included a monkey-patching provision which did not perform this
-    # optimization on functions that were monkey-patched.
 
     class TaskWrapper(FunctionWrapper):
         def run(self, *args, **kwargs):
             return self.__call__(*args, **kwargs)
 
-    return TaskWrapper(wrapped, wrapper)
+    wrapped_task = TaskWrapper(wrapped, wrapper)
+    # Reset __module__ to be less transparent so celery detects our monkey-patching
+    wrapped_task.__module__ = CeleryTaskWrapper.__module__
 
+    return wrapped_task
 
-def instrument_celery_app_task(module):
 
+def instrument_celery_app_task(module):
     # Triggered for both 'celery.app.task' and 'celery.task.base'.
 
-    if hasattr(module, 'BaseTask'):
-
+    if hasattr(module, "BaseTask"):
         # Need to add a wrapper for background task entry point.
 
         # In Celery 2.2 the 'BaseTask' class actually resided in the
         # module 'celery.task.base'. In Celery 2.3 the 'BaseTask' class
         # moved to 'celery.app.task' but an alias to it was retained in
         # the module 'celery.task.base'. We need to detect both module
         # imports, but we check the module name associated with
         # 'BaseTask' to ensure that we do not instrument the class via
         # the alias in Celery 2.3 and later.
 
         # In Celery 2.5+, although 'BaseTask' still exists execution of
         # the task doesn't pass through it. For Celery 2.5+ need to wrap
         # the tracer instead.
 
-        def task_name(task, *args, **kwargs):
-            return task.name
-
         if module.BaseTask.__module__ == module.__name__:
-            module.BaseTask.__call__ = CeleryTaskWrapper(
-                    module.BaseTask.__call__, name=task_name)
+            module.BaseTask.__call__ = CeleryTaskWrapper(module.BaseTask.__call__)
 
 
-def instrument_celery_execute_trace(module):
-
-    # Triggered for 'celery.execute_trace'.
+def wrap_Celery_send_task(wrapped, instance, args, kwargs):
+    transaction = current_transaction()
+    if not transaction:
+        return wrapped(*args, **kwargs)
+
+    # Merge distributed tracing headers into outgoing task headers
+    try:
+        dt_headers = MessageTrace.generate_request_headers(transaction)
+        original_headers = kwargs.get("headers", None)
+        if dt_headers:
+            if not original_headers:
+                kwargs["headers"] = dict(dt_headers)
+            else:
+                kwargs["headers"] = dt_headers = dict(dt_headers)
+                dt_headers.update(dict(original_headers))
+    except Exception:
+        pass
 
-    if hasattr(module, 'build_tracer'):
+    return wrapped(*args, **kwargs)
 
-        # Need to add a wrapper for background task entry point.
 
-        # In Celery 2.5+ we need to wrap the task when tracer is being
-        # created. Note that in Celery 2.5 the 'build_tracer' function
-        # actually resided in the module 'celery.execute.task'. In
-        # Celery 3.0 the 'build_tracer' function moved to
-        # 'celery.task.trace'.
-
-        _build_tracer = module.build_tracer
-
-        def build_tracer(name, task, *args, **kwargs):
-            task = task or module.tasks[name]
-            task = CeleryTaskWrapper(task, name=name)
-            return _build_tracer(name, task, *args, **kwargs)
-
-        module.build_tracer = build_tracer
+def instrument_celery_app_base(module):
+    if hasattr(module, "Celery") and hasattr(module.Celery, "send_task"):
+        wrap_function_wrapper(module, "Celery.send_task", wrap_Celery_send_task)
 
 
 def instrument_celery_worker(module):
-
     # Triggered for 'celery.worker' and 'celery.concurrency.processes'.
 
-    if hasattr(module, 'process_initializer'):
-
+    if hasattr(module, "process_initializer"):
         # We try and force registration of default application after
         # fork of worker process rather than lazily on first request.
 
         # Originally the 'process_initializer' function was located in
         # 'celery.worker'. In Celery 2.5 the function 'process_initializer'
         # was moved to the module 'celery.concurrency.processes'.
 
@@ -198,22 +223,19 @@
             application_instance().activate()
             return _process_initializer(*args, **kwargs)
 
         module.process_initializer = process_initializer
 
 
 def instrument_celery_loaders_base(module):
-
     def force_application_activation(*args, **kwargs):
         application_instance().activate()
 
-    wrap_pre_function(module, 'BaseLoader.init_worker',
-            force_application_activation)
+    wrap_pre_function(module, "BaseLoader.init_worker", force_application_activation)
 
 
 def instrument_billiard_pool(module):
-
     def force_agent_shutdown(*args, **kwargs):
         shutdown_agent()
 
-    if hasattr(module, 'Worker'):
-        wrap_pre_function(module, 'Worker._do_exit', force_agent_shutdown)
+    if hasattr(module, "Worker"):
+        wrap_pre_function(module, "Worker._do_exit", force_agent_shutdown)
```

### Comparing `newrelic-9.8.0/newrelic/hooks/application_gearman.py` & `newrelic-9.9.0/newrelic/hooks/application_gearman.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/component_cornice.py` & `newrelic-9.9.0/newrelic/hooks/component_cornice.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/component_djangorestframework.py` & `newrelic-9.9.0/newrelic/hooks/component_djangorestframework.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/component_flask_rest.py` & `newrelic-9.9.0/newrelic/hooks/component_flask_rest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/component_graphqlserver.py` & `newrelic-9.9.0/newrelic/hooks/component_graphqlserver.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/component_piston.py` & `newrelic-9.9.0/newrelic/hooks/component_piston.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/component_sentry.py` & `newrelic-9.9.0/newrelic/hooks/component_sentry.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/component_tastypie.py` & `newrelic-9.9.0/newrelic/hooks/component_tastypie.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/coroutines_asyncio.py` & `newrelic-9.9.0/newrelic/hooks/coroutines_asyncio.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/coroutines_gevent.py` & `newrelic-9.9.0/newrelic/hooks/coroutines_gevent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_asyncpg.py` & `newrelic-9.9.0/newrelic/hooks/database_asyncpg.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_cx_oracle.py` & `newrelic-9.9.0/newrelic/hooks/database_cx_oracle.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_dbapi2.py` & `newrelic-9.9.0/newrelic/hooks/database_dbapi2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_ibm_db_dbi.py` & `newrelic-9.9.0/newrelic/hooks/database_ibm_db_dbi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_mysql.py` & `newrelic-9.9.0/newrelic/hooks/database_mysql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_mysqldb.py` & `newrelic-9.9.0/newrelic/hooks/database_mysqldb.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_oursql.py` & `newrelic-9.9.0/newrelic/hooks/database_oursql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_postgresql.py` & `newrelic-9.9.0/newrelic/hooks/database_postgresql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_psycopg2.py` & `newrelic-9.9.0/newrelic/hooks/database_psycopg2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_psycopg2cffi.py` & `newrelic-9.9.0/newrelic/hooks/database_psycopg2cffi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_psycopg2ct.py` & `newrelic-9.9.0/newrelic/hooks/database_psycopg2ct.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_pymssql.py` & `newrelic-9.9.0/newrelic/hooks/database_pymssql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_pymysql.py` & `newrelic-9.9.0/newrelic/hooks/database_pymysql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_pyodbc.py` & `newrelic-9.9.0/newrelic/hooks/database_pyodbc.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/database_sqlite.py` & `newrelic-9.9.0/newrelic/hooks/database_sqlite.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_aioredis.py` & `newrelic-9.9.0/newrelic/hooks/datastore_aioredis.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_aredis.py` & `newrelic-9.9.0/newrelic/hooks/datastore_aredis.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_bmemcached.py` & `newrelic-9.9.0/newrelic/hooks/datastore_bmemcached.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_elasticsearch.py` & `newrelic-9.9.0/newrelic/hooks/datastore_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_firestore.py` & `newrelic-9.9.0/newrelic/hooks/datastore_firestore.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_memcache.py` & `newrelic-9.9.0/newrelic/hooks/datastore_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_motor.py` & `newrelic-9.9.0/newrelic/hooks/datastore_motor.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_pyelasticsearch.py` & `newrelic-9.9.0/newrelic/hooks/datastore_pyelasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_pylibmc.py` & `newrelic-9.9.0/newrelic/hooks/datastore_pylibmc.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_pymemcache.py` & `newrelic-9.9.0/newrelic/hooks/datastore_pymemcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_pymongo.py` & `newrelic-9.9.0/newrelic/hooks/datastore_pymongo.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_pysolr.py` & `newrelic-9.9.0/newrelic/hooks/datastore_pysolr.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_redis.py` & `newrelic-9.9.0/newrelic/hooks/datastore_redis.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_solrpy.py` & `newrelic-9.9.0/newrelic/hooks/datastore_solrpy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/datastore_umemcache.py` & `newrelic-9.9.0/newrelic/hooks/datastore_umemcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_botocore.py` & `newrelic-9.9.0/newrelic/hooks/external_botocore.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,18 @@
         chat_completion_message_dict.update(llm_metadata_dict)
 
         transaction.record_custom_event("LlmChatCompletionMessage", chat_completion_message_dict)
 
     for index, message in enumerate(output_message_list):
         index += len(input_message_list)
         content = message.get("content", "")
+        # For anthropic models run via langchain, a list is returned with a dictionary of content inside
+        # We only want to report the raw dictionary in the LLM message event
+        if isinstance(content, list) and len(content) == 1:
+            content = content[0]
 
         if response_id:
             id_ = "%s-%d" % (response_id, index)  # Response ID was set, append message index to it.
         else:
             id_ = str(uuid.uuid4())  # No response IDs, use random UUID
 
         chat_completion_message_dict = {
@@ -258,29 +262,27 @@
     if "messages" in request_body:
         input_message_list = [
             {"role": message.get("role", "user"), "content": message.get("content")}
             for message in request_body.get("messages")
         ]
     else:
         input_message_list = [{"role": "user", "content": request_body.get("prompt")}]
-
     bedrock_attrs["request.max_tokens"] = request_body.get("max_tokens_to_sample")
     bedrock_attrs["request.temperature"] = request_body.get("temperature")
     bedrock_attrs["input_message_list"] = input_message_list
 
     return bedrock_attrs
 
 
 def extract_bedrock_claude_model_response(response_body, bedrock_attrs):
     if response_body:
         response_body = json.loads(response_body)
         role = response_body.get("role", "assistant")
         content = response_body.get("content") or response_body.get("completion")
         output_message_list = [{"role": role, "content": content}]
-
         bedrock_attrs["response.choices.finish_reason"] = response_body.get("stop_reason")
         bedrock_attrs["output_message_list"] = output_message_list
 
     return bedrock_attrs
 
 
 def extract_bedrock_claude_model_streaming_response(response_body, bedrock_attrs):
```

### Comparing `newrelic-9.8.0/newrelic/hooks/external_dropbox.py` & `newrelic-9.9.0/newrelic/hooks/external_dropbox.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_facepy.py` & `newrelic-9.9.0/newrelic/hooks/external_facepy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_feedparser.py` & `newrelic-9.9.0/newrelic/hooks/external_feedparser.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_httplib.py` & `newrelic-9.9.0/newrelic/hooks/external_httplib.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_httplib2.py` & `newrelic-9.9.0/newrelic/hooks/external_httplib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_httpx.py` & `newrelic-9.9.0/newrelic/hooks/external_httpx.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_pywapi.py` & `newrelic-9.9.0/newrelic/hooks/external_pywapi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_requests.py` & `newrelic-9.9.0/newrelic/hooks/external_requests.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_thrift.py` & `newrelic-9.9.0/newrelic/hooks/external_thrift.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_urllib.py` & `newrelic-9.9.0/newrelic/hooks/external_urllib.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_urllib2.py` & `newrelic-9.9.0/newrelic/hooks/external_urllib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_urllib3.py` & `newrelic-9.9.0/newrelic/hooks/external_urllib3.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/external_xmlrpclib.py` & `newrelic-9.9.0/newrelic/hooks/external_xmlrpclib.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_aiohttp.py` & `newrelic-9.9.0/newrelic/hooks/framework_aiohttp.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_ariadne.py` & `newrelic-9.9.0/newrelic/hooks/framework_ariadne.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_bottle.py` & `newrelic-9.9.0/newrelic/hooks/framework_bottle.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_cherrypy.py` & `newrelic-9.9.0/newrelic/hooks/framework_cherrypy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_django.py` & `newrelic-9.9.0/newrelic/hooks/framework_django.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_django_py3.py` & `newrelic-9.9.0/newrelic/hooks/framework_django_py3.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_falcon.py` & `newrelic-9.9.0/newrelic/hooks/framework_falcon.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_fastapi.py` & `newrelic-9.9.0/newrelic/hooks/framework_fastapi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_flask.py` & `newrelic-9.9.0/newrelic/hooks/framework_flask.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_graphene.py` & `newrelic-9.9.0/newrelic/hooks/framework_graphene.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_graphql.py` & `newrelic-9.9.0/newrelic/hooks/framework_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_graphql_py3.py` & `newrelic-9.9.0/newrelic/hooks/framework_graphql_py3.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_grpc.py` & `newrelic-9.9.0/newrelic/hooks/framework_grpc.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_pylons.py` & `newrelic-9.9.0/newrelic/hooks/framework_pylons.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_pyramid.py` & `newrelic-9.9.0/newrelic/hooks/framework_pyramid.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_sanic.py` & `newrelic-9.9.0/newrelic/hooks/framework_sanic.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_starlette.py` & `newrelic-9.9.0/newrelic/hooks/framework_starlette.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_strawberry.py` & `newrelic-9.9.0/newrelic/hooks/framework_strawberry.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_tornado.py` & `newrelic-9.9.0/newrelic/hooks/framework_tornado.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_web2py.py` & `newrelic-9.9.0/newrelic/hooks/framework_web2py.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/framework_webpy.py` & `newrelic-9.9.0/newrelic/hooks/framework_webpy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/logger_logging.py` & `newrelic-9.9.0/newrelic/hooks/logger_logging.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/logger_loguru.py` & `newrelic-9.9.0/newrelic/hooks/logger_loguru.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/logger_structlog.py` & `newrelic-9.9.0/newrelic/hooks/logger_structlog.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/memcache_memcache.py` & `newrelic-9.9.0/newrelic/hooks/memcache_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/messagebroker_confluentkafka.py` & `newrelic-9.9.0/newrelic/hooks/messagebroker_confluentkafka.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/messagebroker_kafkapython.py` & `newrelic-9.9.0/newrelic/hooks/messagebroker_kafkapython.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/messagebroker_pika.py` & `newrelic-9.9.0/newrelic/hooks/messagebroker_pika.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/middleware_flask_compress.py` & `newrelic-9.9.0/newrelic/hooks/middleware_flask_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/middleware_weberror.py` & `newrelic-9.9.0/newrelic/hooks/middleware_weberror.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/mlmodel_langchain.py` & `newrelic-9.9.0/newrelic/hooks/mlmodel_langchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,23 +50,26 @@
     "langchain_community.vectorstores.clickhouse": "Clickhouse",
     "langchain_community.vectorstores.couchbase": "CouchbaseVectorStore",
     "langchain_community.vectorstores.dashvector": "DashVector",
     "langchain_community.vectorstores.databricks_vector_search": "DatabricksVectorSearch",
     "langchain_community.vectorstores.deeplake": "DeepLake",
     "langchain_community.vectorstores.dingo": "Dingo",
     "langchain_community.vectorstores.documentdb": "DocumentDBVectorSearch",
+    "langchain_community.vectorstores.duckdb": "DuckDB",
+    "langchain_community.vectorstores.ecloud_vector_search": "EcloudESVectorStore",
     "langchain_community.vectorstores.elastic_vector_search": "ElasticVectorSearch",
     # "langchain_community.vectorstores.elastic_vector_search": "ElasticKnnSearch", # Deprecated
     "langchain_community.vectorstores.elasticsearch": "ElasticsearchStore",
     "langchain_community.vectorstores.epsilla": "Epsilla",
     "langchain_community.vectorstores.faiss": "FAISS",
     "langchain_community.vectorstores.hanavector": "HanaDB",
     "langchain_community.vectorstores.hippo": "Hippo",
     "langchain_community.vectorstores.hologres": "Hologres",
     "langchain_community.vectorstores.infinispanvs": "InfinispanVS",
+    "langchain_community.vectorstores.inmemory": "InMemoryVectorStore",
     "langchain_community.vectorstores.kdbai": "KDBAI",
     "langchain_community.vectorstores.kinetica": "Kinetica",
     "langchain_community.vectorstores.lancedb": "LanceDB",
     "langchain_community.vectorstores.lantern": "Lantern",
     "langchain_community.vectorstores.llm_rails": "LLMRails",
     "langchain_community.vectorstores.marqo": "Marqo",
     "langchain_community.vectorstores.matching_engine": "MatchingEngine",
@@ -75,14 +78,15 @@
     "langchain_community.vectorstores.momento_vector_index": "MomentoVectorIndex",
     "langchain_community.vectorstores.mongodb_atlas": "MongoDBAtlasVectorSearch",
     "langchain_community.vectorstores.myscale": "MyScale",
     "langchain_community.vectorstores.neo4j_vector": "Neo4jVector",
     "langchain_community.vectorstores.thirdai_neuraldb": "NeuralDBVectorStore",
     "langchain_community.vectorstores.nucliadb": "NucliaDB",
     "langchain_community.vectorstores.opensearch_vector_search": "OpenSearchVectorSearch",
+    "langchain_community.vectorstores.pathway": "PathwayVectorClient",
     "langchain_community.vectorstores.pgembedding": "PGEmbedding",
     "langchain_community.vectorstores.pgvecto_rs": "PGVecto_rs",
     "langchain_community.vectorstores.pgvector": "PGVector",
     "langchain_community.vectorstores.pinecone": "Pinecone",
     "langchain_community.vectorstores.qdrant": "Qdrant",
     "langchain_community.vectorstores.redis.base": "Redis",
     "langchain_community.vectorstores.rocksetdb": "Rockset",
@@ -99,14 +103,15 @@
     "langchain_community.vectorstores.tidb_vector": "TiDBVectorStore",
     "langchain_community.vectorstores.tigris": "Tigris",
     "langchain_community.vectorstores.tiledb": "TileDB",
     "langchain_community.vectorstores.timescalevector": "TimescaleVector",
     "langchain_community.vectorstores.typesense": "Typesense",
     "langchain_community.vectorstores.usearch": "USearch",
     "langchain_community.vectorstores.vald": "Vald",
+    "langchain_community.vectorstores.vdms": "VDMS",
     "langchain_community.vectorstores.vearch": "Vearch",
     "langchain_community.vectorstores.vectara": "Vectara",
     "langchain_community.vectorstores.vespa": "VespaStore",
     "langchain_community.vectorstores.weaviate": "Weaviate",
     "langchain_community.vectorstores.xata": "XataVectorStore",
     "langchain_community.vectorstores.yellowbrick": "Yellowbrick",
     "langchain_community.vectorstores.zep": "ZepVectorStore",
```

### Comparing `newrelic-9.8.0/newrelic/hooks/mlmodel_openai.py` & `newrelic-9.9.0/newrelic/hooks/mlmodel_openai.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/mlmodel_sklearn.py` & `newrelic-9.9.0/newrelic/hooks/mlmodel_sklearn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/template_genshi.py` & `newrelic-9.9.0/newrelic/hooks/template_genshi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/template_jinja2.py` & `newrelic-9.9.0/newrelic/hooks/template_jinja2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/hooks/template_mako.py` & `newrelic-9.9.0/newrelic/hooks/template_mako.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/network/__init__.py` & `newrelic-9.9.0/newrelic/network/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/network/addresses.py` & `newrelic-9.9.0/newrelic/network/addresses.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/network/exceptions.py` & `newrelic-9.9.0/newrelic/network/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/newrelic.ini` & `newrelic-9.9.0/newrelic/newrelic.ini`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/asgiref_compatibility.py` & `newrelic-9.9.0/newrelic/packages/asgiref_compatibility.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/isort/LICENSE` & `newrelic-9.9.0/newrelic/packages/isort/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/isort/stdlibs/py27.py` & `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py27.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/isort/stdlibs/py310.py` & `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py310.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/isort/stdlibs/py311.py` & `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py311.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/isort/stdlibs/py36.py` & `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py36.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/isort/stdlibs/py37.py` & `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py37.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/isort/stdlibs/py38.py` & `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py38.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/isort/stdlibs/py39.py` & `newrelic-9.9.0/newrelic/packages/isort/stdlibs/py39.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/opentelemetry_proto/LICENSE.txt` & `newrelic-9.9.0/newrelic/packages/opentelemetry_proto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/opentelemetry_proto/common_pb2.py` & `newrelic-9.9.0/newrelic/packages/opentelemetry_proto/common_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/opentelemetry_proto/logs_pb2.py` & `newrelic-9.9.0/newrelic/packages/opentelemetry_proto/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/opentelemetry_proto/metrics_pb2.py` & `newrelic-9.9.0/newrelic/packages/opentelemetry_proto/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/opentelemetry_proto/resource_pb2.py` & `newrelic-9.9.0/newrelic/packages/opentelemetry_proto/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/six.py` & `newrelic-9.9.0/newrelic/packages/six.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/LICENSE.txt` & `newrelic-9.9.0/newrelic/packages/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/__init__.py` & `newrelic-9.9.0/newrelic/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/_collections.py` & `newrelic-9.9.0/newrelic/packages/urllib3/_collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,14 +264,32 @@
         except KeyError:
             if default is self.__marker:
                 return []
             return default
         else:
             return vals[1:]
 
+    def _prepare_for_method_change(self):
+        """
+        Remove content-specific header fields before changing the request
+        method to GET or HEAD according to RFC 9110, Section 15.4.
+        """
+        content_specific_headers = [
+            "Content-Encoding",
+            "Content-Language",
+            "Content-Location",
+            "Content-Type",
+            "Content-Length",
+            "Digest",
+            "Last-Modified",
+        ]
+        for header in content_specific_headers:
+            self.discard(header)
+        return self
+
     # Backwards compatibility for httplib
     getheaders = getlist
     getallmatchingheaders = getlist
     iget = getlist
 
     # Backwards compatibility for http.cookiejar
     get_all = getlist
```

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/connection.py` & `newrelic-9.9.0/newrelic/packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/connectionpool.py` & `newrelic-9.9.0/newrelic/packages/urllib3/connectionpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 import socket
 import sys
 import warnings
 from socket import error as SocketError
 from socket import timeout as SocketTimeout
 
+from ._collections import HTTPHeaderDict
 from .connection import (
     BaseSSLError,
     BrokenPipeError,
     DummyConnection,
     HTTPConnection,
     HTTPException,
     HTTPSConnection,
@@ -46,14 +47,21 @@
 from .util.retry import Retry
 from .util.ssl_match_hostname import CertificateError
 from .util.timeout import Timeout
 from .util.url import Url, _encode_target
 from .util.url import _normalize_host as normalize_host
 from .util.url import get_host, parse_url
 
+try:  # Platform-specific: Python 3
+    import weakref
+
+    weakref_finalize = weakref.finalize
+except AttributeError:  # Platform-specific: Python 2
+    from .packages.backports.weakref_finalize import weakref_finalize
+
 xrange = six.moves.xrange
 
 log = logging.getLogger(__name__)
 
 _Default = object()
 
 
@@ -216,14 +224,24 @@
             # We cannot know if the user has added default socket options, so we cannot replace the
             # list.
             self.conn_kw.setdefault("socket_options", [])
 
             self.conn_kw["proxy"] = self.proxy
             self.conn_kw["proxy_config"] = self.proxy_config
 
+        # Do not pass 'self' as callback to 'finalize'.
+        # Then the 'finalize' would keep an endless living (leak) to self.
+        # By just passing a reference to the pool allows the garbage collector
+        # to free self if nobody else has a reference to it.
+        pool = self.pool
+
+        # Close all the HTTPConnections in the pool before the
+        # HTTPConnectionPool object is garbage collected.
+        weakref_finalize(self, _close_pool_connections, pool)
+
     def _new_conn(self):
         """
         Return a fresh :class:`HTTPConnection`.
         """
         self.num_connections += 1
         log.debug(
             "Starting new HTTP connection (%d): %s:%s",
@@ -485,22 +503,16 @@
         Close all pooled connections and disable the pool.
         """
         if self.pool is None:
             return
         # Disable access to the pool
         old_pool, self.pool = self.pool, None
 
-        try:
-            while True:
-                conn = old_pool.get(block=False)
-                if conn:
-                    conn.close()
-
-        except queue.Empty:
-            pass  # Done.
+        # Close all the HTTPConnections in the pool.
+        _close_pool_connections(old_pool)
 
     def is_same_host(self, url):
         """
         Check if the given ``url`` is a member of the same host as this
         connection pool.
         """
         if url.startswith("/"):
@@ -828,15 +840,19 @@
                 **response_kw
             )
 
         # Handle redirect?
         redirect_location = redirect and response.get_redirect_location()
         if redirect_location:
             if response.status == 303:
+                # Change the method according to RFC 9110, Section 15.4.4.
                 method = "GET"
+                # And lose the body not to transfer anything sensitive.
+                body = None
+                headers = HTTPHeaderDict(headers)._prepare_for_method_change()
 
             try:
                 retries = retries.increment(method, url, response=response, _pool=self)
             except MaxRetryError:
                 if retries.raise_on_redirect:
                     response.drain_conn()
                     raise
@@ -1104,7 +1120,18 @@
     # httplib crazily doubles up the square brackets on the Host header.
     # Instead, we need to make sure we never pass ``None`` as the port.
     # However, for backward compatibility reasons we can't actually
     # *assert* that.  See http://bugs.python.org/issue28539
     if host.startswith("[") and host.endswith("]"):
         host = host[1:-1]
     return host
+
+
+def _close_pool_connections(pool):
+    """Drains a queue of connections and closes each one."""
+    try:
+        while True:
+            conn = pool.get(block=False)
+            if conn:
+                conn.close()
+    except queue.Empty:
+        pass  # Done.
```

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/contrib/_appengine_environ.py` & `newrelic-9.9.0/newrelic/packages/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/contrib/_securetransport/bindings.py` & `newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/contrib/_securetransport/low_level.py` & `newrelic-9.9.0/newrelic/packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/contrib/appengine.py` & `newrelic-9.9.0/newrelic/packages/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/contrib/ntlmpool.py` & `newrelic-9.9.0/newrelic/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/contrib/pyopenssl.py` & `newrelic-9.9.0/newrelic/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/contrib/securetransport.py` & `newrelic-9.9.0/newrelic/packages/urllib3/contrib/securetransport.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,17 +60,16 @@
 import shutil
 import socket
 import ssl
 import struct
 import threading
 import weakref
 
-import six
-
 from .. import util
+from ..packages import six
 from ..util.ssl_ import PROTOCOL_TLS_CLIENT
 from ._securetransport.bindings import CoreFoundation, Security, SecurityConst
 from ._securetransport.low_level import (
     _assert_no_error,
     _build_tls_unknown_ca_alert,
     _cert_array_from_pem,
     _create_cfstring_array,
```

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/contrib/socks.py` & `newrelic-9.9.0/newrelic/packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/exceptions.py` & `newrelic-9.9.0/newrelic/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/fields.py` & `newrelic-9.9.0/newrelic/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/filepost.py` & `newrelic-9.9.0/newrelic/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/packages/backports/makefile.py` & `newrelic-9.9.0/newrelic/packages/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/packages/six.py` & `newrelic-9.9.0/newrelic/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/poolmanager.py` & `newrelic-9.9.0/newrelic/packages/urllib3/poolmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import absolute_import
 
 import collections
 import functools
 import logging
 
-from ._collections import RecentlyUsedContainer
+from ._collections import HTTPHeaderDict, RecentlyUsedContainer
 from .connectionpool import HTTPConnectionPool, HTTPSConnectionPool, port_by_scheme
 from .exceptions import (
     LocationValueError,
     MaxRetryError,
     ProxySchemeUnknown,
     ProxySchemeUnsupported,
     URLSchemeUnknown,
@@ -167,15 +167,15 @@
 
     proxy = None
     proxy_config = None
 
     def __init__(self, num_pools=10, headers=None, **connection_pool_kw):
         RequestMethods.__init__(self, headers)
         self.connection_pool_kw = connection_pool_kw
-        self.pools = RecentlyUsedContainer(num_pools, dispose_func=lambda p: p.close())
+        self.pools = RecentlyUsedContainer(num_pools)
 
         # Locally set the pool classes and keys so other PoolManagers can
         # override them.
         self.pool_classes_by_scheme = pool_classes_by_scheme
         self.key_fn_by_scheme = key_fn_by_scheme.copy()
 
     def __enter__(self):
@@ -378,17 +378,20 @@
         redirect_location = redirect and response.get_redirect_location()
         if not redirect_location:
             return response
 
         # Support relative URLs for redirecting.
         redirect_location = urljoin(url, redirect_location)
 
-        # RFC 7231, Section 6.4.4
         if response.status == 303:
+            # Change the method according to RFC 9110, Section 15.4.4.
             method = "GET"
+            # And lose the body not to transfer anything sensitive.
+            kw["body"] = None
+            kw["headers"] = HTTPHeaderDict(kw["headers"])._prepare_for_method_change()
 
         retries = kw.get("retries")
         if not isinstance(retries, Retry):
             retries = Retry.from_int(retries, redirect=redirect)
 
         # Strip headers marked as unsafe to forward to the redirected location.
         # Check remove_headers_on_redirect to avoid a potential network call within
```

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/request.py` & `newrelic-9.9.0/newrelic/packages/urllib3/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import absolute_import
 
+import sys
+
 from .filepost import encode_multipart_formdata
+from .packages import six
 from .packages.six.moves.urllib.parse import urlencode
 
 __all__ = ["RequestMethods"]
 
 
 class RequestMethods(object):
     """
@@ -164,7 +167,25 @@
             extra_kw["body"] = body
             extra_kw["headers"] = {"Content-Type": content_type}
 
         extra_kw["headers"].update(headers)
         extra_kw.update(urlopen_kw)
 
         return self.urlopen(method, url, **extra_kw)
+
+
+if not six.PY2:
+
+    class RequestModule(sys.modules[__name__].__class__):
+        def __call__(self, *args, **kwargs):
+            """
+            If user tries to call this module directly urllib3 v2.x style raise an error to the user
+            suggesting they may need urllib3 v2
+            """
+            raise TypeError(
+                "'module' object is not callable\n"
+                "urllib3.request() method is not supported in this release, "
+                "upgrade to urllib3 v2 to use it\n"
+                "see https://urllib3.readthedocs.io/en/stable/v2-migration-guide.html"
+            )
+
+    sys.modules[__name__].__class__ = RequestModule
```

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/response.py` & `newrelic-9.9.0/newrelic/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/__init__.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/connection.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/proxy.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/request.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/response.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/retry.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/retry.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         ["HEAD", "GET", "PUT", "DELETE", "OPTIONS", "TRACE"]
     )
 
     #: Default status codes to be used for ``status_forcelist``
     RETRY_AFTER_STATUS_CODES = frozenset([413, 429, 503])
 
     #: Default headers to be used for ``remove_headers_on_redirect``
-    DEFAULT_REMOVE_HEADERS_ON_REDIRECT = frozenset(["Authorization"])
+    DEFAULT_REMOVE_HEADERS_ON_REDIRECT = frozenset(["Cookie", "Authorization"])
 
     #: Maximum backoff time.
     DEFAULT_BACKOFF_MAX = 120
 
     def __init__(
         self,
         total=10,
```

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/ssl_.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/ssl_match_hostname.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/ssltransport.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/timeout.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/url.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/urllib3/util/wait.py` & `newrelic-9.9.0/newrelic/packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/wrapt/LICENSE` & `newrelic-9.9.0/newrelic/packages/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/wrapt/__init__.py` & `newrelic-9.9.0/newrelic/packages/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/wrapt/_wrappers.c` & `newrelic-9.9.0/newrelic/packages/wrapt/_wrappers.c`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/wrapt/arguments.py` & `newrelic-9.9.0/newrelic/packages/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/wrapt/decorators.py` & `newrelic-9.9.0/newrelic/packages/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/wrapt/importer.py` & `newrelic-9.9.0/newrelic/packages/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/wrapt/patches.py` & `newrelic-9.9.0/newrelic/packages/wrapt/patches.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/wrapt/weakrefs.py` & `newrelic-9.9.0/newrelic/packages/wrapt/weakrefs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/packages/wrapt/wrappers.py` & `newrelic-9.9.0/newrelic/packages/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/samplers/__init__.py` & `newrelic-9.9.0/newrelic/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/samplers/cpu_usage.py` & `newrelic-9.9.0/newrelic/samplers/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/samplers/data_sampler.py` & `newrelic-9.9.0/newrelic/samplers/data_sampler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/samplers/decorators.py` & `newrelic-9.9.0/newrelic/samplers/decorators.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/samplers/gc_data.py` & `newrelic-9.9.0/newrelic/samplers/gc_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/newrelic/samplers/memory_usage.py` & `newrelic-9.9.0/newrelic/samplers/memory_usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 
 """This module implements a data source for generating metrics about
 memory usage.
 
 """
 import os
 
+from newrelic.core.config import global_settings
 from newrelic.common.system_info import physical_memory_used, total_physical_memory
 from newrelic.samplers.decorators import data_source_generator
 
 
 @data_source_generator(name="Memory Usage")
 def memory_usage_data_source():
+    settings = global_settings()
+
     memory = physical_memory_used()
     total_memory = total_physical_memory()
     pid = os.getpid()
 
     # Calculate memory utilization without 0 division errors
     memory_utilization = (memory / total_memory) if total_memory != 0 else 0
 
     yield ("Memory/Physical", memory)
-    yield ("Memory/Physical/%d" % (pid), memory)
-
     yield ("Memory/Physical/Utilization", memory_utilization)
-    yield ("Memory/Physical/Utilization/%d" % (pid), memory_utilization)
+
+    if settings.memory_runtime_pid_metrics.enabled:
+        yield ("Memory/Physical/%d" % (pid), memory)
+        yield ("Memory/Physical/Utilization/%d" % (pid), memory_utilization)
```

### Comparing `newrelic-9.8.0/newrelic.egg-info/PKG-INFO` & `newrelic-9.9.0/newrelic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic
-Version: 9.8.0
+Version: 9.9.0
 Summary: New Relic Python Agent
 Home-page: https://docs.newrelic.com/docs/apm/agents/python-agent/
 Author: New Relic
 Author-email: support@newrelic.com
 Maintainer: New Relic
 Maintainer-email: support@newrelic.com
 License: Apache-2.0
```

### Comparing `newrelic-9.8.0/newrelic.egg-info/SOURCES.txt` & `newrelic-9.9.0/newrelic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -317,14 +317,15 @@
 newrelic/packages/urllib3/contrib/_securetransport/__init__.py
 newrelic/packages/urllib3/contrib/_securetransport/bindings.py
 newrelic/packages/urllib3/contrib/_securetransport/low_level.py
 newrelic/packages/urllib3/packages/__init__.py
 newrelic/packages/urllib3/packages/six.py
 newrelic/packages/urllib3/packages/backports/__init__.py
 newrelic/packages/urllib3/packages/backports/makefile.py
+newrelic/packages/urllib3/packages/backports/weakref_finalize.py
 newrelic/packages/urllib3/util/__init__.py
 newrelic/packages/urllib3/util/connection.py
 newrelic/packages/urllib3/util/proxy.py
 newrelic/packages/urllib3/util/queue.py
 newrelic/packages/urllib3/util/request.py
 newrelic/packages/urllib3/util/response.py
 newrelic/packages/urllib3/util/retry.py
@@ -464,18 +465,20 @@
 tests/agent_unittests/test_region_aware_settings.py
 tests/agent_unittests/test_sampler_metrics.py
 tests/agent_unittests/test_serverless_mode_settings.py
 tests/agent_unittests/test_signature.py
 tests/agent_unittests/test_trace_cache.py
 tests/agent_unittests/test_utilization_settings.py
 tests/agent_unittests/test_wrappers.py
+tests/application_celery/_target_application.py
 tests/application_celery/conftest.py
-tests/application_celery/tasks.py
-tests/application_celery/test_celery.py
-tests/application_celery/test_celery_max_tasks_per_child.py
+tests/application_celery/test_application.py
+tests/application_celery/test_distributed_tracing.py
+tests/application_celery/test_max_tasks_per_child.py
+tests/application_celery/test_task_methods.py
 tests/application_gearman/conftest.py
 tests/application_gearman/test_gearman.py
 tests/component_djangorestframework/conftest.py
 tests/component_djangorestframework/settings.py
 tests/component_djangorestframework/test_application.py
 tests/component_djangorestframework/urls.py
 tests/component_djangorestframework/views.py
@@ -1169,14 +1172,15 @@
 tests/testing_support/validators/validate_apdex_metrics.py
 tests/testing_support/validators/validate_application_error_event_count.py
 tests/testing_support/validators/validate_application_error_trace_count.py
 tests/testing_support/validators/validate_application_errors.py
 tests/testing_support/validators/validate_browser_attributes.py
 tests/testing_support/validators/validate_code_level_metrics.py
 tests/testing_support/validators/validate_cross_process_headers.py
+tests/testing_support/validators/validate_custom_event.py
 tests/testing_support/validators/validate_custom_event_collector_json.py
 tests/testing_support/validators/validate_custom_events.py
 tests/testing_support/validators/validate_custom_metrics_outside_transaction.py
 tests/testing_support/validators/validate_custom_parameters.py
 tests/testing_support/validators/validate_database_duration.py
 tests/testing_support/validators/validate_database_node.py
 tests/testing_support/validators/validate_database_trace_inputs.py
```

### Comparing `newrelic-9.8.0/setup.py` & `newrelic-9.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_asgiref/conftest.py` & `newrelic-9.9.0/tests/adapter_asgiref/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_asgiref/test_context_propagation.py` & `newrelic-9.9.0/tests/adapter_asgiref/test_context_propagation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_cheroot/conftest.py` & `newrelic-9.9.0/tests/adapter_cheroot/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_cheroot/test_wsgi.py` & `newrelic-9.9.0/tests/adapter_cheroot/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_daphne/conftest.py` & `newrelic-9.9.0/tests/adapter_daphne/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_daphne/test_daphne.py` & `newrelic-9.9.0/tests/adapter_daphne/test_daphne.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gevent/_application.py` & `newrelic-9.9.0/tests/adapter_gevent/_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gevent/conftest.py` & `newrelic-9.9.0/tests/adapter_gevent/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gevent/test_patching.py` & `newrelic-9.9.0/tests/adapter_gevent/test_patching.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gevent/test_pywsgi.py` & `newrelic-9.9.0/tests/adapter_gevent/test_pywsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gunicorn/app.py` & `newrelic-9.9.0/tests/adapter_gunicorn/app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gunicorn/asgi_app.py` & `newrelic-9.9.0/tests/adapter_gunicorn/asgi_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gunicorn/async_app.py` & `newrelic-9.9.0/tests/adapter_gunicorn/async_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gunicorn/conftest.py` & `newrelic-9.9.0/tests/adapter_gunicorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gunicorn/test_aiohttp_app_factory.py` & `newrelic-9.9.0/tests/adapter_gunicorn/test_aiohttp_app_factory.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gunicorn/test_asgi_app.py` & `newrelic-9.9.0/tests/adapter_gunicorn/test_asgi_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gunicorn/test_gaiohttp.py` & `newrelic-9.9.0/tests/adapter_gunicorn/test_gaiohttp.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_gunicorn/worker.py` & `newrelic-9.9.0/tests/adapter_gunicorn/worker.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_hypercorn/conftest.py` & `newrelic-9.9.0/tests/adapter_hypercorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_hypercorn/test_hypercorn.py` & `newrelic-9.9.0/tests/adapter_hypercorn/test_hypercorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_uvicorn/conftest.py` & `newrelic-9.9.0/tests/adapter_uvicorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_uvicorn/test_uvicorn.py` & `newrelic-9.9.0/tests/adapter_uvicorn/test_uvicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_waitress/_application.py` & `newrelic-9.9.0/tests/adapter_waitress/_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_waitress/conftest.py` & `newrelic-9.9.0/tests/adapter_waitress/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/adapter_waitress/test_wsgi.py` & `newrelic-9.9.0/tests/adapter_waitress/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/_test_async_coroutine_trace.py` & `newrelic-9.9.0/tests/agent_features/_test_async_coroutine_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/_test_async_coroutine_transaction.py` & `newrelic-9.9.0/tests/agent_features/_test_async_coroutine_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/_test_async_generator_trace.py` & `newrelic-9.9.0/tests/agent_features/_test_async_generator_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/_test_code_level_metrics.py` & `newrelic-9.9.0/tests/agent_features/_test_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/conftest.py` & `newrelic-9.9.0/tests/agent_features/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_apdex_metrics.py` & `newrelic-9.9.0/tests/agent_features/test_apdex_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_asgi_browser.py` & `newrelic-9.9.0/tests/agent_features/test_asgi_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 
 import pytest
-import six
 from bs4 import BeautifulSoup
 from testing_support.asgi_testing import AsgiTest
 from testing_support.fixtures import override_application_settings
 from testing_support.validators.validate_custom_parameters import (
     validate_custom_parameters,
 )
 from testing_support.validators.validate_transaction_errors import (
@@ -30,14 +29,15 @@
 from newrelic.api.asgi_application import asgi_application
 from newrelic.api.transaction import (
     add_custom_attribute,
     disable_browser_autorum,
     get_browser_timing_header,
 )
 from newrelic.common.encoding_utils import deobfuscate
+from newrelic.packages import six
 
 _runtime_error_name = RuntimeError.__module__ + ":" + RuntimeError.__name__
 
 
 @asgi_application()
 async def target_asgi_application_manual_rum(scope, receive, send):
     text = "<html><head>%s</head><body><p>RESPONSE</p></body></html>"
```

### Comparing `newrelic-9.8.0/tests/agent_features/test_asgi_distributed_tracing.py` & `newrelic-9.9.0/tests/agent_features/test_asgi_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_asgi_transaction.py` & `newrelic-9.9.0/tests/agent_features/test_asgi_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_asgi_w3c_trace_context.py` & `newrelic-9.9.0/tests/agent_features/test_asgi_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_async_context_propagation.py` & `newrelic-9.9.0/tests/agent_features/test_async_context_propagation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_async_generator_trace.py` & `newrelic-9.9.0/tests/agent_features/test_async_generator_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_async_timing.py` & `newrelic-9.9.0/tests/agent_features/test_async_timing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_async_wrapper_detection.py` & `newrelic-9.9.0/tests/agent_features/test_async_wrapper_detection.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_attribute.py` & `newrelic-9.9.0/tests/agent_features/test_attribute.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_attributes_in_action.py` & `newrelic-9.9.0/tests/agent_features/test_attributes_in_action.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_background_task.py` & `newrelic-9.9.0/tests/agent_features/test_background_task.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_browser.py` & `newrelic-9.9.0/tests/agent_features/test_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import re
 import sys
 
-import six
 import webtest
 from testing_support.fixtures import override_application_settings
 from testing_support.validators.validate_custom_parameters import (
     validate_custom_parameters,
 )
 from testing_support.validators.validate_transaction_errors import (
     validate_transaction_errors,
@@ -31,14 +30,15 @@
     add_custom_attribute,
     disable_browser_autorum,
     get_browser_timing_header,
 )
 from newrelic.api.web_transaction import web_transaction
 from newrelic.api.wsgi_application import wsgi_application
 from newrelic.common.encoding_utils import deobfuscate
+from newrelic.packages import six
 
 _runtime_error_name = RuntimeError.__module__ + ":" + RuntimeError.__name__
 
 
 @wsgi_application()
 def target_wsgi_application_manual_rum(environ, start_response):
     status = "200 OK"
```

### Comparing `newrelic-9.8.0/tests/agent_features/test_browser_middleware.py` & `newrelic-9.9.0/tests/agent_features/test_browser_middleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,124 +9,148 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-import six
 import webtest
+from testing_support.fixtures import (
+    capture_transaction_metrics,
+    override_application_settings,
+)
 
 from newrelic.api.wsgi_application import wsgi_application
+from newrelic.packages import six
 
-from testing_support.fixtures import (override_application_settings,
-    capture_transaction_metrics)
-
-PAGE_CONTENTS = b'Hello World'
+PAGE_CONTENTS = b"Hello World"
 
 _browser_enabled_settings = {
-    'browser_monitoring.enabled': True,
+    "browser_monitoring.enabled": True,
 }
 
 _browser_disabled_settings = {
-    'browser_monitoring.enabled': False,
+    "browser_monitoring.enabled": False,
 }
 
+
 @wsgi_application()
 def _app_list(environ, start_response):
-    status = '200 OK'
-    response_headers = [('Content-type', 'text/plain')]
+    status = "200 OK"
+    response_headers = [("Content-type", "text/plain")]
     start_response(status, response_headers)
     return [PAGE_CONTENTS]
+
+
 target_application_list = webtest.TestApp(_app_list)
 
+
 @wsgi_application()
 def _app_iter(environ, start_response):
-    status = '200 OK'
-    response_headers = [('Content-type', 'text/plain')]
+    status = "200 OK"
+    response_headers = [("Content-type", "text/plain")]
     start_response(status, response_headers)
     yield PAGE_CONTENTS
+
+
 target_application_iter = webtest.TestApp(_app_iter)
 
+
 @wsgi_application()
 def _app_str(environ, start_response):
-    status = '200 OK'
-    response_headers = [('Content-type', 'text/plain')]
+    status = "200 OK"
+    response_headers = [("Content-type", "text/plain")]
     start_response(status, response_headers)
     return PAGE_CONTENTS
+
+
 target_application_str = webtest.TestApp(_app_str)
 
+
 @wsgi_application()
 def _app_list_exc_1(environ, start_response):
-    status = '200 OK'
-    response_headers = [('Content-type', 'text/plain')]
+    status = "200 OK"
+    response_headers = [("Content-type", "text/plain")]
     start_response(status, response_headers)
-    1/0
+    1 / 0
     return [PAGE_CONTENTS]
+
+
 target_application_list_exc_1 = webtest.TestApp(_app_list_exc_1)
 
+
 @wsgi_application()
 def _app_list_exc_2(environ, start_response):
-    status = '200 OK'
-    response_headers = [('Content-type', 'text/plain')]
-    1/0
+    status = "200 OK"
+    response_headers = [("Content-type", "text/plain")]
+    1 / 0
     start_response(status, response_headers)
     return [PAGE_CONTENTS]
+
+
 target_application_list_exc_2 = webtest.TestApp(_app_list_exc_2)
 
+
 @wsgi_application()
 def _app_iter_exc_1(environ, start_response):
-    status = '200 OK'
-    response_headers = [('Content-type', 'text/plain')]
+    status = "200 OK"
+    response_headers = [("Content-type", "text/plain")]
     start_response(status, response_headers)
-    1/0
+    1 / 0
     yield PAGE_CONTENTS
+
+
 target_application_iter_exc_1 = webtest.TestApp(_app_iter_exc_1)
 
+
 @wsgi_application()
 def _app_iter_exc_2(environ, start_response):
-    status = '200 OK'
-    response_headers = [('Content-type', 'text/plain')]
-    1/0
+    status = "200 OK"
+    response_headers = [("Content-type", "text/plain")]
+    1 / 0
     start_response(status, response_headers)
     yield PAGE_CONTENTS
+
+
 target_application_iter_exc_2 = webtest.TestApp(_app_iter_exc_2)
 
 _target_applications = [
     target_application_list,
     target_application_iter,
-    pytest.param(target_application_str, marks=pytest.mark.skipif(
-                six.PY3, reason='PY3 webtest expects type(byte) '
-                'so this test doesnt apply')),
+    pytest.param(
+        target_application_str,
+        marks=pytest.mark.skipif(six.PY3, reason="PY3 webtest expects type(byte) " "so this test doesnt apply"),
+    ),
     target_application_list_exc_1,
     target_application_list_exc_2,
     target_application_iter_exc_1,
     target_application_iter_exc_2,
 ]
 
-@pytest.mark.parametrize('target_application', _target_applications)
+
+@pytest.mark.parametrize("target_application", _target_applications)
 def test_metrics_same_with_and_without_browser_middleware(target_application):
     with_browser_metrics = []
     without_browser_metrics = []
 
     @capture_transaction_metrics(with_browser_metrics)
     @override_application_settings(_browser_enabled_settings)
     def run_app_with_browser():
         try:
-            resp = target_application.get('/')
+            resp = target_application.get("/")
         except ZeroDivisionError:
             pass
         else:
             assert resp.body == PAGE_CONTENTS
 
     @capture_transaction_metrics(without_browser_metrics)
     @override_application_settings(_browser_disabled_settings)
     def run_app_without_browser():
         try:
-            resp = target_application.get('/')
+            resp = target_application.get("/")
         except ZeroDivisionError:
             pass
         else:
             assert resp.body == PAGE_CONTENTS
 
     run_app_with_browser()
     run_app_without_browser()
```

### Comparing `newrelic-9.8.0/tests/agent_features/test_cat.py` & `newrelic-9.9.0/tests/agent_features/test_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_code_level_metrics.py` & `newrelic-9.9.0/tests/agent_features/test_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_collector_payloads.py` & `newrelic-9.9.0/tests/agent_features/test_collector_payloads.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_configuration.py` & `newrelic-9.9.0/tests/agent_features/test_configuration.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_coroutine_trace.py` & `newrelic-9.9.0/tests/agent_features/test_coroutine_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_coroutine_transaction.py` & `newrelic-9.9.0/tests/agent_features/test_coroutine_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_custom_events.py` & `newrelic-9.9.0/tests/agent_features/test_custom_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import time
 
 import pytest
 from testing_support.fixtures import (
     function_not_called,
     override_application_settings,
     reset_core_stats_engine,
+)
+from testing_support.validators.validate_custom_event import (
     validate_custom_event_count,
     validate_custom_event_in_application_stats_engine,
 )
 from testing_support.validators.validate_custom_events import validate_custom_events
 
 from newrelic.api.application import application_instance as application
 from newrelic.api.background_task import background_task
```

### Comparing `newrelic-9.8.0/tests/agent_features/test_custom_metrics.py` & `newrelic-9.9.0/tests/agent_features/test_custom_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_datastore_trace.py` & `newrelic-9.9.0/tests/agent_features/test_datastore_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_dead_transactions.py` & `newrelic-9.9.0/tests/agent_features/test_dead_transactions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_dimensional_metrics.py` & `newrelic-9.9.0/tests/agent_features/test_dimensional_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_distributed_tracing.py` & `newrelic-9.9.0/tests/agent_features/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_error_events.py` & `newrelic-9.9.0/tests/agent_features/test_error_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_error_group_callback.py` & `newrelic-9.9.0/tests/agent_features/test_error_group_callback.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_event_loop_wait_time.py` & `newrelic-9.9.0/tests/agent_features/test_event_loop_wait_time.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_exception_messages.py` & `newrelic-9.9.0/tests/agent_features/test_exception_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-import six
 from testing_support.fixtures import (
     reset_core_stats_engine,
     set_default_encoding,
     validate_application_exception_message,
     validate_transaction_exception_message,
 )
 
 from newrelic.api.application import application_instance as application
 from newrelic.api.background_task import background_task
 from newrelic.api.time_trace import notice_error
+from newrelic.packages import six
 
 # Turn off black formatting for this section of the code.
 # While Python 2 has been EOL'd since 2020, New Relic still
 # supports it and therefore these messages need to keep this
 # specific formatting.
 # fmt: off
 UNICODE_MESSAGE = u'I💜🐍'
```

### Comparing `newrelic-9.8.0/tests/agent_features/test_function_trace.py` & `newrelic-9.9.0/tests/agent_features/test_function_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_high_security_mode.py` & `newrelic-9.9.0/tests/agent_features/test_high_security_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,19 @@
 import pytest
 import webtest
 from testing_support.fixtures import (
     override_application_settings,
     override_generic_settings,
     reset_core_stats_engine,
     validate_attributes_complete,
+    validate_request_params_omitted,
+)
+from testing_support.validators.validate_custom_event import (
     validate_custom_event_count,
     validate_custom_event_in_application_stats_engine,
-    validate_request_params_omitted,
 )
 from testing_support.validators.validate_custom_parameters import (
     validate_custom_parameters,
 )
 from testing_support.validators.validate_non_transaction_error_event import (
     validate_non_transaction_error_event,
 )
```

### Comparing `newrelic-9.8.0/tests/agent_features/test_ignore_expected_errors.py` & `newrelic-9.9.0/tests/agent_features/test_ignore_expected_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_lambda_handler.py` & `newrelic-9.9.0/tests/agent_features/test_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_llm_token_count_callback.py` & `newrelic-9.9.0/tests/agent_features/test_llm_token_count_callback.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_log_events.py` & `newrelic-9.9.0/tests/agent_features/test_log_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_logs_in_context.py` & `newrelic-9.9.0/tests/agent_features/test_logs_in_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_metric_normalization.py` & `newrelic-9.9.0/tests/agent_features/test_metric_normalization.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_ml_events.py` & `newrelic-9.9.0/tests/agent_features/test_ml_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_notice_error.py` & `newrelic-9.9.0/tests/agent_features/test_notice_error.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_priority_sampling.py` & `newrelic-9.9.0/tests/agent_features/test_priority_sampling.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_profile_trace.py` & `newrelic-9.9.0/tests/agent_features/test_profile_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_record_llm_feedback_event.py` & `newrelic-9.9.0/tests/agent_features/test_record_llm_feedback_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from testing_support.fixtures import (
-    reset_core_stats_engine,
-    validate_custom_event_count,
-)
+from testing_support.fixtures import reset_core_stats_engine
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 
 from newrelic.api.background_task import background_task
 from newrelic.api.ml_model import record_llm_feedback_event
 
 
 @reset_core_stats_engine()
```

### Comparing `newrelic-9.8.0/tests/agent_features/test_serverless_mode.py` & `newrelic-9.9.0/tests/agent_features/test_serverless_mode.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_span_events.py` & `newrelic-9.9.0/tests/agent_features/test_span_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_stack_trace.py` & `newrelic-9.9.0/tests/agent_features/test_stack_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_supportability_metrics.py` & `newrelic-9.9.0/tests/agent_features/test_supportability_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_synthetics.py` & `newrelic-9.9.0/tests/agent_features/test_synthetics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_time_trace.py` & `newrelic-9.9.0/tests/agent_features/test_time_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py` & `newrelic-9.9.0/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_transaction_name.py` & `newrelic-9.9.0/tests/agent_features/test_transaction_name.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_transaction_trace_segments.py` & `newrelic-9.9.0/tests/agent_features/test_transaction_trace_segments.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_w3c_trace_context.py` & `newrelic-9.9.0/tests/agent_features/test_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_web_transaction.py` & `newrelic-9.9.0/tests/agent_features/test_web_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_features/test_wsgi_attributes.py` & `newrelic-9.9.0/tests/agent_features/test_wsgi_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_streaming/_test_handler.py` & `newrelic-9.9.0/tests/agent_streaming/_test_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_streaming/conftest.py` & `newrelic-9.9.0/tests/agent_streaming/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_streaming/test_infinite_tracing.py` & `newrelic-9.9.0/tests/agent_streaming/test_infinite_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_streaming/test_span_events.py` & `newrelic-9.9.0/tests/agent_streaming/test_span_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_streaming/test_stream_buffer.py` & `newrelic-9.9.0/tests/agent_streaming/test_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_streaming/test_streaming_rpc.py` & `newrelic-9.9.0/tests/agent_streaming/test_streaming_rpc.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/_test_import_hook.py` & `newrelic-9.9.0/tests/agent_unittests/_test_import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/cert.pem` & `newrelic-9.9.0/tests/agent_unittests/cert.pem`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/conftest.py` & `newrelic-9.9.0/tests/agent_unittests/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_agent.py` & `newrelic-9.9.0/tests/agent_unittests/test_agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_agent_connect.py` & `newrelic-9.9.0/tests/agent_unittests/test_agent_connect.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_agent_protocol.py` & `newrelic-9.9.0/tests/agent_unittests/test_agent_protocol.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_check_environment.py` & `newrelic-9.9.0/tests/agent_unittests/test_check_environment.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_connect_response_fields.py` & `newrelic-9.9.0/tests/agent_unittests/test_connect_response_fields.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_distributed_tracing_settings.py` & `newrelic-9.9.0/tests/agent_unittests/test_distributed_tracing_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_encoding_utils.py` & `newrelic-9.9.0/tests/agent_unittests/test_encoding_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_environment.py` & `newrelic-9.9.0/tests/agent_unittests/test_environment.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_full_uri_payloads.py` & `newrelic-9.9.0/tests/agent_unittests/test_full_uri_payloads.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_harvest_loop.py` & `newrelic-9.9.0/tests/agent_unittests/test_harvest_loop.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_http_client.py` & `newrelic-9.9.0/tests/agent_unittests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_import_hook.py` & `newrelic-9.9.0/tests/agent_unittests/test_import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_infinite_trace_settings.py` & `newrelic-9.9.0/tests/agent_unittests/test_infinite_trace_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_package_version_utils.py` & `newrelic-9.9.0/tests/agent_unittests/test_package_version_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_region_aware_settings.py` & `newrelic-9.9.0/tests/agent_unittests/test_region_aware_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_sampler_metrics.py` & `newrelic-9.9.0/tests/agent_unittests/test_sampler_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -148,18 +148,26 @@
 
     for metric in EXPECTED_CPU_METRICS:
         assert metric in metrics_table
 
 
 EXPECTED_MEMORY_METRICS = (
     "Memory/Physical",
-    "Memory/Physical/%d" % PID,
     "Memory/Physical/Utilization",
+    "Memory/Physical/%d" % PID,
     "Memory/Physical/Utilization/%d" % PID,
 )
 
 
-def test_memory_metrics_collection(memory_data_source):
-    metrics_table = set(m[0] for m in (memory_data_source() or ()))
+@pytest.mark.parametrize("enabled", (True, False))
+def test_memory_metrics_collection(memory_data_source, enabled):
+    @override_generic_settings(settings, {"memory_runtime_pid_metrics.enabled": enabled})
+    def _test():
+        metrics_table = set(m[0] for m in (memory_data_source() or ()))
+        if enabled:
+            for metric in EXPECTED_MEMORY_METRICS:
+                assert metric in metrics_table
+        else:
+            assert EXPECTED_MEMORY_METRICS[0] in metrics_table
+            assert EXPECTED_MEMORY_METRICS[1] in metrics_table
 
-    for metric in EXPECTED_MEMORY_METRICS:
-        assert metric in metrics_table
+    _test()
```

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_serverless_mode_settings.py` & `newrelic-9.9.0/tests/agent_unittests/test_serverless_mode_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_signature.py` & `newrelic-9.9.0/tests/agent_unittests/test_signature.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_trace_cache.py` & `newrelic-9.9.0/tests/agent_unittests/test_trace_cache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_utilization_settings.py` & `newrelic-9.9.0/tests/agent_unittests/test_utilization_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/agent_unittests/test_wrappers.py` & `newrelic-9.9.0/tests/agent_unittests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/application_celery/conftest.py` & `newrelic-9.9.0/tests/component_tastypie/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 
 _default_settings = {
     'transaction_tracer.explain_threshold': 0.0,
     'transaction_tracer.transaction_threshold': 0.0,
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
     'debug.record_transaction_failure': True,
+    'debug.log_autorum_middleware': True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (application_celery)',
+        app_name='Python Agent Test (component_tastypie)',
         default_settings=_default_settings)
```

### Comparing `newrelic-9.8.0/tests/application_celery/tasks.py` & `newrelic-9.9.0/tests/framework_flask/_test_application_async.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from celery import Celery
+import webtest
+from _test_application import application
 
+from conftest import async_handler_support
 
-app = Celery('tasks')
+# Async handlers only supported in Flask >2.0.0
+if async_handler_support:
+    @application.route('/async')
+    async def async_page():
+        return 'ASYNC RESPONSE'
 
-@app.task
-def add(x, y):
-    return x + y
-
-@app.task
-def tsum(nums):
-    return sum(nums)
+_test_application = webtest.TestApp(application)
```

### Comparing `newrelic-9.8.0/tests/application_celery/test_celery.py` & `newrelic-9.9.0/tests/application_celery/test_application.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,61 +8,65 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from newrelic.api.background_task import background_task
-from newrelic.api.transaction import ignore_transaction, end_of_transaction
-
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
-from testing_support.validators.validate_code_level_metrics import validate_code_level_metrics
+from _target_application import add, nested_add, shared_task_add, tsum
+from testing_support.validators.validate_code_level_metrics import (
+    validate_code_level_metrics,
+)
+from testing_support.validators.validate_transaction_count import (
+    validate_transaction_count,
+)
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
 
-from tasks import add, tsum
+from newrelic.api.background_task import background_task
+from newrelic.api.transaction import end_of_transaction, ignore_transaction
 
 
 @validate_transaction_metrics(
-        name='test_celery:test_celery_task_as_function_trace',
-        scoped_metrics=[('Function/tasks.add', 1)],
-        background_task=True)
-@validate_code_level_metrics("tasks", "add")
+    name="test_application:test_celery_task_as_function_trace",
+    scoped_metrics=[("Function/_target_application.add", 1)],
+    background_task=True,
+)
+@validate_code_level_metrics("_target_application", "add")
 @background_task()
 def test_celery_task_as_function_trace():
     """
     Calling add() inside a transaction means the agent will record
     add() as a FunctionTrace.
 
     """
     result = add(3, 4)
     assert result == 7
 
 
-@validate_transaction_metrics(
-        name='tasks.add',
-        group='Celery',
-        scoped_metrics=[],
-        background_task=True)
-@validate_code_level_metrics("tasks", "add")
+@validate_transaction_metrics(name="_target_application.add", group="Celery", scoped_metrics=[], background_task=True)
+@validate_code_level_metrics("_target_application", "add")
 def test_celery_task_as_background_task():
     """
     Calling add() outside of a transaction means the agent will create
     a background transaction (with a group of 'Celery') and record add()
     as a background task.
 
     """
     result = add(3, 4)
     assert result == 7
 
+
 @validate_transaction_metrics(
-        name='test_celery:test_celery_tasks_multiple_function_traces',
-        scoped_metrics=[('Function/tasks.add', 1),
-                        ('Function/tasks.tsum', 1)],
-        background_task=True)
-@validate_code_level_metrics("tasks", "tsum")
+    name="test_application:test_celery_tasks_multiple_function_traces",
+    scoped_metrics=[("Function/_target_application.add", 1), ("Function/_target_application.tsum", 1)],
+    background_task=True,
+)
+@validate_code_level_metrics("_target_application", "tsum")
 @background_task()
 def test_celery_tasks_multiple_function_traces():
     add_result = add(5, 6)
     assert add_result == 11
 
     tsum_result = tsum([1, 2, 3, 4])
     assert tsum_result == 10
@@ -70,36 +74,70 @@
 
 @background_task()
 def test_celery_tasks_ignore_transaction():
     """
     No transaction is recorded, due to the call to ignore_transaction(),
     so no validation fixture is used. The purpose of this test is to make
     sure the agent doesn't throw an error.
-
     """
+
     add_result = add(1, 2)
     assert add_result == 3
 
     ignore_transaction()
 
     tsum_result = tsum([1, 2, 3])
     assert tsum_result == 6
 
 
 @validate_transaction_metrics(
-        name='test_celery:test_celery_tasks_end_transaction',
-        scoped_metrics=[('Function/tasks.add', 1)],
-        background_task=True)
+    name="test_application:test_celery_tasks_end_transaction",
+    scoped_metrics=[("Function/_target_application.add", 1)],
+    background_task=True,
+)
 @background_task()
 def test_celery_tasks_end_transaction():
     """
     Only functions that run before the call to end_of_transaction() are
     included in the transaction.
-
     """
+
     add_result = add(1, 2)
     assert add_result == 3
 
     end_of_transaction()
 
     tsum_result = tsum([1, 2, 3])
     assert tsum_result == 6
+
+
+@validate_transaction_metrics(
+    name="_target_application.nested_add",
+    group="Celery",
+    scoped_metrics=[("Function/_target_application.add", 1)],
+    background_task=True,
+)
+@validate_transaction_count(1)
+@validate_code_level_metrics("_target_application", "nested_add")
+def test_celery_nested_tasks():
+    """
+    Celery tasks run inside other celery tasks should not start a new transactions,
+    and should create a function trace instead.
+    """
+
+    add_result = nested_add(1, 2)
+    assert add_result == 3
+
+
+@validate_transaction_metrics(
+    name="_target_application.shared_task_add", group="Celery", scoped_metrics=[], background_task=True
+)
+@validate_code_level_metrics("_target_application", "shared_task_add")
+def test_celery_shared_task_as_background_task():
+    """
+    Calling shared_task_add() outside of a transaction means the agent will create
+    a background transaction (with a group of 'Celery') and record shared_task_add()
+    as a background task.
+
+    """
+    result = shared_task_add(3, 4)
+    assert result == 7
```

### Comparing `newrelic-9.8.0/tests/application_celery/test_celery_max_tasks_per_child.py` & `newrelic-9.9.0/tests/application_celery/test_max_tasks_per_child.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,31 +9,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-
 from billiard import get_context
 from billiard.pool import Worker
+from testing_support.validators.validate_function_called import validate_function_called
 
-from testing_support.validators.validate_function_called import (
-        validate_function_called)
+from newrelic.common.object_wrapper import transient_function_wrapper
 
 
 class OnExit(Exception):
     pass
 
 
-@validate_function_called('newrelic.core.agent', 'Agent.shutdown_agent')
-def test_max_tasks_per_child():
+@transient_function_wrapper("newrelic.core.agent", "Agent.shutdown_agent")
+def mock_agent_shutdown(wrapped, instance, args, kwargs):
+    # Prevent agent from actually shutting down and blocking further tests
+    pass
 
+
+@mock_agent_shutdown
+@validate_function_called("newrelic.core.agent", "Agent.shutdown_agent")
+def test_max_tasks_per_child():
     def on_exit(*args, **kwargs):
         raise OnExit()
 
     ctx = get_context()
-    worker = Worker(ctx.SimpleQueue(), ctx.SimpleQueue(), None,
-            maxtasks=1, on_exit=on_exit)
+    worker = Worker(ctx.SimpleQueue(), ctx.SimpleQueue(), None, maxtasks=1, on_exit=on_exit)
 
     with pytest.raises(OnExit):
         worker._do_exit(None, 0)
```

### Comparing `newrelic-9.8.0/tests/application_gearman/conftest.py` & `newrelic-9.9.0/tests/application_gearman/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/application_gearman/test_gearman.py` & `newrelic-9.9.0/tests/application_gearman/test_gearman.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_djangorestframework/conftest.py` & `newrelic-9.9.0/tests/component_djangorestframework/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_djangorestframework/settings.py` & `newrelic-9.9.0/tests/component_djangorestframework/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_djangorestframework/test_application.py` & `newrelic-9.9.0/tests/component_djangorestframework/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_djangorestframework/urls.py` & `newrelic-9.9.0/tests/component_djangorestframework/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_djangorestframework/views.py` & `newrelic-9.9.0/tests/component_djangorestframework/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_djangorestframework/wsgi.py` & `newrelic-9.9.0/tests/component_djangorestframework/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_flask_rest/_test_application.py` & `newrelic-9.9.0/tests/component_flask_rest/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_flask_rest/conftest.py` & `newrelic-9.9.0/tests/component_flask_rest/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_flask_rest/test_application.py` & `newrelic-9.9.0/tests/component_flask_rest/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_graphqlserver/__init__.py` & `newrelic-9.9.0/tests/component_graphqlserver/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_graphqlserver/_target_schema_async.py` & `newrelic-9.9.0/tests/component_graphqlserver/_target_schema_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_graphqlserver/_test_graphql.py` & `newrelic-9.9.0/tests/component_graphqlserver/_test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_graphqlserver/conftest.py` & `newrelic-9.9.0/tests/component_graphqlserver/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_graphqlserver/test_graphql.py` & `newrelic-9.9.0/tests/component_graphqlserver/test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_tastypie/api.py` & `newrelic-9.9.0/tests/component_tastypie/api.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_tastypie/conftest.py` & `newrelic-9.9.0/tests/cross_agent/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,9 +23,9 @@
     'transaction_tracer.stack_trace_threshold': 0.0,
     'debug.log_data_collector_payloads': True,
     'debug.record_transaction_failure': True,
     'debug.log_autorum_middleware': True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (component_tastypie)',
+        app_name='Python Agent Test (cross_agent_tests)',
         default_settings=_default_settings)
```

### Comparing `newrelic-9.8.0/tests/component_tastypie/settings.py` & `newrelic-9.9.0/tests/component_tastypie/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_tastypie/test_application.py` & `newrelic-9.9.0/tests/component_tastypie/test_application.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,215 +9,199 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-import six
 import webtest
-
 from tastypie import VERSION
+from testing_support.fixtures import override_ignore_status_codes
+from testing_support.validators.validate_code_level_metrics import (
+    validate_code_level_metrics,
+)
+from testing_support.validators.validate_transaction_errors import (
+    validate_transaction_errors,
+)
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
+from wsgi import application
 
 from newrelic.api.background_task import background_task
 from newrelic.api.transaction import end_of_transaction
-
-from testing_support.fixtures import override_ignore_status_codes
-from testing_support.validators.validate_transaction_errors import validate_transaction_errors
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
-from testing_support.validators.validate_code_level_metrics import validate_code_level_metrics
-
-from wsgi import application
+from newrelic.packages import six
 
 test_application = webtest.TestApp(application)
 
 _test_application_scoped_metrics = [
-        ('Function/django.core.handlers.wsgi:WSGIHandler.__call__', 1),
-        ('Function/django.http.response:HttpResponse.close', 1),
-        ('Python/WSGI/Application', 1),
-        ('Python/WSGI/Response', 1),
-        ('Python/WSGI/Finalize', 1),
+    ("Function/django.core.handlers.wsgi:WSGIHandler.__call__", 1),
+    ("Function/django.http.response:HttpResponse.close", 1),
+    ("Python/WSGI/Application", 1),
+    ("Python/WSGI/Response", 1),
+    ("Python/WSGI/Finalize", 1),
 ]
 
 _test_application_index_scoped_metrics = list(_test_application_scoped_metrics)
-_test_application_index_scoped_metrics.append(
-        ('Function/views:index', 1))
+_test_application_index_scoped_metrics.append(("Function/views:index", 1))
 
 
 @validate_code_level_metrics("views", "index")
 @validate_transaction_errors(errors=[])
-@validate_transaction_metrics('views:index',
-        scoped_metrics=_test_application_index_scoped_metrics)
+@validate_transaction_metrics("views:index", scoped_metrics=_test_application_index_scoped_metrics)
 def test_application_index():
-    response = test_application.get('/index/')
+    response = test_application.get("/index/")
     assert response.status_code == 200
-    response.mustcontain('INDEX RESPONSE')
+    response.mustcontain("INDEX RESPONSE")
 
 
 class TastyPieFullDebugMode(object):
     def __init__(self, tastypie_full_debug):
         from django.conf import settings
+
         self.settings = settings
         self.tastypie_full_debug = tastypie_full_debug
 
     def __enter__(self):
         self.settings.TASTYPIE_FULL_DEBUG = self.tastypie_full_debug
         return 500 if self.tastypie_full_debug else 404
 
     def __exit__(self, *args, **kwargs):
         self.settings.TASTYPIE_FULL_DEBUG = False
 
 
 _test_api_base_scoped_metrics = [
-        ('Function/django.core.handlers.wsgi:WSGIHandler.__call__', 1),
-        ('Python/WSGI/Application', 1),
-        ('Python/WSGI/Response', 1),
-        ('Python/WSGI/Finalize', 1),
+    ("Function/django.core.handlers.wsgi:WSGIHandler.__call__", 1),
+    ("Python/WSGI/Application", 1),
+    ("Python/WSGI/Response", 1),
+    ("Python/WSGI/Finalize", 1),
 ]
 
 if six.PY3:
-    _test_api_base_scoped_metrics.append(
-        ('Function/tastypie.resources:Resource.wrap_view.<locals>.wrapper', 1))
+    _test_api_base_scoped_metrics.append(("Function/tastypie.resources:Resource.wrap_view.<locals>.wrapper", 1))
 else:
-    _test_api_base_scoped_metrics.append(
-            ('Function/tastypie.resources:wrapper', 1))
+    _test_api_base_scoped_metrics.append(("Function/tastypie.resources:wrapper", 1))
 
 # django < 1.12 used the RegexURLResolver class and this was updated to URLResolver in later versions
 if VERSION <= (0, 14, 3) and not six.PY3:
-    _test_api_base_scoped_metrics.append(('Function/django.urls.resolvers:RegexURLResolver.resolve', 1))
+    _test_api_base_scoped_metrics.append(("Function/django.urls.resolvers:RegexURLResolver.resolve", 1))
 else:
-    _test_api_base_scoped_metrics.append(('Function/django.urls.resolvers:URLResolver.resolve', 1))
+    _test_api_base_scoped_metrics.append(("Function/django.urls.resolvers:URLResolver.resolve", 1))
 
 
-_test_application_not_found_scoped_metrics = list(
-        _test_api_base_scoped_metrics)
+_test_application_not_found_scoped_metrics = list(_test_api_base_scoped_metrics)
 
 
-@pytest.mark.parametrize('api_version', ['v1', 'v2'])
-@pytest.mark.parametrize('tastypie_full_debug', [True, False])
+@pytest.mark.parametrize("api_version", ["v1", "v2"])
+@pytest.mark.parametrize("tastypie_full_debug", [True, False])
 def test_not_found(api_version, tastypie_full_debug):
-
-    _test_application_not_found_scoped_metrics = list(
-            _test_api_base_scoped_metrics)
+    _test_application_not_found_scoped_metrics = list(_test_api_base_scoped_metrics)
 
     if tastypie_full_debug:
-        _test_application_not_found_scoped_metrics.append(
-                ('Function/django.http.response:HttpResponse.close', 1))
+        _test_application_not_found_scoped_metrics.append(("Function/django.http.response:HttpResponse.close", 1))
     else:
         _test_application_not_found_scoped_metrics.append(
-                (('Function/django.http.response:'
-                    'HttpResponseNotFound.close'), 1))
+            (("Function/django.http.response:" "HttpResponseNotFound.close"), 1)
+        )
 
     _errors = []
 
     if tastypie_full_debug:
-        _errors.append('tastypie.exceptions:NotFound')
+        _errors.append("tastypie.exceptions:NotFound")
 
     @validate_transaction_errors(errors=_errors)
-    @validate_transaction_metrics('api:SimpleResource.dispatch_detail',
-            scoped_metrics=_test_application_not_found_scoped_metrics)
+    @validate_transaction_metrics(
+        "api:SimpleResource.dispatch_detail", scoped_metrics=_test_application_not_found_scoped_metrics
+    )
     def _test_not_found():
         with TastyPieFullDebugMode(tastypie_full_debug) as debug_status:
-            test_application.get('/api/%s/simple/NotFound/' % api_version,
-                    status=debug_status)
+            test_application.get("/api/%s/simple/NotFound/" % api_version, status=debug_status)
 
     _test_not_found()
 
 
-_test_application_object_does_not_exist_scoped_metrics = list(
-        _test_api_base_scoped_metrics)
+_test_application_object_does_not_exist_scoped_metrics = list(_test_api_base_scoped_metrics)
 
-_test_application_object_does_not_exist_scoped_metrics.append(
-        ('Function/tastypie.http:HttpNotFound.close', 1))
+_test_application_object_does_not_exist_scoped_metrics.append(("Function/tastypie.http:HttpNotFound.close", 1))
 
 
-@pytest.mark.parametrize('api_version', ['v1', 'v2'])
-@pytest.mark.parametrize('tastypie_full_debug', [True, False])
+@pytest.mark.parametrize("api_version", ["v1", "v2"])
+@pytest.mark.parametrize("tastypie_full_debug", [True, False])
 @validate_transaction_errors(errors=[])
-@validate_transaction_metrics('api:SimpleResource.dispatch_detail',
-        scoped_metrics=_test_application_object_does_not_exist_scoped_metrics)
+@validate_transaction_metrics(
+    "api:SimpleResource.dispatch_detail", scoped_metrics=_test_application_object_does_not_exist_scoped_metrics
+)
 def test_object_does_not_exist(api_version, tastypie_full_debug):
     with TastyPieFullDebugMode(tastypie_full_debug):
-        test_application.get(
-                '/api/%s/simple/ObjectDoesNotExist/' % api_version, status=404)
+        test_application.get("/api/%s/simple/ObjectDoesNotExist/" % api_version, status=404)
 
 
 _test_application_raises_zerodivision = list(_test_api_base_scoped_metrics)
 _test_application_raises_zerodivision_exceptions = []
 
 if six.PY3:
-    _test_application_raises_zerodivision_exceptions.append(
-            'builtins:ZeroDivisionError')
+    _test_application_raises_zerodivision_exceptions.append("builtins:ZeroDivisionError")
 else:
-    _test_application_raises_zerodivision_exceptions.append(
-            'exceptions:ZeroDivisionError')
+    _test_application_raises_zerodivision_exceptions.append("exceptions:ZeroDivisionError")
 
 
-@pytest.mark.parametrize('api_version', ['v1', 'v2'])
-@pytest.mark.parametrize('tastypie_full_debug', [True, False])
-@validate_transaction_errors(
-        errors=_test_application_raises_zerodivision_exceptions)
+@pytest.mark.parametrize("api_version", ["v1", "v2"])
+@pytest.mark.parametrize("tastypie_full_debug", [True, False])
+@validate_transaction_errors(errors=_test_application_raises_zerodivision_exceptions)
 def test_raises_zerodivision(api_version, tastypie_full_debug):
-
     _test_application_raises_zerodivision = list(_test_api_base_scoped_metrics)
 
     if tastypie_full_debug:
         _test_application_raises_zerodivision.append(
-                (('Function/django.core.handlers.exception:'
-                    'handle_uncaught_exception'), 1))
+            (("Function/django.core.handlers.exception:" "handle_uncaught_exception"), 1)
+        )
     else:
-        _test_application_raises_zerodivision.append(
-                ('Function/tastypie.http:HttpApplicationError.close', 1))
+        _test_application_raises_zerodivision.append(("Function/tastypie.http:HttpApplicationError.close", 1))
 
-    @validate_transaction_metrics('api:SimpleResource.dispatch_detail',
-            scoped_metrics=_test_application_raises_zerodivision)
+    @validate_transaction_metrics(
+        "api:SimpleResource.dispatch_detail", scoped_metrics=_test_application_raises_zerodivision
+    )
     def _test_raises_zerodivision():
         with TastyPieFullDebugMode(tastypie_full_debug):
-            test_application.get(
-                    '/api/%s/simple/ZeroDivisionError/' % api_version,
-                    status=500)
+            test_application.get("/api/%s/simple/ZeroDivisionError/" % api_version, status=500)
 
     _test_raises_zerodivision()
 
 
-@pytest.mark.parametrize('api_version', ['v1', 'v2'])
-@pytest.mark.parametrize('tastypie_full_debug', [True, False])
+@pytest.mark.parametrize("api_version", ["v1", "v2"])
+@pytest.mark.parametrize("tastypie_full_debug", [True, False])
 @override_ignore_status_codes(set())  # don't ignore any status codes
-@validate_transaction_errors(errors=['tastypie.exceptions:NotFound'])
-@validate_transaction_metrics('api:SimpleResource.dispatch_detail',
-        scoped_metrics=_test_application_not_found_scoped_metrics)
+@validate_transaction_errors(errors=["tastypie.exceptions:NotFound"])
+@validate_transaction_metrics(
+    "api:SimpleResource.dispatch_detail", scoped_metrics=_test_application_not_found_scoped_metrics
+)
 def test_record_404_errors(api_version, tastypie_full_debug):
-
-    _test_application_not_found_scoped_metrics = list(
-            _test_api_base_scoped_metrics)
+    _test_application_not_found_scoped_metrics = list(_test_api_base_scoped_metrics)
 
     if tastypie_full_debug:
-        _test_application_not_found_scoped_metrics.append(
-                ('Function/django.http.response:HttpResponse.close', 1))
+        _test_application_not_found_scoped_metrics.append(("Function/django.http.response:HttpResponse.close", 1))
     else:
         _test_application_not_found_scoped_metrics.append(
-                (('Function/django.http.response:'
-                    'HttpResponseNotFound.close'), 1))
+            (("Function/django.http.response:" "HttpResponseNotFound.close"), 1)
+        )
 
-    @validate_transaction_metrics('api:SimpleResource.dispatch_detail',
-            scoped_metrics=_test_application_not_found_scoped_metrics)
+    @validate_transaction_metrics(
+        "api:SimpleResource.dispatch_detail", scoped_metrics=_test_application_not_found_scoped_metrics
+    )
     def _test_not_found():
         with TastyPieFullDebugMode(tastypie_full_debug) as debug_status:
-            test_application.get('/api/%s/simple/NotFound/' % api_version,
-                    status=debug_status)
+            test_application.get("/api/%s/simple/NotFound/" % api_version, status=debug_status)
 
     _test_not_found()
 
 
-@pytest.mark.parametrize('api_version', ['v1', 'v2'])
-@pytest.mark.parametrize('tastypie_full_debug', [True, False])
+@pytest.mark.parametrize("api_version", ["v1", "v2"])
+@pytest.mark.parametrize("tastypie_full_debug", [True, False])
 @validate_transaction_errors(errors=[])
-@validate_transaction_metrics('test_application:test_ended_txn_name',
-        background_task=True)
+@validate_transaction_metrics("test_application:test_ended_txn_name", background_task=True)
 @background_task()
 def test_ended_txn_name(api_version, tastypie_full_debug):
     # if the transaction has ended, do not change the transaction name
     end_of_transaction()
 
     with TastyPieFullDebugMode(tastypie_full_debug) as debug_status:
-        test_application.get('/api/%s/simple/NotFound/' % api_version,
-                status=debug_status)
+        test_application.get("/api/%s/simple/NotFound/" % api_version, status=debug_status)
```

### Comparing `newrelic-9.8.0/tests/component_tastypie/urls.py` & `newrelic-9.9.0/tests/component_tastypie/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_tastypie/views.py` & `newrelic-9.9.0/tests/component_tastypie/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/component_tastypie/wsgi.py` & `newrelic-9.9.0/tests/component_tastypie/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/coroutines_asyncio/conftest.py` & `newrelic-9.9.0/tests/coroutines_asyncio/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/coroutines_asyncio/test_context_propagation.py` & `newrelic-9.9.0/tests/coroutines_asyncio/test_context_propagation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/conftest.py` & `newrelic-9.9.0/tests/template_jinja2/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pytest
-
-from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
-
+from testing_support.fixtures import (  # noqa: F401; pylint: disable=W0611
+    collector_agent_registration_fixture,
+    collector_available_fixture,
+)
 
 _default_settings = {
-    'transaction_tracer.explain_threshold': 0.0,
-    'transaction_tracer.transaction_threshold': 0.0,
-    'transaction_tracer.stack_trace_threshold': 0.0,
-    'debug.log_data_collector_payloads': True,
-    'debug.record_transaction_failure': True,
-    'debug.log_autorum_middleware': True,
+    "transaction_tracer.explain_threshold": 0.0,
+    "transaction_tracer.transaction_threshold": 0.0,
+    "transaction_tracer.stack_trace_threshold": 0.0,
+    "debug.log_data_collector_payloads": True,
+    "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (cross_agent_tests)',
-        default_settings=_default_settings)
+    app_name="Python Agent Test (template_jinja2)", default_settings=_default_settings
+)
```

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/README.md` & `newrelic-9.9.0/tests/cross_agent/fixtures/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/attribute_configuration.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/attribute_configuration.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/cat_map.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/cat_map.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/collector_hostname.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/collector_hostname.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/datastores/README.md` & `newrelic-9.9.0/tests/cross_agent/fixtures/datastores/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/datastores/datastore_instances.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/datastores/datastore_instances.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/distributed_tracing/README.md` & `newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/distributed_tracing/trace_context.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/distributed_tracing/trace_context.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/cases.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/cases.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/cases.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/cases.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-20.10.16.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-20.10.16.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-24.0.2.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-24.0.2.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-too-long.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/docker-too-long.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-characters.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-characters.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-length.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/docker_container_id_v2/invalid-length.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/labels.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/labels.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/codecommit.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/codecommit.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/s3_put.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_put.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/ses.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/ses.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/sns.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/sns.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source/sqs.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source/sqs.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/lambda_event_source.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/lambda_event_source.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md` & `newrelic-9.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/README.md` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt` & `newrelic-9.9.0/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rules.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/rules.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_cookie.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_cookie.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html` & `newrelic-9.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/README.md` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/sql_parsing.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/sql_parsing.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/transaction_segment_terms.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/transaction_segment_terms.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/url_clean.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/url_clean.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/url_domain_extraction.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/url_domain_extraction.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/utilization/README.md` & `newrelic-9.9.0/tests/cross_agent/fixtures/utilization/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/utilization/boot_id.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/utilization/boot_id.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/utilization/utilization_json.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/utilization/utilization_json.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/README.md` & `newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json` & `newrelic-9.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_agent_attributes.py` & `newrelic-9.9.0/tests/cross_agent/test_agent_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_aws_utilization_data.py` & `newrelic-9.9.0/tests/cross_agent/test_aws_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_azure_utilization_data.py` & `newrelic-9.9.0/tests/cross_agent/test_azure_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_boot_id_utilization_data.py` & `newrelic-9.9.0/tests/cross_agent/test_boot_id_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_cat_map.py` & `newrelic-9.9.0/tests/cross_agent/test_cat_map.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_collector_hostname.py` & `newrelic-9.9.0/tests/cross_agent/test_collector_hostname.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_datastore_instance.py` & `newrelic-9.9.0/tests/cross_agent/test_datastore_instance.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_distributed_tracing.py` & `newrelic-9.9.0/tests/cross_agent/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_docker_container_id.py` & `newrelic-9.9.0/tests/cross_agent/test_docker_container_id.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_docker_container_id_v2.py` & `newrelic-9.9.0/tests/cross_agent/test_docker_container_id_v2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_gcp_utilization_data.py` & `newrelic-9.9.0/tests/cross_agent/test_gcp_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_labels_and_rollups.py` & `newrelic-9.9.0/tests/cross_agent/test_labels_and_rollups.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_lambda_event_source.py` & `newrelic-9.9.0/tests/cross_agent/test_lambda_event_source.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_pcf_utilization_data.py` & `newrelic-9.9.0/tests/cross_agent/test_pcf_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_rules.py` & `newrelic-9.9.0/tests/cross_agent/test_rules.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_sql_obfuscation.py` & `newrelic-9.9.0/tests/cross_agent/test_sql_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_system_info.py` & `newrelic-9.9.0/tests/cross_agent/test_system_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_transaction_segment_terms.py` & `newrelic-9.9.0/tests/cross_agent/test_transaction_segment_terms.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_utilization_configs.py` & `newrelic-9.9.0/tests/cross_agent/test_utilization_configs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/cross_agent/test_w3c_trace_context.py` & `newrelic-9.9.0/tests/cross_agent/test_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aioredis/conftest.py` & `newrelic-9.9.0/tests/datastore_aioredis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aioredis/test_custom_conn_pool.py` & `newrelic-9.9.0/tests/datastore_aioredis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aioredis/test_execute_command.py` & `newrelic-9.9.0/tests/datastore_aioredis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aioredis/test_get_and_set.py` & `newrelic-9.9.0/tests/datastore_aioredis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aioredis/test_instance_info.py` & `newrelic-9.9.0/tests/datastore_aioredis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aioredis/test_multiple_dbs.py` & `newrelic-9.9.0/tests/datastore_aioredis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aioredis/test_span_event.py` & `newrelic-9.9.0/tests/datastore_aioredis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aioredis/test_trace_node.py` & `newrelic-9.9.0/tests/datastore_aioredis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aioredis/test_transactions.py` & `newrelic-9.9.0/tests/datastore_aioredis/test_transactions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aioredis/test_uninstrumented_methods.py` & `newrelic-9.9.0/tests/datastore_aioredis/test_uninstrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aredis/conftest.py` & `newrelic-9.9.0/tests/datastore_aredis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aredis/test_custom_conn_pool.py` & `newrelic-9.9.0/tests/datastore_aredis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aredis/test_execute_command.py` & `newrelic-9.9.0/tests/datastore_aredis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aredis/test_get_and_set.py` & `newrelic-9.9.0/tests/datastore_aredis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aredis/test_instance_info.py` & `newrelic-9.9.0/tests/datastore_aredis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aredis/test_multiple_dbs.py` & `newrelic-9.9.0/tests/datastore_aredis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aredis/test_span_event.py` & `newrelic-9.9.0/tests/datastore_aredis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aredis/test_trace_node.py` & `newrelic-9.9.0/tests/datastore_aredis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_aredis/test_uninstrumented_methods.py` & `newrelic-9.9.0/tests/datastore_aredis/test_uninstrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_asyncpg/conftest.py` & `newrelic-9.9.0/tests/datastore_asyncpg/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_asyncpg/test_multiple_dbs.py` & `newrelic-9.9.0/tests/datastore_asyncpg/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_asyncpg/test_query.py` & `newrelic-9.9.0/tests/datastore_asyncpg/test_query.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_bmemcached/conftest.py` & `newrelic-9.9.0/tests/datastore_bmemcached/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_bmemcached/test_memcache.py` & `newrelic-9.9.0/tests/datastore_bmemcached/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_elasticsearch/conftest.py` & `newrelic-9.9.0/tests/datastore_elasticsearch/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_elasticsearch/test_connection.py` & `newrelic-9.9.0/tests/datastore_elasticsearch/test_connection.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_elasticsearch/test_database_duration.py` & `newrelic-9.9.0/tests/datastore_elasticsearch/test_database_duration.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_elasticsearch/test_elasticsearch.py` & `newrelic-9.9.0/tests/datastore_elasticsearch/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_elasticsearch/test_instrumented_methods.py` & `newrelic-9.9.0/tests/datastore_elasticsearch/test_instrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_elasticsearch/test_mget.py` & `newrelic-9.9.0/tests/datastore_elasticsearch/test_mget.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_elasticsearch/test_multiple_dbs.py` & `newrelic-9.9.0/tests/datastore_elasticsearch/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_elasticsearch/test_trace_node.py` & `newrelic-9.9.0/tests/datastore_elasticsearch/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_elasticsearch/test_transport.py` & `newrelic-9.9.0/tests/datastore_elasticsearch/test_transport.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/conftest.py` & `newrelic-9.9.0/tests/datastore_firestore/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_async_batching.py` & `newrelic-9.9.0/tests/datastore_firestore/test_async_batching.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_async_client.py` & `newrelic-9.9.0/tests/datastore_firestore/test_async_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_async_collections.py` & `newrelic-9.9.0/tests/datastore_firestore/test_async_collections.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_async_documents.py` & `newrelic-9.9.0/tests/datastore_firestore/test_async_documents.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_async_query.py` & `newrelic-9.9.0/tests/datastore_firestore/test_async_query.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_async_transaction.py` & `newrelic-9.9.0/tests/datastore_firestore/test_async_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_batching.py` & `newrelic-9.9.0/tests/datastore_firestore/test_batching.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_client.py` & `newrelic-9.9.0/tests/datastore_firestore/test_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_collections.py` & `newrelic-9.9.0/tests/datastore_firestore/test_collections.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_documents.py` & `newrelic-9.9.0/tests/datastore_firestore/test_documents.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_query.py` & `newrelic-9.9.0/tests/datastore_firestore/test_query.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_firestore/test_transaction.py` & `newrelic-9.9.0/tests/datastore_firestore/test_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_memcache/conftest.py` & `newrelic-9.9.0/tests/datastore_memcache/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_memcache/test_all_methods_wrapped.py` & `newrelic-9.9.0/tests/datastore_memcache/test_all_methods_wrapped.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_memcache/test_memcache.py` & `newrelic-9.9.0/tests/datastore_memcache/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_memcache/test_multiple_dbs.py` & `newrelic-9.9.0/tests/datastore_memcache/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_memcache/test_span_event.py` & `newrelic-9.9.0/tests/datastore_memcache/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_mysql/conftest.py` & `newrelic-9.9.0/tests/datastore_mysql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_mysql/test_database.py` & `newrelic-9.9.0/tests/datastore_mysql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_postgresql/conftest.py` & `newrelic-9.9.0/tests/datastore_postgresql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_postgresql/test_database.py` & `newrelic-9.9.0/tests/datastore_postgresql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/conftest.py` & `newrelic-9.9.0/tests/datastore_psycopg2/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_as_string.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_as_string.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_async.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_cursor.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_cursor.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_database_instance_info.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_database_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_explain_plans.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_explain_plans.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_forward_compat.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_forward_compat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_multiple_dbs.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_obfuscation.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_register.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_register.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_rollback.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_rollback.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_slow_sql.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_slow_sql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_span_event.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/test_trace_node.py` & `newrelic-9.9.0/tests/datastore_psycopg2/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2/utils.py` & `newrelic-9.9.0/tests/datastore_psycopg2/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2cffi/conftest.py` & `newrelic-9.9.0/tests/datastore_psycopg2cffi/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2cffi/test_database.py` & `newrelic-9.9.0/tests/datastore_psycopg2cffi/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_psycopg2cffi/test_explain_plans.py` & `newrelic-9.9.0/tests/datastore_psycopg2cffi/test_explain_plans.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pylibmc/conftest.py` & `newrelic-9.9.0/tests/datastore_pylibmc/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pylibmc/test_memcache.py` & `newrelic-9.9.0/tests/datastore_pylibmc/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pymemcache/conftest.py` & `newrelic-9.9.0/tests/datastore_pymemcache/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pymemcache/test_memcache.py` & `newrelic-9.9.0/tests/datastore_pymemcache/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pymongo/conftest.py` & `newrelic-9.9.0/tests/datastore_pymongo/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pymongo/test_pymongo.py` & `newrelic-9.9.0/tests/datastore_pymongo/test_pymongo.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pymssql/conftest.py` & `newrelic-9.9.0/tests/datastore_pymssql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pymssql/test_database.py` & `newrelic-9.9.0/tests/datastore_pymssql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pymysql/conftest.py` & `newrelic-9.9.0/tests/datastore_pymysql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pymysql/test_database.py` & `newrelic-9.9.0/tests/datastore_pymysql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pyodbc/conftest.py` & `newrelic-9.9.0/tests/datastore_pyodbc/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pyodbc/test_pyodbc.py` & `newrelic-9.9.0/tests/datastore_pyodbc/test_pyodbc.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pysolr/conftest.py` & `newrelic-9.9.0/tests/datastore_pysolr/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_pysolr/test_solr.py` & `newrelic-9.9.0/tests/datastore_pysolr/test_solr.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/conftest.py` & `newrelic-9.9.0/tests/datastore_redis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_asyncio.py` & `newrelic-9.9.0/tests/datastore_redis/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_custom_conn_pool.py` & `newrelic-9.9.0/tests/datastore_redis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_execute_command.py` & `newrelic-9.9.0/tests/datastore_redis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_generators.py` & `newrelic-9.9.0/tests/datastore_redis/test_generators.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_get_and_set.py` & `newrelic-9.9.0/tests/datastore_redis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_instance_info.py` & `newrelic-9.9.0/tests/datastore_redis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_multiple_dbs.py` & `newrelic-9.9.0/tests/datastore_redis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_rb.py` & `newrelic-9.9.0/tests/datastore_redis/test_rb.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,130 +8,120 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-''' The purpose of these tests is to confirm that we will record
+""" The purpose of these tests is to confirm that we will record
 record instance info for Redis Blaster commands that go through
 redis.Connection:send_command(). Commands that don't use send_command,
 like the one that use the fanout client, won't have instance info.
-'''
+"""
 
 import pytest
-import redis
-import six
+from testing_support.db_settings import redis_settings
+from testing_support.fixtures import override_application_settings
+from testing_support.util import instance_hostname
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
 
 from newrelic.api.background_task import background_task
 from newrelic.common.package_version_utils import get_package_version_tuple
-
-from testing_support.fixtures import override_application_settings
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
-from testing_support.db_settings import redis_settings
-from testing_support.util import instance_hostname
+from newrelic.packages import six
 
 DB_SETTINGS = redis_settings()[0]
 REDIS_PY_VERSION = get_package_version_tuple("redis")
 
 
 # Settings
 
 _enable_instance_settings = {
-    'datastore_tracer.instance_reporting.enabled': True,
+    "datastore_tracer.instance_reporting.enabled": True,
 }
 _disable_instance_settings = {
-    'datastore_tracer.instance_reporting.enabled': False,
+    "datastore_tracer.instance_reporting.enabled": False,
 }
 
 # Metrics
 
 # We don't record instance metrics when using redis blaster,
 # so we just check for base metrics.
 
 _base_scoped_metrics = (
-        ('Datastore/operation/Redis/get', 1),
-        ('Datastore/operation/Redis/set', 1),
+    ("Datastore/operation/Redis/get", 1),
+    ("Datastore/operation/Redis/set", 1),
 )
 
 _base_rollup_metrics = (
-        ('Datastore/all', 2),
-        ('Datastore/allOther', 2),
-        ('Datastore/Redis/all', 2),
-        ('Datastore/Redis/allOther', 2),
-        ('Datastore/operation/Redis/get', 1),
-        ('Datastore/operation/Redis/set', 1),
+    ("Datastore/all", 2),
+    ("Datastore/allOther", 2),
+    ("Datastore/Redis/all", 2),
+    ("Datastore/Redis/allOther", 2),
+    ("Datastore/operation/Redis/get", 1),
+    ("Datastore/operation/Redis/set", 1),
 )
 
 _disable_rollup_metrics = list(_base_rollup_metrics)
 _enable_rollup_metrics = list(_base_rollup_metrics)
 
-_host = instance_hostname(DB_SETTINGS['host'])
-_port = DB_SETTINGS['port']
+_host = instance_hostname(DB_SETTINGS["host"])
+_port = DB_SETTINGS["port"]
 
-_instance_metric_name = 'Datastore/instance/Redis/%s/%s' % (_host, _port)
+_instance_metric_name = "Datastore/instance/Redis/%s/%s" % (_host, _port)
 
-_enable_rollup_metrics.append(
-        (_instance_metric_name, 2)
-)
+_enable_rollup_metrics.append((_instance_metric_name, 2))
 
-_disable_rollup_metrics.append(
-        (_instance_metric_name, None)
-)
+_disable_rollup_metrics.append((_instance_metric_name, None))
 
 
 # Operations
 def exercise_redis(routing_client):
-    routing_client.set('key', 'value')
-    routing_client.get('key')
+    routing_client.set("key", "value")
+    routing_client.get("key")
 
 
 def exercise_fanout(cluster):
-    with cluster.fanout(hosts='all') as client:
-        client.execute_command('CLIENT', 'LIST')
+    with cluster.fanout(hosts="all") as client:
+        client.execute_command("CLIENT", "LIST")
 
 
 # Tests
-@pytest.mark.skipif(six.PY3, reason='Redis Blaster is Python 2 only.')
-@pytest.mark.skipif(REDIS_PY_VERSION < (2, 10, 2),
-        reason='Redis Blaster requires redis>=2.10.2')
+@pytest.mark.skipif(six.PY3, reason="Redis Blaster is Python 2 only.")
+@pytest.mark.skipif(REDIS_PY_VERSION < (2, 10, 2), reason="Redis Blaster requires redis>=2.10.2")
 @override_application_settings(_enable_instance_settings)
 @validate_transaction_metrics(
-        'test_rb:test_redis_blaster_operation_enable_instance',
-        scoped_metrics=_base_scoped_metrics,
-        rollup_metrics=_enable_rollup_metrics,
-        background_task=True)
+    "test_rb:test_redis_blaster_operation_enable_instance",
+    scoped_metrics=_base_scoped_metrics,
+    rollup_metrics=_enable_rollup_metrics,
+    background_task=True,
+)
 @background_task()
 def test_redis_blaster_operation_enable_instance():
     from rb import Cluster
 
-    cluster = Cluster(
-            hosts={0: {'port': DB_SETTINGS['port']}},
-            host_defaults={'host': DB_SETTINGS['host']}
-    )
+    cluster = Cluster(hosts={0: {"port": DB_SETTINGS["port"]}}, host_defaults={"host": DB_SETTINGS["host"]})
     exercise_fanout(cluster)
 
     client = cluster.get_routing_client()
     exercise_redis(client)
 
 
-@pytest.mark.skipif(six.PY3, reason='Redis Blaster is Python 2 only.')
-@pytest.mark.skipif(REDIS_PY_VERSION < (2, 10,2 ),
-        reason='Redis Blaster requires redis>=2.10.2')
+@pytest.mark.skipif(six.PY3, reason="Redis Blaster is Python 2 only.")
+@pytest.mark.skipif(REDIS_PY_VERSION < (2, 10, 2), reason="Redis Blaster requires redis>=2.10.2")
 @override_application_settings(_disable_instance_settings)
 @validate_transaction_metrics(
-        'test_rb:test_redis_blaster_operation_disable_instance',
-        scoped_metrics=_base_scoped_metrics,
-        rollup_metrics=_disable_rollup_metrics,
-        background_task=True)
+    "test_rb:test_redis_blaster_operation_disable_instance",
+    scoped_metrics=_base_scoped_metrics,
+    rollup_metrics=_disable_rollup_metrics,
+    background_task=True,
+)
 @background_task()
 def test_redis_blaster_operation_disable_instance():
     from rb import Cluster
 
-    cluster = Cluster(
-            hosts={0: {'port': DB_SETTINGS['port']}},
-            host_defaults={'host': DB_SETTINGS['host']}
-    )
+    cluster = Cluster(hosts={0: {"port": DB_SETTINGS["port"]}}, host_defaults={"host": DB_SETTINGS["host"]})
     exercise_fanout(cluster)
 
     client = cluster.get_routing_client()
     exercise_redis(client)
```

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_span_event.py` & `newrelic-9.9.0/tests/datastore_redis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_trace_node.py` & `newrelic-9.9.0/tests/datastore_redis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_redis/test_uninstrumented_methods.py` & `newrelic-9.9.0/tests/datastore_redis/test_uninstrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_rediscluster/conftest.py` & `newrelic-9.9.0/tests/datastore_rediscluster/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_rediscluster/test_uninstrumented_rediscluster_methods.py` & `newrelic-9.9.0/tests/datastore_rediscluster/test_uninstrumented_rediscluster_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_solrpy/conftest.py` & `newrelic-9.9.0/tests/datastore_solrpy/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_solrpy/test_solr.py` & `newrelic-9.9.0/tests/datastore_solrpy/test_solr.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_sqlite/conftest.py` & `newrelic-9.9.0/tests/datastore_sqlite/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_sqlite/test_database.py` & `newrelic-9.9.0/tests/datastore_sqlite/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/datastore_sqlite/test_obfuscation.py` & `newrelic-9.9.0/tests/datastore_sqlite/test_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/_mock_bedrock_encoding_utils.py` & `newrelic-9.9.0/tests/external_botocore/_mock_bedrock_encoding_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/_mock_external_bedrock_server.py` & `newrelic-9.9.0/tests/external_botocore/_mock_external_bedrock_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/_test_bedrock_chat_completion.py` & `newrelic-9.9.0/tests/external_botocore/_test_bedrock_chat_completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,15 +591,15 @@
             {
                 "id": None,  # UUID that varies with each run
                 "llm.conversation_id": "my-awesome-id",
                 "llm.foo": "bar",
                 "request_id": "1a72a1f6-310f-469c-af1d-2c59eb600089",
                 "span_id": None,
                 "trace_id": "trace-id",
-                "content": "[{'type': 'text', 'text': \"Hello! It's nice to meet you.\"}]",
+                "content": "{'type': 'text', 'text': \"Hello! It's nice to meet you.\"}",
                 "role": "assistant",
                 "completion_id": None,
                 "sequence": 1,
                 "response.model": "anthropic.claude-instant-v1",
                 "vendor": "bedrock",
                 "ingest_source": "Python",
                 "is_response": True,
```

### Comparing `newrelic-9.8.0/tests/external_botocore/_test_bedrock_embeddings.py` & `newrelic-9.9.0/tests/external_botocore/_test_bedrock_embeddings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/conftest.py` & `newrelic-9.9.0/tests/external_botocore/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/test_bedrock_chat_completion.py` & `newrelic-9.9.0/tests/external_botocore/test_bedrock_chat_completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,26 +33,26 @@
     chat_completion_streaming_expected_events,
 )
 from conftest import BOTOCORE_VERSION  # pylint: disable=E0611
 from testing_support.fixtures import (
     override_llm_token_callback_settings,
     reset_core_stats_engine,
     validate_attributes,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     disabled_ai_monitoring_streaming_settings,
     events_sans_content,
     events_sans_llm_metadata,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
```

### Comparing `newrelic-9.8.0/tests/external_botocore/test_bedrock_chat_completion_via_langchain.py` & `newrelic-9.9.0/tests/external_botocore/test_bedrock_chat_completion_via_langchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,17 @@
 
 import pytest
 from _test_bedrock_chat_completion import (
     chat_completion_langchain_expected_events,
     chat_completion_langchain_expected_streaming_events,
 )
 from conftest import BOTOCORE_VERSION  # pylint: disable=E0611
-from testing_support.fixtures import (
-    reset_core_stats_engine,
-    validate_attributes,
-    validate_custom_event_count,
-)
+from testing_support.fixtures import reset_core_stats_engine, validate_attributes
 from testing_support.ml_testing_utils import set_trace_info  # noqa: F401
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
 
 from newrelic.api.background_task import background_task
 from newrelic.api.transaction import add_custom_attribute
```

### Comparing `newrelic-9.8.0/tests/external_botocore/test_bedrock_embeddings.py` & `newrelic-9.9.0/tests/external_botocore/test_bedrock_embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,25 +26,25 @@
     embedding_payload_templates,
 )
 from conftest import BOTOCORE_VERSION  # pylint: disable=E0611
 from testing_support.fixtures import (
     override_llm_token_callback_settings,
     reset_core_stats_engine,
     validate_attributes,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     events_sans_content,
     events_sans_llm_metadata,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
```

### Comparing `newrelic-9.8.0/tests/external_botocore/test_boto3_iam.py` & `newrelic-9.9.0/tests/external_botocore/test_boto3_iam.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/test_boto3_s3.py` & `newrelic-9.9.0/tests/external_botocore/test_boto3_s3.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/test_boto3_sns.py` & `newrelic-9.9.0/tests/external_botocore/test_boto3_sns.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/test_botocore_dynamodb.py` & `newrelic-9.9.0/tests/external_botocore/test_botocore_dynamodb.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/test_botocore_ec2.py` & `newrelic-9.9.0/tests/external_botocore/test_botocore_ec2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/test_botocore_s3.py` & `newrelic-9.9.0/tests/external_botocore/test_botocore_s3.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_botocore/test_botocore_sqs.py` & `newrelic-9.9.0/tests/external_botocore/test_botocore_sqs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_feedparser/conftest.py` & `newrelic-9.9.0/tests/external_feedparser/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_feedparser/packages.xml` & `newrelic-9.9.0/tests/external_feedparser/packages.xml`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_feedparser/test_feedparser.py` & `newrelic-9.9.0/tests/external_feedparser/test_feedparser.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_http/conftest.py` & `newrelic-9.9.0/tests/external_http/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_http/test_http.py` & `newrelic-9.9.0/tests/external_http/test_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,32 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-import six
 from testing_support.external_fixtures import (
     cache_outgoing_headers,
     insert_incoming_headers,
 )
-from testing_support.fixtures import (
-    cat_enabled,
-    override_application_settings,
-)
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
+from testing_support.fixtures import cat_enabled, override_application_settings
 from testing_support.validators.validate_cross_process_headers import (
     validate_cross_process_headers,
 )
 from testing_support.validators.validate_external_node_params import (
     validate_external_node_params,
 )
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
 
 from newrelic.api.background_task import background_task
+from newrelic.packages import six
 
 if six.PY2:
     import httplib
 else:
     import http.client as httplib
```

### Comparing `newrelic-9.8.0/tests/external_httplib/conftest.py` & `newrelic-9.9.0/tests/external_httplib/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_httplib/test_httplib.py` & `newrelic-9.9.0/tests/external_httplib/test_httplib.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_httplib/test_urllib.py` & `newrelic-9.9.0/tests/external_httplib/test_urllib.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_httplib/test_urllib2.py` & `newrelic-9.9.0/tests/external_httplib/test_urllib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_httplib2/conftest.py` & `newrelic-9.9.0/tests/external_httplib2/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_httplib2/test_httplib2.py` & `newrelic-9.9.0/tests/external_httplib2/test_httplib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_httpx/conftest.py` & `newrelic-9.9.0/tests/external_httpx/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_httpx/test_client.py` & `newrelic-9.9.0/tests/external_httpx/test_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_requests/conftest.py` & `newrelic-9.9.0/tests/external_requests/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_requests/test_requests.py` & `newrelic-9.9.0/tests/external_requests/test_requests.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_requests/test_span_event.py` & `newrelic-9.9.0/tests/external_requests/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_urllib3/conftest.py` & `newrelic-9.9.0/tests/external_urllib3/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/external_urllib3/test_urllib3.py` & `newrelic-9.9.0/tests/external_urllib3/test_urllib3.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_aiohttp/_target_application.py` & `newrelic-9.9.0/tests/framework_aiohttp/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_aiohttp/conftest.py` & `newrelic-9.9.0/tests/framework_aiohttp/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_aiohttp/test_client.py` & `newrelic-9.9.0/tests/framework_aiohttp/test_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_aiohttp/test_client_async_await.py` & `newrelic-9.9.0/tests/framework_aiohttp/test_client_async_await.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 # limitations under the License.
 
 import asyncio
 
 import aiohttp
 import pytest
 from testing_support.fixtures import cat_enabled
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
 from yarl import URL
 
 from newrelic.api.background_task import background_task
 from newrelic.api.function_trace import function_trace
 
 version_info = tuple(int(_) for _ in aiohttp.__version__.split(".")[:2])
 
@@ -111,76 +113,14 @@
     def task_test():
         task(event_loop, method, exc_expected, local_server_info.url)
 
     task_test()
 
 
 @pytest.mark.parametrize("method,exc_expected", test_matrix)
-def test_client_throw_async_await(event_loop, local_server_info, method, exc_expected):
-    class ThrowerException(ValueError):
-        pass
-
-    @background_task(name="test_client_throw_async_await")
-    async def self_driving_thrower():
-        async with aiohttp.ClientSession() as session:
-            coro = session._request(method.upper(), local_server_info.url)
-
-            # activate the coroutine
-            coro.send(None)
-
-            # inject error
-            coro.throw(ThrowerException())
-
-    @validate_transaction_metrics(
-        "test_client_throw_async_await",
-        background_task=True,
-        scoped_metrics=[
-            (local_server_info.base_metric + method.upper(), 1),
-        ],
-        rollup_metrics=[
-            (local_server_info.base_metric + method.upper(), 1),
-        ],
-    )
-    def task_test():
-        with pytest.raises(ThrowerException):
-            event_loop.run_until_complete(self_driving_thrower())
-
-    task_test()
-
-
-@pytest.mark.parametrize("method,exc_expected", test_matrix)
-def test_client_close_async_await(event_loop, local_server_info, method, exc_expected):
-    @background_task(name="test_client_close_async_await")
-    async def self_driving_closer():
-        async with aiohttp.ClientSession() as session:
-            coro = session._request(method.upper(), local_server_info.url)
-
-            # activate the coroutine
-            coro.send(None)
-
-            # force close
-            coro.close()
-
-    @validate_transaction_metrics(
-        "test_client_close_async_await",
-        background_task=True,
-        scoped_metrics=[
-            (local_server_info.base_metric + method.upper(), 1),
-        ],
-        rollup_metrics=[
-            (local_server_info.base_metric + method.upper(), 1),
-        ],
-    )
-    def task_test():
-        event_loop.run_until_complete(self_driving_closer())
-
-    task_test()
-
-
-@pytest.mark.parametrize("method,exc_expected", test_matrix)
 @cat_enabled
 def test_await_request_async_await(event_loop, local_server_info, method, exc_expected):
     async def request_with_await():
         async with aiohttp.ClientSession() as session:
             coro = session._request(method.upper(), local_server_info.url)
 
             # force await
@@ -236,15 +176,14 @@
 
     task_test()
 
 
 @pytest.mark.parametrize("method,exc_expected", test_matrix)
 @cat_enabled
 def test_create_task_async_await(event_loop, local_server_info, method, exc_expected):
-
     # `loop.create_task` returns a Task object which uses the coroutine's
     # `send` method, not `__next__`
 
     async def fetch_task(loop):
         async with aiohttp.ClientSession() as session:
             coro = getattr(session, method)
             resp = await loop.create_task(coro(local_server_info.url))
```

### Comparing `newrelic-9.8.0/tests/framework_aiohttp/test_client_cat.py` & `newrelic-9.9.0/tests/framework_aiohttp/test_client_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_aiohttp/test_externals.py` & `newrelic-9.9.0/tests/framework_aiohttp/test_externals.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_aiohttp/test_middleware.py` & `newrelic-9.9.0/tests/framework_aiohttp/test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_aiohttp/test_server.py` & `newrelic-9.9.0/tests/framework_aiohttp/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_aiohttp/test_server_cat.py` & `newrelic-9.9.0/tests/framework_aiohttp/test_server_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_aiohttp/test_ws.py` & `newrelic-9.9.0/tests/framework_aiohttp/test_ws.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_ariadne/__init__.py` & `newrelic-9.9.0/tests/framework_ariadne/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_ariadne/_target_application.py` & `newrelic-9.9.0/tests/framework_ariadne/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_ariadne/_target_schema_async.py` & `newrelic-9.9.0/tests/framework_ariadne/_target_schema_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_ariadne/_target_schema_sync.py` & `newrelic-9.9.0/tests/framework_ariadne/_target_schema_sync.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_ariadne/conftest.py` & `newrelic-9.9.0/tests/framework_strawberry/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,29 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import six
 from testing_support.fixtures import (  # noqa: F401; pylint: disable=W0611
     collector_agent_registration_fixture,
     collector_available_fixture,
 )
 
 _default_settings = {
     "transaction_tracer.explain_threshold": 0.0,
     "transaction_tracer.transaction_threshold": 0.0,
     "transaction_tracer.stack_trace_threshold": 0.0,
     "debug.log_data_collector_payloads": True,
     "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-    app_name="Python Agent Test (framework_ariadne)",
+    app_name="Python Agent Test (framework_strawberry)",
     default_settings=_default_settings,
 )
-
-
-if six.PY2:
-    collect_ignore = ["test_application_async.py"]
```

### Comparing `newrelic-9.8.0/tests/framework_ariadne/schema.graphql` & `newrelic-9.9.0/tests/framework_ariadne/schema.graphql`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_ariadne/test_application.py` & `newrelic-9.9.0/tests/framework_ariadne/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_bottle/_target_application.py` & `newrelic-9.9.0/tests/framework_bottle/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_bottle/conftest.py` & `newrelic-9.9.0/tests/framework_bottle/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_bottle/test_application.py` & `newrelic-9.9.0/tests/framework_bottle/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_cherrypy/conftest.py` & `newrelic-9.9.0/tests/framework_cherrypy/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_cherrypy/test_application.py` & `newrelic-9.9.0/tests/framework_cherrypy/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_cherrypy/test_dispatch.py` & `newrelic-9.9.0/tests/framework_cherrypy/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_cherrypy/test_resource.py` & `newrelic-9.9.0/tests/framework_cherrypy/test_resource.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_cherrypy/test_routes.py` & `newrelic-9.9.0/tests/framework_cherrypy/test_routes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/_target_application.py` & `newrelic-9.9.0/tests/framework_django/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/conftest.py` & `newrelic-9.9.0/tests/framework_django/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/dummy_app/__init__.py` & `newrelic-9.9.0/tests/framework_django/dummy_app/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/dummy_app/templatetags/__init__.py` & `newrelic-9.9.0/tests/framework_django/dummy_app/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/dummy_app/templatetags/custom_tags.py` & `newrelic-9.9.0/tests/framework_django/dummy_app/templatetags/custom_tags.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/middleware.py` & `newrelic-9.9.0/tests/framework_django/middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/settings.py` & `newrelic-9.9.0/tests/framework_django/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/templates/main.html` & `newrelic-9.9.0/tests/framework_django/templates/main.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/templates/render_exception.html` & `newrelic-9.9.0/tests/framework_django/templates/render_exception.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/templates/results.html` & `newrelic-9.9.0/tests/framework_django/templates/results.html`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/test_application.py` & `newrelic-9.9.0/tests/framework_django/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/test_asgi_application.py` & `newrelic-9.9.0/tests/framework_django/test_asgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/urls.py` & `newrelic-9.9.0/tests/framework_django/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/views.py` & `newrelic-9.9.0/tests/framework_django/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_django/wsgi.py` & `newrelic-9.9.0/tests/framework_django/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_falcon/_target_application.py` & `newrelic-9.9.0/tests/framework_falcon/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_falcon/conftest.py` & `newrelic-9.9.0/tests/framework_falcon/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_falcon/test_application.py` & `newrelic-9.9.0/tests/framework_falcon/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_fastapi/_target_application.py` & `newrelic-9.9.0/tests/framework_fastapi/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_fastapi/conftest.py` & `newrelic-9.9.0/tests/framework_fastapi/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_fastapi/test_application.py` & `newrelic-9.9.0/tests/framework_fastapi/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/_test_application.py` & `newrelic-9.9.0/tests/framework_flask/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/_test_application_async.py` & `newrelic-9.9.0/tests/framework_flask/_test_not_found.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import pytest
 import webtest
-from _test_application import application
 
-from conftest import async_handler_support
+from flask import Flask
 
-# Async handlers only supported in Flask >2.0.0
-if async_handler_support:
-    @application.route('/async')
-    async def async_page():
-        return 'ASYNC RESPONSE'
+application = Flask(__name__)
+
+@application.errorhandler(404)
+def page_not_found(error):
+    return 'This page does not exist', 404
 
 _test_application = webtest.TestApp(application)
```

### Comparing `newrelic-9.8.0/tests/framework_flask/_test_blueprints.py` & `newrelic-9.9.0/tests/framework_flask/_test_blueprints.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/_test_compress.py` & `newrelic-9.9.0/tests/framework_flask/_test_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/_test_middleware.py` & `newrelic-9.9.0/tests/framework_flask/_test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/_test_not_found.py` & `newrelic-9.9.0/tests/framework_graphene/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,20 +7,7 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-import pytest
-import webtest
-
-from flask import Flask
-
-application = Flask(__name__)
-
-@application.errorhandler(404)
-def page_not_found(error):
-    return 'This page does not exist', 404
-
-_test_application = webtest.TestApp(application)
```

### Comparing `newrelic-9.8.0/tests/framework_flask/_test_user_exceptions.py` & `newrelic-9.9.0/tests/framework_flask/_test_user_exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/_test_views.py` & `newrelic-9.9.0/tests/framework_flask/_test_views.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/_test_views_async.py` & `newrelic-9.9.0/tests/framework_flask/_test_views_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/conftest.py` & `newrelic-9.9.0/tests/framework_flask/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/test_application.py` & `newrelic-9.9.0/tests/framework_flask/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/test_blueprints.py` & `newrelic-9.9.0/tests/framework_flask/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/test_compress.py` & `newrelic-9.9.0/tests/framework_flask/test_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/test_middleware.py` & `newrelic-9.9.0/tests/framework_flask/test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/test_not_found.py` & `newrelic-9.9.0/tests/framework_flask/test_not_found.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/test_user_exceptions.py` & `newrelic-9.9.0/tests/framework_flask/test_user_exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_flask/test_views.py` & `newrelic-9.9.0/tests/framework_flask/test_views.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphene/__init__.py` & `newrelic-9.9.0/tests/framework_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphene/_target_application.py` & `newrelic-9.9.0/tests/framework_graphene/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphene/_target_schema_async.py` & `newrelic-9.9.0/tests/framework_graphene/_target_schema_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphene/_target_schema_sync.py` & `newrelic-9.9.0/tests/framework_graphene/_target_schema_sync.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphene/conftest.py` & `newrelic-9.9.0/tests/framework_graphql/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,34 +9,42 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
-import six
-from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
+from testing_support.fixtures import (  # noqa: F401; pylint: disable=W0611
+    collector_agent_registration_fixture,
+    collector_available_fixture,
+)
 
+from newrelic.packages import six
 
 _default_settings = {
     "transaction_tracer.explain_threshold": 0.0,
     "transaction_tracer.transaction_threshold": 0.0,
     "transaction_tracer.stack_trace_threshold": 0.0,
     "debug.log_data_collector_payloads": True,
     "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-    app_name="Python Agent Test (framework_graphene)",
+    app_name="Python Agent Test (framework_graphql)",
     default_settings=_default_settings,
 )
 
 
-@pytest.fixture(scope="session")
-def app():
-    from _target_application import _target_application
+@pytest.fixture(scope="session", params=["sync-sync", "async-sync", "async-async"])
+def target_application(request):
+    from ._target_application import target_application
+
+    app = target_application.get(request.param, None)
+    if app is None:
+        pytest.skip("Unsupported combination.")
+        return
 
-    return _target_application
+    return "GraphQL", None, app, True, request.param.split("-")[1], 0
 
 
 if six.PY2:
     collect_ignore = ["test_application_async.py"]
```

### Comparing `newrelic-9.8.0/tests/framework_graphene/test_application.py` & `newrelic-9.9.0/tests/framework_graphene/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphql/__init__.py` & `newrelic-9.9.0/tests/framework_strawberry/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphql/_target_application.py` & `newrelic-9.9.0/tests/framework_graphql/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphql/_target_schema_async.py` & `newrelic-9.9.0/tests/framework_graphql/_target_schema_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphql/_target_schema_sync.py` & `newrelic-9.9.0/tests/framework_graphql/_target_schema_sync.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphql/conftest.py` & `newrelic-9.9.0/tests/framework_graphene/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,26 +25,21 @@
     "transaction_tracer.transaction_threshold": 0.0,
     "transaction_tracer.stack_trace_threshold": 0.0,
     "debug.log_data_collector_payloads": True,
     "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-    app_name="Python Agent Test (framework_graphql)",
+    app_name="Python Agent Test (framework_graphene)",
     default_settings=_default_settings,
 )
 
 
-@pytest.fixture(scope="session", params=["sync-sync", "async-sync", "async-async"])
-def target_application(request):
-    from ._target_application import target_application
-
-    app = target_application.get(request.param, None)
-    if app is None:
-        pytest.skip("Unsupported combination.")
-        return
+@pytest.fixture(scope="session")
+def app():
+    from _target_application import _target_application
 
-    return "GraphQL", None, app, True, request.param.split("-")[1], 0
+    return _target_application
 
 
 if six.PY2:
     collect_ignore = ["test_application_async.py"]
```

### Comparing `newrelic-9.8.0/tests/framework_graphql/test_application.py` & `newrelic-9.9.0/tests/framework_graphql/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_graphql/test_application_async.py` & `newrelic-9.9.0/tests/framework_graphql/test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_grpc/_test_common.py` & `newrelic-9.9.0/tests/framework_grpc/_test_common.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_grpc/conftest.py` & `newrelic-9.9.0/tests/framework_grpc/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_grpc/sample_application/__init__.py` & `newrelic-9.9.0/tests/framework_grpc/sample_application/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_grpc/sample_application/sample_application.proto` & `newrelic-9.9.0/tests/framework_grpc/sample_application/sample_application.proto`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_grpc/test_clients.py` & `newrelic-9.9.0/tests/framework_grpc/test_clients.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,112 +10,109 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import grpc
 import pytest
-import six
-
-from newrelic.api.background_task import background_task
-
-from testing_support.validators.validate_transaction_errors import validate_transaction_errors
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
-
 from _test_common import create_request, get_result
+from testing_support.validators.validate_transaction_errors import (
+    validate_transaction_errors,
+)
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
 
+from newrelic.api.background_task import background_task
+from newrelic.packages import six
 
 _test_matrix = [
-    ('service_method_type,service_method_method_name,raises_exception,'
-    'message_count,cancel'), (
-        ('unary_unary', '__call__', False, 1, False),
-        ('unary_unary', '__call__', True, 1, False),
-        ('unary_unary', 'with_call', False, 1, False),
-        ('unary_unary', 'with_call', True, 1, False),
-        ('unary_unary', 'future', False, 1, False),
-        ('unary_unary', 'future', True, 1, False),
-        ('unary_unary', 'future', False, 1, True),
-
-        ('stream_unary', '__call__', False, 1, False),
-        ('stream_unary', '__call__', True, 1, False),
-        ('stream_unary', 'with_call', False, 1, False),
-        ('stream_unary', 'with_call', True, 1, False),
-        ('stream_unary', 'future', False, 1, False),
-        ('stream_unary', 'future', True, 1, False),
-        ('stream_unary', 'future', False, 1, True),
-
-        ('unary_stream', '__call__', False, 1, False),
-        ('unary_stream', '__call__', True, 1, False),
-        ('unary_stream', '__call__', False, 2, False),
-        ('unary_stream', '__call__', True, 2, False),
-        ('unary_stream', '__call__', False, 1, True),
-        ('unary_stream', '__call__', False, 2, True),
-
-        ('stream_stream', '__call__', False, 1, False),
-        ('stream_stream', '__call__', True, 1, False),
-        ('stream_stream', '__call__', False, 2, False),
-        ('stream_stream', '__call__', True, 2, False),
-        ('stream_stream', '__call__', False, 1, True),
-        ('stream_stream', '__call__', False, 2, True),
-)]
+    ("service_method_type,service_method_method_name,raises_exception," "message_count,cancel"),
+    (
+        ("unary_unary", "__call__", False, 1, False),
+        ("unary_unary", "__call__", True, 1, False),
+        ("unary_unary", "with_call", False, 1, False),
+        ("unary_unary", "with_call", True, 1, False),
+        ("unary_unary", "future", False, 1, False),
+        ("unary_unary", "future", True, 1, False),
+        ("unary_unary", "future", False, 1, True),
+        ("stream_unary", "__call__", False, 1, False),
+        ("stream_unary", "__call__", True, 1, False),
+        ("stream_unary", "with_call", False, 1, False),
+        ("stream_unary", "with_call", True, 1, False),
+        ("stream_unary", "future", False, 1, False),
+        ("stream_unary", "future", True, 1, False),
+        ("stream_unary", "future", False, 1, True),
+        ("unary_stream", "__call__", False, 1, False),
+        ("unary_stream", "__call__", True, 1, False),
+        ("unary_stream", "__call__", False, 2, False),
+        ("unary_stream", "__call__", True, 2, False),
+        ("unary_stream", "__call__", False, 1, True),
+        ("unary_stream", "__call__", False, 2, True),
+        ("stream_stream", "__call__", False, 1, False),
+        ("stream_stream", "__call__", True, 1, False),
+        ("stream_stream", "__call__", False, 2, False),
+        ("stream_stream", "__call__", True, 2, False),
+        ("stream_stream", "__call__", False, 1, True),
+        ("stream_stream", "__call__", False, 2, True),
+    ),
+]
 
 
 @pytest.mark.parametrize(*_test_matrix)
-def test_client(service_method_type, service_method_method_name,
-        raises_exception, message_count, cancel, mock_grpc_server, stub):
-
+def test_client(
+    service_method_type, service_method_method_name, raises_exception, message_count, cancel, mock_grpc_server, stub
+):
     port = mock_grpc_server
 
-    service_method_class_name = 'NoTxn%s%s' % (
-            service_method_type.title().replace('_', ''),
-            'Raises' if raises_exception else '')
-    streaming_request = service_method_type.split('_')[0] == 'stream'
-    streaming_response = service_method_type.split('_')[1] == 'stream'
+    service_method_class_name = "NoTxn%s%s" % (
+        service_method_type.title().replace("_", ""),
+        "Raises" if raises_exception else "",
+    )
+    streaming_request = service_method_type.split("_")[0] == "stream"
+    streaming_response = service_method_type.split("_")[1] == "stream"
 
     _test_scoped_metrics = [
-            ('External/localhost:%s/gRPC/SampleApplication/%s' % (port,
-                service_method_class_name), 1),
+        ("External/localhost:%s/gRPC/SampleApplication/%s" % (port, service_method_class_name), 1),
     ]
     _test_rollup_metrics = [
-            ('External/localhost:%s/gRPC/SampleApplication/%s' % (port,
-                service_method_class_name), 1),
-            ('External/localhost:%s/all' % port, 1),
-            ('External/allOther', 1),
-            ('External/all', 1),
+        ("External/localhost:%s/gRPC/SampleApplication/%s" % (port, service_method_class_name), 1),
+        ("External/localhost:%s/all" % port, 1),
+        ("External/allOther", 1),
+        ("External/all", 1),
     ]
 
     if six.PY2:
-        _test_transaction_name = 'test_clients:_test_client'
+        _test_transaction_name = "test_clients:_test_client"
     else:
-        _test_transaction_name = (
-                'test_clients:test_client.<locals>._test_client')
+        _test_transaction_name = "test_clients:test_client.<locals>._test_client"
 
     _errors = []
     if not streaming_response and cancel:
-        _errors.append('grpc:FutureCancelledError')
+        _errors.append("grpc:FutureCancelledError")
     elif raises_exception or cancel:
-        _errors.append('grpc._channel:_Rendezvous')
+        _errors.append("grpc._channel:_Rendezvous")
 
     @validate_transaction_errors(errors=_errors)
-    @validate_transaction_metrics(_test_transaction_name,
-            scoped_metrics=_test_scoped_metrics,
-            rollup_metrics=_test_rollup_metrics,
-            background_task=True)
+    @validate_transaction_metrics(
+        _test_transaction_name,
+        scoped_metrics=_test_scoped_metrics,
+        rollup_metrics=_test_rollup_metrics,
+        background_task=True,
+    )
     @background_task()
     def _test_client():
         service_method_class = getattr(stub, service_method_class_name)
-        service_method_method = getattr(service_method_class,
-                service_method_method_name)
+        service_method_method = getattr(service_method_class, service_method_method_name)
 
         # In the case that we're preparing to cancel a request it's important
         # that the request does not return prior to cancelling. If the request
         # returns prior to cancellation then the response might be valid. In
         # order to force the request to not return, the timesout option is set.
-        request = create_request(streaming_request, count=message_count,
-                timesout=cancel)
+        request = create_request(streaming_request, count=message_count, timesout=cancel)
 
         reply = service_method_method(request, None, None, None)
 
         if isinstance(reply, tuple):
             reply = reply[0]
 
         if cancel:
@@ -127,202 +124,188 @@
             if streaming_response:
                 reply = list(reply)
             else:
                 reply = [reply.result()]
         except (AttributeError, TypeError):
             reply = [reply]
 
-        expected_text = '%s: Hello World' % service_method_type
+        expected_text = "%s: Hello World" % service_method_type
         response_texts_correct = [r.text == expected_text for r in reply]
         assert len(response_texts_correct) == message_count
         assert response_texts_correct and all(response_texts_correct)
 
     try:
         _test_client()
     except grpc.RpcError as e:
         if raises_exception:
-            assert '%s: Hello World' % service_method_type in e.details()
+            assert "%s: Hello World" % service_method_type in e.details()
         elif cancel:
             assert e.code() == grpc.StatusCode.CANCELLED
         else:
             raise
     except grpc.FutureCancelledError:
         assert cancel
 
 
 _test_matrix = [
-    ('service_method_type,service_method_method_name,future_response'), (
-        ('unary_unary', '__call__', False),
-        ('unary_unary', 'with_call', False),
-        ('unary_unary', 'future', True),
-
-        ('stream_unary', '__call__', False),
-        ('stream_unary', 'with_call', False),
-        ('stream_unary', 'future', True),
-
-        ('unary_stream', '__call__', True),
-
-        ('stream_stream', '__call__', True),
-)]
+    ("service_method_type,service_method_method_name,future_response"),
+    (
+        ("unary_unary", "__call__", False),
+        ("unary_unary", "with_call", False),
+        ("unary_unary", "future", True),
+        ("stream_unary", "__call__", False),
+        ("stream_unary", "with_call", False),
+        ("stream_unary", "future", True),
+        ("unary_stream", "__call__", True),
+        ("stream_stream", "__call__", True),
+    ),
+]
 
 
 @pytest.mark.parametrize(*_test_matrix)
-def test_future_timeout_error(service_method_type, service_method_method_name,
-        future_response, mock_grpc_server, stub):
+def test_future_timeout_error(service_method_type, service_method_method_name, future_response, mock_grpc_server, stub):
     port = mock_grpc_server
 
-    service_method_class_name = 'NoTxn%s' % (
-            service_method_type.title().replace('_', ''))
-    streaming_request = service_method_type.split('_')[0] == 'stream'
+    service_method_class_name = "NoTxn%s" % (service_method_type.title().replace("_", ""))
+    streaming_request = service_method_type.split("_")[0] == "stream"
 
     _test_scoped_metrics = [
-            ('External/localhost:%s/gRPC/SampleApplication/%s' % (port,
-                service_method_class_name), 1),
+        ("External/localhost:%s/gRPC/SampleApplication/%s" % (port, service_method_class_name), 1),
     ]
     _test_rollup_metrics = [
-            ('External/localhost:%s/gRPC/SampleApplication/%s' % (port,
-                service_method_class_name), 1),
-            ('External/localhost:%s/all' % port, 1),
-            ('External/allOther', 1),
-            ('External/all', 1),
+        ("External/localhost:%s/gRPC/SampleApplication/%s" % (port, service_method_class_name), 1),
+        ("External/localhost:%s/all" % port, 1),
+        ("External/allOther", 1),
+        ("External/all", 1),
     ]
 
     if six.PY2:
-        _test_transaction_name = 'test_clients:_test_future_timeout_error'
+        _test_transaction_name = "test_clients:_test_future_timeout_error"
     else:
-        _test_transaction_name = (
-                'test_clients:test_future_timeout_error.<locals>.'
-                '_test_future_timeout_error')
+        _test_transaction_name = "test_clients:test_future_timeout_error.<locals>." "_test_future_timeout_error"
 
     @validate_transaction_errors(errors=[])
-    @validate_transaction_metrics(_test_transaction_name,
-            scoped_metrics=_test_scoped_metrics,
-            rollup_metrics=_test_rollup_metrics,
-            background_task=True)
+    @validate_transaction_metrics(
+        _test_transaction_name,
+        scoped_metrics=_test_scoped_metrics,
+        rollup_metrics=_test_rollup_metrics,
+        background_task=True,
+    )
     @background_task()
     def _test_future_timeout_error():
         service_method_class = getattr(stub, service_method_class_name)
-        service_method_method = getattr(service_method_class,
-                service_method_method_name)
+        service_method_method = getattr(service_method_class, service_method_method_name)
 
         request = create_request(streaming_request, count=1, timesout=True)
 
         reply = get_result(service_method_method, request, timeout=0.01)
         assert reply and reply.code() == grpc.StatusCode.DEADLINE_EXCEEDED
 
     _test_future_timeout_error()
 
 
 _test_matrix = [
-    ('service_method_type,service_method_method_name'), (
-        ('unary_unary', 'with_call'),
-        ('unary_unary', 'future'),
-
-        ('stream_unary', 'with_call'),
-        ('stream_unary', 'future'),
-
-)]
+    ("service_method_type,service_method_method_name"),
+    (
+        ("unary_unary", "with_call"),
+        ("unary_unary", "future"),
+        ("stream_unary", "with_call"),
+        ("stream_unary", "future"),
+    ),
+]
 
 
 @pytest.mark.parametrize(*_test_matrix)
-def test_repeated_result(service_method_type, service_method_method_name,
-        mock_grpc_server, stub):
+def test_repeated_result(service_method_type, service_method_method_name, mock_grpc_server, stub):
     port = mock_grpc_server
 
-    service_method_class_name = 'NoTxn%s' % (
-            service_method_type.title().replace('_', ''))
-    streaming_request = service_method_type.split('_')[0] == 'stream'
+    service_method_class_name = "NoTxn%s" % (service_method_type.title().replace("_", ""))
+    streaming_request = service_method_type.split("_")[0] == "stream"
 
     _test_scoped_metrics = [
-            ('External/localhost:%s/gRPC/SampleApplication/%s' % (port,
-                service_method_class_name), 1),
+        ("External/localhost:%s/gRPC/SampleApplication/%s" % (port, service_method_class_name), 1),
     ]
     _test_rollup_metrics = [
-            ('External/localhost:%s/gRPC/SampleApplication/%s' % (port,
-                service_method_class_name), 1),
-            ('External/localhost:%s/all' % port, 1),
-            ('External/allOther', 1),
-            ('External/all', 1),
+        ("External/localhost:%s/gRPC/SampleApplication/%s" % (port, service_method_class_name), 1),
+        ("External/localhost:%s/all" % port, 1),
+        ("External/allOther", 1),
+        ("External/all", 1),
     ]
 
     if six.PY2:
-        _test_transaction_name = 'test_clients:_test_repeated_result'
+        _test_transaction_name = "test_clients:_test_repeated_result"
     else:
-        _test_transaction_name = (
-                'test_clients:'
-                'test_repeated_result.<locals>._test_repeated_result')
+        _test_transaction_name = "test_clients:" "test_repeated_result.<locals>._test_repeated_result"
 
     @validate_transaction_errors(errors=[])
-    @validate_transaction_metrics(_test_transaction_name,
-            scoped_metrics=_test_scoped_metrics,
-            rollup_metrics=_test_rollup_metrics,
-            background_task=True)
+    @validate_transaction_metrics(
+        _test_transaction_name,
+        scoped_metrics=_test_scoped_metrics,
+        rollup_metrics=_test_rollup_metrics,
+        background_task=True,
+    )
     @background_task()
     def _test_repeated_result():
         service_method_class = getattr(stub, service_method_class_name)
-        service_method_method = getattr(service_method_class,
-                service_method_method_name)
+        service_method_method = getattr(service_method_class, service_method_method_name)
 
         request = create_request(streaming_request, count=1, timesout=False)
 
         reply = service_method_method(request)
         if isinstance(reply, tuple):
             reply = reply[1]
 
         reply.result()
         reply.result()
 
     _test_repeated_result()
 
 
 _test_matrix = [
-    ('service_method_type,service_method_method_name,future_response'), (
-        ('unary_stream', '__call__', True),
-        ('stream_stream', '__call__', True),
-)]
+    ("service_method_type,service_method_method_name,future_response"),
+    (
+        ("unary_stream", "__call__", True),
+        ("stream_stream", "__call__", True),
+    ),
+]
 
 
 @pytest.mark.parametrize(*_test_matrix)
-def test_future_cancel(service_method_type, service_method_method_name,
-        future_response, mock_grpc_server, stub):
+def test_future_cancel(service_method_type, service_method_method_name, future_response, mock_grpc_server, stub):
     port = mock_grpc_server
 
-    service_method_class_name = 'NoTxn%s' % (
-            service_method_type.title().replace('_', ''))
-    streaming_request = service_method_type.split('_')[0] == 'stream'
+    service_method_class_name = "NoTxn%s" % (service_method_type.title().replace("_", ""))
+    streaming_request = service_method_type.split("_")[0] == "stream"
 
     _test_scoped_metrics = [
-            ('External/localhost:%s/gRPC/SampleApplication/%s' % (port,
-                service_method_class_name), 1),
+        ("External/localhost:%s/gRPC/SampleApplication/%s" % (port, service_method_class_name), 1),
     ]
     _test_rollup_metrics = [
-            ('External/localhost:%s/gRPC/SampleApplication/%s' % (port,
-                service_method_class_name), 1),
-            ('External/localhost:%s/all' % port, 1),
-            ('External/allOther', 1),
-            ('External/all', 1),
+        ("External/localhost:%s/gRPC/SampleApplication/%s" % (port, service_method_class_name), 1),
+        ("External/localhost:%s/all" % port, 1),
+        ("External/allOther", 1),
+        ("External/all", 1),
     ]
 
     if six.PY2:
-        _test_transaction_name = 'test_clients:_test_future_cancel'
+        _test_transaction_name = "test_clients:_test_future_cancel"
     else:
-        _test_transaction_name = (
-                'test_clients:test_future_cancel.<locals>.'
-                '_test_future_cancel')
+        _test_transaction_name = "test_clients:test_future_cancel.<locals>." "_test_future_cancel"
 
     @validate_transaction_errors(errors=[])
-    @validate_transaction_metrics(_test_transaction_name,
-            scoped_metrics=_test_scoped_metrics,
-            rollup_metrics=_test_rollup_metrics,
-            background_task=True)
+    @validate_transaction_metrics(
+        _test_transaction_name,
+        scoped_metrics=_test_scoped_metrics,
+        rollup_metrics=_test_rollup_metrics,
+        background_task=True,
+    )
     @background_task()
     def _test_future_cancel():
         service_method_class = getattr(stub, service_method_class_name)
-        service_method_method = getattr(service_method_class,
-                service_method_method_name)
+        service_method_method = getattr(service_method_class, service_method_method_name)
 
         request = create_request(streaming_request, count=3, timesout=False)
 
         reply = service_method_method(request)
         for result in reply:
             reply.cancel()
             break
```

### Comparing `newrelic-9.8.0/tests/framework_grpc/test_distributed_tracing.py` & `newrelic-9.9.0/tests/framework_grpc/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_grpc/test_get_url.py` & `newrelic-9.9.0/tests/framework_grpc/test_get_url.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_grpc/test_server.py` & `newrelic-9.9.0/tests/framework_grpc/test_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,177 +8,175 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import six
 import grpc
 import pytest
-from conftest import create_stub_and_channel
 from _test_common import create_request, wait_for_transaction_completion
-from newrelic.core.config import global_settings
+from conftest import create_stub_and_channel
 from testing_support.fixtures import (
-        override_application_settings,
-        override_generic_settings, function_not_called)
-from testing_support.validators.validate_code_level_metrics import validate_code_level_metrics
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
-from testing_support.validators.validate_transaction_errors import validate_transaction_errors
-from testing_support.validators.validate_transaction_event_attributes import validate_transaction_event_attributes
+    function_not_called,
+    override_application_settings,
+    override_generic_settings,
+)
+from testing_support.validators.validate_code_level_metrics import (
+    validate_code_level_metrics,
+)
+from testing_support.validators.validate_transaction_errors import (
+    validate_transaction_errors,
+)
+from testing_support.validators.validate_transaction_event_attributes import (
+    validate_transaction_event_attributes,
+)
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
+
+from newrelic.core.config import global_settings
+from newrelic.packages import six
+
 
 def select_python_version(py2, py3):
     return six.PY3 and py3 or py2
 
 
-if hasattr(grpc, '__version__'):
-    GRPC_VERSION = tuple(int(v) for v in grpc.__version__.split('.'))
+if hasattr(grpc, "__version__"):
+    GRPC_VERSION = tuple(int(v) for v in grpc.__version__.split("."))
 else:
     GRPC_VERSION = None
 
-_test_matrix = ["method_name,streaming_request", [
-    ("DoUnaryUnary", False),
-    ("DoUnaryStream", False),
-    ("DoStreamUnary", True),
-    ("DoStreamStream", True)
-]]
+_test_matrix = [
+    "method_name,streaming_request",
+    [("DoUnaryUnary", False), ("DoUnaryStream", False), ("DoStreamUnary", True), ("DoStreamStream", True)],
+]
 
 
 @pytest.mark.parametrize(*_test_matrix)
 def test_simple(method_name, streaming_request, mock_grpc_server, stub):
     port = mock_grpc_server
     request = create_request(streaming_request)
-    _transaction_name = \
-        "sample_application:SampleApplicationServicer.{}".format(method_name)
+    _transaction_name = "sample_application:SampleApplicationServicer.{}".format(method_name)
     method = getattr(stub, method_name)
 
     @validate_code_level_metrics("sample_application.SampleApplicationServicer", method_name)
     @validate_transaction_metrics(_transaction_name)
-    @override_application_settings({'attributes.include': ['request.*']})
+    @override_application_settings({"attributes.include": ["request.*"]})
     @validate_transaction_event_attributes(
-            required_params={
-                'agent': ['request.uri', 'request.headers.userAgent',
-                    'response.status', 'response.headers.contentType'],
-                'user': [],
-                'intrinsic': ['port'],
-            },
-            exact_attrs={
-                'agent': {},
-                'user': {},
-                'intrinsic': {'port': port}
-            })
+        required_params={
+            "agent": ["request.uri", "request.headers.userAgent", "response.status", "response.headers.contentType"],
+            "user": [],
+            "intrinsic": ["port"],
+        },
+        exact_attrs={"agent": {}, "user": {}, "intrinsic": {"port": port}},
+    )
     @wait_for_transaction_completion
     def _doit():
         response = method(request)
 
         try:
             list(response)
         except Exception:
             pass
 
     _doit()
 
 
 @pytest.mark.parametrize(*_test_matrix)
-def test_raises_response_status(method_name, streaming_request,
-        mock_grpc_server, stub):
+def test_raises_response_status(method_name, streaming_request, mock_grpc_server, stub):
     port = mock_grpc_server
     request = create_request(streaming_request)
 
-    method_name = method_name + 'Raises'
+    method_name = method_name + "Raises"
 
-    _transaction_name = \
-        "sample_application:SampleApplicationServicer.{}".format(method_name)
+    _transaction_name = "sample_application:SampleApplicationServicer.{}".format(method_name)
     method = getattr(stub, method_name)
 
     status_code = str(grpc.StatusCode.UNKNOWN.value[0])
 
     @validate_code_level_metrics("sample_application.SampleApplicationServicer", method_name)
-    @validate_transaction_errors(errors=[select_python_version(
-        py2='exceptions:AssertionError', py3='builtins:AssertionError')])
+    @validate_transaction_errors(
+        errors=[select_python_version(py2="exceptions:AssertionError", py3="builtins:AssertionError")]
+    )
     @validate_transaction_metrics(_transaction_name)
-    @override_application_settings({'attributes.include': ['request.*']})
+    @override_application_settings({"attributes.include": ["request.*"]})
     @validate_transaction_event_attributes(
-            required_params={
-                'agent': ['request.uri', 'request.headers.userAgent',
-                    'response.status'],
-                'user': [],
-                'intrinsic': ['port'],
-            },
-            exact_attrs={
-                'agent': {'response.status': status_code},
-                'user': {},
-                'intrinsic': {'port': port}
-            })
+        required_params={
+            "agent": ["request.uri", "request.headers.userAgent", "response.status"],
+            "user": [],
+            "intrinsic": ["port"],
+        },
+        exact_attrs={"agent": {"response.status": status_code}, "user": {}, "intrinsic": {"port": port}},
+    )
     @wait_for_transaction_completion
     def _doit():
         try:
             response = method(request)
             list(response)
         except Exception:
             pass
 
     _doit()
 
 
 @pytest.mark.parametrize(*_test_matrix)
 def test_abort(method_name, streaming_request, mock_grpc_server, stub):
-    method_name += 'Abort'
+    method_name += "Abort"
     port = mock_grpc_server
     request = create_request(streaming_request)
     method = getattr(stub, method_name)
 
     @validate_code_level_metrics("sample_application.SampleApplicationServicer", method_name)
-    @validate_transaction_errors(errors=[select_python_version(
-        py2='exceptions:Exception', py3='builtins:Exception')])
+    @validate_transaction_errors(errors=[select_python_version(py2="exceptions:Exception", py3="builtins:Exception")])
     @wait_for_transaction_completion
     def _doit():
         with pytest.raises(grpc.RpcError) as error:
             response = method(request)
             list(response)
 
-        assert error.value.details() == 'aborting'
+        assert error.value.details() == "aborting"
         assert error.value.code() == grpc.StatusCode.ABORTED
 
     _doit()
 
 
 @pytest.mark.parametrize(*_test_matrix)
 def test_abort_with_status(method_name, streaming_request, mock_grpc_server, stub):
-    method_name += 'AbortWithStatus'
+    method_name += "AbortWithStatus"
     port = mock_grpc_server
     request = create_request(streaming_request)
     method = getattr(stub, method_name)
 
     @validate_code_level_metrics("sample_application.SampleApplicationServicer", method_name)
-    @validate_transaction_errors(errors=[select_python_version(
-        py2='exceptions:Exception', py3='builtins:Exception')])
+    @validate_transaction_errors(errors=[select_python_version(py2="exceptions:Exception", py3="builtins:Exception")])
     @wait_for_transaction_completion
     def _doit():
         with pytest.raises(grpc.RpcError) as error:
             response = method(request)
             list(response)
 
-        assert error.value.details() == 'abort_with_status'
+        assert error.value.details() == "abort_with_status"
         assert error.value.code() == grpc.StatusCode.ABORTED
 
     _doit()
 
 
 def test_no_exception_client_close(mock_grpc_server):
     port = mock_grpc_server
-    # We can't use the stub_and_channel fixture here as closing 
+    # We can't use the stub_and_channel fixture here as closing
     # that channel will cause any subsequent tests to fail.
     # Instead we create a brand new channel to close.
     stub, channel = create_stub_and_channel(port)
 
     with channel:
         request = create_request(False, timesout=True)
 
-        method = getattr(stub, 'DoUnaryUnary')
+        method = getattr(stub, "DoUnaryUnary")
 
         @validate_transaction_errors(errors=[])
         @wait_for_transaction_completion
         def _doit():
             future_response = method.future(request)
             channel.close()
             with pytest.raises(grpc.RpcError) as error:
@@ -189,17 +187,16 @@
         _doit()
 
 
 def test_newrelic_disabled_no_transaction(mock_grpc_server, stub):
     port = mock_grpc_server
     request = create_request(False)
 
-    method = getattr(stub, 'DoUnaryUnary')
+    method = getattr(stub, "DoUnaryUnary")
 
-    @override_generic_settings(global_settings(), {'enabled': False})
-    @function_not_called('newrelic.core.stats_engine',
-        'StatsEngine.record_transaction')
+    @override_generic_settings(global_settings(), {"enabled": False})
+    @function_not_called("newrelic.core.stats_engine", "StatsEngine.record_transaction")
     @wait_for_transaction_completion
     def _doit():
         method(request)
 
     _doit()
```

### Comparing `newrelic-9.8.0/tests/framework_pyramid/_test_append_slash_app.py` & `newrelic-9.9.0/tests/framework_pyramid/_test_append_slash_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_pyramid/_test_application.py` & `newrelic-9.9.0/tests/framework_pyramid/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_pyramid/conftest.py` & `newrelic-9.9.0/tests/framework_pyramid/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_pyramid/test_append_slash_app.py` & `newrelic-9.9.0/tests/framework_pyramid/test_append_slash_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_pyramid/test_application.py` & `newrelic-9.9.0/tests/framework_pyramid/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_pyramid/test_cornice.py` & `newrelic-9.9.0/tests/framework_pyramid/test_cornice.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_sanic/_target_application.py` & `newrelic-9.9.0/tests/framework_sanic/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_sanic/conftest.py` & `newrelic-9.9.0/tests/framework_sanic/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_sanic/test_application.py` & `newrelic-9.9.0/tests/framework_sanic/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_sanic/test_cross_application.py` & `newrelic-9.9.0/tests/framework_sanic/test_cross_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_starlette/_test_application.py` & `newrelic-9.9.0/tests/framework_starlette/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_starlette/_test_bg_tasks.py` & `newrelic-9.9.0/tests/framework_starlette/_test_bg_tasks.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_starlette/_test_graphql.py` & `newrelic-9.9.0/tests/framework_starlette/_test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_starlette/conftest.py` & `newrelic-9.9.0/tests/framework_starlette/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_starlette/test_application.py` & `newrelic-9.9.0/tests/framework_starlette/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_starlette/test_bg_tasks.py` & `newrelic-9.9.0/tests/framework_starlette/test_bg_tasks.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_strawberry/__init__.py` & `newrelic-9.9.0/tests/testing_support/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_strawberry/_target_application.py` & `newrelic-9.9.0/tests/framework_strawberry/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_strawberry/_target_schema_async.py` & `newrelic-9.9.0/tests/framework_strawberry/_target_schema_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_strawberry/_target_schema_sync.py` & `newrelic-9.9.0/tests/framework_strawberry/_target_schema_sync.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_strawberry/conftest.py` & `newrelic-9.9.0/tests/template_genshi/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,10 +22,9 @@
     "transaction_tracer.transaction_threshold": 0.0,
     "transaction_tracer.stack_trace_threshold": 0.0,
     "debug.log_data_collector_payloads": True,
     "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-    app_name="Python Agent Test (framework_strawberry)",
-    default_settings=_default_settings,
+    app_name="Python Agent Test (template_genshi)", default_settings=_default_settings
 )
```

### Comparing `newrelic-9.8.0/tests/framework_strawberry/test_application.py` & `newrelic-9.9.0/tests/framework_strawberry/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_tornado/_target_application.py` & `newrelic-9.9.0/tests/framework_tornado/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_tornado/conftest.py` & `newrelic-9.9.0/tests/framework_tornado/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_tornado/test_custom_handler.py` & `newrelic-9.9.0/tests/framework_tornado/test_custom_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_tornado/test_externals.py` & `newrelic-9.9.0/tests/framework_tornado/test_externals.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_tornado/test_inbound_cat.py` & `newrelic-9.9.0/tests/framework_tornado/test_inbound_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/framework_tornado/test_server.py` & `newrelic-9.9.0/tests/framework_tornado/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_logging/conftest.py` & `newrelic-9.9.0/tests/logger_logging/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_logging/test_attributes.py` & `newrelic-9.9.0/tests/logger_logging/test_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_logging/test_local_decorating.py` & `newrelic-9.9.0/tests/logger_logging/test_local_decorating.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_logging/test_log_forwarding.py` & `newrelic-9.9.0/tests/logger_logging/test_log_forwarding.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_logging/test_logging_handler.py` & `newrelic-9.9.0/tests/logger_logging/test_logging_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_logging/test_metrics.py` & `newrelic-9.9.0/tests/logger_logging/test_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_logging/test_settings.py` & `newrelic-9.9.0/tests/logger_logging/test_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_loguru/conftest.py` & `newrelic-9.9.0/tests/logger_loguru/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_loguru/test_attributes.py` & `newrelic-9.9.0/tests/logger_loguru/test_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_loguru/test_local_decorating.py` & `newrelic-9.9.0/tests/logger_loguru/test_local_decorating.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_loguru/test_log_forwarding.py` & `newrelic-9.9.0/tests/logger_loguru/test_log_forwarding.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_loguru/test_metrics.py` & `newrelic-9.9.0/tests/logger_loguru/test_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_loguru/test_settings.py` & `newrelic-9.9.0/tests/logger_loguru/test_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_structlog/conftest.py` & `newrelic-9.9.0/tests/logger_structlog/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_structlog/test_attributes.py` & `newrelic-9.9.0/tests/logger_structlog/test_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_structlog/test_local_decorating.py` & `newrelic-9.9.0/tests/logger_structlog/test_local_decorating.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_structlog/test_log_forwarding.py` & `newrelic-9.9.0/tests/logger_structlog/test_log_forwarding.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/logger_structlog/test_metrics.py` & `newrelic-9.9.0/tests/logger_structlog/test_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_confluentkafka/conftest.py` & `newrelic-9.9.0/tests/messagebroker_confluentkafka/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_confluentkafka/test_consumer.py` & `newrelic-9.9.0/tests/messagebroker_confluentkafka/test_consumer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_confluentkafka/test_producer.py` & `newrelic-9.9.0/tests/messagebroker_confluentkafka/test_producer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_confluentkafka/test_serialization.py` & `newrelic-9.9.0/tests/messagebroker_confluentkafka/test_serialization.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_kafkapython/conftest.py` & `newrelic-9.9.0/tests/messagebroker_kafkapython/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_kafkapython/test_consumer.py` & `newrelic-9.9.0/tests/messagebroker_kafkapython/test_consumer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_kafkapython/test_heartbeat.py` & `newrelic-9.9.0/tests/messagebroker_kafkapython/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_kafkapython/test_producer.py` & `newrelic-9.9.0/tests/messagebroker_kafkapython/test_producer.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_kafkapython/test_serialization.py` & `newrelic-9.9.0/tests/messagebroker_kafkapython/test_serialization.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/compat.py` & `newrelic-9.9.0/tests/messagebroker_pika/compat.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/conftest.py` & `newrelic-9.9.0/tests/messagebroker_pika/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/minversion.py` & `newrelic-9.9.0/tests/messagebroker_pika/minversion.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/test_cat.py` & `newrelic-9.9.0/tests/messagebroker_pika/test_cat.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # limitations under the License.
 
 import os
 import random
 import string
 
 import pika
-import six
 from compat import basic_consume
 from testing_support.db_settings import rabbitmq_settings
-from testing_support.fixtures import (
-    cat_enabled,
-    override_application_settings,
+from testing_support.fixtures import cat_enabled, override_application_settings
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
 )
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
+
 from newrelic.api.background_task import background_task
 from newrelic.api.transaction import current_transaction
+from newrelic.packages import six
 
 DB_SETTINGS = rabbitmq_settings()[0]
 
 ENCODING_KEY = "".join(random.choice(string.ascii_lowercase) for _ in range(40))
 _override_settings = {
     "cross_process_id": "1#1",
     "encoding_key": ENCODING_KEY,
```

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/test_distributed_tracing.py` & `newrelic-9.9.0/tests/messagebroker_pika/test_distributed_tracing.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,209 +8,209 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from compat import basic_consume
-import pika
-import six
 import os
 
+import pika
+from compat import basic_consume
+from testing_support.db_settings import rabbitmq_settings
+from testing_support.fixtures import override_application_settings
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
+
 from newrelic.api.background_task import background_task
-from newrelic.api.transaction import current_transaction
 from newrelic.api.function_trace import FunctionTrace
+from newrelic.api.transaction import current_transaction
 from newrelic.common.encoding_utils import DistributedTracePayload
-
-from testing_support.db_settings import rabbitmq_settings
-from testing_support.fixtures import override_application_settings
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
+from newrelic.packages import six
 
 DB_SETTINGS = rabbitmq_settings()[0]
 
 _override_settings = {
-    'primary_application_id': '12345',
-    'account_id': '33',
-    'trusted_account_key': '1',
-    'cross_application_tracer.enabled': True,
-    'distributed_tracing.enabled': True,
+    "primary_application_id": "12345",
+    "account_id": "33",
+    "trusted_account_key": "1",
+    "cross_application_tracer.enabled": True,
+    "distributed_tracing.enabled": True,
 }
 
 _test_distributed_tracing_basic_publish_metrics = [
-    ('Supportability/TraceContext/Create/Success', 1),
-    ('Supportability/DistributedTrace/CreatePayload/Success', 1),
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/Default', 1),
-    ('DurationByCaller/Unknown/Unknown/Unknown/Unknown/all', 1),
-    ('DurationByCaller/Unknown/Unknown/Unknown/Unknown/allOther', 1),
+    ("Supportability/TraceContext/Create/Success", 1),
+    ("Supportability/DistributedTrace/CreatePayload/Success", 1),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/Default", 1),
+    ("DurationByCaller/Unknown/Unknown/Unknown/Unknown/all", 1),
+    ("DurationByCaller/Unknown/Unknown/Unknown/Unknown/allOther", 1),
 ]
 
 
 @validate_transaction_metrics(
-        'test_distributed_tracing:do_basic_publish',
-        rollup_metrics=_test_distributed_tracing_basic_publish_metrics,
-        background_task=True)
+    "test_distributed_tracing:do_basic_publish",
+    rollup_metrics=_test_distributed_tracing_basic_publish_metrics,
+    background_task=True,
+)
 @background_task()
 def do_basic_publish(channel, QUEUE, properties=None):
     channel.basic_publish(
-        exchange='',
+        exchange="",
         routing_key=QUEUE,
-        body='Testing distributed_tracing 123',
+        body="Testing distributed_tracing 123",
         properties=properties,
     )
 
 
 _test_distributed_tracing_basic_consume_rollup_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/Default', None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/Default', None),
-    ('Supportability/DistributedTrace/AcceptPayload/Success', None),
-    ('Supportability/TraceContext/Accept/Success', 1),
-    ('DurationByCaller/App/33/12345/AMQP/all', 1),
-    ('TransportDuration/App/33/12345/AMQP/all', 1),
-    ('DurationByCaller/App/33/12345/AMQP/allOther', 1),
-    ('TransportDuration/App/33/12345/AMQP/allOther', 1)
-
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/Default", None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/Default", None),
+    ("Supportability/DistributedTrace/AcceptPayload/Success", None),
+    ("Supportability/TraceContext/Accept/Success", 1),
+    ("DurationByCaller/App/33/12345/AMQP/all", 1),
+    ("TransportDuration/App/33/12345/AMQP/all", 1),
+    ("DurationByCaller/App/33/12345/AMQP/allOther", 1),
+    ("TransportDuration/App/33/12345/AMQP/allOther", 1),
 ]
 
 if six.PY3:
-    _consume_txn_name = ('test_distributed_tracing:'
-            'test_basic_consume_distributed_tracing_headers.'
-            '<locals>.on_receive')
-else:
     _consume_txn_name = (
-        'test_distributed_tracing:on_receive')
+        "test_distributed_tracing:" "test_basic_consume_distributed_tracing_headers." "<locals>.on_receive"
+    )
+else:
+    _consume_txn_name = "test_distributed_tracing:on_receive"
 
 
 @validate_transaction_metrics(
-        _consume_txn_name,
-        rollup_metrics=_test_distributed_tracing_basic_consume_rollup_metrics,
-        background_task=True,
-        group='Message/RabbitMQ/Exchange/Default')
+    _consume_txn_name,
+    rollup_metrics=_test_distributed_tracing_basic_consume_rollup_metrics,
+    background_task=True,
+    group="Message/RabbitMQ/Exchange/Default",
+)
 def do_basic_consume(channel):
     channel.start_consuming()
 
 
 @override_application_settings(_override_settings)
 def test_basic_consume_distributed_tracing_headers():
     def on_receive(ch, method, properties, msg):
         headers = properties.headers
         assert headers
-        assert 'NewRelicID' not in headers
-        assert 'NewRelicTransaction' not in headers
-        assert msg == b'Testing distributed_tracing 123'
+        assert "NewRelicID" not in headers
+        assert "NewRelicTransaction" not in headers
+        assert msg == b"Testing distributed_tracing 123"
         txn = current_transaction()
 
         assert txn
         assert txn._distributed_trace_state
-        assert txn.parent_type == 'App'
+        assert txn.parent_type == "App"
         assert txn._trace_id.startswith(txn.parent_tx)
         assert txn.parent_span is not None
         assert txn.parent_account == txn.settings.account_id
-        assert txn.parent_transport_type == 'AMQP'
+        assert txn.parent_transport_type == "AMQP"
         assert txn._priority is not None
         assert txn._sampled is not None
 
         ch.stop_consuming()
 
-    with pika.BlockingConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host'])) as connection:
+    with pika.BlockingConnection(pika.ConnectionParameters(DB_SETTINGS["host"])) as connection:
         channel = connection.channel()
-        queue_name = 'TESTDT-%s' % os.getpid()
+        queue_name = "TESTDT-%s" % os.getpid()
         channel.queue_declare(queue_name, durable=False)
 
         properties = pika.BasicProperties()
-        properties.headers = {'Hello': 'World'}
+        properties.headers = {"Hello": "World"}
 
         try:
             basic_consume(channel, queue_name, on_receive, auto_ack=False)
             do_basic_publish(channel, queue_name, properties=properties)
             do_basic_consume(channel)
 
         finally:
             channel.queue_delete(queue_name)
 
 
 _test_distributed_tracing_basic_get_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/Default', None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/Default', 1),
-    ('DurationByCaller/Unknown/Unknown/Unknown/Unknown/all', 1),
-    ('DurationByCaller/Unknown/Unknown/Unknown/Unknown/allOther', 1)
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/Default", None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/Default", 1),
+    ("DurationByCaller/Unknown/Unknown/Unknown/Unknown/all", 1),
+    ("DurationByCaller/Unknown/Unknown/Unknown/Unknown/allOther", 1),
 ]
 
 
 @validate_transaction_metrics(
-        'test_distributed_tracing:do_basic_get',
-        rollup_metrics=_test_distributed_tracing_basic_get_metrics,
-        background_task=True)
+    "test_distributed_tracing:do_basic_get",
+    rollup_metrics=_test_distributed_tracing_basic_get_metrics,
+    background_task=True,
+)
 @background_task()
 def do_basic_get(channel, QUEUE):
     _, properties, msg = channel.basic_get(QUEUE)
     headers = properties.headers
 
     assert headers
-    assert 'NewRelicID' not in headers
-    assert 'NewRelicTransaction' not in headers
-    assert msg == b'Testing distributed_tracing 123'
+    assert "NewRelicID" not in headers
+    assert "NewRelicTransaction" not in headers
+    assert msg == b"Testing distributed_tracing 123"
 
     txn = current_transaction()
 
     assert txn.client_cross_process_id is None
     assert txn.client_account_id is None
     assert txn.client_application_id is None
 
 
 @override_application_settings(_override_settings)
 def test_basic_get_no_distributed_tracing_headers():
-    with pika.BlockingConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host'])) as connection:
+    with pika.BlockingConnection(pika.ConnectionParameters(DB_SETTINGS["host"])) as connection:
         channel = connection.channel()
-        queue_name = 'TESTDT-%s' % os.getpid()
+        queue_name = "TESTDT-%s" % os.getpid()
         channel.queue_declare(queue_name, durable=False)
 
         properties = pika.BasicProperties()
-        properties.headers = {'Hello': 'World'}
+        properties.headers = {"Hello": "World"}
 
         try:
             do_basic_publish(channel, queue_name, properties=properties)
             do_basic_get(channel, queue_name)
         finally:
             channel.queue_delete(queue_name)
 
 
 @override_application_settings(_override_settings)
 def test_distributed_tracing_sends_produce_id():
-    with pika.BlockingConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host'])) as connection:
+    with pika.BlockingConnection(pika.ConnectionParameters(DB_SETTINGS["host"])) as connection:
         channel = connection.channel()
-        queue_name = 'TESTDT-%s' % os.getpid()
+        queue_name = "TESTDT-%s" % os.getpid()
         channel.queue_declare(queue_name, durable=False)
 
         properties = pika.BasicProperties()
-        properties.headers = {'Hello': 'World'}
+        properties.headers = {"Hello": "World"}
 
         try:
+
             @background_task()
             def _publish():
-                with FunctionTrace('foo') as trace:
+                with FunctionTrace("foo") as trace:
                     channel.basic_publish(
-                        exchange='',
+                        exchange="",
                         routing_key=queue_name,
-                        body='Testing distributed_tracing 123',
+                        body="Testing distributed_tracing 123",
                         properties=properties,
                     )
 
                 return trace
 
             trace = _publish()
 
             raw_message = channel.basic_get(queue_name)
         finally:
             channel.queue_delete(queue_name)
 
         properties = raw_message[1]
-        payload = DistributedTracePayload.from_http_safe(
-                properties.headers["newrelic"])
+        payload = DistributedTracePayload.from_http_safe(properties.headers["newrelic"])
 
-        data = payload['d']
+        data = payload["d"]
 
         # The payload should NOT contain the function trace ID
-        assert data['id'] != trace.guid
+        assert data["id"] != trace.guid
```

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/test_memory_leak.py` & `newrelic-9.9.0/tests/messagebroker_pika/test_memory_leak.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/test_pika_async_connection_consume.py` & `newrelic-9.9.0/tests/messagebroker_pika/test_pika_async_connection_consume.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import functools
 
 import pika
 import pytest
-import six
 import tornado
 from compat import basic_consume
 from conftest import (
     BODY,
     CORRELATION_ID,
     EXCHANGE,
     EXCHANGE_2,
@@ -44,71 +43,79 @@
     validate_transaction_metrics,
 )
 from testing_support.validators.validate_tt_collector_json import (
     validate_tt_collector_json,
 )
 
 from newrelic.api.background_task import background_task
-
+from newrelic.packages import six
 
 DB_SETTINGS = rabbitmq_settings()[0]
 
 _message_broker_tt_params = {
-    'queue_name': QUEUE,
-    'routing_key': QUEUE,
-    'correlation_id': CORRELATION_ID,
-    'reply_to': REPLY_TO,
-    'headers': HEADERS.copy(),
+    "queue_name": QUEUE,
+    "routing_key": QUEUE,
+    "correlation_id": CORRELATION_ID,
+    "reply_to": REPLY_TO,
+    "headers": HEADERS.copy(),
 }
 
 
 # Tornado's IO loop is not configurable in versions 5.x and up
 try:
+
     class MyIOLoop(tornado.ioloop.IOLoop.configured_class()):
         def handle_callback_exception(self, *args, **kwargs):
             raise
 
     tornado.ioloop.IOLoop.configure(MyIOLoop)
 except AttributeError:
     pass
 
 connection_classes = [pika.SelectConnection, TornadoConnection]
 
-parametrized_connection = pytest.mark.parametrize('ConnectionClass',
-        connection_classes)
+parametrized_connection = pytest.mark.parametrize("ConnectionClass", connection_classes)
 
 
 _test_select_conn_basic_get_inside_txn_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE, 1),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE, 1),
 ]
 
 if six.PY3:
     _test_select_conn_basic_get_inside_txn_metrics.append(
-        (('Function/test_pika_async_connection_consume:'
-          'test_async_connection_basic_get_inside_txn.'
-          '<locals>.on_message'), 1))
+        (
+            (
+                "Function/test_pika_async_connection_consume:"
+                "test_async_connection_basic_get_inside_txn."
+                "<locals>.on_message"
+            ),
+            1,
+        )
+    )
 else:
-    _test_select_conn_basic_get_inside_txn_metrics.append(
-        ('Function/test_pika_async_connection_consume:on_message', 1))
+    _test_select_conn_basic_get_inside_txn_metrics.append(("Function/test_pika_async_connection_consume:on_message", 1))
 
 
 @parametrized_connection
-@pytest.mark.parametrize('callback_as_partial', [True, False])
-@validate_code_level_metrics("test_pika_async_connection_consume.test_async_connection_basic_get_inside_txn.<locals>", "on_message", py2_namespace="test_pika_async_connection_consume")
+@pytest.mark.parametrize("callback_as_partial", [True, False])
+@validate_code_level_metrics(
+    "test_pika_async_connection_consume.test_async_connection_basic_get_inside_txn.<locals>",
+    "on_message",
+    py2_namespace="test_pika_async_connection_consume",
+)
 @validate_transaction_metrics(
-        ('test_pika_async_connection_consume:'
-                'test_async_connection_basic_get_inside_txn'),
-        scoped_metrics=_test_select_conn_basic_get_inside_txn_metrics,
-        rollup_metrics=_test_select_conn_basic_get_inside_txn_metrics,
-        background_task=True)
+    ("test_pika_async_connection_consume:" "test_async_connection_basic_get_inside_txn"),
+    scoped_metrics=_test_select_conn_basic_get_inside_txn_metrics,
+    rollup_metrics=_test_select_conn_basic_get_inside_txn_metrics,
+    background_task=True,
+)
 @validate_tt_collector_json(message_broker_params=_message_broker_tt_params)
 @background_task()
-def test_async_connection_basic_get_inside_txn(producer, ConnectionClass,
-        callback_as_partial):
+def test_async_connection_basic_get_inside_txn(producer, ConnectionClass, callback_as_partial):
     def on_message(channel, method_frame, header_frame, body):
         assert method_frame
         assert body == BODY
         channel.basic_ack(method_frame.delivery_tag)
         channel.close()
         connection.close()
         connection.ioloop.stop()
@@ -118,30 +125,27 @@
 
     def on_open_channel(channel):
         channel.basic_get(callback=on_message, queue=QUEUE)
 
     def on_open_connection(connection):
         connection.channel(on_open_callback=on_open_channel)
 
-    connection = ConnectionClass(
-            pika.ConnectionParameters(DB_SETTINGS['host']),
-            on_open_callback=on_open_connection)
+    connection = ConnectionClass(pika.ConnectionParameters(DB_SETTINGS["host"]), on_open_callback=on_open_connection)
 
     try:
         connection.ioloop.start()
     except:
         connection.close()
         connection.ioloop.stop()
         raise
 
 
 @parametrized_connection
-@pytest.mark.parametrize('callback_as_partial', [True, False])
-def test_select_connection_basic_get_outside_txn(producer, ConnectionClass,
-        callback_as_partial):
+@pytest.mark.parametrize("callback_as_partial", [True, False])
+def test_select_connection_basic_get_outside_txn(producer, ConnectionClass, callback_as_partial):
     metrics_list = []
 
     @capture_transaction_metrics(metrics_list)
     def test_basic_get():
         def on_message(channel, method_frame, header_frame, body):
             assert method_frame
             assert body == BODY
@@ -156,16 +160,16 @@
         def on_open_channel(channel):
             channel.basic_get(callback=on_message, queue=QUEUE)
 
         def on_open_connection(connection):
             connection.channel(on_open_callback=on_open_channel)
 
         connection = ConnectionClass(
-                pika.ConnectionParameters(DB_SETTINGS['host']),
-                on_open_callback=on_open_connection)
+            pika.ConnectionParameters(DB_SETTINGS["host"]), on_open_callback=on_open_connection
+        )
 
         try:
             connection.ioloop.start()
         except:
             connection.close()
             connection.ioloop.stop()
             raise
@@ -174,207 +178,229 @@
 
     # Confirm that no metrics have been created. This is because no background
     # task should be created for basic_get actions.
     assert not metrics_list
 
 
 _test_select_conn_basic_get_inside_txn_no_callback_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE, None),
 ]
 
 
 @pytest.mark.skipif(
-    condition=pika_version_info[0] > 0,
-    reason='pika 1.0 removed the ability to use basic_get with callback=None')
+    condition=pika_version_info[0] > 0, reason="pika 1.0 removed the ability to use basic_get with callback=None"
+)
 @parametrized_connection
 @validate_transaction_metrics(
-    ('test_pika_async_connection_consume:'
-            'test_async_connection_basic_get_inside_txn_no_callback'),
+    ("test_pika_async_connection_consume:" "test_async_connection_basic_get_inside_txn_no_callback"),
     scoped_metrics=_test_select_conn_basic_get_inside_txn_no_callback_metrics,
     rollup_metrics=_test_select_conn_basic_get_inside_txn_no_callback_metrics,
-    background_task=True)
+    background_task=True,
+)
 @validate_tt_collector_json(message_broker_params=_message_broker_tt_params)
 @background_task()
-def test_async_connection_basic_get_inside_txn_no_callback(producer,
-        ConnectionClass):
+def test_async_connection_basic_get_inside_txn_no_callback(producer, ConnectionClass):
     def on_open_channel(channel):
         channel.basic_get(callback=None, queue=QUEUE)
         channel.close()
         connection.close()
         connection.ioloop.stop()
 
     def on_open_connection(connection):
         connection.channel(on_open_callback=on_open_channel)
 
-    connection = ConnectionClass(
-            pika.ConnectionParameters(DB_SETTINGS['host']),
-            on_open_callback=on_open_connection)
+    connection = ConnectionClass(pika.ConnectionParameters(DB_SETTINGS["host"]), on_open_callback=on_open_connection)
 
     try:
         connection.ioloop.start()
     except:
         connection.close()
         connection.ioloop.stop()
         raise
 
 
 _test_async_connection_basic_get_empty_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE, None),
 ]
 
 
 @parametrized_connection
-@pytest.mark.parametrize('callback_as_partial', [True, False])
+@pytest.mark.parametrize("callback_as_partial", [True, False])
 @validate_transaction_metrics(
-        ('test_pika_async_connection_consume:'
-                'test_async_connection_basic_get_empty'),
-        scoped_metrics=_test_async_connection_basic_get_empty_metrics,
-        rollup_metrics=_test_async_connection_basic_get_empty_metrics,
-        background_task=True)
+    ("test_pika_async_connection_consume:" "test_async_connection_basic_get_empty"),
+    scoped_metrics=_test_async_connection_basic_get_empty_metrics,
+    rollup_metrics=_test_async_connection_basic_get_empty_metrics,
+    background_task=True,
+)
 @validate_tt_collector_json(message_broker_params=_message_broker_tt_params)
 @background_task()
-def test_async_connection_basic_get_empty(ConnectionClass,
-        callback_as_partial):
-    QUEUE = 'test_async_empty'
+def test_async_connection_basic_get_empty(ConnectionClass, callback_as_partial):
+    QUEUE = "test_async_empty"
 
     def on_message(channel, method_frame, header_frame, body):
-        assert False, body.decode('UTF-8')
+        assert False, body.decode("UTF-8")
 
     if callback_as_partial:
         on_message = functools.partial(on_message)
 
     def on_open_channel(channel):
         channel.basic_get(callback=on_message, queue=QUEUE)
         channel.close()
         connection.close()
         connection.ioloop.stop()
 
     def on_open_connection(connection):
         connection.channel(on_open_callback=on_open_channel)
 
-    connection = ConnectionClass(
-            pika.ConnectionParameters(DB_SETTINGS['host']),
-            on_open_callback=on_open_connection)
+    connection = ConnectionClass(pika.ConnectionParameters(DB_SETTINGS["host"]), on_open_callback=on_open_connection)
 
     try:
         connection.ioloop.start()
     except:
         connection.close()
         connection.ioloop.stop()
         raise
 
 
 _test_select_conn_basic_consume_in_txn_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE, None),
 ]
 
 if six.PY3:
     _test_select_conn_basic_consume_in_txn_metrics.append(
-        (('Function/test_pika_async_connection_consume:'
-          'test_async_connection_basic_consume_inside_txn.'
-          '<locals>.on_message'), 1))
+        (
+            (
+                "Function/test_pika_async_connection_consume:"
+                "test_async_connection_basic_consume_inside_txn."
+                "<locals>.on_message"
+            ),
+            1,
+        )
+    )
 else:
-    _test_select_conn_basic_consume_in_txn_metrics.append(
-        ('Function/test_pika_async_connection_consume:on_message', 1))
+    _test_select_conn_basic_consume_in_txn_metrics.append(("Function/test_pika_async_connection_consume:on_message", 1))
 
 
 @parametrized_connection
 @validate_transaction_metrics(
-        ('test_pika_async_connection_consume:'
-                'test_async_connection_basic_consume_inside_txn'),
-        scoped_metrics=_test_select_conn_basic_consume_in_txn_metrics,
-        rollup_metrics=_test_select_conn_basic_consume_in_txn_metrics,
-        background_task=True)
-@validate_code_level_metrics("test_pika_async_connection_consume.test_async_connection_basic_consume_inside_txn.<locals>", "on_message", py2_namespace="test_pika_async_connection_consume")
+    ("test_pika_async_connection_consume:" "test_async_connection_basic_consume_inside_txn"),
+    scoped_metrics=_test_select_conn_basic_consume_in_txn_metrics,
+    rollup_metrics=_test_select_conn_basic_consume_in_txn_metrics,
+    background_task=True,
+)
+@validate_code_level_metrics(
+    "test_pika_async_connection_consume.test_async_connection_basic_consume_inside_txn.<locals>",
+    "on_message",
+    py2_namespace="test_pika_async_connection_consume",
+)
 @validate_tt_collector_json(message_broker_params=_message_broker_tt_params)
 @background_task()
 def test_async_connection_basic_consume_inside_txn(producer, ConnectionClass):
     def on_message(channel, method_frame, header_frame, body):
-        assert hasattr(method_frame, '_nr_start_time')
+        assert hasattr(method_frame, "_nr_start_time")
         assert body == BODY
         channel.basic_ack(method_frame.delivery_tag)
         channel.close()
         connection.close()
         connection.ioloop.stop()
 
     def on_open_channel(channel):
         basic_consume(channel, QUEUE, on_message)
 
     def on_open_connection(connection):
         connection.channel(on_open_callback=on_open_channel)
 
-    connection = ConnectionClass(
-            pika.ConnectionParameters(DB_SETTINGS['host']),
-            on_open_callback=on_open_connection)
+    connection = ConnectionClass(pika.ConnectionParameters(DB_SETTINGS["host"]), on_open_callback=on_open_connection)
 
     try:
         connection.ioloop.start()
     except:
         connection.close()
         connection.ioloop.stop()
         raise
 
 
 _test_select_conn_basic_consume_two_exchanges = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE_2, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE_2, None),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE_2, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE_2, None),
 ]
 
 if six.PY3:
     _test_select_conn_basic_consume_two_exchanges.append(
-        (('Function/test_pika_async_connection_consume:'
-          'test_async_connection_basic_consume_two_exchanges.'
-          '<locals>.on_message_1'), 1))
+        (
+            (
+                "Function/test_pika_async_connection_consume:"
+                "test_async_connection_basic_consume_two_exchanges."
+                "<locals>.on_message_1"
+            ),
+            1,
+        )
+    )
     _test_select_conn_basic_consume_two_exchanges.append(
-        (('Function/test_pika_async_connection_consume:'
-          'test_async_connection_basic_consume_two_exchanges.'
-          '<locals>.on_message_2'), 1))
+        (
+            (
+                "Function/test_pika_async_connection_consume:"
+                "test_async_connection_basic_consume_two_exchanges."
+                "<locals>.on_message_2"
+            ),
+            1,
+        )
+    )
 else:
     _test_select_conn_basic_consume_two_exchanges.append(
-        ('Function/test_pika_async_connection_consume:on_message_1', 1))
+        ("Function/test_pika_async_connection_consume:on_message_1", 1)
+    )
     _test_select_conn_basic_consume_two_exchanges.append(
-        ('Function/test_pika_async_connection_consume:on_message_2', 1))
+        ("Function/test_pika_async_connection_consume:on_message_2", 1)
+    )
 
 
 @parametrized_connection
 @validate_transaction_metrics(
-        ('test_pika_async_connection_consume:'
-                'test_async_connection_basic_consume_two_exchanges'),
-        scoped_metrics=_test_select_conn_basic_consume_two_exchanges,
-        rollup_metrics=_test_select_conn_basic_consume_two_exchanges,
-        background_task=True)
-@validate_code_level_metrics("test_pika_async_connection_consume.test_async_connection_basic_consume_two_exchanges.<locals>", "on_message_1", py2_namespace="test_pika_async_connection_consume")
-@validate_code_level_metrics("test_pika_async_connection_consume.test_async_connection_basic_consume_two_exchanges.<locals>", "on_message_2", py2_namespace="test_pika_async_connection_consume")
+    ("test_pika_async_connection_consume:" "test_async_connection_basic_consume_two_exchanges"),
+    scoped_metrics=_test_select_conn_basic_consume_two_exchanges,
+    rollup_metrics=_test_select_conn_basic_consume_two_exchanges,
+    background_task=True,
+)
+@validate_code_level_metrics(
+    "test_pika_async_connection_consume.test_async_connection_basic_consume_two_exchanges.<locals>",
+    "on_message_1",
+    py2_namespace="test_pika_async_connection_consume",
+)
+@validate_code_level_metrics(
+    "test_pika_async_connection_consume.test_async_connection_basic_consume_two_exchanges.<locals>",
+    "on_message_2",
+    py2_namespace="test_pika_async_connection_consume",
+)
 @background_task()
-def test_async_connection_basic_consume_two_exchanges(producer, producer_2,
-        ConnectionClass):
+def test_async_connection_basic_consume_two_exchanges(producer, producer_2, ConnectionClass):
     global events_received
     events_received = 0
 
     def on_message_1(channel, method_frame, header_frame, body):
         channel.basic_ack(method_frame.delivery_tag)
-        assert hasattr(method_frame, '_nr_start_time')
+        assert hasattr(method_frame, "_nr_start_time")
         assert body == BODY
 
         global events_received
         events_received += 1
 
         if events_received == 2:
             channel.close()
             connection.close()
             connection.ioloop.stop()
 
     def on_message_2(channel, method_frame, header_frame, body):
         channel.basic_ack(method_frame.delivery_tag)
-        assert hasattr(method_frame, '_nr_start_time')
+        assert hasattr(method_frame, "_nr_start_time")
         assert body == BODY
 
         global events_received
         events_received += 1
 
         if events_received == 2:
             channel.close()
@@ -384,98 +410,106 @@
     def on_open_channel(channel):
         basic_consume(channel, QUEUE, on_message_1)
         basic_consume(channel, QUEUE_2, on_message_2)
 
     def on_open_connection(connection):
         connection.channel(on_open_callback=on_open_channel)
 
-    connection = ConnectionClass(
-            pika.ConnectionParameters(DB_SETTINGS['host']),
-            on_open_callback=on_open_connection)
+    connection = ConnectionClass(pika.ConnectionParameters(DB_SETTINGS["host"]), on_open_callback=on_open_connection)
 
     try:
         connection.ioloop.start()
     except:
         connection.close()
         connection.ioloop.stop()
         raise
 
 
 # This should not create a transaction
-@function_not_called('newrelic.core.stats_engine',
-                'StatsEngine.record_transaction')
-@override_application_settings({'debug.record_transaction_failure': True})
+@function_not_called("newrelic.core.stats_engine", "StatsEngine.record_transaction")
+@override_application_settings({"debug.record_transaction_failure": True})
 def test_tornado_connection_basic_consume_outside_transaction(producer):
     def on_message(channel, method_frame, header_frame, body):
-        assert hasattr(method_frame, '_nr_start_time')
+        assert hasattr(method_frame, "_nr_start_time")
         assert body == BODY
         channel.basic_ack(method_frame.delivery_tag)
         channel.close()
         connection.close()
         connection.ioloop.stop()
 
     def on_open_channel(channel):
         basic_consume(channel, QUEUE, on_message)
 
     def on_open_connection(connection):
         connection.channel(on_open_callback=on_open_channel)
 
-    connection = TornadoConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host']),
-            on_open_callback=on_open_connection)
+    connection = TornadoConnection(pika.ConnectionParameters(DB_SETTINGS["host"]), on_open_callback=on_open_connection)
 
     try:
         connection.ioloop.start()
     except:
         connection.close()
         connection.ioloop.stop()
         raise
 
 
 if six.PY3:
-    _txn_name = ('test_pika_async_connection_consume:'
-            'test_select_connection_basic_consume_outside_transaction.'
-            '<locals>.on_message')
+    _txn_name = (
+        "test_pika_async_connection_consume:"
+        "test_select_connection_basic_consume_outside_transaction."
+        "<locals>.on_message"
+    )
     _test_select_connection_consume_outside_txn_metrics = [
-        (('Function/test_pika_async_connection_consume:'
-          'test_select_connection_basic_consume_outside_transaction.'
-          '<locals>.on_message'), None)]
+        (
+            (
+                "Function/test_pika_async_connection_consume:"
+                "test_select_connection_basic_consume_outside_transaction."
+                "<locals>.on_message"
+            ),
+            None,
+        )
+    ]
 else:
-    _txn_name = (
-        'test_pika_async_connection_consume:on_message')
+    _txn_name = "test_pika_async_connection_consume:on_message"
     _test_select_connection_consume_outside_txn_metrics = [
-        ('Function/test_pika_async_connection_consume:on_message', None)]
+        ("Function/test_pika_async_connection_consume:on_message", None)
+    ]
 
 
 # This should create a transaction
 @validate_transaction_metrics(
-        _txn_name,
-        scoped_metrics=_test_select_connection_consume_outside_txn_metrics,
-        rollup_metrics=_test_select_connection_consume_outside_txn_metrics,
-        background_task=True,
-        group='Message/RabbitMQ/Exchange/%s' % EXCHANGE)
-@validate_code_level_metrics("test_pika_async_connection_consume.test_select_connection_basic_consume_outside_transaction.<locals>", "on_message", py2_namespace="test_pika_async_connection_consume")
+    _txn_name,
+    scoped_metrics=_test_select_connection_consume_outside_txn_metrics,
+    rollup_metrics=_test_select_connection_consume_outside_txn_metrics,
+    background_task=True,
+    group="Message/RabbitMQ/Exchange/%s" % EXCHANGE,
+)
+@validate_code_level_metrics(
+    "test_pika_async_connection_consume.test_select_connection_basic_consume_outside_transaction.<locals>",
+    "on_message",
+    py2_namespace="test_pika_async_connection_consume",
+)
 def test_select_connection_basic_consume_outside_transaction(producer):
     def on_message(channel, method_frame, header_frame, body):
-        assert hasattr(method_frame, '_nr_start_time')
+        assert hasattr(method_frame, "_nr_start_time")
         assert body == BODY
         channel.basic_ack(method_frame.delivery_tag)
         channel.close()
         connection.close()
         connection.ioloop.stop()
 
     def on_open_channel(channel):
         basic_consume(channel, QUEUE, on_message)
 
     def on_open_connection(connection):
         connection.channel(on_open_callback=on_open_channel)
 
     connection = pika.SelectConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host']),
-            on_open_callback=on_open_connection)
+        pika.ConnectionParameters(DB_SETTINGS["host"]), on_open_callback=on_open_connection
+    )
 
     try:
         connection.ioloop.start()
     except:
         connection.close()
         connection.ioloop.stop()
         raise
```

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/test_pika_blocking_connection_consume.py` & `newrelic-9.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 import functools
 import os
 
 import pika
 import pytest
-import six
 from compat import basic_consume
 from conftest import BODY, CORRELATION_ID, EXCHANGE, HEADERS, QUEUE, REPLY_TO
 from testing_support.db_settings import rabbitmq_settings
 from testing_support.fixtures import capture_transaction_metrics
 from testing_support.validators.validate_code_level_metrics import (
     validate_code_level_metrics,
 )
@@ -30,68 +29,66 @@
 )
 from testing_support.validators.validate_tt_collector_json import (
     validate_tt_collector_json,
 )
 
 from newrelic.api.background_task import background_task
 from newrelic.api.transaction import end_of_transaction
+from newrelic.packages import six
 
 DB_SETTINGS = rabbitmq_settings()[0]
 
 _message_broker_tt_params = {
-    'queue_name': QUEUE,
-    'routing_key': QUEUE,
-    'correlation_id': CORRELATION_ID,
-    'reply_to': REPLY_TO,
-    'headers': HEADERS.copy(),
+    "queue_name": QUEUE,
+    "routing_key": QUEUE,
+    "correlation_id": CORRELATION_ID,
+    "reply_to": REPLY_TO,
+    "headers": HEADERS.copy(),
 }
 
 _test_blocking_connection_basic_get_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE, 1),
-    (('Function/pika.adapters.blocking_connection:'
-            '_CallbackResult.set_value_once'), 1)
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE, 1),
+    (("Function/pika.adapters.blocking_connection:" "_CallbackResult.set_value_once"), 1),
 ]
 
 
 @validate_transaction_metrics(
-        ('test_pika_blocking_connection_consume:'
-                'test_blocking_connection_basic_get'),
-        scoped_metrics=_test_blocking_connection_basic_get_metrics,
-        rollup_metrics=_test_blocking_connection_basic_get_metrics,
-        background_task=True)
+    ("test_pika_blocking_connection_consume:" "test_blocking_connection_basic_get"),
+    scoped_metrics=_test_blocking_connection_basic_get_metrics,
+    rollup_metrics=_test_blocking_connection_basic_get_metrics,
+    background_task=True,
+)
 @validate_tt_collector_json(message_broker_params=_message_broker_tt_params)
 @background_task()
 def test_blocking_connection_basic_get(producer):
-    with pika.BlockingConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host'])) as connection:
+    with pika.BlockingConnection(pika.ConnectionParameters(DB_SETTINGS["host"])) as connection:
         channel = connection.channel()
         method_frame, _, _ = channel.basic_get(QUEUE)
         assert method_frame
         channel.basic_ack(method_frame.delivery_tag)
 
 
 _test_blocking_connection_basic_get_empty_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE, None),
 ]
 
 
 @validate_transaction_metrics(
-        ('test_pika_blocking_connection_consume:'
-                'test_blocking_connection_basic_get_empty'),
-        scoped_metrics=_test_blocking_connection_basic_get_empty_metrics,
-        rollup_metrics=_test_blocking_connection_basic_get_empty_metrics,
-        background_task=True)
+    ("test_pika_blocking_connection_consume:" "test_blocking_connection_basic_get_empty"),
+    scoped_metrics=_test_blocking_connection_basic_get_empty_metrics,
+    rollup_metrics=_test_blocking_connection_basic_get_empty_metrics,
+    background_task=True,
+)
 @validate_tt_collector_json(message_broker_params=_message_broker_tt_params)
 @background_task()
 def test_blocking_connection_basic_get_empty():
-    QUEUE = 'test_blocking_empty-%s' % os.getpid()
-    with pika.BlockingConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host'])) as connection:
+    QUEUE = "test_blocking_empty-%s" % os.getpid()
+    with pika.BlockingConnection(pika.ConnectionParameters(DB_SETTINGS["host"])) as connection:
         channel = connection.channel()
         channel.queue_declare(queue=QUEUE)
 
         try:
             method_frame, _, _ = channel.basic_get(QUEUE)
             assert method_frame is None
         finally:
@@ -99,16 +96,15 @@
 
 
 def test_blocking_connection_basic_get_outside_transaction(producer):
     metrics_list = []
 
     @capture_transaction_metrics(metrics_list)
     def test_basic_get():
-        with pika.BlockingConnection(
-                pika.ConnectionParameters(DB_SETTINGS['host'])) as connection:
+        with pika.BlockingConnection(pika.ConnectionParameters(DB_SETTINGS["host"])) as connection:
             channel = connection.channel()
             channel.queue_declare(queue=QUEUE)
 
             method_frame, _, _ = channel.basic_get(QUEUE)
             channel.basic_ack(method_frame.delivery_tag)
             assert method_frame
 
@@ -116,147 +112,174 @@
 
     # Confirm that no metrics have been created. This is because no background
     # task should be created for basic_get actions.
     assert not metrics_list
 
 
 _test_blocking_conn_basic_consume_no_txn_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE, None),
 ]
 
 if six.PY3:
-    _txn_name = ('test_pika_blocking_connection_consume:'
-            'test_blocking_connection_basic_consume_outside_transaction.'
-            '<locals>.on_message')
+    _txn_name = (
+        "test_pika_blocking_connection_consume:"
+        "test_blocking_connection_basic_consume_outside_transaction."
+        "<locals>.on_message"
+    )
     _test_blocking_conn_basic_consume_no_txn_metrics.append(
-        (('Function/test_pika_blocking_connection_consume:'
-          'test_blocking_connection_basic_consume_outside_transaction.'
-          '<locals>.on_message'), None))
+        (
+            (
+                "Function/test_pika_blocking_connection_consume:"
+                "test_blocking_connection_basic_consume_outside_transaction."
+                "<locals>.on_message"
+            ),
+            None,
+        )
+    )
 else:
-    _txn_name = ('test_pika_blocking_connection_consume:'
-            'on_message')
+    _txn_name = "test_pika_blocking_connection_consume:" "on_message"
     _test_blocking_conn_basic_consume_no_txn_metrics.append(
-        ('Function/test_pika_blocking_connection_consume:on_message', None))
+        ("Function/test_pika_blocking_connection_consume:on_message", None)
+    )
 
 
-@pytest.mark.parametrize('as_partial', [True, False])
-@validate_code_level_metrics("test_pika_blocking_connection_consume.test_blocking_connection_basic_consume_outside_transaction.<locals>", "on_message", py2_namespace="test_pika_blocking_connection_consume")
+@pytest.mark.parametrize("as_partial", [True, False])
+@validate_code_level_metrics(
+    "test_pika_blocking_connection_consume.test_blocking_connection_basic_consume_outside_transaction.<locals>",
+    "on_message",
+    py2_namespace="test_pika_blocking_connection_consume",
+)
 @validate_transaction_metrics(
-        _txn_name,
-        scoped_metrics=_test_blocking_conn_basic_consume_no_txn_metrics,
-        rollup_metrics=_test_blocking_conn_basic_consume_no_txn_metrics,
-        background_task=True,
-        group='Message/RabbitMQ/Exchange/%s' % EXCHANGE)
+    _txn_name,
+    scoped_metrics=_test_blocking_conn_basic_consume_no_txn_metrics,
+    rollup_metrics=_test_blocking_conn_basic_consume_no_txn_metrics,
+    background_task=True,
+    group="Message/RabbitMQ/Exchange/%s" % EXCHANGE,
+)
 @validate_tt_collector_json(message_broker_params=_message_broker_tt_params)
-def test_blocking_connection_basic_consume_outside_transaction(producer,
-        as_partial):
+def test_blocking_connection_basic_consume_outside_transaction(producer, as_partial):
     def on_message(channel, method_frame, header_frame, body):
-        assert hasattr(method_frame, '_nr_start_time')
+        assert hasattr(method_frame, "_nr_start_time")
         assert body == BODY
         channel.stop_consuming()
 
     if as_partial:
         on_message = functools.partial(on_message)
 
-    with pika.BlockingConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host'])) as connection:
+    with pika.BlockingConnection(pika.ConnectionParameters(DB_SETTINGS["host"])) as connection:
         channel = connection.channel()
 
         basic_consume(channel, QUEUE, on_message)
         try:
             channel.start_consuming()
         except:
             channel.stop_consuming()
             raise
 
 
 _test_blocking_conn_basic_consume_in_txn_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE, None),
 ]
 
 if six.PY3:
     _test_blocking_conn_basic_consume_in_txn_metrics.append(
-        (('Function/test_pika_blocking_connection_consume:'
-          'test_blocking_connection_basic_consume_inside_txn.'
-          '<locals>.on_message'), 1))
+        (
+            (
+                "Function/test_pika_blocking_connection_consume:"
+                "test_blocking_connection_basic_consume_inside_txn."
+                "<locals>.on_message"
+            ),
+            1,
+        )
+    )
 else:
     _test_blocking_conn_basic_consume_in_txn_metrics.append(
-        ('Function/test_pika_blocking_connection_consume:on_message', 1))
+        ("Function/test_pika_blocking_connection_consume:on_message", 1)
+    )
 
 
-@pytest.mark.parametrize('as_partial', [True, False])
-@validate_code_level_metrics("test_pika_blocking_connection_consume.test_blocking_connection_basic_consume_inside_txn.<locals>", "on_message", py2_namespace="test_pika_blocking_connection_consume")
+@pytest.mark.parametrize("as_partial", [True, False])
+@validate_code_level_metrics(
+    "test_pika_blocking_connection_consume.test_blocking_connection_basic_consume_inside_txn.<locals>",
+    "on_message",
+    py2_namespace="test_pika_blocking_connection_consume",
+)
 @validate_transaction_metrics(
-        ('test_pika_blocking_connection_consume:'
-                'test_blocking_connection_basic_consume_inside_txn'),
-        scoped_metrics=_test_blocking_conn_basic_consume_in_txn_metrics,
-        rollup_metrics=_test_blocking_conn_basic_consume_in_txn_metrics,
-        background_task=True)
+    ("test_pika_blocking_connection_consume:" "test_blocking_connection_basic_consume_inside_txn"),
+    scoped_metrics=_test_blocking_conn_basic_consume_in_txn_metrics,
+    rollup_metrics=_test_blocking_conn_basic_consume_in_txn_metrics,
+    background_task=True,
+)
 @validate_tt_collector_json(message_broker_params=_message_broker_tt_params)
 @background_task()
 def test_blocking_connection_basic_consume_inside_txn(producer, as_partial):
     def on_message(channel, method_frame, header_frame, body):
-        assert hasattr(method_frame, '_nr_start_time')
+        assert hasattr(method_frame, "_nr_start_time")
         assert body == BODY
         channel.stop_consuming()
 
     if as_partial:
         on_message = functools.partial(on_message)
 
-    with pika.BlockingConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host'])) as connection:
+    with pika.BlockingConnection(pika.ConnectionParameters(DB_SETTINGS["host"])) as connection:
         channel = connection.channel()
         basic_consume(channel, QUEUE, on_message)
         try:
             channel.start_consuming()
         except:
             channel.stop_consuming()
             raise
 
 
 _test_blocking_conn_basic_consume_stopped_txn_metrics = [
-    ('MessageBroker/RabbitMQ/Exchange/Produce/Named/%s' % EXCHANGE, None),
-    ('MessageBroker/RabbitMQ/Exchange/Consume/Named/%s' % EXCHANGE, None),
-    ('OtherTransaction/Message/RabbitMQ/Exchange/Named/%s' % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Produce/Named/%s" % EXCHANGE, None),
+    ("MessageBroker/RabbitMQ/Exchange/Consume/Named/%s" % EXCHANGE, None),
+    ("OtherTransaction/Message/RabbitMQ/Exchange/Named/%s" % EXCHANGE, None),
 ]
 
 if six.PY3:
     _test_blocking_conn_basic_consume_stopped_txn_metrics.append(
-        (('Function/test_pika_blocking_connection_consume:'
-          'test_blocking_connection_basic_consume_stopped_txn.'
-          '<locals>.on_message'), None))
+        (
+            (
+                "Function/test_pika_blocking_connection_consume:"
+                "test_blocking_connection_basic_consume_stopped_txn."
+                "<locals>.on_message"
+            ),
+            None,
+        )
+    )
 else:
     _test_blocking_conn_basic_consume_stopped_txn_metrics.append(
-        ('Function/test_pika_blocking_connection_consume:on_message', None))
+        ("Function/test_pika_blocking_connection_consume:on_message", None)
+    )
 
 
-@pytest.mark.parametrize('as_partial', [True, False])
+@pytest.mark.parametrize("as_partial", [True, False])
 @validate_transaction_metrics(
-        ('test_pika_blocking_connection_consume:'
-                'test_blocking_connection_basic_consume_stopped_txn'),
-        scoped_metrics=_test_blocking_conn_basic_consume_stopped_txn_metrics,
-        rollup_metrics=_test_blocking_conn_basic_consume_stopped_txn_metrics,
-        background_task=True)
+    ("test_pika_blocking_connection_consume:" "test_blocking_connection_basic_consume_stopped_txn"),
+    scoped_metrics=_test_blocking_conn_basic_consume_stopped_txn_metrics,
+    rollup_metrics=_test_blocking_conn_basic_consume_stopped_txn_metrics,
+    background_task=True,
+)
 @validate_tt_collector_json(message_broker_params=_message_broker_tt_params)
 @background_task()
 def test_blocking_connection_basic_consume_stopped_txn(producer, as_partial):
     def on_message(channel, method_frame, header_frame, body):
-        assert hasattr(method_frame, '_nr_start_time')
+        assert hasattr(method_frame, "_nr_start_time")
         assert body == BODY
         channel.stop_consuming()
 
     end_of_transaction()
 
     if as_partial:
         on_message = functools.partial(on_message)
 
-    with pika.BlockingConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host'])) as connection:
+    with pika.BlockingConnection(pika.ConnectionParameters(DB_SETTINGS["host"])) as connection:
         channel = connection.channel()
         basic_consume(channel, QUEUE, on_message)
         try:
             channel.start_consuming()
         except:
             channel.stop_consuming()
             raise
```

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py` & `newrelic-9.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/test_pika_produce.py` & `newrelic-9.9.0/tests/messagebroker_pika/test_pika_produce.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/messagebroker_pika/test_pika_supportability.py` & `newrelic-9.9.0/tests/messagebroker_pika/test_pika_supportability.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,68 +8,63 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from compat import basic_consume
 import pika
-import six
+from compat import basic_consume
+from conftest import BODY, QUEUE
+from testing_support.db_settings import rabbitmq_settings
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
 
 from newrelic.api.background_task import background_task
-
-from conftest import QUEUE, BODY
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
-from testing_support.db_settings import rabbitmq_settings
+from newrelic.packages import six
 
 DB_SETTINGS = rabbitmq_settings()[0]
 
 
 class CustomPikaChannel(pika.channel.Channel):
     def _on_getok(self, method_frame, header_frame, body):
         if self._on_getok_callback is not None:
             callback = self._on_getok_callback
             self._on_getok_callback = None
             # Use kwargs to pass values to callback
-            callback(channel=self,
-                    method_frame=method_frame.method,
-                    header_frame=header_frame.properties,
-                    body=body)
+            callback(channel=self, method_frame=method_frame.method, header_frame=header_frame.properties, body=body)
 
     def _on_deliver(self, method_frame, header_frame, body):
         consumer_tag = method_frame.method.consumer_tag
 
         if consumer_tag in self._cancelled:
             if self.is_open and consumer_tag not in self._consumers_with_noack:
                 self.basic_reject(method_frame.method.delivery_tag)
             return
 
-        self._consumers[consumer_tag](channel=self,
-                method_frame=method_frame.method,
-                header_frame=header_frame.properties,
-                body=body)
+        self._consumers[consumer_tag](
+            channel=self, method_frame=method_frame.method, header_frame=header_frame.properties, body=body
+        )
 
 
 class CustomPikaConnection(pika.SelectConnection):
     def _create_channel(self, channel_number, on_open_callback):
         return CustomPikaChannel(self, channel_number, on_open_callback)
 
 
-_test_select_connection_supportability_metrics = [
-    ('Supportability/hooks/pika/kwargs_error', 1)
-]
+_test_select_connection_supportability_metrics = [("Supportability/hooks/pika/kwargs_error", 1)]
 
 
 @validate_transaction_metrics(
-        ('test_pika_supportability:'
-                'test_select_connection_supportability_in_txn'),
-        scoped_metrics=(),
-        rollup_metrics=_test_select_connection_supportability_metrics,
-        background_task=True)
+    ("test_pika_supportability:" "test_select_connection_supportability_in_txn"),
+    scoped_metrics=(),
+    rollup_metrics=_test_select_connection_supportability_metrics,
+    background_task=True,
+)
 @background_task()
 def test_select_connection_supportability_in_txn(producer):
     def on_message(channel, method_frame, header_frame, body):
         assert method_frame
         assert body == BODY
         channel.basic_ack(method_frame.delivery_tag)
         channel.close()
@@ -79,42 +74,40 @@
     def on_open_channel(channel):
         channel.basic_get(callback=on_message, queue=QUEUE)
 
     def on_open_connection(connection):
         connection.channel(on_open_callback=on_open_channel)
 
     connection = CustomPikaConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host']),
-            on_open_callback=on_open_connection)
+        pika.ConnectionParameters(DB_SETTINGS["host"]), on_open_callback=on_open_connection
+    )
 
     try:
         connection.ioloop.start()
     except:
         connection.close()
         # Start the IOLoop again so Pika can communicate, it will stop on its
         # own when the connection is closed
         connection.ioloop.stop()
         raise
 
 
 if six.PY3:
-    _txn_name = ('test_pika_supportability:'
-            'test_select_connection_supportability_outside_txn.'
-            '<locals>.on_message')
+    _txn_name = "test_pika_supportability:" "test_select_connection_supportability_outside_txn." "<locals>.on_message"
 else:
-    _txn_name = (
-        'test_pika_supportability:on_message')
+    _txn_name = "test_pika_supportability:on_message"
 
 
 @validate_transaction_metrics(
-        _txn_name,
-        scoped_metrics=(),
-        rollup_metrics=_test_select_connection_supportability_metrics,
-        background_task=True,
-        group='Message/RabbitMQ/Exchange/Unknown')
+    _txn_name,
+    scoped_metrics=(),
+    rollup_metrics=_test_select_connection_supportability_metrics,
+    background_task=True,
+    group="Message/RabbitMQ/Exchange/Unknown",
+)
 def test_select_connection_supportability_outside_txn(producer):
     def on_message(channel, method_frame, header_frame, body):
         assert method_frame
         assert body == BODY
         channel.basic_ack(method_frame.delivery_tag)
         channel.close()
         connection.close()
@@ -123,16 +116,16 @@
     def on_open_channel(channel):
         basic_consume(channel, QUEUE, on_message)
 
     def on_open_connection(connection):
         connection.channel(on_open_callback=on_open_channel)
 
     connection = CustomPikaConnection(
-            pika.ConnectionParameters(DB_SETTINGS['host']),
-            on_open_callback=on_open_connection)
+        pika.ConnectionParameters(DB_SETTINGS["host"]), on_open_callback=on_open_connection
+    )
 
     try:
         connection.ioloop.start()
     except:
         connection.close()
         # Start the IOLoop again so Pika can communicate, it will stop on its
         # own when the connection is closed
```

### Comparing `newrelic-9.8.0/tests/mlmodel_langchain/_mock_external_openai_server.py` & `newrelic-9.9.0/tests/mlmodel_langchain/_mock_external_openai_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_langchain/conftest.py` & `newrelic-9.9.0/tests/mlmodel_langchain/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_langchain/hello.pdf` & `newrelic-9.9.0/tests/mlmodel_langchain/hello.pdf`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_langchain/test_agent.py` & `newrelic-9.9.0/tests/mlmodel_langchain/test_agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_langchain/test_chain.py` & `newrelic-9.9.0/tests/mlmodel_langchain/test_chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,22 @@
 from langchain.chains.openai_functions import (
     create_structured_output_chain,
     create_structured_output_runnable,
 )
 from langchain.prompts import ChatPromptTemplate
 from langchain.schema import BaseOutputParser
 from mock import patch
-from testing_support.fixtures import (
-    reset_core_stats_engine,
-    validate_attributes,
-    validate_custom_event_count,
-)
+from testing_support.fixtures import reset_core_stats_engine, validate_attributes
 from testing_support.ml_testing_utils import (  # noqa: F401
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     events_sans_content,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_transaction_error_event_count import (
     validate_transaction_error_event_count,
 )
```

### Comparing `newrelic-9.8.0/tests/mlmodel_langchain/test_tool.py` & `newrelic-9.9.0/tests/mlmodel_langchain/test_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,24 +17,21 @@
 import uuid
 
 import langchain
 import pydantic
 import pytest
 from langchain.tools import tool
 from mock import patch
-from testing_support.fixtures import (
-    reset_core_stats_engine,
-    validate_attributes,
-    validate_custom_event_count,
-)
+from testing_support.fixtures import reset_core_stats_engine, validate_attributes
 from testing_support.ml_testing_utils import (  # noqa: F401
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_transaction_error_event_count import (
     validate_transaction_error_event_count,
 )
```

### Comparing `newrelic-9.8.0/tests/mlmodel_langchain/test_vectorstore.py` & `newrelic-9.9.0/tests/mlmodel_langchain/test_vectorstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,21 @@
 import copy
 import os
 
 import langchain
 import pytest
 from langchain_community.document_loaders import PyPDFLoader
 from langchain_community.vectorstores.faiss import FAISS
-from testing_support.fixtures import (
-    reset_core_stats_engine,
-    validate_attributes,
-    validate_custom_event_count,
-)
+from testing_support.fixtures import reset_core_stats_engine, validate_attributes
 from testing_support.ml_testing_utils import (  # noqa: F401
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/_mock_external_openai_server.py` & `newrelic-9.9.0/tests/mlmodel_openai/_mock_external_openai_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/conftest.py` & `newrelic-9.9.0/tests/mlmodel_openai/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 
 import openai
 from testing_support.fixtures import (
     override_llm_token_callback_settings,
     reset_core_stats_engine,
     validate_attributes,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     disabled_ai_monitoring_streaming_settings,
     events_sans_content,
     events_sans_llm_metadata,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
 
 from newrelic.api.background_task import background_task
 from newrelic.api.transaction import add_custom_attribute
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_error.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
 import openai
 import pytest
 from testing_support.fixtures import (
     dt_enabled,
     override_llm_token_callback_settings,
     reset_core_stats_engine,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     events_sans_content,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_span_events import validate_span_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_error_v1.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_error_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 import openai
 import pytest
 from testing_support.fixtures import (
     dt_enabled,
     override_llm_token_callback_settings,
     reset_core_stats_engine,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     events_sans_content,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_span_events import validate_span_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_stream.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 
 import openai
 from testing_support.fixtures import (
     override_llm_token_callback_settings,
     reset_core_stats_engine,
     validate_attributes,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     disabled_ai_monitoring_streaming_settings,
     events_sans_content,
     events_sans_llm_metadata,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
 
 from newrelic.api.background_task import background_task
 from newrelic.api.transaction import add_custom_attribute
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_stream_error.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
 import openai
 import pytest
 from testing_support.fixtures import (
     dt_enabled,
     override_llm_token_callback_settings,
     reset_core_stats_engine,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     events_sans_content,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_span_events import validate_span_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_stream_error_v1.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_error_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 
 import openai
 import pytest
 from testing_support.fixtures import (
     dt_enabled,
     override_llm_token_callback_settings,
     reset_core_stats_engine,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     events_sans_content,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_span_events import validate_span_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_stream_v1.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_stream_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 
 import openai
 from testing_support.fixtures import (
     override_llm_token_callback_settings,
     reset_core_stats_engine,
     validate_attributes,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     disabled_ai_monitoring_streaming_settings,
     events_sans_content,
     events_sans_llm_metadata,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
 
 from newrelic.api.background_task import background_task
 from newrelic.api.transaction import add_custom_attribute
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_chat_completion_v1.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_chat_completion_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 
 import openai
 from testing_support.fixtures import (
     override_llm_token_callback_settings,
     reset_core_stats_engine,
     validate_attributes,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     disabled_ai_monitoring_streaming_settings,
     events_sans_content,
     events_sans_llm_metadata,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
 
 from newrelic.api.background_task import background_task
 from newrelic.api.transaction import add_custom_attribute
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_embeddings.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # limitations under the License.
 
 import openai
 from testing_support.fixtures import (  # override_application_settings,
     override_llm_token_callback_settings,
     reset_core_stats_engine,
     validate_attributes,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     events_sans_content,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
 
 from newrelic.api.background_task import background_task
 from newrelic.api.transaction import add_custom_attribute
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_embeddings_error.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 import openai
 import pytest
 from testing_support.fixtures import (
     dt_enabled,
     override_llm_token_callback_settings,
     reset_core_stats_engine,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     events_sans_content,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_span_events import validate_span_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_embeddings_error_v1.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_error_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 
 import openai
 import pytest
 from testing_support.fixtures import (
     dt_enabled,
     override_llm_token_callback_settings,
     reset_core_stats_engine,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     events_sans_content,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_error_trace_attributes import (
     validate_error_trace_attributes,
 )
 from testing_support.validators.validate_span_events import validate_span_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_embeddings_stream_v1.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_stream_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pytest
 from conftest import get_openai_version  # pylint: disable=E0611
-from testing_support.fixtures import (
-    reset_core_stats_engine,
-    validate_custom_event_count,
-)
+from testing_support.fixtures import reset_core_stats_engine
 from testing_support.ml_testing_utils import set_trace_info  # noqa: F401
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 
 from newrelic.api.background_task import background_task
 
 OPENAI_VERSION = get_openai_version()
 SKIP_IF_NO_OPENAI_EMBEDDING_STREAMING_SUPPORT = pytest.mark.skipif(
     OPENAI_VERSION < (1, 8), reason="OpenAI does not support embedding streaming until v1.8"
 )
```

### Comparing `newrelic-9.8.0/tests/mlmodel_openai/test_embeddings_v1.py` & `newrelic-9.9.0/tests/mlmodel_openai/test_embeddings_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 # limitations under the License.
 
 import openai
 from testing_support.fixtures import (
     override_llm_token_callback_settings,
     reset_core_stats_engine,
     validate_attributes,
-    validate_custom_event_count,
 )
 from testing_support.ml_testing_utils import (  # noqa: F401
     add_token_count_to_events,
     disabled_ai_monitoring_record_content_settings,
     disabled_ai_monitoring_settings,
     events_sans_content,
     llm_token_count_callback,
     set_trace_info,
 )
+from testing_support.validators.validate_custom_event import validate_custom_event_count
 from testing_support.validators.validate_custom_events import validate_custom_events
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
 
 from newrelic.api.background_task import background_task
```

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/conftest.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_calibration_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_calibration_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_cluster_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_cluster_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_compose_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_compose_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_covariance_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_covariance_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_cross_decomposition_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_cross_decomposition_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_discriminant_analysis_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_discriminant_analysis_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_dummy_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_dummy_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_ensemble_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_ensemble_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_feature_selection_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_feature_selection_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_gaussian_process_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_gaussian_process_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_inference_events.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_inference_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_kernel_ridge_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_kernel_ridge_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_linear_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_linear_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_metric_scorers.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_metric_scorers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_mixture_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_mixture_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_ml_model.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_ml_model.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_model_selection_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_model_selection_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_multiclass_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_multiclass_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_multioutput_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_multioutput_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_naive_bayes_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_naive_bayes_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_neighbors_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_neighbors_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_neural_network_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_neural_network_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_pipeline_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_pipeline_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_prediction_stats.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_prediction_stats.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_semi_supervised_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_semi_supervised_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_svm_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_svm_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/mlmodel_sklearn/test_tree_models.py` & `newrelic-9.9.0/tests/mlmodel_sklearn/test_tree_models.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/template_genshi/conftest.py` & `newrelic-9.9.0/tests/template_mako/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from testing_support.fixtures import (  # noqa: F401; pylint: disable=W0611
-    collector_agent_registration_fixture,
-    collector_available_fixture,
-)
+from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
 
 _default_settings = {
-    "transaction_tracer.explain_threshold": 0.0,
-    "transaction_tracer.transaction_threshold": 0.0,
-    "transaction_tracer.stack_trace_threshold": 0.0,
-    "debug.log_data_collector_payloads": True,
-    "debug.record_transaction_failure": True,
+    'transaction_tracer.explain_threshold': 0.0,
+    'transaction_tracer.transaction_threshold': 0.0,
+    'transaction_tracer.stack_trace_threshold': 0.0,
+    'debug.log_data_collector_payloads': True,
+    'debug.record_transaction_failure': True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-    app_name="Python Agent Test (template_genshi)", default_settings=_default_settings
-)
+        app_name='Python Agent Test (template_mako)',
+        default_settings=_default_settings)
+
```

### Comparing `newrelic-9.8.0/tests/template_genshi/test_genshi.py` & `newrelic-9.9.0/tests/template_genshi/test_genshi.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/template_jinja2/conftest.py` & `newrelic-9.9.0/tests/framework_ariadne/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,18 +13,25 @@
 # limitations under the License.
 
 from testing_support.fixtures import (  # noqa: F401; pylint: disable=W0611
     collector_agent_registration_fixture,
     collector_available_fixture,
 )
 
+from newrelic.packages import six
+
 _default_settings = {
     "transaction_tracer.explain_threshold": 0.0,
     "transaction_tracer.transaction_threshold": 0.0,
     "transaction_tracer.stack_trace_threshold": 0.0,
     "debug.log_data_collector_payloads": True,
     "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-    app_name="Python Agent Test (template_jinja2)", default_settings=_default_settings
+    app_name="Python Agent Test (framework_ariadne)",
+    default_settings=_default_settings,
 )
+
+
+if six.PY2:
+    collect_ignore = ["test_application_async.py"]
```

### Comparing `newrelic-9.8.0/tests/template_jinja2/test_jinja2.py` & `newrelic-9.9.0/tests/template_jinja2/test_jinja2.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/template_mako/conftest.py` & `newrelic-9.9.0/tests/application_celery/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,22 +7,44 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from testing_support.fixtures import collector_agent_registration_fixture, collector_available_fixture  # noqa: F401; pylint: disable=W0611
+import pytest
+from testing_support.fixtures import (  # noqa: F401; pylint: disable=W0611
+    collector_agent_registration_fixture,
+    collector_available_fixture,
+)
 
 _default_settings = {
-    'transaction_tracer.explain_threshold': 0.0,
-    'transaction_tracer.transaction_threshold': 0.0,
-    'transaction_tracer.stack_trace_threshold': 0.0,
-    'debug.log_data_collector_payloads': True,
-    'debug.record_transaction_failure': True,
+    "transaction_tracer.explain_threshold": 0.0,
+    "transaction_tracer.transaction_threshold": 0.0,
+    "transaction_tracer.stack_trace_threshold": 0.0,
+    "debug.log_data_collector_payloads": True,
+    "debug.record_transaction_failure": True,
 }
 
 collector_agent_registration = collector_agent_registration_fixture(
-        app_name='Python Agent Test (template_mako)',
-        default_settings=_default_settings)
+    app_name="Python Agent Test (application_celery)", default_settings=_default_settings
+)
+
+
+@pytest.fixture(scope="session")
+def celery_config():
+    # Used by celery pytest plugin to configure Celery instance
+    return {
+        "broker_url": "memory://",
+        "result_backend": "cache+memory://",
+    }
+
+
+@pytest.fixture(scope="session")
+def celery_worker_parameters():
+    # Used by celery pytest plugin to configure worker instance
+    return {"shutdown_timeout": 120}
+
 
+@pytest.fixture(scope="session", autouse=True)
+def celery_worker_available(celery_session_worker):
+    yield celery_session_worker
```

### Comparing `newrelic-9.8.0/tests/template_mako/test_mako.py` & `newrelic-9.9.0/tests/template_mako/test_mako.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/__init__.py` & `newrelic-9.9.0/tests/testing_support/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/asgi_testing.py` & `newrelic-9.9.0/tests/testing_support/asgi_testing.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/db_settings.py` & `newrelic-9.9.0/tests/testing_support/db_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/external_fixtures.py` & `newrelic-9.9.0/tests/testing_support/external_fixtures.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/fixture/__init__.py` & `newrelic-9.9.0/tests/testing_support/validators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
```

### Comparing `newrelic-9.8.0/tests/testing_support/fixture/event_loop.py` & `newrelic-9.9.0/tests/testing_support/fixture/event_loop.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/fixtures.py` & `newrelic-9.9.0/tests/testing_support/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     from queue import Queue
 
 from testing_support.sample_applications import (
     error_user_params_added,
     user_attributes_added,
 )
 
-from newrelic.api.ml_model import set_llm_token_count_callback
 from newrelic.admin.record_deploy import record_deploy
 from newrelic.api.application import (
     application_instance,
     application_settings,
     register_application,
 )
+from newrelic.api.ml_model import set_llm_token_count_callback
 from newrelic.common.agent_http import DeveloperModeClient
 from newrelic.common.encoding_utils import json_encode, obfuscate
 from newrelic.common.object_names import callable_name
 from newrelic.common.object_wrapper import (
     ObjectProxy,
     function_wrapper,
     transient_function_wrapper,
@@ -891,64 +891,14 @@
             assert expected_message == message
 
         return result
 
     return _validate_application_exception_message
 
 
-def _validate_custom_event(recorded_event, required_event):
-    assert len(recorded_event) == 2  # [intrinsic, user attributes]
-
-    intrinsics = recorded_event[0]
-
-    assert intrinsics["type"] == required_event[0]["type"]
-
-    now = time.time()
-    assert isinstance(intrinsics["timestamp"], int)
-    assert intrinsics["timestamp"] <= 1000.0 * now
-    assert intrinsics["timestamp"] >= 1000.0 * required_event[0]["timestamp"]
-
-    assert recorded_event[1].items() == required_event[1].items()
-
-
-def validate_custom_event_in_application_stats_engine(required_event):
-    @function_wrapper
-    def _validate_custom_event_in_application_stats_engine(wrapped, instance, args, kwargs):
-        try:
-            result = wrapped(*args, **kwargs)
-        except:
-            raise
-        else:
-            stats = core_application_stats_engine(None)
-            assert stats.custom_events.num_samples == 1
-
-            custom_event = next(iter(stats.custom_events))
-            _validate_custom_event(custom_event, required_event)
-
-        return result
-
-    return _validate_custom_event_in_application_stats_engine
-
-
-def validate_custom_event_count(count):
-    @function_wrapper
-    def _validate_custom_event_count(wrapped, instance, args, kwargs):
-        try:
-            result = wrapped(*args, **kwargs)
-        except:
-            raise
-        else:
-            stats = core_application_stats_engine(None)
-            assert stats.custom_events.num_samples == count, "Expected %d, got %d" % (count, stats.custom_events.num_samples)
-
-        return result
-
-    return _validate_custom_event_count
-
-
 def _validate_node_parenting(node, expected_node):
     assert node.exclusive >= 0, "node.exclusive = %s" % node.exclusive
 
     expected_children = expected_node[1]
 
     def len_error():
         return ("len(node.children)=%s, len(expected_children)=%s, node.children=%s") % (
```

### Comparing `newrelic-9.8.0/tests/testing_support/ml_testing_utils.py` & `newrelic-9.9.0/tests/testing_support/ml_testing_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/mock_external_grpc_server.py` & `newrelic-9.9.0/tests/testing_support/mock_external_grpc_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/mock_external_http_server.py` & `newrelic-9.9.0/tests/testing_support/mock_external_http_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/mock_http_client.py` & `newrelic-9.9.0/tests/testing_support/mock_http_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/sample_applications.py` & `newrelic-9.9.0/tests/testing_support/sample_applications.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/sample_asgi_applications.py` & `newrelic-9.9.0/tests/testing_support/sample_asgi_applications.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/util.py` & `newrelic-9.9.0/tests/testing_support/util.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_apdex_metrics.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_apdex_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_application_error_event_count.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_application_error_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_application_error_trace_count.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_application_error_trace_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_application_errors.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_application_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_browser_attributes.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_browser_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_code_level_metrics.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_cross_process_headers.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_cross_process_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_custom_event_collector_json.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_custom_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_custom_events.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_custom_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_custom_parameters.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_custom_parameters.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_database_duration.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_database_duration.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_database_node.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_database_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_database_trace_inputs.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_database_trace_inputs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_datastore_trace_inputs.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_datastore_trace_inputs.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_dimensional_metric_payload.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_dimensional_metric_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_dimensional_metrics_outside_transaction.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_dimensional_metrics_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_distributed_trace_accepted.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_distributed_trace_accepted.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_distributed_tracing_header.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_distributed_tracing_header.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_error_event_attributes.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_error_event_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_error_event_collector_json.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_error_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_error_trace_attributes.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_error_trace_collector_json.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_error_trace_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_external_node_params.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_external_node_params.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_function_called.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_function_called.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_internal_metrics.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_internal_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_log_event_collector_json.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_log_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_log_event_count.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_log_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_log_event_count_outside_transaction.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_log_event_count_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_log_events.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_log_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_log_events_outside_transaction.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_log_events_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_messagebroker_headers.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_messagebroker_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_metric_payload.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_metric_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_ml_event_count.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_ml_event_count_outside_transaction.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_count_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_ml_event_payload.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_ml_event_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_ml_events.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_ml_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_ml_events_outside_transaction.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_ml_events_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_non_transaction_error_event.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_non_transaction_error_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_outbound_headers.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_outbound_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_serverless_data.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_serverless_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_serverless_metadata.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_serverless_metadata.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_serverless_payload.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_serverless_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_slow_sql_collector_json.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_slow_sql_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_span_events.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_span_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
 
-import six
-
 from newrelic.common.object_wrapper import function_wrapper, transient_function_wrapper
+from newrelic.packages import six
 
 try:
     from newrelic.core.infinite_tracing_pb2 import AttributeValue, Span
 except:
     AttributeValue = None
     Span = None
 
@@ -34,26 +33,24 @@
     expected_agents=[],
     unexpected_agents=[],
     exact_users={},
     expected_users=[],
     unexpected_users=[],
     index=-1,
 ):
-
     # Used for validating a single span event.
     #
     # Since each transaction could produce multiple span events, assert that at
     # least `count` number of those span events meet the criteria, if not,
     # raises an AssertionError.
     #
     # Use this validator once per distinct span event expected.
 
     @function_wrapper
     def _validate_wrapper(wrapped, instance, args, kwargs):
-
         record_transaction_called = []
         recorded_span_events = []
 
         @transient_function_wrapper("newrelic.core.stats_engine", "StatsEngine.record_transaction")
         def capture_span_events(wrapped, instance, args, kwargs):
             events = []
```

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_sql_obfuscation.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_sql_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_synthetics_event.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_synthetics_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_synthetics_transaction_trace.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_synthetics_transaction_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_time_metrics_outside_transaction.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_time_metrics_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_transaction_count.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_transaction_error_event_count.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_error_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_transaction_error_trace_attributes.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_error_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_transaction_errors.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_transaction_event_attributes.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_event_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_transaction_event_collector_json.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_transaction_metrics.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_transaction_slow_sql_count.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_slow_sql_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_transaction_trace_attributes.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_transaction_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_tt_collector_json.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_tt_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_tt_parameters.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_tt_parameters.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tests/testing_support/validators/validate_tt_segment_params.py` & `newrelic-9.9.0/tests/testing_support/validators/validate_tt_segment_params.py`

 * *Files identical despite different names*

### Comparing `newrelic-9.8.0/tox.ini` & `newrelic-9.9.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,16 @@
     python-agent_features-{py27,py37,py38,py39,py310,py311,py312}-{with,without}_extensions,
     python-agent_features-{pypy27,pypy310}-without_extensions,
     python-agent_streaming-{py37,py38,py39,py310,py311,py312}-protobuf04-{with,without}_extensions,
     python-agent_streaming-py27-grpc0125-{with,without}_extensions,
     python-agent_streaming-py39-protobuf{03,0319}-{with,without}_extensions,
     python-agent_unittests-{py27,py37,py38,py39,py310,py311,py312}-{with,without}_extensions,
     python-agent_unittests-{pypy27,pypy310}-without_extensions,
-    python-application_celery-{py27,py37,py38,py39,py310,py311,py312,pypy27,pypy310},
+    python-application_celery-{py37,py38,py39,py310,py311,py312,pypy310}-celerylatest,
+    python-application_celery-py311-celery{0503,0502,0501},
     python-component_djangorestframework-{py37,py38,py39,py310,py311,py312}-djangorestframeworklatest,
     python-component_flask_rest-py37-flaskrestx110,
     python-component_flask_rest-{py38,py39,py310,py311,py312,pypy310}-flaskrestxlatest,
     python-component_flask_rest-{py27,pypy27}-flaskrestx051,
     python-component_graphqlserver-{py37,py38,py39,py310,py311,py312},
     python-component_tastypie-{py37,py38,py39,py310,py311,py312,pypy310}-tastypielatest,
     python-coroutines_asyncio-{py37,py38,py39,py310,py311,py312,pypy310},
@@ -110,16 +111,15 @@
     python-external_http-{py27,py37,py38,py39,py310,py311,py312,pypy27},
     python-external_httplib-{py27,py37,py38,py39,py310,py311,py312,pypy27,pypy310},
     python-external_httplib2-{py27,py37,py38,py39,py310,py311,py312,pypy27,pypy310},
     python-external_httpx-{py37,py38,py39,py310,py311,py312},
     python-external_requests-{py27,py37,py38,py39,py310,py311,py312,pypy27,pypy310},
     python-external_urllib3-{py27,py37,py38,py39,py310,py311,py312,pypy27,pypy310}-urllib3latest,
     python-external_urllib3-{py27,py37,pypy27}-urllib3{0109},
-    python-framework_aiohttp-{py37,py38,py39,py310,py311,pypy310}-aiohttp03,
-    python-framework_aiohttp-py312-aiohttp030900rc0,
+    python-framework_aiohttp-{py37,py38,py39,py310,py311,py312,pypy310}-aiohttp03,
     python-framework_ariadne-{py37,py38,py39,py310,py311,py312}-ariadnelatest,
     python-framework_ariadne-py37-ariadne{0011,0012,0013},
     python-framework_bottle-{py27,py37,py38,py39,py310,py311,py312,pypy27,pypy310}-bottle0012,
     python-framework_cherrypy-{py37,py38,py39,py310,py311,py312,pypy310}-CherryPylatest,
     python-framework_django-{py37,py38,py39,py310,py311,py312}-Djangolatest,
     python-framework_django-{py39}-Django{0202,0300,0301,0302,0401},
     python-framework_falcon-{py37,py312}-falcon0300,
@@ -160,15 +160,16 @@
     redis-datastore_redis-{py37,py38,py39,py310,py311,py312,pypy310}-redis{0400,latest},
     rediscluster-datastore_rediscluster-{py37,py311,py312,pypy310}-redislatest,
     solr-datastore_pysolr-{py27,py37,py38,py39,py310,py311,py312,pypy27,pypy310},
 
 [testenv]
 deps =
     # Base Dependencies
-    {py37,py38,py39,py310,py311,py312,pypy310}: pytest==7.2.2
+    {py38,py39,py310,py311,py312,pypy310}: pytest==8.1.1
+    py37: pytest==7.4.4
     {py27,pypy27}: pytest==4.6.11
     iniconfig
     coverage
     WebTest==2.0.35
 
     # Test Suite Dependencies
     adapter_asgiref-asgireflatest: asgiref
@@ -197,15 +198,18 @@
     adapter_uvicorn: typing-extensions
     adapter_waitress: WSGIProxy2
     adapter_waitress-waitress02: waitress<2.1
     adapter_waitress-waitresslatest: waitress
     agent_features: beautifulsoup4
     agent_features-{py37,py38,py39,py310,py311,py312,pypy310}: protobuf
     agent_features-{py27,pypy27}: protobuf<3.18.0
-    application_celery: celery<6.0
+    application_celery-celerylatest: celery[pytest]
+    application_celery-celery0503: celery[pytest]<5.4
+    application_celery-celery0502: celery[pytest]<5.3
+    application_celery-celery0501: celery[pytest]<5.2
     application_celery-{py37,pypy310}: importlib-metadata<5.0
     mlmodel_sklearn: pandas
     mlmodel_sklearn: protobuf
     mlmodel_sklearn: numpy
     mlmodel_sklearn-scikitlearnlatest: scikit-learn
     mlmodel_sklearn-scikitlearnlatest: scipy
     mlmodel_sklearn-scikitlearn0101: scikit-learn<1.1
```

