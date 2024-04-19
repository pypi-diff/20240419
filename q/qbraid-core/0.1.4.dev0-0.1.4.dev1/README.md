# Comparing `tmp/qbraid_core-0.1.4.dev0.tar.gz` & `tmp/qbraid_core-0.1.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid_core-0.1.4.dev0.tar", last modified: Thu Apr 18 16:28:50 2024, max compression
+gzip compressed data, was "qbraid_core-0.1.4.dev1.tar", last modified: Fri Apr 19 19:46:16 2024, max compression
```

## Comparing `qbraid_core-0.1.4.dev0.tar` & `qbraid_core-0.1.4.dev1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.525451 qbraid_core-0.1.4.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.509451 qbraid_core-0.1.4.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.509451 qbraid_core-0.1.4.dev0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-18 16:28:50.525451 qbraid_core-0.1.4.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.513451 qbraid_core-0.1.4.dev0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.517451 qbraid_core-0.1.4.dev0/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.517451 qbraid_core-0.1.4.dev0/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.517451 qbraid_core-0.1.4.dev0/qbraid_core/services/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/admin/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.517451 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.517451 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/proxy_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/qbraid_core/system/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.525451 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 16:28:50.000000 qbraid_core-0.1.4.dev0/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:28:50.525451 qbraid_core-0.1.4.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/environments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/environments/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/environments/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/quantum/test_aws_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/quantum/test_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/system/
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/system/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/system/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/system/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/system/test_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.521451 qbraid_core-0.1.4.dev0/tests/top_level/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/top_level/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/top_level/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/top_level/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tests/top_level/test_sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:28:50.525451 qbraid_core-0.1.4.dev0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-18 16:28:46.000000 qbraid_core-0.1.4.dev0/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.931794 qbraid_core-0.1.4.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.915794 qbraid_core-0.1.4.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.915794 qbraid_core-0.1.4.dev1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.915794 qbraid_core-0.1.4.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-19 19:46:16.931794 qbraid_core-0.1.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.919793 qbraid_core-0.1.4.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.919793 qbraid_core-0.1.4.dev1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.919793 qbraid_core-0.1.4.dev1/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.919793 qbraid_core-0.1.4.dev1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.919793 qbraid_core-0.1.4.dev1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/services/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/admin/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/proxy_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:46:16.931794 qbraid_core-0.1.4.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tests/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tests/environments/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tests/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/quantum/test_aws_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/quantum/test_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/system/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/system/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/system/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/system/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tests/top_level/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/top_level/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/top_level/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/top_level/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/top_level/test_sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tools/verify_headers.py
```

### Comparing `qbraid_core-0.1.4.dev0/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid_core-0.1.4.dev1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid_core-0.1.4.dev1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/.github/workflows/docs.yml` & `qbraid_core-0.1.4.dev1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/.github/workflows/format.yml` & `qbraid_core-0.1.4.dev1/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/.github/workflows/main.yml` & `qbraid_core-0.1.4.dev1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/.github/workflows/publish.yml` & `qbraid_core-0.1.4.dev1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/.github/workflows/test-publish.yml` & `qbraid_core-0.1.4.dev1/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/.gitignore` & `qbraid_core-0.1.4.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/LICENSE` & `qbraid_core-0.1.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/PKG-INFO` & `qbraid_core-0.1.4.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.4.dev0
+Version: 0.1.4.dev1
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid_core-0.1.4.dev0/README.md` & `qbraid_core-0.1.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/Makefile` & `qbraid_core-0.1.4.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/_static/cards/jupyter.png` & `qbraid_core-0.1.4.dev1/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/_static/cards/python.png` & `qbraid_core-0.1.4.dev1/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/_static/cards/terminal.png` & `qbraid_core-0.1.4.dev1/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/_static/css/custom.css` & `qbraid_core-0.1.4.dev1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/_static/css/s4defs-roles.css` & `qbraid_core-0.1.4.dev1/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/_static/favicon.ico` & `qbraid_core-0.1.4.dev1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/_static/logo.png` & `qbraid_core-0.1.4.dev1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/conf.py` & `qbraid_core-0.1.4.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/index.rst` & `qbraid_core-0.1.4.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/docs/make.bat` & `qbraid_core-0.1.4.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/pyproject.toml` & `qbraid_core-0.1.4.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.4.dev0"
+version = "0.1.4.dev1"
 authors = [
     {name = "qBraid Development Team", email = "contact@qbraid.com"},
 ]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["qbraid", "quantum", "cloud"]
