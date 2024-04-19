# Comparing `tmp/qbraid_cli-0.8.dev4.tar.gz` & `tmp/qbraid_cli-0.8.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid_cli-0.8.dev4.tar", last modified: Fri Apr 12 21:20:55 2024, max compression
+gzip compressed data, was "qbraid_cli-0.8.0.dev5.tar", last modified: Fri Apr 19 21:53:52 2024, max compression
```

## Comparing `qbraid_cli-0.8.dev4.tar` & `qbraid_cli-0.8.0.dev5.tar`

### file list

```diff
@@ -1,160 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.153820 qbraid_cli-0.8.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.125820 qbraid_cli-0.8.dev4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.125820 qbraid_cli-0.8.dev4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.129819 qbraid_cli-0.8.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/MANIFEST.IN
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-12 21:20:55.153820 qbraid_cli-0.8.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.129819 qbraid_cli-0.8.dev4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.129819 qbraid_cli-0.8.dev4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    30522 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.129819 qbraid_cli-0.8.dev4/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.129819 qbraid_cli-0.8.dev4/docs/_static/style/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/style/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/style/s4defs-roles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.133819 qbraid_cli-0.8.dev4/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/configure.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/devices-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/envs-activate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/envs-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/envs-uninstall.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/envs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/jobs-add.rst
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/jobs-disable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/jobs-enable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/jobs-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/kernels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.133819 qbraid_cli-0.8.dev4/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/guide/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.133819 qbraid_cli-0.8.dev4/qbraid_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 21:20:54.000000 qbraid_cli-0.8.dev4/qbraid_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.137820 qbraid_cli-0.8.dev4/qbraid_cli/configure/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/configure/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/configure/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.137820 qbraid_cli-0.8.dev4/qbraid_cli/credits/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/credits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/credits/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.137820 qbraid_cli-0.8.dev4/qbraid_cli/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/devices/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/devices/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.137820 qbraid_cli-0.8.dev4/qbraid_cli/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/envs/activate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/envs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/envs/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/envs/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/qbraid_cli/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/jobs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/jobs/toggle_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/jobs/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/qbraid_cli/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/kernels/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.149820 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:20:55.153820 qbraid_cli-0.8.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/test_configure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_configure/test_configure_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_configure/test_prompt_for_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_configure/test_validate_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/test_credits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_credits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_credits/test_credits_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/test_devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_devices/test_devices_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_devices/test_validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/test_envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/test_envs/test_activate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_activate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_activate_pyenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_find_shell_rc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_print_activate_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.145820 qbraid_cli-0.8.dev4/tests/test_envs/test_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.145820 qbraid_cli-0.8.dev4/tests/test_envs/test_create/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_create_qbraid_env_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_replace_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_update_state_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.145820 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_installed_envs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_is_valid_env_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_request_delete_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_validate_env_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.145820 qbraid_cli-0.8.dev4/tests/test_jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.145820 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_disable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.149820 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_aws_configure_dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_confirm_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_disable_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_enable_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_get_package_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.149820 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_get_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_handle_jobs_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_run_progress_get_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_validate_library.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.149820 qbraid_cli-0.8.dev4/tests/test_kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_kernels/test_kernels_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.149820 qbraid_cli-0.8.dev4/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tools/split_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.559953 qbraid_cli-0.8.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.535953 qbraid_cli-0.8.0.dev5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.535953 qbraid_cli-0.8.0.dev5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.535953 qbraid_cli-0.8.0.dev5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/MANIFEST.IN
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-19 21:53:52.559953 qbraid_cli-0.8.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.539953 qbraid_cli-0.8.0.dev5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.539953 qbraid_cli-0.8.0.dev5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    30522 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/_static/api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.539953 qbraid_cli-0.8.0.dev5/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.539953 qbraid_cli-0.8.0.dev5/docs/_static/style/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/_static/style/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/_static/style/s4defs-roles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.543953 qbraid_cli-0.8.0.dev5/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/configure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/devices-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/envs-activate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/envs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/envs-uninstall.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/envs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/jobs-add.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/jobs-disable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/jobs-enable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/jobs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/kernels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/cli/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.543953 qbraid_cli-0.8.0.dev5/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/guide/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.543953 qbraid_cli-0.8.0.dev5/qbraid_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-19 21:53:52.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.547953 qbraid_cli-0.8.0.dev5/qbraid_cli/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/admin/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/admin/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/admin/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.547953 qbraid_cli-0.8.0.dev5/qbraid_cli/configure/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/configure/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/configure/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.547953 qbraid_cli-0.8.0.dev5/qbraid_cli/credits/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/credits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/credits/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.547953 qbraid_cli-0.8.0.dev5/qbraid_cli/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/devices/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/devices/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.547953 qbraid_cli-0.8.0.dev5/qbraid_cli/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/envs/activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/envs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/envs/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/envs/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.547953 qbraid_cli-0.8.0.dev5/qbraid_cli/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/jobs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/jobs/toggle_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/jobs/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.551953 qbraid_cli-0.8.0.dev5/qbraid_cli/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/kernels/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/qbraid_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.559953 qbraid_cli-0.8.0.dev5/qbraid_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-19 21:53:52.000000 qbraid_cli-0.8.0.dev5/qbraid_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-19 21:53:52.000000 qbraid_cli-0.8.0.dev5/qbraid_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:53:52.000000 qbraid_cli-0.8.0.dev5/qbraid_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 21:53:52.000000 qbraid_cli-0.8.0.dev5/qbraid_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-19 21:53:52.000000 qbraid_cli-0.8.0.dev5/qbraid_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 21:53:52.000000 qbraid_cli-0.8.0.dev5/qbraid_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:53:52.559953 qbraid_cli-0.8.0.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.551953 qbraid_cli-0.8.0.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.551953 qbraid_cli-0.8.0.dev5/tests/test_configure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_configure/test_configure_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_configure/test_prompt_for_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_configure/test_validate_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.551953 qbraid_cli-0.8.0.dev5/tests/test_credits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_credits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_credits/test_credits_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.551953 qbraid_cli-0.8.0.dev5/tests/test_devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_devices/test_devices_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_devices/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.551953 qbraid_cli-0.8.0.dev5/tests/test_envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.551953 qbraid_cli-0.8.0.dev5/tests/test_envs/test_activate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_activate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_activate/test_activate_pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_activate/test_find_shell_rc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_activate/test_print_activate_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.551953 qbraid_cli-0.8.0.dev5/tests/test_envs/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_app/test_envs_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_app/test_envs_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_app/test_envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_app/test_envs_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.555953 qbraid_cli-0.8.0.dev5/tests/test_envs/test_create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_create/test_create_qbraid_env_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_create/test_replace_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_create/test_update_state_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.555953 qbraid_cli-0.8.0.dev5/tests/test_envs/test_data_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_data_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_data_handling/test_installed_envs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_data_handling/test_is_valid_env_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_data_handling/test_request_delete_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_envs/test_data_handling/test_validate_env_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.555953 qbraid_cli-0.8.0.dev5/tests/test_jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.555953 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_app/test_jobs_disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_app/test_jobs_enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_app/test_jobs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_app/test_jobs_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.555953 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_toggle_braket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_toggle_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_toggle_braket/test_confirm_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_toggle_braket/test_disable_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_toggle_braket/test_enable_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_toggle_braket/test_get_package_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.559953 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_validation/test_get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_validation/test_handle_jobs_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_validation/test_run_progress_get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_jobs/test_validation/test_validate_library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.559953 qbraid_cli-0.8.0.dev5/tests/test_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tests/test_kernels/test_kernels_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:53:52.559953 qbraid_cli-0.8.0.dev5/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tools/split_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-19 21:53:47.000000 qbraid_cli-0.8.0.dev5/tools/verify_headers.py
```

### Comparing `qbraid_cli-0.8.dev4/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid_cli-0.8.0.dev5/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid_cli-0.8.0.dev5/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/.github/workflows/docs.yml` & `qbraid_cli-0.8.0.dev5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/.github/workflows/format.yml` & `qbraid_cli-0.8.0.dev5/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/.github/workflows/main.yml` & `qbraid_cli-0.8.0.dev5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/.github/workflows/publish.yml` & `qbraid_cli-0.8.0.dev5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/.github/workflows/test-publish.yml` & `qbraid_cli-0.8.0.dev5/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/.gitignore` & `qbraid_cli-0.8.0.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/.readthedocs.yml` & `qbraid_cli-0.8.0.dev5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/CONTRIBUTING.md` & `qbraid_cli-0.8.0.dev5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/Makefile` & `qbraid_cli-0.8.0.dev5/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/PKG-INFO` & `qbraid_cli-0.8.0.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-cli
-Version: 0.8.0.dev4
+Version: 0.8.0.dev5
 Summary: Command Line Interface for interacting with all parts of the qBraid platform.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -25,26 +25,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.12.1
 Requires-Dist: rich>=10.11.0
 Requires-Dist: jupyter_client<9.0.0,>=7.0.0
