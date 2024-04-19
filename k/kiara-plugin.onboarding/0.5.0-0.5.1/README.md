# Comparing `tmp/kiara_plugin.onboarding-0.5.0.tar.gz` & `tmp/kiara_plugin_onboarding-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.onboarding-0.5.0.tar", last modified: Mon Nov 13 09:22:32 2023, max compression
+gzip compressed data, was "kiara_plugin_onboarding-0.5.1.tar", last modified: Fri Apr 19 13:24:39 2024, max compression
```

## Comparing `kiara_plugin.onboarding-0.5.0.tar` & `kiara_plugin_onboarding-0.5.1.tar`

### file list

```diff
@@ -1,92 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.656245 kiara_plugin.onboarding-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.644245 kiara_plugin.onboarding-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.648245 kiara_plugin.onboarding-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.github/workflows/build-linux.yaml.rej
--rw-r--r--   0 runner    (1001) docker     (127)      698 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2023-11-13 09:22:32.656245 kiara_plugin.onboarding-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.644245 kiara_plugin.onboarding-0.5.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/ci/conda/conda-pkg-patch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/ci/conda/kiara_plugin.onboarding/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/ci/conda/kiara_plugin.onboarding/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (127)      854 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.648245 kiara_plugin.onboarding-0.5.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33121 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/examples/pipelines/example_pipeline_onboarding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.648245 kiara_plugin.onboarding-0.5.0/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 09:22:32.656245 kiara_plugin.onboarding-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.648245 kiara_plugin.onboarding-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.648245 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/models/
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.656245 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/modules/
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.656245 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/modules/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/modules/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/modules/files/import_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/modules/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.656245 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.656245 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.656245 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/utils/download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.652245 kiara_plugin.onboarding-0.5.0/src/kiara_plugin.onboarding.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2023-11-13 09:22:32.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin.onboarding.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2023-11-13 09:22:32.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin.onboarding.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 09:22:32.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin.onboarding.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-11-13 09:22:32.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin.onboarding.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-11-13 09:22:32.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin.onboarding.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-13 09:22:32.000000 kiara_plugin.onboarding-0.5.0/src/kiara_plugin.onboarding.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.656245 kiara_plugin.onboarding-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:32.656245 kiara_plugin.onboarding-0.5.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      236 2023-11-13 09:22:14.000000 kiara_plugin.onboarding-0.5.0/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.796837 kiara_plugin_onboarding-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.804838 kiara_plugin_onboarding-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.804838 kiara_plugin_onboarding-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.796837 kiara_plugin_onboarding-0.5.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.804838 kiara_plugin_onboarding-0.5.1/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/ci/conda/conda-pkg-patch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.804838 kiara_plugin_onboarding-0.5.1/ci/conda/kiara_plugin.onboarding/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/ci/conda/kiara_plugin.onboarding/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.808838 kiara_plugin_onboarding-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.808838 kiara_plugin_onboarding-0.5.1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.800837 kiara_plugin_onboarding-0.5.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.808838 kiara_plugin_onboarding-0.5.1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.808838 kiara_plugin_onboarding-0.5.1/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33121 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.808838 kiara_plugin_onboarding-0.5.1/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/jobs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/jobs/download_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/jobs/download_file_bundle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/jobs/download_file_bundle_from_github.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/jobs/download_file_bundle_subfolder.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/jobs/download_file_from_github.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.808838 kiara_plugin_onboarding-0.5.1/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/examples/pipelines/example_pipeline_onboarding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/pixi.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.800837 kiara_plugin_onboarding-0.5.1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.808838 kiara_plugin_onboarding-0.5.1/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.800837 kiara_plugin_onboarding-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.800837 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.812837 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.812837 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.812837 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.812837 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/download/
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/download/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/download/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.812837 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/files/import_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.812837 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.812837 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.812837 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/utils/download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/src/kiara_plugin.onboarding.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-19 13:24:39.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin.onboarding.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-19 13:24:39.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin.onboarding.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:24:39.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin.onboarding.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-19 13:24:39.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin.onboarding.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-19 13:24:39.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin.onboarding.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 13:24:39.000000 kiara_plugin_onboarding-0.5.1/src/kiara_plugin.onboarding.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.800837 kiara_plugin_onboarding-0.5.1/tests/job_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file_bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file_bundle/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file_bundle_from_github/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file_bundle_from_github/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file_bundle_incl_files_1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file_bundle_incl_files_1/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file_bundle_subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file_bundle_subfolder/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file_from_github/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/job_tests/download_file_from_github/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/tests/resources/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/resources/jobs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/resources/jobs/download_file_bundle_incl_files_1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:39.816838 kiara_plugin_onboarding-0.5.1/tests/resources/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/resources/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      236 2024-04-19 13:24:34.000000 kiara_plugin_onboarding-0.5.1/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.onboarding-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin_onboarding-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin_onboarding-0.5.1/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/.github/workflows/build-darwin.yaml` & `kiara_plugin_onboarding-0.5.1/.github/workflows/build-darwin.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -10,17 +10,23 @@
     name: pytest on darwin
     runs-on: macos-11
     strategy:
       matrix:
         python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "${{ matrix.python_version }}"
-      - uses: actions/checkout@v3
+      - name: pip cache
+        id: pip-cache
+        uses: actions/cache@v4
+        with:
+          path: ~/.cache/pip
+          key: ${{ runner.os }}-pip-${{ matrix.python_version }}
+      - uses: actions/checkout@v4
       - name: install kiara_plugin.onboarding
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
       - name: Test with pytest
         run: make test