@@ -60,8 +60,8 @@
 [tool.pylint.MASTER]
 ignore-paths = [
   "^.*\\_version.py$",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-ra"
-testpaths = ["tests"]
+testpaths = ["tests"]
```

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/__init__.py` & `qbraid_core-0.1.4.dev1/qbraid_core/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/_compat.py` & `qbraid_core-0.1.4.dev1/qbraid_core/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/client.py` & `qbraid_core-0.1.4.dev1/qbraid_core/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/config.py` & `qbraid_core-0.1.4.dev1/qbraid_core/config.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/exceptions.py` & `qbraid_core-0.1.4.dev1/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/registry.py` & `qbraid_core-0.1.4.dev1/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/retry.py` & `qbraid_core-0.1.4.dev1/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/admin/client.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/admin/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/__init__.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/client.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/create.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/paths.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/paths.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/state.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/environments/validate.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/__init__.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/adapter.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/client.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/proxy.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/services/quantum/proxy_braket.py` & `qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/proxy_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/sessions.py` & `qbraid_core-0.1.4.dev1/qbraid_core/sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/system/__init__.py` & `qbraid_core-0.1.4.dev1/qbraid_core/system/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/system/exceptions.py` & `qbraid_core-0.1.4.dev1/qbraid_core/system/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/system/executables.py` & `qbraid_core-0.1.4.dev1/qbraid_core/system/executables.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/system/generic.py` & `qbraid_core-0.1.4.dev1/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/system/packages.py` & `qbraid_core-0.1.4.dev1/qbraid_core/system/packages.py`

 * *Files 16% similar despite different names*

```diff
@@ -180,7 +180,57 @@
         ) from err
 
     if len(all_versions) == 0:
         raise VersionNotFoundError(f"No versions found for {package}")
 
     latest_version = all_versions[-1]
     return latest_version
+
+
+def extract_include_sys_site_pkgs_value(file_path: Union[str, Path]) -> Optional[bool]:
+    """Extracts the value of the 'include-system-site-packages' setting from a file."""
+    try:
+        with open(file_path, "r", encoding="utf-8") as file:
+            for line in file:
+                if line.startswith("include-system-site-packages"):
+                    parts = line.strip().split("=")
+                    if len(parts) == 2:
+                        value = parts[1].strip().lower()
+                        if value == "true":
+                            return True
+                        if value == "false":
+                            return False
+                    break
+    except FileNotFoundError as err:
+        raise FileNotFoundError("The specified file was not found.") from err
+    except Exception as err:
+        raise QbraidSystemError("An error occurred while reading the file.") from err
+
+    return None
+
+
+def set_include_sys_site_pkgs_value(value: bool, file_path: Union[str, Path]) -> None:
+    """Sets the value of the 'include-system-site-packages' setting in a file."""
+    try:
+        with open(file_path, "r", encoding="utf-8") as file:
+            lines = file.readlines()
+
+        # Track whether the target line was found
+        found = False
+        for i, line in enumerate(lines):
+            if line.startswith("include-system-site-packages"):
+                lines[i] = f"include-system-site-packages = {str(value).lower()}\n"
+                found = True
+                break
+
+        if not found:
+            raise ValueError(
+                "The 'include-system-site-packages' setting was not found in the file."
+            )
+
+        with open(file_path, "w", encoding="utf-8") as file:
+            file.writelines(lines)
+
+    except FileNotFoundError as err:
+        raise FileNotFoundError("The specified file was not found.") from err
+    except Exception as err:
+        raise QbraidSystemError("An error occurred while updating the file") from err
```

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/system/threader.py` & `qbraid_core-0.1.4.dev1/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core/system/versions.py` & `qbraid_core-0.1.4.dev1/qbraid_core/system/versions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core.egg-info/PKG-INFO` & `qbraid_core-0.1.4.dev1/qbraid_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.4.dev0
+Version: 0.1.4.dev1
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid_core-0.1.4.dev0/qbraid_core.egg-info/SOURCES.txt` & `qbraid_core-0.1.4.dev1/qbraid_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/environments/fixtures/environments.py` & `qbraid_core-0.1.4.dev1/tests/environments/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/environments/test_client.py` & `qbraid_core-0.1.4.dev1/tests/environments/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/environments/test_create.py` & `qbraid_core-0.1.4.dev1/tests/environments/test_create.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/environments/test_paths.py` & `qbraid_core-0.1.4.dev1/tests/environments/test_paths.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/environments/test_state.py` & `qbraid_core-0.1.4.dev1/tests/environments/test_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/environments/test_validate.py` & `qbraid_core-0.1.4.dev1/tests/environments/test_validate.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/quantum/test_aws_configure.py` & `qbraid_core-0.1.4.dev1/tests/quantum/test_aws_configure.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/quantum/test_proxy.py` & `qbraid_core-0.1.4.dev1/tests/quantum/test_proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/system/test_executables.py` & `qbraid_core-0.1.4.dev1/tests/system/test_executables.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/system/test_generic.py` & `qbraid_core-0.1.4.dev1/tests/system/test_generic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/system/test_versions.py` & `qbraid_core-0.1.4.dev1/tests/system/test_versions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/top_level/test_client.py` & `qbraid_core-0.1.4.dev1/tests/top_level/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/top_level/test_compat.py` & `qbraid_core-0.1.4.dev1/tests/top_level/test_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/top_level/test_config.py` & `qbraid_core-0.1.4.dev1/tests/top_level/test_config.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tests/top_level/test_sessions.py` & `qbraid_core-0.1.4.dev1/tests/top_level/test_sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev0/tools/verify_headers.py` & `qbraid_core-0.1.4.dev1/tools/verify_headers.py`

 * *Files identical despite different names*

