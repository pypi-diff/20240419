# Comparing `tmp/kiara_plugin.develop-0.5.0.tar.gz` & `tmp/kiara_plugin_develop-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.develop-0.5.0.tar", last modified: Mon Nov 13 11:11:26 2023, max compression
+gzip compressed data, was "kiara_plugin_develop-0.5.1.tar", last modified: Fri Apr 19 10:43:38 2024, max compression
```

## Comparing `kiara_plugin.develop-0.5.0.tar` & `kiara_plugin_develop-0.5.1.tar`

### file list

```diff
@@ -1,196 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.508981 kiara_plugin.develop-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.516981 kiara_plugin.develop-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.508981 kiara_plugin.develop-0.5.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/commitlint.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/docs/development/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/docs/development/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/docs/development/core/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/docs/development/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      516 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/docs/packaging.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/docs/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.508981 kiara_plugin.develop-0.5.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33121 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.520981 kiara_plugin.develop-0.5.0/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/examples/pipelines/example_pipeline_develop.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_models.fbs
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_models.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.524981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.508981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.524981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.524981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.508981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.524981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.524981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.524981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.508981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.524981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33398 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/example_job_{{ cookiecutter.project_slug }}.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/pixi.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.512981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.512981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.512981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.512981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      298 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_kiara_modules_default.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/log.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11081 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/output.txt
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/pixi.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.512981 kiara_plugin.develop-0.5.0/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.528981 kiara_plugin.develop-0.5.0/scripts/development/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1521 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/scripts/development/install_dev_env.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.532981 kiara_plugin.develop-0.5.0/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.512981 kiara_plugin.develop-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.512981 kiara_plugin.develop-0.5.0/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.532981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.532981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/conda/
--rw-r--r--   0 runner    (1001) docker     (127)    20236 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/conda/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/conda/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.532981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.532981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/interfaces/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/interfaces/cli/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/interfaces/cli/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/interfaces/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.532981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/modules/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/modules/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7807 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/templates/flatbuffers/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/templates/flatbuffers/schema_def.fbs.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/templates/meta.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/schema/flatbuffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/schema/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.532981 kiara_plugin.develop-0.5.0/src/kiara_plugin.develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2023-11-13 11:11:26.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin.develop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2023-11-13 11:11:26.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin.develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 11:11:26.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin.develop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-11-13 11:11:26.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin.develop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-13 11:11:26.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin.develop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-13 11:11:26.000000 kiara_plugin.develop-0.5.0/src/kiara_plugin.develop.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:26.536981 kiara_plugin.develop-0.5.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2023-11-13 11:11:16.000000 kiara_plugin.develop-0.5.0/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.239065 kiara_plugin_develop-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.203065 kiara_plugin_develop-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.215065 kiara_plugin_develop-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.215065 kiara_plugin_develop-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-19 10:43:38.239065 kiara_plugin_develop-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.203065 kiara_plugin_develop-0.5.1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.215065 kiara_plugin_develop-0.5.1/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/commitlint.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.215065 kiara_plugin_develop-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.219065 kiara_plugin_develop-0.5.1/docs/development/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.219065 kiara_plugin_develop-0.5.1/docs/development/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/docs/development/core/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/docs/development/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/docs/packaging.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.219065 kiara_plugin_develop-0.5.1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/docs/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.219065 kiara_plugin_develop-0.5.1/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/docs/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.207065 kiara_plugin_develop-0.5.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.219065 kiara_plugin_develop-0.5.1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.219065 kiara_plugin_develop-0.5.1/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33121 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.219065 kiara_plugin_develop-0.5.1/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/examples/jobs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/examples/jobs/simple_1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.219065 kiara_plugin_develop-0.5.1/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/examples/pipelines/example_pipeline_develop.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_models.fbs
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_models.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.223065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.207065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.223065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.223065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.207065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.223065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.223065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.223065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.207065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.223065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.223065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33398 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.223065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/example_job_{{ cookiecutter.project_slug }}.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.223065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/pixi.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.207065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.207065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.207065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.207065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/jobs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      298 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_kiara_modules_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/log.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/pixi.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.211065 kiara_plugin_develop-0.5.1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/scripts/development/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1521 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/scripts/development/install_dev_env.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.227065 kiara_plugin_develop-0.5.1/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:43:38.239065 kiara_plugin_develop-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.211065 kiara_plugin_develop-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.211065 kiara_plugin_develop-0.5.1/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.231065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.231065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.231065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/interfaces/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/interfaces/cli/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/interfaces/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/interfaces/cli/pkg_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.231065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.231065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/modules/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/modules/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.231065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.231065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/conda/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/rattler/
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/rattler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/rattler/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/rattler/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7807 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/templates/flatbuffers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/templates/flatbuffers/schema_def.fbs.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/templates/meta.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/templates/rattler-build-recipe.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/schema/flatbuffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/schema/javascript.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17219 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/utils/pkg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/src/kiara_plugin.develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-19 10:43:38.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin.develop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-04-19 10:43:38.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin.develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:43:38.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin.develop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-19 10:43:38.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin.develop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-19 10:43:38.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin.develop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 10:43:38.000000 kiara_plugin_develop-0.5.1/src/kiara_plugin.develop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/tests/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/tests/resources/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/tests/resources/jobs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:38.235065 kiara_plugin_develop-0.5.1/tests/resources/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/tests/resources/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-04-19 10:43:32.000000 kiara_plugin_develop-0.5.1/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.develop-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin_develop-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin_develop-0.5.1/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/.github/workflows/build-darwin.yaml` & `kiara_plugin_develop-0.5.1/.github/workflows/build-darwin.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 jobs:
   test-darwin:
     name: pytest on darwin
     runs-on: macos-11
     strategy:
       matrix:
-        python_version: ["3.8", "3.9", "3.10", "3.11"]
+        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.develop
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
       - name: Test with pytest
         run: make test
```

### Comparing `kiara_plugin.develop-0.5.0/.github/workflows/build-linux.yaml` & `kiara_plugin_develop-0.5.1/.github/workflows/build-linux.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -4,186 +4,264 @@
 
 jobs:
 
 #  commitlint:
 #    name: lint commit message
 #    runs-on: ubuntu-latest
 #    steps:
-#      - uses: actions/checkout@v3
+#      - uses: actions/checkout@v4
 #        with:
 #          fetch-depth: 0
 #      - uses: wagoid/commitlint-github-action@v4
 
   test-linux:
     name: pytest on linux
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python_version: ["3.8", "3.9", "3.10", "3.11"]
+        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
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
       - name: install kiara_plugin.develop
-        run: pip install -U .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
-      - name: Test with pytest
-        run: make test
+      - name: test with pytest
+        run: pytest --cov-report=xml --cov=kiara_plugin.develop tests
+      - name: Coveralls
+        uses: coverallsapp/github-action@v2
+        with:
+          parallel: true
+          flag-name: run ${{ join(matrix.*, ' - ') }}
+          format: cobertura
+          file: coverage.xml
 
