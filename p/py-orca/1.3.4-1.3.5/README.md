# Comparing `tmp/py-orca-1.3.4.tar.gz` & `tmp/py_orca-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-orca-1.3.4.tar", last modified: Mon Mar  4 13:50:26 2024, max compression
+gzip compressed data, was "py_orca-1.3.5.tar", last modified: Fri Apr 19 02:05:47 2024, max compression
```

## Comparing `py-orca-1.3.4.tar` & `py_orca-1.3.5.tar`

### file list

```diff
@@ -1,127 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.287237 py-orca-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-04 13:49:38.000000 py-orca-1.3.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-03-04 13:49:38.000000 py-orca-1.3.4/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.271237 py-orca-1.3.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-04 13:49:38.000000 py-orca-1.3.4/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.271237 py-orca-1.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-03-04 13:49:38.000000 py-orca-1.3.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-04 13:49:38.000000 py-orca-1.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-04 13:49:38.000000 py-orca-1.3.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-04 13:49:38.000000 py-orca-1.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-04 13:49:38.000000 py-orca-1.3.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-04 13:49:38.000000 py-orca-1.3.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-04 13:49:38.000000 py-orca-1.3.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-03-04 13:49:38.000000 py-orca-1.3.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-04 13:49:38.000000 py-orca-1.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-03-04 13:50:26.287237 py-orca-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-04 13:49:38.000000 py-orca-1.3.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)   425961 2024-03-04 13:49:38.000000 py-orca-1.3.4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-04 13:49:38.000000 py-orca-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-03-04 13:49:38.000000 py-orca-1.3.4/demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      669 2024-03-04 13:49:38.000000 py-orca-1.3.4/dev_setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.271237 py-orca-1.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-04 13:49:38.000000 py-orca-1.3.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.271237 py-orca-1.3.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-04 13:49:38.000000 py-orca-1.3.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-04 13:49:38.000000 py-orca-1.3.4/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-04 13:49:38.000000 py-orca-1.3.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-03-04 13:49:38.000000 py-orca-1.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-04 13:49:38.000000 py-orca-1.3.4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-04 13:49:38.000000 py-orca-1.3.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-04 13:49:38.000000 py-orca-1.3.4/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-04 13:49:38.000000 py-orca-1.3.4/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-04 13:49:38.000000 py-orca-1.3.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-04 13:49:38.000000 py-orca-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-04 13:49:38.000000 py-orca-1.3.4/requirements-airflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-04 13:50:26.291236 py-orca-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-04 13:49:38.000000 py-orca-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.263237 py-orca-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.271237 py-orca-1.3.4/src/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/docker/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.271237 py-orca-1.3.4/src/orca/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.275236 py-orca-1.3.4/src/orca/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/airflow/provider_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.275236 py-orca-1.3.4/src/orca/services/
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.275236 py-orca-1.3.4/src/orca/services/base/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/base/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/base/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/base/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.275236 py-orca-1.3.4/src/orca/services/nextflowtower/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/nextflowtower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/nextflowtower/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/nextflowtower/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/nextflowtower/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/nextflowtower/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/nextflowtower/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11134 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/nextflowtower/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/nextflowtower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.275236 py-orca-1.3.4/src/orca/services/sevenbridges/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/sevenbridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/sevenbridges/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/sevenbridges/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/sevenbridges/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/sevenbridges/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/sevenbridges/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.279236 py-orca-1.3.4/src/orca/services/synapse/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/synapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/synapse/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/synapse/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/synapse/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-03-04 13:49:38.000000 py-orca-1.3.4/src/orca/services/synapse/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.283237 py-orca-1.3.4/src/py_orca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-03-04 13:50:26.000000 py-orca-1.3.4/src/py_orca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-04 13:50:26.000000 py-orca-1.3.4/src/py_orca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 13:50:26.000000 py-orca-1.3.4/src/py_orca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-04 13:50:26.000000 py-orca-1.3.4/src/py_orca.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 13:50:26.000000 py-orca-1.3.4/src/py_orca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-04 13:50:26.000000 py-orca-1.3.4/src/py_orca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-04 13:50:26.000000 py-orca-1.3.4/src/py_orca.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.279236 py-orca-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.279236 py-orca-1.3.4/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/acceptance/test_cavatica.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.279236 py-orca-1.3.4/tests/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/airflow/test_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.279236 py-orca-1.3.4/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.279236 py-orca-1.3.4/tests/services/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/base/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/base/test_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/base/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/base/test_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/base/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/base/test_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.283237 py-orca-1.3.4/tests/services/nextflowtower/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/nextflowtower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/nextflowtower/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    27650 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/nextflowtower/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/nextflowtower/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/nextflowtower/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/nextflowtower/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/nextflowtower/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/nextflowtower/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/nextflowtower/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.283237 py-orca-1.3.4/tests/services/sevenbridges/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/sevenbridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/sevenbridges/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/sevenbridges/test_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/sevenbridges/test_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/sevenbridges/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/sevenbridges/test_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:50:26.283237 py-orca-1.3.4/tests/services/synapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/synapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/synapse/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/synapse/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/services/synapse/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-04 13:49:38.000000 py-orca-1.3.4/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-03-04 13:49:38.000000 py-orca-1.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.650712 py_orca-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-19 02:04:57.000000 py_orca-1.3.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-19 02:04:57.000000 py_orca-1.3.5/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.634712 py_orca-1.3.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 02:04:57.000000 py_orca-1.3.5/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.634712 py_orca-1.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-19 02:04:57.000000 py_orca-1.3.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-19 02:04:57.000000 py_orca-1.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 02:04:57.000000 py_orca-1.3.5/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-19 02:04:57.000000 py_orca-1.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-19 02:04:57.000000 py_orca-1.3.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 02:04:57.000000 py_orca-1.3.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-19 02:04:57.000000 py_orca-1.3.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-04-19 02:04:57.000000 py_orca-1.3.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 02:04:57.000000 py_orca-1.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-04-19 02:05:47.650712 py_orca-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-19 02:04:57.000000 py_orca-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-19 02:04:57.000000 py_orca-1.3.5/demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      669 2024-04-19 02:04:57.000000 py_orca-1.3.5/dev_setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.634712 py_orca-1.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-19 02:04:57.000000 py_orca-1.3.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.634712 py_orca-1.3.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 02:04:57.000000 py_orca-1.3.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 02:04:57.000000 py_orca-1.3.5/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 02:04:57.000000 py_orca-1.3.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-19 02:04:57.000000 py_orca-1.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 02:04:57.000000 py_orca-1.3.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-19 02:04:57.000000 py_orca-1.3.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-19 02:04:57.000000 py_orca-1.3.5/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 02:04:57.000000 py_orca-1.3.5/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-19 02:04:57.000000 py_orca-1.3.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-19 02:04:57.000000 py_orca-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 02:04:57.000000 py_orca-1.3.5/requirements-airflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-19 02:05:47.650712 py_orca-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-19 02:04:57.000000 py_orca-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.630712 py_orca-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.634712 py_orca-1.3.5/src/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/docker/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.634712 py_orca-1.3.5/src/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.634712 py_orca-1.3.5/src/orca/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/airflow/provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.634712 py_orca-1.3.5/src/orca/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.638712 py_orca-1.3.5/src/orca/services/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/base/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/base/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/base/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.638712 py_orca-1.3.5/src/orca/services/nextflowtower/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/nextflowtower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/nextflowtower/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/nextflowtower/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/nextflowtower/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/nextflowtower/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/nextflowtower/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11134 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/nextflowtower/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/nextflowtower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.638712 py_orca-1.3.5/src/orca/services/sevenbridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/sevenbridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/sevenbridges/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/sevenbridges/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/sevenbridges/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/sevenbridges/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/sevenbridges/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.638712 py_orca-1.3.5/src/orca/services/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/synapse/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/synapse/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/synapse/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-19 02:04:57.000000 py_orca-1.3.5/src/orca/services/synapse/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.646712 py_orca-1.3.5/src/py_orca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-04-19 02:05:47.000000 py_orca-1.3.5/src/py_orca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-19 02:05:47.000000 py_orca-1.3.5/src/py_orca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:05:47.000000 py_orca-1.3.5/src/py_orca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 02:05:47.000000 py_orca-1.3.5/src/py_orca.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:05:47.000000 py_orca-1.3.5/src/py_orca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-19 02:05:47.000000 py_orca-1.3.5/src/py_orca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 02:05:47.000000 py_orca-1.3.5/src/py_orca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.642712 py_orca-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.642712 py_orca-1.3.5/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/acceptance/test_cavatica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.642712 py_orca-1.3.5/tests/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/airflow/test_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.642712 py_orca-1.3.5/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.642712 py_orca-1.3.5/tests/services/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/base/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/base/test_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/base/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/base/test_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/base/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/base/test_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.646712 py_orca-1.3.5/tests/services/nextflowtower/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/nextflowtower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/nextflowtower/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27650 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/nextflowtower/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/nextflowtower/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/nextflowtower/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/nextflowtower/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/nextflowtower/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12063 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/nextflowtower/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/nextflowtower/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.646712 py_orca-1.3.5/tests/services/sevenbridges/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/sevenbridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/sevenbridges/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/sevenbridges/test_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/sevenbridges/test_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/sevenbridges/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/sevenbridges/test_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:05:47.646712 py_orca-1.3.5/tests/services/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/synapse/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/synapse/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/services/synapse/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 02:04:57.000000 py_orca-1.3.5/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-19 02:04:57.000000 py_orca-1.3.5/tox.ini
```

### Comparing `py-orca-1.3.4/.coveragerc` & `py_orca-1.3.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/.env.example` & `py_orca-1.3.5/.env.example`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/.github/workflows/ci.yml` & `py_orca-1.3.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/.gitignore` & `py_orca-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/.pre-commit-config.yaml` & `py_orca-1.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/CHANGELOG.md` & `py_orca-1.3.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/CONTRIBUTING.md` & `py_orca-1.3.5/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -242,15 +242,21 @@
    running `tox -- -k <NAME OF THE FALLING TEST> --pdb`).
    You can also setup breakpoints manually instead of using the `--pdb` option.
 
 ## Maintainer tasks
 
 ### Releases
 
-If you are part of the group of maintainers and have correct user permissions
+If you are a member of the DPE team at Sage Bionetworks, you can simply publish a new release on GitHub in the Releases tab.
+
+1. Create a new tag which is unique and incremental to the previous version. This repository uses [Semantic Versioning](https://semver.org/).
+1. Monitor the GitHub Action which will be triggered by the new release.
+1. Once the Action is complete, ensure that the new release is published to PyPI and can be installed.
+
+If you are NOT a member of the DPE team at Sage Bionetworks, but you are part of the group of maintainers and have correct user permissions
 on [PyPI], the following steps can be used to release a new version for
 `orca`:
 
 1. Make sure all unit tests are successful.
 2. Tag the current commit on the main branch with a release tag, e.g., `v1.2.3`.
 3. Push the new tag to the upstream [repository],
    e.g., `git push upstream v1.2.3`
```