```

### Comparing `kiara_plugin.onboarding-0.5.0/.github/workflows/build-linux.yaml` & `kiara_plugin_onboarding-0.5.1/.github/workflows/build-linux.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -17,24 +17,37 @@
     name: pytest on linux
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "${{ matrix.python_version }}"
-      - uses: actions/checkout@v3
+      - name: pip cache
+        id: pip-cache
+        uses: actions/cache@v4
+        with:
+          path: ~/.cache/pip
+          key: ${{ runner.os }}-pip-${{ matrix.python_version }}
+      - uses: actions/checkout@v4
       - name: install kiara_plugin.onboarding
-        run: pip install -U .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
-      - name: Test with pytest
-        run: make test
+      - name: test with pytest
+        run: pytest --cov-report=xml --cov=kiara_plugin.onboarding tests
+      - name: Coveralls
+        uses: coverallsapp/github-action@v2
+        with:
+          parallel: true
+          flag-name: run ${{ join(matrix.*, ' - ') }}
+          format: cobertura
+          file: coverage.xml
 
 # Uncomment this if you have coveralls.io setup with this repo
 #  coverage:
 #    name: create and publish test coverage
 #    runs-on: ubuntu-latest
 #    steps:
 #      - name: "Set up Python 3.9"
@@ -49,68 +62,74 @@
 #      - name: Run coverage
 #        run: coverage run -m pytest tests
 #      - name: Upload coverage data to coveralls.io
 #        run: coveralls --service=github
 #        env:
 #          GITHUB_TOKEN:  ${{ secrets.GITHUB_TOKEN }}""
 
-
-# Uncomment this if you want to run mypy
   mypy-linux:
     name: mypy check on linux
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "${{ matrix.python_version }}"
-      - uses: actions/checkout@v3
+      - name: pip cache
+        id: pip-cache
+        uses: actions/cache@v4
+        with:
+          path: ~/.cache/pip
+          key: $${{ runner.os }}-pip-${{ matrix.python_version }}
+      - uses: actions/checkout@v4
       - name: install kiara_plugin.onboarding
-        run: pip install -U .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: Test with mypy
         run: make mypy
 
   linting-linux:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Install Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - name: pip cache
         id: pip-cache
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ~/.cache/pip
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/setup.*') }}
+          key: ${{ runner.os }}-pip-3.12
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -U ruff
       # Include `--format=github` to enable automatic inline annotations.
       - name: Run Ruff
-        run: ruff --output-format=github src/
+        run: ruff check --output-format=github src/
 
   build_python_package:
     name: build python package
     runs-on: ubuntu-latest
-    needs:
-      - test-linux
-      - mypy-linux
-      - linting-linux
     steps:
-      - name: Set up Python 3.11
-        uses: actions/setup-python@v4
+      - name: Set up Python 3.12
+        uses: actions/setup-python@v5
         with:
-          python-version: "3.11"
-      - uses: actions/checkout@v3
+          python-version: "3.12"
+      - name: pip cache
+        id: pip-cache
+        uses: actions/cache@v4
+        with:
+          path: ~/.cache/pip
+          key: ${{ runner.os }}-pip-3.12
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: install pip
         run: pip install -U pip setuptools setuptools_scm build
       - name: create packages
         run: python -m build
       - name: upload artifacts
@@ -121,70 +140,93 @@
 
   release_python_package:
     name: publish python package to pypi
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     runs-on: ubuntu-latest
     needs:
       - build_python_package
-    env:
-        GEMFURY_PUSH_TOKEN: ${{ secrets.GEMFURY_PUSH_TOKEN }}
+      - build_conda_package
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
       - name: Retrieve build distributions
         uses: actions/download-artifact@v3
         with:
           name: build-dists
           path: dist/
       - name: publish to PyPI  # make sure you have pypi trusted publishing configured for this repo
         uses: pypa/gh-action-pypi-publish@release/v1
 
-  build_and_release_conda_package:
+  build_conda_package:
     name: conda package build (and upload if release)
     runs-on: ubuntu-latest
-    needs:
-      - test-linux
-      - mypy-linux   # uncomment if this step is enabled
-      - linting-linux   # uncomment if this step is enabled
     steps:
-      - name: "Set up Python 3.11"
-        uses: actions/setup-python@v4
+      - name: "Set up Python 3.12"
+        uses: actions/setup-python@v5
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - name: pip cache
         id: pip-cache
-        uses: actions/cache@v3
+        uses: actions/cache@v4
         with:
           path: ~/.cache/pip
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/setup.*') }}
-      - uses: actions/checkout@v3
+          key: ${{ runner.os }}-pip-3.12
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - name: install kiara
-        run: pip install kiara
-      - name: install required plugin packages
-        run: pip install git+https://github.com/DHARPA-Project/kiara_plugin.develop.git@develop
+      - name: install kiara_plugin.develop
+        run: pip install kiara_plugin.develop
       - name: build conda package
-        if: ${{ ( github.ref == 'refs/heads/develop') }}
-        run: kiara conda build-package --patch-data ci/conda/conda-pkg-patch.yaml .
-      - name: extract tag name
-        run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
-      - name: build & publish conda package
-        if: ${{ startsWith(github.ref, 'refs/tags/') }}
-        run: kiara conda build-package --publish --user dharpa --token ${{ secrets.ANACONDA_PUSH_TOKEN }} --patch-data ci/conda/conda-pkg-patch.yaml .
+        run: kiara build conda pkg --channel dharpa --channel conda-forge --patch-data ci/conda/conda-pkg-patch.yaml --output-folder build-dir .
+      - name: upload artifacts
+        uses: actions/upload-artifact@v4
+        with:
+          name: conda-pkgs
+          path: build-dir/
+
+  release_conda_package:
+    name: publish python package to anaconda
+    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
+    runs-on: ubuntu-latest
+    needs:
+      - test-linux
+      - mypy-linux
+      - linting-linux
+      - build_python_package
+      - build_conda_package
+    steps:
+      - name: "Set up Python 3.12"
+        uses: actions/setup-python@v5
+        with:
+          python-version: "3.12"
+      - name: pip cache
+        id: pip-cache
+        uses: actions/cache@v4
+        with:
+          path: ~/.cache/pip
+          key: ${{ runner.os }}-pip-3.12
+      - name: install kiara_plugin.develop
+        run: pip install kiara_plugin.develop
+      - name: Retrieve build distributions
+        uses: actions/download-artifact@v4
+        with:
+          name: conda-pkgs
+          path: build-dir/
+      - name: release conda package
+        run: kiara build conda publish --user dharpa --channel dharpa --token ${{ secrets.ANACONDA_PUSH_TOKEN }} build-dir
 
   merge_tag_to_main:
     name: merge current tag to main branch
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     needs:
       - release_python_package