-# Uncomment this if you have coveralls.io setup with this repo
-#  coverage:
-#    name: create and publish test coverage
-#    runs-on: ubuntu-latest
-#    steps:
-#      - name: "Set up Python 3.9"
-#        uses: actions/setup-python@v4
-#        with:
-#          python-version: "3.9"
-#      - uses: actions/checkout@v3
-#      - name: install kiara
-#        run: pip install -U .[all,dev_testing]
-#      - name: display installed kiara and module package versions
-#        run: pip list | grep kiara
-#      - name: Run coverage
-#        run: coverage run -m pytest tests
-#      - name: coveralls
-#        uses: coverallsapp/github-action@v2
+  coverage:
+    name: test coverage
+    runs-on: ubuntu-latest
+    needs:
+      - test-linux
+    steps:
+      - name: Coveralls Finished
+        uses: coverallsapp/github-action@v2
+        with:
+          parallel-finished: true
 
-# Uncomment this if you want to run mypy
   mypy-linux:
     name: mypy check on linux
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python_version: ["3.8", "3.9", "3.10", "3.11"]
+        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
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
       - name: install kiara_plugin.develop
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
         run: ruff --output-format=github src/
 
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
         run: pip install -U pip setuptools setuptools_scm wheel
       - name: install 'build' package
         run: pip install -U build
       - name: create packages
         run: python -m build
       - name: upload artifacts
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: build-dists
           path: dist/
 
   release_python_package:
     name: publish python package to pypi
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     runs-on: ubuntu-latest
     needs:
+      - test-linux
+      - mypy-linux
+      - linting-linux
+      - build_conda_package
       - build_python_package
     env:
         GEMFURY_PUSH_TOKEN: ${{ secrets.GEMFURY_PUSH_TOKEN }}
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
       - name: Retrieve build distributions
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: build-dists
           path: dist/
       - name: publish to PyPI  # make sure you have pypi trusted publishing configured for this repo
         uses: pypa/gh-action-pypi-publish@release/v1
 
-  build_and_release_conda_package:
+  build_conda_package:
     name: conda package build (and upload if release)
     runs-on: ubuntu-latest
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
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+      - name: install kiara
+        run: pip install kiara
+      - name: install required plugin packages
+        run: pip install git+https://github.com/DHARPA-Project/kiara_plugin.develop.git@develop
+      - name: build conda package
+        run: kiara build conda pkg --patch-data ci/conda/conda-pkg-patch.yaml --output-folder build-dir .
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
     needs:
       - test-linux
       - mypy-linux
       - linting-linux
+      - build_python_package
+      - build_conda_package
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
-        with:
-          fetch-depth: 0
+          key: ${{ runner.os }}-pip-3.12
       - name: install kiara
         run: pip install kiara
       - name: install required plugin packages
         run: pip install git+https://github.com/DHARPA-Project/kiara_plugin.develop.git@develop
-      - name: build conda package
-        if: ${{ ( github.ref == 'refs/heads/develop') }}
-        run: kiara conda build-package --patch-data ci/conda/conda-pkg-patch.yaml .
-      - name: extract tag name
-        run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
-      - name: build & publish conda package
-        if: ${{ startsWith(github.ref, 'refs/tags/') }}
-        run: kiara conda build-package --publish --user dharpa --token ${{ secrets.ANACONDA_PUSH_TOKEN }} --patch-data ci/conda/conda-pkg-patch.yaml .
+      - name: Retrieve build distributions
+        uses: actions/download-artifact@v4
+        with:
+          name: conda-pkgs
+          path: build-dir/
+      - name: release conda package
+        run: kiara build conda publish --user dharpa --channel dharpa --token ${{ secrets.ANACONDA_PUSH_TOKEN }} build-dir
+
+#  build_and_release_conda_package:
+#    name: conda package build (and upload if release)
+#    runs-on: ubuntu-latest
+#    needs:
+#      - test-linux
+#      - mypy-linux
+#      - linting-linux
+#    steps:
+#      - name: "Set up Python 3.11"
+#        uses: actions/setup-python@v5
+#        with:
+#          python-version: "3.11"
+#      - name: pip cache
+#        id: pip-cache
+#        uses: actions/cache@v4
+#        with:
+#          path: ~/.cache/pip
+#          key: ${{ runner.os }}-pip-${{ hashFiles('**/setup.*') }}
+#      - uses: actions/checkout@v4
+#        with:
+#          fetch-depth: 0
+#      - name: install kiara
+#        run: pip install kiara
+#      - name: install required plugin packages
+#        run: pip install git+https://github.com/DHARPA-Project/kiara_plugin.develop.git@develop
+#      - name: build conda package
+#        if: ${{ ( github.ref == 'refs/heads/develop') }}
+#        run: kiara build conda pkg --patch-data ci/conda/conda-pkg-patch.yaml .
+#      - name: extract tag name
+#        run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
+#      - name: build & publish conda package
+#        if: ${{ startsWith(github.ref, 'refs/tags/') }}
+#        run: kiara build conda pkg --publish --user dharpa --token ${{ secrets.ANACONDA_PUSH_TOKEN }} --patch-data ci/conda/conda-pkg-patch.yaml .
 
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

### Comparing `kiara_plugin.develop-0.5.0/.github/workflows/build-windows.yaml` & `kiara_plugin_develop-0.5.1/.github/workflows/build-windows.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -12,10 +12,10 @@
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.develop
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: Test with pytest
         run: make test
```

### Comparing `kiara_plugin.develop-0.5.0/.gitignore` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -43,25 +43,25 @@
 cover/*
 MANIFEST
 
 # Per-project virtualenvs
 .venv*/
 pip-wheel-metadata/
 .python-version
-src/kiara_plugin/develop/version.txt
+src/kiara_plugin/{{ cookiecutter.project_slug }}/version.txt
 .direnv
 public
 site
 .dephell_report
 .mypy_cache
 .env
 docs/api-documentation.md
 .frkl
 .envrc
 build.sh
 onefile.spec
 *_complete.zsh.zwc
 ci/conda/**/build
-ci/conda/kiara_plugin.develop/
+ci/conda/kiara_plugin.{{ cookiecutter.project_slug }}/meta.yaml
 .pixi
 pixi.lock
 dev.py
```

### Comparing `kiara_plugin.develop-0.5.0/.pre-commit-config.yaml` & `kiara_plugin_develop-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/LICENSE` & `kiara_plugin_develop-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/Makefile` & `kiara_plugin_develop-0.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/PKG-INFO` & `kiara_plugin_develop-0.5.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.develop
-Version: 0.5.0
+Version: 0.5.1
 Summary: Development utilities for kiara.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.develop
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.develop
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.develop
 Keywords: kiara
@@ -19,21 +19,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: kiara<0.6.0,>=0.5.1
-Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.0
-Requires-Dist: kiara_plugin.tabular<0.6.0,>=0.5.0
-Requires-Dist: kiara_plugin.onboarding<0.6.0,>=0.5.0
+Requires-Dist: kiara<0.6.0,>=0.5.10
+Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.1
+Requires-Dist: build>=1.2.1
 Requires-Dist: diskcache>=5.4.0
 Requires-Dist: httpx>=0.23.0
 Requires-Dist: pydantic-to-typescript>=1.0.10