### Comparing `py-orca-1.3.4/LICENSE.txt` & `py_orca-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/PKG-INFO` & `py_orca-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-orca
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python package for connecting services and building data pipelines
 Home-page: https://github.com/Sage-Bionetworks-Workflows/py-orca
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/Sage-Bionetworks-Workflows/py-orca
 Project-URL: Tracker, https://github.com/Sage-Bionetworks-Workflows/py-orca/issues
@@ -18,16 +18,16 @@
 License-File: LICENSE.txt
 Requires-Dist: apache-airflow==2.7.2
 Requires-Dist: pydantic~=1.10
 Requires-Dist: sqlalchemy<2.0
 Requires-Dist: typing-extensions~=4.5
 Provides-Extra: all
 Requires-Dist: challengeutils~=4.3; extra == "all"
-Requires-Dist: synapseclient~=2.7; extra == "all"
-Requires-Dist: fs-synapse~=1.0; extra == "all"
+Requires-Dist: synapseclient~=4.1; extra == "all"
+Requires-Dist: fs-synapse~=2.0; extra == "all"
 Requires-Dist: sevenbridges-python~=2.9; extra == "all"
 Requires-Dist: requests~=2.28; extra == "all"
 Requires-Dist: urllib3<2.0; extra == "all"
 Provides-Extra: testing
 Requires-Dist: setuptools~=65.0; extra == "testing"
 Requires-Dist: pytest~=7.0; extra == "testing"
 Requires-Dist: pytest-cov~=4.0; extra == "testing"
