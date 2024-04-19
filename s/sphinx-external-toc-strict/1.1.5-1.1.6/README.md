# Comparing `tmp/sphinx_external_toc_strict-1.1.5.tar.gz` & `tmp/sphinx_external_toc_strict-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_external_toc_strict-1.1.5.tar", last modified: Fri Apr 19 04:38:51 2024, max compression
+gzip compressed data, was "sphinx_external_toc_strict-1.1.6.tar", last modified: Fri Apr 19 05:39:23 2024, max compression
```

## Comparing `sphinx_external_toc_strict-1.1.5.tar` & `sphinx_external_toc_strict-1.1.6.tar`

### file list

```diff
@@ -1,239 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.987968 sphinx_external_toc_strict-1.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.935968 sphinx_external_toc_strict-1.1.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.939967 sphinx_external_toc_strict-1.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/kit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/python-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/quality.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/test-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/testsuite.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    31595 2024-04-19 04:38:51.987968 sphinx_external_toc_strict-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.939967 sphinx_external_toc_strict-1.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/asset-gesture-like-thumbs-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/asset-table-of-contents.svg
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/credit.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/sphinx-external-toc-strict-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/sphinx-external-toc-strict-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   147326 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/toc-graphic.png
--rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/toc_tree.pptx
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/code/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/compat.rst
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/constrants.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/filename_suffix.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/parsing_shared.rst
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/parsing_strictyaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/pep518_read.rst
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/tools_strictyaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/version_semantic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/example/globfolder/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/example/globfolder/page1.rst
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/example/globfolder/page2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/example/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/example/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/example/subfolder/page.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-black.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-docutils-source.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1111839 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-python.txt
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-sphinx-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-strictyaml-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-strictyaml-source.txt
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-toc-strict.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/requirements.pip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/user_guide/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/user_guide/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/user_guide/regressions.md
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/user_guide/sphinx.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/user_guide/why.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/howto.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17383 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/igor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.947967 sphinx_external_toc_strict-1.1.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/dev.pip
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/kit.in
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/kit.pip
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/manage.in
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/manage.pip
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/mypy.pip
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/pins.pip
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/pip-tools.pip
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/pip.pip
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/prod.in
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/prod.pip
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/tox.pip
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 04:38:51.987968 sphinx_external_toc_strict-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.935968 sphinx_external_toc_strict-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.951968 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/filename_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/filename_suffix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_shared.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_strictyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/pep518_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/pep518_read.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19183 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/tools_strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/tools_strictyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/version_semantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/version_semantic.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.967967 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31595 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.955968 sphinx_external_toc_strict-1.1.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.955968 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/bad_option_value.yml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/bad_url.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/doc_multiple_times.yml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/doc_validation_fail.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/empty_items.yml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/empty_subtrees.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/entry_not_a_mapping.yml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/entry_unknown_link_type.yml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/file_and_glob_present.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/item_then_subtrees_key.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/items_in_glob.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/items_in_url.yml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/list.yml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/no_root.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/subtree_with_no_items.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/unknown_keys.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/unknown_keys_nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/unknown_usecase.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.959967 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/chapters.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/jb_docs_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/list_and_nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/numbered_chapters.yml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/numbered_depth.yml
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/numbered_depth_parts_subset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/numbered_parts.yml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/numbered_parts_subset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/parts.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/simple_dict.yml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/simple_list.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.959967 sphinx_external_toc_strict-1.1.5/tests/_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/basic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/basic_compressed.yml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/caption_not_entries.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/exclude_missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/glob.yml
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/glob_md.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/tableofcontents.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.959967 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/contains_toctree.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/file_not_in_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/multiple_tableofcontents.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/no_glob_match.yml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/tableofcontents_no_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.959967 sphinx_external_toc_strict-1.1.5/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_cli/test_create_toc.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_filename_suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.963967 sphinx_external_toc_strict-1.1.5/tests/test_parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_pep518_read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.963967 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_basic_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_basic_compressed_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_caption_not_entries_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_glob_md_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_tableofcontents_.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.967967 sphinx_external_toc_strict-1.1.5/tests/test_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_create_site_map_from_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_basic_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_chapters_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_list_and_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_numbered_chapters_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_numbered_depth_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_numbered_depth_parts_subset_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_numbered_parts_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_numbered_parts_subset_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_parts_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_simple_dict_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_simple_list_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_version_semantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.507507 sphinx_external_toc_strict-1.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.459507 sphinx_external_toc_strict-1.1.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.459507 sphinx_external_toc_strict-1.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.github/workflows/kit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.github/workflows/python-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.github/workflows/quality.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.github/workflows/test-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.github/workflows/testsuite.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31595 2024-04-19 05:39:23.507507 sphinx_external_toc_strict-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.463507 sphinx_external_toc_strict-1.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.463507 sphinx_external_toc_strict-1.1.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/_static/asset-gesture-like-thumbs-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/_static/asset-table-of-contents.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/_static/credit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/_static/sphinx-external-toc-strict-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/_static/sphinx-external-toc-strict-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   147326 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/_static/toc-graphic.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/_static/toc_tree.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.463507 sphinx_external_toc_strict-1.1.6/docs/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/compat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/constrants.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/filename_suffix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/parsing_shared.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/parsing_strictyaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/pep518_read.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/todo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/tools_strictyaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/code/version_semantic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.463507 sphinx_external_toc_strict-1.1.6/docs/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.467507 sphinx_external_toc_strict-1.1.6/docs/example/globfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/example/globfolder/page1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/example/globfolder/page2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/example/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.467507 sphinx_external_toc_strict-1.1.6/docs/example/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/example/subfolder/page.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-black.inv
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-black.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-docutils-source.inv
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-docutils-source.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   136075 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-python.inv
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-sphinx-docs.inv
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-sphinx-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-strictyaml-docs.inv
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-strictyaml-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-strictyaml-source.inv
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-strictyaml-source.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-toc-strict.inv
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/objects-toc-strict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/requirements.pip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.467507 sphinx_external_toc_strict-1.1.6/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/user_guide/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/user_guide/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/user_guide/regressions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/user_guide/sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/docs/user_guide/why.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/howto.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17383 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/igor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.467507 sphinx_external_toc_strict-1.1.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/dev.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/kit.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/kit.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/manage.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/manage.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/mypy.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/pins.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/pip-tools.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/pip.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/prod.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/prod.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/requirements/tox.pip
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 05:39:23.507507 sphinx_external_toc_strict-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.455507 sphinx_external_toc_strict-1.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.471507 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 05:39:23.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/filename_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/filename_suffix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/parsing_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/parsing_shared.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/parsing_strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/parsing_strictyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/pep518_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/pep518_read.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19183 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/tools_strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/tools_strictyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/version_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/version_semantic.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.487507 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31595 2024-04-19 05:39:23.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-19 05:39:23.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:39:23.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 05:39:23.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-19 05:39:23.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 05:39:23.000000 sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.475507 sphinx_external_toc_strict-1.1.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.475507 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/bad_option_value.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/bad_url.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/doc_multiple_times.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/doc_validation_fail.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/empty_items.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/empty_subtrees.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/entry_not_a_mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/entry_unknown_link_type.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/file_and_glob_present.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/item_then_subtrees_key.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/items_in_glob.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/items_in_url.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/list.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/no_root.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/subtree_with_no_items.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/unknown_keys.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/unknown_keys_nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_bad_toc_files/unknown_usecase.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.479507 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/chapters.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/jb_docs_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/list_and_nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/numbered_chapters.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/numbered_depth.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/numbered_depth_parts_subset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/numbered_parts.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/numbered_parts_subset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/parts.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/simple_dict.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/simple_list.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.479507 sphinx_external_toc_strict-1.1.6/tests/_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_toc_files/basic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_toc_files/basic_compressed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_toc_files/caption_not_entries.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_toc_files/exclude_missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_toc_files/glob.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_toc_files/glob_md.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_toc_files/nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_toc_files/tableofcontents.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.479507 sphinx_external_toc_strict-1.1.6/tests/_warning_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_warning_toc_files/contains_toctree.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_warning_toc_files/file_not_in_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_warning_toc_files/multiple_tableofcontents.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_warning_toc_files/no_glob_match.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/_warning_toc_files/tableofcontents_no_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.479507 sphinx_external_toc_strict-1.1.6/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_cli/test_create_toc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_filename_suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.483507 sphinx_external_toc_strict-1.1.6/tests/test_parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_create_toc_dict_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_create_toc_dict_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_create_toc_dict_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_create_toc_dict_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_create_toc_dict_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_create_toc_dict_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_create_toc_dict_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_create_toc_dict_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_pep518_read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.483507 sphinx_external_toc_strict-1.1.6/tests/test_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_sphinx/test_success_basic_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_sphinx/test_success_basic_compressed_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_sphinx/test_success_caption_not_entries_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_sphinx/test_success_glob_md_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_sphinx/test_success_tableofcontents_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:39:23.487507 sphinx_external_toc_strict-1.1.6/tests/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_create_site_map_from_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_file_to_sitemap_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_file_to_sitemap_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_file_to_sitemap_basic_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_file_to_sitemap_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_file_to_sitemap_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_file_to_sitemap_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_file_to_sitemap_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_file_to_sitemap_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_file_to_sitemap_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_chapters_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_list_and_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_numbered_chapters_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_numbered_depth_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_numbered_depth_parts_subset_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_numbered_parts_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_numbered_parts_subset_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_parts_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_simple_dict_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_simple_list_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tests/test_version_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-19 05:39:16.000000 sphinx_external_toc_strict-1.1.6/tox.ini
```

### Comparing `sphinx_external_toc_strict-1.1.5/.github/workflows/codeql-analysis.yml` & `sphinx_external_toc_strict-1.1.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/.github/workflows/dependency-review.yml` & `sphinx_external_toc_strict-1.1.6/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/.github/workflows/kit.yml` & `sphinx_external_toc_strict-1.1.6/.github/workflows/kit.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/.github/workflows/python-nightly.yml` & `sphinx_external_toc_strict-1.1.6/.github/workflows/python-nightly.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/.github/workflows/quality.yml` & `sphinx_external_toc_strict-1.1.6/.github/workflows/quality.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/.github/workflows/release.yml` & `sphinx_external_toc_strict-1.1.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/.github/workflows/test-coverage.yml` & `sphinx_external_toc_strict-1.1.6/.github/workflows/test-coverage.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/.github/workflows/testsuite.yml` & `sphinx_external_toc_strict-1.1.6/.github/workflows/testsuite.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/.gitignore` & `sphinx_external_toc_strict-1.1.6/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -130,8 +130,7 @@
 
 .vscode/
 ~$*
 
 # Removed from project
 retired/
 src/sphinx_external_toc_strict/_version.py