-Requires-Dist: qbraid-core>=0.1.2
+Requires-Dist: ipykernel
+Requires-Dist: qbraid-core>=0.1.3
 Provides-Extra: jobs
 Requires-Dist: amazon-braket-sdk>=1.48.1; extra == "jobs"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
-Requires-Dist: docutils<0.21; extra == "docs"
+Requires-Dist: docutils<0.22; extra == "docs"
 Requires-Dist: toml; extra == "docs"
 Requires-Dist: build; extra == "docs"
 Requires-Dist: m2r; extra == "docs"
 Requires-Dist: typer; extra == "docs"
 
 <img width="full" alt="qbraid_cli" src="https://qbraid-static.s3.amazonaws.com/logos/qbraid-cli-banner.png">
```

### Comparing `qbraid_cli-0.8.dev4/README.md` & `qbraid_cli-0.8.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/Makefile` & `qbraid_cli-0.8.0.dev5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/_static/api-key.png` & `qbraid_cli-0.8.0.dev5/docs/_static/api-key.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/_static/cards/jupyter.png` & `qbraid_cli-0.8.0.dev5/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/_static/cards/python.png` & `qbraid_cli-0.8.0.dev5/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/_static/cards/terminal.png` & `qbraid_cli-0.8.0.dev5/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/_static/favicon.ico` & `qbraid_cli-0.8.0.dev5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/_static/logo.png` & `qbraid_cli-0.8.0.dev5/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/_static/style/custom.css` & `qbraid_cli-0.8.0.dev5/docs/_static/style/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/_static/style/s4defs-roles.css` & `qbraid_cli-0.8.0.dev5/docs/_static/style/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/configure.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/configure.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/devices-list.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/devices-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/envs-activate.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/envs-activate.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/envs-list.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/envs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/envs-uninstall.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/envs-uninstall.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/envs.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/envs.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/jobs-add.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/jobs-add.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/jobs-disable.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/jobs-disable.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/jobs-enable.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/jobs-enable.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/jobs-list.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/jobs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/jobs.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/kernels.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/kernels.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/cli/qbraid.rst` & `qbraid_cli-0.8.0.dev5/docs/cli/qbraid.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/conf.py` & `qbraid_cli-0.8.0.dev5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/guide/overview.rst` & `qbraid_cli-0.8.0.dev5/docs/guide/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/docs/index.rst` & `qbraid_cli-0.8.0.dev5/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -99,13 +99,14 @@
 
 .. toctree::
    :maxdepth: 1
    :caption: CLI API Reference
    :hidden:
 
    tree/qbraid