+Requires-Dist: license-expression>=30.1.0
+Requires-Dist: setuptools>=64
+Requires-Dist: setuptools_scm[toml]>8
+Requires-Dist: wheel
 Provides-Extra: dev-documentation
 Requires-Dist: kiara[dev_documentation]; extra == "dev-documentation"
 Provides-Extra: dev-testing
 Requires-Dist: kiara[dev_testing]; extra == "dev-testing"
 Provides-Extra: dev-utils
 Requires-Dist: kiara[dev_utils]; extra == "dev-utils"
 Provides-Extra: dev-all
@@ -71,80 +74,62 @@
 
 
 ### Prepare development environment
 
 If you only want to work on the modules, and not the core *Kiara* codebase, follow the instructions below. Otherwise, please
 check the notes on how to setup a *Kiara* development environment under (TODO).
 
-#### Linux & Mac OS X (using make)
+#### Using `pixi` (recommended)
 
-For *NIX-like operating system, setting up a development environment is relatively easy:
+The recommended way to setup a development environment is to use [pixi](https://github.com/prefix-dev/pixi). Check out [their install instructions](https://github.com/prefix-dev/pixi#installation).
 
-```console
-git clone https://github.com/DHARPA-Project/kiara_plugin.develop.git
-cd kiara_plugin.develop
-python3 -m venv .venv
-source .venv/bin/activate
-make init
-```
+Once you have `pixi` installed, you need to initialize the environment once:
 
-#### Windows (or manual pip install)
+```
+pixi run install-dev-env
+```
 
-It's impossible to lay out all the ways Python can be installed on a machine, and virtual- (or conda-)envs can be created, so I'll assume you know how to do this.
-One simple way is to install the [Anaconda (individual edition)](https://docs.anaconda.com/anaconda/install/index.html), then use the Anaconda navigator to create a new environment, install the 'git' package in it (if your system does not already have it), and use the 'Open Terminal' option of that environment to start up a terminal that has that virtual-/conda-environment activated.
+You also need to do this whenever a depdendency of this plugin is updated (for example the core `kiara` package).
 
-Once that is done, `cd` into a directory where you want this project folder to live, and do:
+Once that is done, you can enter the environment with:
 
-```console
-# make sure your virtual env is activated!!!
-git clone https://github.com/DHARPA-Project/kiara_plugin.develop.git
-cd kiara_plugin.develop
-pip install --extra-index-url https://pypi.fury.io/dharpa/ -U -e .[all_dev]
+```
+pixi shell
 ```
 
-#### Try it out
-
-After this is done, you should be able to run the included example module via:
+This will start a sub-shell with the virtual environment activated, and all dependencies of the plugin package installed. To confirm it works, you can run any `kiara` command:
 
-```console
-kiara run develop_example text_1="xxx" text_2="yyy"
+```
+kiara --version
+# or
+kiara operation list
+# or
 ...
 ...
 ```
 
-### Re-activate the development environment
-
-The 'prepare' step from above only has to be done once. After that, to re-enable your virtual environment,
-you'll need to navigate to the directory again (wherever that is, in your case), and run the ``source`` command from before again:
+Once you are finished with your development session, you can exit the sub-shell as you would normally do in such cases:
 
-```console
-cd path/to/kiara_plugin.develop
-source .venv/bin/activate  # if it isn't activated already, for example by the Anaconda navigator
-kiara --help  # or whatever, point is, kiara should be available for you now,
+```
+exit
 ```
 
-### ``make`` targets (Linux & Mac OS X)
+Alternatively, you can also run the `kiara` executable directly, it is located in `.pixi/env/bin/kiara`. So either adapt your `PATH` variable, or do something like:
 
-- ``init``: init development project (install project & dev dependencies into virtualenv, as well as pre-commit git hook)
-- ``update-dependencies``: update development dependencies (mainly the core ``kiara`` package from git)
-- ``flake``: run *flake8* tests
-- ``mypy``: run mypy tests
-- ``test``: run unit tests
-- ``docs``: create static documentation pages (under ``build/site``)
-- ``serve-docs``: serve documentation pages (incl. auto-reload) for getting direct feedback when working on documentation
-- ``clean``: clean build directories
+```
+.pixi/env/bin/kiara operation list
+```
 
-For details (and other, minor targets), check the ``Makefile``.
+In most cases it's recommended to use a pixi shell though.
 
 
-### Running tests
+### Using pre-defined development-related tasks
 
-``` console
-> make test
-# or
-> make coverage
-```
+The included `pixi.toml` file includes some useful tasks that help with development:
 
+- `pixi run pre-commit-check`: runs a set of checks against all files
+- `pixi run tests`: runs the unit tests
+- `pixi run mypy`: run mypy checks
 
 ## Copyright & license
 
 This project is MPL v2.0 licensed, for the license text please check the [LICENSE](/LICENSE) file in this repository.
```

### Comparing `kiara_plugin.develop-0.5.0/docs/development/core/index.md` & `kiara_plugin_develop-0.5.1/docs/development/core/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/docs/development/index.md` & `kiara_plugin_develop-0.5.1/docs/development/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/docs/index.md` & `kiara_plugin_develop-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/docs/packaging.md` & `kiara_plugin_develop-0.5.1/docs/packaging.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin_develop-0.5.1/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin_develop-0.5.1/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/examples/pipelines/example_pipeline_develop.yaml` & `kiara_plugin_develop-0.5.1/examples/pipelines/example_pipeline_develop.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 pipeline_name: example_pipeline_develop
 doc: Example pipeline for the develop plugin.
 steps:
   - step_id: add_hello_string
-    module_type: example_proj.example
+    module_type: develop.example
     module_config:
       separator: " "
       constants:
         text_1: "Hello"
       defaults:
         text_2: "World"
   - step_id: add_exclamation_mark
-    module_type: example_proj.example
+    module_type: develop.example
     module_config:
       separator: ""
       constants:
         text_2: "!"
     input_links:
       text_1: add_hello_string.text
```

### Comparing `kiara_plugin.develop-0.5.0/kiara_models.ts` & `kiara_plugin_develop-0.5.1/kiara_models.ts`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 jobs:
   test-darwin:
     name: pytest on darwin
     runs-on: macos-11
     strategy:
       matrix:
-        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+        python_version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - name: "Set up Python {% raw %}${{ matrix.python_version }}{% endraw %}"
         uses: actions/setup-python@v4
         with:
           python-version: "{% raw %}${{ matrix.python_version }}{% endraw %}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.{{ cookiecutter.project_slug }}
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
       - name: Test with pytest
         run: make test
```

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -22,56 +22,54 @@
     steps:
       - name: "Set up Python {% raw %}${{ matrix.python_version }}{% endraw %}"
         uses: actions/setup-python@v4
         with:
           python-version: "{% raw %}${{ matrix.python_version }}{% endraw %}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.{{ cookiecutter.project_slug }}
-        run: pip install -U .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
-      - name: Test with pytest
-        run: make test
+      - name: test with pytest
+        run: pytest --cov-report=xml --cov=kiara_plugin.{{ cookiecutter.project_slug }} tests
+      - name: Coveralls
+        uses: coverallsapp/github-action@v2
+        with:
+          parallel: true
+          flag-name: run {% raw %}${{ join(matrix.*, ' - ') }}{% endraw %}
+          format: cobertura
+          file: coverage.xml
 
-# Uncomment this if you have coveralls.io setup with this repo
-#  coverage:
-#    name: create and publish test coverage
-#    runs-on: ubuntu-latest
-#    steps:
-#      - name: "Set up Python 3.9"
-#        uses: actions/setup-python@v4
-#        with:
-#          python-version: "3.9"
-#      - uses: actions/checkout@v3
-#      - name: install kiara
-#        run: pip install -U .[all,dev_testing]
-#      - name: display installed kiara and module package versions
-#        run: pip list | grep kiara
-#      - name: Run coverage
-#        run: coverage run -m pytest tests
-#      - name: coveralls
-#        uses: coverallsapp/github-action@v2
-
-# Uncomment this if you want to run mypy
-#  mypy-linux:
-#    name: mypy check on linux
-#    runs-on: ubuntu-latest
-#    strategy:
-#      matrix:
-#        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
-#    steps:
-#      - name: "Set up Python {% raw %}${{ matrix.python_version }}{% endraw %}"
-#        uses: actions/setup-python@v4
-#        with:
-#          python-version: "{% raw %}${{ matrix.python_version }}{% endraw %}"
-#      - uses: actions/checkout@v3
-#      - name: install kiara_plugin.{{ cookiecutter.project_slug }}
-#        run: pip install -U .[all,dev_testing]
-#      - name: Test with mypy
-#        run: make mypy
+  coverage:
+    name: test coverage
+    runs-on: ubuntu-latest
+    needs:
+      - test-linux
+    steps:
+      - name: Coveralls Finished
+        uses: coverallsapp/github-action@v2
+        with:
+          parallel-finished: true
+
+  mypy-linux:
+    name: mypy check on linux
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+    steps:
+      - name: "Set up Python {% raw %}${{ matrix.python_version }}{% endraw %}"
+        uses: actions/setup-python@v4
+        with:
+          python-version: "{% raw %}${{ matrix.python_version }}{% endraw %}"
+      - uses: actions/checkout@v3
+      - name: install kiara_plugin.{{ cookiecutter.project_slug }}
+        run: pip install -U .[dev_testing]
+      - name: Test with mypy
+        run: make mypy
 
   linting-linux:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Install Python
         uses: actions/setup-python@v4
@@ -92,16 +90,16 @@
         run: ruff --output-format=github src/
 
   build_python_package:
     name: build python package
     runs-on: ubuntu-latest
     needs:
       - test-linux
-#      - mypy-linux
-#      - linting-linux
+      - mypy-linux
+      - linting-linux
     steps:
       - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
       - uses: actions/checkout@v3
         with:
@@ -134,16 +132,16 @@
         uses: pypa/gh-action-pypi-publish@release/v1
 
   build_and_release_conda_package:
     name: conda package build (and upload if release)
     runs-on: ubuntu-latest
     needs:
       - test-linux
-      # - mypy-linux   # uncomment if this step is enabled
-      # - linting-linux   # uncomment if this step is enabled
+      - mypy-linux
+      - linting-linux
     steps:
       - name: "Set up Python 3.11"
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
       - name: pip cache
         id: pip-cache
```

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/README.md` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -28,80 +28,62 @@
 
 
 ### Prepare development environment
 
 If you only want to work on the modules, and not the core *Kiara* codebase, follow the instructions below. Otherwise, please
 check the notes on how to setup a *Kiara* development environment under (TODO).
 
-#### Linux & Mac OS X (using make)
+#### Using `pixi` (recommended)
 
-For *NIX-like operating system, setting up a development environment is relatively easy:
+The recommended way to setup a development environment is to use [pixi](https://github.com/prefix-dev/pixi). Check out [their install instructions](https://github.com/prefix-dev/pixi#installation).
 
-```console
-git clone https://github.com/{{ cookiecutter.github_user }}/kiara_plugin.{{ cookiecutter.project_slug }}.git
-cd kiara_plugin.{{ cookiecutter.project_slug }}
-python3 -m venv .venv
-source .venv/bin/activate
-make init
-```
+Once you have `pixi` installed, you need to initialize the environment once:
 
-#### Windows (or manual pip install)
+```
+pixi run install-dev-env
+```
 
-It's impossible to lay out all the ways Python can be installed on a machine, and virtual- (or conda-)envs can be created, so I'll assume you know how to do this.
-One simple way is to install the [Anaconda (individual edition)](https://docs.anaconda.com/anaconda/install/index.html), then use the Anaconda navigator to create a new environment, install the 'git' package in it (if your system does not already have it), and use the 'Open Terminal' option of that environment to start up a terminal that has that virtual-/conda-environment activated.
+You also need to do this whenever a depdendency of this plugin is updated (for example the core `kiara` package).
 
-Once that is done, `cd` into a directory where you want this project folder to live, and do:
+Once that is done, you can enter the environment with:
 
-```console
-# make sure your virtual env is activated!!!
-git clone https://github.com/{{ cookiecutter.github_user }}/kiara_plugin.{{ cookiecutter.project_slug }}.git
-cd kiara_plugin.{{ cookiecutter.project_slug }}
-pip install --extra-index-url https://pypi.fury.io/dharpa/ -U -e .[all_dev]
+```
+pixi shell
 ```
 
-#### Try it out
-
-After this is done, you should be able to run the included example module via:
+This will start a sub-shell with the virtual environment activated, and all dependencies of the plugin package installed. To confirm it works, you can run any `kiara` command:
 
-```console
-kiara run {{ cookiecutter.project_slug }}_example text_1="xxx" text_2="yyy"
+```
+kiara --version
+# or
+kiara operation list
+# or
 ...
 ...
 ```
 
-### Re-activate the development environment
-
-The 'prepare' step from above only has to be done once. After that, to re-enable your virtual environment,
-you'll need to navigate to the directory again (wherever that is, in your case), and run the ``source`` command from before again:
+Once you are finished with your development session, you can exit the sub-shell as you would normally do in such cases:
 
-```console
-cd path/to/kiara_plugin.{{ cookiecutter.project_slug }}
-source .venv/bin/activate  # if it isn't activated already, for example by the Anaconda navigator
-kiara --help  # or whatever, point is, kiara should be available for you now,
+```
+exit
 ```
 
-### ``make`` targets (Linux & Mac OS X)
+Alternatively, you can also run the `kiara` executable directly, it is located in `.pixi/env/bin/kiara`. So either adapt your `PATH` variable, or do something like:
 
-- ``init``: init development project (install project & dev dependencies into virtualenv, as well as pre-commit git hook)
-- ``update-dependencies``: update development dependencies (mainly the core ``kiara`` package from git)
-- ``flake``: run *flake8* tests
-- ``mypy``: run mypy tests
-- ``test``: run unit tests
-- ``docs``: create static documentation pages (under ``build/site``)
-- ``serve-docs``: serve documentation pages (incl. auto-reload) for getting direct feedback when working on documentation
-- ``clean``: clean build directories
+```
+.pixi/env/bin/kiara operation list
+```
 
-For details (and other, minor targets), check the ``Makefile``.
+In most cases it's recommended to use a pixi shell though.
 
 
-### Running tests
+### Using pre-defined development-related tasks
 
-``` console
-> make test
-# or
-> make coverage
-```
+The included `pixi.toml` file includes some useful tasks that help with development:
 
+- `pixi run pre-commit-check`: runs a set of checks against all files
+- `pixi run tests`: runs the unit tests
+- `pixi run mypy`: run mypy checks
 
 ## Copyright & license
 
 This project is MPL v2.0 licensed, for the license text please check the [LICENSE](/LICENSE) file in this repository.
```

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 pipeline_name: example_pipeline_{{ cookiecutter.project_slug }}
 doc: Example pipeline for the {{ cookiecutter.project_slug }} plugin.
 steps:
   - step_id: add_hello_string
-    module_type: example_proj.example
+    module_type: {{ cookiecutter.project_slug }}.example
     module_config:
       separator: " "
       constants:
         text_1: "Hello"
       defaults:
         text_2: "World"
   - step_id: add_exclamation_mark
-    module_type: example_proj.example
+    module_type: {{ cookiecutter.project_slug }}.example
     module_config:
       separator: ""
       constants:
         text_2: "!"
     input_links:
       text_1: add_hello_string.text
```

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/pixi.toml` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/pixi.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [project]
 name = "kiara-plugin-{{ cookiecutter.project_slug }}"
 version = "0.1.0"
 description = "{{ cookiecutter.project_short_description }}"
 authors = ["{{ cookiecutter.full_name }} <{{ cookiecutter.email }}>"]
-channels = ["conda-forge", "dharpa"]
+channels = ["dharpa", "conda-forge"]
 platforms = ["linux-64", "win-64", "osx-64", "osx-arm64"]
 
 [tasks]
-install-dev-env = "pip install -e '.[dev_utils]'
+install-dev-env = "pip install --upgrade -e '.[dev_utils]'"
 pre-commit-check = ".pixi/env/bin/pre-commit run --all-files"
+tests = "py.test"
+mypy = "mypy  --namespace-packages --explicit-package-base src/kiara_plugin/{{ cookiecutter.project_slug }}"
 kiara = ".pixi/env/bin/kiara"
 show-versions = ".pixi/env/bin/kiara --version"
 delete-context = ".pixi/env/bin/kiara context delete"
+install-dev-dependency = ".pixi/env/bin/pip install -e"
 
 [dependencies]
 python = "3.11.*"
 pip = "23.3.*"
```

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
-    "kiara>=0.5.1,<0.6.0",
+    "kiara>=0.5.10rc10,<0.6.0",
     "kiara_plugin.core_types>=0.5.0,<0.6.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]"
@@ -235,9 +235,13 @@
 plugins = [
     "pydantic.mypy"
 ]
 
 
 # mypy per-module options:
 [[tool.mypy.overrides]]
-module = ["placholder.dummy.*"]
+module = [
+    "appdirs.*",
+    "pyarrow.*",
+    "ruamel.*"
+]
 ignore_missing_imports = true
```

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py` & `kiara_plugin_develop-0.5.1/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,53 +13,80 @@
 import os
 import tempfile
 import uuid
 from pathlib import Path
 
 import pytest
 
+from kiara.api import JobDesc, KiaraAPI
 from kiara.context import KiaraConfig
-from kiara.interfaces.python_api import KiaraAPI
+from kiara.interfaces.python_api.base_api import BaseAPI
 from kiara.interfaces.python_api.models.job import JobTest
-from kiara.utils.testing import get_tests_for_job, list_job_descs
+from kiara.utils.testing import get_init_job, get_tests_for_job, list_job_descs
 
 ROOT_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
-JOBS_FOLDER = Path(os.path.join(ROOT_DIR, "examples", "jobs"))
-
+JOBS_FOLDERS = [Path(os.path.join(ROOT_DIR, "tests", "resources", "jobs")), Path(os.path.join(ROOT_DIR, "examples", "jobs"))]
 
 def create_temp_dir():
     session_id = str(uuid.uuid4())
     TEMP_DIR = Path(os.path.join(tempfile.gettempdir(), "kiara_tests"))
 
     instance_path = os.path.join(
         TEMP_DIR.resolve().absolute(), f"instance_{session_id}"
     )
     return instance_path
 
+def get_job_alias(job_desc: JobDesc) -> str:
+    return job_desc.job_alias
 
 @pytest.fixture
-def kiara_api() -> KiaraAPI:
+def kiara_api() -> BaseAPI:
 
     instance_path = create_temp_dir()
     kc = KiaraConfig.create_in_folder(instance_path)
-    api = KiaraAPI(kc)
+    api = BaseAPI(kc)
     return api
 
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
 
-@pytest.fixture(params=list_job_descs(JOBS_FOLDER))
-def example_job_test(request, kiara_api) -> JobTest:
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

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/mkdocs.yml` & `kiara_plugin_develop-0.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/pyproject.toml` & `kiara_plugin_develop-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -43,21 +43,24 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
-    "kiara>=0.5.1,<0.6.0",
-    "kiara_plugin.core_types>=0.5.0,<0.6.0",
-    "kiara_plugin.tabular>=0.5.0,<0.6.0",
-    "kiara_plugin.onboarding>=0.5.0,<0.6.0",
+    "kiara>=0.5.10,<0.6.0",
+    "kiara_plugin.core_types>=0.5.1,<0.6.0",
+    "build>=1.2.1",
     "diskcache>=5.4.0",
     "httpx>=0.23.0",
-    "pydantic-to-typescript>=1.0.10"
+    "pydantic-to-typescript>=1.0.10",
+    "license-expression>=30.1.0",
+    "setuptools>=64",
+    "setuptools_scm[toml]>8",
+    "wheel"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]",
 ]
@@ -76,15 +79,16 @@
 
 [project.entry-points."kiara.plugin"]
 develop = "kiara_plugin.develop"
 
 [project.entry-points."kiara.cli_subcommands"]
 debug = "kiara_plugin.develop.interfaces.cli.debug:debug"
 dev = "kiara_plugin.develop.interfaces.cli.dev:dev_group"
-conda = "kiara_plugin.develop.interfaces.cli.conda:conda"
+#conda = "kiara_plugin.develop.interfaces.cli.conda:conda"
+build = "kiara_plugin.develop.interfaces.cli.pkg_build:pkg_build"
 
 
 [project.entry-points."kiara.data_types"]
 develop = "kiara_plugin.develop:find_data_types"
 
 [project.entry-points."kiara.model_classes"]
 develop = "kiara_plugin.develop:find_model_classes"
@@ -249,11 +253,15 @@
 ]
 
 
 # mypy per-module options:
 [[tool.mypy.overrides]]
 module = [
     "appdirs.*",
+    "build.*",
     "diskcache.*",
-    "pydantic2ts.*"
+    "license_expression.*",
+    "pydantic2ts.*",
+    "pyarrow.*",
+    "ruamel.*"
 ]
 ignore_missing_imports = true
```

### Comparing `kiara_plugin.develop-0.5.0/scripts/development/install_dev_env.sh` & `kiara_plugin_develop-0.5.1/scripts/development/install_dev_env.sh`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin_develop-0.5.1/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/scripts/documentation/gen_info_pages.py` & `kiara_plugin_develop-0.5.1/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/scripts/documentation/gen_module_doc.py` & `kiara_plugin_develop-0.5.1/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/__init__.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/conda/models.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/rattler/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     model_config = ConfigDict(extra=Extra.forbid)
 
     pkg_name: str = Field(description="The package name.")
     pkg_version: str = Field(
         description="The package version, either version number, or git branch/tag."
     )
     pkg_url: str = Field(description="The package url.")
+    pkg_is_local: bool = Field(description="Is the package a local project.", default=False)
     pkg_hash: Union[str, None] = Field(
         description="The package hash (sha256), if not git url.", default=None
     )
     host_requirements: List[str] = Field(
         description="The host dependencies for this package.",
         default_factory=DEFAULT_HOST_DEPENDENCIES,
     )
@@ -135,14 +136,20 @@
 
     def create_conda_spec(self) -> str:
 
         template = self.jinja_environment().get_template("meta.yaml.j2")
         result: str = template.render(pkg_info=self)
         return result
 
+    def create_rattler_build_recipe(self) -> str:
+
+        template = self.jinja_environment().get_template("rattler-build-recipe.yaml.j2")
+        result: str = template.render(pkg_info=self)
+        return result
+
 
 class RunDetails(BaseModel):
 
     cmd: str = Field(description="The command that was run.")
     args: List[str] = Field(description="The arguments to the command.")
     exit_code: int = Field(description="The command exit code.")
     stdout: str = Field(description="The command output.")
@@ -152,7 +159,16 @@
 class CondaBuildPackageDetails(RunDetails):
 
     base_dir: str = Field(description="The base directory.")
     build_dir: str = Field(description="The build directory.")
     meta_file: str = Field(description="The path to the package meta file.")
     package: PkgSpec = Field(description="Package metadata.")
     build_artifact: str = Field(description="Path to the package build artifact.")
+
+class RattlerBuildPackageDetails(BaseModel):
+
+    run_details: List[RunDetails] = Field(description="The run details.")
+    base_dir: str = Field(description="The base directory.")
+    build_dir: str = Field(description="The build directory.")
+    meta_file: str = Field(description="The path to the package meta file.")
+    package: PkgSpec = Field(description="Package metadata.")
+    build_artifacts: List[str] = Field(description="Path to the package build artifacts.")
```

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/conda/states.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/pkg_build/conda/states.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,118 +1,23 @@
 # -*- coding: utf-8 -*-
-import abc
 import io
 import json
 import os
 import platform
 import shutil
 import subprocess
 import tarfile
 import tempfile
 import urllib
 from pathlib import Path
 from typing import Any, Dict, List, Mapping, Union
 
 from kiara.utils.cli import terminal_print
 from kiara_plugin.develop.defaults import KIARA_DEV_MICROMAMBA_TARGET_PREFIX
-
-
-class State(abc.ABC):
-    def __init__(self, state_id: str, **config):
-
-        self._state_id: str = state_id
-        self._config: Mapping[str, Any] = config
-        self._states: Union[None, "States"] = None
-        self._state_details: Union[None, Mapping[str, None]] = None
-
-    @property
-    def state_id(self):
-        return self._state_id
-
-    def ensure_state(self, state_id: str):
-
-        if self._states is None:
-            raise Exception("States not set (yet). This is a bug.")
-
-        self._states.get_state(state_id).resolve()
-
-    def get_other_state_detail(self, state_id: str, key: str):
-
-        if self._states is None:
-            raise Exception("States not set (yet). This is a bug.")
-
-        return self._states.get_state(state_id).get_detail(key)
-
-    def get_config(self, key: str) -> Any:
-
-        if key not in self._config.keys():
-            raise Exception(
-                f"No config key '{key}' in state type '{self.__class__.__name__}'."
-            )
-        return self._config[key]
-
-    def resolve(self) -> Mapping[str, Any]:
-
-        if self._state_details is not None:
-            return self._state_details
-
-        self._state_details = self._resolve()
-        if self._state_details is None:
-            raise Exception(
-                f"No state details for: {self.__class__.__name__}. This is a bug."
-            )
-        return self._state_details
-
-    def purge(self):
-
-        self._purge()
-        self._state_details = None
-
-    @abc.abstractmethod
-    def _resolve(self) -> Mapping[str, Any]:
-        pass
-
-    @abc.abstractmethod
-    def _purge(self):
-        pass
-
-    def get_detail(self, key: str):
-
-        details = self.resolve()
-        return details[key]
-
-    def get_details(self) -> Mapping[str, Any]:
-        return self.resolve()
-
-
-class States(object):
-    def __init__(self) -> None:
-
-        self._states: Dict[str, State] = {}
-
-    def add_state(self, state: State):
-
-        if state.state_id in self._states.keys():
-            raise Exception(
-                f"Can't add state with id '{state.state_id}: id already registered."
-            )
-        self._states[state.state_id] = state
-        state._states = self
-
-    def resolve(self, state_id: str):
-        self._states[state_id].resolve()
-
-    def get_state(self, state_id: str):
-        return self._states[state_id]
-
-    def get_state_detail(self, state_id: str, key: str):
-        return self._states[state_id].get_detail(key)
-
-    def get_state_details(self, state_id: str) -> Mapping[str, Any]:
-        return self._states[state_id].get_details()
+from kiara_plugin.develop.pkg_build.states import State
 
 
 class MicroMambaAvailable(State):
     def _check(self) -> Union[None, Mapping[str, Any]]:
 
         root_path: str = self.get_config("root_path")
         bin_path = os.path.join(root_path, "bin", "micromamba")
```

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/data_types.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/data_types.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/defaults.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/models.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/modules/__init__.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/modules/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/templates/meta.yaml.j2` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/templates/meta.yaml.j2`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/schema/__init__.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/schema/flatbuffers.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/schema/flatbuffers.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/schema/javascript.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/schema/javascript.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin/develop/utils.py` & `kiara_plugin_develop-0.5.1/src/kiara_plugin/develop/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
 # helper function, from: https://gist.github.com/thelinuxkid/5114777
+import os
 import selectors
 import subprocess
 from pathlib import Path
 from subprocess import Popen
-from typing import Callable, Generator, Union
+from typing import TYPE_CHECKING, Callable, Generator, Union
 
-from kiara_plugin.develop.conda import RunDetails
+if TYPE_CHECKING:
+    from kiara_plugin.develop.pkg_build.models import RunDetails
 
 newlines = ["\n", "\r\n", "\r"]
 
 
 def unbuffered(
     proc: Popen, stdout_prefix: str = "", stderr_prefix: str = ""
 ) -> Generator[str, None, None]:
@@ -50,41 +52,50 @@
         else:
             continue
 
         break
 
 
 class ExecutionException(Exception):
-    def __init__(self, msg, run_details: RunDetails):
+    def __init__(self, msg, run_details: "RunDetails"):
         self._run_details = run_details
         super().__init__(msg)
 
     @property
-    def run_details(self) -> RunDetails:
+    def run_details(self) -> "RunDetails":
         return self._run_details
 
 
 def execute(
     cmd: str,
     *args: str,
     stdout_callback: Union[Callable, None] = None,
     stderr_callback: Union[Callable, None] = None,
     cwd: Union[None, str, Path] = None,
-) -> RunDetails:
+    env_vars: Union[None, dict] = None,
+) -> "RunDetails":
+
+    from kiara_plugin.develop.pkg_build.models import RunDetails
 
     stdout_output = []
     stderr_output = []
     _args = list(args)
+
+    process_env_vars = os.environ.copy()
+    if env_vars:
+        process_env_vars.update(env_vars)
+
     with subprocess.Popen(
         [cmd,*_args],
         shell=False,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         universal_newlines=True,
         cwd=cwd,
+        env=process_env_vars
     ) as proc:
         for line in unbuffered(proc, stdout_prefix="o-", stderr_prefix="e-"):
             if line.startswith("o-"):
                 _line = line[2:]
                 if stdout_callback:
                     stdout_callback(_line)
                 stdout_output.append(_line)
```

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin.develop.egg-info/PKG-INFO` & `kiara_plugin_develop-0.5.1/src/kiara_plugin.develop.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kiara-plugin.develop
-Version: 0.5.0
+Name: kiara_plugin.develop
+Version: 0.5.1
 Summary: Development utilities for kiara.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.develop
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.develop
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.develop
 Keywords: kiara
@@ -19,21 +19,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: kiara<0.6.0,>=0.5.1
-Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.0
-Requires-Dist: kiara_plugin.tabular<0.6.0,>=0.5.0
-Requires-Dist: kiara_plugin.onboarding<0.6.0,>=0.5.0
+Requires-Dist: kiara<0.6.0,>=0.5.10
+Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.1
+Requires-Dist: build>=1.2.1
 Requires-Dist: diskcache>=5.4.0
 Requires-Dist: httpx>=0.23.0
 Requires-Dist: pydantic-to-typescript>=1.0.10
+Requires-Dist: license-expression>=30.1.0
+Requires-Dist: setuptools>=64
+Requires-Dist: setuptools_scm[toml]>8
+Requires-Dist: wheel
 Provides-Extra: dev-documentation
 Requires-Dist: kiara[dev_documentation]; extra == "dev-documentation"
 Provides-Extra: dev-testing
 Requires-Dist: kiara[dev_testing]; extra == "dev-testing"
 Provides-Extra: dev-utils
 Requires-Dist: kiara[dev_utils]; extra == "dev-utils"
 Provides-Extra: dev-all
@@ -71,80 +74,62 @@
 
 
 ### Prepare development environment
 
 If you only want to work on the modules, and not the core *Kiara* codebase, follow the instructions below. Otherwise, please
 check the notes on how to setup a *Kiara* development environment under (TODO).
 
-#### Linux & Mac OS X (using make)
+#### Using `pixi` (recommended)
 
-For *NIX-like operating system, setting up a development environment is relatively easy:
+The recommended way to setup a development environment is to use [pixi](https://github.com/prefix-dev/pixi). Check out [their install instructions](https://github.com/prefix-dev/pixi#installation).
 
-```console
-git clone https://github.com/DHARPA-Project/kiara_plugin.develop.git
-cd kiara_plugin.develop
-python3 -m venv .venv
-source .venv/bin/activate
-make init
-```
+Once you have `pixi` installed, you need to initialize the environment once:
 
-#### Windows (or manual pip install)
+```
+pixi run install-dev-env
+```
 
-It's impossible to lay out all the ways Python can be installed on a machine, and virtual- (or conda-)envs can be created, so I'll assume you know how to do this.
-One simple way is to install the [Anaconda (individual edition)](https://docs.anaconda.com/anaconda/install/index.html), then use the Anaconda navigator to create a new environment, install the 'git' package in it (if your system does not already have it), and use the 'Open Terminal' option of that environment to start up a terminal that has that virtual-/conda-environment activated.
+You also need to do this whenever a depdendency of this plugin is updated (for example the core `kiara` package).
 
-Once that is done, `cd` into a directory where you want this project folder to live, and do:
+Once that is done, you can enter the environment with:
 
-```console
-# make sure your virtual env is activated!!!
-git clone https://github.com/DHARPA-Project/kiara_plugin.develop.git
-cd kiara_plugin.develop
-pip install --extra-index-url https://pypi.fury.io/dharpa/ -U -e .[all_dev]
+```
+pixi shell
 ```
 
-#### Try it out
-
-After this is done, you should be able to run the included example module via:
+This will start a sub-shell with the virtual environment activated, and all dependencies of the plugin package installed. To confirm it works, you can run any `kiara` command:
 
-```console
-kiara run develop_example text_1="xxx" text_2="yyy"
+```
+kiara --version
+# or
+kiara operation list
+# or
 ...
 ...
 ```
 
-### Re-activate the development environment
-
-The 'prepare' step from above only has to be done once. After that, to re-enable your virtual environment,
-you'll need to navigate to the directory again (wherever that is, in your case), and run the ``source`` command from before again:
+Once you are finished with your development session, you can exit the sub-shell as you would normally do in such cases:
 
-```console
-cd path/to/kiara_plugin.develop
-source .venv/bin/activate  # if it isn't activated already, for example by the Anaconda navigator
-kiara --help  # or whatever, point is, kiara should be available for you now,
+```
+exit
 ```
 
-### ``make`` targets (Linux & Mac OS X)
+Alternatively, you can also run the `kiara` executable directly, it is located in `.pixi/env/bin/kiara`. So either adapt your `PATH` variable, or do something like:
 
-- ``init``: init development project (install project & dev dependencies into virtualenv, as well as pre-commit git hook)
-- ``update-dependencies``: update development dependencies (mainly the core ``kiara`` package from git)
-- ``flake``: run *flake8* tests
-- ``mypy``: run mypy tests
-- ``test``: run unit tests
-- ``docs``: create static documentation pages (under ``build/site``)
-- ``serve-docs``: serve documentation pages (incl. auto-reload) for getting direct feedback when working on documentation
-- ``clean``: clean build directories
+```
+.pixi/env/bin/kiara operation list
+```
 
-For details (and other, minor targets), check the ``Makefile``.
+In most cases it's recommended to use a pixi shell though.
 
 
-### Running tests
+### Using pre-defined development-related tasks
 
-``` console
-> make test
-# or
-> make coverage
-```
+The included `pixi.toml` file includes some useful tasks that help with development:
 
+- `pixi run pre-commit-check`: runs a set of checks against all files
+- `pixi run tests`: runs the unit tests
+- `pixi run mypy`: run mypy checks
 
 ## Copyright & license
 
 This project is MPL v2.0 licensed, for the license text please check the [LICENSE](/LICENSE) file in this repository.
```

### Comparing `kiara_plugin.develop-0.5.0/src/kiara_plugin.develop.egg-info/SOURCES.txt` & `kiara_plugin_develop-0.5.1/src/kiara_plugin.develop.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 commitlint.config.js
 cookiecutter.json
 environment.yaml
 kiara_models.fbs
 kiara_models.ts
 log.txt
 mkdocs.yml
-output.txt
 pixi.toml
 pyproject.toml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/suggest-a-module.md
 .github/workflows/build-darwin.yaml
 .github/workflows/build-linux.yaml
 .github/workflows/build-windows.yaml
@@ -34,14 +33,15 @@
 docs/stylesheets/extra.css
 docs/usage/index.md
 examples/data/Readme.md
 examples/data/journals/JournalEdges1902.csv
 examples/data/journals/JournalNodes1902.csv
 examples/data/journals/Readme.md
 examples/jobs/Readme.md
+examples/jobs/simple_1.yaml
 examples/pipelines/Readme.md
 examples/pipelines/example_pipeline_develop.yaml
 kiara_plugin.{{ cookiecutter.project_slug }}/.envrc.disabled
 kiara_plugin.{{ cookiecutter.project_slug }}/.git_archival.txt
 kiara_plugin.{{ cookiecutter.project_slug }}/.gitattributes
 kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore
 kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml
@@ -87,14 +87,16 @@
 kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/.gitkeep
 kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py
 kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py
 kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_kiara_modules_default.py
 kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py
 kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.yaml
 kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/.gitkeep
+kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/jobs/.gitkeep
+kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/pipelines/.gitkeep
 scripts/development/install_dev_env.sh
 scripts/documentation/gen_api_doc_pages.py
 scripts/documentation/gen_info_pages.py
 scripts/documentation/gen_module_doc.py
 src/kiara_plugin.develop.egg-info/PKG-INFO
 src/kiara_plugin.develop.egg-info/SOURCES.txt
 src/kiara_plugin.develop.egg-info/dependency_links.txt
@@ -102,32 +104,41 @@
 src/kiara_plugin.develop.egg-info/requires.txt
 src/kiara_plugin.develop.egg-info/top_level.txt
 src/kiara_plugin/develop/__init__.py
 src/kiara_plugin/develop/data_types.py
 src/kiara_plugin/develop/defaults.py
 src/kiara_plugin/develop/models.py
 src/kiara_plugin/develop/py.typed
-src/kiara_plugin/develop/utils.py
-src/kiara_plugin/develop/conda/__init__.py
-src/kiara_plugin/develop/conda/models.py
-src/kiara_plugin/develop/conda/states.py
 src/kiara_plugin/develop/interfaces/__init__.py
 src/kiara_plugin/develop/interfaces/cli/__init__.py
-src/kiara_plugin/develop/interfaces/cli/conda.py
 src/kiara_plugin/develop/interfaces/cli/debug.py
 src/kiara_plugin/develop/interfaces/cli/dev.py
+src/kiara_plugin/develop/interfaces/cli/pkg_build.py
 src/kiara_plugin/develop/modules/__init__.py
 src/kiara_plugin/develop/modules/pipelines/__init__.py
 src/kiara_plugin/develop/pipelines/.gitkeep
 src/kiara_plugin/develop/pipelines/__init__.py
+src/kiara_plugin/develop/pkg_build/__init__.py
+src/kiara_plugin/develop/pkg_build/models.py
+src/kiara_plugin/develop/pkg_build/states.py
+src/kiara_plugin/develop/pkg_build/conda/__init__.py
+src/kiara_plugin/develop/pkg_build/conda/states.py
+src/kiara_plugin/develop/pkg_build/rattler/__init__.py
+src/kiara_plugin/develop/pkg_build/rattler/models.py
+src/kiara_plugin/develop/pkg_build/rattler/states.py
 src/kiara_plugin/develop/resources/.gitkeep
 src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh
 src/kiara_plugin/develop/resources/templates/meta.yaml.j2
+src/kiara_plugin/develop/resources/templates/rattler-build-recipe.yaml.j2
 src/kiara_plugin/develop/resources/templates/recipe.yaml.j2
 src/kiara_plugin/develop/resources/templates/flatbuffers/schema_def.fbs.j2
 src/kiara_plugin/develop/schema/__init__.py
 src/kiara_plugin/develop/schema/flatbuffers.py
 src/kiara_plugin/develop/schema/javascript.py
+src/kiara_plugin/develop/utils/__init__.py
+src/kiara_plugin/develop/utils/pkg_utils.py
 tests/conftest.py
 tests/test_job_descs.py
 tests/test_kiara_modules_default.py
-tests/resources/.gitkeep
+tests/resources/.gitkeep
+tests/resources/jobs/.gitkeep
+tests/resources/pipelines/.gitkeep
```

### Comparing `kiara_plugin.develop-0.5.0/tests/conftest.py` & `kiara_plugin_develop-0.5.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,52 +14,78 @@
 import tempfile
 import uuid
 from pathlib import Path
 
 import pytest
 
 from kiara.context import KiaraConfig
-from kiara.interfaces.python_api import KiaraAPI
+from kiara.api import KiaraAPI, JobDesc
 from kiara.interfaces.python_api.models.job import JobTest
-from kiara.utils.testing import get_tests_for_job, list_job_descs
+from kiara.utils.testing import get_tests_for_job, list_job_descs, get_init_job
 
 ROOT_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
-JOBS_FOLDER = Path(os.path.join(ROOT_DIR, "examples", "jobs"))
-
+JOBS_FOLDERS = [Path(os.path.join(ROOT_DIR, "tests", "resources", "jobs")), Path(os.path.join(ROOT_DIR, "examples", "jobs"))]
 
 def create_temp_dir():
     session_id = str(uuid.uuid4())
     TEMP_DIR = Path(os.path.join(tempfile.gettempdir(), "kiara_tests"))
 
     instance_path = os.path.join(
         TEMP_DIR.resolve().absolute(), f"instance_{session_id}"
     )
     return instance_path
 
+def get_job_alias(job_desc: JobDesc) -> str:
+    return job_desc.job_alias
 
 @pytest.fixture
 def kiara_api() -> KiaraAPI:
 
     instance_path = create_temp_dir()
     kc = KiaraConfig.create_in_folder(instance_path)
     api = KiaraAPI(kc)
     return api
 
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
 
-@pytest.fixture(params=list_job_descs(JOBS_FOLDER))
-def example_job_test(request, kiara_api) -> JobTest:
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

### Comparing `kiara_plugin.develop-0.5.0/tests/test_job_descs.py` & `kiara_plugin_develop-0.5.1/tests/test_job_descs.py`

 * *Files identical despite different names*