```

### Comparing `py-orca-1.3.4/README.md` & `py_orca-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/demo.py` & `py_orca-1.3.5/demo.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/dev_setup.sh` & `py_orca-1.3.5/dev_setup.sh`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/docs/Makefile` & `py_orca-1.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/docs/conf.py` & `py_orca-1.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/docs/index.md` & `py_orca-1.3.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/pyproject.toml` & `py_orca-1.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/setup.cfg` & `py_orca-1.3.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 all = 
 	challengeutils~=4.3
-	synapseclient~=2.7
-	fs-synapse~=1.0
+	synapseclient~=4.1
+	fs-synapse~=2.0
 	sevenbridges-python~=2.9
 	requests~=2.28
 	urllib3<2.0
 testing = 
 	setuptools~=65.0
 	pytest~=7.0
 	pytest-cov~=4.0
```

### Comparing `py-orca-1.3.4/setup.py` & `py_orca-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/__init__.py` & `py_orca-1.3.5/src/orca/__init__.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/airflow/provider_info.py` & `py_orca-1.3.5/src/orca/airflow/provider_info.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/__init__.py` & `py_orca-1.3.5/src/orca/services/__init__.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/base/client_factory.py` & `py_orca-1.3.5/src/orca/services/base/client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/base/config.py` & `py_orca-1.3.5/src/orca/services/base/config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/base/hook.py` & `py_orca-1.3.5/src/orca/services/base/hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/base/ops.py` & `py_orca-1.3.5/src/orca/services/base/ops.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/nextflowtower/__init__.py` & `py_orca-1.3.5/src/orca/services/nextflowtower/__init__.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/nextflowtower/client.py` & `py_orca-1.3.5/src/orca/services/nextflowtower/client.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/nextflowtower/client_factory.py` & `py_orca-1.3.5/src/orca/services/nextflowtower/client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/nextflowtower/config.py` & `py_orca-1.3.5/src/orca/services/nextflowtower/config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/nextflowtower/hook.py` & `py_orca-1.3.5/src/orca/services/nextflowtower/hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/nextflowtower/models.py` & `py_orca-1.3.5/src/orca/services/nextflowtower/models.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/nextflowtower/ops.py` & `py_orca-1.3.5/src/orca/services/nextflowtower/ops.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/nextflowtower/utils.py` & `py_orca-1.3.5/src/orca/services/nextflowtower/utils.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/sevenbridges/client_factory.py` & `py_orca-1.3.5/src/orca/services/sevenbridges/client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/sevenbridges/config.py` & `py_orca-1.3.5/src/orca/services/sevenbridges/config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/sevenbridges/hook.py` & `py_orca-1.3.5/src/orca/services/sevenbridges/hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/sevenbridges/models.py` & `py_orca-1.3.5/src/orca/services/sevenbridges/models.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/sevenbridges/ops.py` & `py_orca-1.3.5/src/orca/services/sevenbridges/ops.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/synapse/client_factory.py` & `py_orca-1.3.5/src/orca/services/synapse/client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/synapse/config.py` & `py_orca-1.3.5/src/orca/services/synapse/config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/synapse/hook.py` & `py_orca-1.3.5/src/orca/services/synapse/hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/src/orca/services/synapse/ops.py` & `py_orca-1.3.5/src/orca/services/synapse/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
         """
         # Trigger indexing
         self.trigger_indexing(submission_view)
 
         # Get all submissions for the given ``submission_view``
         query_results = self.client.tableQuery(
-            f"select * from {submission_view} where status = '{submission_status}'"
+            f"select id from {submission_view} where status = '{submission_status}'"
         )
 
         submission_ids = query_results.asDataFrame()["id"].tolist()
 
         return submission_ids
 
     def update_submission_status(
```

### Comparing `py-orca-1.3.4/src/py_orca.egg-info/PKG-INFO` & `py_orca-1.3.5/src/py_orca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-orca
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python package for connecting services and building data pipelines
 Home-page: https://github.com/Sage-Bionetworks-Workflows/py-orca
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/Sage-Bionetworks-Workflows/py-orca
 Project-URL: Tracker, https://github.com/Sage-Bionetworks-Workflows/py-orca/issues
@@ -18,16 +18,16 @@
 License-File: LICENSE.txt
 Requires-Dist: apache-airflow==2.7.2
 Requires-Dist: pydantic~=1.10
 Requires-Dist: sqlalchemy<2.0
 Requires-Dist: typing-extensions~=4.5
 Provides-Extra: all
 Requires-Dist: challengeutils~=4.3; extra == "all"
-Requires-Dist: synapseclient~=2.7; extra == "all"
-Requires-Dist: fs-synapse~=1.0; extra == "all"
+Requires-Dist: synapseclient~=4.1; extra == "all"
+Requires-Dist: fs-synapse~=2.0; extra == "all"
 Requires-Dist: sevenbridges-python~=2.9; extra == "all"
 Requires-Dist: requests~=2.28; extra == "all"
 Requires-Dist: urllib3<2.0; extra == "all"
 Provides-Extra: testing
 Requires-Dist: setuptools~=65.0; extra == "testing"
 Requires-Dist: pytest~=7.0; extra == "testing"
 Requires-Dist: pytest-cov~=4.0; extra == "testing"
```

### Comparing `py-orca-1.3.4/src/py_orca.egg-info/SOURCES.txt` & `py_orca-1.3.5/src/py_orca.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 .isort.cfg
 .pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE.txt
-Pipfile
-Pipfile.lock
 README.md
 demo.py
 dev_setup.sh
 pyproject.toml
 requirements-airflow.txt
 setup.cfg
 setup.py
```

### Comparing `py-orca-1.3.4/src/py_orca.egg-info/requires.txt` & `py_orca-1.3.5/src/py_orca.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 apache-airflow==2.7.2
 pydantic~=1.10
 sqlalchemy<2.0
 typing-extensions~=4.5
 
 [all]
 challengeutils~=4.3
-synapseclient~=2.7
-fs-synapse~=1.0
+synapseclient~=4.1
+fs-synapse~=2.0
 sevenbridges-python~=2.9
 requests~=2.28
 urllib3<2.0
 
 [dev]
 pre-commit~=2.0
 sphinx-rtd-theme~=1.0
```

### Comparing `py-orca-1.3.4/tests/acceptance/test_cavatica.py` & `py_orca-1.3.5/tests/acceptance/test_cavatica.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/airflow/test_provider_info.py` & `py_orca-1.3.5/tests/airflow/test_provider_info.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/base/conftest.py` & `py_orca-1.3.5/tests/services/base/conftest.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/base/test_client_factory.py` & `py_orca-1.3.5/tests/services/base/test_client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/base/test_config.py` & `py_orca-1.3.5/tests/services/base/test_config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/base/test_hook.py` & `py_orca-1.3.5/tests/services/base/test_hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/base/test_meta.py` & `py_orca-1.3.5/tests/services/base/test_meta.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/base/test_ops.py` & `py_orca-1.3.5/tests/services/base/test_ops.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/nextflowtower/conftest.py` & `py_orca-1.3.5/tests/services/nextflowtower/conftest.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/nextflowtower/responses.py` & `py_orca-1.3.5/tests/services/nextflowtower/responses.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/nextflowtower/test_client.py` & `py_orca-1.3.5/tests/services/nextflowtower/test_client.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/nextflowtower/test_config.py` & `py_orca-1.3.5/tests/services/nextflowtower/test_config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/nextflowtower/test_integration.py` & `py_orca-1.3.5/tests/services/nextflowtower/test_integration.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/nextflowtower/test_models.py` & `py_orca-1.3.5/tests/services/nextflowtower/test_models.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/nextflowtower/test_ops.py` & `py_orca-1.3.5/tests/services/nextflowtower/test_ops.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/nextflowtower/test_utils.py` & `py_orca-1.3.5/tests/services/nextflowtower/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/sevenbridges/conftest.py` & `py_orca-1.3.5/tests/services/sevenbridges/conftest.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/sevenbridges/test_client_factory.py` & `py_orca-1.3.5/tests/services/sevenbridges/test_client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/sevenbridges/test_hook.py` & `py_orca-1.3.5/tests/services/sevenbridges/test_hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/sevenbridges/test_ops.py` & `py_orca-1.3.5/tests/services/sevenbridges/test_ops.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/synapse/conftest.py` & `py_orca-1.3.5/tests/services/synapse/conftest.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.3.4/tests/services/synapse/test_ops.py` & `py_orca-1.3.5/tests/services/synapse/test_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             # Calling the function to be tested
             result = mocked_ops.get_submissions_with_status(
                 submission_view, submission_status
             )
 
             # Assertions
             syn_mock.tableQuery.assert_called_once_with(
-                f"select * from {submission_view} where status = '{submission_status}'"
+                f"select id from {submission_view} where status = '{submission_status}'"
             )
             table_mock.asDataFrame.assert_called()
             assert result == input_dict["id"]
 
 
 def test_update_submission_status(
     mocker: pytest.fixture, mocked_ops: MagicMock
```

### Comparing `py-orca-1.3.4/tox.ini` & `py_orca-1.3.5/tox.ini`

 * *Files identical despite different names*