+   tree/qbraid_admin
    tree/qbraid_configure
    tree/qbraid_credits
    tree/qbraid_devices
    tree/qbraid_envs
    tree/qbraid_jobs
-   tree/qbraid_kernels
+   tree/qbraid_kernels
```

#### html2text {}

```diff
@@ -5,9 +5,9 @@
 _[_t_e_r_m_i_n_a_l_]
 _**_**_**_**_ _CC_LL_II_ _**_**_**_**
 _[_t_e_r_m_i_n_a_l_]
 _**_**_**_**_ _SS_DD_KK_ _**_**_**_**
 _[_t_e_r_m_i_n_a_l_]
 | .. toctree:: :maxdepth: 1 :caption: CLI User Guide :hidden: guide/overview ..
 toctree:: :maxdepth: 1 :caption: CLI API Reference :hidden: tree/qbraid tree/
-qbraid_configure tree/qbraid_credits tree/qbraid_devices tree/qbraid_envs tree/
-qbraid_jobs tree/qbraid_kernels
+qbraid_admin tree/qbraid_configure tree/qbraid_credits tree/qbraid_devices
+tree/qbraid_envs tree/qbraid_jobs tree/qbraid_kernels
```

### Comparing `qbraid_cli-0.8.dev4/docs/make.bat` & `qbraid_cli-0.8.0.dev5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/pyproject.toml` & `qbraid_cli-0.8.0.dev5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-cli"
-version = "0.8.0.dev4"
+version = "0.8.0.dev5"
 description = "Command Line Interface for interacting with all parts of the qBraid platform."
 readme = "README.md"
 authors = [{ name = "qBraid Development Team", email = "contact@qbraid.com" }]
 license = { text = "Proprietary" }
 keywords = ["qbraid", "cli", "quantum", "cloud"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -26,29 +26,30 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "typer>=0.12.1",
     "rich>=10.11.0",
     "jupyter_client>=7.0.0,<9.0.0",
-    "qbraid-core>=0.1.2",
+    "ipykernel",
+    "qbraid-core>=0.1.3",
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://www.qbraid.com/"
 Documentation = "https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html"
 "Bug Tracker" = "https://github.com/qBraid/qBraid-Lab/issues"
 Discord = "https://discord.gg/KugF6Cnncm"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git"
 
 [project.optional-dependencies]
 jobs = ["amazon-braket-sdk>=1.48.1"]
 dev = ["black", "isort", "pylint", "pytest"]
-docs = ["sphinx~=7.2.6", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.21", "toml", "build", "m2r", "typer"]
+docs = ["sphinx~=7.2.6", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.22", "toml", "build", "m2r", "typer"]
 
 [project.scripts]
 qbraid = "qbraid_cli.main:app"
 
 [tool.setuptools_scm]
 write_to = "qbraid_cli/_version.py"
```

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/configure/actions.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/configure/actions.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/configure/app.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/configure/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/credits/app.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/credits/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/devices/app.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/devices/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/devices/validation.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/devices/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
 Module for validating command arguments for qBraid devices commands.
 
-
 """
 
 from typing import Optional, Union
 
 from qbraid_cli.handlers import validate_item
```

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/envs/activate.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/envs/activate.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/envs/app.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/envs/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/envs/create.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/envs/create.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/envs/data_handling.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/envs/data_handling.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/exceptions.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/handlers.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/handlers.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/jobs/app.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/jobs/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/jobs/toggle_braket.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/jobs/toggle_braket.py`

 * *Files 23% similar despite different names*

```diff
@@ -116,40 +116,19 @@
         raise typer.Exit()
 
 
 def aws_configure_dummy() -> None:
     """
     Initializes AWS configuration and credentials files with placeholder values.
 
-    This function ensures the existence of AWS config and credentials files in the user's home
-    directory. If these files do not already exist, it creates them and populates them with
-    placeholder values for the AWS access key and secret access key. While AWS credentials are not
-    required when submitting quantum tasks through qBraid, Amazon Braket requires these files to be
-    present to prevent configuration errors.
     """
-    aws_dir = Path.home() / ".aws"
-    config_path = aws_dir / "config"
-    credentials_path = aws_dir / "credentials"
-
-    def configure_aws():
-        aws_dir.mkdir(exist_ok=True)
-        if not config_path.exists():
-            config_content = "[default]\nregion = us-east-1\noutput = json\n"
-            config_path.write_text(config_content)
-        if not credentials_path.exists():
-            access_key, secret_key = "MYACCESSKEY", "MYSECRETKEY"
-            credentials_content = (
-                f"[default]\n"
-                f"aws_access_key_id = {access_key}\n"
-                f"aws_secret_access_key = {secret_key}\n"
-            )
-            credentials_path.write_text(credentials_content)
+    from qbraid_core.services.quantum.proxy_braket import aws_configure
 
     try:
-        handle_filesystem_operation(configure_aws, aws_dir)
+        handle_filesystem_operation(aws_configure, Path.home() / ".aws")
     except QbraidException:
         handle_error(message="Failed to configure qBraid quantum jobs.")
 
 
 def enable_braket(auto_confirm: bool = False):
     """Enable qBraid quantum jobs for Amazon Braket."""
     installed, latest, path, python_exe = run_progress_task(
```

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/jobs/validation.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/jobs/validation.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/kernels/app.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/kernels/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli/main.py` & `qbraid_cli-0.8.0.dev5/qbraid_cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 
 """
 Entrypoint for the qBraid CLI.
 
 """
 
 import typer
-import urllib3
 
+from qbraid_cli.admin.app import admin_app
 from qbraid_cli.configure.app import configure_app
 from qbraid_cli.credits.app import credits_app
 from qbraid_cli.devices.app import devices_app
 from qbraid_cli.envs.app import envs_app
 from qbraid_cli.jobs.app import jobs_app
 from qbraid_cli.kernels.app import kernels_app
 
 app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
+
+app.add_typer(admin_app, name="admin")
 app.add_typer(configure_app, name="configure")
+app.add_typer(credits_app, name="credits")
+app.add_typer(devices_app, name="devices")
 app.add_typer(envs_app, name="envs")
 app.add_typer(jobs_app, name="jobs")
-app.add_typer(devices_app, name="devices")
 app.add_typer(kernels_app, name="kernels")
-app.add_typer(credits_app, name="credits")
-
-urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def version_callback(value: bool):
     """Show the version and exit."""
     if value:
         from ._version import __version__
```

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli.egg-info/PKG-INFO` & `qbraid_cli-0.8.0.dev5/qbraid_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-cli
-Version: 0.8.0.dev4
+Version: 0.8.0.dev5
 Summary: Command Line Interface for interacting with all parts of the qBraid platform.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -25,26 +25,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.12.1
 Requires-Dist: rich>=10.11.0
 Requires-Dist: jupyter_client<9.0.0,>=7.0.0
-Requires-Dist: qbraid-core>=0.1.2
+Requires-Dist: ipykernel
+Requires-Dist: qbraid-core>=0.1.3
 Provides-Extra: jobs
 Requires-Dist: amazon-braket-sdk>=1.48.1; extra == "jobs"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
-Requires-Dist: docutils<0.21; extra == "docs"
+Requires-Dist: docutils<0.22; extra == "docs"
 Requires-Dist: toml; extra == "docs"
 Requires-Dist: build; extra == "docs"
 Requires-Dist: m2r; extra == "docs"
 Requires-Dist: typer; extra == "docs"
 
 <img width="full" alt="qbraid_cli" src="https://qbraid-static.s3.amazonaws.com/logos/qbraid-cli-banner.png">
```

### Comparing `qbraid_cli-0.8.dev4/qbraid_cli.egg-info/SOURCES.txt` & `qbraid_cli-0.8.0.dev5/qbraid_cli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 qbraid_cli/main.py
 qbraid_cli.egg-info/PKG-INFO
 qbraid_cli.egg-info/SOURCES.txt
 qbraid_cli.egg-info/dependency_links.txt
 qbraid_cli.egg-info/entry_points.txt
 qbraid_cli.egg-info/requires.txt
 qbraid_cli.egg-info/top_level.txt
+qbraid_cli/admin/__init__.py
+qbraid_cli/admin/app.py
+qbraid_cli/admin/headers.py
+qbraid_cli/admin/validation.py
 qbraid_cli/configure/__init__.py
 qbraid_cli/configure/actions.py
 qbraid_cli/configure/app.py
 qbraid_cli/credits/__init__.py
 qbraid_cli/credits/app.py
 qbraid_cli/devices/__init__.py
 qbraid_cli/devices/app.py
@@ -105,15 +109,14 @@
 tests/test_jobs/__init__.py
 tests/test_jobs/test_app/__init__.py
 tests/test_jobs/test_app/test_jobs_disable.py
 tests/test_jobs/test_app/test_jobs_enable.py
 tests/test_jobs/test_app/test_jobs_list.py
 tests/test_jobs/test_app/test_jobs_state.py
 tests/test_jobs/test_toggle_braket/__init__.py
-tests/test_jobs/test_toggle_braket/test_aws_configure_dummy.py
 tests/test_jobs/test_toggle_braket/test_confirm_updates.py
 tests/test_jobs/test_toggle_braket/test_disable_braket.py
 tests/test_jobs/test_toggle_braket/test_enable_braket.py
 tests/test_jobs/test_toggle_braket/test_get_package_data.py
 tests/test_jobs/test_validation/__init__.py
 tests/test_jobs/test_validation/test_get_state.py
 tests/test_jobs/test_validation/test_handle_jobs_state.py
```

### Comparing `qbraid_cli-0.8.dev4/tests/test_configure/test_configure_set.py` & `qbraid_cli-0.8.0.dev5/tests/test_configure/test_configure_set.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_configure/test_prompt_for_config.py` & `qbraid_cli-0.8.0.dev5/tests/test_configure/test_prompt_for_config.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_configure/test_validate_input.py` & `qbraid_cli-0.8.0.dev5/tests/test_configure/test_validate_input.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_credits/test_credits_value.py` & `qbraid_cli-0.8.0.dev5/tests/test_credits/test_credits_value.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_devices/test_devices_list.py` & `qbraid_cli-0.8.0.dev5/tests/test_devices/test_devices_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_devices/test_validations.py` & `qbraid_cli-0.8.0.dev5/tests/test_devices/test_validations.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_activate_pyenv.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_activate/test_activate_pyenv.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_find_shell_rc.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_activate/test_find_shell_rc.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_print_activate_command.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_activate/test_print_activate_command.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_activate.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_app/test_envs_activate.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_create.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_app/test_envs_create.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_list.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_app/test_envs_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_remove.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_app/test_envs_remove.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_create_qbraid_env_assets.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_create/test_create_qbraid_env_assets.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_replace_str.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_create/test_replace_str.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_update_state_json.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_create/test_update_state_json.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_installed_envs_data.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_data_handling/test_installed_envs_data.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_is_valid_env_name.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_data_handling/test_is_valid_env_name.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_request_delete_env.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_data_handling/test_request_delete_env.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_validate_env_name.py` & `qbraid_cli-0.8.0.dev5/tests/test_envs/test_data_handling/test_validate_env_name.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_disable.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_app/test_jobs_disable.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_enable.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_app/test_jobs_enable.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_list.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_app/test_jobs_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_state.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_app/test_jobs_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_confirm_updates.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_toggle_braket/test_confirm_updates.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_disable_braket.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_toggle_braket/test_disable_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_enable_braket.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_toggle_braket/test_enable_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_get_package_data.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_toggle_braket/test_get_package_data.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_get_state.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_validation/test_get_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_handle_jobs_state.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_validation/test_handle_jobs_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_run_progress_get_state.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_validation/test_run_progress_get_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_validate_library.py` & `qbraid_cli-0.8.0.dev5/tests/test_jobs/test_validation/test_validate_library.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tests/test_kernels/test_kernels_list.py` & `qbraid_cli-0.8.0.dev5/tests/test_kernels/test_kernels_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tools/split_rst.py` & `qbraid_cli-0.8.0.dev5/tools/split_rst.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.dev4/tools/verify_headers.py` & `qbraid_cli-0.8.0.dev5/tools/verify_headers.py`

 * *Files identical despite different names*