-      - build_and_release_conda_package
+      - release_conda_package
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - run: git config --global user.email "markus@frkl.io"
     - run: git config --global user.name "Markus Binsteiner"
     - name: extract tag name
       run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
     - name: checkout main branch
```

### Comparing `kiara_plugin.onboarding-0.5.0/.gitignore` & `kiara_plugin_onboarding-0.5.1/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -48,20 +48,20 @@
 pip-wheel-metadata/
 .python-version
 src/kiara_plugin/onboarding/version.txt
 .direnv
 public
 site
 .dephell_report
-.direnv
 .mypy_cache
 .env
 docs/api-documentation.md
 .frkl
 .envrc
 build.sh
 onefile.spec
 *_complete.zsh.zwc
 ci/conda/**/build
 ci/conda/kiara_plugin.onboarding/meta.yaml
 .pixi
+pixi.lock
 dev.py
```

### Comparing `kiara_plugin.onboarding-0.5.0/.pre-commit-config.yaml` & `kiara_plugin_onboarding-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/LICENSE` & `kiara_plugin_onboarding-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/Makefile` & `kiara_plugin_onboarding-0.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/ci/conda/kiara_plugin.onboarding/meta.yaml.template` & `kiara_plugin_onboarding-0.5.1/ci/conda/kiara_plugin.onboarding/meta.yaml.template`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/docs/development.md` & `kiara_plugin_onboarding-0.5.1/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/docs/index.md` & `kiara_plugin_onboarding-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin_onboarding-0.5.1/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin_onboarding-0.5.1/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/mkdocs.yml` & `kiara_plugin_onboarding-0.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/pyproject.toml` & `kiara_plugin_onboarding-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
-    "kiara>=0.5.1,<0.6.0",
-    "kiara_plugin.core_types>=0.5.0,<0.6.0",
+    "kiara>=0.5.10,<0.6.0",
+    "kiara_plugin.core_types>=0.5.1,<0.6.0",
     "httpx>=0.23.0",
     "pyzenodo3>=1.0.2",
     "PyGithub>=1.58.0",
     "pyzotero>=1.5.9"
 ]
 dynamic = ["version"]
 
@@ -240,10 +240,15 @@
     "pydantic.mypy"
 ]
 
 
 # mypy per-module options:
 [[tool.mypy.overrides]]
 module = [
-    "pyzenodo3.*"
+    "patoolib.*",
+    "pyzenodo3.*",
+    "ruamel.*",
+    "appdirs.*",
+    "pyarrow.*",
+    "ruamel.*"
 ]
 ignore_missing_imports = true
```

### Comparing `kiara_plugin.onboarding-0.5.0/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin_onboarding-0.5.1/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/scripts/documentation/gen_info_pages.py` & `kiara_plugin_onboarding-0.5.1/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/scripts/documentation/gen_module_doc.py` & `kiara_plugin_onboarding-0.5.1/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/__init__.py` & `kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/models/__init__.py` & `kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/modules/__init__.py` & `kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,190 +1,199 @@
 # -*- coding: utf-8 -*-
-from typing import List, Union
+import abc
+import atexit
+import shutil
+import tempfile
+from typing import TYPE_CHECKING, Any, Dict, List, Union
 
 from pydantic import Field
 
-from kiara.exceptions import KiaraException
-from kiara.models.filesystem import FolderImportConfig
+from kiara.exceptions import KiaraException, KiaraProcessingException
 from kiara.models.module import KiaraModuleConfig
 from kiara.models.values.value import ValueMap
 from kiara.modules import KiaraModule, ValueMapSchema
-from kiara.registries.models import ModelRegistry
-from kiara_plugin.onboarding.models import OnboardDataModel
-from kiara_plugin.onboarding.utils.download import (
-    get_onboard_model_cls,
-    onboard_file,
-    onboard_file_bundle,
-)
+
+if TYPE_CHECKING:
+    from kiara.models.filesystem import FolderImportConfig, KiaraFile, KiaraFileBundle
 
 
 class OnboardFileConfig(KiaraModuleConfig):
 
