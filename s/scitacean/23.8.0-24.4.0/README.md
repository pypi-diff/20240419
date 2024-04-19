# Comparing `tmp/scitacean-23.8.0.tar.gz` & `tmp/scitacean-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scitacean-23.8.0.tar", last modified: Mon Aug 28 12:37:17 2023, max compression
+gzip compressed data, was "scitacean-24.4.0.tar", last modified: Fri Apr 19 13:49:21 2024, max compression
```

## Comparing `scitacean-23.8.0.tar` & `scitacean-24.4.0.tar`

### file list

```diff
@@ -1,216 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.047668 scitacean-23.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.015668 scitacean-23.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (999)      278 2023-08-28 12:37:04.000000 scitacean-23.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.019668 scitacean-23.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)     1683 2023-08-28 12:37:04.000000 scitacean-23.8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (999)      581 2023-08-28 12:37:04.000000 scitacean-23.8.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (999)      885 2023-08-28 12:37:04.000000 scitacean-23.8.0/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1035 2023-08-28 12:37:04.000000 scitacean-23.8.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1203 2023-08-28 12:37:04.000000 scitacean-23.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (999)      282 2023-08-28 12:37:04.000000 scitacean-23.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)     1171 2023-08-28 12:37:04.000000 scitacean-23.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     5224 2023-08-28 12:37:04.000000 scitacean-23.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (999)     1005 2023-08-28 12:37:04.000000 scitacean-23.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (999)     1522 2023-08-28 12:37:04.000000 scitacean-23.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 12:37:04.000000 scitacean-23.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     4278 2023-08-28 12:37:17.047668 scitacean-23.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1447 2023-08-28 12:37:04.000000 scitacean-23.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (999)      656 2023-08-28 12:37:04.000000 scitacean-23.8.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.019668 scitacean-23.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (999)       29 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.019668 scitacean-23.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (999)     4602 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/_static/anaconda-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.019668 scitacean-23.8.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (999)     2605 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (999)    15406 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (999)     8270 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (999)     6814 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.019668 scitacean-23.8.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (999)     1493 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/_templates/scitacean-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1270 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/_templates/scitacean-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (999)     6565 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.023668 scitacean-23.8.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (999)     3850 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/developer/coding-conventions.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1061 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/developer/dependency-management.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2554 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/developer/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (999)      236 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2515 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/developer/testing.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1542 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.023668 scitacean-23.8.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (999)     1439 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     5198 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/release-notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.023668 scitacean-23.8.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (999)     6222 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/user-guide/classes-and-concepts.rst
--rw-r--r--   0 runner    (1001) docker     (999)     9028 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/user-guide/downloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)      132 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)      347 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/user-guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (999)    10241 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/user-guide/logo.png
--rw-r--r--   0 runner    (1001) docker     (999)    24036 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/user-guide/testing.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)    12750 2023-08-28 12:37:04.000000 scitacean-23.8.0/docs/user-guide/uploading.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)     3267 2023-08-28 12:37:04.000000 scitacean-23.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.027668 scitacean-23.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (999)      124 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (999)     1124 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (999)      593 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (999)      214 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (999)     2567 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (999)      269 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (999)     4231 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (999)      589 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (999)       83 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (999)      788 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (999)        6 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (999)      266 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.031668 scitacean-23.8.0/requirements-pydantic2/
--rw-r--r--   0 runner    (1001) docker     (999)       71 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements-pydantic2/base.in
--rw-r--r--   0 runner    (1001) docker     (999)     1292 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements-pydantic2/base.txt
--rw-r--r--   0 runner    (1001) docker     (999)       83 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements-pydantic2/test.in
--rw-r--r--   0 runner    (1001) docker     (999)      858 2023-08-28 12:37:04.000000 scitacean-23.8.0/requirements-pydantic2/test.txt
--rw-r--r--   0 runner    (1001) docker     (999)      198 2023-08-28 12:37:17.047668 scitacean-23.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.007668 scitacean-23.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.031668 scitacean-23.8.0/src/scitacean/
--rw-r--r--   0 runner    (1001) docker     (999)      965 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    12971 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_base_model.py
--rw-r--r--   0 runner    (1001) docker     (999)    46147 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_dataset_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.031668 scitacean-23.8.0/src/scitacean/_html_repr/
--rw-r--r--   0 runner    (1001) docker     (999)      931 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2279 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/_attachment_html.py
--rw-r--r--   0 runner    (1001) docker     (999)     1873 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/_common_html.py
--rw-r--r--   0 runner    (1001) docker     (999)     6229 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/_dataset_html.py
--rw-r--r--   0 runner    (1001) docker     (999)     2328 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.035668 scitacean-23.8.0/src/scitacean/_html_repr/images/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2434 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/images/lock.svg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.035668 scitacean-23.8.0/src/scitacean/_html_repr/styles/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2097 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/styles/attachment.css
--rw-r--r--   0 runner    (1001) docker     (999)     3231 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/styles/dataset.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.035668 scitacean-23.8.0/src/scitacean/_html_repr/templates/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      220 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/templates/attachment_field_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (999)      825 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/templates/attachment_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (999)      309 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/templates/dataset_field_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (999)     1650 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/templates/dataset_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (999)      182 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/templates/files_repr.html.template
--rw-r--r--   0 runner    (1001) docker     (999)      126 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_html_repr/templates/metadata_repr.html.template
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.035668 scitacean-23.8.0/src/scitacean/_internal/
--rw-r--r--   0 runner    (1001) docker     (999)      121 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1188 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_internal/dataclass_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (999)     1786 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_internal/docker.py
--rw-r--r--   0 runner    (1001) docker     (999)     3043 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_internal/file_counter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1008 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_internal/orcid.py
--rw-r--r--   0 runner    (1001) docker     (999)      582 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/_internal/pydantic_compat.py
--rw-r--r--   0 runner    (1001) docker     (999)    34094 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/client.py
--rw-r--r--   0 runner    (1001) docker     (999)     4934 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/datablock.py
--rw-r--r--   0 runner    (1001) docker     (999)    16832 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/dataset.py
--rw-r--r--   0 runner    (1001) docker     (999)      501 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/error.py
--rw-r--r--   0 runner    (1001) docker     (999)    15172 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/file.py
--rw-r--r--   0 runner    (1001) docker     (999)     9441 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (999)      567 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/logging.py
--rw-r--r--   0 runner    (1001) docker     (999)    28542 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/model.py
--rw-r--r--   0 runner    (1001) docker     (999)     4547 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/pid.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.035668 scitacean-23.8.0/src/scitacean/testing/
--rw-r--r--   0 runner    (1001) docker     (999)      169 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1771 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/_pytest_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.035668 scitacean-23.8.0/src/scitacean/testing/backend/
--rw-r--r--   0 runner    (1001) docker     (999)     2752 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3521 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/backend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (999)     1310 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/backend/_pytest_helpers.py
--rw-r--r--   0 runner    (1001) docker     (999)     3058 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     1339 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/backend/docker-compose-backend-template.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     7953 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/backend/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (999)    11257 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/backend/seed.py
--rw-r--r--   0 runner    (1001) docker     (999)    12336 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/client.py
--rw-r--r--   0 runner    (1001) docker     (999)     2852 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/docs.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.039668 scitacean-23.8.0/src/scitacean/testing/sftp/
--rw-r--r--   0 runner    (1001) docker     (999)      267 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/sftp/Dockerfile-sftp-server
--rw-r--r--   0 runner    (1001) docker     (999)     4242 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/sftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1288 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/sftp/_pytest_helpers.py
--rw-r--r--   0 runner    (1001) docker     (999)     4812 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/sftp/_sftp.py
--rw-r--r--   0 runner    (1001) docker     (999)      836 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/sftp/docker-compose-sftp-server.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     6662 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/sftp/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.039668 scitacean-23.8.0/src/scitacean/testing/sftp/sftp_server_seed/
--rw-r--r--   0 runner    (1001) docker     (999)        8 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/sftp/sftp_server_seed/table.csv
--rw-r--r--   0 runner    (1001) docker     (999)       31 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/sftp/sftp_server_seed/text.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.039668 scitacean-23.8.0/src/scitacean/testing/ssh/
--rw-r--r--   0 runner    (1001) docker     (999)     4196 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1279 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/ssh/_pytest_helpers.py
--rw-r--r--   0 runner    (1001) docker     (999)     4498 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/ssh/_ssh.py
--rw-r--r--   0 runner    (1001) docker     (999)      808 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/ssh/docker-compose-ssh-server.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     7332 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/ssh/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.039668 scitacean-23.8.0/src/scitacean/testing/ssh/ssh_server_seed/
--rw-r--r--   0 runner    (1001) docker     (999)        8 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/ssh/ssh_server_seed/table.csv
--rw-r--r--   0 runner    (1001) docker     (999)       31 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/ssh/ssh_server_seed/text.txt
--rw-r--r--   0 runner    (1001) docker     (999)     9216 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/strategies.py
--rw-r--r--   0 runner    (1001) docker     (999)     5177 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/testing/transfer.py
--rw-r--r--   0 runner    (1001) docker     (999)     8402 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.039668 scitacean-23.8.0/src/scitacean/transfer/
--rw-r--r--   0 runner    (1001) docker     (999)      121 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    11452 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/transfer/sftp.py
--rw-r--r--   0 runner    (1001) docker     (999)    18056 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/transfer/ssh.py
--rw-r--r--   0 runner    (1001) docker     (999)     1322 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/transfer/util.py
--rw-r--r--   0 runner    (1001) docker     (999)     2876 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.039668 scitacean-23.8.0/src/scitacean/util/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3633 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/util/credentials.py
--rw-r--r--   0 runner    (1001) docker     (999)     2589 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/util/formatter.py
--rw-r--r--   0 runner    (1001) docker     (999)      453 2023-08-28 12:37:04.000000 scitacean-23.8.0/src/scitacean/warning.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.031668 scitacean-23.8.0/src/scitacean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     4278 2023-08-28 12:37:16.000000 scitacean-23.8.0/src/scitacean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     5820 2023-08-28 12:37:17.000000 scitacean-23.8.0/src/scitacean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 12:37:16.000000 scitacean-23.8.0/src/scitacean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      127 2023-08-28 12:37:16.000000 scitacean-23.8.0/src/scitacean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       10 2023-08-28 12:37:16.000000 scitacean-23.8.0/src/scitacean.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.043668 scitacean-23.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      121 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.043668 scitacean-23.8.0/tests/client/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5432 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/client/attachment_client_test.py
--rw-r--r--   0 runner    (1001) docker     (999)     2665 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/client/client_test.py
--rw-r--r--   0 runner    (1001) docker     (999)     2730 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/client/datablock_client_test.py
--rw-r--r--   0 runner    (1001) docker     (999)     4652 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/client/dataset_client_test.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.043668 scitacean-23.8.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (999)      121 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1016 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/common/files.py
--rw-r--r--   0 runner    (1001) docker     (999)     1011 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (999)    16661 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/dataset_fields_test.py
--rw-r--r--   0 runner    (1001) docker     (999)    24350 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (999)    13372 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/download_test.py
--rw-r--r--   0 runner    (1001) docker     (999)    13231 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/file_test.py
--rw-r--r--   0 runner    (1001) docker     (999)     7703 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/filesystem_test.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.043668 scitacean-23.8.0/tests/html_repr/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/html_repr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1246 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/html_repr/html_repr_test.py
--rw-r--r--   0 runner    (1001) docker     (999)     9268 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.043668 scitacean-23.8.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1837 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/testing/strategies_test.py
--rw-r--r--   0 runner    (1001) docker     (999)     3607 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/thumbnail_test.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.043668 scitacean-23.8.0/tests/transfer/
--rw-r--r--   0 runner    (1001) docker     (999)      129 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    14552 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/transfer/sftp_test.py
--rw-r--r--   0 runner    (1001) docker     (999)    14809 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/transfer/ssh_test.py
--rw-r--r--   0 runner    (1001) docker     (999)     8829 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/upload_test.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.043668 scitacean-23.8.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2182 2023-08-28 12:37:04.000000 scitacean-23.8.0/tests/util/formatter_test.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.011668 scitacean-23.8.0/tools/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.043668 scitacean-23.8.0/tools/model-generation/
--rw-r--r--   0 runner    (1001) docker     (999)     2038 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/README.md
--rw-r--r--   0 runner    (1001) docker     (999)     3576 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/generate_models.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.043668 scitacean-23.8.0/tools/model-generation/spec/
--rw-r--r--   0 runner    (1001) docker     (999)    13009 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1251 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/spec/dataset-fields.yml
--rw-r--r--   0 runner    (1001) docker     (999)      275 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/spec/field-name-overrides.yml
--rw-r--r--   0 runner    (1001) docker     (999)      482 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/spec/field-type-overrides.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1080 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/spec/field-validations.yml
--rw-r--r--   0 runner    (1001) docker     (999)      401 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/spec/masked-fields.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2762 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/spec/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 12:37:17.047668 scitacean-23.8.0/tools/model-generation/templates/
--rw-r--r--   0 runner    (1001) docker     (999)      607 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     8356 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/templates/dataset_fields.py.jinja
--rw-r--r--   0 runner    (1001) docker     (999)     7491 2023-08-28 12:37:04.000000 scitacean-23.8.0/tools/model-generation/templates/model.py.jinja
--rw-r--r--   0 runner    (1001) docker     (999)     1345 2023-08-28 12:37:04.000000 scitacean-23.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.529352 scitacean-24.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-19 13:49:16.000000 scitacean-24.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 13:49:16.000000 scitacean-24.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-19 13:49:16.000000 scitacean-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-19 13:49:16.000000 scitacean-24.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-19 13:49:16.000000 scitacean-24.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-19 13:49:16.000000 scitacean-24.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 13:49:16.000000 scitacean-24.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-19 13:49:21.529352 scitacean-24.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-19 13:49:16.000000 scitacean-24.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-19 13:49:16.000000 scitacean-24.4.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_static/anaconda-icon.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_templates/scitacean-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/_templates/scitacean-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/developer/coding-conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/developer/dependency-management.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/developer/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/developer/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.505351 scitacean-24.4.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/release-notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.509351 scitacean-24.4.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/classes-and-concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/downloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/testing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-04-19 13:49:16.000000 scitacean-24.4.0/docs/user-guide/uploading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-19 13:49:16.000000 scitacean-24.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.509351 scitacean-24.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-19 13:49:16.000000 scitacean-24.4.0/requirements/wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:49:21.529352 scitacean-24.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.497351 scitacean-24.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.513351 scitacean-24.4.0/src/scitacean/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45884 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_dataset_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.513351 scitacean-24.4.0/src/scitacean/_html_repr/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/_attachment_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/_common_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/_dataset_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.513351 scitacean-24.4.0/src/scitacean/_html_repr/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/images/lock.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.513351 scitacean-24.4.0/src/scitacean/_html_repr/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/styles/attachment.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/styles/common.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/styles/dataset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.517351 scitacean-24.4.0/src/scitacean/_html_repr/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/attachment_field_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/attachment_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/dataset_field_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/dataset_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/files_repr.html.template
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_html_repr/templates/metadata_repr.html.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.517351 scitacean-24.4.0/src/scitacean/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/dataclass_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/file_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/_internal/orcid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40371 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/datablock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20122 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28055 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.517351 scitacean-24.4.0/src/scitacean/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/_pytest_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.517351 scitacean-24.4.0/src/scitacean/testing/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/_pytest_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/docker-compose-backend-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/backend/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.521351 scitacean-24.4.0/src/scitacean/testing/sftp/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/Dockerfile-sftp-server
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/_pytest_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/_sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/docker-compose-sftp-server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.521351 scitacean-24.4.0/src/scitacean/testing/sftp/sftp_server_seed/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/sftp_server_seed/table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/sftp/sftp_server_seed/text.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/testing/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.521351 scitacean-24.4.0/src/scitacean/transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/transfer/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/transfer/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/transfer/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.521351 scitacean-24.4.0/src/scitacean/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/util/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/util/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-19 13:49:16.000000 scitacean-24.4.0/src/scitacean/warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/src/scitacean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-19 13:49:21.000000 scitacean-24.4.0/src/scitacean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-19 13:49:21.000000 scitacean-24.4.0/src/scitacean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:49:21.000000 scitacean-24.4.0/src/scitacean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 13:49:21.000000 scitacean-24.4.0/src/scitacean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 13:49:21.000000 scitacean-24.4.0/src/scitacean.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.521351 scitacean-24.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/attachment_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/datablock_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/dataset_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/client/sample_client_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/dataset_fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29310 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/download_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/filesystem_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/html_repr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/html_repr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/html_repr/html_repr_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/testing/strategies_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/thumbnail_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/transfer/link_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14556 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/transfer/sftp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/upload_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-19 13:49:16.000000 scitacean-24.4.0/tests/util/formatter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.501351 scitacean-24.4.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tools/model-generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/generate_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tools/model-generation/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/dataset-fields.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/field-name-overrides.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/field-type-overrides.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/field-validations.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/masked-fields.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/spec/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:49:21.525352 scitacean-24.4.0/tools/model-generation/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/templates/dataset_fields.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-19 13:49:16.000000 scitacean-24.4.0/tools/model-generation/templates/model.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-19 13:49:16.000000 scitacean-24.4.0/tox.ini
```

### Comparing `scitacean-23.8.0/.github/workflows/ci.yml` & `scitacean-24.4.0/.github/workflows/ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -8,48 +8,53 @@
   pull_request:
 
 jobs:
   formatting:
     name: Formatting and static analysis
     runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v3
-        with:
-          submodules: true
-      - uses: actions/setup-python@v3
-        with:
-          python-version: 3.8
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e static
-      - uses: stefanzweifel/git-auto-commit-action@v4
+      - uses: stefanzweifel/git-auto-commit-action@v5
         with:
           commit_message: Apply automatic formatting
 
+  type-checking:
+    name: Type checking
+    needs: formatting
+    runs-on: ubuntu-22.04
+    steps:
+      - uses: actions/checkout@v3
+      - uses: actions/setup-python@v5
+        with:
+          python-version: 3.11
+      - run: python -m pip install --upgrade pip
+      - run: python -m pip install -r requirements/ci.txt
+      - run: tox -e mypy
+
   tests:
     name: Tests ${{ matrix.os }} ${{ matrix.tox }}
     needs: formatting
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
-          - {python: '3.11', os: ubuntu-22.04, tox: pydantic2-full}
+          - {python: '3.12', os: ubuntu-22.04, tox: py312-full}
           - {python: '3.11', os: ubuntu-22.04, tox: py311-full}
           - {python: '3.10', os: ubuntu-22.04, tox: py310-full}
-          - {python: '3.9', os: ubuntu-22.04, tox: py39-full}
-          - {python: '3.8', os: ubuntu-22.04, tox: py38-full}
-          - {python: '3.8', os: macos-12, tox: py38}
-          - {python: '3.8', os: windows-2022, tox: py38}
+          - {python: '3.10', os: macos-12, tox: py310}
+          - {python: '3.10', os: windows-2022, tox: py310}
     steps:
       - run: sudo apt install --yes docker-compose
         if: ${{ contains(matrix.variant.os, 'ubuntu') }}
-      - uses: actions/checkout@v3
-        with:
-          submodules: true
-      - uses: actions/setup-python@v3
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e ${{ matrix.tox }}
 
   docs:
```

### Comparing `scitacean-23.8.0/.github/workflows/codeql-analysis.yml` & `scitacean-24.4.0/.github/workflows/codeql-analysis.yml`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     permissions:
       actions: read
       contents: read
       security-events: write
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     # Initializes the CodeQL tools for scanning.
     - name: Initialize CodeQL
-      uses: github/codeql-action/init@v2
+      uses: github/codeql-action/init@v3
       with:
         languages: python
 
     - name: Perform CodeQL Analysis
-      uses: github/codeql-action/analyze@v2
+      uses: github/codeql-action/analyze@v3
```

### Comparing `scitacean-23.8.0/.github/workflows/dependency-review.yml` & `scitacean-24.4.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/.github/workflows/docs.yml` & `scitacean-24.4.0/.github/workflows/docs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 
 jobs:
   docs:
     name: Build documentation
     runs-on: ubuntu-22.04
     steps:
       - run: sudo apt install --yes pandoc
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v3
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: 3.11
       - run: python -m pip install --upgrade pip
       - run: python -m pip install -r requirements/ci.txt
       - run: tox -e docs
       - run: touch html/.nojekyll
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: documentation
           path: html/
-      - uses: JamesIves/github-pages-deploy-action@v4.4.3
+      - uses: JamesIves/github-pages-deploy-action@v4.5.0
         if: ${{ inputs.publish }}
         with:
           branch: gh-pages
           folder: html
           single-commit: true
           ssh-key: ${{ secrets.GH_PAGES_DEPLOY_KEY }}
```

### Comparing `scitacean-23.8.0/.pre-commit-config.yaml` & `scitacean-24.4.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.5.0
   hooks:
     - id: check-added-large-files
     - id: check-json
+    - id: check-merge-conflict
     - id: check-toml
     - id: check-yaml
     - id: detect-private-key
     - id: end-of-file-fixer
     - id: trailing-whitespace
       args: [--markdown-linebreak-ext=md]
-- repo: https://github.com/psf/black
-  rev: 23.7.0
-  hooks:
-    - id: black
 - repo: https://github.com/kynan/nbstripout
-  rev: 0.6.0
+  rev: 0.7.1
   hooks:
     - id: nbstripout
       types: ["jupyter"]
       args: ["--drop-empty-cells",
              "--extra-keys 'metadata.language_info.version cell.metadata.jp-MarkdownHeadingCollapsed cell.metadata.pycharm'"]
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: 'v0.0.285'
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.4.0
   hooks:
+    - id: ruff-format
+      types_or: [ python, pyi ]
     - id: ruff
-      args: ["--fix"]
+      args: [--fix, --exit-non-zero-on-fix]
+      types_or: [ python, pyi, jupyter ]
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.5
+  rev: v2.2.6
   hooks:
     - id: codespell
       additional_dependencies:
         - tomli
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: v1.10.0
   hooks:
```

### Comparing `scitacean-23.8.0/CODE_OF_CONDUCT.md` & `scitacean-24.4.0/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 posting via an official social media account, or acting as an appointed
 representative at an online or offline event.
 
 ## Enforcement
 
 Instances of abusive, harassing, or otherwise unacceptable behavior may be
 reported to the community leaders responsible for enforcement at
-jan-lukas.wynen@ess.eu.
+jan-lukas.wynen[at]ess.eu.
 All complaints will be reviewed and investigated promptly and fairly.
 
 All community leaders are obligated to respect the privacy and security of the
 reporter of any incident.
 
 ## Enforcement Guidelines
```

### Comparing `scitacean-23.8.0/CONTRIBUTING.md` & `scitacean-24.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/LICENSE` & `scitacean-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/PKG-INFO` & `scitacean-24.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitacean
-Version: 23.8.0
+Version: 24.4.0
 Summary: High-level interface for SciCat
 Author: Scitacean contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, SciCat Project
         All rights reserved.
         
@@ -33,32 +33,39 @@
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Documentation, https://scicatproject.github.io/scitacean
 Project-URL: Bug Tracker, https://github.com/SciCatProject/scitacean/issues
 Project-URL: Source, https://github.com/SciCatProject/scitacean
 Keywords: scicat
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: ssh
+License-File: LICENSE
+Requires-Dist: email-validator
+Requires-Dist: pydantic>=2
+Requires-Dist: python-dateutil
+Requires-Dist: requests>=2.31
 Provides-Extra: sftp
+Requires-Dist: paramiko; extra == "sftp"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: filelock; extra == "test"
+Requires-Dist: hypothesis; extra == "test"
+Requires-Dist: pyyaml; extra == "test"
 
 [![PyPI badge](https://img.shields.io/pypi/v/scitacean.svg?style=flat-square&color=green)](https://pypi.python.org/pypi/scitacean)
 [![Anaconda-Server Badge](https://img.shields.io/conda/vn/conda-forge/scitacean?style=flat-square&color=green)](https://anaconda.org/conda-forge/scitacean)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7520487.svg)](https://doi.org/10.5281/zenodo.7520487)
 [![License: BSD 3-Clause](https://img.shields.io/github/license/SciCatProject/scitacean?style=flat-square&color=yellowgreen)](LICENSE)
 
 <picture>
```

### Comparing `scitacean-23.8.0/README.md` & `scitacean-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/docs/_static/favicon.ico` & `scitacean-24.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/docs/_static/logo-dark.svg` & `scitacean-24.4.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/docs/_static/logo.svg` & `scitacean-24.4.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/docs/_templates/scitacean-class-template.rst` & `scitacean-24.4.0/docs/_templates/scitacean-class-template.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {{ fullname | escape | underline }}
 
 {% set constructors = {"Client": ["from_credentials", "from_token", "without_login"],
                        "Dataset": ["__init__", "from_download_models"],
-                       "File": ["from_local", "from_download_model"],
+                       "File": ["from_local", "from_remote", "from_download_model"],
                        "OrigDatablockProxy": ["__init__", "from_download_model"],
                        "PID": ["__init__", "parse"],
                        "ScicatClient": ["from_credentials", "from_token", "without_login"],
                        "Thumbnail": ["__init__", "load_file", "parse"],
                       } %}
 {% set regular_methods = methods | reject("in", constructors.get(name, []) + ["__init__"]) | list %}
```

### Comparing `scitacean-23.8.0/docs/_templates/scitacean-module-template.rst` & `scitacean-24.4.0/docs/_templates/scitacean-module-template.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/docs/conf.py` & `scitacean-24.4.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 
 # -- Options for HTML output ----------------------------------------------
 
 html_theme = "pydata_sphinx_theme"
 html_theme_options = {
     "primary_sidebar_end": ["edit-this-page", "sourcelink"],
     "secondary_sidebar_items": [],
+    "navbar_persistent": ["search-button"],
     "show_nav_level": 1,
     "header_links_before_dropdown": 4,
     "pygment_light_style": "github-light-high-contrast",
     "pygment_dark_style": "github-dark-high-contrast",
     "logo": {
         "image_light": "_static/logo.svg",
         "image_dark": "_static/logo-dark.svg",
@@ -135,18 +136,20 @@
             "url": "https://pypi.org/project/scitacean/",
             "icon": "fa-brands fa-python",
             "type": "fontawesome",
         },
         {
             "name": "Conda",
             "url": "https://anaconda.org/conda-forge/scitacean",
-            "icon": "_static/anaconda-logo.svg",
-            "type": "local",
+            "icon": "fa-custom fa-anaconda",
+            "type": "fontawesome",
         },
     ],
+    "footer_start": ["copyright", "sphinx-version"],
+    "footer_end": ["doc_version", "theme-version"],
 }
 html_context = {
     "doc_path": "docs",
 }
 html_sidebars = {
     "**": ["sidebar-nav-bs", "page-toc"],
 }
@@ -156,14 +159,15 @@
 html_favicon = "_static/favicon.ico"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 html_css_files = ["css/custom.css"]
+html_js_files = ["anaconda-icon.js"]
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "scitaceandoc"
 
 # -- Options for doctest --------------------------------------------------
```

### Comparing `scitacean-23.8.0/docs/developer/coding-conventions.rst` & `scitacean-24.4.0/docs/developer/coding-conventions.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Coding conventions
 ==================
 
 Formatting
 ----------
 
-There are no explicit formatting conventions since we use ``black`` to enforce a format.
+There are no explicit formatting conventions since we use ``ruff`` to enforce a format.
 
 Docstrings
 ~~~~~~~~~~
 
 The exception to this are Python docstrings, for which we use the
 `numpy docstring format <https://www.sphinx-doc.org/en/master/usage/extensions/example_numpy.html>`_.
 We use a tool to automatically insert type hints into the docstrings.
@@ -59,14 +59,17 @@
           >>> scitacean.foo(1, 2)
           3
 
         And also:
 
           >>> scitacean.foo(1, 3)
           6
+
+
+        .. versionadded:: v23.08.0
         """
 
 The order of sections is fixed as shown in the example.
 
 * **Short description** (*required*) A single sentence describing the purpose of the function / class.
 * **Long description** (*optional*) One or more paragraphs of detailed explanations.
   Can include additional sections like ``Warning`` or ``Hint``.
@@ -101,14 +104,16 @@
 * **See Also** (*optional*) List of related functions and / or classes.
   The function / class name should include the module it is in but without reST markup.
   For simple cases, the explanation can be left out.
   In this case, the colon should be omitted as well and multiple entries must be separated by commas.
 * **Examples** (*optional*) Example code given using ``>>>`` as the Python prompt.
   May include text before, after, and between code blocks.
   Note the spacing in the example.
+* **Version info** (*optional*) ``versionadded``, ``versionchanged``, and ``deprecated`` directives are placed at the end.
+  They must be separated from the previous section by *two* empty lines in order to render properly.
 
 Some functions can be sufficiently described by a single sentence.
 In this case, the 'Parameters' and 'Returns' sections may be omitted and the docstring should be laid out on a single line.
 If it does not fit on a single line, it is too complicated.
 For example
 
 .. code-block:: python
```

### Comparing `scitacean-23.8.0/docs/developer/dependency-management.rst` & `scitacean-24.4.0/docs/developer/dependency-management.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/docs/developer/getting-started.rst` & `scitacean-24.4.0/docs/developer/getting-started.rst`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 .. code-block:: sh
 
     pip install -r requirements/dev.txt
 
 Additionally, building the documentation requires `pandoc <https://pandoc.org/>`_ which is not on PyPI and needs to be installed through other means.
 (E.g. with your OS package manager.)
 
-If you want to run tests against a real backend or SSH server, you also need ``docker-compose``.
+If you want to run tests against a real backend or SFTP server, you also need ``docker-compose``.
 See `Testing <./testing.rst>`_ for what this is good for and why.
 
 Install the package
 ~~~~~~~~~~~~~~~~~~~
 
 Install the package in editable mode using
 
@@ -52,36 +52,36 @@
 
         Run the tests using
 
         .. code-block:: sh
 
             python -m pytest -n<number-of-threads>
 
-        Or to run tests against a real backend and SSH server (see setup above)
+        Or to run tests against a real backend and SFTP server (see setup above)
 
 
         .. code-block:: sh
 
-            pytest --backend-tests --ssh-tests
+            pytest --backend-tests --sftp-tests
 
         Note that the setup and teardown of the backend takes several seconds.
 
     .. tab-item:: tox
 
         Run the tests using (e.g. python 3.10)
 
         .. code-block:: sh
 
             tox -e py310
 
-        Or to also run backend tests use
+        Or to also run backend and SFTP tests use
 
         .. code-block:: sh
 
-            tox -e py310-backend
+            tox -e py310-full
 
 Building the docs
 -----------------
 
 .. tab-set::
 
     .. tab-item:: Manually
```

### Comparing `scitacean-23.8.0/docs/developer/testing.rst` & `scitacean-24.4.0/docs/developer/testing.rst`

 * *Files 17% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 However, there are two problems.
 For one, the fakes do not have perfect fidelity, that is, some edge cases do not work.
 And the visible behavior slightly deviates from a real client, e.g. the content of error messages or how datasets are modified during upload.
 In addition, the fakes are relatively complex and may diverge from the real implementations.
 
 To mitigate these problems, the fake client is tested alongside a real client.
 But to (mostly) avoid the downsides stated in the beginning, the real client is connected to a local SciCat server.
-See ``src/testing/backend.py`` and ``tests/conftest.py`` for the concrete setup.
+See the `src/scitacean/backend <https://github.com/SciCatProject/scitacean/tree/main/src/scitacean/testing/backend>`_ folder and `tests/conftest.py <https://github.com/SciCatProject/scitacean/blob/main/tests/conftest.py>`_ file for the concrete setup.
 The backend is launched in a docker container with the image of the latest release of the SciCat backend.
-Tests in ``tests/client`` are then run with both the fake and the real client to ensure that both produce the same results.
+Tests in `tests/client <https://github.com/SciCatProject/scitacean/tree/main/tests/client>`_ are then run with both the fake and the real client to ensure that both produce the same results.
 
 Use ``--backend-tests`` with ``pytest`` to run these tests.
 
 SFTP file transfer
 ------------------
 
 Testing :class:`scitacean.transfer.sftp.SFTPFileTransfer` requires an SFTP server.
-``tests/common/sftp_server.py`` contains helpers for managing one via Docker.
+:mod:`scitacean.testing.sftp` contains helpers for managing one via Docker.
 Tests can use it by depending on the ``sftp_fileserver`` fixture.
-See the documentation in ``tests/common/sftp_server.py`` for how it works.
+See the `documentation <https://scicatproject.github.io/scitacean/user-guide/testing.html#Local-SFTP-fileserver>`_ for how it works.
 
 Note that those tests may leave a small directory behind.
 This is an issue with file ownership and permissions caused by making the Docker volumes writable.
 It should not be a problem in practice as those files will only be in temporary directories which should get cleaned up at reboot.
 
 Use ``--sftp-tests`` with ``pytest`` to run these tests.
```

### Comparing `scitacean-23.8.0/docs/index.rst` & `scitacean-24.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/docs/reference/index.rst` & `scitacean-24.4.0/docs/reference/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 ~~~~~~~~~~~~~
 
 .. autosummary::
    :toctree: ../generated/classes
    :template: scitacean-class-template.rst
    :recursive:
 
-   transfer.ssh.SSHFileTransfer
+   transfer.link.LinkFileTransfer
+   transfer.sftp.SFTPFileTransfer
 
 Auxiliary classes
 ~~~~~~~~~~~~~~~~~
 
 .. autosummary::
    :toctree: ../generated/classes
    :template: scitacean-class-template.rst
```

### Comparing `scitacean-23.8.0/docs/release-notes.rst` & `scitacean-24.4.0/docs/release-notes.rst`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 Release notes
 =============
 
 
 .. Template, copy this to create a new section after a release:
 
-   vYY.0M.MICRO (Unreleased)
-   -------------------------
+   vversion
+   --------
 
    Security
    ~~~~~~~~
 
    Features
    ~~~~~~~~
 
@@ -28,14 +28,70 @@
 
    Deprecations
    ~~~~~~~~~~~~
 
    Stability, Maintainability, and Testing
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+v24.04.0
+--------
+
+Features
+~~~~~~~~
+
+* Added functions for downloading and uploading samples: :meth:`Client.get_sample`, :meth:`Client.upload_new_sample_now`.
+* Added :class:`transfer.link.LinkFileTransfer`.
+* :class:`Client` and :class:`ScicatClient` now check whether a token has expired and raise and exception if it has.
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+* **Dropped support for Python 3.9.**
+* **Dropped support for Pydantic v1.**
+* Removed deprecated ``transfer.ssh.SSHFileTransfer`` in favor of :class:`transfer.sftp.SFTPFileTransfer`.
+
+Bugfixes
+~~~~~~~~
+
+* Fixed testing setup to explicitly define user accounts in the test backend.
+
+v23.10.0
+--------
+
+Features
+~~~~~~~~
+
+* Python 3.12 is officially supported.
+* Added dict-like methods, :meth:`Dataset.keys`, :meth:`Dataset.values` and :meth:`Dataset.items`.
+* Added dict-like item setter/getter, :meth:`Dataset.__getitem__` and :meth:`Dataset.__setitem__`.
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+* **Dropped support for Python 3.8.**
+* ``Dataset.type`` is now read only.
+
+Bugfixes
+~~~~~~~~
+
+* :class:`scitacean.Client` no longer requires a file transfer during upload if the dataset has no files that need to be uploaded.
+* The HTML representation of datasets no longer flags read-only fields with a value as broken.
+* Preserve ``meta`` in ``Dataset.replace`` and allow replacing it.
+  This also affects ``Dataset.replace_files`` and ``Client.download_files``.
+
+Deprecations
+~~~~~~~~~~~~
+
+* Deprecated support for Pydantic v1. It is scheduled for full removal in release 23.12.0.
+
+Stability, Maintainability, and Testing
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* The codebase now gets type-checked in CI.
+
 v23.08.0 (2023-08-28)
 ---------------------
 
 Features
 ~~~~~~~~
 
 * File downloads now use the checksum algorithm stored in SciCat when possible.
@@ -43,14 +99,15 @@
 * Added ``SFTPFileTransfer`` which is similar to ``SSHFileTransfer`` but relies only on SFTP.
 * Added support for attachments.
 
 Bugfixes
 ~~~~~~~~
 
 * Fields of derived datasets are no longer initialized when downloading raw datasets and vice versa.
+* Consistent table styling implemented for Jupyter notebooks in browser and vscode for both dark and light themes.
 
 Deprecations
 ~~~~~~~~~~~~
 
 * Deprecated ``SSHFileTransfer`` in favor of ``SFTPFileTransfer``.
 
 v23.07.0 (2023-07-07)
@@ -180,15 +237,15 @@
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 * A number of attributes of Dataset are now read only.
 * ``Dataset.new`` was removed, use the regular ``__init__`` method instead.
 * ``File.provide_locally`` was removed in favor of :meth:`Client.download_files`.
-* ``ESSTestFileTransfer`` was renamed to :class:`transfer.ssh.SSHFileTransfer`.
+* ``ESSTestFileTransfer`` was renamed to ``transfer.ssh.SSHFileTransfer``.
 
 Bugfixes
 ~~~~~~~~
 
 * It is not possible to log in with username+password as a non-functional user.
 * Added and fixed a number of type annotations.
```

### Comparing `scitacean-23.8.0/docs/user-guide/classes-and-concepts.rst` & `scitacean-24.4.0/docs/user-guide/classes-and-concepts.rst`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/docs/user-guide/downloading.ipynb` & `scitacean-24.4.0/docs/user-guide/downloading.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9873842592592592%*

 * *Differences: {"'cells'": "{0: {'id': '0', 'source': {insert: [(43, 'See [Developer "*

 * *            'Documentation/Testing](../developer/testing.rst) if you are interested in the '*

 * *            "details.')], delete: [43]}}, 1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3'}, 4: "*

 * *            "{'id': '4'}, 5: {'id': '5'}, 6: {'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: "*

 * *            "{'id': '9'}, 10: {'id': '10'}, 11: {'id': '11'}, 12: {'id': '12'}, 13: {'id': '13'}, "*

 * *            "14: {'id': '14'}, 15: {'id': '15'}, 16: {'id […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "594ba90e-8388-434c-8d33-c9001f64b6c8",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# Downloading datasets\n",
                 "\n",
                 "All communication with SciCat is handled by a client object.\n",
                 "Normally, one would construct one using something like\n",
                 "\n",
@@ -44,246 +44,246 @@
                 "\n",
                 "The file transfer needs to authenticate separately from the SciCat connection.\n",
                 "By default, it requires an SSH agent to be running an set up for the selected `host`.\n",
                 "\n",
                 "For the purposes of this guide, we don't want to connect to a real SciCat server in order to avoid the complications associated with that.\n",
                 "So we set up a fake client that only pretends to connect to SciCat and file servers.\n",
                 "Everything else in this guide works in the same way with a real client.\n",
-                "See [Developer Documentation/Testing](../developer/testing.rst) if you are interested in the detatils."
+                "See [Developer Documentation/Testing](../developer/testing.rst) if you are interested in the details."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "22f329e2-624f-4406-93d4-55913e83624d",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scitacean.testing.docs import setup_fake_client\n",
                 "client = setup_fake_client()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4e8aea34-fb1f-469c-b2d6-c7d64880b7da",
+            "id": "2",
             "metadata": {},
             "source": [
                 "## Metadata\n",
                 "\n",
                 "We need the ID (`pid`) of a dataset in order to download it.\n",
                 "The fake client provides a dataset with id `20.500.12269/72fe3ff6-105b-4c7f-b9d0-073b67c90ec3`.\n",
                 "We can download it using"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9388ae93-2b8a-4388-8451-26dd263345d8",
+            "id": "3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dset = client.get_dataset(\"20.500.12269/72fe3ff6-105b-4c7f-b9d0-073b67c90ec3\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "29dbb19b-a46e-4140-ae59-9f41ddf86340",
+            "id": "4",
             "metadata": {},
             "source": [
                 "Datasets can easily be inspected in Jupyter notebooks:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c4ca91c2-2c51-4dee-906e-4c97c0b7a1e7",
+            "id": "5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dset"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "08363dcc-4a11-40b6-af47-8c6096754868",
+            "id": "6",
             "metadata": {},
             "source": [
                 "All attributes listed above can be accessed directly:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "26d06a21-8cc7-4364-b289-37041f455d9c",
+            "id": "7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dset.type"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d78b40ef-4494-49a8-ae2f-233188ba52eb",
+            "id": "8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dset.name"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bd441bbd-58f7-47bf-ac14-edd730c05ab4",
+            "id": "9",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dset.owner"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b8ddc42b-b43d-4f95-b40a-235af77d9d27",
+            "id": "10",
             "metadata": {},
             "source": [
                 "See [Dataset](../generated/classes/scitacean.Dataset.rst) for a list of available fields.\n",
                 "\n",
                 "In addition, datasets can have free form scientific metadata which we can be accessed using"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c7788a40-0d56-442c-ad19-6fe5205bc476",
+            "id": "11",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dset.meta"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "020840e2-9291-4d1c-b8e1-b25709fcf790",
+            "id": "12",
             "metadata": {},
             "source": [
                 "## Files\n",
                 "\n",
                 "The data files associated with this dataset can be accessed using"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2fcb8261-ff87-4788-adbd-6e6fd7a9d2f1",
+            "id": "13",
             "metadata": {},
             "outputs": [],
             "source": [
                 "for f in dset.files:\n",
                 "    print(f\"{f.remote_access_path(dset.source_folder) = }\")\n",
                 "    print(f\"{f.local_path = }\")\n",
                 "    print(f\"{f.size = } bytes\")\n",
                 "    print(\"----\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c5fb8c86-ccf7-4245-99da-b5b49dce4c5d",
+            "id": "14",
             "metadata": {},
             "source": [
                 "Note that the `local_path` for both files is `None`.\n",
                 "This indicates that the files have not been downloaded.\n",
                 "Indeed, `client.get_dataset` downloads only the metadata from SciCat, not the files.\n",
                 "\n",
                 "We can download the first file using"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "39f3e892-919c-495b-ad9a-37c6ca46aafb",
+            "id": "15",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dset_with_local_file = client.download_files(dset, target=\"download\", select=\"flux.dat\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dfe6545b-4c3b-4998-9831-aece5c3bb116",
+            "id": "16",
             "metadata": {},
             "outputs": [],
             "source": [
                 "for f in dset_with_local_file.files:\n",
                 "    print(f\"{f.remote_access_path(dset.source_folder) = }\")\n",
                 "    print(f\"{f.local_path = }\")\n",
                 "    print(f\"{f.size = } bytes\")\n",
                 "    print(\"----\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0097c9f9-ff98-4bd2-971f-70fd1001d186",
+            "id": "17",
             "metadata": {},
             "source": [
                 "Which populates the `local_path`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cc9fec2d-51e8-462f-9c1d-e510ec2eefbf",
+            "id": "18",
             "metadata": {},
             "outputs": [],
             "source": [
                 "file = list(dset_with_local_file.files)[0]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "84f086f8-e930-4ccb-ad22-5b5e0bb0cc6e",
+            "id": "19",
             "metadata": {},
             "outputs": [],
             "source": [
                 "file.local_path"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "28a14e32-f2fa-45d4-9b62-2c6f04abeffb",
+            "id": "20",
             "metadata": {},
             "source": [
                 "We can use it to read the file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7b1ffde0-e2b9-47ff-ac68-3d327a18c124",
+            "id": "21",
             "metadata": {},
             "outputs": [],
             "source": [
                 "with file.local_path.open(\"r\") as f:\n",
                 "    print(f.read())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1492ed89-a0e0-46c2-b24a-7e621f230b20",
+            "id": "22",
             "metadata": {},
             "source": [
                 "If we wanted to download all files, we could pass `select=True` (or nothing, `True` is the default) to `client.download_files`.\n",
                 "See [Client.download_files](../generated/classes/scitacean.Client.rst#scitacean.Client.download_files) for more options to select files."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "eee2b6c2-8f6f-447e-a392-e5dc84eab6cc",
+            "id": "23",
             "metadata": {
                 "nbsphinx": "hidden",
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# This cell is hidden.\n",
```

### Comparing `scitacean-23.8.0/docs/user-guide/logo.png` & `scitacean-24.4.0/docs/user-guide/logo.png`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/docs/user-guide/testing.ipynb` & `scitacean-24.4.0/docs/user-guide/testing.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9871386054421769%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3'}, 4: {'id': '4'}, 5: "*

 * *            "{'id': '5'}, 6: {'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: {'id': '9'}, 10: "*

 * *            "{'id': '10'}, 11: {'id': '11'}, 12: {'id': '12'}, 13: {'id': '13'}, 14: {'id': '14'}, "*

 * *            "15: {'id': '15'}, 16: {'id': '16'}, 17: {'id': '17'}, 18: {'id': '18'}, 19: {'id': "*

 * *            "'19'}, 20: {'id': '20'}, 21: {'id': '21'}, 22: {'id': '22'}, 23: {'id': '23'}, 24: "*

 * *            "{'id':  […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "955a4d05-166f-4456-8dac-f81d0e40805a",
+            "id": "0",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "# Testing code with Scitacean\n",
                 "\n",
                 "Testing programs that use Scitacean can be tricky as those tests might require access to a SciCat server or fileserver.\n",
@@ -22,15 +22,15 @@
                 "\n",
                 "First, create a test dataset and file."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "53ae8816-eea4-49f4-a0d0-20d037f3d1e5",
+            "id": "1",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from scitacean import Dataset\n",
                 "\n",
@@ -45,39 +45,39 @@
                 "    creation_location=\"UnseenUniversity\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e7ff9e70-9d75-4e15-b0ad-ccddc02741fd",
+            "id": "2",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "\n",
                 "path = Path(\"test-data/spellbook.txt\")\n",
                 "path.parent.mkdir(parents=True, exist_ok=True)\n",
                 "with path.open(\"w\") as f:\n",
                 "    f.write(\"fireball power=1000 mana=123\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e7985c81-0df3-4f18-a417-8d5ed8afd5ee",
+            "id": "3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "dataset.add_local_files(\"test-data/spellbook.txt\", base_path=\"test-data\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "94eace31-d349-40e6-8942-1ceea4830f0f",
+            "id": "4",
             "metadata": {
                 "tags": []
             },
             "source": [
                 "## FakeClient\n",
                 "\n",
                 "[scitacean.testing.client.FakeClient](../generated/modules/scitacean.testing.client.FakeClient.rst) has the same interface as the regular [Client](../generated/classes/scitacean.Client.rst) but never connects to any SciCat server.\n",
@@ -86,135 +86,135 @@
                 "First, create a `FakeClient`.\n",
                 "The url is completely arbitrary and only needs to be passed for parity with the real client."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "59eae44f-46a6-4a07-98cc-81104a25503b",
+            "id": "5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scitacean.testing.client import FakeClient\n",
                 "from scitacean.testing.transfer import FakeFileTransfer\n",
                 "\n",
                 "client = FakeClient.without_login(\n",
                 "    url=\"https://fake.scicat\",\n",
                 "    file_transfer=FakeFileTransfer())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e566a6bd-e7e1-4c0b-bb80-c92bcc1b30ba",
+            "id": "6",
             "metadata": {},
             "source": [
                 "### Upload\n",
                 "\n",
                 "And now we can upload our test dataset as usual:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "06e47461-c6c8-456f-ac04-10541fbe8907",
+            "id": "7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "finalized = client.upload_new_dataset_now(dataset)\n",
                 "str(finalized)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d882e803-0609-4940-8033-788d0b735b20",
+            "id": "8",
             "metadata": {},
             "source": [
                 "However, this did not talk to a SciCat server.\n",
                 "We can check if the fake upload was successful by inspecting the `client`.\n",
                 "`client.datasets` is a `dict` that contains all datasets known to the fake server keyed by PID:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "22860c6e-b880-4baf-8709-e80fb8d5781a",
+            "id": "9",
             "metadata": {},
             "outputs": [],
             "source": [
                 "client.datasets.keys()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a8d0bcbe-48d6-41f1-95fc-7c39426c3cfb",
+            "id": "10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "pid = list(client.datasets.keys())[0]\n",
                 "client.datasets[pid]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "25c2ddd3-0105-4370-b57e-65ac94e67b28",
+            "id": "11",
             "metadata": {},
             "source": [
                 "The client has recorded the upload from earlier.\n",
                 "However, it stored the dataset as a [model](../generated/modules/scitacean.model.rst), not as a regular `Dataset` object.\n",
                 "In addition, since the dataset has a file, an original datablock was uploaded as well: (Datablocks store metadata and paths of files in SciCat.)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b9538f81-18d6-4441-9c09-b8dc4c8c1c71",
+            "id": "12",
             "metadata": {},
             "outputs": [],
             "source": [
                 "client.orig_datablocks.keys()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "05633fd9-1286-40f4-91ca-4e8c1a2df299",
+            "id": "13",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# use the pid of the dataset\n",
                 "client.orig_datablocks[pid]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "792d672e-325e-4b5b-80d7-4c71baa6c71d",
+            "id": "14",
             "metadata": {},
             "source": [
                 "When writing tests, those recorded dataset and datablock models can be used to check if an upload worked.\n",
                 "\n",
                 "### Download\n",
                 "\n",
                 "`FakeClient` can also download datasets that are stored in its `datasets` dictionary:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d2e9d67d-8ae1-4462-8035-1907bb3a98fc",
+            "id": "15",
             "metadata": {},
             "outputs": [],
             "source": [
                 "downloaded = client.get_dataset(pid)\n",
                 "str(downloaded)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2919ab29-8d74-416d-b611-d1f1b5ba8fdb",
+            "id": "16",
             "metadata": {},
             "source": [
                 "This is now an actual `Dataset` object like you would get from a real client.\n",
                 "\n",
                 "If we want to test downloads independently of uploads, we can populate `client.datasets` and `cliend.orig_datablocks` manually.\n",
                 "But keep in mind that those store *models*. See the [model reference](../generated/modules/scitacean.model.rst) for an overview.\n",
                 "And also note that `orig_datablocks` stores a list of models for each dataset as there can be multiple datablocks per dataset.\n",
@@ -228,29 +228,29 @@
                 "\n",
                 "If a test requires these properties, consider using a locally deployed SciCat server.\n",
                 "See in particular the [developer documentation on testing](../developer/testing.rst)."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "da104640-ce5f-4e04-81fd-878167b8bd08",
+            "id": "17",
             "metadata": {},
             "source": [
                 "## FakeFileTransfer\n",
                 "\n",
                 "`FakeClient` used above only fakes a SciCat server, i.e. handling of metadata.\n",
                 "If we also want to test file uploads and downloads, we can use [scitacean.testing.transfer.FakeFileTransfer](../generated/modules/scitacean.testing.transfer.FakeFileTransfer.rst).\n",
                 "\n",
                 "Starting from a clean slate, create a fake client with a fake file transfer as above:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7457b8a6-b067-443d-adda-88cc97af22f5",
+            "id": "18",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from scitacean.testing.client import FakeClient\n",
                 "from scitacean.testing.transfer import FakeFileTransfer\n",
@@ -258,113 +258,113 @@
                 "client = FakeClient.without_login(\n",
                 "    url=\"https://fake.scicat\",\n",
                 "    file_transfer=FakeFileTransfer())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "15d15535-78c1-440f-b50e-626ea5457cd0",
+            "id": "19",
             "metadata": {},
             "source": [
                 "And upload a dataset:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9e74e0fe-225a-4899-908c-e24002ad1a0c",
+            "id": "20",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "finalized = client.upload_new_dataset_now(dataset)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "09f3c366-74ef-41bc-82ca-188cfdd240a3",
+            "id": "21",
             "metadata": {},
             "source": [
                 "The file transfer has recorded the upload of the file without actually uploading it anywhere.\n",
                 "We can inspect all files on the fake fileserver using:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e015c1f5-1f6b-4289-b6a5-435bcdf02512",
+            "id": "22",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "client.file_transfer.files"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a1b67454-e63c-42d1-85a9-f1b16d0219c8",
+            "id": "23",
             "metadata": {},
             "source": [
                 "This is a dictionary keyed by [remote_access_path](../generated/classes/scitacean.File.rst#scitacean.File.remote_access_path) to the content of the file.\n",
                 "\n",
                 "We can also download the file."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cc713b35-29d5-4a36-a51b-c3f437e8e4f7",
+            "id": "24",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "downloaded = client.get_dataset(finalized.pid)\n",
                 "with_downloaded_file = client.download_files(downloaded, target=\"test-data/download\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ce5bd08a-9399-4c3b-9a92-ea5ae733e29a",
+            "id": "25",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "file = list(with_downloaded_file.files)[0]\n",
                 "file"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d3135347-569b-49c2-8726-e65cdc07ac0b",
+            "id": "26",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "with file.local_path.open() as f:\n",
                 "    print(f.read())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2489a7d3-4f49-4112-b68b-96a96f8733e4",
+            "id": "27",
             "metadata": {},
             "source": [
                 "If we want to test downloads independently of uploads, we can populate `client.file_transfer.files` manually."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7fc127dd-5ab3-4df6-a971-65a883d4afc2",
+            "id": "28",
             "metadata": {},
             "source": [
                 "## Local SciCat server\n",
                 "\n",
                 "[scitacean.testing.backend](../generated/modules/scitacean.testing.backend.rst) provides tools to set up a SciCat backend and API in a Docker container on the local machine.\n",
                 "It is primarily intended to be used via the [pytest](https://docs.pytest.org/) fixtures in [scitacean.testing.backend.fixtures](../generated/modules/scitacean.testing.backend.fixtures.rst).\n",
                 "\n",
@@ -384,15 +384,15 @@
                 "\n",
                 "To this end, add the following in your `conftest.py`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "778c07f6-199c-4e46-a66e-0196f4fbdbd4",
+            "id": "29",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import pytest\n",
                 "from scitacean.testing.backend import add_pytest_option as add_backend_option\n",
@@ -404,65 +404,65 @@
                 "\n",
                 "def pytest_addoption(parser: pytest.Parser) -> None:\n",
                 "    add_backend_option(parser)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "630a84a8-abef-4fda-b4dc-efeeaacf2043",
+            "id": "30",
             "metadata": {},
             "source": [
                 "The backend will only be launched when the corresponding command line option is given.\n",
                 "By default, this is `--backend-tests` but it can be changed via the `option` argument of `add_pytest_option`.\n",
                 "\n",
                 "### Use SciCat in tests\n",
                 "\n",
                 "Tests that require the server can now request it as a fixture:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cb966da1-46c8-4a8b-ab49-2930e1bf4c3a",
+            "id": "31",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "def test_something_with_scicat(require_scicat_backend):\n",
                 "    # test something\n",
                 "    ..."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6095c70a-4b02-456a-a64c-54bf96278695",
+            "id": "32",
             "metadata": {},
             "source": [
                 "The `require_scicat_backend` fixture will ensure that the backend is running during the test.\n",
                 "If backend tests have not been enabled by the command line option, the test will be skipped.\n",
                 "\n",
                 "The simplest way to connect to the server is to request the `client` or `real_client` fixture:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ef74ea13-c110-4087-b0f8-e5770a7e13b3",
+            "id": "33",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def test_something_with_scicat_client(client):\n",
                 "    # test something\n",
                 "    ..."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "30560dea-7d42-4d5a-a259-d8c1415efb05",
+            "id": "34",
             "metadata": {},
             "source": [
                 "The `client` fixture provides both a client connected to the SciCat server and a fake client.\n",
                 "(Both without a file transfer).\n",
                 "The test will run two times, once with each client if backend tests are enabled.\n",
                 "If they are disabled, the test will only run with a fake client.\n",
                 "\n",
@@ -470,92 +470,92 @@
                 "Make sure to also request `require_scicat_backend` in this case to skip the test if backend tests are disabled.\n",
                 "Or skip them explicitly:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "070daa80-8cc7-4e4f-97ac-74a383e0c023",
+            "id": "35",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def test_something_with_real_client(real_client):\n",
                 "    if real_client is None:\n",
                 "        pytest.skip(\"Backend tests disabled\")\n",
                 "        # or do something else\n",
                 "    \n",
                 "    # do the actual tests"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a3e4ec61-e127-4ce4-81a3-0781521b73d6",
+            "id": "36",
             "metadata": {},
             "source": [
                 "### Seed data\n",
                 "\n",
                 "The database used by the local SciCat server is seeded with a number of datasets from [scitacean.testing.backend.seed](../generated/modules/scitacean.testing.backend.seed.rst).\n",
                 "These datasets are accessible via both real and fake clients.\n",
                 "\n",
                 "To access the seed, use for example:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "432b8c32-7ecf-4638-b364-5ec98cc40ce1",
+            "id": "37",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scitacean.testing.backend import seed\n",
                 "\n",
                 "def test_download_raw(client):\n",
                 "    dset = seed.INITIAL_DATASETS[\"raw\"]\n",
                 "    downloaded = client.get_dataset(dset.pid)\n",
                 "    assert downloaded.owner == dset.owner"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "cc6f9f5f-884a-4986-baba-654cb0fd941c",
+            "id": "38",
             "metadata": {},
             "source": [
                 "Both clients, i.e., also the fake client, require that the database has been seeded, even when backend tests are disabled.\n",
                 "You can ensure this by requesting either `scicat_backend` or `require_scicat_backend` along `fake_client` in your test.\n",
                 "To write a test that uses only a fake client but with seed, use"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fc260196-0ade-4773-8bad-b53a1a6740f2",
+            "id": "39",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def test_seeded_fake(fake_client, scicat_backend):\n",
                 "    dset = seed.INITIAL_DATASETS[\"raw\"]\n",
                 "    downloaded = fake_client.get_dataset(dset.pid)\n",
                 "    assert downloaded.owner == dset.owner"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "e67d6111-9589-403e-a7ad-6f35b5d82db4",
+            "id": "40",
             "metadata": {},
             "source": [
                 "This will run the test both when backend tests are enabled and disabled.\n",
                 "In the latter case, the server is never launched and `fake_client` is seeded in a different way.\n",
                 "This different way of seeding corresponds to how [scitacean.testing.client.FakeClient](../generated/modules/scitacean.testing.client.FakeClient.rst) processes uploaded files.\n",
                 "So it may not be entirely the same as with a real backend.\n",
                 "See in particular the [Fidelity](#Fidelity) section"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "97930d15-517a-4cea-bf2b-38ed700220b3",
+            "id": "41",
             "metadata": {},
             "source": [
                 "## Local SFTP fileserver\n",
                 "\n",
                 "[scitacean.testing.sftp](../generated/modules/scitacean.testing.sftp.rst) provides tools to set up an SFTP server in a Docker container on the local machine.\n",
                 "It is primarily intended to be used via the [pytest](https://docs.pytest.org/) fixtures in [scitacean.testing.sftp.fixtures](../generated/modules/scitacean.testing.sftp.fixtures.rst).\n",
                 "\n",
@@ -575,15 +575,15 @@
                 "\n",
                 "To this end, add the following in your `conftest.py`: (Or merge it into the setup for backend tests from above.)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1d1f763b-1f56-4574-a7d5-5d77e85b888d",
+            "id": "42",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pytest\n",
                 "from scitacean.testing.sftp import add_pytest_option as add_sftp_option\n",
                 "\n",
                 "\n",
@@ -593,55 +593,55 @@
                 "\n",
                 "def pytest_addoption(parser: pytest.Parser) -> None:\n",
                 "    add_sftp_option(parser)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0d92f3dd-986c-4f2c-acec-00b6e55ae87b",
+            "id": "43",
             "metadata": {},
             "source": [
                 "The SFTP server will only be launched when the corresponding command line option is given.\n",
                 "By default, this is `--sftp-tests` but it can be changed via the `option` argument of `add_pytest_option`.\n",
                 "\n",
                 "### Use SFTP in tests\n",
                 "\n",
                 "Tests that require the server can now request it as a fixture:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8e63fde0-827e-4fd5-b55f-980843253813",
+            "id": "44",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def test_something_with_sftp(require_sftp_fileserver):\n",
                 "    # test something\n",
                 "    ..."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3126d0d9-727a-4d55-aff1-6b31fd5df91f",
+            "id": "45",
             "metadata": {},
             "source": [
                 "The `require_sftp_fileserver` fixture will ensure that the SFTP server is running during the test.\n",
                 "If SFTP tests have not been enabled by the command line option, the test will be skipped.\n",
                 "\n",
                 "Connecting to the server is not as straight forward as for the SciCat backend.\n",
                 "It requires passing a special `connect` function to the file transfer.\n",
                 "This can be done by requesting `sftp_connect_with_username_password`.\n",
                 "For example, the following opens a connection to the server to upload a file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "599b4199-ff30-4899-ab22-0af2b504ecae",
+            "id": "46",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scitacean.transfer.sftp import SFTPFileTransfer\n",
                 "\n",
                 "def test_sftp_upload(\n",
                 "    sftp_access,\n",
@@ -658,15 +658,15 @@
                 "        ...\n",
                 "    # assert that the file has been copied to sftp_data_dir\n",
                 "    ..."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c083ed37-0c9d-425a-bce3-a2ad44b47a43",
+            "id": "47",
             "metadata": {},
             "source": [
                 "Uploaded files are readable on the host.\n",
                 "So the test can read from `sftp_data_dir` to check if the upload succeeded.\n",
                 "This directory is mounted as `/data` on the server.\n",
                 "\n",
                 "Using an SFTP file transfer with `Client` requires some extra steps.\n",
@@ -678,15 +678,15 @@
                 "The server's filesystem gets seeded with some files from https://github.com/SciCatProject/scitacean/tree/main/src/scitacean/testing/sftp/sftp_server_seed.\n",
                 "Those files are copied to `sftp_data_dir` on the host which is mounted to `/data/seed` on the server."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a811256e-db50-450b-839c-fe9eb2e45c57",
+            "id": "48",
             "metadata": {
                 "nbsphinx": "hidden",
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# This cell is hidden.\n",
```

### Comparing `scitacean-23.8.0/docs/user-guide/uploading.ipynb` & `scitacean-24.4.0/docs/user-guide/uploading.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9871506008359456%*

 * *Differences: {"'cells'": "{0: {'id': '0'}, 1: {'id': '1'}, 2: {'id': '2'}, 3: {'id': '3'}, 4: {'id': '4'}, 5: "*

 * *            "{'id': '5'}, 6: {'id': '6'}, 7: {'id': '7'}, 8: {'id': '8'}, 9: {'id': '9'}, 10: "*

 * *            "{'id': '10'}, 11: {'id': '11'}, 12: {'id': '12'}, 13: {'id': '13'}, 14: {'id': '14'}, "*

 * *            "15: {'id': '15'}, 16: {'id': '16'}, 17: {'id': '17'}, 18: {'id': '18'}, 19: {'id': "*

 * *            "'19', 'source': {insert: [(4, 'However, the folder is ultimately determined by the "*

 * *            'file tr […]*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "e1d98ec6-9bab-4a7e-b75c-8defc9d184d0",
+            "id": "0",
             "metadata": {},
             "source": [
                 "# Uploading datasets\n",
                 "\n",
                 "Please read [Downloading datasets](./downloading.ipynb) first as it explains the general setup.\n",
                 "\n",
                 "We connect to SciCat and a file server using a [Client](../generated/classes/scitacean.Client.rst):\n",
@@ -23,61 +23,61 @@
                 ".\n",
                 "As with the downloading guide, we use a fake client instead of the real one shown above."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "78fec2b3-b03b-4711-b10b-48c5b9ab78e6",
+            "id": "1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scitacean.testing.docs import setup_fake_client\n",
                 "client = setup_fake_client()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a1c15f19-f83f-4fda-a83c-59ece80b81f8",
+            "id": "2",
             "metadata": {},
             "source": [
                 "This is especially useful here as datasets cannot be deleted from SciCat by regular users, and we don't want to pollute the database with our test data.\n",
                 "\n",
                 "First, we need to generate some data to upload:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9f32e0e2-e5b1-4a61-b7fa-07f495a8db99",
+            "id": "3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from pathlib import Path\n",
                 "\n",
                 "path = Path(\"data/witchcraft.dat\")\n",
                 "path.parent.mkdir(parents=True, exist_ok=True)\n",
                 "with path.open(\"w\") as f:\n",
                 "    f.write(\"7.9 13 666\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "acbcc0a4-fc75-4555-8665-a2bf4fb9c498",
+            "id": "4",
             "metadata": {},
             "source": [
                 "## Create a new dataset\n",
                 "\n",
                 "With the totally realistic data in hand, we can construct a dataset."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d85b8c79-9a4f-4c3b-bf20-e1b1bd4ccdab",
+            "id": "5",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from scitacean import Dataset\n",
                 "\n",
@@ -97,15 +97,15 @@
                 "    data_format=\"space-separated\",\n",
                 "    source_folder=\"/somewhere/on/remote\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "53bfee0c-82b3-4e2f-ad4b-929ea7df6519",
+            "id": "6",
             "metadata": {},
             "source": [
                 "There are many more fields that can be filled in as needed.\n",
                 "See [scitacean.Dataset](../generated/classes/scitacean.Dataset.rst).\n",
                 "\n",
                 "Some fields require an explanation:\n",
                 "\n",
@@ -114,89 +114,89 @@
                 "\n",
                 "Now we can attach our file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "01e303db-0e94-450a-acce-3ab48d034bb3",
+            "id": "7",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "dset.add_local_files(\"data/witchcraft.dat\", base_path=\"data\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "21d4bdcf-3cd4-4aea-898d-fa8713c48ff4",
+            "id": "8",
             "metadata": {},
             "source": [
                 "Setting the `base_path` to `\"data\"` means that the file will be uploaded to `source_folder/withcraft.dat` where `source_folder` will be determined by the file transfer.\n",
                 "(See below.)\n",
                 "If we did not set `base_path`, the file would end up in `source-dir/data/withcraft.dat`.\n",
                 "\n",
                 "Now, let's inspect the dataset."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "27ea91e9-5d9d-4856-b452-b20d3b3009da",
+            "id": "9",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "dset"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1c1c11a1-c29d-4c92-9efc-d120d5bf2582",
+            "id": "10",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "len(list(dset.files))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d0763ba4-5fa4-4db8-b7ac-ed225efd3993",
+            "id": "11",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "dset.size  # in bytes"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "249c1e79-40be-4e2c-bfa2-8b662604ede0",
+            "id": "12",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "file = list(dset.files)[0]\n",
                 "print(f\"{file.remote_access_path(dset.source_folder) = }\")\n",
                 "print(f\"{file.local_path = }\")\n",
                 "print(f\"{file.size = } bytes\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "38938be4-382d-4025-bbe1-19804cd13d8e",
+            "id": "13",
             "metadata": {},
             "source": [
                 "The file has a `local_path` but no `remote_access_path` which means that it exists on the local file system (where we put it earlier) but not on the remote file server accessible by SciCat.\n",
                 "The location can also be queried using `file.is_on_local` and `file.is_on_remote`.\n",
                 "\n",
                 "Likewise, the dataset only exists in memory on our local machine and not on SciCat.\n",
                 "Nothing has been uploaded yet.\n",
@@ -206,26 +206,26 @@
                 "\n",
                 "Once the dataset is ready, we can upload it using"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "46ac5ffe-c544-49b4-baf2-a71b3008f5af",
+            "id": "14",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "finalized = client.upload_new_dataset_now(dset)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b4dcd592-8228-436f-8969-05f2627cc473",
+            "id": "15",
             "metadata": {},
             "source": [
                 "<div class=\"alert alert-warning\">\n",
                 "    <b>WARNING:</b>\n",
                 "\n",
                 "This action cannot be undone by a regular user!\n",
                 "Contact an admin if you uploaded a dataset accidentally.\n",
@@ -238,97 +238,97 @@
                 "It returns a new dataset that is a copy of the input with some updated information generated by SciCat and the file transfer.\n",
                 "For example, it has been assigned a new ID:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e98e4339-970b-4b0b-9d3c-2dd03b9794c2",
+            "id": "16",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "finalized.pid"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "19d91fd6-0f6a-4bb3-9d9e-f71295623352",
+            "id": "17",
             "metadata": {},
             "source": [
                 "And the remote access path of our file has been set:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6c6d3650-410c-4ab6-9f56-fcd5290c8004",
+            "id": "18",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "list(finalized.files)[0].remote_access_path(finalized.source_folder)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5d5cd1c0-97fc-4931-acba-f2bea3ab1d7c",
+            "id": "19",
             "metadata": {},
             "source": [
                 "## Location of uploaded files\n",
                 "\n",
                 "All files associated with a dataset will be uploaded to the same folder.\n",
                 "This folder may be at the path we specify when making the dataset, i.e. `dset.source_folder`.\n",
-                "However, the folder is ultimately determined by the file transfer (in this case `SSHFileTransfer`) and it may choose to override the `source_folder` that we set.\n",
+                "However, the folder is ultimately determined by the file transfer (in this case SFTPFileTransfer`) and it may choose to override the `source_folder` that we set.\n",
                 "In this example, since we don't tell the file transfer otherwise, it respects `dset.source_folder` and uploads the files to that location.\n",
                 "See the [File transfer](../reference/index.rst#file-transfer) reference for information how to control this behavior.\n",
                 "The reason for this is that facilities may have a specific structure on their file server and Scitacean's file transfers can be used to enforce that.\n",
                 "\n",
                 "In any case, we can find out where files were uploaded by inspecting the finalized dataset that was returned by `client.upload_new_dataset_now`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "71beba39-b330-4251-bc2a-5584eb246fb2",
+            "id": "20",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "finalized.source_folder"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "95201e00-8119-4c34-9fe5-2d2bb58d826d",
+            "id": "21",
             "metadata": {},
             "source": [
                 "Or by looking at each file individually as shown in the section above."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ebbfc735-e8eb-4ceb-b5fb-ca252dd9ee6f",
+            "id": "22",
             "metadata": {},
             "source": [
                 "## Attaching images to datasets\n",
                 "\n",
                 "It is possible to attach *small* images to datasets.\n",
                 "In SciCat, this is done by creating 'attachment' objects which contain the image.\n",
                 "Scitacean handles those via the `attachments` property of `Dataset`.\n",
                 "For our locally created dataset, the property is an empty list and we can add an attachment like this:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5f15eedf-ab14-4f1b-8659-d8f62c6975bc",
+            "id": "23",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scitacean import Attachment, Thumbnail\n",
                 "\n",
                 "dset.attachments.append(\n",
                 "    Attachment(\n",
@@ -338,57 +338,57 @@
                 "    )\n",
                 ")\n",
                 "dset.attachments[0]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "986b6271-4faf-4b2c-9283-872f6fdf8281",
+            "id": "24",
             "metadata": {},
             "source": [
                 "We used `Thumbnail.load_file` because it properly encodes the file for SciCat.\n",
                 "\n",
                 "When we then upload the dataset, the client automatically uploads all attachments as well.\n",
                 "Note that this creates a new dataset in SciCat.\n",
                 "If you want to add attachments to an existing dataset after upload, you need to use the lower-level API through `client.scicat.create_attachment_for_dataset` or the web interface directly."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f82de9eb-2a34-436c-8694-1a13af82cb66",
+            "id": "25",
             "metadata": {},
             "outputs": [],
             "source": [
                 "finalized = client.upload_new_dataset_now(dset)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7f686546-da06-4c15-b357-b44da8bfc328",
+            "id": "26",
             "metadata": {},
             "source": [
                 "In order to download the attachments again, we can pass `attachments=True` when downloading the dataset:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b8a673c7-20b2-4e0e-a003-016227821651",
+            "id": "27",
             "metadata": {},
             "outputs": [],
             "source": [
                 "downloaded = client.get_dataset(finalized.pid, attachments=True)\n",
                 "downloaded.attachments[0]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d8dbbd21-81a6-4610-965a-5e23446d593f",
+            "id": "28",
             "metadata": {
                 "nbsphinx": "hidden",
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# This cell is hidden.\n",
```

### Comparing `scitacean-23.8.0/pyproject.toml` & `scitacean-24.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 [build-system]
 requires = [
-    "setuptools>=45",
-    "setuptools_scm[toml]>=7.0",
+    "setuptools>=68",
+    "setuptools_scm[toml]>=8.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scitacean"
 description = "High-level interface for SciCat"
 license = { "file" = "LICENSE" }
 authors = [{ name = "Scitacean contributors" }]
 readme = "README.md"
 keywords = ["scicat"]
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Typing :: Typed",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dependencies = [
     "email-validator",
-    "pydantic >= 1.9",
+    "pydantic >= 2",
     "python-dateutil",
     "requests >= 2.31",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Documentation" = "https://scicatproject.github.io/scitacean"
 "Bug Tracker" = "https://github.com/SciCatProject/scitacean/issues"
 "Source" = "https://github.com/SciCatProject/scitacean"
 
 [project.optional-dependencies]
-ssh = ["fabric"]
 sftp = ["paramiko"]
 test = ["filelock", "hypothesis", "pyyaml"]
 
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 testpaths = "tests"
 addopts = """
 --strict-config
 --strict-markers
+--disable-socket
+--allow-hosts=127.0.0.1,::1
 -ra
 -v
 --hypothesis-profile=scitacean
 """
 filterwarnings = [
     "error",
     # Many tests don't set a checksum, so File raises this warning.
     "ignore:Cannot check if local file:UserWarning",
-    # Internal deprecations.
-    "ignore:SSHFileTransfer is deprecated:scitacean.VisibleDeprecationWarning",
-    # From fabric / invoke
-    "ignore:_SixMetaPathImporter:ImportWarning",
-    "ignore:the imp module is deprecated in favour of importlib:DeprecationWarning",
 ]
 
 [tool.mypy]
 plugins = "pydantic.mypy"
 mypy_path = "src"
 exclude = ["docs/conf.py", "tools/model-generation", "venv"]
 ignore_missing_imports = true
@@ -90,29 +86,40 @@
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 
 [tool.ruff]
 line-length = 88
-select = ["B", "D", "E", "F", "I", "S", "T20", "PGH", "FBT003", "RUF"]
+extend-include = ["*.ipynb"]
+extend-exclude = [".*", "__pycache__", "build", "dist", "venv"]
+
+[tool.ruff.lint]
+select = ["B", "D", "E", "F", "G", "I", "S", "T20", "UP", "PGH", "FBT003", "RUF"]
 ignore = [
     "B905", # `zip()` without an explicit `strict=` parameter
     "S324", # insecure hsh function; we don't use hashing for security
     "E741", "E742", "E743", # do not use names ‘l’, ‘O’, or ‘I’; they are not a problem with a proper font
-    "D100", "D101", "D102", "D103", "D104", "D105", # TODO remove D10* once everything has docstrings
+    "UP038",  # does not seem to work and leads to slower code
+    "E111", "E114", "E117", "D206", "D300",  # conflict with ruff format
+    "D105",
 ]
-extend-exclude = [".*", "__pycache__", "build", "dist", "venv"]
 fixable = ["I001"]
+isort.known-first-party = ["scitacean"]
+pydocstyle.convention = "numpy"
 
-[tool.ruff.per-file-ignores]
-"tests/*" = ["S101"]  # asserts are fine in tests
+[tool.ruff.lint.per-file-ignores]
+"tests/*" = [
+    "S101",  # asserts are fine in tests
+    "D10",  # no docstrings required in tests
+]
+"docs/*" = [
+    "D", "E402", "F811", "F841", "RUF015", "S101", "T201",
+]
+"*.ipynb" = ["I"]
+"docs/conf.py" = ["D10"]
+"tools/*" = ["D10"]
+"src/scitacean/model.py" = ["D10"]
 "src/scitacean/testing/strategies.py" = ["D401"]
 
-[tool.ruff.isort]
-known-first-party = ["scitacean"]
-
-[tool.ruff.pydocstyle]
-convention = "numpy"
-
 [tool.codespell]
 ignore-words-list = "specfield"
```

### Comparing `scitacean-23.8.0/requirements/base.txt` & `scitacean-24.4.0/requirements/base.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,63 @@
-# SHA1:f8c625c62cb057cead0d70b0a458c8aed4f43459
+# SHA1:6b8a253be2c23e3bf131e90c6b06c34bf612344f
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-bcrypt==4.0.1
+annotated-types==0.6.0
+    # via pydantic
+bcrypt==4.1.2
     # via paramiko
-certifi==2023.7.22
+certifi==2024.2.2
     # via requests
-cffi==1.15.1
+cffi==1.16.0
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==3.2.0
+charset-normalizer==3.3.2
     # via requests
-cryptography==41.0.3
+cryptography==42.0.5
     # via paramiko
 decorator==5.1.1
     # via fabric
 deprecated==1.2.14
     # via fabric
-dnspython==2.4.2
+dnspython==2.6.1
     # via email-validator
-email-validator==2.0.0.post2
-    # via -r requirements/base.in
-fabric==3.2.1
-    # via -r requirements/base.in
-idna==3.4
+email-validator==2.1.1
+    # via -r base.in
+fabric==3.2.2
+    # via -r base.in
+idna==3.7
     # via
     #   email-validator
     #   requests
 invoke==2.2.0
     # via fabric
-paramiko==3.3.1
+paramiko==3.4.0
     # via
-    #   -r requirements/base.in
+    #   -r base.in
     #   fabric
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pydantic==1.10.12
-    # via -r requirements/base.in
+pydantic==2.7.0
+    # via -r base.in
+pydantic-core==2.18.1
+    # via pydantic
 pynacl==1.5.0
     # via paramiko
-python-dateutil==2.8.2
-    # via -r requirements/base.in
+python-dateutil==2.9.0.post0
+    # via -r base.in
 requests==2.31.0
-    # via -r requirements/base.in
+    # via -r base.in
 six==1.16.0
     # via python-dateutil
-typing-extensions==4.7.1
-    # via pydantic
-urllib3==2.0.4
+typing-extensions==4.11.0
+    # via
+    #   pydantic
+    #   pydantic-core
+urllib3==2.2.1
     # via requests
-wrapt==1.15.0
+wrapt==1.16.0
     # via deprecated
```

### Comparing `scitacean-23.8.0/requirements/ci.txt` & `scitacean-24.4.0/requirements/ci.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # SHA1:7bdf31978c0210720b3420242d2f1d74927c098c
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-cachetools==5.3.1
+cachetools==5.3.3
     # via tox
 chardet==5.2.0
     # via tox
 colorama==0.4.6
     # via tox
-distlib==0.3.7
+distlib==0.3.8
     # via virtualenv
-filelock==3.12.2
+filelock==3.13.4
     # via
     #   tox
     #   virtualenv
-packaging==23.1
+packaging==24.0
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.10.0
+platformdirs==4.2.0
     # via
     #   tox
     #   virtualenv
-pluggy==1.3.0
+pluggy==1.4.0
     # via tox
-pyproject-api==1.5.4
+pyproject-api==1.6.1
     # via tox
-tox==4.10.0
-    # via -r requirements/ci.in
-virtualenv==20.24.3
+tomli==2.0.1
+    # via
+    #   pyproject-api
+    #   tox
+tox==4.14.2
+    # via -r ci.in
+virtualenv==20.25.3
     # via tox
```

### Comparing `scitacean-23.8.0/requirements/docs.txt` & `scitacean-24.4.0/requirements/docs.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,213 +1,208 @@
-# SHA1:330f38cb197740f43425c68384e5bd0b8ba57335
+# SHA1:4abccc1a686655d0cf411d9fa981ce865ab25d57
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
 -r test.txt
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
-asttokens==2.2.1
+asttokens==2.4.1
     # via stack-data
-autodoc-pydantic==1.9.0
-    # via -r requirements/docs.in
-babel==2.12.1
+autodoc-pydantic==2.1.0
+    # via -r docs.in
+babel==2.14.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
-backcall==0.2.0
-    # via ipython
-beautifulsoup4==4.12.2
+beautifulsoup4==4.12.3
     # via
     #   nbconvert
     #   pydata-sphinx-theme
-bleach==6.0.0
+bleach==6.1.0
     # via nbconvert
-comm==0.1.4
+comm==0.2.2
     # via ipykernel
-debugpy==1.6.7.post1
+debugpy==1.8.1
     # via ipykernel
 defusedxml==0.7.1
     # via nbconvert
 docutils==0.20.1
     # via
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx
-executing==1.2.0
+executing==2.0.1
     # via stack-data
-fastjsonschema==2.18.0
+fastjsonschema==2.19.1
     # via nbformat
 imagesize==1.4.1
     # via sphinx
-ipykernel==6.25.1
-    # via -r requirements/docs.in
-ipython==8.14.0
+ipykernel==6.29.4
+    # via -r docs.in
+ipython==8.23.0
     # via
-    #   -r requirements/docs.in
+    #   -r docs.in
     #   ipykernel
-jedi==0.19.0
+jedi==0.19.1
     # via ipython
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-jsonschema==4.19.0
+jsonschema==4.21.1
     # via nbformat
-jsonschema-specifications==2023.7.1
+jsonschema-specifications==2023.12.1
     # via jsonschema
-jupyter-client==8.3.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   nbclient
-jupyter-core==5.3.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   nbclient
     #   nbconvert
     #   nbformat
-jupyterlab-pygments==0.2.2
+jupyterlab-pygments==0.3.0
     # via nbconvert
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==3.0.1
+mistune==3.0.2
     # via nbconvert
 myst-parser==2.0.0
-    # via -r requirements/docs.in
-nbclient==0.8.0
+    # via -r docs.in
+nbclient==0.10.0
     # via nbconvert
-nbconvert==7.7.4
+nbconvert==7.16.3
     # via nbsphinx
-nbformat==5.9.2
+nbformat==5.10.4
     # via
     #   nbclient
     #   nbconvert
     #   nbsphinx
 nbsphinx==0.9.3
-    # via -r requirements/docs.in
-nest-asyncio==1.5.7
+    # via -r docs.in
+nest-asyncio==1.6.0
     # via ipykernel
-pandocfilters==1.5.0
+pandocfilters==1.5.1
     # via nbconvert
-parso==0.8.3
+parso==0.8.4
     # via jedi
-pexpect==4.8.0
-    # via ipython
-pickleshare==0.7.5
+pexpect==4.9.0
     # via ipython
-platformdirs==3.10.0
+platformdirs==4.2.0
     # via jupyter-core
-prompt-toolkit==3.0.39
+prompt-toolkit==3.0.43
     # via ipython
-psutil==5.9.5
+psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pydata-sphinx-theme==0.13.3
-    # via -r requirements/docs.in
-pygments==2.16.1
+pydantic-settings==2.2.1
+    # via autodoc-pydantic
+pydata-sphinx-theme==0.15.2
+    # via -r docs.in
+pygments==2.17.2
     # via
     #   accessible-pygments
     #   ipython
     #   nbconvert
     #   pydata-sphinx-theme
     #   sphinx
-pyzmq==25.1.1
+python-dotenv==1.0.1
+    # via pydantic-settings
+pyzmq==26.0.1
     # via
     #   ipykernel
     #   jupyter-client
-referencing==0.30.2
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
-rpds-py==0.9.2
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
 snowballstemmer==2.2.0
     # via sphinx
-soupsieve==2.4.1
+soupsieve==2.5
     # via beautifulsoup4
-sphinx==7.1.0
+sphinx==7.3.7
     # via
-    #   -r requirements/docs.in
+    #   -r docs.in
     #   autodoc-pydantic
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
     #   sphinx-copybutton
     #   sphinx-design
-    #   sphinxcontrib-applehelp
-    #   sphinxcontrib-devhelp
-    #   sphinxcontrib-htmlhelp
-    #   sphinxcontrib-qthelp
-    #   sphinxcontrib-serializinghtml
-sphinx-autodoc-typehints==1.24.0
-    # via -r requirements/docs.in
+sphinx-autodoc-typehints==2.1.0
+    # via -r docs.in
 sphinx-copybutton==0.5.2
-    # via -r requirements/docs.in
+    # via -r docs.in
 sphinx-design==0.5.0
-    # via -r requirements/docs.in
-sphinxcontrib-applehelp==1.0.7
+    # via -r docs.in
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.5
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.4
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.6
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.9
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-stack-data==0.6.2
+stack-data==0.6.3
     # via ipython
 tinycss2==1.2.1
     # via nbconvert
-tornado==6.3.3
+tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-traitlets==5.9.0
+traitlets==5.14.3
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
     #   nbclient
     #   nbconvert
     #   nbformat
     #   nbsphinx
-wcwidth==0.2.6
+wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
```

### Comparing `scitacean-23.8.0/requirements/static.txt` & `scitacean-24.4.0/requirements/static.txt`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 cfgv==3.4.0
     # via pre-commit
-distlib==0.3.7
+distlib==0.3.8
     # via virtualenv
-filelock==3.12.2
+filelock==3.13.4
     # via virtualenv
-identify==2.5.27
+identify==2.5.35
     # via pre-commit
 nodeenv==1.8.0
     # via pre-commit
-platformdirs==3.10.0
+platformdirs==4.2.0
     # via virtualenv
-pre-commit==3.3.3
-    # via -r requirements/static.in
+pre-commit==3.7.0
+    # via -r static.in
 pyyaml==6.0.1
     # via pre-commit
-virtualenv==20.24.3
+virtualenv==20.25.3
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `scitacean-23.8.0/src/scitacean/__init__.py` & `scitacean-24.4.0/src/scitacean/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
+
+"""High-level interface for SciCat."""
 
 import importlib.metadata
 
 try:
     __version__ = importlib.metadata.version(__package__ or __name__)
 except importlib.metadata.PackageNotFoundError:
     __version__ = "0.0.0"
 
 from .client import Client
 from .datablock import OrigDatablock
 from .dataset import Dataset
 from .error import FileUploadError, IntegrityError, ScicatCommError, ScicatLoginError
 from .file import File
 from .filesystem import RemotePath
-from .model import Attachment, DatasetType
+from .model import Attachment, DatasetType, Sample
 from .pid import PID
 from .thumbnail import Thumbnail
 from .warning import VisibleDeprecationWarning
 
 __all__ = (
     "Attachment",
     "Client",
@@ -26,12 +28,13 @@
     "DatasetType",
     "File",
     "FileUploadError",
     "IntegrityError",
     "OrigDatablock",
     "PID",
     "RemotePath",
+    "Sample",
     "ScicatCommError",
     "ScicatLoginError",
     "Thumbnail",
     "VisibleDeprecationWarning",
 )
```

### Comparing `scitacean-23.8.0/src/scitacean/_base_model.py` & `scitacean-24.4.0/src/scitacean/_base_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 """Types and functions to implement models for communication with SciCat."""
+
 from __future__ import annotations
 
 import dataclasses
+from collections.abc import Iterable
 from datetime import datetime
 from typing import (
     Any,
     ClassVar,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    Type,
     TypeVar,
-    Union,
     overload,
 )
 
 import pydantic
 from dateutil.parser import parse as parse_datetime
 
 from ._internal.orcid import is_valid_orcid
-from ._internal.pydantic_compat import is_pydantic_v1
-from .filesystem import RemotePath
 from .logging import get_logger
-from .pid import PID
-from .thumbnail import Thumbnail
 
 try:
     # Python 3.11+
     from enum import StrEnum
 
     class DatasetType(StrEnum):
         """Type of Dataset."""
@@ -53,140 +44,101 @@
 
     del Enum
 
 
 class BaseModel(pydantic.BaseModel):
     """Base class for Pydantic models for communication with SciCat."""
 
-    if is_pydantic_v1():
-
-        class Config:
-            extra = pydantic.Extra.forbid
-            json_encoders = {  # noqa: RUF012
-                PID: lambda v: str(v),
-                RemotePath: lambda v: v.posix,
-                Thumbnail: lambda v: v.serialize(),
-            }
-
-    else:
-        model_config = pydantic.ConfigDict(
-            extra="forbid",
-        )
+    model_config = pydantic.ConfigDict(
+        extra="forbid",
+    )
 
-    _user_mask: ClassVar[Tuple[str, ...]]
-    _masked_fields: ClassVar[Optional[Tuple[str, ...]]] = None
+    _user_mask: ClassVar[tuple[str, ...]]
+    _masked_fields: ClassVar[tuple[str, ...] | None] = None
 
     # Some schemas contain fields that we don't want to use in Scitacean.
     # Normally, omitting them from the model would result in an error when
     # building a model from the JSON returned by SciCat.
     # The following subclass hook allows models to mark fields as masked.
     # Those will be silently dropped by __init__.
     # Note also the comment for _IGNORED_KWARGS below.
     def __init_subclass__(
-        cls, /, masked: Optional[Iterable[str]] = None, **kwargs: Any
+        cls, /, masked: Iterable[str] | None = None, **kwargs: Any
     ) -> None:
         super().__init_subclass__(**kwargs)
         cls._user_mask = tuple(masked) if masked is not None else ()
 
     def __init__(self, **kwargs: Any) -> None:
         self._delete_ignored_args(kwargs)
         super().__init__(**kwargs)
 
-    def _delete_ignored_args(self, args: Dict[str, Any]) -> None:
+    def _delete_ignored_args(self, args: dict[str, Any]) -> None:
         if self._masked_fields is None:
             self._init_mask(self)
         for key in self._masked_fields:  # type: ignore[union-attr]
             args.pop(key, None)
 
     # Initializing the mask requires the field names which
     # are only available on instances.
     # So initialization needs to be deferred until the first instantiation of the model.
     # The mask is cached afterward.
     @classmethod
-    def _init_mask(cls: Type[ModelType], instance: ModelType) -> None:
+    def _init_mask(cls: type[ModelType], instance: ModelType) -> None:
         def get_name(name: str, field: Any) -> Any:
             return field.alias if field.alias is not None else name
 
         field_names = {
-            get_name(name, field) for name, field in instance.get_model_fields().items()
+            get_name(name, field) for name, field in instance.model_fields.items()
         }
         default_mask = tuple(key for key in _IGNORED_KWARGS if key not in field_names)
         cls._masked_fields = cls._user_mask + default_mask
 
     @classmethod
-    def user_model_type(cls) -> Optional[Type[BaseUserModel]]:
+    def user_model_type(cls) -> type[BaseUserModel] | None:
         """Return the user model type for this model.
 
         Returns ``None`` if there is no user model, e.g., for ``Dataset``
         where there is a custom class instead of a plain model.
         """
         return None
 
     @classmethod
-    def upload_model_type(cls) -> Optional[Type[BaseModel]]:
+    def upload_model_type(cls) -> type[BaseModel] | None:
         """Return the upload model type for this model.
 
         Returns ``None`` if the model cannot be uploaded or this is an upload model.
         """
         return None
 
     @classmethod
-    def download_model_type(cls) -> Optional[Type[BaseModel]]:
+    def download_model_type(cls) -> type[BaseModel] | None:
         """Return the download model type for this model.
 
         Returns ``None`` if this is a download model.
         """
         return None
 
-    if is_pydantic_v1():
-
-        @classmethod
-        def get_model_fields(cls) -> Dict[str, Any]:
-            return cls.__fields__  # type: ignore[return-value]
-
-        def model_dump(self, *args: Any, **kwargs: Any) -> Dict[str, Any]:
-            return self.dict(*args, **kwargs)
-
-        def model_dump_json(self, *args: Any, **kwargs: Any) -> str:
-            return self.json(*args, **kwargs)
-
-        @classmethod
-        def model_construct(
-            cls: Type[ModelType], *args: Any, **kwargs: Any
-        ) -> ModelType:
-            return cls.construct(*args, **kwargs)
-
-        @classmethod
-        def model_rebuild(cls, *args: Any, **kwargs: Any) -> Optional[bool]:
-            return cls.update_forward_refs(*args, **kwargs)
-
-    else:
-
-        @classmethod
-        def get_model_fields(cls) -> Dict[str, pydantic.fields.FieldInfo]:
-            return cls.model_fields
-
 
 @dataclasses.dataclass
 class BaseUserModel:
     """Base class for user models.
 
     Child classes must be dataclasses.
     """
 
     @classmethod
-    def _download_model_dict(cls, download_model: Any) -> Dict[str, Any]:
+    def _download_model_dict(cls, download_model: Any) -> dict[str, Any]:
         return {
             field.name: getattr(
                 download_model, _model_field_name_of(cls.__name__, field.name)
             )
             for field in dataclasses.fields(cls)
         }
 
-    def _upload_model_dict(self) -> Dict[str, Any]:
+    def _upload_model_dict(self) -> dict[str, Any]:
         _check_ready_for_upload(self)
         return {
             _model_field_name_of(self.__class__.__name__, field.name): getattr(
                 self, field.name
             )
             for field in dataclasses.fields(self)
             if not field.name.startswith("_")
@@ -196,38 +148,38 @@
     def from_download_model(cls, download_model: Any) -> BaseUserModel:
         raise NotImplementedError("Function does not exist for BaseUserModel")
 
     def make_upload_model(self) -> BaseModel:
         raise NotImplementedError("Function does not exist for BaseUserModel")
 
     @classmethod
-    def upload_model_type(cls) -> Optional[Type[BaseModel]]:
+    def upload_model_type(cls) -> type[BaseModel] | None:
         """Return the upload model type for this user model.
 
         Returns ``None`` if the model cannot be uploaded.
         """
         return None
 
     @classmethod
-    def download_model_type(cls) -> Type[BaseModel]:
+    def download_model_type(cls) -> type[BaseModel]:
         """Return the download model type for this user model."""
         # There is no sensible default value here as there always exists a download
         # model.
         # All child classes must implement this function.
         raise NotImplementedError("Function does not exist for BaseUserModel")
 
-    def _repr_html_(self) -> Optional[str]:
+    def _repr_html_(self) -> str | None:
         """Return an HTML representation of the model if possible."""
         from ._html_repr import user_model_html_repr
 
         return user_model_html_repr(self)
 
 
 def construct(
-    model: Type[PydanticModelType],
+    model: type[PydanticModelType],
     *,
     _strict_validation: bool = True,
     _quiet: bool = False,
     **fields: Any,
 ) -> PydanticModelType:
     """Instantiate a SciCat model.
 
@@ -267,15 +219,15 @@
                 "The returned object may be incomplete or broken. "
                 "In particular, some fields may not have the correct type",
                 str(e),
             )
         return model.model_construct(**fields)
 
 
-def validate_datetime(value: Optional[Union[str, datetime]]) -> Optional[datetime]:
+def validate_datetime(value: str | datetime | None) -> datetime | None:
     """Convert strings to datetimes.
 
     This uses dateutil.parser.parse instead of Pydantic's builtin parser in order to
     produce results that are consistent with user inputs.
     Pydantic uses a custom type for timezones which is not fully compatible with
     dateutil's.
     """
@@ -285,84 +237,78 @@
 
 
 def validate_drop(_: Any) -> None:
     """Return ``None``."""
     return None
 
 
-def validate_emails(value: Optional[str]) -> Optional[str]:
+def validate_emails(value: str | None) -> str | None:
     if value is None:
         return value
     return ";".join(pydantic.validate_email(item)[1] for item in value.split(";"))
 
 
-def validate_orcids(value: Optional[str]) -> Optional[str]:
+def validate_orcids(value: str | None) -> str | None:
     if value is None:
         return value
     try:
         if is_valid_orcid(value):
             return value
     except (RuntimeError, ValueError, TypeError):
         pass
     raise ValueError(
         "value is not a valid ORCID, "
         "note that ORCIDs must be prefixed with 'https://orcid.org'."
     )
 
 
 @overload
-def convert_download_to_user_model(download_model: None) -> None:
-    ...
+def convert_download_to_user_model(download_model: None) -> None: ...
 
 
 @overload
-def convert_download_to_user_model(download_model: BaseModel) -> BaseUserModel:
-    ...
+def convert_download_to_user_model(download_model: BaseModel) -> BaseUserModel: ...
 
 
 @overload
 def convert_download_to_user_model(
     download_model: Iterable[BaseModel],
-) -> List[BaseUserModel]:
-    ...
+) -> list[BaseUserModel]: ...
 
 
 def convert_download_to_user_model(
-    download_model: Optional[Union[BaseModel, Iterable[BaseModel]]]
-) -> Optional[Union[BaseUserModel, List[BaseUserModel]]]:
+    download_model: BaseModel | Iterable[BaseModel] | None,
+) -> BaseUserModel | list[BaseUserModel] | None:
     """Construct user models from download models."""
     if download_model is None:
         return download_model
     if isinstance(download_model, BaseModel):
         if (user_type := download_model.user_model_type()) is None:
             raise TypeError("Cannot convert to user model in this way.")
         return user_type.from_download_model(download_model)
     return list(map(convert_download_to_user_model, download_model))
 
 
 @overload
-def convert_user_to_upload_model(user_model: None) -> None:
-    ...
+def convert_user_to_upload_model(user_model: None) -> None: ...
 
 
 @overload
-def convert_user_to_upload_model(user_model: BaseUserModel) -> BaseModel:
-    ...
+def convert_user_to_upload_model(user_model: BaseUserModel) -> BaseModel: ...
 
 
 @overload
 def convert_user_to_upload_model(
     user_model: Iterable[BaseUserModel],
-) -> List[BaseModel]:
-    ...
+) -> list[BaseModel]: ...
 
 
 def convert_user_to_upload_model(
-    user_model: Optional[Union[BaseUserModel, Iterable[BaseUserModel]]]
-) -> Optional[Union[BaseModel, List[BaseModel]]]:
+    user_model: BaseUserModel | Iterable[BaseUserModel] | None,
+) -> BaseModel | list[BaseModel] | None:
     """Construct upload models from user models."""
     if user_model is None:
         return None
     if isinstance(user_model, BaseUserModel):
         return user_model.make_upload_model()
     return list(map(convert_user_to_upload_model, user_model))
```

### Comparing `scitacean-23.8.0/src/scitacean/_dataset_fields.py` & `scitacean-24.4.0/src/scitacean/_dataset_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ##########################################
 # This file was automatically generated. #
 # Do not modify it directly!             #
 ##########################################
 
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # flake8: noqa
 
 """Base class for Dataset."""
 
 from __future__ import annotations
 
 from datetime import datetime, timezone
@@ -1050,19 +1050,14 @@
         self._meta = meta
 
     @property
     def type(self) -> DatasetType:
         """Characterize type of dataset, either 'raw' or 'derived'. Autofilled when choosing the proper inherited models."""
         return self._type
 
-    @type.setter
-    def type(self, type: Union[DatasetType, Literal["raw", "derived"]]) -> None:
-        """Characterize type of dataset, either 'raw' or 'derived'. Autofilled when choosing the proper inherited models."""
-        self._type = DatasetType(type)
-
     @staticmethod
     def _prepare_fields_from_download(
         download_model: DownloadDataset,
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         init_args = {}
         read_only = {}
         for field in DatasetBase._FIELD_SPEC:
```

### Comparing `scitacean-23.8.0/src/scitacean/_html_repr/__init__.py` & `scitacean-24.4.0/src/scitacean/_html_repr/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """HTML representations for Jupyter."""
+
 from __future__ import annotations
 
+from collections.abc import Callable
 from functools import lru_cache
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
+from typing import TYPE_CHECKING, Any
 
 from ._attachment_html import attachment_html_repr
 from ._dataset_html import dataset_html_repr
 
 if TYPE_CHECKING:
     from ..model import BaseUserModel
 
 
 @lru_cache(maxsize=1)
-def _user_model_reprs() -> Dict[type, Callable[[Any], str]]:
+def _user_model_reprs() -> dict[type, Callable[[Any], str]]:
     from ..model import Attachment
 
     return {Attachment: attachment_html_repr}
 
 
-def user_model_html_repr(user_model: BaseUserModel) -> Optional[str]:
+def user_model_html_repr(user_model: BaseUserModel) -> str | None:
     """HTML representation of a user model f implemented."""
     if (repr_fn := _user_model_reprs().get(type(user_model))) is not None:
         return repr_fn(user_model)
     return None
 
 
 __all__ = ["dataset_html_repr", "user_model_html_repr"]
```

### Comparing `scitacean-23.8.0/src/scitacean/_html_repr/_attachment_html.py` & `scitacean-24.4.0/src/scitacean/_html_repr/_attachment_html.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,59 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """HTML representations for attachments for Jupyter."""
 
 from __future__ import annotations
 
 import dataclasses
-from typing import List
 
 from ..model import Attachment, UploadAttachment
 from . import _resources
 from ._common_html import Field, format_field_flag, format_type, format_value
 
 
 def attachment_html_repr(attachment: Attachment) -> str:
     template = _resources.attachment_repr_template()
     style_sheet = _resources.attachment_style()
     rows = "\n".join(_format_field(field) for field in _get_fields(attachment))
-    thumbnail = attachment.thumbnail._repr_mimebundle_(include=("text/html",))[
-        "text/html"
-    ]
+    if attachment.thumbnail is None:
+        thumbnail = ""
+    else:
+        bundle = attachment.thumbnail._repr_mimebundle_(include=("text/html",))
+        thumbnail = bundle["text/html"]  # type: ignore[assignment]
     return template.substitute(
         style_sheet=style_sheet,
         caption=format_value(attachment.caption),
         rows=rows,
         thumbnail=thumbnail,
     )
 
 
 def _format_field(field: Field) -> str:
     name = field.name
     flag = format_field_flag(field)
-    typ = _format_type(field.type)
+    typ = format_type(field.type)
     value = format_value(field.value)
 
     template = _resources.attachment_field_repr_template()
     return template.substitute(
         name=name,
         flag=flag,
         type=typ,
         value=value,
     )
 
 
-# Types are strings in Attachment because of
-# from __future__ import annotations
-def _format_type(typ: str) -> str:
-    if typ.startswith("Optional["):
-        typ = typ[9:-1]
-    return format_type(typ)
-
-
 _EXCLUDED_FIELDS = {
     "caption",
     "thumbnail",
 }
 
 
-def _get_fields(attachment: Attachment) -> List[Field]:
+def _get_fields(attachment: Attachment) -> list[Field]:
     fields = [
         Field(
             name=_strip_leading_underscore(field.name),
             value=getattr(attachment, field.name),
             type=field.type,
             description="",
             read_only=_is_read_only(field.name),
@@ -75,8 +68,8 @@
 
 
 def _strip_leading_underscore(s: str) -> str:
     return s[1:] if s.startswith("_") else s
 
 
 def _is_read_only(field_name: str) -> bool:
-    return field_name not in UploadAttachment.__fields__
+    return field_name not in UploadAttachment.model_fields
```

### Comparing `scitacean-23.8.0/src/scitacean/_html_repr/_common_html.py` & `scitacean-24.4.0/src/scitacean/_html_repr/_common_html.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Common functions for HTML reprs."""
 
 import html
 from datetime import datetime
-from typing import Any, List, Optional
+from typing import Any
 
 from .._internal.dataclass_wrapper import dataclass_optional_args
 from ..filesystem import RemotePath
 from ..model import History, Lifecycle, Relationship, Technique
 from ..pid import PID
 from . import _resources
 
@@ -17,47 +17,51 @@
 class Field:
     name: str
     value: Any
     type: type
     description: str
     read_only: bool
     required: bool
-    error: Optional[str]
+    error: str | None
     main: bool
 
 
 _TYPE_NAME = {
     str: "str",
     int: "int",
     bool: "bool",
     dict: "dict",
     datetime: "datetime",
     History: "History",
     Lifecycle: "Lifecycle",
     PID: "PID",
     RemotePath: "RemotePath",
-    List[str]: "list[str]",
-    List[PID]: "list[PID]",
-    List[Relationship]: "list[Relationship]",
-    List[Technique]: "list[Technique]",
-    List[dict]: "list[dict]",  # type: ignore[type-arg]
+    list[str]: "list[str]",
+    list[PID]: "list[PID]",
+    list[Relationship]: "list[Relationship]",
+    list[Technique]: "list[Technique]",
+    list[dict]: "list[dict]",  # type: ignore[type-arg]
 }
 
 
 def format_value(val: Any) -> str:
     """Return a str repr for a field value."""
     if val is None:
         return '<span class="cean-empty-field">None</span>'
     if isinstance(val, datetime):
         return val.strftime("%Y-%m-%d %H:%M:%S%z")
     return html.escape(str(val))
 
 
 def format_type(typ: Any) -> str:
     """Return a concise str repr for a type."""
+    # Types are strings model.py because of
+    # from __future__ import annotations
+    if isinstance(typ, str) and typ.startswith("Optional["):
+        typ = typ[9:-1]
     try:
         return _TYPE_NAME[typ]
     except KeyError:
         return html.escape(str(typ))
 
 
 def format_field_flag(field: Field) -> str:
```

### Comparing `scitacean-23.8.0/src/scitacean/_html_repr/_dataset_html.py` & `scitacean-24.4.0/src/scitacean/_html_repr/_dataset_html.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """HTML representations of datasets for Jupyter."""
 
 import html
-from typing import Any, Dict, Iterable, List, Optional
+from collections.abc import Iterable
+from typing import Any
 
 import pydantic
 
 from ..dataset import Dataset
 from ..model import DatasetType
 from . import _resources
 from ._common_html import Field, format_field_flag, format_type, format_value
@@ -128,15 +129,15 @@
     "creation_time",
     "proposal_id",
     "sample_id",
     "input_datasets",
 }
 
 
-def _get_fields(dset: Dataset) -> List[Field]:
+def _get_fields(dset: Dataset) -> list[Field]:
     validation = _validate(dset)
     fields = [
         Field(
             name=field.name,
             value=getattr(dset, field.name, None),
             type=field.type,
             description=field.description,
@@ -151,22 +152,20 @@
     ]
     return sorted(
         sorted(fields, key=lambda field: field.name),
         key=lambda field: not field.required,
     )
 
 
-def _check_error(field: Dataset.Field, validation: Dict[str, str]) -> Optional[str]:
-    if field.name in validation:
-        # TODO validation uses model names (camelCase)
-        return validation[field.name]
-    return None
+def _check_error(field: Dataset.Field, validation: dict[str, str]) -> str | None:
+    field_spec = next(filter(lambda f: f.name == field.name, Dataset.fields()))
+    return validation.get(field_spec.scicat_name, None)
 
 
-def _validate(dset: Dataset) -> Dict[str, str]:
+def _validate(dset: Dataset) -> dict[str, str]:
     def single_elem(xs: Iterable[Any]) -> Any:
         (x,) = xs
         return x
 
     try:
         dset.validate()
         return {}
@@ -205,10 +204,13 @@
             return f"{size_in_bytes/n:.2f} {prefix}iB"
     return f"{size_in_bytes} B"
 
 
 def _row_highlight_classes(field: Field) -> str:
     if field.required and field.value is None:
         return "cean-missing-value"
-    if field.error:
+    # Do not flag read-only fields with a value as errors.
+    # Validation is geared towards uploading where such fields must be None.
+    # But here, we don't want to flag downloaded datasets as bad because of this.
+    if field.error and not (field.read_only and field.error.startswith("Extra inputs")):
         return "cean-error"
     return ""
```

### Comparing `scitacean-23.8.0/src/scitacean/_html_repr/_resources.py` & `scitacean-24.4.0/src/scitacean/_html_repr/_resources.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Handler for packaged assets."""
 
 import importlib.resources
 from functools import lru_cache
 from string import Template
 
 
 def _read_text(filename: str, group: str) -> str:
-    if hasattr(importlib.resources, "files"):
-        # Use new API added in Python 3.9
-        return (
-            importlib.resources.files(f"scitacean._html_repr.{group}")
-            .joinpath(filename)
-            .read_text()
-        )
-    # Old API, deprecated as of Python 3.11
-    # When this is removed, also remove the __init__.py files in the resource folders.
-    return importlib.resources.read_text(f"scitacean._html_repr.{group}", filename)
+    return (
+        importlib.resources.files(f"scitacean._html_repr.{group}")
+        .joinpath(filename)
+        .read_text()
+    )
 
 
 def _preprocess_style(css: str) -> str:
     import re
 
     # line breaks are not needed
     css = css.replace("\n", "")
@@ -59,21 +54,27 @@
 
 @lru_cache(maxsize=1)
 def attachment_field_repr_template() -> Template:
     return Template(_read_text("attachment_field_repr.html.template", "templates"))
 
 
 @lru_cache(maxsize=1)
+def common_style() -> str:
+    sheet = _preprocess_style(_read_text("common.css", "styles"))
+    return f"<style>{sheet}</style>"
+
+
+@lru_cache(maxsize=1)
 def dataset_style() -> str:
     sheet = _preprocess_style(_read_text("dataset.css", "styles"))
-    return f"<style>{sheet}</style>"
+    return f"{common_style()}<style>{sheet}</style>"
 
 
 @lru_cache(maxsize=1)
 def attachment_style() -> str:
     sheet = _preprocess_style(_read_text("attachment.css", "styles"))
-    return f"<style>{sheet}</style>"
+    return f"{common_style()}<style>{sheet}</style>"
 
 
-@lru_cache()
+@lru_cache
 def image(name: str) -> str:
     return _read_text(name, "images")
```

### Comparing `scitacean-23.8.0/src/scitacean/_html_repr/images/lock.svg` & `scitacean-24.4.0/src/scitacean/_html_repr/images/lock.svg`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/src/scitacean/_html_repr/styles/attachment.css` & `scitacean-24.4.0/src/scitacean/_html_repr/styles/attachment.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 tr.cean-header {
-    border-bottom: 2px solid var(--jp-layout-color3);
+    border-bottom: 2px solid var(--cean-layout-color-border);
 }
 
 .jp-RenderedHTMLCommon tbody tr.cean-header:hover {
     /* disable hover color in table header */
-    background: var(--jp-layout-color0);
+    background: var(--cean-layout-color-background);
 }
 
 .cean-attachment .cean-info-line {
     /* match the margin of the tables */
     margin-left: 1em;
     font-weight: bold;
 }
@@ -38,39 +38,39 @@
 
 .cean-field-type {
     width: 12%;
     text-align: left !important;
 }
 
 td.cean-field-type {
-    color: var(--jp-content-font-color2);
+    color: var(--cean-font-color-field-type);
 }
 
 .cean-field-value {
     width: 39%;
     text-align: left !important;
 }
 
 .cean-field-description {
     width: 27%;
     text-align: left !important;
 }
 
 td.cean-field-description {
-    color: var(--jp-content-font-color1);
+    color: var(--cean-font-color-field-description);
 }
 
 .cean-field-value:hover span,
 .cean-field-description:hover span {
     white-space: normal;
     overflow: visible;
 }
 
 .cean-empty-field {
-    color: var(--jp-content-font-color2);
+    color: var(--cean-font-color-empty);
 }
 
 table.cean-attachment-table {
     /* space between details marker and table */
     margin-left: 1em !important;
     /* remove space between tables */
     margin-bottom: 0;
@@ -104,9 +104,9 @@
   max-width: 100%;
   height: auto;
 }
 
 .cean-lock path {
     /* Override the color used in the SVG.
        This requires there to be only a single fill color. */
-    fill: var(--jp-content-font-color2) !important;
+    fill: var(--cean-lock-fill) !important;
 }
```

### Comparing `scitacean-23.8.0/src/scitacean/_html_repr/templates/attachment_repr.html.template` & `scitacean-24.4.0/src/scitacean/_html_repr/templates/attachment_repr.html.template`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/src/scitacean/_html_repr/templates/dataset_repr.html.template` & `scitacean-24.4.0/src/scitacean/_html_repr/templates/dataset_repr.html.template`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/src/scitacean/_internal/dataclass_wrapper.py` & `scitacean-24.4.0/src/scitacean/_internal/dataclass_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Python version-independent dataclasses."""
 
 import dataclasses
-from typing import Any, Callable, Type, TypeVar
+from collections.abc import Callable
+from typing import Any, TypeVar
 
 T = TypeVar("T")
 
 
 try:
     from typing import dataclass_transform
 except ImportError:
-    from typing import Tuple, Union
-
     F = TypeVar("F")
 
     def dataclass_transform(
         *,
         eq_default: bool = True,
         order_default: bool = False,
         kw_only_default: bool = False,
         frozen_default: bool = False,
-        field_specifiers: Tuple[Union[Type[Any], Callable[..., Any]], ...] = (),
+        field_specifiers: tuple[type[Any] | Callable[..., Any], ...] = (),
         **kwargs: Any,
     ) -> Callable[[T], T]:
         def impl(f: F) -> F:
             return f
 
         return impl
 
 
 @dataclass_transform()
 def dataclass_optional_args(
     kw_only: bool = False, slots: bool = False, **kwargs: Any
-) -> Callable[[Type[T]], Type[T]]:
+) -> Callable[[type[T]], type[T]]:
     """Create a dataclass with modern arguments."""
     try:
         # Python 3.10+
         return dataclasses.dataclass(kw_only=kw_only, slots=slots, **kwargs)
     except TypeError:
         # Fallback for older Python
         return dataclasses.dataclass(**kwargs)
```

### Comparing `scitacean-23.8.0/src/scitacean/_internal/docker.py` & `scitacean-24.4.0/src/scitacean/_internal/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # ruff: noqa: S603, S607
 """Helpers to manage docker containers.
 
 Primarily meant for testing.
 """
+
 import json
 import os
 import subprocess
-from typing import Any, Union
+from typing import Any
 
-_PathLike = Union[str, os.PathLike]
+_PathLike = str | os.PathLike[str]
 
 
 def docker_compose_up(config_file: _PathLike, *services: str) -> None:
     subprocess.check_call(
         [
             "docker",
             "compose",
```

### Comparing `scitacean-23.8.0/src/scitacean/_internal/file_counter.py` & `scitacean-24.4.0/src/scitacean/_internal/file_counter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
+from collections.abc import Generator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Generator
 
 import filelock
 
 
 class FileCounter:
     """Atomic counter based on a file.
 
@@ -57,15 +57,15 @@
             if count == 0:
                 self._path.unlink()
             else:
                 self._write(count)
             yield count
 
     def _read(self) -> int:
-        with open(self._path, "r") as f:
+        with open(self._path) as f:
             c = int(f.read())
             return c
 
     def _write(self, count: int) -> None:
         with open(self._path, "w") as f:
             f.write(str(count))
```

### Comparing `scitacean-23.8.0/src/scitacean/_internal/orcid.py` & `scitacean-24.4.0/src/scitacean/_internal/orcid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 """Validator for ORCIDs.
 
 Based on
 https://support.orcid.org/hc/en-us/articles/360006897674-Structure-of-the-ORCID-Identifier
 """
```

### Comparing `scitacean-23.8.0/src/scitacean/client.py` & `scitacean-24.4.0/src/scitacean/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Client to handle communication with SciCat servers."""
 
 from __future__ import annotations
 
 import dataclasses
 import datetime
 import re
 import warnings
+from collections.abc import Callable, Iterable, Iterator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
+from typing import Any
 from urllib.parse import quote_plus
 
 import requests
 
 from . import model
 from ._base_model import convert_download_to_user_model
 from .dataset import Dataset
 from .error import ScicatCommError, ScicatLoginError
 from .file import File
+from .filesystem import RemotePath
 from .logging import get_logger
 from .pid import PID
 from .typing import DownloadConnection, FileTransfer, UploadConnection
-from .util.credentials import SecretStr, StrStorage
+from .util.credentials import ExpiringToken, SecretStr, StrStorage
 
 
 class Client:
     """SciCat client to communicate with a server.
 
     Clients hold all information needed to communicate with a SciCat instance
     and a filesystem that holds data files (via ``file_transfer``).
@@ -40,31 +42,31 @@
     and `Uploading Datasets <../../user-guide/uploading.ipynb>`_.
     """
 
     def __init__(
         self,
         *,
         client: ScicatClient,
-        file_transfer: Optional[FileTransfer],
+        file_transfer: FileTransfer | None,
     ):
         """Initialize a client.
 
         Do not use directly, instead use :func:`Client.from_token`
         or :func:`Client.from_credentials`!
         """
         self._client = client
         self._file_transfer = file_transfer
 
     @classmethod
     def from_token(
         cls,
         *,
         url: str,
-        token: Union[str, StrStorage],
-        file_transfer: Optional[FileTransfer] = None,
+        token: str | StrStorage,
+        file_transfer: FileTransfer | None = None,
     ) -> Client:
         """Create a new client and authenticate with a token.
 
         Parameters
         ----------
         url:
             URL of the SciCat api.
@@ -85,17 +87,17 @@
 
     # TODO rename to login? and provide logout?
     @classmethod
     def from_credentials(
         cls,
         *,
         url: str,
-        username: Union[str, StrStorage],
-        password: Union[str, StrStorage],
-        file_transfer: Optional[FileTransfer] = None,
+        username: str | StrStorage,
+        password: str | StrStorage,
+        file_transfer: FileTransfer | None = None,
     ) -> Client:
         """Create a new client and authenticate with username and password.
 
         Parameters
         ----------
         url:
             URL of the SciCat api.
@@ -117,15 +119,15 @@
                 url=url, username=username, password=password
             ),
             file_transfer=file_transfer,
         )
 
     @classmethod
     def without_login(
-        cls, *, url: str, file_transfer: Optional[FileTransfer] = None
+        cls, *, url: str, file_transfer: FileTransfer | None = None
     ) -> Client:
         """Create a new client without authentication.
 
         The client can only download public datasets and not upload at all.
 
         Parameters
         ----------
@@ -149,21 +151,21 @@
         """Low-level client for SciCat.
 
         Should typically not be used by users of Scitacean!
         """
         return self._client
 
     @property
-    def file_transfer(self) -> Optional[FileTransfer]:
+    def file_transfer(self) -> FileTransfer | None:
         """Stored handler for file down-/uploads."""
         return self._file_transfer
 
     def get_dataset(
         self,
-        pid: Union[str, PID],
+        pid: str | PID,
         strict_validation: bool = False,
         attachments: bool = False,
     ) -> Dataset:
         """Download a dataset from SciCat.
 
         Does not download any files.
 
@@ -208,21 +210,46 @@
 
         return Dataset.from_download_models(
             dataset_model=dataset,
             orig_datablock_models=orig_datablocks or [],
             attachment_models=attachment_models,
         )
 
+    def get_sample(
+        self,
+        sample_id: str,
+        strict_validation: bool = False,
+    ) -> model.Sample:
+        """Download a sample from SciCat.
+
+        Parameters
+        ----------
+        sample_id:
+            ID of the sample.
+        strict_validation:
+            If ``True``, the sample must pass validation.
+            If ``False``, a sample is still returned if validation fails.
+            Note that some sample fields may have a bad value or type.
+            A warning will be logged if validation fails.
+
+        Returns
+        -------
+        :
+            The downloaded sample.
+        """
+        sample_model = self.scicat.get_sample_model(
+            sample_id, strict_validation=strict_validation
+        )
+        return model.Sample.from_download_model(sample_model)
+
     def upload_new_dataset_now(self, dataset: Dataset) -> Dataset:
         """Upload a dataset as a new entry to SciCat immediately.
 
         The dataset is inserted as a new entry in the database and will
         never overwrite existing data.
-        To this end, the input dataset's ID is ignored and a new one is
-        assigned automatically.
 
         Attachments are also uploaded automatically.
         This happens after the upload of files and the dataset itself.
         So if uploading the attachments fails, check the dataset in SciCat to
         determine which attachments you need to re-upload
         (using :meth:`ScicatClient.create_attachment_for_dataset`).
 
@@ -242,23 +269,21 @@
         scitacean.ScicatCommError
             If the upload to SciCat fails.
         RuntimeError
             If the file upload fails or if a critical error is encountered
             and some files or a partial dataset are left on the servers.
             Note the error message if that happens.
         """
-        dataset = dataset.replace(
-            source_folder=self._expect_file_transfer().source_folder_for(dataset)
-        )
-        dataset.validate()
-        # TODO skip if there are no files
-        with self._connect_for_file_upload(dataset) as con:
+        dataset = dataset.replace(source_folder=self._source_folder_for(dataset))
+        files_to_upload = _files_to_upload(dataset.files)
+        self.scicat.validate_dataset_model(dataset.make_upload_model())
+        with self._connect_for_file_upload(dataset, files_to_upload) as con:
             # TODO check if any remote file is out of date.
             #  if so, raise an error. We never overwrite remote files!
-            uploaded_files = con.upload_files(*dataset.files)
+            uploaded_files = con.upload_files(*files_to_upload)
             dataset = dataset.replace_files(*uploaded_files)
             try:
                 finalized_model = self.scicat.create_dataset_model(
                     dataset.make_upload_model()
                 )
             except ScicatCommError:
                 con.revert_upload(*uploaded_files)
@@ -275,17 +300,45 @@
 
         return Dataset.from_download_models(
             dataset_model=finalized_model,
             orig_datablock_models=finalized_orig_datablocks,
             attachment_models=finalized_attachments,
         )
 
+    def upload_new_sample_now(self, sample: model.Sample) -> model.Sample:
+        """Upload a sample as a new entry to SciCat immediately.
+
+        The sample is inserted as a new entry in the database and will
+        never overwrite existing data.
+        To this end, the input sample's ID is ignored and a new one is
+        assigned automatically.
+
+        Parameters
+        ----------
+        sample:
+            The sample to upload.
+
+        Returns
+        -------
+        :
+            A copy of the input sample with fields adjusted
+            according to the response of the server.
+
+        Raises
+        ------
+        scitacean.ScicatCommError
+            If the upload to SciCat fails.
+        """
+        sample = dataclasses.replace(sample, sample_id=None)
+        finalized_model = self.scicat.create_sample_model(sample.make_upload_model())
+        return model.Sample.from_download_model(finalized_model)
+
     def _upload_orig_datablocks(
-        self, orig_datablocks: Optional[List[model.UploadOrigDatablock]]
-    ) -> List[model.DownloadOrigDatablock]:
+        self, orig_datablocks: list[model.UploadOrigDatablock] | None
+    ) -> list[model.DownloadOrigDatablock]:
         if not orig_datablocks:
             return []
 
         try:
             return [
                 self.scicat.create_orig_datablock(orig_datablock)
                 for orig_datablock in orig_datablocks
@@ -295,16 +348,16 @@
                 "Failed to upload original datablocks for SciCat dataset "
                 f"{orig_datablocks[0].datasetId}:"
                 f"\n{exc.args}\nThe dataset and data files were successfully uploaded "
                 "but are not linked with each other. Please fix the dataset manually!"
             ) from exc
 
     def _upload_attachments_for_dataset(
-        self, attachments: List[model.UploadAttachment], *, dataset_id: PID
-    ) -> List[model.DownloadAttachment]:
+        self, attachments: list[model.UploadAttachment], *, dataset_id: PID
+    ) -> list[model.DownloadAttachment]:
         try:
             return [
                 self.scicat.create_attachment_for_dataset(
                     attachment, dataset_id=dataset_id
                 )
                 for attachment in attachments
             ]
@@ -312,33 +365,48 @@
             raise RuntimeError(
                 f"Failed to upload attachments for SciCat dataset {dataset_id}:"
                 f"\n{exc.args}\nThe dataset and data files were successfully uploaded "
                 "and will not be reverted. Please upload the attachments manually!"
             ) from exc
 
     @contextmanager
-    def _connect_for_file_upload(self, dataset: Dataset) -> Iterator[UploadConnection]:
-        with self._expect_file_transfer().connect_for_upload(dataset) as con:
-            yield con
+    def _connect_for_file_upload(
+        self, dataset: Dataset, files_to_upload: Iterable[File]
+    ) -> Iterator[UploadConnection]:
+        if not files_to_upload:
+            yield _NullUploadConnection()
+        else:
+            with self._expect_file_transfer().connect_for_upload(dataset) as con:
+                yield con
+
+    def _source_folder_for(self, dataset: Dataset) -> RemotePath:
+        if self._file_transfer is not None:
+            return self._file_transfer.source_folder_for(dataset)
+        if dataset.source_folder is None:
+            raise ValueError(
+                "Cannot determine source_folder for dataset because "
+                "the dataset's source_folder is None and there is no file transfer."
+            )
+        return dataset.source_folder
 
     def _expect_file_transfer(self) -> FileTransfer:
         if self.file_transfer is None:
             raise ValueError(
                 "Cannot upload/download files because no file transfer is set. "
                 "Specify one when constructing a client."
             )
         return self.file_transfer
 
     def download_files(
         self,
         dataset: Dataset,
         *,
-        target: Union[str, Path],
+        target: str | Path,
         select: FileSelector = True,
-        checksum_algorithm: Optional[str] = None,
+        checksum_algorithm: str | None = None,
         force: bool = False,
     ) -> Dataset:
         r"""Download files of a dataset.
 
         Makes selected files available on the local filesystem using the file transfer
         object stored in the client.
 
@@ -487,30 +555,32 @@
 
 class ScicatClient:
     """Low-level client to call the SciCat API."""
 
     def __init__(
         self,
         url: str,
-        token: Optional[Union[str, StrStorage]],
-        timeout: Optional[datetime.timedelta],
+        token: str | StrStorage | None,
+        timeout: datetime.timedelta | None,
     ):
         # Need to add a final /
         self._base_url = url[:-1] if url.endswith("/") else url
         self._timeout = datetime.timedelta(seconds=10) if timeout is None else timeout
-        self._token: Optional[StrStorage] = (
-            SecretStr(token) if isinstance(token, str) else token
+        self._token: StrStorage | None = (
+            ExpiringToken.from_jwt(SecretStr(token))
+            if isinstance(token, str)
+            else token
         )
 
     @classmethod
     def from_token(
         cls,
         url: str,
-        token: Union[str, StrStorage],
-        timeout: Optional[datetime.timedelta] = None,
+        token: str | StrStorage,
+        timeout: datetime.timedelta | None = None,
     ) -> ScicatClient:
         """Create a new low-level client and authenticate with a token.
 
         Parameters
         ----------
         url:
             URL of the SciCat api.
@@ -526,17 +596,17 @@
         """
         return ScicatClient(url=url, token=token, timeout=timeout)
 
     @classmethod
     def from_credentials(
         cls,
         url: str,
-        username: Union[str, StrStorage],
-        password: Union[str, StrStorage],
-        timeout: Optional[datetime.timedelta] = None,
+        username: str | StrStorage,
+        password: str | StrStorage,
+        timeout: datetime.timedelta | None = None,
     ) -> ScicatClient:
         """Create a new low-level client and authenticate with username and password.
 
         Parameters
         ----------
         url:
             URL of the SciCat api.
@@ -568,15 +638,15 @@
                 )
             ),
             timeout=timeout,
         )
 
     @classmethod
     def without_login(
-        cls, url: str, timeout: Optional[datetime.timedelta] = None
+        cls, url: str, timeout: datetime.timedelta | None = None
     ) -> ScicatClient:
         """Create a new low-level client without authentication.
 
         The client can only download public datasets and not upload at all.
 
         Parameters
         ----------
@@ -633,15 +703,15 @@
             model.DownloadDataset,
             _strict_validation=strict_validation,
             **dset_json,
         )
 
     def get_orig_datablocks(
         self, pid: PID, strict_validation: bool = False
-    ) -> List[model.DownloadOrigDatablock]:
+    ) -> list[model.DownloadOrigDatablock]:
         """Fetch all orig datablocks from SciCat for a given dataset.
 
         Parameters
         ----------
         pid:
             Unique ID of the *dataset*.
             Must include the facility ID.
@@ -669,15 +739,15 @@
         return [
             _make_orig_datablock(dblock, strict_validation=strict_validation)
             for dblock in dblock_json
         ]
 
     def get_attachments_for_dataset(
         self, pid: PID, strict_validation: bool = False
-    ) -> List[model.DownloadAttachment]:
+    ) -> list[model.DownloadAttachment]:
         """Fetch all attachments from SciCat for a given dataset.
 
         Parameters
         ----------
         pid:
             Unique ID of the *dataset*.
             Must include the facility ID.
@@ -707,16 +777,57 @@
                 model.DownloadAttachment,
                 _strict_validation=strict_validation,
                 **attachment,
             )
             for attachment in attachment_json
         ]
 
+    def get_sample_model(
+        self, sample_id: str, strict_validation: bool = False
+    ) -> model.DownloadSample:
+        """Fetch a sample from SciCat.
+
+        Parameters
+        ----------
+        sample_id:
+            ID of the sample to fetch.
+        strict_validation:
+            If ``True``, the sample must pass validation.
+            If ``False``, a sample is still returned if validation fails.
+            Note that some fields may have a bad value or type.
+            A warning will be logged if validation fails.
+
+        Returns
+        -------
+        :
+            A model of the sample.
+
+        Raises
+        ------
+        scitacean.ScicatCommError
+            If the sample does not exist or communication fails for some other reason.
+        """
+        sample_json = self._call_endpoint(
+            cmd="get",
+            url=f"samples/{quote_plus(sample_id)}",
+            operation="get_sample_model",
+        )
+        if not sample_json:
+            raise ScicatCommError(
+                f"Cannot get sample with {sample_id=}, "
+                f"no such sample in SciCat at {self._base_url}."
+            )
+        return model.construct(
+            model.DownloadSample,
+            _strict_validation=strict_validation,
+            **sample_json,
+        )
+
     def create_dataset_model(
-        self, dset: Union[model.UploadDerivedDataset, model.UploadRawDataset]
+        self, dset: model.UploadDerivedDataset | model.UploadRawDataset
     ) -> model.DownloadDataset:
         """Create a new dataset in SciCat.
 
         The dataset PID must be either
 
         - ``None``, in which case SciCat assigns an ID,
         - an unused id, in which case SciCat uses it for the new dataset.
@@ -825,37 +936,95 @@
                 "The server reported success but did not return a finalized attachment."
                 " This likely means that there is no dataset with this ID."
             )
         return model.construct(
             model.DownloadAttachment, _strict_validation=False, **uploaded
         )
 
+    def create_sample_model(self, sample: model.UploadSample) -> model.DownloadSample:
+        """Create a new sample in SciCat.
+
+        The sample ID must be either
+
+        - ``None``, in which case SciCat assigns an ID,
+        - an unused id, in which case SciCat uses it for the new sample.
+
+        If the ID already exists, creation will fail without
+        modification to the database.
+        Unless the new sample is identical to the existing one,
+        in which case, nothing happens.
+
+        Parameters
+        ----------
+        sample:
+            Model of the sample to create.
+
+        Returns
+        -------
+        :
+            The uploaded sample as returned by SciCat.
+            This is the input plus some modifications.
+
+        Raises
+        ------
+        scitacean.ScicatCommError
+            If SciCat refuses the sample or communication
+            fails for some other reason.
+        """
+        uploaded = self._call_endpoint(
+            cmd="post", url="samples", data=sample, operation="create_sample_model"
+        )
+        return model.construct(
+            model.DownloadSample, _strict_validation=False, **uploaded
+        )
+
+    def validate_dataset_model(
+        self, dset: model.UploadDerivedDataset | model.UploadRawDataset
+    ) -> None:
+        """Validate a dataset in SciCat.
+
+        Parameters
+        ----------
+        dset:
+            Model of the dataset to validate.
+
+        Raises
+        ------
+        ValueError
+            If the dataset does not pass validation.
+        """
+        response = self._call_endpoint(
+            cmd="post",
+            url="datasets/isValid",
+            data=dset,
+            operation="validate_dataset_model",
+        )
+        if not response["valid"]:
+            raise ValueError(f"Dataset {dset} did not pass validation in SciCat.")
+
     def _send_to_scicat(
-        self, *, cmd: str, url: str, data: Optional[model.BaseModel] = None
+        self, *, cmd: str, url: str, data: model.BaseModel | None = None
     ) -> requests.Response:
         if self._token is not None:
             token = self._token.get_str()
-            params = {"access_token": token}
             headers = {"Authorization": f"Bearer {token}"}
         else:
             token = ""
-            params = {}
             headers = {}
 
         if data is not None:
             headers["Content-Type"] = "application/json"
 
         try:
             return requests.request(
                 method=cmd,
                 url=url,
                 data=data.model_dump_json(exclude_none=True)
                 if data is not None
                 else None,
-                params=params,
                 headers=headers,
                 timeout=self._timeout.seconds,
                 stream=False,
                 verify=True,
             )
         except Exception as exc:
             # Remove concrete request function call from backtrace to hide the token.
@@ -868,15 +1037,15 @@
             ) from None
 
     def _call_endpoint(
         self,
         *,
         cmd: str,
         url: str,
-        data: Optional[model.BaseModel] = None,
+        data: model.BaseModel | None = None,
         operation: str,
     ) -> Any:
         full_url = _url_concat(self._base_url, url)
         logger = get_logger()
         logger.info("Calling SciCat API at %s for operation '%s'", full_url, operation)
 
         response = self._send_to_scicat(cmd=cmd, url=full_url, data=data)
@@ -910,15 +1079,15 @@
     err = re.sub(r"token=[\w\-./]+", "token=<HIDDEN>", err)
     if token:  # token can be ""
         err = err.replace(token, "<HIDDEN>")
     return err
 
 
 def _make_orig_datablock(
-    fields: Dict[str, Any], strict_validation: bool
+    fields: dict[str, Any], strict_validation: bool
 ) -> model.DownloadOrigDatablock:
     files = [
         model.construct(
             model.DownloadDataFile, _strict_validation=strict_validation, **file_fields
         )
         for file_fields in fields["dataFileList"]
     ]
@@ -938,15 +1107,15 @@
         json={"username": username.get_str(), "password": password.get_str()},
         stream=False,
         verify=True,
         timeout=timeout.seconds,
     )
     if not response.ok:
         get_logger().info(
-            "Failed to log in via endpoint Users/login: %s", response.json()["error"]
+            "Failed to log in via endpoint Users/login: %s", response.text
         )
     return response
 
 
 def _log_in_via_auth_msad(
     url: str, username: StrStorage, password: StrStorage, timeout: datetime.timedelta
 ) -> requests.Response:
@@ -959,17 +1128,15 @@
         _url_concat(base_url, "auth/msad"),
         json={"username": username.get_str(), "password": password.get_str()},
         stream=False,
         verify=True,
         timeout=timeout.seconds,
     )
     if not response.ok:
-        get_logger().error(
-            "Failed to log in via auth/msad: %s", response.json()["error"]
-        )
+        get_logger().error("Failed to log in via auth/msad: %s", response.text)
     return response
 
 
 def _get_token(
     url: str, username: StrStorage, password: StrStorage, timeout: datetime.timedelta
 ) -> str:
     """Log in using the provided username + password.
@@ -989,52 +1156,80 @@
 
     response = _log_in_via_auth_msad(
         url=url, username=username, password=password, timeout=timeout
     )
     if response.ok:
         return str(response.json()["access_token"])
 
-    get_logger().error("Failed log in:  %s", response.json()["error"])
+    get_logger().error("Failed log in:  %s", response.text)
     raise ScicatLoginError(response.content)
 
 
-FileSelector = Union[
-    bool, str, List[str], Tuple[str], re.Pattern, Callable[[File], bool]
-]
+FileSelector = (
+    bool | str | list[str] | tuple[str] | re.Pattern[str] | Callable[[File], bool]
+)
 
 
 def _file_selector(select: FileSelector) -> Callable[[File], bool]:
     if select is True:
         return lambda _: True
     if select is False:
         return lambda _: False
     if isinstance(select, str):
         return lambda f: f.remote_path == select
     if isinstance(select, (list, tuple)):
-        return lambda f: f.remote_path in select  # type: ignore[operator]
+        return lambda f: f.remote_path in select
     if isinstance(select, re.Pattern):
-        return lambda f: (
-            select.search(f.remote_path.posix) is not None  # type: ignore[union-attr]
-        )
+        return lambda f: (select.search(f.remote_path.posix) is not None)
     return select
 
 
-def _select_files(select: FileSelector, dataset: Dataset) -> List[File]:
+def _select_files(select: FileSelector, dataset: Dataset) -> list[File]:
     selector = _file_selector(select)
     return [f for f in dataset.files if selector(f)]
 
 
 def _remove_up_to_date_local_files(
-    files: List[File], checksum_algorithm: Optional[str]
-) -> List[File]:
+    files: list[File], checksum_algorithm: str | None
+) -> list[File]:
     def is_up_to_date(file: File) -> bool:
         if checksum_algorithm is not None:
             file = dataclasses.replace(file, checksum_algorithm=checksum_algorithm)
         return file.local_is_up_to_date()
 
     return [
         file
         for file in files
         if not (
             file.local_path.exists() and is_up_to_date(file)  # type: ignore[union-attr]
         )
     ]
+
+
+def _files_to_upload(files: Iterable[File]) -> list[File]:
+    for file in files:
+        if file.is_on_local and file.is_on_remote:
+            raise ValueError(
+                f"Refusing to upload file at remote_path={file.remote_path} "
+                "because it is both on local and remote and it is unclear what "
+                "to do. If you want to perform the upload, set the local path to None."
+            )
+    return [file for file in files if file.local_path is not None]
+
+
+class _NullUploadConnection:
+    """File-upload connection that does not upload anything.
+
+    Raises if called with files because uit should only be used by Client
+    when there are no files to upload.
+    """
+
+    def upload_files(self, *files: File) -> list[File]:
+        """Raise if given files."""
+        if files:
+            raise RuntimeError("Internal error: Bad upload connection")
+        return []
+
+    def revert_upload(self, *files: File) -> None:
+        """Raise if given files."""
+        if files:
+            raise RuntimeError("Internal error: Bad upload connection")
```

### Comparing `scitacean-23.8.0/src/scitacean/datablock.py` & `scitacean-24.4.0/src/scitacean/datablock.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 """Wrappers for (Orig)Datablocks."""
 
 from __future__ import annotations
 
 import dataclasses
+from collections.abc import Iterable, Iterator
 from datetime import datetime
-from typing import TYPE_CHECKING, Iterable, Iterator, List, Optional
+from typing import TYPE_CHECKING
 
 from .file import File
 from .model import DownloadOrigDatablock, UploadOrigDatablock
 from .pid import PID
 
 if TYPE_CHECKING:
     from .dataset import Dataset
@@ -25,28 +26,29 @@
 
     Instances of this class are mutable as opposed to
     :class:`scitacean.model.OrigDatablock`.
     They are used for building datasets and get converted to/from pydantic
     models for communication with a server.
     """
 
-    _files: List[File] = dataclasses.field(init=False)
-    checksum_algorithm: Optional[str] = None
-    access_groups: Optional[List[str]] = None
-    instrument_group: Optional[str] = None
-    owner_group: Optional[str] = None
-    init_files: dataclasses.InitVar[Optional[Iterable[File]]] = None
-    _created_at: Optional[datetime] = None
-    _created_by: Optional[str] = None
-    _dataset_id: Optional[PID] = None
-    _id: Optional[str] = None
-    _updated_at: Optional[datetime] = None
-    _updated_by: Optional[str] = None
+    _files: list[File] = dataclasses.field(init=False)
+    checksum_algorithm: str | None = None
+    instrument_group: str | None = None
+    owner_group: str | None = None
+    init_files: dataclasses.InitVar[Iterable[File] | None] = None
+    _access_groups: list[str] | None = None
+    _created_at: datetime | None = None
+    _created_by: str | None = None
+    _dataset_id: PID | None = None
+    _id: str | None = None
+    _is_published: bool | None = None
+    _updated_at: datetime | None = None
+    _updated_by: str | None = None
 
-    def __post_init__(self, init_files: Optional[Iterable[File]]) -> None:
+    def __post_init__(self, init_files: Iterable[File] | None) -> None:
         self._files = list(init_files) if init_files is not None else []
 
     @classmethod
     def from_download_model(
         cls,
         orig_datablock_model: DownloadOrigDatablock,
     ) -> OrigDatablock:
@@ -62,20 +64,21 @@
         :
             A new instance.
         """
         dblock = orig_datablock_model
         return OrigDatablock(
             checksum_algorithm=dblock.chkAlg,
             owner_group=dblock.ownerGroup,
-            access_groups=dblock.accessGroups,
             instrument_group=dblock.instrumentGroup,
+            _access_groups=dblock.accessGroups,
             _created_at=dblock.createdAt,
             _created_by=dblock.createdBy,
             _dataset_id=orig_datablock_model.datasetId,
             _id=orig_datablock_model.id,
+            _is_published=orig_datablock_model.isPublished,
             _updated_at=dblock.updatedAt,
             _updated_by=dblock.updatedBy,
             init_files=[
                 File.from_download_model(file, checksum_algorithm=dblock.chkAlg)
                 for file in dblock.dataFileList or ()
             ],
         )
@@ -87,43 +90,53 @@
 
     @property
     def size(self) -> int:
         """Total size of all files."""
         return sum(file.size for file in self.files)
 
     @property
-    def created_at(self) -> Optional[datetime]:
+    def access_groups(self) -> list[str] | None:
+        """Access groups for this datablock."""
+        return self._access_groups
+
+    @property
+    def created_at(self) -> datetime | None:
         """Creation time of this orig datablock."""
         return self._created_at
 
     @property
-    def created_by(self) -> Optional[str]:
+    def created_by(self) -> str | None:
         """User who created this orig datablock."""
         return self._created_by
 
     @property
-    def updated_at(self) -> Optional[datetime]:
+    def updated_at(self) -> datetime | None:
         """Last update time of this orig datablock."""
         return self._updated_at
 
     @property
-    def updated_by(self) -> Optional[str]:
+    def updated_by(self) -> str | None:
         """User who last updated this datablock."""
         return self._updated_by
 
     @property
-    def dataset_id(self) -> Optional[PID]:
+    def dataset_id(self) -> PID | None:
         """PID of the dataset this datablock belongs to."""
         return self._dataset_id
 
     @property
-    def datablock_id(self) -> Optional[str]:
+    def datablock_id(self) -> str | None:
         """ID of this datablock."""
         return self._id
 
+    @property
+    def is_published(self) -> bool | None:
+        """Return whether the datablock is public on SciCat."""
+        return self._is_published
+
     def add_files(self, *files: File) -> None:
         """Append files to the datablock.
 
         Parameters
         ----------
         files:
             File objects to add.
@@ -148,11 +161,11 @@
         """
         owner_group = self.owner_group or dataset.owner_group
         return UploadOrigDatablock(
             chkAlg=self.checksum_algorithm,
             size=self.size,
             dataFileList=[file.make_model(for_archive=False) for file in self.files],
             datasetId=dataset.pid,  # type: ignore[arg-type]
-            ownerGroup=owner_group,  # type: ignore[arg-type]
+            ownerGroup=owner_group,
             accessGroups=self.access_groups or dataset.access_groups,
             instrumentGroup=self.instrument_group or dataset.instrument_group,
         )
```

### Comparing `scitacean-23.8.0/src/scitacean/dataset.py` & `scitacean-24.4.0/src/scitacean/testing/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,516 +1,429 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
-"""Main dataset structure."""
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
+"""Fake client for testing."""
 
 from __future__ import annotations
 
-import dataclasses
-import itertools
-from datetime import datetime, timezone
-from pathlib import Path
-from typing import (
-    Any,
-    Dict,
-    Generator,
-    Iterable,
-    List,
-    Literal,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-)
-
-from ._base_model import convert_download_to_user_model, convert_user_to_upload_model
-from ._dataset_fields import DatasetBase
-from .datablock import OrigDatablock
-from .file import File
-from .model import (
-    Attachment,
-    DatasetType,
-    DownloadAttachment,
-    DownloadDataset,
-    DownloadOrigDatablock,
-    UploadAttachment,
-    UploadDerivedDataset,
-    UploadOrigDatablock,
-    UploadRawDataset,
-)
-from .pid import PID
+import datetime
+import functools
+import uuid
+from collections.abc import Callable
+from copy import deepcopy
+from typing import Any
+
+from .. import model
+from ..client import Client, ScicatClient
+from ..error import ScicatCommError
+from ..pid import PID
+from ..typing import FileTransfer
+from ..util.credentials import StrStorage
+
+
+def _conditionally_disabled(func: Callable[..., Any]) -> Callable[..., Any]:
+    @functools.wraps(func)
+    def impl(self, *args, **kwargs):  # type: ignore[no-untyped-def]
+        if (exc := self.main.disabled.get(func.__name__)) is not None:
+            raise exc
+        return func(self, *args, **kwargs)
+
+    return impl
+
+
+# Inherits from Client to satisfy type hints.
+class FakeClient(Client):
+    """Mimics a client without accessing the internet.
+
+    This class is a stand in for :class:`scitacean.Client` to emulate downloading and
+    uploading of datasets without actually accessing a SciCat server.
+
+    Since this client fakes communication with SciCat, it stores raw
+    `pydantic <https://docs.pydantic.dev/>`_ models, namely
+
+    - ``FakeClient.datasets``:
+            :class:`dict` of :class:`scitacean.model.DownloadDataset`,
+            indexed by dataset PID.
+    - ``FakeClient.orig_datablocks``:
+            :class:`dict` of lists of :class:`scitacean.model.DownloadOrigDatablock`,
+            indexed by the *dataset* ID.
+    - ``FakeClient.attachments``:
+            :class:`dict` of lists of :class:`scitacean.model.DownloadAttachment`,
+            indexed by the *dataset* ID.
+
+    Individual functions can be disabled (that is, made to raise an exception)
+    using the ``disabled`` argument of the initializer.
+
+    Important
+    ---------
+    ``FakeClient`` does not behave exactly like a ``Client`` connected to a real
+    server as that would require reimplementing a large part of the SciCat backend.
+    You should thus always also test your code against a (potentially locally deployed)
+    real server.
+
+    In particular, do not rely on specific error messages or the detailed settings
+    in the datasets returned by ``FakeClient.upload_new_dataset_now``!
+
+    Examples
+    --------
+    Set up a fake client for download:
+
+    .. code-block:: python
+
+        client = FakeClient()
+        pid = PID(prefix="sample.prefix", pid="1234-5678-abcd")
+        client.datasets[pid] = model.DownloadDataset(pid=pid, ...)
+        client.orig_datablocks[pid] = [model.OrigDatablock(
+            datasetId=str(pid),
+            ...
+        )]
+        client.get_dataset(pid)
+
+    Upload a dataset:
+
+    .. code-block:: python
+
+        client = FakeClient(file_transfer=FakeFileTransfer())
+        finalized = client.upload_new_dataset_now(dset)
+
+        # contains new dataset and datablock:
+        client.datasets[finalized.pid]
+        client.orig_datablocks[finalized.pid]
+
+    Disable a method:
+
+    .. code-block:: python
+
+        client = FakeClient(
+            disable={"create_dataset_model": RuntimeError("Upload failed")})
+        # raises RuntimeError("Upload failed"):
+        client.upload_new_dataset_now(dset)
+
+    See Also
+    --------
+    scitacean.testing.transfer.FakeFileTransfer: Fake file up-/downloads
+        without a real server.
+    """
 
-
-class Dataset(DatasetBase):
-    @classmethod
-    def from_download_models(
-        cls,
-        dataset_model: DownloadDataset,
-        orig_datablock_models: List[DownloadOrigDatablock],
-        attachment_models: Optional[Iterable[DownloadAttachment]] = None,
-    ) -> Dataset:
-        """Construct a new dataset from SciCat download models.
-
-        Parameters
-        ----------
-        dataset_model:
-            Model of the dataset.
-        orig_datablock_models:
-            List of all associated original datablock models for the dataset.
-        attachment_models:
-            List of all associated attachment models for the dataset.
-            Use ``None`` if the attachments were not downloaded.
-            Use an empty list if the attachments were downloaded, but there aren't any.
-
-        Returns
-        -------
-        :
-            A new Dataset instance.
-        """
-        init_args, read_only = DatasetBase._prepare_fields_from_download(dataset_model)
-        dset = cls(**init_args)
-        for key, val in read_only.items():
-            setattr(dset, key, val)
-        dset._attachments = convert_download_to_user_model(  # type: ignore[assignment]
-            attachment_models
-        )
-        if orig_datablock_models is not None:
-            dset._orig_datablocks.extend(
-                map(OrigDatablock.from_download_model, orig_datablock_models)
-            )
-        return dset
-
-    @classmethod
-    def fields(
-        cls,
-        dataset_type: Optional[Union[DatasetType, Literal["derived", "raw"]]] = None,
-        read_only: Optional[bool] = None,
-    ) -> Generator[Dataset.Field, None, None]:
-        """Iterate over dataset fields.
-
-        This is similar to :func:`dataclasses.fields`.
-
-        Parameters
-        ----------
-        dataset_type:
-            If set, return only the fields for this dataset type.
-            If unset, do not filter fields.
-        read_only:
-            If true or false, return only fields which are read-only
-            or allow write-access, respectively.
-            If unset, do not filter fields.
-
-        Returns
-        -------
-        :
-            Iterable over the fields of datasets.
-        """
-        it = iter(DatasetBase._FIELD_SPEC)
-        if dataset_type is not None:
-            attr = (
-                "used_by_derived"
-                if dataset_type == DatasetType.DERIVED
-                else "used_by_raw"
-            )
-            it = filter(lambda field: getattr(field, attr), it)
-        if read_only is not None:
-            it = filter(lambda field: field.read_only == read_only, it)
-        yield from it
-
-    def __str__(self) -> str:
-        args = ", ".join(
-            f"{field.name}={value}"
-            for field in self.fields()
-            if (value := getattr(self, field.name)) is not None
-        )
-        return f"Dataset({args})"
-
-    def _repr_html_(self) -> str:
-        # Import here to prevent cycle.
-        from ._html_repr import dataset_html_repr
-
-        return dataset_html_repr(self)
-
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, Dataset):
-            return False
-        eq = all(
-            getattr(self, field.name) == getattr(other, field.name)
-            for field in Dataset.fields()
-        )
-        eq = (
-            eq
-            and self._orig_datablocks == other._orig_datablocks
-            and self._attachments == other._attachments
-        )
-        return eq
-
-    @property
-    def number_of_files(self) -> int:
-        """Number of files in directly accessible storage in the dataset.
-
-        This includes files on both the local and remote filesystems.
-
-        Corresponds to OrigDatablocks.
-        """
-        return sum(len(tuple(dblock.files)) for dblock in self._orig_datablocks)
-
-    @property
-    def number_of_files_archived(self) -> int:
-        """Total number of archived files in the dataset.
-
-        Corresponds to Datablocks.
-        """
-        return 0
-
-    @property
-    def packed_size(self) -> int:
-        """Total size of all datablock package files created for this dataset."""
-        return 0
-
-    @property
-    def size(self) -> int:
-        """Total size of files in directly accessible storage in the dataset.
-
-        This includes files on both the local and remote filesystems.
-
-        Corresponds to OrigDatablocks.
-        """
-        return sum(file.size for file in self.files)
-
-    @property
-    def files(self) -> Tuple[File, ...]:
-        """Files linked with the dataset."""
-        return tuple(
-            itertools.chain.from_iterable(
-                dblock.files for dblock in self._orig_datablocks
-            )
-        )
-
-    @property
-    def attachments(self) -> Optional[List[Attachment]]:
-        """List of attachments for this dataset.
-
-        This property can be in two distinct 'falsy' states:
-
-        - ``dset.attachments is None``: It is unknown whether there are attachments.
-          This happens when datasets are downloaded without downloading the attachments.
-        - ``dset.attachments == []``: It is known that there are no attachments.
-          This happens either when downloading datasets or when initializing datasets
-          locally without assigning attachments.
-        """
-        return self._attachments
-
-    @attachments.setter
-    def attachments(self, attachments: Optional[List[Attachment]]) -> None:
-        """List of attachments for this dataset.
-
-        See the docs of the getter for an explanation of ``None`` vs ``[]``.
-        It is unlikely that you ever need to set the attachments to ``None``.
-        """
-        self._attachments = attachments
-
-    def add_files(self, *files: File, datablock: Union[int, str, PID] = -1) -> None:
-        """Add files to the dataset."""
-        self._get_or_add_orig_datablock(datablock).add_files(*files)
-
-    def add_local_files(
+    def __init__(
         self,
-        *paths: Union[str, Path],
-        base_path: Union[str, Path] = "",
-        datablock: Union[int, str] = -1,
+        *,
+        file_transfer: FileTransfer | None = None,
+        disable: dict[str, Exception] | None = None,
     ) -> None:
-        """Add files on the local file system to the dataset.
+        """Initialize a fake client with empty dataset storage.
 
         Parameters
         ----------
-        paths:
-            Local paths to the files.
-        base_path:
-            The remote paths will be set up according to
-
-            ``remotes = [path.relative_to(base_path) for path in paths]``.
-        datablock:
-            Advanced feature, do not set unless you know what this is!
-
-            Select the orig datablock to store the file in.
-            If an ``int``, use the datablock with that index.
-            If a ``str`` or ``PID``, use the datablock with that id;
-            if there is none with matching id, raise ``KeyError``.
-        """
-        self.add_files(
-            *(File.from_local(path, base_path=base_path) for path in paths),
-            datablock=datablock,
-        )
+        file_transfer:
+            Typically :class:`scitacean.testing.transfer.FakeFileTransfer`
+            but may be a real file transfer.
+        disable:
+            ``dict`` of function names to exceptions.
+            Functions listed here raise the given exception
+            when called and do nothing else.
+        """
+        super().__init__(client=FakeScicatClient(self), file_transfer=file_transfer)
+
+        self.disabled = {} if disable is None else dict(disable)
+        self.datasets: dict[PID, model.DownloadDataset] = {}
+        self.orig_datablocks: dict[PID, list[model.DownloadOrigDatablock]] = {}
+        self.attachments: dict[PID, list[model.DownloadAttachment]] = {}
+        self.samples: dict[str, model.DownloadSample] = {}
 
-    def replace(
-        self,
+    @classmethod
+    def from_token(
+        cls,
         *,
-        _read_only: Optional[Dict[str, Any]] = None,
-        _orig_datablocks: Optional[List[OrigDatablock]] = None,
-        **replacements: Any,
-    ) -> Dataset:
-        """Return a new dataset with replaced fields.
-
-        Parameters starting with an underscore are for internal use.
-        Using them may result in a broken dataset.
-
-        Parameters
-        ----------
-        replacements:
-            New field values.
+        url: str,
+        token: str | StrStorage,
+        file_transfer: FileTransfer | None = None,
+    ) -> FakeClient:
+        """Create a new fake client.
 
-        Returns
-        -------
-        :
-            The new dataset has the same fields as the input but all fields given
-            as keyword arguments are replaced by the given values.
+        All arguments except ``file_Transfer`` are ignored.
         """
-        _read_only = _read_only or {}
-
-        def get_val(source: Dict[str, Any], name: str) -> Any:
-            try:
-                return source.pop(name)
-            except KeyError:
-                return getattr(self, name)
-
-        read_only = {
-            field.name: get_val(_read_only, field.name)
-            for field in Dataset.fields(read_only=True)
-        }
-        DatasetBase._convert_readonly_fields_in_place(read_only)
-        kwargs = {
-            **{
-                field.name: get_val(replacements, field.name)
-                for field in Dataset.fields(read_only=False)
-            },
-        }
-        attachments = get_val(replacements, "attachments")
-        if replacements or _read_only:
-            raise TypeError(
-                f"Invalid arguments: {', '.join((*replacements, *_read_only))}"
-            )
-        dset = Dataset(
-            **kwargs,
-        )
-        dset._orig_datablocks.extend(
-            _orig_datablocks if _orig_datablocks is not None else self._orig_datablocks
-        )
-        dset._attachments = list(attachments) if attachments is not None else None
-        for key, val in read_only.items():
-            setattr(dset, "_" + key, val)
-        return dset
-
-    def as_new(self) -> Dataset:
-        """Return a new dataset with lifecycle-related fields erased.
-
-        The returned dataset has the same fields as ``self``.
-        But fields that indicate when the dataset was created or
-        by who are set to ``None``.
-        This if, for example, ``created_at``, ``history``, and ``lifecycle``.
-
-        Returns
-        -------
-        :
-            A new dataset without lifecycle-related fields.
-        """
-        return self.replace(
-            _read_only={field.name: None for field in Dataset.fields(read_only=True)},
-            creation_time=datetime.now(tz=timezone.utc),
-        )
+        return FakeClient(file_transfer=file_transfer)
 
-    def derive(
-        self,
+    @classmethod
+    def from_credentials(
+        cls,
         *,
-        keep: Iterable[str] = (
-            "contact_email",
-            "investigator",
-            "orcid_of_owner",
-            "owner",
-            "owner_email",
-            "techniques",
-        ),
-    ) -> Dataset:
-        """Return a new dataset that is derived from self.
-
-        The returned dataset has most fields set to ``None``.
-        But a number of fields can be carried over from ``self``.
-        By default, this assumes that the owner of the derived dataset is the same
-        as the owner of the original.
-        This can be customized with the ``keep`` argument.
-
-        Parameters
-        ----------
-        keep:
-            Fields to copy over to the derived dataset.
+        url: str,
+        username: str | StrStorage,
+        password: str | StrStorage,
+        file_transfer: FileTransfer | None = None,
+    ) -> FakeClient:
+        """Create a new fake client.
 
-        Returns
-        -------
-        :
-            A new derived dataset.
-
-        Raises
-        ------
-        ValueError
-            If ``self`` has no PID.
-            The derived dataset requires a PID in order to link back to ``self``.
+        All arguments except ``file_Transfer`` are ignored.
         """
-        if self.pid is None:
-            raise ValueError("Cannot make a derived datasets because self.pid is None.")
-        return Dataset(
-            type=DatasetType.DERIVED,
-            input_datasets=[self.pid],
-            creation_time=datetime.now(tz=timezone.utc),
-            **{name: getattr(self, name) for name in keep},
-        )
-
-    def replace_files(self, *files: File) -> Dataset:
-        """Return a new dataset with replaced files.
-
-        For each argument, if the input dataset has a file with the
-        same remote path, that file is replaced.
-        Otherwise, a new file is added.
-        Other existing files are kept in the returned dataset.
+        return FakeClient(file_transfer=file_transfer)
 
-        Parameters
-        ----------
-        files:
-            New files for the dataset.
+    @classmethod
+    def without_login(
+        cls, *, url: str, file_transfer: FileTransfer | None = None
+    ) -> FakeClient:
+        """Create a new fake client.
 
-        Returns
-        -------
-        :
-            A new dataset with given files.
+        All arguments except ``file_Transfer`` are ignored.
         """
+        return FakeClient(file_transfer=file_transfer)
 
-        def new_or_old(old: File) -> File:
-            for new in files:
-                if old.remote_path == new.remote_path:
-                    return new
-            return old
-
-        return self.replace(
-            _orig_datablocks=[
-                dataclasses.replace(dblock, init_files=map(new_or_old, dblock.files))
-                for dblock in self._orig_datablocks
-            ]
-        )
 
-    def add_orig_datablock(self, *, checksum_algorithm: Optional[str]) -> OrigDatablock:
-        """Append a new orig datablock to the list of orig datablocks.
+class FakeScicatClient(ScicatClient):
+    """Mimics a ScicatClient, to be used by FakeClient."""
 
-        Parameters
-        ----------
-        checksum_algorithm:
-            Use this algorithm to compute checksums of files
-            associated with this datablock.
-
-        Returns
-        -------
-        :
-            The newly added datablock.
-        """
-        dblock = OrigDatablock(
-            checksum_algorithm=checksum_algorithm, _dataset_id=self.pid
-        )
-        self._orig_datablocks.append(dblock)
-        return dblock
+    def __init__(self, main_client: FakeClient) -> None:
+        super().__init__(url="", token="", timeout=datetime.timedelta(seconds=60))
+        self.main = main_client
 
-    def _lookup_orig_datablock(self, id_: str) -> OrigDatablock:
+    @_conditionally_disabled
+    def get_dataset_model(
+        self, pid: PID, strict_validation: bool = False
+    ) -> model.DownloadDataset:
+        """Fetch a dataset from SciCat."""
+        _ = strict_validation  # unused by fake
+        try:
+            return self.main.datasets[pid]
+        except KeyError:
+            raise ScicatCommError(f"Unable to retrieve dataset {pid}") from None
+
+    @_conditionally_disabled
+    def get_orig_datablocks(
+        self, pid: PID, strict_validation: bool = False
+    ) -> list[model.DownloadOrigDatablock]:
+        """Fetch an orig datablock from SciCat."""
+        _ = strict_validation  # unused by fake
         try:
-            return next(db for db in self._orig_datablocks if db.datablock_id == id_)
-        except StopIteration:
-            raise KeyError(f"No OrigDatablock with id {id_}") from None
-
-    def _get_or_add_orig_datablock(self, key: Union[int, str, PID]) -> OrigDatablock:
-        if isinstance(key, PID):
-            key = str(PID)
-        if isinstance(key, str):
-            return self._lookup_orig_datablock(key)
-        # The 0th datablock is implicitly always there and created on demand.
-        if key in (0, -1) and not self._orig_datablocks:
-            return self.add_orig_datablock(
-                checksum_algorithm=self._default_checksum_algorithm
+            return self.main.orig_datablocks[pid]
+        except KeyError:
+            raise ScicatCommError(
+                f"Unable to retrieve orig datablock for dataset {pid}"
+            ) from None
+
+    @_conditionally_disabled
+    def get_attachments_for_dataset(
+        self, pid: PID, strict_validation: bool = False
+    ) -> list[model.DownloadAttachment]:
+        """Fetch all attachments from SciCat for a given dataset."""
+        _ = strict_validation  # unused by fake
+        return self.main.attachments.get(pid) or []
+
+    @_conditionally_disabled
+    def get_sample_model(
+        self, sample_id: str, strict_validation: bool = False
+    ) -> model.DownloadSample:
+        """Fetch a sample from SciCat."""
+        _ = strict_validation  # unused by fake
+        try:
+            return self.main.samples[sample_id]
+        except KeyError:
+            raise ScicatCommError(f"Unable to retrieve sample {sample_id}") from None
+
+    @_conditionally_disabled
+    def create_dataset_model(
+        self, dset: model.UploadDerivedDataset | model.UploadRawDataset
+    ) -> model.DownloadDataset:
+        """Create a new dataset in SciCat."""
+        ingested = _process_dataset(dset)
+        pid: PID = ingested.pid  # type: ignore[assignment]
+        if pid in self.main.datasets:
+            raise ScicatCommError(
+                f"Cannot create dataset with pid '{pid}' "
+                "because there already is a dataset with this pid."
             )
-        return self._orig_datablocks[key]
-
-    def make_upload_model(self) -> Union[UploadDerivedDataset, UploadRawDataset]:
-        """Construct a SciCat upload model from self."""
-        model: Union[Type[UploadRawDataset], Type[UploadDerivedDataset]] = (
-            UploadRawDataset if self.type == DatasetType.RAW else UploadDerivedDataset
-        )
-        # Datablocks are not included here because they are handled separately
-        # by make_datablock_upload_models and their own endpoints.
-        special = ("relationships", "techniques")
-        return model(
-            numberOfFiles=self.number_of_files,
-            numberOfFilesArchived=self.number_of_files_archived,
-            size=self.size,
-            packedSize=self.packed_size,
-            scientificMetadata=self._meta or None,
-            techniques=convert_user_to_upload_model(  # type: ignore[arg-type]
-                self.techniques
-            ),
-            relationships=convert_user_to_upload_model(  # type: ignore[arg-type]
-                self.relationships
-            ),
-            **{
-                field.scicat_name: value
-                for field in self.fields()
-                if field.name not in special
-                and (value := getattr(self, field.name)) is not None
-            },
-        )
+        self.main.datasets[pid] = ingested
+        return ingested
 
-    def make_datablock_upload_models(self) -> DatablockUploadModels:
-        """Build models for all contained (orig) datablocks.
+    @_conditionally_disabled
+    def create_orig_datablock(
+        self, dblock: model.UploadOrigDatablock
+    ) -> model.DownloadOrigDatablock:
+        """Create a new orig datablock in SciCat."""
+        dataset_id = dblock.datasetId
+        if (dset := self.main.datasets.get(dataset_id)) is None:
+            raise ScicatCommError(f"No dataset with id {dataset_id}")
+        ingested = _process_orig_datablock(dblock, dset)
+        self.main.orig_datablocks.setdefault(dataset_id, []).append(ingested)
+        return ingested
 
-        Returns
-        -------
-        :
-            Structure with datablock and orig datablock models.
-        """
-        if self.number_of_files == 0:
-            return DatablockUploadModels(orig_datablocks=None)
-        return DatablockUploadModels(
-            orig_datablocks=[
-                dblock.make_upload_model(self) for dblock in self._orig_datablocks
-            ]
-        )
-
-    def make_attachment_upload_models(self) -> List[UploadAttachment]:
-        """Build models for all registered attachments.
-
-        Raises
-        ------
-        ValueError
-            If ``self.attachments`` is ``None``,
-            i.e., the attachments are uninitialized.
-
-        Returns
-        -------
-        :
-            List of attachment models.
-        """
-        if self.attachments is None:
+    @_conditionally_disabled
+    def create_attachment_for_dataset(
+        self,
+        attachment: model.UploadAttachment,
+        dataset_id: PID | None = None,
+    ) -> model.DownloadAttachment:
+        """Create a new attachment for a dataset in SciCat."""
+        if dataset_id is None:
+            dataset_id = attachment.datasetId
+        if dataset_id is None:
             raise ValueError(
-                "Cannot make upload models for attachments because "
-                "the attachments are uninitialized."
+                "Cannot determine the dataset ID for attachment. "
+                "Specify the ID as a function argument or in the attachment."
             )
-        return [a.make_upload_model() for a in self.attachments]
-
-    def validate(self) -> None:
-        """Validate the fields of the dataset.
 
-        Raises :class:`pydantic.ValidationError` if validation fails.
-        Returns normally if it passes.
-        """
-        self.make_upload_model()
-
-
-@dataclasses.dataclass
-class DatablockUploadModels:
-    """Pydantic models for (orig) datablocks."""
-
-    # TODO
-    # datablocks: Optional[List[UploadDatablock]]
-    orig_datablocks: Optional[List[UploadOrigDatablock]]
-    """Orig datablocks"""
+        ingested = _process_attachment(attachment, dataset_id)
+        if dataset_id not in self.main.datasets:
+            raise ScicatCommError(f"No dataset with id {dataset_id}")
+        self.main.attachments.setdefault(dataset_id, []).append(ingested)
+        return ingested
+
+    @_conditionally_disabled
+    def create_sample_model(self, sample: model.UploadSample) -> model.DownloadSample:
+        """Create a new sample in SciCat."""
+        ingested = _process_sample(sample)
+        if ingested.sampleId in self.main.samples:
+            raise ScicatCommError(
+                f"Cannot create sample with id '{ingested.sampleId}' "
+                "because there already is a sample with this id."
+            )
+        sample_id: str = ingested.sampleId  # type: ignore[assignment]
+        self.main.samples[sample_id] = ingested
+        return ingested
+
+    @_conditionally_disabled
+    def validate_dataset_model(
+        self, dset: model.UploadDerivedDataset | model.UploadRawDataset
+    ) -> None:
+        """Validate model remotely in SciCat."""
+        # Models were locally validated on construction, assume they are valid.
+        pass
+
+
+def _model_dict(mod: model.BaseModel) -> dict[str, Any]:
+    return {
+        key: deepcopy(val)
+        for key in mod.model_fields.keys()
+        if (val := getattr(mod, key)) is not None
+    }
+
+
+def _process_relationship(
+    relationship: model.UploadRelationship,
+) -> model.DownloadRelationship:
+    return model.DownloadRelationship(**_model_dict(relationship))
+
+
+def _process_technique(technique: model.UploadTechnique) -> model.DownloadTechnique:
+    return model.DownloadTechnique(**_model_dict(technique))
+
+
+def _process_data_file(file: model.UploadDataFile) -> model.DownloadDataFile:
+    return model.DownloadDataFile(**_model_dict(file))
+
+
+def _process_dataset(
+    dset: model.UploadDerivedDataset | model.UploadRawDataset,
+) -> model.DownloadDataset:
+    created_at = datetime.datetime.now(tz=datetime.timezone.utc)
+    # TODO use user login if possible
+    # Using strict_validation=False because the input model should already be validated.
+    # If there are validation errors, it was probably intended by the user.
+    fields = _model_dict(dset)
+    if "relationships" in fields:
+        fields["relationships"] = list(
+            map(_process_relationship, fields["relationships"])
+        )
+    if "techniques" in fields:
+        fields["techniques"] = list(map(_process_technique, fields["techniques"]))
+    return model.construct(
+        model.DownloadDataset,
+        _strict_validation=False,
+        pid=PID.generate(prefix="PID.prefix.a0b1"),
+        createdBy="fake",
+        createdAt=created_at,
+        updatedBy="fake",
+        updatedAt=created_at,
+        **fields,
+    )
+
+
+def _process_orig_datablock(
+    dblock: model.UploadOrigDatablock,
+    dset: model.DownloadDataset,
+) -> model.DownloadOrigDatablock:
+    created_at = datetime.datetime.now(tz=datetime.timezone.utc)
+    # TODO use user login if possible
+    # TODO more fields
+    # Using strict_validation=False because the input model should already be validated.
+    # If there are validation errors, it was probably intended by the user.
+    fields = _model_dict(dblock)
+    if "dataFileList" in fields:
+        fields["dataFileList"] = list(map(_process_data_file, fields["dataFileList"]))
+    fields["accessGroups"] = dset.accessGroups
+    processed = model.construct(
+        model.DownloadOrigDatablock,
+        _strict_validation=False,
+        createdBy="fake",
+        createdAt=created_at,
+        updatedBy="fake",
+        updatedAt=created_at,
+        **fields,
+    )
+    return processed
+
+
+def _process_attachment(
+    attachment: model.UploadAttachment, dataset_id: PID | None = None
+) -> model.DownloadAttachment:
+    created_at = datetime.datetime.now(tz=datetime.timezone.utc)
+    fields = _model_dict(attachment)
+    if fields.get("id") is None:
+        fields["id"] = str(uuid.uuid4())
+    if dataset_id is not None:
+        fields["datasetId"] = dataset_id
+    # Using strict_validation=False because the input model should already be validated.
+    # If there are validation errors, it was probably intended by the user.
+    return model.construct(
+        model.DownloadAttachment,
+        _strict_validation=False,
+        createdBy="fake",
+        createdAt=created_at,
+        updatedBy="fake",
+        updatedAt=created_at,
+        **fields,
+    )
+
+
+def _process_sample(sample: model.UploadSample) -> model.DownloadSample:
+    created_at = datetime.datetime.now(tz=datetime.timezone.utc)
+    fields = _model_dict(sample)
+    if fields.get("sampleId") is None:
+        fields["sampleId"] = str(uuid.uuid4())
+    # Using strict_validation=False because the input model should already be validated.
+    # If there are validation errors, it was probably intended by the user.
+    return model.construct(
+        model.DownloadSample,
+        _strict_validation=False,
+        createdBy="fake",
+        createdAt=created_at,
+        updatedBy="fake",
+        updatedAt=created_at,
+        **fields,
+    )
+
+
+def process_uploaded_dataset(
+    dataset: model.UploadDerivedDataset | model.UploadRawDataset,
+    orig_datablocks: list[model.UploadOrigDatablock] | None,
+    attachments: list[model.UploadAttachment] | None,
+) -> tuple[
+    model.DownloadDataset,
+    list[model.DownloadOrigDatablock] | None,
+    list[model.DownloadAttachment] | None,
+]:
+    """Process a dataset as if it was uploaded to SciCat.
+
+    This function attempts to mimic how SciCat converts uploaded dataset
+    (and associated) models to the in-database (and download) models.
+    It is not completely faithful to the real SciCat but only an approximation.
+    """
+    ds = _process_dataset(dataset)
+    dblocks = (
+        [_process_orig_datablock(db, ds) for db in orig_datablocks]
+        if orig_datablocks is not None
+        else None
+    )
+    atts = (
+        list(map(_process_attachment, attachments)) if attachments is not None else None
+    )
+    return ds, dblocks, atts
```

### Comparing `scitacean-23.8.0/src/scitacean/file.py` & `scitacean-24.4.0/src/scitacean/file.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Class to represent files."""
 
 from __future__ import annotations
 
 import dataclasses
 import warnings
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import NoReturn, Optional, Union, cast
+from typing import NoReturn, cast
+
+import dateutil.parser
 
 from .error import IntegrityError
 from .filesystem import RemotePath, checksum_of_file, file_modification_time, file_size
 from .logging import get_logger
 from .model import DownloadDataFile, UploadDataFile
 
 
@@ -37,45 +39,43 @@
          local                                  remote
            │                                      │
            │ uploaded                  downloaded │
            │                                      │
            └───────────> local+remote <───────────┘
     """
 
-    local_path: Optional[Path]
+    local_path: Path | None
     """Path to the file on the local filesystem."""
     remote_path: RemotePath
     """Path to the file on the remote filesystem."""
-    remote_gid: Optional[str]
+    remote_gid: str | None
     """Unix group ID on remote."""
-    remote_perm: Optional[str]
+    remote_perm: str | None
     """Unix file mode on remote."""
-    remote_uid: Optional[str]
+    remote_uid: str | None
     """Unix user ID on remote."""
-    checksum_algorithm: Optional[str] = None
+    checksum_algorithm: str | None = None
     """Algorithm to use for checksums."""
-    _remote_size: Optional[int] = dataclasses.field(default=None, repr=False)
-    _remote_creation_time: Optional[datetime] = dataclasses.field(
-        default=None, repr=False
-    )
-    _remote_checksum: Optional[str] = dataclasses.field(default=None, repr=False)
-    _checksum_cache: Optional[_Checksum] = dataclasses.field(
+    _remote_size: int | None = dataclasses.field(default=None, repr=False)
+    _remote_creation_time: datetime | None = dataclasses.field(default=None, repr=False)
+    _remote_checksum: str | None = dataclasses.field(default=None, repr=False)
+    _checksum_cache: _Checksum | None = dataclasses.field(
         default=None, compare=False, repr=False
     )
 
     @classmethod
     def from_local(
         cls,
-        path: Union[str, Path],
+        path: str | Path,
         *,
-        base_path: Union[str, Path] = "",
-        remote_path: Optional[Union[str, RemotePath]] = None,
-        remote_uid: Optional[str] = None,
-        remote_gid: Optional[str] = None,
-        remote_perm: Optional[str] = None,
+        base_path: str | Path = "",
+        remote_path: str | RemotePath | None = None,
+        remote_uid: str | None = None,
+        remote_gid: str | None = None,
+        remote_perm: str | None = None,
     ) -> File:
         """Link a file on the local filesystem.
 
         Given following ``path``, ``base_path``, and ``source_folder``::
 
             path:                      somewhere/on/local/folder/file.nxs
             base_bath:                 somewhere/on/local
@@ -88,45 +88,117 @@
 
         ``remote_path`` can also be overridden, in which case ``path`` and
         ``base_path`` are not used to deduce the "actual remote location".
 
         Parameters
         ----------
         path:
-            Full path the local file.
+            Full path of the local file.
         base_path:
             Only use ``path.relative_to(base_path)`` to determine the remote location.
         remote_path:
             Path on the remote, relative to ``source_folder``.
         remote_uid:
             User ID on the remote. Will be determined automatically on upload.
         remote_gid:
             Group ID on the remote. Will be determined automatically on upload.
         remote_perm:
             File permissions on the remote. Will be determined automatically on upload.
+
+        Returns
+        -------
+        :
+            A new file object.
         """
         path = Path(path)
         if not remote_path:
             remote_path = RemotePath.from_local(path.relative_to(base_path))
         return File(
             local_path=path,
             remote_path=RemotePath(remote_path),
             remote_gid=remote_gid,
             remote_perm=remote_perm,
             remote_uid=remote_uid,
             _checksum_cache=_Checksum(),
         )
 
     @classmethod
+    def from_remote(
+        cls,
+        remote_path: str | RemotePath,
+        size: int,
+        creation_time: datetime | str,
+        checksum: str | None = None,
+        checksum_algorithm: str | None = None,
+        remote_uid: str | None = None,
+        remote_gid: str | None = None,
+        remote_perm: str | None = None,
+    ) -> File:
+        """Construct a new file object for a remote file.
+
+        The local path of the returned ``File`` is ``None``.
+
+        Parameters
+        ----------
+        remote_path:
+            Path the remote file relative to the dataset's source folder.
+        size:
+            Size in bytes on the remote filesystem.
+        creation_time:
+            Date and time the file was created on the remote filesystem.
+            If a ``str``, it is parsed using ``dateutil.parser.parse``.
+        checksum:
+            Checksum of the file.
+        checksum_algorithm:
+            Algorithm used to compute the given checksum.
+            Must be passed when ``checksum is not None``.
+        remote_uid:
+            User ID on the remote.
+        remote_gid:
+            Group ID on the remote.
+        remote_perm:
+            File permissions on the remote.
+
+        Returns
+        -------
+        :
+            A new file object.
+
+
+        .. versionadded:: 23.10.0
+        """
+        if checksum is not None and checksum_algorithm is None:
+            raise TypeError(
+                "Must specify checksum_algorithm when providing a checksum."
+            )
+
+        creation_time = (
+            creation_time
+            if isinstance(creation_time, datetime)
+            else dateutil.parser.parse(creation_time)
+        )
+        return File(
+            local_path=None,
+            remote_path=RemotePath(remote_path),
+            remote_uid=remote_uid,
+            remote_gid=remote_gid,
+            remote_perm=remote_perm,
+            _remote_size=size,
+            _remote_creation_time=creation_time,
+            _remote_checksum=checksum,
+            checksum_algorithm=checksum_algorithm,
+        )
+
+    @classmethod
     def from_download_model(
         cls,
         model: DownloadDataFile,
         *,
-        checksum_algorithm: Optional[str] = None,
-        local_path: Optional[Union[str, Path]] = None,
+        checksum_algorithm: str | None = None,
+        local_path: str | Path | None = None,
     ) -> File:
         """Construct a new file object from a SciCat download model.
 
         Parameters
         ----------
         model:
             Pydantic model for the file.
@@ -170,15 +242,15 @@
         If the file exists on local, return the time the local file was last modified.
         Otherwise, return the stored time in the catalogue.
         """
         if self.is_on_local:
             return file_modification_time(cast(Path, self.local_path))
         return self._remote_creation_time  # type: ignore[return-value]
 
-    def checksum(self) -> Optional[str]:
+    def checksum(self) -> str | None:
         """Return the checksum of the file.
 
         This can take a long time to compute for large files.
 
         If the file exists on local, return the current checksum of the local file.
         Otherwise, return the stored checksum in the catalogue.
 
@@ -192,17 +264,15 @@
         if self.checksum_algorithm is None:
             return None
         return self._checksum_cache.get(  # type: ignore[union-attr]
             path=self.local_path,  # type: ignore[arg-type]
             algorithm=self.checksum_algorithm,
         )
 
-    def remote_access_path(
-        self, source_folder: Union[RemotePath, str]
-    ) -> Optional[RemotePath]:
+    def remote_access_path(self, source_folder: RemotePath | str) -> RemotePath | None:
         """Full path to the file on the remote if it exists."""
         return (source_folder / self.remote_path) if self.is_on_remote else None
 
     @property
     def is_on_remote(self) -> bool:
         """True if the file is on remote."""
         return self._remote_size is not None
@@ -270,20 +340,20 @@
             time=self.creation_time,
             uid=self.remote_uid,
         )
 
     def uploaded(
         self,
         *,
-        remote_path: Optional[Union[str, RemotePath]] = None,
-        remote_uid: Optional[str] = None,
-        remote_gid: Optional[str] = None,
-        remote_perm: Optional[str] = None,
-        remote_creation_time: Optional[datetime] = None,
-        remote_size: Optional[int] = None,
+        remote_path: str | RemotePath | None = None,
+        remote_uid: str | None = None,
+        remote_gid: str | None = None,
+        remote_perm: str | None = None,
+        remote_creation_time: datetime | None = None,
+        remote_size: int | None = None,
     ) -> File:
         """Return new file metadata after an upload.
 
         Assumes that the input file exists on local.
         The returned object is on both local and remote.
 
         Parameters
@@ -316,20 +386,18 @@
             remote_perm=remote_perm,
             _remote_creation_time=remote_creation_time,
         )
         return dataclasses.replace(
             self,
             _remote_size=remote_size if remote_size is not None else self.size,
             _remote_checksum=self.checksum(),
-            **{
-                key: val for key, val in args.items() if val is not None
-            },  # type: ignore[arg-type]
+            **{key: val for key, val in args.items() if val is not None},  # type: ignore[arg-type]
         )
 
-    def downloaded(self, *, local_path: Union[str, Path]) -> File:
+    def downloaded(self, *, local_path: str | Path) -> File:
         """Return new file metadata after a download.
 
         Assumes that the input file exists on remote.
         The returned object is on both local and remote.
 
         Parameters
         ----------
@@ -404,18 +472,18 @@
     raise typ(msg)
 
 
 class _Checksum:
     """Compute and cache the checksum of a file."""
 
     def __init__(self) -> None:
-        self._value: Optional[str] = None
-        self._path: Optional[Path] = None
-        self._algorithm: Optional[str] = None
-        self._access_time: Optional[datetime] = None
+        self._value: str | None = None
+        self._path: Path | None = None
+        self._algorithm: str | None = None
+        self._access_time: datetime | None = None
 
     def get(self, *, path: Path, algorithm: str) -> str:
         if self._is_out_of_date(path=path, algorithm=algorithm):
             self._update(path=path, algorithm=algorithm)
         return self._value  # type: ignore[return-value]
 
     def _is_out_of_date(self, *, path: Path, algorithm: str) -> bool:
```

### Comparing `scitacean-23.8.0/src/scitacean/filesystem.py` & `scitacean-24.4.0/src/scitacean/filesystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Filesystem utilities.
 
 Scitacean distinguishes between paths on the local filesystem and
 paths on the remote file server.
 The former are encoded ad :class:`pathlib.Path`
 and the latter as :class:`scitacean.filesystem.RemotePath`.
 But conversions from plain strings are usually supported but should be used with care.
@@ -12,38 +12,18 @@
 from __future__ import annotations
 
 import hashlib
 import os
 import re
 from datetime import datetime, timezone
 from pathlib import Path, PurePath
-from typing import Any, Callable, Generator, Optional, TypeVar, Union
+from typing import Any, TypeVar
 
-from ._internal.pydantic_compat import is_pydantic_v1
-
-if not is_pydantic_v1():
-    from typing import Type
-
-    from pydantic import GetCoreSchemaHandler
-    from pydantic_core import core_schema
-
-    def _get_remote_path_core_schema(
-        cls: Type[RemotePath], _source_type: Any, _handler: GetCoreSchemaHandler
-    ) -> core_schema.CoreSchema:
-        return core_schema.no_info_after_validator_function(
-            cls,
-            core_schema.union_schema(
-                [core_schema.is_instance_schema(RemotePath), core_schema.str_schema()]
-            ),
-            serialization=core_schema.plain_serializer_function_ser_schema(
-                lambda p: p.posix if isinstance(p, RemotePath) else str(p),
-                info_arg=False,
-                return_schema=core_schema.str_schema(),
-            ),
-        )
+from pydantic import GetCoreSchemaHandler
+from pydantic_core import core_schema
 
 
 class RemotePath:
     """A path on the remote filesystem.
 
     Remote paths do not need to correspond to a regular filesystem path like
     :class:`pathlib.PosixPath` or :class:`pathlib.WindowsPath`.
@@ -52,15 +32,15 @@
 
     RemotePath is strict about input types in order to prompt the user to think about
     correct, cross-platform handling of paths.
     In particular, there is only limited interoperability with local paths as
     the two should almost never be mixed.
     """
 
-    def __init__(self, *path_segments: Union[str, RemotePath]) -> None:
+    def __init__(self, *path_segments: str | RemotePath) -> None:
         """Initialize from given path segments."""
         for segment in path_segments:
             if isinstance(segment, (PurePath, Path)):  # type: ignore[unreachable]
                 raise TypeError(
                     "OS paths are not supported by RemotePath.__init__. "
                     "use RemotePath.from_local instead."
                 )
@@ -82,15 +62,15 @@
     def to_local(self) -> PurePath:
         """Return self as a local, OS-specific path."""
         segments = self._path.split("/")
         if segments[0] == "":
             segments = ["/"] + segments[1:]
         return PurePath(*segments)
 
-    def __truediv__(self, other: Union[str, RemotePath]) -> RemotePath:
+    def __truediv__(self, other: str | RemotePath) -> RemotePath:
         """Join two path segments."""
         if isinstance(other, (PurePath, Path)):  # type: ignore[unreachable]
             raise TypeError("OS paths are not supported when concatenating RemotePath.")
         this = _strip_trailing_slash(self.posix)
         other = _strip_leading_slash(_strip_trailing_slash(_posix(other)))
         return RemotePath(f"{this}/{other}")
 
@@ -123,15 +103,15 @@
 
     @property
     def name(self) -> str:
         """The name of the file with all directories removed."""
         return self._path.rstrip("/").rsplit("/", 1)[-1]
 
     @property
-    def suffix(self) -> Optional[str]:
+    def suffix(self) -> str | None:
         """The file extension including a leading period."""
         parts = self.name.rsplit(".", 1)
         if len(parts) == 1:
             return None
         return "." + parts[1]
 
     @property
@@ -168,31 +148,36 @@
             name = parts[0]
             suffix = "." + parts[1] if len(parts) > 1 else ""
             return (name[: max(1, max_length - len(suffix))] + suffix)[:max_length]
 
         return RemotePath("/".join(map(trunc, self._path.split("/"))))
 
     @classmethod
-    def validate(cls, value: Union[str, RemotePath]) -> RemotePath:
+    def validate(cls, value: str | RemotePath) -> RemotePath:
         """Pydantic validator for RemotePath fields."""
         return RemotePath(value)
 
-    if is_pydantic_v1():
-
-        @classmethod
-        def __get_validators__(
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, _source_type: Any, _handler: GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
+        return core_schema.no_info_after_validator_function(
             cls,
-        ) -> Generator[Callable[[Union[str, RemotePath]], RemotePath], None, None]:
-            yield cls.validate
-
-    else:
-        __get_pydantic_core_schema__ = classmethod(_get_remote_path_core_schema)
+            core_schema.union_schema(
+                [core_schema.is_instance_schema(RemotePath), core_schema.str_schema()]
+            ),
+            serialization=core_schema.plain_serializer_function_ser_schema(
+                lambda p: p.posix if isinstance(p, RemotePath) else str(p),
+                info_arg=False,
+                return_schema=core_schema.str_schema(),
+            ),
+        )
 
 
-def _posix(path: Union[str, RemotePath]) -> str:
+def _posix(path: str | RemotePath) -> str:
     return path.posix if isinstance(path, RemotePath) else path
 
 
 def _strip_trailing_slash(s: str) -> str:
     return s[:-1] if s.endswith("/") else s
 
 
@@ -207,23 +192,19 @@
 
 def file_modification_time(path: Path) -> datetime:
     """Return the time in UTC when a local file was last modified."""
     return datetime.fromtimestamp(path.stat().st_mtime).astimezone(timezone.utc)
 
 
 def _new_hash(algorithm: str) -> Any:
-    try:
-        return hashlib.new(algorithm, usedforsecurity=False)
-    except TypeError:
-        # Fallback for Python < 3.9
-        return hashlib.new(algorithm)
+    return hashlib.new(algorithm, usedforsecurity=False)
 
 
 # size based on http://git.savannah.gnu.org/gitweb/?p=coreutils.git;a=blob;f=src/ioblksize.h;h=ed2f4a9c4d77462f357353eb73ee4306c28b37f1;hb=HEAD#l23  # noqa: E501
-def checksum_of_file(path: Union[str, Path], *, algorithm: str) -> str:
+def checksum_of_file(path: str | Path, *, algorithm: str) -> str:
     """Compute the checksum of a local file.
 
     Parameters
     ----------
     path:
         Path of the file on the local filesystem.
     algorithm:
@@ -238,15 +219,15 @@
     buffer = memoryview(bytearray(128 * 1024))
     with open(path, "rb", buffering=0) as file:
         for n in iter(lambda: file.readinto(buffer), 0):
             chk.update(buffer[:n])
     return chk.hexdigest()  # type: ignore[no-any-return]
 
 
-P = TypeVar("P", bound=Union[str, Path, RemotePath])
+P = TypeVar("P", bound=str | Path | RemotePath)
 
 
 def escape_path(path: P) -> P:
     """Escape disallowed characters for file paths.
 
     Replaces
 
@@ -266,13 +247,11 @@
     Returns
     -------
     :
         ``path`` with offending characters replaced.
         Has the same type as ``path``.
     """
     s = (
-        path.posix
-        if isinstance(path, RemotePath)
-        else os.fspath(path)  # type: ignore[arg-type]
+        path.posix if isinstance(path, RemotePath) else os.fspath(path)  # type: ignore[arg-type]
     )
     no_utf = s.encode("ascii", "backslashreplace").decode("ascii")
     return type(path)(re.sub(r"[^\w .\-]", "_", no_utf))  # type: ignore[return-value]
```

### Comparing `scitacean-23.8.0/src/scitacean/logging.py` & `scitacean-24.4.0/src/scitacean/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Utilities for logging in Scitacean.
 
 The object returned by :func:`scitacean.get_logger` is the only logger
 used by Scitacean. Scitacean does not configure it in any way.
 You are free to do so.
 """
```

### Comparing `scitacean-23.8.0/src/scitacean/model.py` & `scitacean-24.4.0/src/scitacean/model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ##########################################
 # This file was automatically generated. #
 # Do not modify it directly!             #
 ##########################################
 
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Models for communication with SciCat and user facing dataclasses.
 
 The high-level :class:`scitacean.Client` and :class:`scitacean.Dataset` return objects
 from the SciCat database in the form of 'user models'.
 Those are usually all that is required for working with Scitacean.
 
 At a lower level, those models are converted to or from upload or download models,
@@ -77,15 +77,15 @@
 
    construct
 """
 
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Type
+from typing import Any
 
 import pydantic
 from pydantic import NonNegativeInt
 
 from ._base_model import (
     BaseModel,
     BaseUserModel,
@@ -93,631 +93,640 @@
     construct,
     validate_datetime,
     validate_drop,
     validate_emails,
     validate_orcids,
 )
 from ._internal.dataclass_wrapper import dataclass_optional_args
-from ._internal.pydantic_compat import field_validator
 from .filesystem import RemotePath
 from .pid import PID
 from .thumbnail import Thumbnail
 
 
 class DownloadDataset(
     BaseModel, masked=("attachments", "datablocks", "origdatablocks")
 ):
-    contactEmail: Optional[str] = None
-    creationLocation: Optional[str] = None
-    creationTime: Optional[datetime] = None
-    inputDatasets: Optional[List[PID]] = None
-    investigator: Optional[str] = None
-    numberOfFilesArchived: Optional[NonNegativeInt] = None
-    owner: Optional[str] = None
-    ownerGroup: Optional[str] = None
-    principalInvestigator: Optional[str] = None
-    sourceFolder: Optional[RemotePath] = None
-    type: Optional[DatasetType] = None
-    usedSoftware: Optional[List[str]] = None
-    accessGroups: Optional[List[str]] = None
-    version: Optional[str] = None
-    classification: Optional[str] = None
-    comment: Optional[str] = None
-    createdAt: Optional[datetime] = None
-    createdBy: Optional[str] = None
-    dataFormat: Optional[str] = None
-    dataQualityMetrics: Optional[int] = None
-    description: Optional[str] = None
-    endTime: Optional[datetime] = None
-    history: Optional[None] = None
-    instrumentGroup: Optional[str] = None
-    instrumentId: Optional[str] = None
-    isPublished: Optional[bool] = None
-    jobLogData: Optional[str] = None
-    jobParameters: Optional[Dict[str, Any]] = None
-    keywords: Optional[List[str]] = None
-    license: Optional[str] = None
-    datasetlifecycle: Optional[DownloadLifecycle] = None
-    scientificMetadata: Optional[Dict[str, Any]] = None
-    datasetName: Optional[str] = None
-    numberOfFiles: Optional[NonNegativeInt] = None
-    orcidOfOwner: Optional[str] = None
-    ownerEmail: Optional[str] = None
-    packedSize: Optional[NonNegativeInt] = None
-    pid: Optional[PID] = None
-    proposalId: Optional[str] = None
-    relationships: Optional[List[DownloadRelationship]] = None
-    sampleId: Optional[str] = None
-    sharedWith: Optional[List[str]] = None
-    size: Optional[NonNegativeInt] = None
-    sourceFolderHost: Optional[str] = None
-    techniques: Optional[List[DownloadTechnique]] = None
-    updatedAt: Optional[datetime] = None
-    updatedBy: Optional[str] = None
-    validationStatus: Optional[str] = None
+    contactEmail: str | None = None
+    creationLocation: str | None = None
+    creationTime: datetime | None = None
+    inputDatasets: list[PID] | None = None
+    investigator: str | None = None
+    numberOfFilesArchived: NonNegativeInt | None = None
+    owner: str | None = None
+    ownerGroup: str | None = None
+    principalInvestigator: str | None = None
+    sourceFolder: RemotePath | None = None
+    type: DatasetType | None = None
+    usedSoftware: list[str] | None = None
+    accessGroups: list[str] | None = None
+    version: str | None = None
+    classification: str | None = None
+    comment: str | None = None
+    createdAt: datetime | None = None
+    createdBy: str | None = None
+    dataFormat: str | None = None
+    dataQualityMetrics: int | None = None
+    description: str | None = None
+    endTime: datetime | None = None
+    history: None = None
+    instrumentGroup: str | None = None
+    instrumentId: str | None = None
+    isPublished: bool | None = None
+    jobLogData: str | None = None
+    jobParameters: dict[str, Any] | None = None
+    keywords: list[str] | None = None
+    license: str | None = None
+    datasetlifecycle: DownloadLifecycle | None = None
+    scientificMetadata: dict[str, Any] | None = None
+    datasetName: str | None = None
+    numberOfFiles: NonNegativeInt | None = None
+    orcidOfOwner: str | None = None
+    ownerEmail: str | None = None
+    packedSize: NonNegativeInt | None = None
+    pid: PID | None = None
+    proposalId: str | None = None
+    relationships: list[DownloadRelationship] | None = None
+    sampleId: str | None = None
+    sharedWith: list[str] | None = None
+    size: NonNegativeInt | None = None
+    sourceFolderHost: str | None = None
+    techniques: list[DownloadTechnique] | None = None
+    updatedAt: datetime | None = None
+    updatedBy: str | None = None
+    validationStatus: str | None = None
 
-    @field_validator("creationTime", "createdAt", "endTime", "updatedAt", mode="before")
+    @pydantic.field_validator(
+        "creationTime", "createdAt", "endTime", "updatedAt", mode="before"
+    )
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
-    @field_validator("history", mode="before")
+    @pydantic.field_validator("history", mode="before")
     def _validate_drop(cls, value: Any) -> Any:
         return validate_drop(value)
 
-    @field_validator("contactEmail", "ownerEmail", mode="before")
+    @pydantic.field_validator("contactEmail", "ownerEmail", mode="before")
     def _validate_emails(cls, value: Any) -> Any:
         return validate_emails(value)
 
-    @field_validator("orcidOfOwner", mode="before")
+    @pydantic.field_validator("orcidOfOwner", mode="before")
     def _validate_orcids(cls, value: Any) -> Any:
         return validate_orcids(value)
 
 
 class UploadDerivedDataset(BaseModel):
     contactEmail: str
     creationTime: datetime
-    inputDatasets: List[PID]
+    inputDatasets: list[PID]
     investigator: str
     numberOfFilesArchived: NonNegativeInt
     owner: str
     ownerGroup: str
     sourceFolder: RemotePath
     type: DatasetType
-    usedSoftware: List[str]
-    accessGroups: Optional[List[str]] = None
-    classification: Optional[str] = None
-    comment: Optional[str] = None
-    dataQualityMetrics: Optional[int] = None
-    description: Optional[str] = None
-    instrumentGroup: Optional[str] = None
-    isPublished: Optional[bool] = None
-    jobLogData: Optional[str] = None
-    jobParameters: Optional[Dict[str, Any]] = None
-    keywords: Optional[List[str]] = None
-    license: Optional[str] = None
-    scientificMetadata: Optional[Dict[str, Any]] = None
-    datasetName: Optional[str] = None
-    numberOfFiles: Optional[NonNegativeInt] = None
-    orcidOfOwner: Optional[str] = None
-    ownerEmail: Optional[str] = None
-    packedSize: Optional[NonNegativeInt] = None
-    relationships: Optional[List[UploadRelationship]] = None
-    sharedWith: Optional[List[str]] = None
-    size: Optional[NonNegativeInt] = None
-    sourceFolderHost: Optional[str] = None
-    techniques: Optional[List[UploadTechnique]] = None
-    validationStatus: Optional[str] = None
+    usedSoftware: list[str]
+    accessGroups: list[str] | None = None
+    classification: str | None = None
+    comment: str | None = None
+    dataQualityMetrics: int | None = None
+    description: str | None = None
+    instrumentGroup: str | None = None
+    isPublished: bool | None = None
+    jobLogData: str | None = None
+    jobParameters: dict[str, Any] | None = None
+    keywords: list[str] | None = None
+    license: str | None = None
+    scientificMetadata: dict[str, Any] | None = None
+    datasetName: str | None = None
+    numberOfFiles: NonNegativeInt | None = None
+    orcidOfOwner: str | None = None
+    ownerEmail: str | None = None
+    packedSize: NonNegativeInt | None = None
+    relationships: list[UploadRelationship] | None = None
+    sharedWith: list[str] | None = None
+    size: NonNegativeInt | None = None
+    sourceFolderHost: str | None = None
+    techniques: list[UploadTechnique] | None = None
+    validationStatus: str | None = None
 
-    @field_validator("creationTime", mode="before")
+    @pydantic.field_validator("creationTime", mode="before")
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
-    @field_validator("contactEmail", "ownerEmail", mode="before")
+    @pydantic.field_validator("contactEmail", "ownerEmail", mode="before")
     def _validate_emails(cls, value: Any) -> Any:
         return validate_emails(value)
 
-    @field_validator("orcidOfOwner", mode="before")
+    @pydantic.field_validator("orcidOfOwner", mode="before")
     def _validate_orcids(cls, value: Any) -> Any:
         return validate_orcids(value)
 
 
 class UploadRawDataset(BaseModel):
     contactEmail: str
     creationLocation: str
     creationTime: datetime
     numberOfFilesArchived: NonNegativeInt
     owner: str
     ownerGroup: str
     principalInvestigator: str
     sourceFolder: RemotePath
     type: DatasetType
-    accessGroups: Optional[List[str]] = None
-    classification: Optional[str] = None
-    comment: Optional[str] = None
-    dataFormat: Optional[str] = None
-    dataQualityMetrics: Optional[int] = None
-    description: Optional[str] = None
-    endTime: Optional[datetime] = None
-    instrumentGroup: Optional[str] = None
-    instrumentId: Optional[str] = None
-    isPublished: Optional[bool] = None
-    keywords: Optional[List[str]] = None
-    license: Optional[str] = None
-    scientificMetadata: Optional[Dict[str, Any]] = None
-    datasetName: Optional[str] = None
-    numberOfFiles: Optional[NonNegativeInt] = None
-    orcidOfOwner: Optional[str] = None
-    ownerEmail: Optional[str] = None
-    packedSize: Optional[NonNegativeInt] = None
-    proposalId: Optional[str] = None
-    relationships: Optional[List[UploadRelationship]] = None
-    sampleId: Optional[str] = None
-    sharedWith: Optional[List[str]] = None
-    size: Optional[NonNegativeInt] = None
-    sourceFolderHost: Optional[str] = None
-    techniques: Optional[List[UploadTechnique]] = None
-    validationStatus: Optional[str] = None
+    accessGroups: list[str] | None = None
+    classification: str | None = None
+    comment: str | None = None
+    dataFormat: str | None = None
+    dataQualityMetrics: int | None = None
+    description: str | None = None
+    endTime: datetime | None = None
+    instrumentGroup: str | None = None
+    instrumentId: str | None = None
+    isPublished: bool | None = None
+    keywords: list[str] | None = None
+    license: str | None = None
+    scientificMetadata: dict[str, Any] | None = None
+    datasetName: str | None = None
+    numberOfFiles: NonNegativeInt | None = None
+    orcidOfOwner: str | None = None
+    ownerEmail: str | None = None
+    packedSize: NonNegativeInt | None = None
+    proposalId: str | None = None
+    relationships: list[UploadRelationship] | None = None
+    sampleId: str | None = None
+    sharedWith: list[str] | None = None
+    size: NonNegativeInt | None = None
+    sourceFolderHost: str | None = None
+    techniques: list[UploadTechnique] | None = None
+    validationStatus: str | None = None
 
-    @field_validator("creationTime", "endTime", mode="before")
+    @pydantic.field_validator("creationTime", "endTime", mode="before")
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
-    @field_validator("contactEmail", "ownerEmail", mode="before")
+    @pydantic.field_validator("contactEmail", "ownerEmail", mode="before")
     def _validate_emails(cls, value: Any) -> Any:
         return validate_emails(value)
 
-    @field_validator("orcidOfOwner", mode="before")
+    @pydantic.field_validator("orcidOfOwner", mode="before")
     def _validate_orcids(cls, value: Any) -> Any:
         return validate_orcids(value)
 
 
 class DownloadAttachment(BaseModel):
-    caption: Optional[str] = None
-    ownerGroup: Optional[str] = None
-    accessGroups: Optional[List[str]] = None
-    createdAt: Optional[datetime] = None
-    createdBy: Optional[str] = None
-    datasetId: Optional[PID] = None
-    id: Optional[str] = None
-    instrumentGroup: Optional[str] = None
-    proposalId: Optional[str] = None
-    sampleId: Optional[str] = None
-    thumbnail: Optional[Thumbnail] = None
-    updatedAt: Optional[datetime] = None
-    updatedBy: Optional[str] = None
+    caption: str | None = None
+    ownerGroup: str | None = None
+    accessGroups: list[str] | None = None
+    createdAt: datetime | None = None
+    createdBy: str | None = None
+    datasetId: PID | None = None
+    id: str | None = None
+    instrumentGroup: str | None = None
+    isPublished: bool | None = None
+    proposalId: str | None = None
+    sampleId: str | None = None
+    thumbnail: Thumbnail | None = None
+    updatedAt: datetime | None = None
+    updatedBy: str | None = None
 
-    @field_validator("createdAt", "updatedAt", mode="before")
+    @pydantic.field_validator("createdAt", "updatedAt", mode="before")
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
     @classmethod
-    def user_model_type(cls) -> Type[Attachment]:
+    def user_model_type(cls) -> type[Attachment]:
         return Attachment
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadAttachment]:
+    def upload_model_type(cls) -> type[UploadAttachment]:
         return UploadAttachment
 
 
 class UploadAttachment(BaseModel):
     caption: str
     ownerGroup: str
-    accessGroups: Optional[List[str]] = None
-    datasetId: Optional[PID] = None
-    id: Optional[str] = None
-    instrumentGroup: Optional[str] = None
-    proposalId: Optional[str] = None
-    sampleId: Optional[str] = None
-    thumbnail: Optional[Thumbnail] = None
+    accessGroups: list[str] | None = None
+    datasetId: PID | None = None
+    id: str | None = None
+    instrumentGroup: str | None = None
+    proposalId: str | None = None
+    sampleId: str | None = None
+    thumbnail: Thumbnail | None = None
 
     @classmethod
-    def user_model_type(cls) -> Type[Attachment]:
+    def user_model_type(cls) -> type[Attachment]:
         return Attachment
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadAttachment]:
+    def download_model_type(cls) -> type[DownloadAttachment]:
         return DownloadAttachment
 
 
 class DownloadOrigDatablock(BaseModel):
-    dataFileList: Optional[List[DownloadDataFile]] = None
-    datasetId: Optional[PID] = None
-    ownerGroup: Optional[str] = None
-    size: Optional[NonNegativeInt] = None
-    id: Optional[str] = pydantic.Field(alias="_id", default=None)
-    accessGroups: Optional[List[str]] = None
-    chkAlg: Optional[str] = None
-    createdAt: Optional[datetime] = None
-    createdBy: Optional[str] = None
-    instrumentGroup: Optional[str] = None
-    updatedAt: Optional[datetime] = None
-    updatedBy: Optional[str] = None
+    dataFileList: list[DownloadDataFile] | None = None
+    datasetId: PID | None = None
+    size: NonNegativeInt | None = None
+    id: str | None = pydantic.Field(alias="_id", default=None)
+    accessGroups: list[str] | None = None
+    chkAlg: str | None = None
+    createdAt: datetime | None = None
+    createdBy: str | None = None
+    instrumentGroup: str | None = None
+    isPublished: bool | None = None
+    ownerGroup: str | None = None
+    updatedAt: datetime | None = None
+    updatedBy: str | None = None
 
-    @field_validator("createdAt", "updatedAt", mode="before")
+    @pydantic.field_validator("createdAt", "updatedAt", mode="before")
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadOrigDatablock]:
+    def upload_model_type(cls) -> type[UploadOrigDatablock]:
         return UploadOrigDatablock
 
 
 class UploadOrigDatablock(BaseModel):
-    dataFileList: List[UploadDataFile]
+    dataFileList: list[UploadDataFile]
     datasetId: PID
-    ownerGroup: str
     size: NonNegativeInt
-    accessGroups: Optional[List[str]] = None
-    chkAlg: Optional[str] = None
-    instrumentGroup: Optional[str] = None
+    accessGroups: list[str] | None = None
+    chkAlg: str | None = None
+    instrumentGroup: str | None = None
+    ownerGroup: str | None = None
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadOrigDatablock]:
+    def download_model_type(cls) -> type[DownloadOrigDatablock]:
         return DownloadOrigDatablock
 
 
 class DownloadDatablock(BaseModel):
-    archiveId: Optional[str] = None
-    dataFileList: Optional[List[DownloadDataFile]] = None
-    packedSize: Optional[NonNegativeInt] = None
-    size: Optional[NonNegativeInt] = None
-    version: Optional[str] = None
-    id: Optional[str] = pydantic.Field(alias="_id", default=None)
-    accessGroups: Optional[List[str]] = None
-    chkAlg: Optional[str] = None
-    createdAt: Optional[datetime] = None
-    createdBy: Optional[str] = None
-    datasetId: Optional[PID] = None
-    instrumentGroup: Optional[str] = None
-    ownerGroup: Optional[str] = None
-    updatedAt: Optional[datetime] = None
-    updatedBy: Optional[str] = None
+    archiveId: str | None = None
+    dataFileList: list[DownloadDataFile] | None = None
+    packedSize: NonNegativeInt | None = None
+    size: NonNegativeInt | None = None
+    version: str | None = None
+    id: str | None = pydantic.Field(alias="_id", default=None)
+    accessGroups: list[str] | None = None
+    chkAlg: str | None = None
+    createdAt: datetime | None = None
+    createdBy: str | None = None
+    datasetId: PID | None = None
+    instrumentGroup: str | None = None
+    isPublished: bool | None = None
+    ownerGroup: str | None = None
+    updatedAt: datetime | None = None
+    updatedBy: str | None = None
 
-    @field_validator("createdAt", "updatedAt", mode="before")
+    @pydantic.field_validator("createdAt", "updatedAt", mode="before")
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadDatablock]:
+    def upload_model_type(cls) -> type[UploadDatablock]:
         return UploadDatablock
 
 
 class UploadDatablock(BaseModel):
     archiveId: str
-    dataFileList: List[UploadDataFile]
+    dataFileList: list[UploadDataFile]
     packedSize: NonNegativeInt
     size: NonNegativeInt
     version: str
-    chkAlg: Optional[str] = None
+    chkAlg: str | None = None
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadDatablock]:
+    def download_model_type(cls) -> type[DownloadDatablock]:
         return DownloadDatablock
 
 
 class DownloadLifecycle(BaseModel):
-    archivable: Optional[bool] = None
-    archiveRetentionTime: Optional[datetime] = None
-    archiveReturnMessage: Optional[Dict[str, Any]] = None
-    archiveStatusMessage: Optional[str] = None
-    dateOfDiskPurging: Optional[datetime] = None
-    dateOfPublishing: Optional[datetime] = None
-    exportedTo: Optional[str] = None
-    isOnCentralDisk: Optional[bool] = None
-    publishable: Optional[bool] = None
-    publishedOn: Optional[datetime] = None
-    retrievable: Optional[bool] = None
-    retrieveIntegrityCheck: Optional[bool] = None
-    retrieveReturnMessage: Optional[Dict[str, Any]] = None
-    retrieveStatusMessage: Optional[str] = None
+    archivable: bool | None = None
+    archiveRetentionTime: datetime | None = None
+    archiveReturnMessage: dict[str, Any] | None = None
+    archiveStatusMessage: str | None = None
+    dateOfDiskPurging: datetime | None = None
+    dateOfPublishing: datetime | None = None
+    exportedTo: str | None = None
+    isOnCentralDisk: bool | None = None
+    publishable: bool | None = None
+    publishedOn: datetime | None = None
+    retrievable: bool | None = None
+    retrieveIntegrityCheck: bool | None = None
+    retrieveReturnMessage: dict[str, Any] | None = None
+    retrieveStatusMessage: str | None = None
 
-    @field_validator(
+    @pydantic.field_validator(
         "archiveRetentionTime",
         "dateOfDiskPurging",
         "dateOfPublishing",
         "publishedOn",
         mode="before",
     )
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
     @classmethod
-    def user_model_type(cls) -> Type[Lifecycle]:
+    def user_model_type(cls) -> type[Lifecycle]:
         return Lifecycle
 
 
 class DownloadTechnique(BaseModel):
-    name: Optional[str] = None
-    pid: Optional[str] = None
+    name: str | None = None
+    pid: str | None = None
 
     @classmethod
-    def user_model_type(cls) -> Type[Technique]:
+    def user_model_type(cls) -> type[Technique]:
         return Technique
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadTechnique]:
+    def upload_model_type(cls) -> type[UploadTechnique]:
         return UploadTechnique
 
 
 class UploadTechnique(BaseModel):
     name: str
     pid: str
 
     @classmethod
-    def user_model_type(cls) -> Type[Technique]:
+    def user_model_type(cls) -> type[Technique]:
         return Technique
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadTechnique]:
+    def download_model_type(cls) -> type[DownloadTechnique]:
         return DownloadTechnique
 
 
 class DownloadRelationship(BaseModel):
-    pid: Optional[PID] = None
-    relationship: Optional[str] = None
+    pid: PID | None = None
+    relationship: str | None = None
 
     @classmethod
-    def user_model_type(cls) -> Type[Relationship]:
+    def user_model_type(cls) -> type[Relationship]:
         return Relationship
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadRelationship]:
+    def upload_model_type(cls) -> type[UploadRelationship]:
         return UploadRelationship
 
 
 class UploadRelationship(BaseModel):
     pid: PID
     relationship: str
 
     @classmethod
-    def user_model_type(cls) -> Type[Relationship]:
+    def user_model_type(cls) -> type[Relationship]:
         return Relationship
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadRelationship]:
+    def download_model_type(cls) -> type[DownloadRelationship]:
         return DownloadRelationship
 
 
 class DownloadHistory(BaseModel):
-    id: Optional[str] = pydantic.Field(alias="_id", default=None)
-    updatedAt: Optional[datetime] = None
-    updatedBy: Optional[datetime] = None
+    id: str | None = pydantic.Field(alias="_id", default=None)
+    updatedAt: datetime | None = None
+    updatedBy: datetime | None = None
 
-    @field_validator("updatedAt", mode="before")
+    @pydantic.field_validator("updatedAt", mode="before")
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
     @classmethod
-    def user_model_type(cls) -> Type[History]:
+    def user_model_type(cls) -> type[History]:
         return History
 
 
 class DownloadDataFile(BaseModel):
-    path: Optional[str] = None
-    size: Optional[NonNegativeInt] = None
-    time: Optional[datetime] = None
-    chk: Optional[str] = None
-    gid: Optional[str] = None
-    perm: Optional[str] = None
-    uid: Optional[str] = None
+    path: str | None = None
+    size: NonNegativeInt | None = None
+    time: datetime | None = None
+    chk: str | None = None
+    gid: str | None = None
+    perm: str | None = None
+    uid: str | None = None
 
-    @field_validator("time", mode="before")
+    @pydantic.field_validator("time", mode="before")
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadDataFile]:
+    def upload_model_type(cls) -> type[UploadDataFile]:
         return UploadDataFile
 
 
 class UploadDataFile(BaseModel):
     path: str
     size: NonNegativeInt
     time: datetime
-    chk: Optional[str] = None
-    gid: Optional[str] = None
-    perm: Optional[str] = None
-    uid: Optional[str] = None
+    chk: str | None = None
+    gid: str | None = None
+    perm: str | None = None
+    uid: str | None = None
 
-    @field_validator("time", mode="before")
+    @pydantic.field_validator("time", mode="before")
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadDataFile]:
+    def download_model_type(cls) -> type[DownloadDataFile]:
         return DownloadDataFile
 
 
 class DownloadInstrument(BaseModel):
-    customMetadata: Optional[Dict[str, Any]] = None
-    name: Optional[str] = None
-    pid: Optional[str] = None
-    uniqueName: Optional[str] = None
+    customMetadata: dict[str, Any] | None = None
+    name: str | None = None
+    pid: str | None = None
+    uniqueName: str | None = None
 
     @classmethod
-    def user_model_type(cls) -> Type[Instrument]:
+    def user_model_type(cls) -> type[Instrument]:
         return Instrument
 
 
 class DownloadSample(BaseModel):
-    ownerGroup: Optional[str] = None
-    accessGroups: Optional[List[str]] = None
-    createdAt: Optional[datetime] = None
-    createdBy: Optional[str] = None
-    description: Optional[str] = None
-    instrumentGroup: Optional[str] = None
-    isPublished: Optional[bool] = None
-    owner: Optional[str] = None
-    sampleCharacteristics: Optional[Dict[str, Any]] = None
-    sampleId: Optional[str] = None
-    updatedAt: Optional[datetime] = None
-    updatedBy: Optional[str] = None
+    ownerGroup: str | None = None
+    accessGroups: list[str] | None = None
+    createdAt: datetime | None = None
+    createdBy: str | None = None
+    description: str | None = None
+    instrumentGroup: str | None = None
+    isPublished: bool | None = None
+    owner: str | None = None
+    sampleCharacteristics: dict[str, Any] | None = None
+    sampleId: str | None = None
+    updatedAt: datetime | None = None
+    updatedBy: str | None = None
 
-    @field_validator("createdAt", "updatedAt", mode="before")
+    @pydantic.field_validator("createdAt", "updatedAt", mode="before")
     def _validate_datetime(cls, value: Any) -> Any:
         return validate_datetime(value)
 
     @classmethod
-    def user_model_type(cls) -> Type[Sample]:
+    def user_model_type(cls) -> type[Sample]:
         return Sample
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadSample]:
+    def upload_model_type(cls) -> type[UploadSample]:
         return UploadSample
 
 
 class UploadSample(BaseModel):
     ownerGroup: str
-    accessGroups: Optional[List[str]] = None
-    description: Optional[str] = None
-    instrumentGroup: Optional[str] = None
-    isPublished: Optional[bool] = None
-    owner: Optional[str] = None
-    sampleCharacteristics: Optional[Dict[str, Any]] = None
-    sampleId: Optional[str] = None
+    accessGroups: list[str] | None = None
+    description: str | None = None
+    instrumentGroup: str | None = None
+    isPublished: bool | None = None
+    owner: str | None = None
+    sampleCharacteristics: dict[str, Any] | None = None
+    sampleId: str | None = None
 
     @classmethod
-    def user_model_type(cls) -> Type[Sample]:
+    def user_model_type(cls) -> type[Sample]:
         return Sample
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadSample]:
+    def download_model_type(cls) -> type[DownloadSample]:
         return DownloadSample
 
 
 @dataclass_optional_args(kw_only=True, slots=True)
 class Attachment(BaseUserModel):
     caption: str
     owner_group: str
-    access_groups: Optional[List[str]] = None
-    dataset_id: Optional[PID] = None
-    id: Optional[str] = None
-    instrument_group: Optional[str] = None
-    proposal_id: Optional[str] = None
-    sample_id: Optional[str] = None
-    thumbnail: Optional[Thumbnail] = None
-    _created_at: Optional[datetime] = None
-    _created_by: Optional[str] = None
-    _updated_at: Optional[datetime] = None
-    _updated_by: Optional[str] = None
+    access_groups: list[str] | None = None
+    dataset_id: PID | None = None
+    id: str | None = None
+    instrument_group: str | None = None
+    proposal_id: str | None = None
+    sample_id: str | None = None
+    thumbnail: Thumbnail | None = None
+    _created_at: datetime | None = None
+    _created_by: str | None = None
+    _is_published: bool | None = None
+    _updated_at: datetime | None = None
+    _updated_by: str | None = None
 
     @property
-    def created_at(self) -> Optional[datetime]:
+    def created_at(self) -> datetime | None:
         return self._created_at
 
     @property
-    def created_by(self) -> Optional[str]:
+    def created_by(self) -> str | None:
         return self._created_by
 
     @property
-    def updated_at(self) -> Optional[datetime]:
+    def is_published(self) -> bool | None:
+        return self._is_published
+
+    @property
+    def updated_at(self) -> datetime | None:
         return self._updated_at
 
     @property
-    def updated_by(self) -> Optional[str]:
+    def updated_by(self) -> str | None:
         return self._updated_by
 
     @classmethod
     def from_download_model(cls, download_model: DownloadAttachment) -> Attachment:
         """Construct an instance from an associated SciCat download model."""
         return cls(**cls._download_model_dict(download_model))
 
     def make_upload_model(self) -> UploadAttachment:
         """Construct a SciCat upload model from self."""
         return UploadAttachment(**self._upload_model_dict())
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadAttachment]:
+    def upload_model_type(cls) -> type[UploadAttachment]:
         return UploadAttachment
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadAttachment]:
+    def download_model_type(cls) -> type[DownloadAttachment]:
         return DownloadAttachment
 
 
 @dataclass_optional_args(kw_only=True, slots=True)
 class Lifecycle(BaseUserModel):
-    _archivable: Optional[bool] = None
-    _archive_retention_time: Optional[datetime] = None
-    _archive_return_message: Optional[Dict[str, Any]] = None
-    _archive_status_message: Optional[str] = None
-    _date_of_disk_purging: Optional[datetime] = None
-    _date_of_publishing: Optional[datetime] = None
-    _exported_to: Optional[str] = None
-    _is_on_central_disk: Optional[bool] = None
-    _publishable: Optional[bool] = None
-    _published_on: Optional[datetime] = None
-    _retrievable: Optional[bool] = None
-    _retrieve_integrity_check: Optional[bool] = None
-    _retrieve_return_message: Optional[Dict[str, Any]] = None
-    _retrieve_status_message: Optional[str] = None
+    _archivable: bool | None = None
+    _archive_retention_time: datetime | None = None
+    _archive_return_message: dict[str, Any] | None = None
+    _archive_status_message: str | None = None
+    _date_of_disk_purging: datetime | None = None
+    _date_of_publishing: datetime | None = None
+    _exported_to: str | None = None
+    _is_on_central_disk: bool | None = None
+    _publishable: bool | None = None
+    _published_on: datetime | None = None
+    _retrievable: bool | None = None
+    _retrieve_integrity_check: bool | None = None
+    _retrieve_return_message: dict[str, Any] | None = None
+    _retrieve_status_message: str | None = None
 
     @property
-    def archivable(self) -> Optional[bool]:
+    def archivable(self) -> bool | None:
         return self._archivable
 
     @property
-    def archive_retention_time(self) -> Optional[datetime]:
+    def archive_retention_time(self) -> datetime | None:
         return self._archive_retention_time
 
     @property
-    def archive_return_message(self) -> Optional[Dict[str, Any]]:
+    def archive_return_message(self) -> dict[str, Any] | None:
         return self._archive_return_message
 
     @property
-    def archive_status_message(self) -> Optional[str]:
+    def archive_status_message(self) -> str | None:
         return self._archive_status_message
 
     @property
-    def date_of_disk_purging(self) -> Optional[datetime]:
+    def date_of_disk_purging(self) -> datetime | None:
         return self._date_of_disk_purging
 
     @property
-    def date_of_publishing(self) -> Optional[datetime]:
+    def date_of_publishing(self) -> datetime | None:
         return self._date_of_publishing
 
     @property
-    def exported_to(self) -> Optional[str]:
+    def exported_to(self) -> str | None:
         return self._exported_to
 
     @property
-    def is_on_central_disk(self) -> Optional[bool]:
+    def is_on_central_disk(self) -> bool | None:
         return self._is_on_central_disk
 
     @property
-    def publishable(self) -> Optional[bool]:
+    def publishable(self) -> bool | None:
         return self._publishable
 
     @property
-    def published_on(self) -> Optional[datetime]:
+    def published_on(self) -> datetime | None:
         return self._published_on
 
     @property
-    def retrievable(self) -> Optional[bool]:
+    def retrievable(self) -> bool | None:
         return self._retrievable
 
     @property
-    def retrieve_integrity_check(self) -> Optional[bool]:
+    def retrieve_integrity_check(self) -> bool | None:
         return self._retrieve_integrity_check
 
     @property
-    def retrieve_return_message(self) -> Optional[Dict[str, Any]]:
+    def retrieve_return_message(self) -> dict[str, Any] | None:
         return self._retrieve_return_message
 
     @property
-    def retrieve_status_message(self) -> Optional[str]:
+    def retrieve_status_message(self) -> str | None:
         return self._retrieve_status_message
 
     @classmethod
     def from_download_model(cls, download_model: DownloadLifecycle) -> Lifecycle:
         """Construct an instance from an associated SciCat download model."""
         return cls(**cls._download_model_dict(download_model))
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadLifecycle]:
+    def download_model_type(cls) -> type[DownloadLifecycle]:
         return DownloadLifecycle
 
 
 @dataclass_optional_args(kw_only=True, slots=True)
 class Technique(BaseUserModel):
     name: str
     pid: str
@@ -728,19 +737,19 @@
         return cls(**cls._download_model_dict(download_model))
 
     def make_upload_model(self) -> UploadTechnique:
         """Construct a SciCat upload model from self."""
         return UploadTechnique(**self._upload_model_dict())
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadTechnique]:
+    def upload_model_type(cls) -> type[UploadTechnique]:
         return UploadTechnique
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadTechnique]:
+    def download_model_type(cls) -> type[DownloadTechnique]:
         return DownloadTechnique
 
 
 @dataclass_optional_args(kw_only=True, slots=True)
 class Relationship(BaseUserModel):
     pid: PID
     relationship: str
@@ -751,129 +760,129 @@
         return cls(**cls._download_model_dict(download_model))
 
     def make_upload_model(self) -> UploadRelationship:
         """Construct a SciCat upload model from self."""
         return UploadRelationship(**self._upload_model_dict())
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadRelationship]:
+    def upload_model_type(cls) -> type[UploadRelationship]:
         return UploadRelationship
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadRelationship]:
+    def download_model_type(cls) -> type[DownloadRelationship]:
         return DownloadRelationship
 
 
 @dataclass_optional_args(kw_only=True, slots=True)
 class History(BaseUserModel):
-    __id: Optional[str] = None
-    _updated_at: Optional[datetime] = None
-    _updated_by: Optional[datetime] = None
+    __id: str | None = None
+    _updated_at: datetime | None = None
+    _updated_by: datetime | None = None
 
     @property
-    def _id(self) -> Optional[str]:
+    def _id(self) -> str | None:
         return self.__id
 
     @property
-    def updated_at(self) -> Optional[datetime]:
+    def updated_at(self) -> datetime | None:
         return self._updated_at
 
     @property
-    def updated_by(self) -> Optional[datetime]:
+    def updated_by(self) -> datetime | None:
         return self._updated_by
 
     @classmethod
     def from_download_model(cls, download_model: DownloadHistory) -> History:
         """Construct an instance from an associated SciCat download model."""
         return cls(**cls._download_model_dict(download_model))
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadHistory]:
+    def download_model_type(cls) -> type[DownloadHistory]:
         return DownloadHistory
 
 
 @dataclass_optional_args(kw_only=True, slots=True)
 class Instrument(BaseUserModel):
-    _custom_metadata: Optional[Dict[str, Any]] = None
-    _name: Optional[str] = None
-    _pid: Optional[str] = None
-    _unique_name: Optional[str] = None
+    _custom_metadata: dict[str, Any] | None = None
+    _name: str | None = None
+    _pid: str | None = None
+    _unique_name: str | None = None
 
     @property
-    def custom_metadata(self) -> Optional[Dict[str, Any]]:
+    def custom_metadata(self) -> dict[str, Any] | None:
         return self._custom_metadata
 
     @property
-    def name(self) -> Optional[str]:
+    def name(self) -> str | None:
         return self._name
 
     @property
-    def pid(self) -> Optional[str]:
+    def pid(self) -> str | None:
         return self._pid
 
     @property
-    def unique_name(self) -> Optional[str]:
+    def unique_name(self) -> str | None:
         return self._unique_name
 
     @classmethod
     def from_download_model(cls, download_model: DownloadInstrument) -> Instrument:
         """Construct an instance from an associated SciCat download model."""
         return cls(**cls._download_model_dict(download_model))
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadInstrument]:
+    def download_model_type(cls) -> type[DownloadInstrument]:
         return DownloadInstrument
 
 
 @dataclass_optional_args(kw_only=True, slots=True)
 class Sample(BaseUserModel):
     owner_group: str
-    access_groups: Optional[List[str]] = None
-    description: Optional[str] = None
-    instrument_group: Optional[str] = None
-    is_published: Optional[bool] = None
-    owner: Optional[str] = None
-    sample_characteristics: Optional[Dict[str, Any]] = None
-    sample_id: Optional[str] = None
-    _created_at: Optional[datetime] = None
-    _created_by: Optional[str] = None
-    _updated_at: Optional[datetime] = None
-    _updated_by: Optional[str] = None
+    access_groups: list[str] | None = None
+    description: str | None = None
+    instrument_group: str | None = None
+    is_published: bool | None = None
+    owner: str | None = None
+    sample_characteristics: dict[str, Any] | None = None
+    sample_id: str | None = None
+    _created_at: datetime | None = None
+    _created_by: str | None = None
+    _updated_at: datetime | None = None
+    _updated_by: str | None = None
 
     @property
-    def created_at(self) -> Optional[datetime]:
+    def created_at(self) -> datetime | None:
         return self._created_at
 
     @property
-    def created_by(self) -> Optional[str]:
+    def created_by(self) -> str | None:
         return self._created_by
 
     @property
-    def updated_at(self) -> Optional[datetime]:
+    def updated_at(self) -> datetime | None:
         return self._updated_at
 
     @property
-    def updated_by(self) -> Optional[str]:
+    def updated_by(self) -> str | None:
         return self._updated_by
 
     @classmethod
     def from_download_model(cls, download_model: DownloadSample) -> Sample:
         """Construct an instance from an associated SciCat download model."""
         return cls(**cls._download_model_dict(download_model))
 
     def make_upload_model(self) -> UploadSample:
         """Construct a SciCat upload model from self."""
         return UploadSample(**self._upload_model_dict())
 
     @classmethod
-    def upload_model_type(cls) -> Type[UploadSample]:
+    def upload_model_type(cls) -> type[UploadSample]:
         return UploadSample
 
     @classmethod
-    def download_model_type(cls) -> Type[DownloadSample]:
+    def download_model_type(cls) -> type[DownloadSample]:
         return DownloadSample
 
 
 # Some models contain fields that are other models which are defined
 # further down in the file.
 # Instead of ordering models according to their dependencies, resolve
 # references once all classes have been defined.
```

### Comparing `scitacean-23.8.0/src/scitacean/pid.py` & `scitacean-24.4.0/src/scitacean/pid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,56 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
+"""Helper type for handling persistent identifiers."""
+
 from __future__ import annotations
 
 import uuid
-from typing import Callable, Generator, Optional, Union
-
-import pydantic
-
-from ._internal.pydantic_compat import is_pydantic_v1
-
-if not is_pydantic_v1():
-    from typing import Any, Type
+from typing import Any
 
-    from pydantic import GetCoreSchemaHandler
-    from pydantic_core import core_schema
-
-    def _get_pid_core_schema(
-        cls: Type[PID], _source_type: Any, _handler: GetCoreSchemaHandler
-    ) -> core_schema.CoreSchema:
-        return core_schema.no_info_after_validator_function(
-            cls.parse,
-            core_schema.union_schema(
-                [core_schema.is_instance_schema(PID), core_schema.str_schema()]
-            ),
-            serialization=core_schema.plain_serializer_function_ser_schema(
-                cls.__str__, info_arg=False, return_schema=core_schema.str_schema()
-            ),
-        )
+from pydantic import GetCoreSchemaHandler, ValidationError
+from pydantic_core import core_schema
 
 
 class PID:
-    """Stores the ID of database item.
+    """Stores the persistent identifier of a database item.
 
     The ID is split into a prefix and the main identifier.
     The prefix identifies an instance of SciCat and the main identifier a dataset.
 
     The two components are merged using a "/", i.e.
 
     .. code-block:: python
 
-        full_id = PID.prefix + '/' + PID.pid
+        full_id = PID.prefix + "/" + PID.pid
 
     Equivalently, ``str`` can be used to construct the full id:
 
     .. code-block:: python
 
         full_id = str(PID)
     """
 
     __slots__ = ("_pid", "_prefix")
 
-    def __init__(self, *, pid: str, prefix: Optional[str] = None):
+    def __init__(self, *, pid: str, prefix: str | None = None):
         """Initialize an instance from individual components.
 
         Parameters
         ----------
         pid:
             Main part of the ID which uniquely identifies a dataset.
         prefix:
             Identifies the instance of SciCat.
         """
         self._pid = pid
         self._prefix = prefix
 
     @classmethod
-    def parse(cls, x: Union[str, PID]) -> PID:
+    def parse(cls, x: str | PID) -> PID:
         """Build a PID from a string.
 
         The string is split at the first "/" to determine
         prefix and main ID.
         This means that it only works if the prefix and main ID do
         not contain any slashes.
 
@@ -87,15 +69,15 @@
             return PID(pid=x.pid, prefix=x.prefix)
         pieces = x.split("/", 1)
         if len(pieces) == 1:
             return PID(pid=pieces[0], prefix=None)
         return PID(prefix=pieces[0], pid=pieces[1])
 
     @classmethod
-    def generate(cls, *, prefix: Optional[str] = None) -> PID:
+    def generate(cls, *, prefix: str | None = None) -> PID:
         """Create a new unique PID.
 
         Uses UUID4 to generate the ID.
 
         Parameters
         ----------
         prefix:
@@ -110,15 +92,15 @@
 
     @property
     def pid(self) -> str:
         """Main part of the ID."""
         return self._pid
 
     @property
-    def prefix(self) -> Optional[str]:
+    def prefix(self) -> str | None:
         """Prefix part of the ID if there is one."""
         return self._prefix
 
     @property
     def without_prefix(self) -> PID:
         """Return a new PID with the prefix set to None."""
         return PID(pid=self.pid, prefix=None)
@@ -136,25 +118,28 @@
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, PID):
             return False
         return self.prefix == other.prefix and self.pid == other.pid
 
     @classmethod
-    def validate(cls, value: Union[str, PID]) -> PID:
+    def validate(cls, value: str | PID) -> PID:
         """Pydantic validator for PID fields."""
         if isinstance(value, str):
             return PID.parse(value)
         if isinstance(value, PID):
             return value
-        raise pydantic.ValidationError("expected a PID or str")
-
-    if is_pydantic_v1():
+        raise ValidationError("expected a PID or str")
 
-        @classmethod
-        def __get_validators__(
-            cls,
-        ) -> Generator[Callable[[Union[str, PID]], PID], None, None]:
-            yield cls.validate
-
-    else:
-        __get_pydantic_core_schema__ = classmethod(_get_pid_core_schema)
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, _source_type: Any, _handler: GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
+        return core_schema.no_info_after_validator_function(
+            cls.parse,
+            core_schema.union_schema(
+                [core_schema.is_instance_schema(PID), core_schema.str_schema()]
+            ),
+            serialization=core_schema.plain_serializer_function_ser_schema(
+                cls.__str__, info_arg=False, return_schema=core_schema.str_schema()
+            ),
+        )
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/_pytest_helpers.py` & `scitacean-24.4.0/src/scitacean/testing/_pytest_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 from pathlib import Path
-from typing import Optional, Tuple, Union
 
 import pytest
 
 from .._internal.file_counter import FileCounter, NullCounter
 
 
 def using_xdist(request: pytest.FixtureRequest) -> bool:
@@ -26,27 +25,27 @@
         return tmp_path_factory.getbasetemp().parent
     return tmp_path_factory.getbasetemp()
 
 
 def init_pytest_work_dir(
     request: pytest.FixtureRequest,
     tmp_path_factory: pytest.TempPathFactory,
-    name: Optional[str],
-) -> Tuple[Path, Union[FileCounter, NullCounter]]:
+    name: str | None,
+) -> tuple[Path, FileCounter | NullCounter]:
     """Create a working directory and initialize an atomic counter and lock for it."""
     return init_work_dir(request, root_tmp_dir(request, tmp_path_factory), name)
 
 
 def init_work_dir(
-    request: pytest.FixtureRequest, base_path: Path, name: Optional[str]
-) -> Tuple[Path, Union[FileCounter, NullCounter]]:
+    request: pytest.FixtureRequest, base_path: Path, name: str | None
+) -> tuple[Path, FileCounter | NullCounter]:
     """Create a working directory and initialize an atomic counter and lock for it."""
     target_dir = base_path / name if name else base_path
     target_dir.mkdir(exist_ok=True)
 
-    counter: Union[FileCounter, NullCounter]
+    counter: FileCounter | NullCounter
     if using_xdist(request):
         counter = FileCounter(target_dir / "counter")
     else:
         counter = NullCounter()
 
     return target_dir, counter
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/backend/__init__.py` & `scitacean-24.4.0/src/scitacean/testing/backend/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Utilities for running tests against a locally deployed SciCat backend.
 
 This subpackage provides tools for using a real SciCat backend running in docker
 containers on the local machine.
 It, therefore, requires docker to be installed and running.
 The package is in particular intended to be used with
 `pytest <https://docs.pytest.org>`_ and the fixtures provided by the
@@ -59,36 +59,33 @@
 .. rubric:: Functions
 
 .. autosummary::
    :toctree: ../functions
 
    add_pytest_option
    backend_enabled
-   can_connect
    configure
    skip_if_not_backend
    start_backend
    stop_backend
    wait_until_backend_is_live
 """
 
 from . import config, seed
 from ._backend import (
-    can_connect,
     configure,
     start_backend,
     stop_backend,
     wait_until_backend_is_live,
 )
 from ._pytest_helpers import add_pytest_option, backend_enabled, skip_if_not_backend
 
 __all__ = [
     "add_pytest_option",
     "backend_enabled",
-    "can_connect",
     "config",
     "configure",
     "seed",
     "skip_if_not_backend",
     "start_backend",
     "stop_backend",
     "wait_until_backend_is_live",
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/backend/_backend.py` & `scitacean-24.4.0/src/scitacean/testing/backend/_backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 import importlib.resources
 import os
 import time
 from copy import deepcopy
-from typing import Any, Dict, Union
+from pathlib import Path
+from typing import Any
 from urllib.parse import urljoin
 
 import requests
 import yaml
 
 from ..._internal.docker import docker_compose_down, docker_compose_up
 from . import config
 
-_PathLike = Union[str, os.PathLike]
+_PathLike = str | os.PathLike[str]
 
 
 def _read_yaml(filename: str) -> Any:
-    if hasattr(importlib.resources, "files"):
-        # Use new API added in Python 3.9
-        return yaml.safe_load(
-            importlib.resources.files("scitacean.testing.backend")
-            .joinpath(filename)
-            .read_text()
-        )
-    # Old API, deprecated as of Python 3.11
     return yaml.safe_load(
-        importlib.resources.read_text("scitacean.testing.backend", filename)
+        importlib.resources.files("scitacean.testing.backend")
+        .joinpath(filename)
+        .read_text()
     )
 
 
-def _docker_compose_template() -> Dict[str, Any]:
+def _docker_compose_template() -> dict[str, Any]:
     template = _read_yaml("docker-compose-backend-template.yaml")
     return template  # type: ignore[no-any-return]
 
 
-def _apply_config(template: Dict[str, Any]) -> Dict[str, Any]:
+def _apply_config(
+    template: dict[str, Any], account_config_path: Path
+) -> dict[str, Any]:
     res = deepcopy(template)
     scicat = res["services"]["scicat"]
     ports = scicat["ports"][0].split(":")
     scicat["ports"] = [f"{ports[0]}:{config.SCICAT_PORT}"]
 
     env = scicat["environment"]
     env["PORT"] = config.SCICAT_PORT
     env["PID_PREFIX"] = config.PID_PREFIX
     env["SITE"] = config.SITE
 
+    scicat["volumes"] = [
+        f"{account_config_path}:/home/node/app/functionalAccounts.json",
+    ]
+
     return res
 
 
 def configure(target_path: _PathLike) -> None:
     """Build a docker-compose file for the testing backend.
 
     Parameters
     ----------
     target_path:
         Generate a docker-compose file at this path.
     """
-    c = yaml.dump(_apply_config(_docker_compose_template()))
+    account_config_path = Path(target_path).parent / "functionalAccounts.json"
+    config.dump_account_config(account_config_path)
+    c = yaml.dump(_apply_config(_docker_compose_template(), account_config_path))
     if "PLACEHOLDER" in c:
         raise RuntimeError("Incorrect config")
 
     with open(target_path, "w") as f:
         f.write(c)
 
 
@@ -71,32 +74,35 @@
 
 
 def stop_backend(docker_compose_file: _PathLike) -> None:
     """Stop the docker container with SciCat backend and remove volumes."""
     docker_compose_down(docker_compose_file)
 
 
-def can_connect() -> bool:
+def _can_connect() -> tuple[bool, str]:
     """Test the connection to the testing SciCat backend.
 
     Returns
     -------
     :
-        True if the backend is reachable, False otherwise.
+        The first element indicates whether the connection was successful.
+        The second element is an error message.
     """
     scicat_access = config.local_access("user1")
     try:
         response = requests.post(
             urljoin(scicat_access.url, "Users/login"),
             json=scicat_access.user.credentials,
             timeout=0.5,
         )
-    except requests.ConnectionError:
-        return False
-    return response.ok
+    except requests.ConnectionError as err:
+        return False, str(err)
+    if response.ok:
+        return True, ""
+    return False, str(f"{response}: {response.text}")
 
 
 def wait_until_backend_is_live(max_time: float, n_tries: int) -> None:
     """Sleep until a connection to the backend can be made.
 
     The backend takes a few seconds to become usable after the
     docker container was started.
@@ -112,12 +118,13 @@
 
     Raises
     ------
     RuntimeError
         If no connection can be made within the time limit.
     """
     for _ in range(n_tries):
-        if can_connect():
+        if _can_connect()[0]:
             return
         time.sleep(max_time / n_tries)
-    if not can_connect():
-        raise RuntimeError("Cannot connect to backend")
+    ok, err = _can_connect()
+    if not ok:
+        raise RuntimeError(f"Cannot connect to backend: {err}")
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/backend/_pytest_helpers.py` & `scitacean-24.4.0/src/scitacean/testing/backend/_pytest_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
-from typing import Optional
 
 import pytest
 
-_COMMAND_LINE_OPTION: Optional[str] = None
+_COMMAND_LINE_OPTION: str | None = None
 
 
 def add_pytest_option(parser: pytest.Parser, option: str = "--backend-tests") -> None:
     """Add a command-line option to pytest to toggle backend tests.
 
     Parameters
     ----------
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/backend/config.py` & `scitacean-24.4.0/src/scitacean/testing/backend/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Backend configuration."""
 
+import json
 from dataclasses import dataclass
-from typing import Dict
+from pathlib import Path
 
 
 @dataclass
 class SciCatUser:
     """A SciCat user.
 
     Warning
@@ -19,28 +20,38 @@
 
     username: str
     password: str
     email: str
     group: str
 
     @property
-    def credentials(self) -> Dict[str, str]:
+    def credentials(self) -> dict[str, str]:
         """Return login credentials for this user.
 
         User as
 
         .. code-block:: python
 
             client = Client.from_credentials(url="...", **user.credentials)
         """
         return {
             "username": self.username,
             "password": self.password,
         }
 
+    def dump(self) -> dict[str, str | bool]:
+        """Return a dict that can be serialized to functionalAccounts.json."""
+        return {
+            "username": self.username,
+            "password": self.password,
+            "email": self.email,
+            "role": self.group,
+            "global": False,
+        }
+
 
 # see https://github.com/SciCatProject/scicat-backend-next/blob/master/src/config/configuration.ts
 USERS = {
     "ingestor": SciCatUser(
         username="ingestor",
         password="aman",  # noqa: S106
         email="scicatingestor@your.site",
@@ -112,7 +123,13 @@
 
     Returns
     -------
     :
         Parameters for the local SciCat backend.
     """
     return SciCatAccess(url=f"http://localhost:{SCICAT_PORT}/api/v3/", user=USERS[user])
+
+
+def dump_account_config(path: Path) -> None:
+    """Write a functional account config for the backend."""
+    with path.open("w") as f:
+        json.dump([user.dump() for user in USERS.values()], f)
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/backend/docker-compose-backend-template.yaml` & `scitacean-24.4.0/src/scitacean/testing/backend/docker-compose-backend-template.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -7,37 +7,32 @@
 # https://github.com/SciCatProject/scicat-backend-next/pkgs/container/backend-next/97880429?tag=stable
 #
 # See https://scicatproject.github.io/documentation/Development/v4.x/backend/configuration.html
 # for a list of all env variables.
 
 services:
   mongodb:
-    image: bitnami/mongodb:4.2
-    volumes:
-      - mongodb_data:/bitnami
+    image: mongo:latest
     ports:
       - "27017:27017"
 
   scicat:
     image: ghcr.io/scicatproject/backend-next:stable
     container_name: scitacean-test-scicat
     depends_on:
       - mongodb
     ports:
       - 3000:PLACEHOLDER
     environment:
       DOI_PREFIX: DOI.SAMPLE.PREFIX
+      ELASTICSEARCH_ENABLED: no
       HTTP_MAX_REDIRECTS: 1  # Scitacean should not require redirects
       HTTP_TIMEOUT: 5000  # in ms
       JWT_EXPIRES_IN: 3600  # in s (expiry of token)
       JWT_SECRET: a_scicat_secret
       LOGBOOK_ENABLED: no  # we don't test these endpoints
       MONGODB_URI: mongodb://mongodb:27017/scicat
 
       # Those are configured in Python
       PID_PREFIX: PLACEHOLDER
       SITE: PLACEHOLDER
       PORT: PLACEHOLDER
-
-volumes:
-  mongodb_data:
-    driver: local
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/backend/fixtures.py` & `scitacean-24.4.0/src/scitacean/testing/backend/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # mypy: disable-error-code="no-untyped-def"
 """Pytest fixtures to manage and access a local SciCat backend."""
 
 import logging
+from collections.abc import Generator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Generator, Optional, Type, Union
 
 import pytest
 
 from ..._internal import docker
 from ..._internal.file_counter import FileCounter, NullCounter
 from ...client import Client
 from .._pytest_helpers import init_pytest_work_dir
@@ -69,15 +69,15 @@
             for a in seed.INITIAL_ATTACHMENTS.values()
         }
     )
     return client
 
 
 @pytest.fixture()
-def real_client(scicat_access: SciCatAccess, scicat_backend: bool) -> Optional[Client]:
+def real_client(scicat_access: SciCatAccess, scicat_backend: bool) -> Client | None:
     """Fixture that returns a real client if backend tests are enabled.
 
     Returns
     -------
     :
         If backend tests are enabled, a real client that is connected to
         the testing backend.
@@ -88,15 +88,15 @@
     return Client.from_credentials(
         url=scicat_access.url,
         **scicat_access.user.credentials,  # type: ignore[arg-type]
     )
 
 
 @pytest.fixture(params=["real", "fake"])
-def client(request, scicat_backend) -> Union[Client, FakeClient]:
+def client(request, scicat_backend) -> Client | FakeClient:
     """Fixture that returns a real and a fake client.
 
     Using this fixture makes tests run twice, once with a real client
     and once with a fake client.
     If backend tests are disabled, the test with a real client gets skipped.
 
     Returns
@@ -152,15 +152,15 @@
         ):
             yield True
 
 
 @contextmanager
 def _prepare_without_backend(
     scicat_access: SciCatAccess,
-    counter: Union[FileCounter, NullCounter],
+    counter: FileCounter | NullCounter,
     target_dir: Path,
 ) -> Generator[None, None, None]:
     with counter.increment() as count:
         if count == 1:
             _seed_database(
                 FakeClient, scicat_access=scicat_access, target_dir=target_dir
             )
@@ -168,15 +168,15 @@
             seed.seed_worker(target_dir)
     yield
 
 
 @contextmanager
 def _prepare_with_backend(
     scicat_access: SciCatAccess,
-    counter: Union[FileCounter, NullCounter],
+    counter: FileCounter | NullCounter,
     target_dir: Path,
 ) -> Generator[None, None, None]:
     try:
         with counter.increment() as count:
             if count == 1:
                 _backend_docker_up(target_dir)
                 _seed_database(
@@ -190,15 +190,15 @@
     finally:
         with counter.decrement() as count:
             if count == 0:
                 _backend_docker_down(target_dir)
 
 
 def _seed_database(
-    client_class: Union[Type[Client], Type[FakeClient]],
+    client_class: type[Client] | type[FakeClient],
     scicat_access: SciCatAccess,
     target_dir: Path,
 ) -> None:
     client = client_class.from_credentials(
         url=scicat_access.url,
         **scicat_access.user.credentials,  # type: ignore[arg-type]
     )
@@ -213,15 +213,15 @@
     log = logging.getLogger("scitacean.testing")
     log.info(
         "Starting docker container with SciCat backend from %s", docker_compose_file
     )
     configure(docker_compose_file)
     docker.docker_compose_up(docker_compose_file)
     log.info("Waiting for SciCat docker to become accessible")
-    wait_until_backend_is_live(max_time=20, n_tries=20)
+    wait_until_backend_is_live(max_time=60, n_tries=40)
     log.info("Successfully connected to SciCat backend")
 
 
 def _backend_docker_down(target_dir: Path) -> None:
     # Check if container is running because the fixture can call this function
     # if there was an exception in _backend_docker_up.
     # In that case, there is nothing to tear down.
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/backend/seed.py` & `scitacean-24.4.0/src/scitacean/testing/backend/seed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 """Initial contents of the SciCat testing backend.
 
 The contents of this module are used to initialize
 the local database before making it available to tests.
 """
 
 import pickle
 from copy import deepcopy
 from pathlib import Path
-from typing import Dict, List, Union
 
 from dateutil.parser import parse as parse_datetime
 
 from ... import model
 from ...client import Client
 from ...filesystem import RemotePath
 from ...model import (
@@ -30,15 +29,15 @@
     UploadTechnique,
 )
 from ...pid import PID
 from ...thumbnail import Thumbnail
 from .config import SITE, SciCatAccess, SciCatUser
 
 # Dataset models to upload to the database.
-_DATASETS: Dict[str, Union[UploadRawDataset, UploadDerivedDataset]] = {
+_DATASETS: dict[str, UploadRawDataset | UploadDerivedDataset] = {
     "raw": UploadRawDataset(
         ownerGroup="PLACEHOLDER",
         accessGroups=["uu", "faculty"],
         classification="IN=medium,AV=low,CO=low",
         contactEmail="ponder.stibbons@uu.am",
         creationTime=parse_datetime("2004-06-13T01:45:28.100Z"),
         datasetName="My darkest magic yet",
@@ -127,15 +126,15 @@
         investigator="who?!",
         inputDatasets=[],
         usedSoftware=["scitacean"],
     ),
 }
 
 # Orig datablocks to upload to the database.
-_ORIG_DATABLOCKS: Dict[str, List[UploadOrigDatablock]] = {
+_ORIG_DATABLOCKS: dict[str, list[UploadOrigDatablock]] = {
     "raw": [
         UploadOrigDatablock(
             datasetId=PID(pid="PLACEHOLDER"),
             ownerGroup="PLACEHOLDER",
             size=619,
             accessGroups=["uu", "faculty"],
             chkAlg="md5",
@@ -199,15 +198,15 @@
                     perm="0",
                 ),
             ],
         )
     ],
 }
 
-_ATTACHMENTS: Dict[str, List[UploadAttachment]] = {
+_ATTACHMENTS: dict[str, list[UploadAttachment]] = {
     "derived": [
         UploadAttachment(
             caption="Process Overview",
             ownerGroup="PLACEHOLDER",
             accessGroups=["uu"],
             datasetId=PID(pid="PLACEHOLDER"),
             thumbnail=Thumbnail(mime="image/png", data=b"nag;aso;i"),
@@ -219,24 +218,24 @@
             datasetId=PID(pid="PLACEHOLDER"),
             thumbnail=Thumbnail(mime="image/jpeg", data=b"gj0ajs93jka2jv89a"),
             sampleId="kjsdf",
         ),
     ]
 }
 
-INITIAL_DATASETS: Dict[str, DownloadDataset] = {}
+INITIAL_DATASETS: dict[str, DownloadDataset] = {}
 """Initial datasets in the testing database."""
-INITIAL_ORIG_DATABLOCKS: Dict[str, List[DownloadOrigDatablock]] = {}
+INITIAL_ORIG_DATABLOCKS: dict[str, list[DownloadOrigDatablock]] = {}
 """Initial orig datablocks in the testing database."""
-INITIAL_ATTACHMENTS: Dict[str, List[DownloadAttachment]] = {}
+INITIAL_ATTACHMENTS: dict[str, list[DownloadAttachment]] = {}
 
 
 def _apply_config_dataset(
-    dset: Union[UploadRawDataset, UploadDerivedDataset], user: SciCatUser
-) -> Union[UploadRawDataset, UploadDerivedDataset]:
+    dset: UploadRawDataset | UploadDerivedDataset, user: SciCatUser
+) -> UploadRawDataset | UploadDerivedDataset:
     dset = deepcopy(dset)
     dset.owner = user.username
     dset.ownerGroup = user.group
     dset.ownerEmail = user.email
     return dset
 
 
@@ -254,15 +253,15 @@
 ) -> UploadAttachment:
     attachment = deepcopy(attachment)
     attachment.ownerGroup = user.group
     return attachment
 
 
 def _create_dataset_model(
-    client: Client, dset: Union[UploadRawDataset, UploadDerivedDataset]
+    client: Client, dset: UploadRawDataset | UploadDerivedDataset
 ) -> DownloadDataset:
     uploaded = client.scicat.create_dataset_model(dset)
     # pid is a str if validation fails but we need a PID for fake clients.
     uploaded.pid = PID.parse(uploaded.pid)  # type: ignore[arg-type]
     return uploaded
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/docs.py` & `scitacean-24.4.0/src/scitacean/testing/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
                 ),
             ],
         )
     ]
 
 
 def setup_fake_client() -> FakeClient:
+    """Create a fake client for use in the user guide."""
     client = FakeClient.from_token(
         url="fake-url.sci/api/v3",
         token="fake-token",  # noqa: S106
         file_transfer=FakeFileTransfer(fs=None),
     )
     _create_raw_dataset(client)
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/sftp/__init__.py` & `scitacean-24.4.0/src/scitacean/testing/sftp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,23 +98,21 @@
 """
 
 from ._pytest_helpers import add_pytest_option, sftp_enabled, skip_if_not_sftp
 from ._sftp import (
     IgnorePolicy,
     SFTPAccess,
     SFTPUser,
-    can_connect,
     configure,
     local_access,
     wait_until_sftp_server_is_live,
 )
 
 __all__ = [
     "add_pytest_option",
-    "can_connect",
     "configure",
     "local_access",
     "sftp_enabled",
     "skip_if_not_sftp",
     "wait_until_sftp_server_is_live",
     "IgnorePolicy",
     "SFTPAccess",
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/sftp/_pytest_helpers.py` & `scitacean-24.4.0/src/scitacean/testing/sftp/_pytest_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
-from typing import Optional
 
 import pytest
 
-_COMMAND_LINE_OPTION: Optional[str] = None
+_COMMAND_LINE_OPTION: str | None = None
 
 
 def add_pytest_option(parser: pytest.Parser, option: str = "--sftp-tests") -> None:
     """Add a command-line option to pytest to toggle SFTP tests.
 
     Parameters
     ----------
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/sftp/_sftp.py` & `scitacean-24.4.0/src/scitacean/testing/sftp/_sftp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 import importlib.resources
 import time
+from collections.abc import Iterable
 from dataclasses import dataclass
 from functools import lru_cache
 from pathlib import Path
-from typing import Any, Dict, Iterable, Tuple, Union
+from typing import Any
 
 import paramiko
 import yaml
 
 
 @dataclass
 class SFTPUser:
@@ -21,57 +22,44 @@
 class SFTPAccess:
     host: str
     port: int
     user: SFTPUser
 
 
 def _read_resource_text(filename: str) -> str:
-    if hasattr(importlib.resources, "files"):
-        # Use new API added in Python 3.9
-        return (
-            importlib.resources.files("scitacean.testing.sftp")
-            .joinpath(filename)
-            .read_text()
-        )
-    # Old API, deprecated as of Python 3.11
-    return importlib.resources.read_text("scitacean.testing.sftp", filename)
+    return (
+        importlib.resources.files("scitacean.testing.sftp")
+        .joinpath(filename)
+        .read_text()
+    )
 
 
 def _read_resource_yaml(filename: str) -> Any:
     return yaml.safe_load(_read_resource_text(filename))
 
 
 @lru_cache(maxsize=1)
-def _docker_compose_file() -> Dict[str, Any]:
-    return _read_resource_yaml(
+def _docker_compose_file() -> dict[str, Any]:
+    return _read_resource_yaml(  # type: ignore[no-any-return]
         "docker-compose-sftp-server.yaml"
-    )  # type: ignore[no-any-return]
+    )
 
 
 @lru_cache(maxsize=1)
 def _docker_file() -> str:
     return _read_resource_text("Dockerfile-sftp-server")
 
 
-def _seed_files() -> Iterable[Tuple[str, str]]:
-    if hasattr(importlib.resources, "files"):
-        # Use new API added in Python 3.9
-        yield from (
-            (file.name, file.read_text())
-            for file in importlib.resources.files("scitacean.testing.sftp")
-            .joinpath("sftp_server_seed")
-            .iterdir()
-        )
-    else:
-        # Old API, deprecated as of Python 3.11
-        with importlib.resources.path(
-            "scitacean.testing.sftp", "sftp_server_seed"
-        ) as seed_dir:
-            for path in seed_dir.iterdir():
-                yield path.name, path.read_text()
+def _seed_files() -> Iterable[tuple[str, str]]:
+    yield from (
+        (file.name, file.read_text())
+        for file in importlib.resources.files("scitacean.testing.sftp")
+        .joinpath("sftp_server_seed")
+        .iterdir()
+    )
 
 
 def local_access() -> SFTPAccess:
     config = _docker_compose_file()
     service = config["services"]["scitacean-test-sftp-server"]
     env = {k: v for k, v in map(lambda s: s.split("="), service["environment"])}
     return SFTPAccess(
@@ -85,15 +73,15 @@
 
 
 def _copy_seed(target_seed_dir: Path) -> None:
     for name, content in _seed_files():
         target_seed_dir.joinpath(name).write_text(content)
 
 
-def configure(target_dir: Union[Path, str]) -> Path:
+def configure(target_dir: Path | str) -> Path:
     """Generate a config file for docker compose and copy seed data."""
     target_dir = Path(target_dir)
     target_seed_dir = target_dir / "data" / "seed"
     target_seed_dir.mkdir(parents=True)
     _copy_seed(target_seed_dir)
 
     config_target = target_dir / "docker-compose.yaml"
@@ -104,31 +92,31 @@
         f"""DATA_DIR={target_dir / 'data'}
 SEED_DIR={target_seed_dir}"""
     )
 
     return config_target
 
 
-def can_connect(sftp_access: SFTPAccess) -> bool:
+def _can_connect(sftp_access: SFTPAccess) -> bool:
     try:
         _make_client(sftp_access)
     except paramiko.SSHException:
         return False
     return True
 
 
 def wait_until_sftp_server_is_live(
     sftp_access: SFTPAccess, max_time: float, n_tries: int
 ) -> None:
     # The container takes a while to be fully live.
     for _ in range(n_tries):
-        if can_connect(sftp_access):
+        if _can_connect(sftp_access):
             return
         time.sleep(max_time / n_tries)
-    if not can_connect(sftp_access):
+    if not _can_connect(sftp_access):
         raise RuntimeError("Cannot connect to SFTP server")
 
 
 def cleanup_data_dir(
     sftp_access: SFTPAccess, sftp_connect_with_username_password: Any
 ) -> None:
     # Delete all directories created by tests.
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/sftp/docker-compose-sftp-server.yaml` & `scitacean-24.4.0/src/scitacean/testing/sftp/docker-compose-sftp-server.yaml`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/src/scitacean/testing/sftp/fixtures.py` & `scitacean-24.4.0/src/scitacean/testing/sftp/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # mypy: disable-error-code="no-untyped-def"
 """Pytest fixtures to manage and access a local SFTP server."""
 
 import logging
+from collections.abc import Callable, Generator
 from pathlib import Path
-from typing import Callable, Generator, Optional
 
 import pytest
 from paramiko import SFTPClient, SSHClient
 
 from ..._internal import docker
 from .._pytest_helpers import init_work_dir, root_tmp_dir
 from ._pytest_helpers import sftp_enabled, skip_if_not_sftp
@@ -36,15 +36,15 @@
     skip_if_not_sftp(request)
     return local_access()
 
 
 @pytest.fixture(scope="session")
 def sftp_base_dir(
     request: pytest.FixtureRequest, tmp_path_factory: pytest.TempPathFactory
-) -> Optional[Path]:
+) -> Path | None:
     """Fixture that returns the base working directory for the SFTP server setup.
 
     Returns
     -------
     :
         A path to a directory on the host machine.
         The directory gets populated by the
@@ -55,15 +55,15 @@
     """
     if not sftp_enabled(request):
         return None
     return root_tmp_dir(request, tmp_path_factory) / "scitacean-sftp"
 
 
 @pytest.fixture(scope="session")
-def sftp_data_dir(sftp_base_dir: Optional[Path]) -> Optional[Path]:
+def sftp_data_dir(sftp_base_dir: Path | None) -> Path | None:
     """Fixture that returns the data directory for the SFTP server setup.
 
     Returns
     -------
     :
         A path to a directory on the host machine.
         The directory is mounted as ``/data`` on the server.
@@ -85,16 +85,16 @@
     skip_if_not_sftp(request)
 
 
 @pytest.fixture(scope="session")
 def sftp_fileserver(
     request: pytest.FixtureRequest,
     sftp_access: SFTPAccess,
-    sftp_base_dir: Optional[Path],
-    sftp_data_dir: Optional[Path],
+    sftp_base_dir: Path | None,
+    sftp_data_dir: Path | None,
     sftp_connect_with_username_password,
 ) -> Generator[bool, None, None]:
     """Fixture to declare that a test needs a local SFTP server.
 
     If SFTP tests are enabled, this fixture configures and starts an SFTP server
     in a docker container the first time a test requests it.
     The server and container will be stopped and removed at the end of the test session.
@@ -176,15 +176,15 @@
         raise RuntimeError("SFTP docker container is already running")
     docker_compose_file = target_dir / "docker-compose.yaml"
     log = logging.getLogger("scitacean.testing")
     log.info("Starting docker container with SFTP server from %s", docker_compose_file)
     configure(target_dir)
     docker.docker_compose_up(docker_compose_file)
     log.info("Waiting for SFTP docker to become accessible")
-    wait_until_sftp_server_is_live(sftp_access=sftp_access, max_time=20, n_tries=20)
+    wait_until_sftp_server_is_live(sftp_access=sftp_access, max_time=60, n_tries=40)
     log.info("Successfully connected to SFTP server")
     # Give the user write access.
     docker.docker_compose_run(
         docker_compose_file, "scitacean-test-sftp-server", "chown", "1000:1000", "/data"
     )
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/strategies.py` & `scitacean-24.4.0/src/scitacean/testing/strategies.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Hypothesis strategies for generating datasets.
 
 This module defines a number of
 `Hypothesis <https://hypothesis.readthedocs.io/en/latest/>`_ strategies to
 generate test inputs.
 
 Note
@@ -27,33 +27,33 @@
 
 Select the 'scitacean' profile during tests using the
 ``--hypothesis-profile=scitacean`` command line option.
 """
 
 import string
 from functools import partial
-from typing import Any, Dict, Optional
+from typing import Any
 
 from email_validator import EmailNotValidError, ValidatedEmail, validate_email
 from hypothesis import strategies as st
 
 from .. import PID, Dataset, DatasetType, RemotePath, model
 from .._internal.orcid import orcid_checksum
 
 
 # email_validator and by extension pydantic is more picky than hypothesis
 # so make sure that generated emails actually pass model validation.
-def _validate_email(email: str) -> Optional[ValidatedEmail]:
+def _validate_email(email: str) -> ValidatedEmail | None:
     try:
         return validate_email(email, check_deliverability=False)
     except EmailNotValidError:
         return None
 
 
-def _is_valid_email(validated_email: Optional[ValidatedEmail]) -> bool:
+def _is_valid_email(validated_email: ValidatedEmail | None) -> bool:
     return validated_email is not None
 
 
 def emails() -> st.SearchStrategy[str]:
     """A strategy for generating email addresses as strings.
 
     This differs from :func:`hypothesis.strategies.emails` in that it
@@ -103,15 +103,15 @@
     return st.lists(
         emails(),
         min_size=1,
         max_size=max_emails,
     ).map(lambda email: ";".join(email))
 
 
-def _email_field_strategy(field: Dataset.Field) -> st.SearchStrategy[Optional[str]]:
+def _email_field_strategy(field: Dataset.Field) -> st.SearchStrategy[str | None]:
     if field.required:
         return multi_emails()
     return st.none() | multi_emails()
 
 
 def orcids() -> st.SearchStrategy[str]:
     """A strategy for generating ORCID ids.
@@ -129,38 +129,38 @@
         return "https://orcid.org/" + "-".join(
             digits[i : i + 4] for i in range(0, 16, 4)
         )
 
     return st.text(alphabet="0123456789", min_size=16, max_size=16).map(make_orcid)
 
 
-def _orcid_field_strategy(field: Dataset.Field) -> st.SearchStrategy[Optional[str]]:
+def _orcid_field_strategy(field: Dataset.Field) -> st.SearchStrategy[str | None]:
     if field.required:
         return orcids()
     return st.none() | orcids()
 
 
 def _scientific_metadata_strategy(
     field: Dataset.Field,
-) -> st.SearchStrategy[Dict[str, Any]]:
+) -> st.SearchStrategy[dict[str, Any]]:
     return st.dictionaries(
         keys=st.text(),
         values=st.text() | st.dictionaries(keys=st.text(), values=st.text()),
     )
 
 
 def _job_parameters_strategy(
     field: Dataset.Field,
-) -> st.SearchStrategy[Optional[Dict[str, str]]]:
-    return st.from_type(Optional[Dict[str, str]])  # type: ignore[arg-type]
+) -> st.SearchStrategy[dict[str, str] | None]:
+    return st.from_type(dict[str, str] | None)  # type: ignore[arg-type]
 
 
 def _lifecycle_strategy(
     field: Dataset.Field,
-) -> st.SearchStrategy[Optional[model.Lifecycle]]:
+) -> st.SearchStrategy[model.Lifecycle | None]:
     # Lifecycle contains fields that have `Any` types which `st.from_type` can't handle.
     return st.sampled_from((None, model.Lifecycle()))
 
 
 _SPECIAL_FIELDS = {
     "contact_email": _email_field_strategy,
     "history": lambda field: st.none(),
@@ -188,29 +188,29 @@
 )
 
 
 def _field_strategy(field: Dataset.Field) -> st.SearchStrategy[Any]:
     if (strategy := _SPECIAL_FIELDS.get(field.name)) is not None:
         return strategy(field)
 
-    typ = field.type if field.required else Optional[field.type]
+    typ = field.type if field.required else field.type | None
     return st.from_type(typ)  # type:ignore[arg-type]
 
 
 def _make_dataset(
-    *, type: DatasetType, args: Dict[str, Any], read_only: Dict[str, Any]
+    *, type: DatasetType, args: dict[str, Any], read_only: dict[str, Any]
 ) -> Dataset:
     dset = Dataset(type=type, **args)
     for key, val in read_only.items():
         setattr(dset, "_" + key, val)
     return dset
 
 
 def datasets(
-    type: Optional[DatasetType] = None, for_upload: bool = False, **fields: Any
+    type: DatasetType | None = None, for_upload: bool = False, **fields: Any
 ) -> st.SearchStrategy[Dataset]:
     """A strategy for generating datasets.
 
     This strategy can populate all dataset fields.
     However, there are some limitations:
 
     - Some complex models may be uninitialized, e.g., ``lifecycle``.
@@ -290,15 +290,15 @@
         return val if isinstance(val, st.SearchStrategy) else st.just(val)
 
     def make_arg(field: Dataset.Field) -> st.SearchStrategy[Any]:
         if field.name in fields:
             return make_fixed_arg(field.name)
         return _field_strategy(field)
 
-    def make_args(read_only: bool) -> Dict[str, st.SearchStrategy[Any]]:
+    def make_args(read_only: bool) -> dict[str, st.SearchStrategy[Any]]:
         return {
             field.name: make_arg(field)
             for field in Dataset.fields(read_only=read_only, dataset_type=type)
             if field.name != "type"
         }
 
     args = st.fixed_dictionaries(
```

### Comparing `scitacean-23.8.0/src/scitacean/testing/transfer.py` & `scitacean-24.4.0/src/scitacean/testing/transfer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Fake file transfer."""
 
+from collections.abc import Iterator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Dict, Iterator, List, Optional, Union
+from typing import Any
 
 try:
     from pyfakefs.fake_filesystem import FakeFilesystem
 except ImportError:
     from typing import TypeAlias
 
     FakeFilesystem: TypeAlias = Any  # type: ignore[no-redef]
@@ -18,60 +19,64 @@
 from ..filesystem import RemotePath
 from ..transfer.util import source_folder_for
 
 
 class FakeDownloadConnection:
     """'Download' files from a fake file transfer."""
 
-    def __init__(self, fs: Optional[FakeFilesystem], files: Dict[RemotePath, bytes]):
+    def __init__(self, fs: FakeFilesystem | None, files: dict[RemotePath, bytes]):
         self.files = files
         self.fs = fs
 
     def download_file(self, *, remote: RemotePath, local: Path) -> None:
+        """Download a single file."""
         if self.fs is not None:
             self.fs.create_file(local, contents=self.files[remote])
         else:
             with open(local, "wb") as f:
                 f.write(self.files[remote])
 
-    def download_files(self, *, remote: List[RemotePath], local: List[Path]) -> None:
+    def download_files(self, *, remote: list[RemotePath], local: list[Path]) -> None:
+        """Download multiple files."""
         for r, l in zip(remote, local):
             self.download_file(remote=r, local=l)
 
 
 class FakeUploadConnection:
     """'Upload' files to a fake file transfer."""
 
     def __init__(
         self,
-        files: Dict[RemotePath, bytes],
-        reverted: Dict[RemotePath, bytes],
+        files: dict[RemotePath, bytes],
+        reverted: dict[RemotePath, bytes],
         source_folder: RemotePath,
     ):
         self.files = files
         self.reverted = reverted
         self._source_folder = source_folder
 
     def _remote_path(self, filename: RemotePath) -> RemotePath:
         return self._source_folder / filename
 
-    def _upload_file(self, *, remote: RemotePath, local: Optional[Path]) -> RemotePath:
+    def _upload_file(self, *, remote: RemotePath, local: Path | None) -> RemotePath:
         if local is None:
             raise ValueError(f"No local path for file {remote}")
         remote = self._remote_path(remote)
         with open(local, "rb") as f:
             self.files[remote] = f.read()
         return remote
 
-    def upload_files(self, *files: File) -> List[File]:
+    def upload_files(self, *files: File) -> list[File]:
+        """Upload files."""
         for file in files:
             self._upload_file(remote=file.remote_path, local=file.local_path)
         return list(files)
 
     def revert_upload(self, *files: File) -> None:
+        """Remove uploaded files."""
         for file in files:
             remote = self._remote_path(file.remote_path)
             self.reverted[remote] = self.files.pop(remote)
 
 
 class FakeFileTransfer:
     """Mimic a file down-/upload handler.
@@ -85,34 +90,33 @@
     --------
     Using the ``fs`` fixture from pyfakefs in pytest:
 
     .. code-block:: python
 
         def test_upload(fs):
             client = FakeClient.from_token(
-                url="...",
-                token="...",
-                file_transfer=FakeFileTransfer(fs=fs))
+                url="...", token="...", file_transfer=FakeFileTransfer(fs=fs)
+            )
             dset = ...
             client.upload_new_dataset_now(dset)
             assert client.file_transfer.files[expected_remote_path] == file_content
 
     See Also
     --------
     scitacean.testing.client.FakeClient:
         Client to mimic a SciCat server.
     """
 
     def __init__(
         self,
         *,
-        fs: Optional[FakeFilesystem] = None,
-        files: Optional[Dict[Union[str, RemotePath], bytes]] = None,
-        reverted: Optional[Dict[Union[str, RemotePath], bytes]] = None,
-        source_folder: Optional[Union[str, RemotePath]] = None,
+        fs: FakeFilesystem | None = None,
+        files: dict[str | RemotePath, bytes] | None = None,
+        reverted: dict[str | RemotePath, bytes] | None = None,
+        source_folder: str | RemotePath | None = None,
     ):
         """Initialize a file transfer.
 
         Parameters
         ----------
         fs:
             Fake filesystem. If given, files are down-/uploaded to/from this
@@ -130,28 +134,31 @@
         """
         self.fs = fs
         self.files = _remote_path_dict(files)
         self.reverted = _remote_path_dict(reverted)
         self._source_folder_pattern = source_folder
 
     def source_folder_for(self, dataset: Dataset) -> RemotePath:
+        """Return the source folder for a given dataset."""
         return source_folder_for(dataset, self._source_folder_pattern)
 
     @contextmanager
     def connect_for_download(self) -> Iterator[FakeDownloadConnection]:
+        """Open a connection for downloads."""
         yield FakeDownloadConnection(fs=self.fs, files=self.files)
 
     @contextmanager
     def connect_for_upload(self, dataset: Dataset) -> Iterator[FakeUploadConnection]:
+        """Open a connection for uploads."""
         yield FakeUploadConnection(
             files=self.files,
             reverted=self.reverted,
             source_folder=self.source_folder_for(dataset),
         )
 
 
 def _remote_path_dict(
-    d: Optional[Dict[Union[str, RemotePath], bytes]]
-) -> Dict[RemotePath, bytes]:
+    d: dict[str | RemotePath, bytes] | None,
+) -> dict[RemotePath, bytes]:
     if d is None:
         return {}
     return {RemotePath(path): contents for path, contents in d.items()}
```

### Comparing `scitacean-23.8.0/src/scitacean/thumbnail.py` & `scitacean-24.4.0/src/scitacean/thumbnail.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,24 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Thumbnail type for encoding images."""
 
 from __future__ import annotations
 
 import base64
 import mimetypes
 import os
 import re
-from typing import Callable, Dict, Generator, Optional, Union
+from collections.abc import Callable
+from typing import Any
 
-import pydantic
+from pydantic import GetCoreSchemaHandler
+from pydantic_core import core_schema
 
 from ._internal.dataclass_wrapper import dataclass_optional_args
-from ._internal.pydantic_compat import is_pydantic_v1
-
-if not is_pydantic_v1():
-    from typing import Any, Type
-
-    from pydantic import GetCoreSchemaHandler
-    from pydantic_core import core_schema
-
-    def _get_thumbnail_core_schema(
-        cls: Type[Thumbnail], _source_type: Any, _handler: GetCoreSchemaHandler
-    ) -> core_schema.CoreSchema:
-        return core_schema.no_info_after_validator_function(
-            cls.parse,
-            core_schema.union_schema(
-                [core_schema.is_instance_schema(Thumbnail), core_schema.str_schema()]
-            ),
-            serialization=core_schema.plain_serializer_function_ser_schema(
-                cls.serialize, info_arg=False, return_schema=core_schema.str_schema()
-            ),
-        )
 
 
 @dataclass_optional_args(init=False, kw_only=True, slots=True)
 class Thumbnail:
     """Encodes an image to be used as a thumbnail in SciCat.
 
     Thumbnails are *small* images used, e.g., in attachments.
@@ -69,23 +51,23 @@
     Access the raw bytes:
 
     .. code-block:: python
 
         data: bytes = thumbnail.decoded_data()
     """
 
-    mime: Optional[str]
+    mime: str | None
     """Complete MIME type in the form ``type/subtype``."""
     _encoded_data: str
 
     def __init__(
         self,
-        mime: Optional[str],
-        data: Optional[bytes] = None,
-        _encoded_data: Optional[str] = None,
+        mime: str | None,
+        data: bytes | None = None,
+        _encoded_data: str | None = None,
     ) -> None:
         """Create a new thumbnail object.
 
         Parameters
         ----------
         mime:
             The MIME type of the thumbnail.
@@ -108,15 +90,15 @@
                 self._encoded_data = base64.b64encode(data).decode("utf-8")
             else:
                 raise TypeError("Only only of data and _encoded_data may be given")
 
         self.mime = mime
 
     @classmethod
-    def load_file(cls, path: Union[os.PathLike[str], str]) -> Thumbnail:
+    def load_file(cls, path: os.PathLike[str] | str) -> Thumbnail:
         """Construct a thumbnail from data loaded from a file.
 
         Parameters
         ----------
         path:
             The path to the file.
 
@@ -128,15 +110,15 @@
         """
         with open(path, "rb") as f:
             data = f.read()
         encoded_data = base64.b64encode(data).decode("utf-8")
         return Thumbnail(mime=mimetypes.guess_type(path)[0], _encoded_data=encoded_data)
 
     @classmethod
-    def parse(cls, encoded: Union[str, Thumbnail], /) -> Thumbnail:
+    def parse(cls, encoded: str | Thumbnail, /) -> Thumbnail:
         """Construct a thumbnail from a string as used by SciCat.
 
         Parameters
         ----------
         encoded:
             A string containing a MIME content-header and the thumbnail
             in base64 encoding.
@@ -178,22 +160,22 @@
         Thumbnail.parse:
             The inverse operation.
         """
         mime_str = f"data:{self.mime};base64," if self.mime is not None else ""
         return mime_str + self.encoded_data()
 
     @property
-    def mime_type(self) -> Optional[str]:
+    def mime_type(self) -> str | None:
         """The MIME type, i.e., the first part of ``type/subtype``."""
         if self.mime is None:
             return None
         return self.mime.split("/", 1)[0]
 
     @property
-    def mime_subtype(self) -> Optional[str]:
+    def mime_subtype(self) -> str | None:
         """The MIME subtype, i.e., the second part of ``type/subtype``."""
         if self.mime is None:
             return None
         return self.mime.split("/", 1)[1]
 
     def encoded_data(self) -> str:
         """Return the base64-encoded data of the thumbnail."""
@@ -207,19 +189,19 @@
         return f"Thumbnail({self.mime}, len:{len(self.encoded_data())}B)"
 
     def __repr__(self) -> str:
         return f"Thumbnail(mime={self.mime}, data={self.decoded_data()!r})"
 
     def _repr_mimebundle_(
         self, include: Any = None, exclude: Any = None
-    ) -> Dict[str, Union[bytes, str]]:
+    ) -> dict[str, bytes | str]:
         def decoded() -> bytes:
             return self.decoded_data()
 
-        repr_fns = {
+        repr_fns: dict[str, Callable[[], bytes | str]] = {
             "image/png": decoded,
             "image/jpeg": decoded,
             "image/svg+xml": decoded,
             "application/pdf": decoded,
             "text/html": lambda: f"<img src={self.serialize()}>",
             "text/plain": self.__str__,
         }
@@ -232,33 +214,27 @@
             return {self.mime: repr_fns[self.mime]()}
         return {
             mime: fn()
             for mime in {"text/html", "text/plain"}
             if (fn := repr_fns.get(mime))
         }
 
-    if is_pydantic_v1():
-
-        @classmethod
-        def validate(cls, value: Union[str, Thumbnail]) -> Thumbnail:
-            """Pydantic validator for Thumbnail fields."""
-            if isinstance(value, str):
-                return Thumbnail.parse(value)
-            if isinstance(value, Thumbnail):
-                return value
-            raise pydantic.ValidationError("expected a Thumbnail or str")
-
-        @classmethod
-        def __get_validators__(
-            cls,
-        ) -> Generator[Callable[[Union[str, Thumbnail]], Thumbnail], None, None]:
-            yield cls.validate
-
-    else:
-        __get_pydantic_core_schema__ = classmethod(_get_thumbnail_core_schema)
+    @classmethod
+    def __get_pydantic_core_schema__(
+        cls, _source_type: Any, _handler: GetCoreSchemaHandler
+    ) -> core_schema.CoreSchema:
+        return core_schema.no_info_after_validator_function(
+            cls.parse,
+            core_schema.union_schema(
+                [core_schema.is_instance_schema(Thumbnail), core_schema.str_schema()]
+            ),
+            serialization=core_schema.plain_serializer_function_ser_schema(
+                cls.serialize, info_arg=False, return_schema=core_schema.str_schema()
+            ),
+        )
 
 
 # A regex that matches encoded thumbnails with header.
 # Expected form: data:image/png;base64,the-data
 _MESSAGE_REGEX = re.compile(
     r"^(?:data:)?"  # optional data: prefix
     "(?:([^/]+/[^;]+)(?:;.*)?,)?"  # MIME content-header
```

### Comparing `scitacean-23.8.0/src/scitacean/transfer/sftp.py` & `scitacean-24.4.0/src/scitacean/transfer/sftp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,89 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
+"""SFTP file transfer."""
 
 import os
+from collections.abc import Callable, Iterator
 from contextlib import contextmanager
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import Callable, Iterator, List, Optional, Union
 
-from invoke.exceptions import UnexpectedExit
 from paramiko import SFTPAttributes, SFTPClient, SSHClient
 
 from ..dataset import Dataset
 from ..error import FileUploadError
 from ..file import File
 from ..filesystem import RemotePath
 from ..logging import get_logger
 from .util import source_folder_for
 
 
 class SFTPDownloadConnection:
+    """Connection for downloading files with SFTP.
+
+    Should be created using
+    :meth:`scitacean.transfer.sftp.SFTPFileTransfer.connect_for_download`.
+    """
+
     def __init__(self, *, sftp_client: SFTPClient, host: str) -> None:
         self._sftp_client = sftp_client
         self._host = host
 
-    def download_files(self, *, remote: List[RemotePath], local: List[Path]) -> None:
+    def download_files(self, *, remote: list[RemotePath], local: list[Path]) -> None:
         """Download files from the given remote path."""
         for r, l in zip(remote, local):
             self.download_file(remote=r, local=l)
 
     def download_file(self, *, remote: RemotePath, local: Path) -> None:
+        """Download a file from the given remote path."""
         get_logger().info(
             "Downloading file %s from host %s to %s",
             remote,
             self._host,
             local,
         )
         self._sftp_client.get(remotepath=remote.posix, localpath=os.fspath(local))
 
 
 class SFTPUploadConnection:
+    """Connection for uploading files with SFTP.
+
+    Should be created using
+    :meth:`scitacean.transfer.sftp.SFTPFileTransfer.connect_for_upload`.
+    """
+
     def __init__(
         self, *, sftp_client: SFTPClient, source_folder: RemotePath, host: str
     ) -> None:
         self._sftp_client = sftp_client
         self._source_folder = source_folder
         self._host = host
 
     @property
     def source_folder(self) -> RemotePath:
+        """The source folder this connection uploads to."""
         return self._source_folder
 
-    def remote_path(self, filename: Union[str, RemotePath]) -> RemotePath:
+    def remote_path(self, filename: str | RemotePath) -> RemotePath:
+        """Return the complete remote path for a given path."""
         return self.source_folder / filename
 
     def _make_source_folder(self) -> None:
         try:
             _mkdir_remote(self._sftp_client, self.source_folder)
         except OSError as exc:
             raise FileUploadError(
                 f"Failed to create source folder {self.source_folder}: {exc.args}"
             ) from None
 
-    def upload_files(self, *files: File) -> List[File]:
+    def upload_files(self, *files: File) -> list[File]:
         """Upload files to the remote folder."""
         self._make_source_folder()
-        uploaded = []
+        uploaded: list[File] = []
         try:
             uploaded.extend(self._upload_file(file) for file in files)
         except Exception:
             self.revert_upload(*uploaded)
             raise
         return uploaded
 
@@ -105,61 +120,55 @@
             try:
                 get_logger().info(
                     "Removing empty remote directory %s on host %s",
                     self.source_folder,
                     self._host,
                 )
                 self._sftp_client.rmdir(self.source_folder.posix)
-            except UnexpectedExit as exc:
+            except OSError as exc:
                 get_logger().warning(
-                    "Failed to remove empty remote directory %s on host:\n%s",
+                    "Failed to remove empty remote directory %s on host %s:\n%s",
                     self.source_folder,
                     self._host,
-                    exc.result,
+                    exc,
                 )
 
-    def _revert_upload_single(
-        self, *, remote: RemotePath, local: Optional[Path]
-    ) -> None:
+    def _revert_upload_single(self, *, remote: RemotePath, local: Path | None) -> None:
         remote_path = self.remote_path(remote)
         get_logger().info(
             "Reverting upload of file %s to %s on host %s",
             local,
             remote_path,
             self._host,
         )
 
         try:
             self._sftp_client.remove(remote_path.posix)
-        except UnexpectedExit as exc:
-            get_logger().warning(
-                "Error reverting file %s:\n%s", remote_path, exc.result
-            )
+        except OSError as exc:
+            get_logger().warning("Error reverting file %s:\n%s", remote_path, exc)
             return
 
 
 class SFTPFileTransfer:
     """Upload / download files using SFTP.
 
     Configuration & Authentication
     ------------------------------
     The file transfer connects to the server at the address given
     as the ``host`` constructor argument.
     This may be
 
     - a full url such as ``some.fileserver.edu``,
-    - an IP address like ``127.0.0.1``,
-    - or a host defined in the user's openSFTP config file.
+    - or an IP address like ``127.0.0.1``.
 
-    The file transfer can authenticate using username+password.
-    It will ask for those on the command line.
-    However, it is **highly recommended to set up a key and use an SFTP agent!**
-    This increases security as Scitacean no longer has to handle credentials itself.
-    And it is required for automated programs where a user cannot enter credentials
-    on a command line.
+    The file transfer can currently only authenticate through an SSH agent.
+    The agent must be set up for the chosen host and hold a valid key.
+    If this is not the case, it is possible to inject a custom ``connect`` function
+    that authenticates in a different way.
+    See the examples below.
 
     Upload folder
     -------------
     The file transfer can take an optional ``source_folder`` as a constructor argument.
     If it is given, ``SFTPFileTransfer`` uploads all files to it and ignores the
     source folder set in the dataset.
     If it is not given, ``SFTPFileTransfer`` uses the dataset's source folder.
@@ -172,52 +181,76 @@
 
     Examples
     --------
     Given
 
     .. code-block:: python
 
-        dset = Dataset(type="raw",
-                       name="my-dataset",
-                       source_folder="/dataset/source",
-                       )
+        dset = Dataset(
+            type="raw",
+            name="my-dataset",
+            source_folder="/dataset/source",
+        )
 
     This uploads to ``/dataset/source``:
 
     .. code-block:: python
 
         file_transfer = SFTPFileTransfer(host="fileserver")
 
     This uploads to ``/transfer/folder``:
 
     .. code-block:: python
 
         file_transfer = SFTPFileTransfer(host="fileserver",
-                                        source_folder="transfer/folder")
+                                         source_folder="transfer/folder")
 
     This uploads to ``/transfer/my-dataset``:
     (Note that ``{name}`` is replaced by ``dset.name``.)
 
     .. code-block:: python
 
         file_transfer = SFTPFileTransfer(host="fileserver",
                                         source_folder="transfer/{name}")
 
-    A useful approach is to include a unique ID in the source folder, for example
+    A useful approach is to include a unique ID in the source folder, for example,
     ``"/some/base/folder/{uid}"``, to avoid clashes between different datasets.
     Scitacean will fill in the ``"{uid}"`` placeholder with a new UUID4.
+
+    The connection and authentication method can be customized
+    using the ``connect`` argument.
+    For example, to use a specific username + SSH key file, use the following:
+
+    .. code-block:: python
+
+        def connect(host, port):
+            from paramiko import SSHClient
+
+            client = SSHClient()
+            client.load_system_host_keys()
+            client.connect(
+                hostname=host,
+                port=port,
+                username="<username>",
+                key_filename="<key-file-name>",
+            )
+            return client.open_sftp()
+
+        file_transfer = SFTPFileTransfer(host="fileserver", connect=connect)
+
+    The :class:`paramiko.client.SSHClient` can be configured as needed in this function.
     """
 
     def __init__(
         self,
         *,
         host: str,
         port: int = 22,
-        source_folder: Optional[Union[str, RemotePath]] = None,
-        connect: Optional[Callable[[str, Optional[int]], SFTPClient]] = None,
+        source_folder: str | RemotePath | None = None,
+        connect: Callable[[str, int | None], SFTPClient] | None = None,
     ) -> None:
         """Construct a new SFTP file transfer.
 
         Parameters
         ----------
         host:
             URL or name of the server to connect to.
@@ -232,17 +265,15 @@
             for the server instead of the builtin method.
             The function arguments are ``host`` and ``port`` as determined by the
             arguments to ``__init__`` shown above.
         """
         self._host = host
         self._port = port
         self._source_folder_pattern = (
-            RemotePath(source_folder)
-            if isinstance(source_folder, str)
-            else source_folder
+            RemotePath(source_folder) if source_folder is not None else None
         )
         self._connect = connect
 
     def source_folder_for(self, dataset: Dataset) -> RemotePath:
         """Return the source folder used for the given dataset."""
         return source_folder_for(dataset, self._source_folder_pattern)
 
@@ -271,25 +302,28 @@
             yield SFTPUploadConnection(
                 sftp_client=sftp_client, source_folder=source_folder, host=self._host
             )
         finally:
             sftp_client.close()
 
 
-def _default_connect(host: str, port: int) -> SFTPClient:
+def _default_connect(host: str, port: int | None) -> SFTPClient:
     client = SSHClient()
     client.load_system_host_keys()
-    client.connect(hostname=host, port=port)
+    if port is not None:
+        client.connect(hostname=host, port=port)
+    else:
+        client.connect(hostname=host)
     return client.open_sftp()
 
 
 def _connect(
     host: str,
     port: int,
-    connect: Optional[Callable[[str, Optional[int]], SFTPClient]],
+    connect: Callable[[str, int | None], SFTPClient] | None,
 ) -> SFTPClient:
     try:
         if connect is None:
             connect = _default_connect
         return connect(host, port)
     except Exception as exc:
         # We pass secrets as arguments to functions called in this block, and those
@@ -311,15 +345,15 @@
         sftp.mkdir(path.posix)
     elif not _is_remote_dir(st_stat):
         raise FileExistsError(
             f"Cannot make directory because path points to a file: {path}"
         )
 
 
-def _try_remote_stat(sftp: SFTPClient, path: RemotePath) -> Optional[SFTPAttributes]:
+def _try_remote_stat(sftp: SFTPClient, path: RemotePath) -> SFTPAttributes | None:
     try:
         return sftp.stat(path.posix)
     except FileNotFoundError:
         return None
 
 
 def _is_remote_dir(st_stat: SFTPAttributes) -> bool:
```

### Comparing `scitacean-23.8.0/src/scitacean/transfer/util.py` & `scitacean-24.4.0/src/scitacean/transfer/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Common utilities for file transfers."""
 
-from typing import Optional, Union
 from uuid import uuid4
 
 from ..dataset import Dataset
 from ..filesystem import RemotePath
 from ..util.formatter import DatasetPathFormatter
 
 
-def source_folder_for(
-    dataset: Dataset, pattern: Optional[Union[str, RemotePath]]
-) -> RemotePath:
+def source_folder_for(dataset: Dataset, pattern: str | RemotePath | None) -> RemotePath:
     """Get or build the source folder for a dataset.
 
     Parameters
     ----------
     dataset:
         Build the source folder for this dataset.
     pattern:
```

### Comparing `scitacean-23.8.0/src/scitacean/typing.py` & `scitacean-24.4.0/src/scitacean/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 """Definitions for type checking."""
 
+from contextlib import AbstractContextManager
 from pathlib import Path
-from typing import ContextManager, List, Protocol
+from typing import Protocol
 
 from .dataset import Dataset
 from .file import File
 from .filesystem import RemotePath
 
 
 class DownloadConnection(Protocol):
     """An open connection to the file server for downloads."""
 
-    def download_files(self, *, remote: List[RemotePath], local: List[Path]) -> None:
+    def download_files(self, *, remote: list[RemotePath], local: list[Path]) -> None:
         """Download files from the file server.
 
         Parameters
         ----------
         remote:
             The full path to the file on the server.
         local:
             Desired path of the file on the local filesystem.
         """
 
 
 class Downloader(Protocol):
     """Handler for file downloads."""
 
-    def connect_for_download(self) -> ContextManager[DownloadConnection]:
+    def connect_for_download(self) -> AbstractContextManager[DownloadConnection]:
         """Open a connection to the file server.
 
         Returns
         -------
         :
             A connection object that can download files.
         """
 
 
 class UploadConnection(Protocol):
     """An open connection to the file server for uploads."""
 
-    def upload_files(self, *files: File) -> List[File]:
+    def upload_files(self, *files: File) -> list[File]:
         """Upload files to the file server.
 
         Parameters
         ----------
         files:
             Specify which files to upload including local and remote paths.
 
@@ -86,15 +87,17 @@
 
         Returns
         -------
         :
             The source folder for ``dataset``.
         """
 
-    def connect_for_upload(self, dataset: Dataset) -> ContextManager[UploadConnection]:
+    def connect_for_upload(
+        self, dataset: Dataset
+    ) -> AbstractContextManager[UploadConnection]:
         """Open a connection to the file server.
 
         Parameters
         ----------
         dataset:
             Dataset whose files will be uploaded.
```

### Comparing `scitacean-23.8.0/src/scitacean/util/credentials.py` & `scitacean-24.4.0/src/scitacean/util/credentials.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Tools for securely handling credentials."""
+
 from __future__ import annotations
 
-import datetime
-from typing import NoReturn, Optional, Union
+from datetime import datetime, timedelta, timezone
+from typing import NoReturn
+
+from .._internal.jwt import expiry
 
 
 class StrStorage:
     """Base class for storing a string.
 
     Instances can be nested to combine different specialized features.
     """
 
-    def __init__(self, value: Optional[Union[str, StrStorage]]):
+    def __init__(self, value: str | StrStorage | None):
         self._value = value
 
     def get_str(self) -> str:
         """Return the stored plain str object."""
         if self._value is None:
             # If the implementation chooses to not
             # store the string in memory.
@@ -31,96 +34,80 @@
     def __str__(self) -> str:
         return str(self._value)
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self._value!r})"
 
 
-# TODO implement
-# class KeyringStr(StrStorage):
-#     """Store a string in the user's keyring.
-#
-#     Should be the bottom level StrStorage because it erases any nested
-#     StrStorage objects and stores and returns plain strs.
-#     """
-#
-#     def __init__(self, *, key: str, value: Optional[Union[str, StrStorage]]):
-#         super().__init__(None)
-#         # TODO dummy implementation
-#         self._ring = {}
-#         self._key = key
-#         if value is not None:
-#             if isinstance(value, StrStorage):
-#                 self._store(value.get_str())
-#             else:
-#                 self._store(value)
-#
-#     def _store(self, value: str):
-#         self._ring[self._key] = value
-#
-#     def _retrieve(self) -> str:
-#         return self._ring[self._key]
-#
-#     def get_str(self) -> str:
-#         return self._retrieve()
-#
-#     def __str__(self) -> str:
-#         return "???"
-#
-#     def __repr__(self) -> str:
-#         return f"KeyringStr(key='{self._key}', value={str(self)})"
-
-
 class SecretStr(StrStorage):
     """Minimize the risk of exposing a secret.
 
     Stores a string and blocks the most common pathways
     of leaking it to logs or files.
 
     Attention
     ---------
     The string may be stored as a regular, unencrypted str object and can
     still be leaked through introspection methods.
     """
 
-    def __init__(self, value: Union[str, StrStorage]):
+    def __init__(self, value: str | StrStorage):
         super().__init__(value)
 
     def __str__(self) -> str:
         return "***"
 
     def __repr__(self) -> str:
         return "SecretStr(***)"
 
     # prevent pickling
     def __reduce_ex__(self, protocol: object) -> NoReturn:
         raise TypeError("SecretStr must not be pickled")
 
 
-class TimeLimitedStr(StrStorage):
-    """A string that expires after some time."""
+class ExpiringToken(StrStorage):
+    """A JWT token that expires after some time."""
 
     def __init__(
         self,
         *,
-        value: Union[str, StrStorage],
-        expires_at: datetime.datetime,
-        tolerance: Optional[datetime.timedelta] = None,
+        value: str | StrStorage,
+        expires_at: datetime,
+        denial_period: timedelta | None = None,
     ):
         super().__init__(value)
-        if tolerance is None:
-            tolerance = datetime.timedelta(seconds=10)
-        self._expires_at = expires_at - tolerance
+        if denial_period is None:
+            denial_period = timedelta(seconds=2)
+        self._expires_at = expires_at - denial_period
+        self._check_expiry()
+
+    @classmethod
+    def from_jwt(cls, value: str | StrStorage) -> ExpiringToken:
+        """Create a new ExpiringToken from a JSON web token."""
+        value_str = value if isinstance(value, str) else value.get_str()
+        try:
+            expires_at = expiry(value_str)
+        except ValueError:
+            expires_at = datetime.now(tz=timezone.utc) + timedelta(weeks=100)
+        return cls(
+            value=value,
+            expires_at=expires_at,
+        )
 
     def get_str(self) -> str:
-        if self._is_expired():
-            raise RuntimeError("Login has expired")
+        """Return the stored plain str object."""
+        self._check_expiry()
         return super().get_str()
 
-    def _is_expired(self) -> bool:
-        return datetime.datetime.now() > self._expires_at
+    def _check_expiry(self) -> None:
+        if datetime.now(tz=self._expires_at.tzinfo) > self._expires_at:
+            raise RuntimeError(
+                "SciCat login has expired. You need to create a new client either by "
+                "logging in through `Client.from_credentials` or by getting a new "
+                "access token from the SciCat web interface."
+            )
 
     def __repr__(self) -> str:
         return (
             f"TimeLimitedStr(expires_at={self._expires_at.isoformat()}, "
             f"value={self._value!r}"
         )
```

### Comparing `scitacean-23.8.0/src/scitacean/util/formatter.py` & `scitacean-24.4.0/src/scitacean/util/formatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """String-formatting tools."""
 
+from collections.abc import Iterable
 from string import Formatter
-from typing import Any, Iterable, Optional, Tuple
+from typing import Any
 
 from ..filesystem import escape_path
 
 try:
     from typing import LiteralString, TypeVar
 
     StrOrLiteralStr = TypeVar("StrOrLiteralStr", LiteralString, str)
@@ -48,28 +49,31 @@
     Fields that are used by the formatter must not be ``None``.
     Otherwise, a :class:`ValueError` will be raised.
     """
 
     def parse(
         self, format_string: str
     ) -> Iterable[
-        Tuple[
+        tuple[
             StrOrLiteralStr,
-            Optional[StrOrLiteralStr],
-            Optional[StrOrLiteralStr],
-            Optional[StrOrLiteralStr],
+            StrOrLiteralStr | None,
+            StrOrLiteralStr | None,
+            StrOrLiteralStr | None,
         ]
     ]:
-        def add0(field_name: Optional[str]) -> Optional[str]:
+        """Parse a format string."""
+
+        def add0(field_name: str | None) -> str | None:
             if field_name == "uid":
                 return field_name
             if isinstance(field_name, str):
                 return "dset." + field_name
             return None
 
         return ((t[0], add0(t[1]), t[2], t[3]) for t in super().parse(format_string))
 
     def format_field(self, value: Any, format_spec: str) -> str:
+        """Format a field with the given spec."""
         if value is None:
             raise ValueError("Cannot format path, dataset field is None")
         formatted: str = super().format_field(value, format_spec)
         return escape_path(formatted)
```

### Comparing `scitacean-23.8.0/src/scitacean.egg-info/PKG-INFO` & `scitacean-24.4.0/src/scitacean.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitacean
-Version: 23.8.0
+Version: 24.4.0
 Summary: High-level interface for SciCat
 Author: Scitacean contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2023, SciCat Project
         All rights reserved.
         
@@ -33,32 +33,39 @@
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Documentation, https://scicatproject.github.io/scitacean
 Project-URL: Bug Tracker, https://github.com/SciCatProject/scitacean/issues
 Project-URL: Source, https://github.com/SciCatProject/scitacean
 Keywords: scicat
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: ssh
+License-File: LICENSE
+Requires-Dist: email-validator
+Requires-Dist: pydantic>=2
+Requires-Dist: python-dateutil
+Requires-Dist: requests>=2.31
 Provides-Extra: sftp
+Requires-Dist: paramiko; extra == "sftp"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: filelock; extra == "test"
+Requires-Dist: hypothesis; extra == "test"
+Requires-Dist: pyyaml; extra == "test"
 
 [![PyPI badge](https://img.shields.io/pypi/v/scitacean.svg?style=flat-square&color=green)](https://pypi.python.org/pypi/scitacean)
 [![Anaconda-Server Badge](https://img.shields.io/conda/vn/conda-forge/scitacean?style=flat-square&color=green)](https://anaconda.org/conda-forge/scitacean)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7520487.svg)](https://doi.org/10.5281/zenodo.7520487)
 [![License: BSD 3-Clause](https://img.shields.io/github/license/SciCatProject/scitacean?style=flat-square&color=yellowgreen)](LICENSE)
 
 <picture>
```

### Comparing `scitacean-23.8.0/src/scitacean.egg-info/SOURCES.txt` & `scitacean-24.4.0/src/scitacean.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 SECURITY.md
 pyproject.toml
-setup.cfg
 tox.ini
 .github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/dependency-review.yml
 .github/workflows/docs.yml
 .github/workflows/release.yml
 docs/.gitignore
 docs/conf.py
 docs/index.rst
 docs/release-notes.rst
-docs/_static/anaconda-logo.svg
+docs/_static/anaconda-icon.js
 docs/_static/favicon.ico
 docs/_static/logo-dark.svg
 docs/_static/logo.svg
 docs/_static/css/custom.css
+docs/_templates/doc_version.html
 docs/_templates/scitacean-class-template.rst
 docs/_templates/scitacean-module-template.rst
 docs/developer/coding-conventions.rst
 docs/developer/dependency-management.rst
 docs/developer/getting-started.rst
 docs/developer/index.rst
 docs/developer/testing.rst
@@ -43,24 +43,22 @@
 requirements/base.txt
 requirements/ci.in
 requirements/ci.txt
 requirements/dev.in
 requirements/dev.txt
 requirements/docs.in
 requirements/docs.txt
+requirements/mypy.in
+requirements/mypy.txt
 requirements/static.in
 requirements/static.txt
 requirements/test.in
 requirements/test.txt
 requirements/wheels.in
 requirements/wheels.txt
-requirements-pydantic2/base.in
-requirements-pydantic2/base.txt
-requirements-pydantic2/test.in
-requirements-pydantic2/test.txt
 src/scitacean/__init__.py
 src/scitacean/_base_model.py
 src/scitacean/_dataset_fields.py
 src/scitacean/client.py
 src/scitacean/datablock.py
 src/scitacean/dataset.py
 src/scitacean/error.py
@@ -83,28 +81,29 @@
 src/scitacean/_html_repr/_common_html.py
 src/scitacean/_html_repr/_dataset_html.py
 src/scitacean/_html_repr/_resources.py
 src/scitacean/_html_repr/images/__init__.py
 src/scitacean/_html_repr/images/lock.svg
 src/scitacean/_html_repr/styles/__init__.py
 src/scitacean/_html_repr/styles/attachment.css
+src/scitacean/_html_repr/styles/common.css
 src/scitacean/_html_repr/styles/dataset.css
 src/scitacean/_html_repr/templates/__init__.py
 src/scitacean/_html_repr/templates/attachment_field_repr.html.template
 src/scitacean/_html_repr/templates/attachment_repr.html.template
 src/scitacean/_html_repr/templates/dataset_field_repr.html.template
 src/scitacean/_html_repr/templates/dataset_repr.html.template
 src/scitacean/_html_repr/templates/files_repr.html.template
 src/scitacean/_html_repr/templates/metadata_repr.html.template
 src/scitacean/_internal/__init__.py
 src/scitacean/_internal/dataclass_wrapper.py
 src/scitacean/_internal/docker.py
 src/scitacean/_internal/file_counter.py
+src/scitacean/_internal/jwt.py
 src/scitacean/_internal/orcid.py
-src/scitacean/_internal/pydantic_compat.py
 src/scitacean/testing/__init__.py
 src/scitacean/testing/_pytest_helpers.py
 src/scitacean/testing/client.py
 src/scitacean/testing/docs.py
 src/scitacean/testing/strategies.py
 src/scitacean/testing/transfer.py
 src/scitacean/testing/backend/__init__.py
@@ -118,24 +117,17 @@
 src/scitacean/testing/sftp/__init__.py
 src/scitacean/testing/sftp/_pytest_helpers.py
 src/scitacean/testing/sftp/_sftp.py
 src/scitacean/testing/sftp/docker-compose-sftp-server.yaml
 src/scitacean/testing/sftp/fixtures.py
 src/scitacean/testing/sftp/sftp_server_seed/table.csv
 src/scitacean/testing/sftp/sftp_server_seed/text.txt
-src/scitacean/testing/ssh/__init__.py
-src/scitacean/testing/ssh/_pytest_helpers.py
-src/scitacean/testing/ssh/_ssh.py
-src/scitacean/testing/ssh/docker-compose-ssh-server.yaml
-src/scitacean/testing/ssh/fixtures.py
-src/scitacean/testing/ssh/ssh_server_seed/table.csv
-src/scitacean/testing/ssh/ssh_server_seed/text.txt
 src/scitacean/transfer/__init__.py
+src/scitacean/transfer/link.py
 src/scitacean/transfer/sftp.py
-src/scitacean/transfer/ssh.py
 src/scitacean/transfer/util.py
 src/scitacean/util/__init__.py
 src/scitacean/util/credentials.py
 src/scitacean/util/formatter.py
 tests/__init__.py
 tests/conftest.py
 tests/dataset_fields_test.py
@@ -147,23 +139,24 @@
 tests/thumbnail_test.py
 tests/upload_test.py
 tests/client/__init__.py
 tests/client/attachment_client_test.py
 tests/client/client_test.py
 tests/client/datablock_client_test.py
 tests/client/dataset_client_test.py
+tests/client/sample_client_test.py
 tests/common/__init__.py
 tests/common/files.py
 tests/html_repr/__init__.py
 tests/html_repr/html_repr_test.py
 tests/testing/__init__.py
 tests/testing/strategies_test.py
 tests/transfer/__init__.py
+tests/transfer/link_test.py
 tests/transfer/sftp_test.py
-tests/transfer/ssh_test.py
 tests/util/__init__.py
 tests/util/formatter_test.py
 tools/model-generation/README.md
 tools/model-generation/generate_models.py
 tools/model-generation/spec/__init__.py
 tools/model-generation/spec/dataset-fields.yml
 tools/model-generation/spec/field-name-overrides.yml
```

### Comparing `scitacean-23.8.0/tests/client/attachment_client_test.py` & `scitacean-24.4.0/tests/client/attachment_client_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # mypy: disable-error-code="arg-type"
 
 from copy import deepcopy
 
 import pytest
 from dateutil.parser import parse as parse_date
```

### Comparing `scitacean-23.8.0/tests/client/datablock_client_test.py` & `scitacean-24.4.0/tests/client/datablock_client_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # mypy: disable-error-code="arg-type"
 
 import pytest
 from dateutil.parser import parse as parse_date
 
 from scitacean import Client
 from scitacean.client import ScicatClient
@@ -48,15 +48,14 @@
         dataFileList=[
             UploadDataFile(
                 path="data.nxs", size=9235, time=parse_date("2023-08-18T13:52:33.000Z")
             )
         ],
         datasetId="PLACEHOLDER",
         ownerGroup=scicat_access.user.group,
-        accessGroups=["group1", "2nd_group"],
     )
 
 
 @pytest.mark.parametrize("key", ("raw", "derived"))
 def test_get_orig_datablock(scicat_client, key):
     dblock = INITIAL_ORIG_DATABLOCKS[key][0]
     downloaded = scicat_client.get_orig_datablocks(dblock.datasetId)
@@ -70,13 +69,14 @@
     downloaded = scicat_client.get_orig_datablocks(uploaded.pid)
     assert len(downloaded) == 1
     downloaded = downloaded[0]
     for key, expected in orig_datablock:
         # The database populates a number of fields that are orig_datablock in dset.
         # But we don't want to test those here as we don't want to test the database.
         if expected is not None and key != "dataFileList":
-            assert expected == dict(downloaded)[key], f"key = {key}"
+            assert dict(downloaded)[key] == expected, f"key = {key}"
+    assert downloaded.accessGroups == derived_dataset.accessGroups
     for i in range(len(orig_datablock.dataFileList)):
         for key, expected in orig_datablock.dataFileList[i]:
             assert (
-                expected == dict(downloaded.dataFileList[i])[key]
+                dict(downloaded.dataFileList[i])[key] == expected
             ), f"i = {i}, key = {key}"
```

### Comparing `scitacean-23.8.0/tests/client/dataset_client_test.py` & `scitacean-24.4.0/tests/client/dataset_client_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # mypy: disable-error-code="arg-type, index"
 
 import pydantic
 import pytest
 from dateutil.parser import parse as parse_date
 
 from scitacean import PID, Client, RemotePath, ScicatCommError
@@ -40,14 +40,17 @@
     )
 
 
 @pytest.mark.parametrize("key", ("raw", "derived"))
 def test_get_dataset_model(scicat_client, key):
     dset = INITIAL_DATASETS[key]
     downloaded = scicat_client.get_dataset_model(dset.pid)
+    # The backend may update the dataset after upload.
+    # We cannot easily predict when that happens.
+    downloaded.updatedAt = dset.updatedAt
     assert downloaded == dset
 
 
 def test_get_dataset_model_bad_id(scicat_client):
     with pytest.raises(ScicatCommError):
         scicat_client.get_dataset_model(PID(pid="bad-pid"))
 
@@ -58,14 +61,21 @@
     for key, expected in finalized:
         # The database populates a number of fields that are None in dset.
         # But we don't want to test those here as we don't want to test the database.
         if expected is not None:
             assert expected == dict(downloaded)[key], f"key = {key}"
 
 
+def test_validate_dataset_model(real_client, require_scicat_backend, derived_dataset):
+    real_client.scicat.validate_dataset_model(derived_dataset)
+    derived_dataset.contactEmail = "NotAnEmail"
+    with pytest.raises(ValueError):
+        real_client.scicat.validate_dataset_model(derived_dataset)
+
+
 def test_get_dataset(client):
     dset = INITIAL_DATASETS["raw"]
     dblock = INITIAL_ORIG_DATABLOCKS["raw"][0]
     downloaded = client.get_dataset(dset.pid)
 
     assert downloaded.source_folder == dset.sourceFolder
     assert downloaded.creation_time == dset.creationTime
```

### Comparing `scitacean-23.8.0/tests/common/files.py` & `scitacean-24.4.0/tests/common/files.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 import hashlib
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import Any, Dict, Optional, Union
+from typing import Any
 
 from pyfakefs.fake_filesystem import FakeFilesystem
 
 
 def make_file(
-    fs: FakeFilesystem, path: Union[str, Path], contents: Optional[bytes] = None
-) -> Dict[str, Any]:
+    fs: FakeFilesystem, path: str | Path, contents: bytes | None = None
+) -> dict[str, Any]:
     if contents is None:
         contents = b"a bunch of file contents" * len(str(path))
     path = Path(path)
 
     checksum = hashlib.new("md5")
     checksum.update(contents)
     checksum_digest = checksum.hexdigest()
```

### Comparing `scitacean-23.8.0/tests/conftest.py` & `scitacean-24.4.0/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 import hypothesis
 import pytest
 
 from scitacean.testing.backend import add_pytest_option as add_backend_option
 from scitacean.testing.sftp import add_pytest_option as add_sftp_option
-from scitacean.testing.ssh import add_pytest_option as add_ssh_option
 
 pytest_plugins = (
     "scitacean.testing.backend.fixtures",
     "scitacean.testing.sftp.fixtures",
-    "scitacean.testing.ssh.fixtures",
 )
 
 
 # The datasets strategy requires a large amount of memory and time.
 # This is not good but hard to avoid.
 # So simply disable health checks and accept that tests are slow.
 hypothesis.settings.register_profile(
@@ -26,8 +24,7 @@
     ],
 )
 
 
 def pytest_addoption(parser: pytest.Parser) -> None:
     add_backend_option(parser)
     add_sftp_option(parser)
-    add_ssh_option(parser)
```

### Comparing `scitacean-23.8.0/tests/dataset_fields_test.py` & `scitacean-24.4.0/tests/dataset_fields_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # mypy: disable-error-code="arg-type"
 
 # These tests use Dataset instead of DatasetFields in order to test the
 # public interface and make sure that Dataset does not break any behavior.
 
 from datetime import datetime, timedelta, timezone
-from typing import Union
 
 import dateutil.parser
 import pydantic
 import pytest
 from hypothesis import assume, given, settings
 from hypothesis import strategies as st
 
@@ -23,14 +22,16 @@
     UploadDerivedDataset,
     UploadRawDataset,
 )
 
 # Fields whose types are not supported by hypothesis.
 # E.g. because they contain `Any`.
 _UNGENERATABLE_FIELDS = ("job_parameters", "meta")
+# Fields that are readonly, but still required in the constructor.
+_NOT_SETTABLE_FIELDS = ("type",)
 
 
 def test_init_dataset_with_only_type():
     dset = Dataset(type="raw")
     assert dset.type == DatasetType.RAW
 
 
@@ -56,15 +57,15 @@
     expected = datetime.now(tz=timezone.utc)
     dset = Dataset(type="raw")
     assert dset.creation_time is not None
     assert abs(dset.creation_time - expected) < timedelta(seconds=30)
 
 
 def test_init_dataset_can_set_creation_time():
-    dt: Union[str, datetime]
+    dt: str | datetime
 
     dt = dateutil.parser.parse("2022-01-10T11:14:52.623Z")
     dset = Dataset(type="derived", creation_time=dt)
     assert dset.creation_time == dt
 
     dt = dateutil.parser.parse("2022-01-10T11:14:52+02:00")
     dset = Dataset(type="derived", creation_time=dt)
@@ -103,15 +104,19 @@
     value = data.draw(st.from_type(field.type))
     dset = Dataset(type="raw", **{field.name: value})
     assert getattr(dset, field.name) == value
 
 
 @pytest.mark.parametrize(
     "field",
-    (f for f in Dataset.fields(read_only=False) if f.name not in _UNGENERATABLE_FIELDS),
+    (
+        f
+        for f in Dataset.fields(read_only=False)
+        if f.name not in _UNGENERATABLE_FIELDS and f.name not in _NOT_SETTABLE_FIELDS
+    ),
     ids=lambda f: f.name,
 )
 @given(st.data())
 @settings(max_examples=10)
 def test_can_set_writable_fields(field, data):
     value = data.draw(st.from_type(field.type))
     dset = Dataset(type="raw")
@@ -219,21 +224,21 @@
 
     assert len(list(dset.files)) == 2
     assert dset.number_of_files == 2
     assert dset.number_of_files_archived == 0
     assert dset.packed_size == 0
     assert dset.size == 6123 + 551
 
-    (f0,) = [f for f in dset.files if f.remote_path.suffix == ".dat"]
+    (f0,) = (f for f in dset.files if f.remote_path.suffix == ".dat")
     assert f0.remote_access_path(dset.source_folder) == "/hex/source91/file1.dat"
     assert f0.local_path is None
     assert f0.size == 6123
     assert f0.make_model().path == "file1.dat"
 
-    (f1,) = [f for f in dset.files if f.remote_path.suffix == ".png"]
+    (f1,) = (f for f in dset.files if f.remote_path.suffix == ".png")
     assert f1.remote_access_path(dset.source_folder) == "/hex/source91/sub/file2.png"
     assert f1.local_path is None
     assert f1.size == 551
     assert f1.make_model().path == "sub/file2.png"
 
 
 def test_init_from_models_sets_files_multi_datablocks():
@@ -286,21 +291,21 @@
 
     assert len(list(dset.files)) == 2
     assert dset.number_of_files == 2
     assert dset.number_of_files_archived == 0
     assert dset.packed_size == 0
     assert dset.size == 6123 + 992
 
-    (f0,) = [f for f in dset.files if f.remote_path.suffix == ".dat"]
+    (f0,) = (f for f in dset.files if f.remote_path.suffix == ".dat")
     assert f0.remote_access_path(dset.source_folder) == "/hex/source91/file1.dat"
     assert f0.local_path is None
     assert f0.size == 6123
     assert f0.make_model().path == "file1.dat"
 
-    (f1,) = [f for f in dset.files if f.remote_path.suffix == ".png"]
+    (f1,) = (f for f in dset.files if f.remote_path.suffix == ".png")
     assert f1.remote_access_path(dset.source_folder) == "/hex/source91/sub/file2.png"
     assert f1.local_path is None
     assert f1.size == 992
     assert f1.make_model().path == "sub/file2.png"
 
 
 def test_fields_type_filter_derived():
```

### Comparing `scitacean-23.8.0/tests/dataset_test.py` & `scitacean-24.4.0/tests/dataset_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # mypy: disable-error-code="arg-type, union-attr"
 
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
 
 import pytest
 from dateutil.parser import parse as parse_datetime
@@ -643,14 +643,43 @@
     initial.add_files(file)
     replaced = initial.replace(owner="a-new-owner")
     assert replaced.number_of_files == 1
     assert replaced.size == 6163
     assert list(replaced.files) == list(initial.files)
 
 
+@given(sst.datasets())
+@settings(max_examples=1)
+def test_replace_preserves_meta(initial):
+    initial.meta["key"] = "val"
+    replaced = initial.replace(owner="a-new-owner")
+    assert replaced.meta == {"key": "val"}
+
+
+@given(sst.datasets())
+@settings(max_examples=1)
+def test_replace_meta(initial):
+    initial.meta["key"] = {"value": 2, "unit": "m"}
+    initial.meta["old-key"] = "old-val"
+    replaced = initial.replace(
+        owner="a-new-owner",
+        meta={"key": {"value": 3, "unit": "m"}, "new-key": "new-val"},
+    )
+    assert replaced.meta == {"key": {"value": 3, "unit": "m"}, "new-key": "new-val"}
+
+
+@given(sst.datasets())
+@settings(max_examples=1)
+def test_replace_remove_meta(initial):
+    initial.meta["key"] = {"value": 2, "unit": "m"}
+    initial.meta["old-key"] = "old-val"
+    replaced = initial.replace(owner="a-new-owner", meta=None)
+    assert replaced.meta == {}
+
+
 @pytest.mark.parametrize(
     "attachments",
     (None, [], [model.Attachment(caption="Attachment 1", owner_group="owner")]),
 )
 @given(initial=sst.datasets())
 @settings(max_examples=1)
 def test_replace_preserves_attachments(initial, attachments):
@@ -761,7 +790,120 @@
 )
 @given(initial=sst.datasets(pid=PID(pid="some-id")))
 @settings(max_examples=1)
 def test_derive_removes_attachments(initial, attachments):
     initial.attachments = attachments
     derived = initial.derive()
     assert derived.attachments == []
+
+
+def invalid_field_example(my_type):
+    if my_type == DatasetType.DERIVED:
+        return "data_format", "sth_not_None"
+    elif my_type == DatasetType.RAW:
+        return "job_log_data", "sth_not_None"
+    else:
+        raise ValueError(my_type, " is not valid DatasetType.")
+
+
+@given(initial=sst.datasets(for_upload=True))
+@settings(max_examples=10)
+def test_dataset_dict_like_keys_per_type(initial: Dataset) -> None:
+    my_names = set(
+        field.name for field in Dataset._FIELD_SPEC if field.used_by(initial.type)
+    )
+    assert set(initial.keys()) == my_names
+
+
+@given(initial=sst.datasets(for_upload=True))
+@settings(max_examples=10)
+def test_dataset_dict_like_keys_including_invalid_field(initial):
+    invalid_name, invalid_value = invalid_field_example(initial.type)
+
+    my_names = set(
+        field.name for field in Dataset._FIELD_SPEC if field.used_by(initial.type)
+    )
+    assert invalid_name not in my_names
+    my_names.add(invalid_name)
+
+    setattr(initial, invalid_name, invalid_value)
+
+    assert set(initial.keys()) == my_names
+
+
+@given(initial=sst.datasets(for_upload=True))
+@settings(max_examples=10)
+def test_dataset_dict_like_values(initial: Dataset) -> None:
+    for key, value in zip(initial.keys(), initial.values()):
+        assert value == getattr(initial, key)
+
+
+@given(initial=sst.datasets(for_upload=True))
+@settings(max_examples=10)
+def test_dataset_dict_like_values_with_invalid_field(initial: Dataset) -> None:
+    setattr(initial, *invalid_field_example(initial.type))
+    for key, value in zip(initial.keys(), initial.values()):
+        assert value == getattr(initial, key)
+
+
+@given(initial=sst.datasets(for_upload=True))
+@settings(max_examples=10)
+def test_dataset_dict_like_items_with_invalid_field(initial: Dataset) -> None:
+    setattr(initial, *invalid_field_example(initial.type))
+    for key, value in initial.items():
+        assert value == getattr(initial, key)
+
+
+@given(initial=sst.datasets(for_upload=True))
+@settings(max_examples=10)
+def test_dataset_dict_like_getitem(initial):
+    assert initial["type"] == initial.type
+
+
+@pytest.mark.parametrize(
+    ("is_attr", "wrong_field"), ((True, "size"), (False, "OBVIOUSLYWRONGNAME"))
+)
+@given(initial=sst.datasets(for_upload=True))
+@settings(max_examples=10)
+def test_dataset_dict_like_getitem_wrong_field_raises(initial, is_attr, wrong_field):
+    # 'size' should be included in the field later.
+    # It is now excluded because it is ``manual`` field. See issue#151.
+    assert hasattr(initial, wrong_field) == is_attr
+    with pytest.raises(KeyError, match=f"{wrong_field} is not a valid field name."):
+        initial[wrong_field]
+
+
+@given(initial=sst.datasets(for_upload=True))
+@settings(max_examples=10)
+def test_dataset_dict_like_setitem(initial: Dataset) -> None:
+    import uuid
+
+    sample_comment = uuid.uuid4().hex
+    assert initial["comment"] != sample_comment
+    initial["comment"] = sample_comment
+    assert initial["comment"] == sample_comment
+
+
+@given(initial=sst.datasets(for_upload=True))
+@settings(max_examples=10)
+def test_dataset_dict_like_setitem_invalid_field(initial: Dataset) -> None:
+    # ``__setitem__`` doesn't check if the item is invalid for the current type or not.
+    invalid_field, invalid_value = invalid_field_example(initial.type)
+    assert initial[invalid_field] is None
+    initial[invalid_field] = invalid_value
+    assert initial[invalid_field] == invalid_value
+
+
+@pytest.mark.parametrize(
+    ("is_attr", "wrong_field", "wrong_value"),
+    ((True, "size", 10), (False, "OBVIOUSLYWRONGNAME", "OBVIOUSLYWRONGVALUE")),
+)
+@given(initial=sst.datasets(for_upload=True))
+@settings(max_examples=10)
+def test_dataset_dict_like_setitem_wrong_field_raises(
+    initial, is_attr, wrong_field, wrong_value
+):
+    # ``manual`` fields such as ``size`` should raise with ``__setitem__``.
+    # However, it may need more specific error message.
+    assert hasattr(initial, wrong_field) == is_attr
+    with pytest.raises(KeyError, match=f"{wrong_field} is not a valid field name."):
+        initial[wrong_field] = wrong_value
```

### Comparing `scitacean-23.8.0/tests/download_test.py` & `scitacean-24.4.0/tests/download_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 import hashlib
 import re
 from contextlib import contextmanager
+from copy import deepcopy
 from pathlib import Path
-from typing import Union
 
 import pytest
 from dateutil.parser import parse as parse_date
 
 from scitacean import PID, Client, Dataset, DatasetType, File, IntegrityError
 from scitacean.filesystem import RemotePath
 from scitacean.logging import logger_name
@@ -52,14 +52,18 @@
         ownerGroup="faculty",
         packedSize=0,
         pid=PID(prefix="UU.000", pid="5125.ab.663.8c9f"),
         principalInvestigator="m.ridcully@uu.am",
         size=sum(f.size for f in data_files[0]),
         sourceFolder=RemotePath("/src/stibbons/774"),
         type=DatasetType.RAW,
+        scientificMetadata={
+            "height": {"value": 0.3, "unit": "m"},
+            "mass": "hefty",
+        },
     )
     block = DownloadOrigDatablock(
         chkAlg="md5",
         ownerGroup="faculty",
         size=sum(f.size for f in data_files[0]),
         datasetId=PID(prefix="UU.000", pid="5125.ab.663.8c9f"),
         _id="0941.66.abff.41de",
@@ -69,15 +73,15 @@
         dataset_model=model, orig_datablock_models=[block]
     )
     return dset, {
         dset.source_folder / name: content for name, content in data_files[1].items()
     }
 
 
-def load(name: Union[str, Path]) -> bytes:
+def load(name: str | Path) -> bytes:
     with open(name, "rb") as f:
         return f.read()
 
 
 def test_download_files_creates_local_files_select_all(fs, dataset_and_files):
     dataset, contents = dataset_and_files
     client = Client.without_login(
@@ -184,19 +188,26 @@
     assert load("download/file1.dat") == contents["/src/stibbons/774/file1.dat"]
     assert not Path("download/log/what-happened.log").exists()
     assert not Path("download/thaum.dat").exists()
 
 
 def test_download_files_returns_updated_dataset(fs, dataset_and_files):
     dataset, contents = dataset_and_files
+    original = deepcopy(dataset)
     client = Client.without_login(
         url="/", file_transfer=FakeFileTransfer(fs=fs, files=contents)
     )
     finalized = client.download_files(dataset, target="./download")
 
+    assert dataset == original
+    assert all(
+        getattr(finalized, field.name) == getattr(original, field.name)
+        for field in original.fields()
+    )
+    assert finalized.meta == original.meta
     for f in finalized.files:
         assert f.is_on_local
     for f in dataset.files:
         assert not f.is_on_local  # original is unchanged
 
 
 def test_download_files_ignores_checksum_if_alg_is_none(fs, dataset_and_files):
```

### Comparing `scitacean-23.8.0/tests/file_test.py` & `scitacean-24.4.0/tests/file_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 import hashlib
 from dataclasses import replace
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
 
 import pytest
 from dateutil.parser import parse as parse_date
@@ -109,14 +109,65 @@
     file = File.from_local(
         Path("data", "subdir", "file.dat"), base_path=Path("data") / "subdir"
     )
     assert file.remote_path == RemotePath("file.dat")
     assert file.make_model().path == "file.dat"
 
 
+def test_file_from_remote_default_args():
+    file = File.from_remote(
+        remote_path="/remote/source/file.nxs",
+        size=6123,
+        creation_time="2023-09-27T16:00:15Z",
+    )
+    assert file.local_path is None
+    assert isinstance(file.remote_path, RemotePath)
+    assert file.remote_path == "/remote/source/file.nxs"
+    assert file.size == 6123
+    assert isinstance(file.creation_time, datetime)
+    assert file.creation_time == parse_date("2023-09-27T16:00:15Z")
+    assert file.checksum() is None
+    assert file.checksum_algorithm is None
+    assert file.remote_uid is None
+    assert file.remote_gid is None
+    assert file.remote_perm is None
+
+
+def test_file_from_remote_all_args():
+    file = File.from_remote(
+        remote_path="/remote/image.png",
+        size=9,
+        creation_time=parse_date("2023-10-09T08:12:59Z"),
+        checksum="abcde",
+        checksum_algorithm="md5",
+        remote_uid="user-usy",
+        remote_gid="groupy-group",
+        remote_perm="wrx",
+    )
+    assert file.local_path is None
+    assert file.remote_path == "/remote/image.png"
+    assert file.size == 9
+    assert file.creation_time == parse_date("2023-10-09T08:12:59Z")
+    assert file.checksum() == "abcde"
+    assert file.checksum_algorithm == "md5"
+    assert file.remote_uid == "user-usy"
+    assert file.remote_gid == "groupy-group"
+    assert file.remote_perm == "wrx"
+
+
+def test_file_from_remote_checksum_requires_algorithm():
+    with pytest.raises(TypeError, match="checksum"):
+        File.from_remote(
+            remote_path="/remote/image.png",
+            size=9,
+            creation_time="2023-10-09T08:12:59Z",
+            checksum="abcde",
+        )
+
+
 def test_file_from_download_model():
     model = DownloadDataFile(
         path="dir/image.jpg", size=12345, time=parse_date("2022-06-22T15:42:53.123Z")
     )
     file = File.from_download_model(model)
 
     assert file.remote_access_path("/remote/folder") == "/remote/folder/dir/image.jpg"
```

### Comparing `scitacean-23.8.0/tests/filesystem_test.py` & `scitacean-24.4.0/tests/filesystem_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 import hashlib
 from datetime import datetime, timedelta, timezone
 from pathlib import Path, PurePath, PurePosixPath, PureWindowsPath
 
 import pytest
 from hypothesis import given
 from hypothesis import strategies as st
```

### Comparing `scitacean-23.8.0/tests/html_repr/html_repr_test.py` & `scitacean-24.4.0/tests/html_repr/html_repr_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 from scitacean import Attachment, Dataset, RemotePath, Thumbnail
 
 
 # We don't want to test the concrete layout as that may change
 # without breaking anything. So just make sure that the result
 # contains the relevant data.
@@ -34,11 +34,12 @@
     att = Attachment(
         caption="THE_CAPTION.jpg",
         owner_group="ThePeople",
         thumbnail=Thumbnail(mime="image/jpeg", _encoded_data="YWJjZA=="),
     )
 
     res = att._repr_html_()
+    assert isinstance(res, str)
 
     assert "THE_CAPTION.jpg" in res
     assert "ThePeople" in res
     assert "YWJjZA==" in res
```

### Comparing `scitacean-23.8.0/tests/model_test.py` & `scitacean-24.4.0/tests/model_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 import dataclasses
-from typing import Type, TypeVar
+from typing import TypeVar
 
 import pytest
 from dateutil.parser import parse as parse_date
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 from scitacean import PID, DatasetType, RemotePath, model
@@ -16,15 +16,15 @@
     UploadDerivedDataset,
     UploadRawDataset,
 )
 
 T = TypeVar("T")
 
 
-def build_user_model_for_upload(cls: Type[T]) -> st.SearchStrategy[T]:
+def build_user_model_for_upload(cls: type[T]) -> st.SearchStrategy[T]:
     private_fields = {
         field.name: st.none()
         for field in dataclasses.fields(cls)  # type: ignore[arg-type]
         if field.name.startswith("_")
     }
     return st.builds(cls, **private_fields)
```

### Comparing `scitacean-23.8.0/tests/testing/strategies_test.py` & `scitacean-24.4.0/tests/testing/strategies_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 from dateutil.parser import parse as parse_datetime
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 from scitacean import PID, DatasetType
 from scitacean.testing import strategies as sst
```

### Comparing `scitacean-23.8.0/tests/thumbnail_test.py` & `scitacean-24.4.0/tests/thumbnail_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 import pytest
 
 from scitacean import Thumbnail
 
 
 def test_mime_type():
```

### Comparing `scitacean-23.8.0/tests/transfer/sftp_test.py` & `scitacean-24.4.0/tests/transfer/sftp_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2022 Scitacean contributors (https://github.com/SciCatProject/scitacean)
 # mypy: disable-error-code="no-untyped-def, return-value, arg-type, union-attr"
 
 import dataclasses
 import tempfile
+from collections.abc import Iterator
 from contextlib import contextmanager
 from datetime import datetime, timedelta, timezone
 from pathlib import Path
-from typing import Iterator
 
 import paramiko
 import pytest
 
 from scitacean import Dataset, File, RemotePath
 from scitacean.testing.client import FakeClient
 from scitacean.testing.sftp import IgnorePolicy, skip_if_not_sftp
@@ -275,15 +275,15 @@
     assert datetime.now(tz=timezone.utc) - uploaded.creation_time < timedelta(seconds=5)
 
 
 class CorruptingSFTP(paramiko.SFTPClient):
     """Appends bytes to uploaded files to simulate a broken transfer."""
 
     def put(self, localpath, remotepath, callback=None, confirm=True):
-        with open(localpath, "r") as f:
+        with open(localpath) as f:
             content = f.read()
         with tempfile.TemporaryDirectory() as tempdir:
             corrupted_path = Path(tempdir) / "corrupted"
             with open(corrupted_path, "w") as f:
                 f.write(content + "\nevil bytes")
             super().put(str(corrupted_path), remotepath, callback, confirm)
```

### Comparing `scitacean-23.8.0/tests/upload_test.py` & `scitacean-24.4.0/tests/upload_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 from contextlib import contextmanager
+from typing import cast
 
 import pytest
 from dateutil.parser import parse as parse_date
 
 from scitacean import (
+    PID,
     Attachment,
     Client,
     Dataset,
     DatasetType,
+    File,
     ScicatCommError,
     Thumbnail,
 )
 from scitacean.testing.client import FakeClient
 from scitacean.testing.transfer import FakeFileTransfer
 
 from .common.files import make_file
@@ -118,14 +121,96 @@
         }
     )
     assert finalized == expected
     with pytest.raises(ScicatCommError):
         client.scicat.get_orig_datablocks(finalized.pid)
 
 
+def test_upload_without_files_does_not_need_file_transfer(dataset):
+    client = FakeClient()
+    finalized = client.upload_new_dataset_now(dataset)
+    pid = cast(PID, finalized.pid)
+    expected = client.get_dataset(pid, attachments=True).replace(
+        # The backend may update the dataset after upload
+        _read_only={
+            "updated_at": finalized.updated_at,
+            "updated_by": finalized.updated_by,
+        }
+    )
+    assert finalized == expected
+    with pytest.raises(ScicatCommError):
+        client.scicat.get_orig_datablocks(pid)
+
+
+def test_upload_without_files_does_not_need_revert_files(dataset):
+    client = FakeClient(
+        disable={"create_dataset_model": ScicatCommError("Ingestion failed")}
+    )
+    with pytest.raises(ScicatCommError):
+        # Does not raise from attempting to access the file transfer.
+        client.upload_new_dataset_now(dataset)
+
+
+def test_upload_with_only_remote_files_does_not_need_file_transfer(dataset):
+    dataset.add_files(
+        File.from_remote(
+            remote_path="source/file1.h5", size=512, creation_time=dataset.creation_time
+        )
+    )
+
+    client = FakeClient()
+    finalized = client.upload_new_dataset_now(dataset)
+    pid = cast(PID, finalized.pid)
+    expected = client.get_dataset(pid, attachments=True).replace(
+        # The backend may update the dataset after upload
+        _read_only={
+            "updated_at": finalized.updated_at,
+            "updated_by": finalized.updated_by,
+        }
+    )
+    assert finalized == expected
+
+
+def test_upload_with_both_remote_and_local_files(client, dataset_with_files):
+    original_file_names = set(
+        dataset_with_files.source_folder / file.remote_path
+        for file in dataset_with_files.files
+    )
+    dataset_with_files.add_files(
+        File.from_remote(
+            remote_path="file1.h5", size=6123, creation_time="2019-09-09T19:29:39Z"
+        )
+    )
+
+    finalized = client.upload_new_dataset_now(dataset_with_files)
+    expected = client.get_dataset(finalized.pid, attachments=True).replace(
+        # The backend may update the dataset after upload
+        _read_only={
+            "updated_at": finalized.updated_at,
+            "updated_by": finalized.updated_by,
+        }
+    )
+    assert finalized == expected
+    # Does not include the remote file "file1.h5"
+    assert get_file_transfer(client).files.keys() == original_file_names
+
+
+def test_upload_with_file_with_both_remote_and_local_path(client, dataset_with_files):
+    file = File.from_remote(
+        remote_path="file1.h5", size=6123, creation_time="2019-09-09T19:29:39Z"
+    )
+    file = file.downloaded(local_path="/local/file1.h5")
+    dataset_with_files.add_files(file)
+
+    # Client w/o file transfer to ensure that the client never attempts to upload.
+    client = FakeClient()
+    with pytest.raises(ValueError, match="path"):
+        client.upload_new_dataset_now(dataset_with_files)
+
+
 def test_upload_creates_dataset_and_datablock(client, dataset_with_files):
     finalized = client.upload_new_dataset_now(dataset_with_files)
     assert client.datasets[finalized.pid].createdAt == finalized.created_at
     assert client.datasets[finalized.pid].datasetName == finalized.name
     assert client.datasets[finalized.pid].owner == finalized.owner
     assert client.datasets[finalized.pid].size == finalized.size
 
@@ -190,14 +275,28 @@
     )
     with pytest.raises(ScicatCommError):
         client.upload_new_dataset_now(dataset_with_files)
 
     assert not get_file_transfer(client).files
 
 
+def test_upload_does_not_create_dataset_if_validation_fails(dataset_with_files, fs):
+    client = FakeClient(
+        disable={"validate_dataset_model": ValueError("Validation failed")},
+        file_transfer=FakeFileTransfer(fs=fs),
+    )
+    with pytest.raises(ValueError):
+        client.upload_new_dataset_now(dataset_with_files)
+
+    assert not client.datasets
+    assert not client.orig_datablocks
+    assert not client.attachments
+    assert not get_file_transfer(client).files
+
+
 def test_failed_datablock_upload_does_not_revert(dataset_with_files, fs):
     client = FakeClient(
         disable={"create_orig_datablock": ScicatCommError("Ingestion failed")},
         file_transfer=FakeFileTransfer(fs=fs),
     )
     with pytest.raises(RuntimeError):
         client.upload_new_dataset_now(dataset_with_files)
```

### Comparing `scitacean-23.8.0/tests/util/formatter_test.py` & `scitacean-24.4.0/tests/util/formatter_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 import pytest
 
 from scitacean import PID, Dataset
 from scitacean.util.formatter import DatasetPathFormatter
```

### Comparing `scitacean-23.8.0/tools/model-generation/README.md` & `scitacean-24.4.0/tools/model-generation/README.md`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/tools/model-generation/generate_models.py` & `scitacean-24.4.0/tools/model-generation/generate_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 
 """Generate Python classes for SciCat models."""
+
 import argparse
 import subprocess
 import tempfile
+from collections.abc import Generator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Dict, Generator
+from typing import Any
 
 from jinja2 import Environment, FileSystemLoader, Template
 from spec import DatasetSpec, Spec, load_specs
 from templates import BANNER
 
 # Set to the URL of the JSON schema.
 # See the README for details.
@@ -56,29 +58,29 @@
     return _template("model")
 
 
 def _dataset_fields_template() -> Template:
     return _template("dataset_fields")
 
 
-def generate_models(specs: Dict[str, Spec]) -> str:
+def generate_models(specs: dict[str, Spec]) -> str:
     specs = dict(specs)
     dset_spec = specs.pop("Dataset")
     return _model_template().render(banner=BANNER, specs=specs, dset_spec=dset_spec)
 
 
 def generate_dataset_fields(dset_spec: DatasetSpec) -> str:
     return _dataset_fields_template().render(banner=BANNER, spec=dset_spec)
 
 
-def format_with_black(path: Path) -> None:
+def format_with_ruff(path: Path) -> None:
     # Root of Scitacean repo
     base_path = Path(__file__).resolve().parent.parent.parent
     subprocess.check_call(
-        ["black", path.resolve().relative_to(base_path)],  # noqa: S603, S607
+        ["ruff", "format", path.resolve().relative_to(base_path)],  # noqa: S603, S607
         cwd=base_path,
     )
 
 
 @contextmanager
 def _scicat_backend() -> Generator[None, None, None]:
     from scitacean.testing import backend
@@ -90,15 +92,15 @@
         try:
             backend.wait_until_backend_is_live(max_time=20, n_tries=20)
             yield
         finally:
             backend.stop_backend(docker_file)
 
 
-def load(real_backend: bool) -> Dict[str, Any]:
+def load(real_backend: bool) -> dict[str, Any]:
     if not real_backend:
         return load_specs(SCHEMA_URL)
 
     with _scicat_backend():
         from scitacean.testing.backend import config
 
         return load_specs(f"http://localhost:{config.SCICAT_PORT}/explorer-json")
@@ -107,16 +109,16 @@
 def main() -> None:
     args = _parse_args()
     specs = load(args.launch_scicat)
     dset_spec = specs["Dataset"]
 
     with open(MODEL_OUT_PATH, "w") as f:
         f.write(generate_models(specs))
-    format_with_black(MODEL_OUT_PATH)
+    format_with_ruff(MODEL_OUT_PATH)
 
     with open(DSET_FIELDS_OUT_PATH, "w") as f:
         f.write(generate_dataset_fields(dset_spec))
-    format_with_black(DSET_FIELDS_OUT_PATH)
+    format_with_ruff(DSET_FIELDS_OUT_PATH)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `scitacean-23.8.0/tools/model-generation/spec/__init__.py` & `scitacean-24.4.0/tools/model-generation/spec/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Load model specifications."""
+
 import dataclasses
 import re
 import sys
 from copy import deepcopy
 from functools import lru_cache
 from pathlib import Path
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Any, Literal
 
 import yaml
 
 from .schema import Schema, SchemaField, load_schemas
 
 
 @dataclasses.dataclass
 class _UpDownSchemas:
     download: Schema
-    upload: Optional[Schema]
+    upload: Schema | None
 
 
 @dataclasses.dataclass
 class _DatasetSchemas:
     download: Schema
     upload_derived: Schema
     upload_raw: Schema
@@ -30,18 +31,18 @@
 @dataclasses.dataclass
 class SpecField:
     name: str
     scicat_name: str
     description: str
     type: str
     required: bool  # Required in upload.
-    default: Optional[str] = None
+    default: str | None = None
     upload: bool = False
     download: bool = False
-    validation: Optional[str] = None
+    validation: str | None = None
 
     def full_type_for(self, kind: Literal["download", "upload", "user"]) -> str:
         return (
             self.type_for(kind)
             if self.required and kind != "download"
             else f"Optional[{self.type_for(kind)}]"
         )
@@ -61,31 +62,31 @@
         return self.type
 
 
 @dataclasses.dataclass
 class Spec:
     name: str
     download_name: str = dataclasses.field(init=False)
-    upload_name: Optional[str] = dataclasses.field(init=False)
-    fields: Dict[str, SpecField]
-    masked_fields_download: Dict[str, SpecField] = dataclasses.field(init=False)
-    masked_fields_upload: Dict[str, SpecField] = dataclasses.field(init=False)
+    upload_name: str | None = dataclasses.field(init=False)
+    fields: dict[str, SpecField]
+    masked_fields_download: dict[str, SpecField] = dataclasses.field(init=False)
+    masked_fields_upload: dict[str, SpecField] = dataclasses.field(init=False)
 
     def __post_init__(self) -> None:
         if _SCHEMA_GROUPS.get(self.name, (None, None))[0]:
             self.upload_name = f"Upload{self.name}"
         else:
             self.upload_name = None
         self.download_name = f"Download{self.name}"
         self.masked_fields_download = {}
         self.masked_fields_upload = {}
 
     def fields_for(
         self, kind: Literal["download", "upload", "user"]
-    ) -> List[SpecField]:
+    ) -> list[SpecField]:
         return sorted(
             sorted(
                 filter(
                     lambda field: (kind == "download" and field.download)
                     or (kind == "upload" and field.upload)
                     or (kind == "user"),
                     self.fields.values(),
@@ -100,45 +101,45 @@
 class DatasetFieldConversion:
     func: str
     arg_type: str
 
 
 @dataclasses.dataclass
 class DatasetField(SpecField):
-    conversion: Optional[DatasetFieldConversion] = None
-    default: Optional[Any] = None
+    conversion: DatasetFieldConversion | None = None
+    default: Any | None = None
     manual: bool = False
 
     # These are only used for upload models.
     # For downloads, all fields should be considered as used.
     used_by_derived: bool = False
     used_by_raw: bool = False
 
 
 @dataclasses.dataclass
 class DatasetSpec(Spec):
     download_name: str = dataclasses.field(default="DownloadDataset", init=False)
-    upload_name: Optional[str] = dataclasses.field(default="UploadDataset", init=False)
-    fields: Dict[str, DatasetField]
+    upload_name: str | None = dataclasses.field(default="UploadDataset", init=False)
+    fields: dict[str, DatasetField]
 
     def dset_fields_for(
         self,
         kind: Literal["download", "upload", "user"],
         dset_type: Literal["derived", "raw"],
-    ) -> List[DatasetField]:
+    ) -> list[DatasetField]:
         return list(
             filter(
                 lambda field: field.used_by_derived
                 if dset_type == "derived"
                 else field.used_by_raw,
                 self.fields_for(kind),
             )
         )
 
-    def user_dset_fields(self, manual: Optional[bool] = None) -> List[DatasetField]:
+    def user_dset_fields(self, manual: bool | None = None) -> list[DatasetField]:
         if manual is None:
             return list(self.fields.values())
         return [field for field in self.fields.values() if field.manual == manual]
 
 
 _SCHEMA_GROUPS = {
     "Attachment": ("CreateAttachmentDto", "Attachment"),
@@ -151,16 +152,16 @@
     "DataFile": ("DataFile", "DataFile"),
     "Instrument": (None, "Instrument"),
     "Sample": ("CreateSampleDto", "SampleClass"),
 }
 
 
 def _collect_schemas(
-    schemas: Dict[str, Schema]
-) -> Dict[str, Union[_UpDownSchemas, _DatasetSchemas]]:
+    schemas: dict[str, Schema],
+) -> dict[str, _UpDownSchemas | _DatasetSchemas]:
     return {
         "Dataset": _DatasetSchemas(
             upload_derived=schemas["CreateDerivedDatasetDto"],
             upload_raw=schemas["CreateRawDatasetDto"],
             download=schemas["DatasetClass"],
         ),
         **{
@@ -199,15 +200,15 @@
                     f"Mismatch in field {name}:\n"
                     f" {source_key}:\n {val}\n {key}:\n {getattr(field, name)}\n"
                 )
     return val
 
 
 def _merge_field(
-    name: str, download: Optional[SchemaField], upload: Optional[SchemaField]
+    name: str, download: SchemaField | None, upload: SchemaField | None
 ) -> SpecField:
     fields = {"download": download, "upload": upload}
     return SpecField(
         name=_camel_case_to_snake_case(_get_common_field_attr("name", **fields)),
         scicat_name=name,
         description=_get_common_field_attr(
             "description", allow_mismatch=True, **fields
@@ -237,17 +238,17 @@
         name=name,
         fields=fields,
     )
 
 
 def _merge_dataset_field(
     name: str,
-    download: Optional[SchemaField],
-    raw_upload: Optional[SchemaField],
-    derived_upload: Optional[SchemaField],
+    download: SchemaField | None,
+    raw_upload: SchemaField | None,
+    derived_upload: SchemaField | None,
 ) -> DatasetField:
     fields = {
         "download": download,
         "raw_upload": raw_upload,
         "derived_upload": derived_upload,
     }
     required = (raw_upload is not None and raw_upload.required) or (
@@ -286,16 +287,16 @@
     return DatasetSpec(
         name=name,
         fields=fields,
     )
 
 
 @lru_cache
-def _masked_fields() -> Dict[str, List[str]]:
-    with open(Path(__file__).resolve().parent / "masked-fields.yml", "r") as f:
+def _masked_fields() -> dict[str, list[str]]:
+    with open(Path(__file__).resolve().parent / "masked-fields.yml") as f:
         return yaml.safe_load(f)
 
 
 def _mask_fields(spec: Spec) -> Spec:
     spec = deepcopy(spec)
     masked = _masked_fields()
     for field_name in masked.get(spec.name, []):
@@ -311,30 +312,30 @@
         else:
             spec.masked_fields_upload[field_name] = spec.fields[field_name]
             spec.masked_fields_download[field_name] = spec.fields.pop(field_name)
     return spec
 
 
 @lru_cache
-def _field_name_overrides() -> Dict[str, Dict[str, str]]:
-    with open(Path(__file__).resolve().parent / "field-name-overrides.yml", "r") as f:
+def _field_name_overrides() -> dict[str, dict[str, str]]:
+    with open(Path(__file__).resolve().parent / "field-name-overrides.yml") as f:
         return yaml.safe_load(f)
 
 
 def _postprocess_field_names(spec: Spec) -> Spec:
     spec = deepcopy(spec)
     overrides = _field_name_overrides()
     for field_name, override in overrides.get(spec.name, {}).items():
         spec.fields[field_name].name = override
     return spec
 
 
 @lru_cache
-def _field_type_overrides() -> Dict[str, Dict[str, str]]:
-    with open(Path(__file__).resolve().parent / "field-type-overrides.yml", "r") as f:
+def _field_type_overrides() -> dict[str, dict[str, str]]:
+    with open(Path(__file__).resolve().parent / "field-type-overrides.yml") as f:
         return yaml.safe_load(f)
 
 
 def _postprocess_field_types(spec: Spec) -> Spec:
     spec = deepcopy(spec)
 
     # Convert type names in the schema to Scitacean class names.
@@ -347,16 +348,16 @@
     overrides = _field_type_overrides()
     for field_name, override in overrides.get(spec.name, {}).items():
         spec.fields[field_name].type = override
     return spec
 
 
 @lru_cache
-def _field_validations() -> Dict[str, Dict[str, str]]:
-    with open(Path(__file__).resolve().parent / "field-validations.yml", "r") as f:
+def _field_validations() -> dict[str, dict[str, str]]:
+    with open(Path(__file__).resolve().parent / "field-validations.yml") as f:
         return yaml.safe_load(f)
 
 
 def _assign_validations(spec: Spec) -> Spec:
     validations = _field_validations()
     if spec.name not in validations:
         return spec
@@ -368,16 +369,16 @@
                 spec.fields[field_name].type = "NonNegativeInt"
             else:
                 spec.fields[field_name].validation = validation
     return spec
 
 
 @lru_cache
-def _dataset_field_customizations() -> Dict[str, Any]:
-    with open(Path(__file__).resolve().parent / "dataset-fields.yml", "r") as f:
+def _dataset_field_customizations() -> dict[str, Any]:
+    with open(Path(__file__).resolve().parent / "dataset-fields.yml") as f:
         return yaml.safe_load(f)
 
 
 def _extend_dataset_fields(spec: DatasetSpec) -> DatasetSpec:
     customizations = _dataset_field_customizations()
     spec = deepcopy(spec)
 
@@ -387,15 +388,15 @@
         if (conv := customizations["conversions"].get(name)) is not None:
             field.conversion = DatasetFieldConversion(**conv)
         if name in customizations["extra_read_only"]:
             field.upload = False
     return spec
 
 
-def load_specs(schema_url: str) -> Dict[str, Any]:
+def load_specs(schema_url: str) -> dict[str, Any]:
     schemas = _collect_schemas(load_schemas(schema_url))
     dataset_schema = schemas.pop("Dataset")
     specs = {
         "Dataset": _extend_dataset_fields(
             _build_dataset_spec("Dataset", dataset_schema)
         ),
         **{name: _build_spec(name, updown) for name, updown in schemas.items()},
```

### Comparing `scitacean-23.8.0/tools/model-generation/spec/dataset-fields.yml` & `scitacean-24.4.0/tools/model-generation/spec/dataset-fields.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/tools/model-generation/spec/field-validations.yml` & `scitacean-24.4.0/tools/model-generation/spec/field-validations.yml`

 * *Files identical despite different names*

### Comparing `scitacean-23.8.0/tools/model-generation/spec/schema.py` & `scitacean-24.4.0/tools/model-generation/spec/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Load schemas from a SciCat API."""
 
 import dataclasses
-from typing import Any, Dict, Optional
+from typing import Any
 
 import requests
 
 
 @dataclasses.dataclass
 class SchemaField:
     name: str
     description: str
     type: str
     required: bool
-    default: Optional[str]
+    default: str | None
 
 
 @dataclasses.dataclass
 class Schema:
     name: str
-    fields: Dict[str, SchemaField]
+    fields: dict[str, SchemaField]
 
 
-def parse_field_type(spec: Dict[str, Any]):
+def parse_field_type(spec: dict[str, Any]):
     if "allOf" in spec:
         if len(spec["allOf"]) != 1:
             raise ValueError("More than one alternative type in 'allOf'")
         return parse_field_type(spec["allOf"][0])
     if "$ref" in spec:
         return spec["$ref"].rsplit("/", 1)[1]
     if "enum" in spec:
@@ -45,45 +45,45 @@
     if spec["type"] == "array":
         return "List[{}]".format(parse_field_type(spec["items"]))
     if spec["type"] == "object":
         return "Dict[str, Any]"
     raise ValueError(f"Unknown field type: {spec['type']}")
 
 
-def parse_schema_fields(spec: Dict[str, Any]) -> Dict[str, SchemaField]:
+def parse_schema_fields(spec: dict[str, Any]) -> dict[str, SchemaField]:
     return {
         name: SchemaField(
             name=name,
             description=field_spec.get("description", ""),
             type=parse_field_type(field_spec),
             required=name in spec.get("required", ()),
             default=field_spec.get("default", None),
         )
         for name, field_spec in spec["properties"].items()
     }
 
 
-def parse_schemas(spec: Dict[str, Any]) -> Dict[str, Schema]:
+def parse_schemas(spec: dict[str, Any]) -> dict[str, Schema]:
     schemas = {}
     for name, field_spec in spec.items():
         print(f"Parsing schema {name}")  # noqa: T201
         schemas[name] = Schema(name=name, fields=parse_schema_fields(field_spec))
     return schemas
 
 
-def fetch_specs(url: str) -> Dict[str, Any]:
+def fetch_specs(url: str) -> dict[str, Any]:
     """Download the raw schema JSON from the API.
 
     ``url`` needs to point to a 'json-explorer' of a SciCat backend with version >= 4.
     E.g. ``http://localhost:3000/explorer-json`` for a locally running instance.
     """
     response = requests.get(url, timeout=10)
     if not response.ok:
         raise RuntimeError(
             f"Failed to fetch specs: {response.status_code} {response.reason}"
         )
     return response.json()
 
 
-def load_schemas(url: str) -> Dict[str, Schema]:
+def load_schemas(url: str) -> dict[str, Schema]:
     spec_json = fetch_specs(url)
     return parse_schemas(spec_json["components"]["schemas"])
```

### Comparing `scitacean-23.8.0/tools/model-generation/templates/__init__.py` & `scitacean-24.4.0/tools/model-generation/templates/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Templates to generate models and other classes."""
 
 from pathlib import Path
 from string import Template
 
 TEMPLATE_DIR = Path(__file__).resolve().parent
 
@@ -11,9 +11,9 @@
 # This file was automatically generated. #
 # Do not modify it directly!             #
 ##########################################
 """
 
 
 def load_template(name: str) -> Template:
-    with open(TEMPLATE_DIR / f"{name}.py.template", "r") as f:
+    with open(TEMPLATE_DIR / f"{name}.py.template") as f:
         return Template(f.read())
```

### Comparing `scitacean-23.8.0/tools/model-generation/templates/dataset_fields.py.jinja` & `scitacean-24.4.0/tools/model-generation/templates/dataset_fields.py.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 {%- else -%}
 {{ ty }}
 {%- endif -%}
 {% endmacro %}
 
 {{ banner }}
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 # flake8: noqa
 
 """Base class for Dataset."""
 
 from __future__ import annotations
 
 from datetime import datetime, timezone
@@ -189,19 +189,14 @@
         self._meta = meta
 
     @property
     def type(self) -> DatasetType:
         """Characterize type of dataset, either 'raw' or 'derived'. Autofilled when choosing the proper inherited models."""
         return self._type
 
-    @type.setter
-    def type(self, type: Union[DatasetType, Literal["raw", "derived"]]) -> None:
-        """Characterize type of dataset, either 'raw' or 'derived'. Autofilled when choosing the proper inherited models."""
-        self._type = DatasetType(type)
-
     @staticmethod
     def _prepare_fields_from_download(
         download_model: DownloadDataset
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         init_args = {}
         read_only = {}
         for field in DatasetBase._FIELD_SPEC:
```

### Comparing `scitacean-23.8.0/tools/model-generation/templates/model.py.jinja` & `scitacean-24.4.0/tools/model-generation/templates/model.py.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {%- macro validations(fields) %}
 {%- for validation in ("datetime", "drop", "emails", "orcids") %}
 {%- set fields = fields|selectattr("validation", "eq", validation)|list -%}
 {% if fields %}
 
-    @field_validator({{ fields|map("attr", "scicat_name")|map("quote")|join(", ") }}, mode="before")
+    @pydantic.field_validator({{ fields|map("attr", "scicat_name")|map("quote")|join(", ") }}, mode="before")
     def _validate_{{ validation }}(cls, value: Any) -> Any:
         return validate_{{ validation }}(value)
 {%- endif %}
 {%- endfor %}
 {% endmacro -%}
 
 {% macro mask_keyword(spec, kind) %}
@@ -28,15 +28,15 @@
 {%- else %}
     {{ field.scicat_name }}: {{ field.full_type_for(kind) }}{% if not field.required or kind == "download" %} = None{% endif -%}
 {%- endif -%}
 {% endmacro %}
 
 {{ banner }}
 # SPDX-License-Identifier: BSD-3-Clause
-# Copyright (c) 2023 SciCat Project (https://github.com/SciCatProject/scitacean)
+# Copyright (c) 2024 SciCat Project (https://github.com/SciCatProject/scitacean)
 """Models for communication with SciCat and user facing dataclasses.
 
 The high-level :class:`scitacean.Client` and :class:`scitacean.Dataset` return objects
 from the SciCat database in the form of 'user models'.
 Those are usually all that is required for working with Scitacean.
 
 At a lower level, those models are converted to or from upload or download models,
@@ -105,15 +105,14 @@
     construct,
     validate_datetime,
     validate_drop,
     validate_emails,
     validate_orcids,
 )
 from ._internal.dataclass_wrapper import dataclass_optional_args
-from ._internal.pydantic_compat import field_validator
 from .filesystem import RemotePath
 from .pid import PID
 from .thumbnail import Thumbnail
 
 {% set fields = dset_spec.fields_for("download") -%}
 class DownloadDataset(BaseModel{{ mask_keyword(dset_spec, "download") }}):
 {%- for field in fields -%}
```