-docs/*.inv
```

### Comparing `sphinx_external_toc_strict-1.1.5/.pre-commit-config.yaml` & `sphinx_external_toc_strict-1.1.6/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -52,22 +52,7 @@
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.7.1
     hooks:
     - id: mypy
       pass_filenames: false
       entry: mypy src/sphinx_external_toc_strict/
-
-  - repo: local
-    hooks:
-      - id: remove-intersphinx-inventory-files
-        name: remove-intersphinx-inventory-files
-        entry: python igor.py quietly "make inv2txt" docs/
-        language: python
-        pass_filenames: false
-        description: >
-          Remove intersphinx .inv file that has corresponding .txt file
-        stages:
-        - commit
-        - merge-commit
-        - push
-        - manual
```

### Comparing `sphinx_external_toc_strict-1.1.5/.readthedocs.yml` & `sphinx_external_toc_strict-1.1.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/CHANGELOG.md` & `sphinx_external_toc_strict-1.1.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/CHANGES.rst` & `sphinx_external_toc_strict-1.1.6/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,31 @@
 
    Feature request
    .................
 
    Known regressions
    ..................
 
-   1. Dropped support for hidden document files
-
    Commit items for NEXT VERSION
    ..............................
 
 .. scriv-start-here
 
+.. _changes_1-1-6:
+
+Version 1.1.6 — 2024-04-19
+--------------------------
+
+- ci(.gitignore): remove ignore of docs/*.inv
+- ci(tox): in docs do not build_inv after clean_inv
+- ci(pre-commit): remove remove-intersphinx-inventory-files, need docs/*.inv
+- docs(Makefile): store *.inv needed by readthedocs
+- docs: remove objects-python.txt, excessive file size
+- docs: in code manual, add todo list page
+
 .. _changes_1-1-5:
 
 Version 1.1.5 — 2024-04-19
 --------------------------
 
 - docs(Makefile): for targets build_inv and clean_inv only use relative paths
 - docs(Makefile): for targets doctest and linkcheck require target build_inv
```

### Comparing `sphinx_external_toc_strict-1.1.5/CONTRIBUTING.md` & `sphinx_external_toc_strict-1.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/LICENSE` & `sphinx_external_toc_strict-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/Makefile` & `sphinx_external_toc_strict-1.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/NOTICE.txt` & `sphinx_external_toc_strict-1.1.6/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/PKG-INFO` & `sphinx_external_toc_strict-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-external-toc-strict
-Version: 1.1.5
+Version: 1.1.6
 Summary: A sphinx extension that allows the site-map to be defined in a single YAML file.
 Author-email: Dave Faulkmore <faulkmore@protonmail.com>
 License: MIT License
         
         Copyright (c) 2021 Executable Books
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sphinx_external_toc_strict-1.1.5/README.rst` & `sphinx_external_toc_strict-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/Makefile` & `sphinx_external_toc_strict-1.1.6/docs/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 .PHONY: html
 html:				## Sphinx build html. Only whats been changed
 ifeq ($(is_venv),1)
 	@$(SPHINXBUILDNOOPT) -b html "$(SOURCEDIR)" "$(BUILDDIR)/html"
 endif
 
 .PHONY: htmlall
-htmlall: build_inv		## Sphinx build clean and build html
+htmlall:				## Sphinx build clean and build html
 ifeq ($(is_venv),1)
 	@$(SPHINXBUILD) -b html "$(SOURCEDIR)" "$(BUILDDIR)/html"
 endif
 
 # @$(SPHINXBUILD) -b latexpdf "$(SOURCEDIR)" "$(BUILDDIR)/latex"
 .PHONY: pdf
 pdf:				## Sphinx build pdf
@@ -80,15 +80,15 @@
 	@$(SPHINXBUILDNOOPT) -M latexpdf "$(SOURCEDIR)" "$(BUILDDIR)"
 
 endif
 
 ##@ Test
 
 .PHONY: linkcheck
-linkcheck: build_inv	## Sphinx check urls within docs and code base
+linkcheck:				## Sphinx check urls within docs and code base
 ifeq ($(is_venv),1)
 	@$(SPHINXBUILD) -b linkcheck "$(SOURCEDIR)" "$(BUILDDIR)" || echo "$(err_check_web_conn). exit code $$?"
 endif
 
 .PHONY: _objects
 _objects:
 ifeq ($(is_venv),1)
@@ -133,15 +133,15 @@
 obj_strictyaml:
 
 # Stubbornly insists on repeating on outdated files.
 # -T show tracebacks on Exception
 # -q quiet
 # --keep-going even if there are warnings
 .PHONY: doctest
-doctest: build_inv		## Confirm in-doc code does what it claims
+doctest:				## Confirm in-doc code does what it claims
 ifeq ($(is_venv),1)
 	@$(MAKE) htmlall
 	$(SPHINXBUILDNOOPT) -b doctest "$(SOURCEDIR)" "$(BUILDDIR)"
 endif
 
 ##@ Misc
```

### Comparing `sphinx_external_toc_strict-1.1.5/docs/_static/asset-gesture-like-thumbs-up.svg` & `sphinx_external_toc_strict-1.1.6/docs/_static/asset-gesture-like-thumbs-up.svg`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/_static/asset-table-of-contents.svg` & `sphinx_external_toc_strict-1.1.6/docs/_static/asset-table-of-contents.svg`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/_static/credit.txt` & `sphinx_external_toc_strict-1.1.6/docs/_static/credit.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/_static/sphinx-external-toc-strict-logo.png` & `sphinx_external_toc_strict-1.1.6/docs/_static/sphinx-external-toc-strict-logo.png`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/_static/sphinx-external-toc-strict-logo.svg` & `sphinx_external_toc_strict-1.1.6/docs/_static/sphinx-external-toc-strict-logo.svg`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/_static/toc-graphic.png` & `sphinx_external_toc_strict-1.1.6/docs/_static/toc-graphic.png`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/_static/toc_tree.pptx` & `sphinx_external_toc_strict-1.1.6/docs/_static/toc_tree.pptx`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/_toc.yml` & `sphinx_external_toc_strict-1.1.6/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/code/cli.rst` & `sphinx_external_toc_strict-1.1.6/docs/code/cli.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/conf.py` & `sphinx_external_toc_strict-1.1.6/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 
 # Original author Chris Sewell <chrisj_sewell@hotmail.com>
 # copyright = "2021, Executable Book Project"
 
 # @@@ editable
 copyright = "2023–2024, Dave Faulkmore"
 # The short X.Y.Z version.
-version = "1.1.5"
+version = "1.1.6"
 # The full version, including alpha/beta/rc tags.
-release = "1.1.5"
+release = "1.1.6"
 # The date of release, in "monthname day, year" format.
 release_date = "April 19, 2024"
 # @@@ end
 
 v = parse(release)
 version_short = f"{v.major}.{v.minor}"
 # version_xyz = f"{v.major}.{v.minor}.{v.micro}"
@@ -133,15 +133,15 @@
         "https://github.com/crdoconnor/strictyaml",
         ("objects-strictyaml-source.inv", "objects-strictyaml-source.txt"),
     ),
     "docutils-source": (
         "https://docutils.sourceforge.io",
         ("objects-docutils-source.inv", "objects-docutils-source.txt"),
     ),
-    "sphinx-docs": (  # source logging-strict
+    "sphinx-docs": (  # source logging-strict. Alternative? https://www.sphinx-doc.org/objects.inv
         "https://www.sphinx-doc.org/en/master",
         ("objects-sphinx-docs.inv", "objects-sphinx-docs.txt"),
     ),
     "toc-strict": (
         "https://sphinx-external-toc-strict.readthedocs.io/en/latest",
         ("objects-toc-strict.inv", "objects-toc-strict.txt"),
     ),
```

### Comparing `sphinx_external_toc_strict-1.1.5/docs/intro.rst` & `sphinx_external_toc_strict-1.1.6/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/objects-sphinx-docs.txt` & `sphinx_external_toc_strict-1.1.6/docs/objects-sphinx-docs.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/objects-strictyaml-docs.txt` & `sphinx_external_toc_strict-1.1.6/docs/objects-strictyaml-docs.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/objects-strictyaml-source.txt` & `sphinx_external_toc_strict-1.1.6/docs/objects-strictyaml-source.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/requirements.pip` & `sphinx_external_toc_strict-1.1.6/docs/requirements.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/user_guide/api.rst` & `sphinx_external_toc_strict-1.1.6/docs/user_guide/api.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/user_guide/cli.rst` & `sphinx_external_toc_strict-1.1.6/docs/user_guide/cli.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/user_guide/regressions.md` & `sphinx_external_toc_strict-1.1.6/docs/user_guide/regressions.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
   The sphinx extension
   [sphinx-multitoc-numbering](https://github.com/executablebooks/sphinx-multitoc-numbering)
   which is supposed to fix this issue. However the package is unmaintained and **does not work**
 
   Package needs to be tested. There is a waiting PR that needs to be looked at too!
 
+## Dropped support
+
+- hidden document files
+
 ## Enhancements
 
 These are proposed enhancements
 
 - change theme to [sphinx-book-theme#304](https://github.com/executablebooks/sphinx-book-theme/pull/304)
 
 - CLI command to generate toc from existing documentation ``toctrees`` (and then remove toctree directives)
```

### Comparing `sphinx_external_toc_strict-1.1.5/docs/user_guide/sphinx.rst` & `sphinx_external_toc_strict-1.1.6/docs/user_guide/sphinx.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/docs/user_guide/why.rst` & `sphinx_external_toc_strict-1.1.6/docs/user_guide/why.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/howto.txt` & `sphinx_external_toc_strict-1.1.6/howto.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/igor.py` & `sphinx_external_toc_strict-1.1.6/igor.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/pyproject.toml` & `sphinx_external_toc_strict-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
     "https://github.com/psf/black/blob/ea66d40dd7f1eaa20256e6fccaf6d7b853ccc541/src/black/files.py#L57",
     "https://github.com/csachs/pyproject-flake8/blob/16b9dd4d2f19dcf0bfb3a3110f98227627cd67fe/pflake8/__init__.py#L22",
     "https://github.com/csachs/pyproject-flake8/blob/16b9dd4d2f19dcf0bfb3a3110f98227627cd67fe/pflake8/__init__.py#L86",
     "https://github.com/executablebooks/sphinx-external-toc/#development-notes",
 ]
 myst_enable_extensions = ["colon_fence", "html_image"]
 external_toc_exclude_missing = true
+todo_include_todos = true
 
 exclude_patterns = [
     "_build",
     "Thumbs.db",
     ".DS_Store",
 ]
 doctest_show_successes = false
```

### Comparing `sphinx_external_toc_strict-1.1.5/requirements/dev.pip` & `sphinx_external_toc_strict-1.1.6/requirements/dev.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/requirements/kit.in` & `sphinx_external_toc_strict-1.1.6/requirements/kit.in`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/requirements/kit.pip` & `sphinx_external_toc_strict-1.1.6/requirements/kit.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/requirements/manage.pip` & `sphinx_external_toc_strict-1.1.6/requirements/manage.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/requirements/pip-tools.pip` & `sphinx_external_toc_strict-1.1.6/requirements/pip-tools.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/requirements/prod.pip` & `sphinx_external_toc_strict-1.1.6/requirements/prod.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/requirements/tox.in` & `sphinx_external_toc_strict-1.1.6/requirements/tox.in`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/requirements/tox.pip` & `sphinx_external_toc_strict-1.1.6/requirements/tox.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/setup.py` & `sphinx_external_toc_strict-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/__init__.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/_compat.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/_compat.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/api.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/api.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/api.pyi` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/api.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/cli.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/constants.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/constants.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/constants.pyi` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/constants.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/events.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/events.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/events.pyi` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/events.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/filename_suffix.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/filename_suffix.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/filename_suffix.pyi` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/filename_suffix.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_shared.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/parsing_shared.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_shared.pyi` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/parsing_shared.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_strictyaml.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/parsing_strictyaml.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_strictyaml.pyi` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/parsing_strictyaml.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/pep518_read.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/pep518_read.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/pep518_read.pyi` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/pep518_read.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/tools_strictyaml.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/tools_strictyaml.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/tools_strictyaml.pyi` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/tools_strictyaml.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/version_semantic.py` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict/version_semantic.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/PKG-INFO` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-external-toc-strict
-Version: 1.1.5
+Version: 1.1.6
 Summary: A sphinx extension that allows the site-map to be defined in a single YAML file.
 Author-email: Dave Faulkmore <faulkmore@protonmail.com>
 License: MIT License
         
         Copyright (c) 2021 Executable Books
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/SOURCES.txt` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,26 @@
 .github/workflows/release.yml
 .github/workflows/test-coverage.yml
 .github/workflows/testsuite.yml
 docs/Makefile
 docs/_toc.yml
 docs/conf.py
 docs/intro.rst
+docs/objects-black.inv
 docs/objects-black.txt
+docs/objects-docutils-source.inv
 docs/objects-docutils-source.txt
-docs/objects-python.txt
+docs/objects-python.inv
+docs/objects-sphinx-docs.inv
 docs/objects-sphinx-docs.txt
+docs/objects-strictyaml-docs.inv
 docs/objects-strictyaml-docs.txt
+docs/objects-strictyaml-source.inv
 docs/objects-strictyaml-source.txt
+docs/objects-toc-strict.inv
 docs/objects-toc-strict.txt
 docs/requirements.in
 docs/requirements.pip
 docs/_static/asset-gesture-like-thumbs-up.svg
 docs/_static/asset-table-of-contents.svg
 docs/_static/credit.txt
 docs/_static/sphinx-external-toc-strict-logo.png
@@ -50,14 +56,15 @@
 docs/code/events.rst
 docs/code/exceptions.rst
 docs/code/filename_suffix.rst
 docs/code/index.rst
 docs/code/parsing_shared.rst
 docs/code/parsing_strictyaml.rst
 docs/code/pep518_read.rst
+docs/code/todo.rst
 docs/code/tools_strictyaml.rst
 docs/code/version_semantic.rst
 docs/example/index.rst
 docs/example/globfolder/page1.rst
 docs/example/globfolder/page2.rst
 docs/example/subfolder/page.rst
 docs/user_guide/api.rst
```

### Comparing `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/requires.txt` & `sphinx_external_toc_strict-1.1.6/src/sphinx_external_toc_strict.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/chapters.yml` & `sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/chapters.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/jb_docs_toc.yml` & `sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/jb_docs_toc.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/parts.yml` & `sphinx_external_toc_strict-1.1.6/tests/_jb_migrate_toc_files/parts.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/_toc_files/glob_md.yml` & `sphinx_external_toc_strict-1.1.6/tests/_toc_files/glob_md.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/conftest.py` & `sphinx_external_toc_strict-1.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_api.py` & `sphinx_external_toc_strict-1.1.6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_cli/test_create_toc.txt` & `sphinx_external_toc_strict-1.1.6/tests/test_cli/test_create_toc.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_cli.py` & `sphinx_external_toc_strict-1.1.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_filename_suffix.py` & `sphinx_external_toc_strict-1.1.6/tests/test_filename_suffix.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_glob_md_.yml` & `sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_create_toc_dict_glob_md_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_basic_.yml` & `sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_basic_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml` & `sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_glob_md_.yml` & `sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_glob_md_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_nested_.yml` & `sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_nested_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml` & `sphinx_external_toc_strict-1.1.6/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_parsing.py` & `sphinx_external_toc_strict-1.1.6/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_pep518_read.py` & `sphinx_external_toc_strict-1.1.6/tests/test_pep518_read.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_tableofcontents_.xml` & `sphinx_external_toc_strict-1.1.6/tests/test_sphinx/test_success_tableofcontents_.xml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_sphinx.py` & `sphinx_external_toc_strict-1.1.6/tests/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_tools/test_create_site_map_from_path.yml` & `sphinx_external_toc_strict-1.1.6/tests/test_tools/test_create_site_map_from_path.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_chapters_.yml` & `sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_chapters_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml` & `sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_parts_.yml` & `sphinx_external_toc_strict-1.1.6/tests/test_tools/test_migrate_jb_parts_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_tools.py` & `sphinx_external_toc_strict-1.1.6/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tests/test_version_semantic.py` & `sphinx_external_toc_strict-1.1.6/tests/test_version_semantic.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.5/tox.ini` & `sphinx_external_toc_strict-1.1.6/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -41,21 +41,18 @@
 # -q to get all warnings, and once with -QW to get a success/fail status
 # return.
 deps =
     -r docs/requirements.pip
 allowlist_externals =
     make
 commands =
-    make --directory=docs build_inv
     sphinx-build -b html -aEnqW docs docs/_build/html
     rst2html.py --strict README.rst docs/_build/trash
     - sphinx-build -b html -b linkcheck -aEnq docs docs/_build/html
     - sphinx-build -b html -b linkcheck -aEnQW docs docs/_build/html
-commands_post =
-    make  --directory=docs clean_inv
 
 [testenv:lint]
 description = pre-commit and build
 # Minimum of PYVERSIONS
 basepython = python3.9
 deps =
     -r requirements/dev.pip
```