-    onboard_type: Union[None, str] = Field(
-        description="The name of the type of onboarding.", default=None
+    result_file_name: Union[str, None] = Field(
+        description="The file name to use for the downloaded file, if not provided it will be auto-generated.",
+        default=None,
     )
     attach_metadata: Union[bool, None] = Field(
-        description="Whether to attach metadata.", default=None
+        description="Whether to attach metadata. If 'None', a user input will be created.",
+        default=True,
     )
 
 
 ONBOARDING_MODEL_NAME_PREFIX = "onboarding.file.from."
 
 
 class OnboardFileModule(KiaraModule):
     """A generic module that imports a file from one of several possible sources."""
 
-    _module_type_name = "import.file"
     _config_cls = OnboardFileConfig
 
+    @abc.abstractmethod
+    def create_onboard_inputs_schema(self) -> Dict[str, Any]:
+        pass
+
     def create_inputs_schema(
         self,
     ) -> ValueMapSchema:
 
-        result = {
-            "source": {
-                "type": "string",
-                "doc": "The source uri of the file to be onboarded.",
-                "optional": False,
-            },
-            "file_name": {
-                "type": "string",
-                "doc": "The file name to use for the onboarded file (defaults to source file name if possible).",
-                "optional": True,
-            },
-        }
+        result = self.create_onboard_inputs_schema()
 
-        if self.get_config_value("attach_metadata") is None:
-            result["attach_metadata"] = {
-                "type": "boolean",
-                "doc": "Whether to attach onboarding metadata to the result file.",
-                "default": True,
-            }
-
-        onboard_type: Union[str, None] = self.get_config_value("onboard_type")
-        if not onboard_type:
-            onboard_model_cls = None
-        else:
-            onboard_model_cls = get_onboard_model_cls(onboard_type)
-
-        if not onboard_model_cls:
-
-            available = (
-                ModelRegistry.instance()
-                .get_models_of_type(OnboardDataModel)
-                .item_infos.keys()
+        if "file_name" in result.keys():
+            raise KiaraException(
+                msg="The 'file_name' input is not allowed in the onboard inputs schema for an implementing class of 'OnboardFileModule'."
             )
+        result["file_name"] = {
+            "type": "string",
+            "doc": "The file name to use for the downloaded file, if not provided it will be auto-generated.",
+            "optional": True,
+        }
 
-            if not available:
-                raise KiaraException(msg="No onboard models available. This is a bug.")
-
-            idx = len(ONBOARDING_MODEL_NAME_PREFIX)
-            allowed = sorted((x[idx:] for x in available))
+        if "attach_metadata" in result.keys():
+            raise KiaraException(
+                msg="The 'attach_metadata' input is not allowed in the onboard inputs schema for an implementing class of 'OnboardFileModule'."
+            )
 
-            result["onboard_type"] = {
+        file_name = self.get_config_value("result_file_name")
+        if file_name is None:
+            result["file_name"] = {
                 "type": "string",
-                "type_config": {"allowed_strings": allowed},
-                "doc": "The type of onboarding to use. Allowed: {}".format(
-                    ", ".join(allowed)
-                ),
+                "doc": "The file name to use for the downloaded file, if not provided it will be generated from the last token of the url.",
                 "optional": True,
             }
-        elif onboard_model_cls.get_config_fields():
-            result = {
-                "onboard_config": {
-                    "type": "kiara_model",
-                    "type_config": {
-                        "kiara_model_id": self.get_config_value("onboard_type"),
-                    },
-                }
+
+        attach_metadata = self.get_config_value("attach_metadata")
+        if attach_metadata is None:
+            result["attach_metadata"] = {
+                "type": "boolean",
+                "doc": "Whether to attach onboarding metadata to the result file.",
+                "default": True,
             }
 
         return result
 
     def create_outputs_schema(
         self,
     ) -> ValueMapSchema:
 
         result = {"file": {"type": "file", "doc": "The file that was onboarded."}}
-        return result
-
-    def process(self, inputs: ValueMap, outputs: ValueMap):
 
-        onboard_type = self.get_config_value("onboard_type")
+        return result
 
-        source: str = inputs.get_value_data("source")
-        file_name: Union[str, None] = inputs.get_value_data("file_name")
+    @abc.abstractmethod
+    def retrieve_file(
+        self, inputs: ValueMap, file_name: Union[str, None], attach_metadata: bool
+    ) -> "KiaraFile":
+        pass
 
-        if not onboard_type:
+    def process(self, inputs: ValueMap, outputs: ValueMap):
 
-            user_input_onboard_type = inputs.get_value_data("onboard_type")
-            if user_input_onboard_type:
-                onboard_type = (
-                    f"{ONBOARDING_MODEL_NAME_PREFIX}{user_input_onboard_type}"
-                )
+        if "file_name" not in inputs.keys():
+            file_name = self.get_config_value("file_name")
+        else:
+            file_name = inputs.get_value_data("file_name")
 
-        attach_metadata = self.get_config_value("attach_metadata")
-        if attach_metadata is None:
+        if "attach_metadata" not in inputs.keys():
+            # must be 'True' or 'False', otherwise we'd have an input
+            attach_metadata: bool = self.get_config_value("attach_metadata")
+        else:
             attach_metadata = inputs.get_value_data("attach_metadata")
 
-        data = onboard_file(
-            source=source,
-            file_name=file_name,
-            onboard_type=onboard_type,
-            attach_metadata=attach_metadata,
-        )
+        result = self.retrieve_file(inputs, file_name, attach_metadata)
 
-        outputs.set_value("file", data)
+        outputs.set_value("file", result)
 
 
 class OnboardFileBundleConfig(KiaraModuleConfig):
 
-    onboard_type: Union[None, str] = Field(
-        description="The name of the type of onboarding.", default=None
+    result_bundle_name: Union[str, None] = Field(
+        description="The bundle name use for the downloaded file, if not provided it will be auto-generated.",
+        default=None,
     )
-    attach_metadata: Union[bool, None] = Field(
-        description="Whether to attach onboarding metadata.", default=None
+
+    attach_metadata_to_bundle: Union[bool, None] = Field(
+        description="Whether to attach the download metadata to the result file bundle instance. If 'None', a user input will be created.",
+        default=True,
+    )
+    attach_metadata_to_files: Union[bool, None] = Field(
+        description="Whether to attach the download metadata to each file in the resulting bundle.",
+        default=False,
     )
     sub_path: Union[None, str] = Field(description="The sub path to use.", default=None)
     include_files: Union[None, List[str]] = Field(
-        description="File types to include.", default=None
+        description="List of file types (strings) to include. A match happens if the end of the filename matches a token in this list.",
+        default=None,
     )
     exclude_files: Union[None, List[str]] = Field(
-        description="File types to include.", default=None
+        description="List of file types (strings) to exclude. A match happens if the end of the filename matches a token in this list.",
+        default=None,
     )
     exclude_dirs: Union[None, List[str]] = Field(
-        description="Exclude directories that end with one of those tokens.",
+        description="Exclude directories that end with one of those tokens (list of strings).",
         default=None,
     )
 
 
 class OnboardFileBundleModule(KiaraModule):
     """A generic module that imports a file from one of several possible sources."""
 
-    _module_type_name = "import.file_bundle"
     _config_cls = OnboardFileBundleConfig
 
+    @abc.abstractmethod
+    def create_onboard_inputs_schema(self) -> Dict[str, Any]:
+        pass
+
     def create_inputs_schema(
         self,
     ) -> ValueMapSchema:
 
-        result = {
-            "source": {
+        result = self.create_onboard_inputs_schema()
+
+        for forbidden in [
+            "bundle_name",
+            "attach_metadata_to_bundle",
+            "attach_metadata_to_files",
+            "sub_path",
+            "include_files",
+            "exclude_files",
+            "exclude_dirs",
+        ]:
+            if forbidden in result.keys():
+                raise KiaraException(
+                    msg=f"The '{forbidden}' input is not allowed in the onboard inputs schema for an implementing class of 'OnboardFileBundleModule'."
+                )
+
+        if self.get_config_value("result_bundle_name") is None:
+            result["bundle_name"] = {
                 "type": "string",
-                "doc": "The source uri of the file to be onboarded.",
-                "optional": False,
+                "doc": "The bundle name use for the downloaded file, if not provided it will be autogenerated.",
+                "optional": True,
             }
-        }
 
-        if self.get_config_value("attach_metadata") is None:
-            result["attach_metadata"] = {
+        if self.get_config_value("attach_metadata_to_bundle") is None:
+            result["attach_metadata_to_bundle"] = {
                 "type": "boolean",
-                "doc": "Whether to attach onboarding metadata.",
+                "doc": "Whether to attach the download metadata to the result file bundle instance.",
                 "default": True,
             }
+        if self.get_config_value("attach_metadata_to_files") is None:
+            result["attach_metadata_to_bundle"] = {
+                "type": "boolean",
+                "doc": "Whether to attach the download metadata to each file in the resulting bundle.",
+                "default": False,
+            }
+
         if self.get_config_value("sub_path") is None:
             result["sub_path"] = {
                 "type": "string",
                 "doc": "The sub path to use. If not specified, the root of the source folder will be used.",
                 "optional": True,
             }
         if self.get_config_value("include_files") is None:
@@ -203,52 +212,14 @@
         if self.get_config_value("exclude_dirs") is None:
             result["exclude_dirs"] = {
                 "type": "list",
                 "doc": "Exclude directories that end with one of those tokens. If not specified, no directories are excluded.",
                 "optional": True,
             }
 
-        onboard_type: Union[str, None] = self.get_config_value("onboard_type")
-        if not onboard_type:
-            onboard_model_cls = None
-        else:
-            onboard_model_cls = get_onboard_model_cls(onboard_type)
-
-        if not onboard_model_cls:
-
-            available = (
-                ModelRegistry.instance()
-                .get_models_of_type(OnboardDataModel)
-                .item_infos.keys()
-            )
-
-            if not available:
-                raise KiaraException(msg="No onboard models available. This is a bug.")
-
-            idx = len(ONBOARDING_MODEL_NAME_PREFIX)
-            allowed = sorted((x[idx:] for x in available))
-
-            result["onboard_type"] = {
-                "type": "string",
-                "type_config": {"allowed_strings": allowed},
-                "doc": "The type of onboarding to use. Allowed: {}".format(
-                    ", ".join(allowed)
-                ),
-                "optional": True,
-            }
-        elif onboard_model_cls.get_config_fields():
-            result = {
-                "onboard_config": {
-                    "type": "kiara_model",
-                    "type_config": {
-                        "kiara_model_id": self.get_config_value("onboard_type"),
-                    },
-                }
-            }
-
         return result
 
     def create_outputs_schema(
         self,
     ) -> ValueMapSchema:
 
         result = {
@@ -257,23 +228,19 @@
                 "doc": "The file_bundle that was onboarded.",
             }
         }
         return result
 
     def process(self, inputs: ValueMap, outputs: ValueMap):
 
-        onboard_type = self.get_config_value("onboard_type")
-        source: str = inputs.get_value_data("source")
+        from kiara.models.filesystem import FolderImportConfig, KiaraFileBundle
 
-        if onboard_type:
-            user_input_onboard_type = inputs.get_value_data("onboard_type")
-            if not user_input_onboard_type:
-                onboard_type = (
-                    f"{ONBOARDING_MODEL_NAME_PREFIX}{user_input_onboard_type}"
-                )
+        bundle_name = self.get_config_value("result_bundle_name")
+        if bundle_name is None:
+            bundle_name = inputs.get_value_data("bundle_name")
 
         sub_path = self.get_config_value("sub_path")
         if sub_path is None:
             sub_path = inputs.get_value_data("sub_path")
 
         include = self.get_config_value("include_files")
         if include is None:
@@ -298,19 +265,104 @@
             import_config_data["include_files"] = include
         if exclude:
             import_config_data["exclude_files"] = exclude
         if exclude_dirs:
             import_config_data["exclude_dirs"] = exclude_dirs
 
         import_config = FolderImportConfig(**import_config_data)
-        attach_metadata = self.get_config_value("attach_metadata")
-        if attach_metadata is None:
-            attach_metadata = inputs.get_value_data("attach_metadata")
 
-        imported_bundle = onboard_file_bundle(
-            source=source,
+        attach_metadata_to_bundle = self.get_config_value("attach_metadata_to_bundle")
+        if attach_metadata_to_bundle is None:
+            attach_metadata_to_bundle = inputs.get_value_data(
+                "attach_metadata_to_bundle"
+            )
+
+        attach_metadata_to_files = self.get_config_value("attach_metadata_to_files")
+        if attach_metadata_to_files is None:
+            attach_metadata_to_files = inputs.get_value_data("attach_metadata_to_files")
+
+        archive = self.retrieve_archive(
+            inputs=inputs,
+            bundle_name=bundle_name,
+            attach_metadata_to_bundle=attach_metadata_to_bundle,
+            attach_metadata_to_files=attach_metadata_to_files,
             import_config=import_config,
-            onboard_type=onboard_type,
-            attach_metadata=attach_metadata,
         )
+        if isinstance(archive, KiaraFileBundle):
+            result = archive
+        else:
+            result = self.extract_archive(
+                archive_file=archive,
+                bundle_name=bundle_name,
+                attach_metadata_to_bundle=attach_metadata_to_bundle,
+                attach_metadata_to_files=attach_metadata_to_files,
+                import_config=import_config,
+            )
+
+        outputs.set_value("file_bundle", result)
+
+    @abc.abstractmethod
+    def retrieve_archive(
+        self,
+        inputs: ValueMap,
+        bundle_name: Union[str, None],
+        attach_metadata_to_bundle: bool,
+        attach_metadata_to_files: bool,
+        import_config: "FolderImportConfig",
+    ) -> Union["KiaraFile", "KiaraFileBundle"]:
+        """Retrieve an archive file, or the actual result file bundle."""
+
+    def extract_archive(
+        self,
+        archive_file: "KiaraFile",
+        bundle_name: Union[str, None],
+        attach_metadata_to_bundle: bool,
+        attach_metadata_to_files: bool,
+        import_config: "FolderImportConfig",
+    ) -> "KiaraFileBundle":
+        """Extract the archive file that was returned in 'retrieve_archive'."""
+
+        from kiara.models.filesystem import KiaraFileBundle
+
+        out_dir = tempfile.mkdtemp()
+
+        def del_out_dir():
+            shutil.rmtree(out_dir, ignore_errors=True)
+
+        atexit.register(del_out_dir)
+
+        error = None
+        try:
+            shutil.unpack_archive(archive_file.path, out_dir)
+        except Exception:
+            # try patool, maybe we're lucky
+            try:
+                import patoolib
+
+                patoolib.extract_archive(archive_file.path, outdir=out_dir)
+            except Exception as e:
+                error = e
+
+        if error is not None:
+            raise KiaraProcessingException(f"Could not extract archive: {error}.")
+
+        path = out_dir
+
+        if not bundle_name:
+            bundle_name = archive_file.file_name
+            if import_config.sub_path:
+                bundle_name = f"{bundle_name}#{import_config.sub_path}"
+
+        bundle = KiaraFileBundle.import_folder(
+            path, bundle_name=bundle_name, import_config=import_config
+        )
+
+        if attach_metadata_to_bundle:
+            metadata = archive_file.metadata["download_info"]
+            bundle.metadata["download_info"] = metadata
+
+        if attach_metadata_to_files or True:
+            metadata = archive_file.metadata["download_info"]
+            for kf in bundle.included_files.values():
+                kf.metadata["download_info"] = metadata
 
-        outputs.set_value("file_bundle", imported_bundle)
+        return bundle
```

### Comparing `kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/modules/files/import_file.py` & `kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/files/import_file.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py` & `kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/modules/files/import_file_bundle.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.onboarding-0.5.0/src/kiara_plugin/onboarding/utils/download.py` & `kiara_plugin_onboarding-0.5.1/src/kiara_plugin/onboarding/utils/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # -*- coding: utf-8 -*-
 import atexit
 import os
 import tempfile
 from datetime import datetime
 from functools import lru_cache
 from pathlib import Path
-from typing import Dict, List, Mapping, Tuple, Type, Union
+from typing import Any, Dict, List, Mapping, Tuple, Type, Union
 
 from pydantic import BaseModel, Field
 
 from kiara.exceptions import KiaraException
 from kiara.models.filesystem import FolderImportConfig, KiaraFile, KiaraFileBundle
+from kiara.utils.dates import get_current_time_incl_timezone
 from kiara.utils.files import unpack_archive
 from kiara.utils.json import orjson_dumps
 from kiara_plugin.onboarding.models import OnboardDataModel
 
 
 class DownloadMetadata(BaseModel):
     url: str = Field(description="The url of the download request.")
     response_headers: List[Dict[str, str]] = Field(
         description="The response headers of the download request."
     )
-    request_time: str = Field(description="The time the request was made.")
+    request_time: datetime = Field(description="The time the request was made.")
+    download_time_in_seconds: float = Field(
+        description="How long the download took in seconds."
+    )
 
 
 class DownloadBundleMetadata(DownloadMetadata):
     import_config: FolderImportConfig = Field(
         description="The import configuration that was used to import the files from the source bundle."
     )
 
@@ -52,38 +56,40 @@
     attach_metadata: bool = True,
     return_md5_hash: bool = False,
 ) -> Union[KiaraFile, Tuple[KiaraFile, str]]:
 
     import hashlib
 
     import httpx
-    import pytz
 
     if not file_name:
         # TODO: make this smarter, using content-disposition headers if available
         file_name = url.split("/")[-1]
 
     if not target:
         tmp_file = tempfile.NamedTemporaryFile(delete=False, suffix=file_name)
 
         def rm_tmp_file():
+            tmp_file.close()
             os.unlink(tmp_file.name)
 
         atexit.register(rm_tmp_file)
 
         _target = Path(tmp_file.name)
     else:
         _target = Path(target)
         _target.parent.mkdir(parents=True, exist_ok=True)
 
     if return_md5_hash:
         hash_md5 = hashlib.md5()  # noqa
 
     history = []
-    datetime.utcnow().replace(tzinfo=pytz.utc)
+
+    request_time = get_current_time_incl_timezone()
+
     with open(_target, "wb") as f:
         with httpx.stream("GET", url, follow_redirects=True) as r:
             if r.status_code < 200 or r.status_code >= 399:
                 raise KiaraException(
                     f"Could not download file from {url}: status code {r.status_code}."
                 )
             history.append(dict(r.headers))
@@ -91,20 +97,22 @@
                 history.append(dict(h.headers))
             for data in r.iter_bytes():
                 if return_md5_hash:
                     hash_md5.update(data)
                 f.write(data)
 
     result_file = KiaraFile.load_file(_target.as_posix(), file_name)
-
+    now_time = get_current_time_incl_timezone()
+    delta = (now_time - request_time).total_seconds()
     if attach_metadata:
         metadata = {
             "url": url,
             "response_headers": history,
-            "request_time": datetime.utcnow().replace(tzinfo=pytz.utc).isoformat(),
+            "request_time": request_time,
+            "download_time_in_seconds": delta,
         }
         _metadata: DownloadMetadata = DownloadMetadata(**metadata)
         result_file.metadata["download_info"] = _metadata.model_dump()
         result_file.metadata_schemas["download_info"] = orjson_dumps(
             DownloadMetadata.model_json_schema()
         )
 
@@ -133,18 +141,23 @@
         _, suffix = os.path.splitext(parsed_url.path)
     except Exception:
         pass
     if not suffix:
         suffix = ""
 
     tmp_file = tempfile.NamedTemporaryFile(delete=False, suffix=suffix)
-    atexit.register(tmp_file.close)
+
+    def rm_tmp_file():
+        tmp_file.close()
+        os.unlink(tmp_file.name)
+
+    atexit.register(rm_tmp_file)
 
     history = []
-    datetime.utcnow().replace(tzinfo=pytz.utc)
+    # datetime.utcnow().replace(tzinfo=pytz.utc)
     with open(tmp_file.name, "wb") as f:
         with httpx.stream("GET", url, follow_redirects=True) as r:
             history.append(dict(r.headers))
             for h in r.history:
                 history.append(dict(h.headers))
             for data in r.iter_bytes():
                 f.write(data)
@@ -354,7 +367,76 @@
         imported_bundle = KiaraFileBundle.from_archive_file(
             imported_bundle_file, import_config=import_config
         )
     else:
         imported_bundle = result
 
     return imported_bundle
+
+
+def download_zenodo_file_bundle(
+    doi: str,
+    version: Union[None, str],
+    attach_metadata_to_bundle: bool,
+    attach_metadata_to_files: bool,
+    bundle_name: Union[str, None] = None,
+    import_config: Union[None, Mapping[str, Any], FolderImportConfig] = None,
+) -> KiaraFileBundle:
+
+    import pyzenodo3
+
+    from kiara.models.filesystem import KiaraFile, KiaraFileBundle
+
+    if "/zenodo." not in doi:
+        doi = f"10.5281/zenodo.{doi}"
+
+    zen = pyzenodo3.Zenodo()
+
+    if version:
+        raise NotImplementedError("Downloading versioned records is not yet supported.")
+
+    record = zen.find_record_by_doi(doi)
+
+    base_path = KiaraFileBundle.create_tmp_dir()
+
+    for _available_file in record.data["files"]:
+        match = _available_file
+
+        url = match["links"]["self"]
+        checksum = match["checksum"][4:]
+
+        file_path = _available_file["key"]
+        full_path = base_path / file_path
+
+        file_name = file_path.split("/")[-1]
+
+        # TODO: filter here already, so we don't need to download files we don't want
+
+        result_file: KiaraFile
+        result_file, result_checksum = download_file(  # type: ignore
+            url=url,
+            target=full_path.as_posix(),
+            file_name=file_name,
+            attach_metadata=True,
+            return_md5_hash=True,
+        )
+
+        if checksum != result_checksum:
+            raise KiaraException(
+                msg=f"Can't download file '{file_name}' from zenodo, invalid checksum: {checksum} != {result_checksum}"
+            )
+
+    if not bundle_name:
+        bundle_name = doi
+    result = KiaraFileBundle.import_folder(
+        source=base_path.as_posix(),
+        bundle_name=bundle_name,
+        import_config=import_config,
+    )
+    if attach_metadata_to_bundle:
+        result.metadata["zenodo_record_data"] = record.data
+
+    if attach_metadata_to_files:
+        for file in result.included_files.values():
+            file.metadata["zenodo_record_data"] = record.data
+
+    return result
```

### Comparing `kiara_plugin.onboarding-0.5.0/src/kiara_plugin.onboarding.egg-info/SOURCES.txt` & `kiara_plugin_onboarding-0.5.1/src/kiara_plugin.onboarding.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -8,33 +8,38 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 commitlint.config.js
 mkdocs.yml
+pixi.toml
 pyproject.toml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/suggest-a-module.md
 .github/workflows/build-darwin.yaml
 .github/workflows/build-linux.yaml
-.github/workflows/build-linux.yaml.rej
 .github/workflows/build-windows.yaml
 ci/conda/conda-pkg-patch.yaml
 ci/conda/kiara_plugin.onboarding/meta.yaml.template
 docs/SUMMARY.md
 docs/development.md
 docs/index.md
 docs/usage.md
 docs/stylesheets/extra.css
 examples/data/Readme.md
 examples/data/journals/JournalEdges1902.csv
 examples/data/journals/JournalNodes1902.csv
 examples/data/journals/Readme.md
 examples/jobs/Readme.md
+examples/jobs/download_file.yaml
+examples/jobs/download_file_bundle.yaml
+examples/jobs/download_file_bundle_from_github.yaml
+examples/jobs/download_file_bundle_subfolder.yaml
+examples/jobs/download_file_from_github.yaml
 examples/pipelines/Readme.md
 examples/pipelines/example_pipeline_onboarding.yaml
 scripts/documentation/gen_api_doc_pages.py
 scripts/documentation/gen_info_pages.py
 scripts/documentation/gen_module_doc.py
 src/kiara_plugin.onboarding.egg-info/PKG-INFO
 src/kiara_plugin.onboarding.egg-info/SOURCES.txt
@@ -43,20 +48,31 @@
 src/kiara_plugin.onboarding.egg-info/requires.txt
 src/kiara_plugin.onboarding.egg-info/top_level.txt
 src/kiara_plugin/onboarding/__init__.py
 src/kiara_plugin/onboarding/data_types.py
 src/kiara_plugin/onboarding/py.typed
 src/kiara_plugin/onboarding/models/__init__.py
 src/kiara_plugin/onboarding/modules/__init__.py
-src/kiara_plugin/onboarding/modules/zenodo.py
+src/kiara_plugin/onboarding/modules/download/__init__.py
+src/kiara_plugin/onboarding/modules/download/github.py
+src/kiara_plugin/onboarding/modules/download/zenodo.py
 src/kiara_plugin/onboarding/modules/files/__init__.py
 src/kiara_plugin/onboarding/modules/files/import_file.py
 src/kiara_plugin/onboarding/modules/files/import_file_bundle.py
 src/kiara_plugin/onboarding/pipelines/.gitkeep
 src/kiara_plugin/onboarding/pipelines/__init__.py
 src/kiara_plugin/onboarding/resources/.gitkeep
 src/kiara_plugin/onboarding/utils/__init__.py
 src/kiara_plugin/onboarding/utils/download.py
 tests/conftest.py
 tests/test_job_descs.py
 tests/test_kiara_modules_default.py
-tests/resources/.gitkeep
+tests/job_tests/download_file/outputs.py
+tests/job_tests/download_file_bundle/outputs.py
+tests/job_tests/download_file_bundle_from_github/outputs.py
+tests/job_tests/download_file_bundle_incl_files_1/outputs.py
+tests/job_tests/download_file_bundle_subfolder/outputs.py
+tests/job_tests/download_file_from_github/outputs.py
+tests/resources/.gitkeep
+tests/resources/jobs/.gitkeep
+tests/resources/jobs/download_file_bundle_incl_files_1.yaml
+tests/resources/pipelines/.gitkeep
```

### Comparing `kiara_plugin.onboarding-0.5.0/tests/conftest.py` & `kiara_plugin_onboarding-0.5.1/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,53 +13,87 @@
 import os
 import tempfile
 import uuid
 from pathlib import Path
 
 import pytest
 
+from kiara.api import JobDesc, KiaraAPI
 from kiara.context import KiaraConfig
-from kiara.interfaces.python_api import KiaraAPI
 from kiara.interfaces.python_api.models.job import JobTest
-from kiara.utils.testing import get_tests_for_job, list_job_descs
+from kiara.utils.testing import get_init_job, get_tests_for_job, list_job_descs
 
 ROOT_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
-JOBS_FOLDER = Path(os.path.join(ROOT_DIR, "examples", "jobs"))
+JOBS_FOLDERS = [
+    Path(os.path.join(ROOT_DIR, "tests", "resources", "jobs")),
+    Path(os.path.join(ROOT_DIR, "examples", "jobs")),
+]
 
 
 def create_temp_dir():
     session_id = str(uuid.uuid4())
     TEMP_DIR = Path(os.path.join(tempfile.gettempdir(), "kiara_tests"))
 
     instance_path = os.path.join(
         TEMP_DIR.resolve().absolute(), f"instance_{session_id}"
     )
     return instance_path
 
 
+def get_job_alias(job_desc: JobDesc) -> str:
+    return job_desc.job_alias
+
+
 @pytest.fixture
 def kiara_api() -> KiaraAPI:
 
     instance_path = create_temp_dir()
     kc = KiaraConfig.create_in_folder(instance_path)
     api = KiaraAPI(kc)
     return api
 
 
-@pytest.fixture(params=list_job_descs(JOBS_FOLDER))
-def example_job_test(request, kiara_api) -> JobTest:
+@pytest.fixture
+def kiara_api_init_example() -> KiaraAPI:
+    instance_path = create_temp_dir()
+    kc = KiaraConfig.create_in_folder(instance_path)
+    api = KiaraAPI(kc)
+
+    init_jobs = []
+    for jobs_folder in JOBS_FOLDERS:
+        init_job = get_init_job(jobs_folder)
+        if init_job is not None:
+            init_jobs.append(init_job)
+
+    if not init_jobs:
+        return api
+
+    for init_job in init_jobs:
+        results = api.run_job(init_job, comment="Init example job")
+
+        if not init_job.save:
+            continue
+
+        for field_name, alias_name in init_job.save.items():
+            api.store_value(results[field_name], alias_name)
+
+    return api
+
+
+@pytest.fixture(params=list_job_descs(JOBS_FOLDERS), ids=get_job_alias)
+def example_job_test(request, kiara_api_init_example) -> JobTest:
 
     job_tests_folder = Path(os.path.join(ROOT_DIR, "tests", "job_tests"))
 
     job_desc = request.param
     tests = get_tests_for_job(
         job_alias=job_desc.job_alias, job_tests_folder=job_tests_folder
     )
 
-    job_test = JobTest(kiara_api=kiara_api, job_desc=job_desc, tests=tests)
+    job_test = JobTest(kiara_api=kiara_api_init_example, job_desc=job_desc, tests=tests)
     return job_test
 
 
 @pytest.fixture
 def example_data_folder() -> Path:
     return Path(os.path.join(ROOT_DIR, "examples", "data"))
```

### Comparing `kiara_plugin.onboarding-0.5.0/tests/test_job_descs.py` & `kiara_plugin_onboarding-0.5.1/tests/test_job_descs.py`

 * *Files identical despite different names*

