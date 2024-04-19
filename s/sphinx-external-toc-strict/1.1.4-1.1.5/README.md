# Comparing `tmp/sphinx_external_toc_strict-1.1.4.tar.gz` & `tmp/sphinx_external_toc_strict-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_external_toc_strict-1.1.4.tar", last modified: Fri Apr 19 03:58:20 2024, max compression
+gzip compressed data, was "sphinx_external_toc_strict-1.1.5.tar", last modified: Fri Apr 19 04:38:51 2024, max compression
```

## Comparing `sphinx_external_toc_strict-1.1.4.tar` & `sphinx_external_toc_strict-1.1.5.tar`

### file list

```diff
@@ -1,239 +1,239 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.980598 sphinx_external_toc_strict-1.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.928598 sphinx_external_toc_strict-1.1.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.932597 sphinx_external_toc_strict-1.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/kit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/python-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/quality.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/test-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/testsuite.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    31604 2024-04-19 03:58:20.980598 sphinx_external_toc_strict-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/asset-gesture-like-thumbs-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/asset-table-of-contents.svg
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/credit.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/sphinx-external-toc-strict-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/sphinx-external-toc-strict-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   147326 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/toc-graphic.png
--rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/toc_tree.pptx
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/code/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/compat.rst
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/constrants.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/filename_suffix.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/parsing_shared.rst
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/parsing_strictyaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/pep518_read.rst
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/tools_strictyaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/version_semantic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/example/globfolder/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/example/globfolder/page1.rst
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/example/globfolder/page2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/example/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/example/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/example/subfolder/page.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-black.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-docutils-source.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1111839 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-python.txt
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-sphinx-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-strictyaml-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-strictyaml-source.txt
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-toc-strict.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/requirements.pip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.940598 sphinx_external_toc_strict-1.1.4/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/user_guide/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/user_guide/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/user_guide/regressions.md
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/user_guide/sphinx.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/user_guide/why.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/howto.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17383 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/igor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.940598 sphinx_external_toc_strict-1.1.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/dev.pip
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/kit.in
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/kit.pip
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/manage.in
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/manage.pip
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/mypy.pip
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/pins.pip
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/pip-tools.pip
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/pip.pip
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/prod.in
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/prod.pip
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/tox.pip
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:58:20.980598 sphinx_external_toc_strict-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.928598 sphinx_external_toc_strict-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.944598 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/filename_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/filename_suffix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_shared.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_strictyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/pep518_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/pep518_read.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19183 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/tools_strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/tools_strictyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/version_semantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/version_semantic.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.960598 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31604 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.948598 sphinx_external_toc_strict-1.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.948598 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/bad_option_value.yml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/bad_url.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/doc_multiple_times.yml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/doc_validation_fail.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/empty_items.yml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/empty_subtrees.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/entry_not_a_mapping.yml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/entry_unknown_link_type.yml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/file_and_glob_present.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/item_then_subtrees_key.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/items_in_glob.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/items_in_url.yml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/list.yml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/no_root.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/subtree_with_no_items.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/unknown_keys.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/unknown_keys_nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/unknown_usecase.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.952597 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/chapters.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/jb_docs_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/list_and_nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/numbered_chapters.yml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/numbered_depth.yml
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/numbered_depth_parts_subset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/numbered_parts.yml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/numbered_parts_subset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/parts.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/simple_dict.yml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/simple_list.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.952597 sphinx_external_toc_strict-1.1.4/tests/_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/basic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/basic_compressed.yml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/caption_not_entries.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/exclude_missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/glob.yml
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/glob_md.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/tableofcontents.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.952597 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/contains_toctree.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/file_not_in_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/multiple_tableofcontents.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/no_glob_match.yml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/tableofcontents_no_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.952597 sphinx_external_toc_strict-1.1.4/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_cli/test_create_toc.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_filename_suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.956598 sphinx_external_toc_strict-1.1.4/tests/test_parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_pep518_read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.956598 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_basic_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_basic_compressed_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_caption_not_entries_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_glob_md_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_tableofcontents_.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.960598 sphinx_external_toc_strict-1.1.4/tests/test_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_create_site_map_from_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_basic_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_chapters_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_list_and_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_numbered_chapters_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_numbered_depth_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_numbered_depth_parts_subset_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_numbered_parts_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_numbered_parts_subset_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_parts_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_simple_dict_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_simple_list_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_version_semantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.987968 sphinx_external_toc_strict-1.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.935968 sphinx_external_toc_strict-1.1.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.939967 sphinx_external_toc_strict-1.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/kit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/python-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/quality.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/test-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.github/workflows/testsuite.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31595 2024-04-19 04:38:51.987968 sphinx_external_toc_strict-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.939967 sphinx_external_toc_strict-1.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/asset-gesture-like-thumbs-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/asset-table-of-contents.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/credit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/sphinx-external-toc-strict-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/sphinx-external-toc-strict-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   147326 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/toc-graphic.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_static/toc_tree.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/compat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/constrants.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/filename_suffix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/parsing_shared.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/parsing_strictyaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/pep518_read.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/tools_strictyaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/code/version_semantic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/example/globfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/example/globfolder/page1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/example/globfolder/page2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/example/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/example/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/example/subfolder/page.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-black.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-docutils-source.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1111839 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-sphinx-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-strictyaml-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-strictyaml-source.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/objects-toc-strict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/requirements.pip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.943967 sphinx_external_toc_strict-1.1.5/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/user_guide/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/user_guide/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/user_guide/regressions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/user_guide/sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/docs/user_guide/why.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/howto.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17383 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/igor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.947967 sphinx_external_toc_strict-1.1.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/dev.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/kit.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/kit.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/manage.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/manage.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/mypy.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/pins.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/pip-tools.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/pip.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/prod.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/prod.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/requirements/tox.pip
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 04:38:51.987968 sphinx_external_toc_strict-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.935968 sphinx_external_toc_strict-1.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.951968 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/filename_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/filename_suffix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_shared.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_strictyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/pep518_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/pep518_read.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19183 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/tools_strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/tools_strictyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/version_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/version_semantic.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.967967 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31595 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 04:38:51.000000 sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.955968 sphinx_external_toc_strict-1.1.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.955968 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/bad_option_value.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/bad_url.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/doc_multiple_times.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/doc_validation_fail.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/empty_items.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/empty_subtrees.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/entry_not_a_mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/entry_unknown_link_type.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/file_and_glob_present.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/item_then_subtrees_key.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/items_in_glob.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/items_in_url.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/list.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/no_root.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/subtree_with_no_items.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/unknown_keys.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/unknown_keys_nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_bad_toc_files/unknown_usecase.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.959967 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/chapters.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/jb_docs_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/list_and_nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/numbered_chapters.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/numbered_depth.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/numbered_depth_parts_subset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/numbered_parts.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/numbered_parts_subset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/parts.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/simple_dict.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/simple_list.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.959967 sphinx_external_toc_strict-1.1.5/tests/_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/basic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/basic_compressed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/caption_not_entries.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/exclude_missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/glob.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/glob_md.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_toc_files/tableofcontents.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.959967 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/contains_toctree.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/file_not_in_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/multiple_tableofcontents.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/no_glob_match.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/_warning_toc_files/tableofcontents_no_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.959967 sphinx_external_toc_strict-1.1.5/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_cli/test_create_toc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_filename_suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.963967 sphinx_external_toc_strict-1.1.5/tests/test_parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_pep518_read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.963967 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_basic_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_basic_compressed_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_caption_not_entries_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_glob_md_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_tableofcontents_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 04:38:51.967967 sphinx_external_toc_strict-1.1.5/tests/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_create_site_map_from_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_basic_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_file_to_sitemap_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_chapters_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_list_and_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_numbered_chapters_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_numbered_depth_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_numbered_depth_parts_subset_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_numbered_parts_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_numbered_parts_subset_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_parts_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_simple_dict_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_simple_list_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tests/test_version_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-19 04:38:43.000000 sphinx_external_toc_strict-1.1.5/tox.ini
```

### Comparing `sphinx_external_toc_strict-1.1.4/.github/workflows/codeql-analysis.yml` & `sphinx_external_toc_strict-1.1.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/.github/workflows/dependency-review.yml` & `sphinx_external_toc_strict-1.1.5/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/.github/workflows/kit.yml` & `sphinx_external_toc_strict-1.1.5/.github/workflows/kit.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/.github/workflows/python-nightly.yml` & `sphinx_external_toc_strict-1.1.5/.github/workflows/python-nightly.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/.github/workflows/quality.yml` & `sphinx_external_toc_strict-1.1.5/.github/workflows/quality.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/.github/workflows/release.yml` & `sphinx_external_toc_strict-1.1.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/.github/workflows/test-coverage.yml` & `sphinx_external_toc_strict-1.1.5/.github/workflows/test-coverage.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/.github/workflows/testsuite.yml` & `sphinx_external_toc_strict-1.1.5/.github/workflows/testsuite.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/.gitignore` & `sphinx_external_toc_strict-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/.pre-commit-config.yaml` & `sphinx_external_toc_strict-1.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/.readthedocs.yml` & `sphinx_external_toc_strict-1.1.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/CHANGELOG.md` & `sphinx_external_toc_strict-1.1.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/CHANGES.rst` & `sphinx_external_toc_strict-1.1.5/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,22 @@
    1. Dropped support for hidden document files
 
    Commit items for NEXT VERSION
    ..............................
 
 .. scriv-start-here
 
+.. _changes_1-1-5:
+
+Version 1.1.5 — 2024-04-19
+--------------------------
+
+- docs(Makefile): for targets build_inv and clean_inv only use relative paths
+- docs(Makefile): for targets doctest and linkcheck require target build_inv
+
 .. _changes_1-1-4:
 
 Version 1.1.4 — 2024-04-19
 --------------------------
 
 - ci(.readthedocs.yml): py311 --> py39, do not build pdf, and notes
 - docs: defend assertions, links, in comparison table
```

### Comparing `sphinx_external_toc_strict-1.1.4/CONTRIBUTING.md` & `sphinx_external_toc_strict-1.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/LICENSE` & `sphinx_external_toc_strict-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/Makefile` & `sphinx_external_toc_strict-1.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/NOTICE.txt` & `sphinx_external_toc_strict-1.1.5/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/PKG-INFO` & `sphinx_external_toc_strict-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-external-toc-strict
-Version: 1.1.4
+Version: 1.1.5
 Summary: A sphinx extension that allows the site-map to be defined in a single YAML file.
 Author-email: Dave Faulkmore <faulkmore@protonmail.com>
 License: MIT License
         
         Copyright (c) 2021 Executable Books
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -292,15 +292,15 @@
    :header: "Matric", "TOC", "TOC-Strict"
    :widths: auto
 
    "yaml package", `pyyaml / yaml <https://hitchdev.com/strictyaml/why-not/>`_, `strictyaml / ruemel.yaml <https://hitchdev.com/strictyaml/why/>`_
    ".hidden.files.rst", "Yes", "No"
    "docs theme", `sphinx-book-theme <https://sphinx-book-theme.readthedocs.io/en/latest>`_, `alabaster <https://alabaster.readthedocs.io/en/latest/>`_
    "markdown support", "Yes", "Yes"
-   "both", `No <https://github.com/executablebooks/sphinx-external-toc/tree/main#development-notes>`_, "Yes, root doc must be ``index.rst``"
+   "both", `No <https://github.com/executablebooks/sphinx-external-toc/#development-notes>`_, "Yes, root doc must be ``index.rst``"
    "dump yaml", "use yaml.dump", "[package].parsing_strictyaml.dump_yaml"
    "static type checking", "patchy", "Yes (99%)"
    "coverage", "patchy", "maximium"
    "in-code manual", "No", "Yes"
 
 The core API should be compatible. To avoid confusion, on the command line, rather than ``sphinx-etoc``, use ``sphinx-etoc-strict``
```

### Comparing `sphinx_external_toc_strict-1.1.4/README.rst` & `sphinx_external_toc_strict-1.1.5/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
    :header: "Matric", "TOC", "TOC-Strict"
    :widths: auto
 
    "yaml package", `pyyaml / yaml <https://hitchdev.com/strictyaml/why-not/>`_, `strictyaml / ruemel.yaml <https://hitchdev.com/strictyaml/why/>`_
    ".hidden.files.rst", "Yes", "No"
    "docs theme", `sphinx-book-theme <https://sphinx-book-theme.readthedocs.io/en/latest>`_, `alabaster <https://alabaster.readthedocs.io/en/latest/>`_
    "markdown support", "Yes", "Yes"
-   "both", `No <https://github.com/executablebooks/sphinx-external-toc/tree/main#development-notes>`_, "Yes, root doc must be ``index.rst``"
+   "both", `No <https://github.com/executablebooks/sphinx-external-toc/#development-notes>`_, "Yes, root doc must be ``index.rst``"
    "dump yaml", "use yaml.dump", "[package].parsing_strictyaml.dump_yaml"
    "static type checking", "patchy", "Yes (99%)"
    "coverage", "patchy", "maximium"
    "in-code manual", "No", "Yes"
 
 The core API should be compatible. To avoid confusion, on the command line, rather than ``sphinx-etoc``, use ``sphinx-etoc-strict``
```

### Comparing `sphinx_external_toc_strict-1.1.4/docs/Makefile` & `sphinx_external_toc_strict-1.1.5/docs/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -29,39 +29,39 @@
 
 # Convert *.txt --> *.inv Base folder only
 # sphobjinv convert -q zlib objects-toc-strict.txt objects-toc-strict.inv
 .PHONY: build_inv
 build_inv:				## inventory base folder only .txt --> .inv
 ifeq ($(is_venv),1)
 	@while read f_path; do
-	  if [[ -f "$(SOURCEDIR)/$${f_path}.txt" ]]; then
-	    [[ ! -f "$(SOURCEDIR)/$${f_path}.inv" ]] && sphobjinv convert -q zlib "$(SOURCEDIR)/$${f_path}.txt" "$(SOURCEDIR)/$${f_path}.inv" ||:
+	  if [[ -f "$${f_path}.txt" ]]; then
+	    [[ ! -f "$${f_path}.inv" ]] && sphobjinv convert -q zlib "$${f_path}.txt" "$${f_path}.inv" ||:
 	  fi
 	done < <(/bin/find $(SOURCEDIR) -maxdepth 1 -type f -name "*.txt" -exec basename {} .txt \;)
 endif
 
 .PHONY: inv2txt
 inv2txt:				## .inv without .txt convert to .txt
 inv2txt: | _inv2txt clean_inv
 
 #  Revert *.inv --> .txt Base folder only. .inv without cooresponding .txt
 .PHONY: _inv2txt
 _inv2txt:
 	@while read f_path; do
-	  if [[ -f "$(SOURCEDIR)/$${f_path}.inv" ]] && [[ ! -f "$(SOURCEDIR)/$${f_path}.txt" ]]; then
-	    sphobjinv convert -q plain "$(SOURCEDIR)/$${f_path}.inv" "$(SOURCEDIR)/$${f_path}.txt" ||:
+	  if [[ -f "$${f_path}.inv" ]] && [[ ! -f "$${f_path}.txt" ]]; then
+	    sphobjinv convert -q plain "$${f_path}.inv" "$${f_path}.txt" ||:
 	  fi
 	done < <(/bin/find $(SOURCEDIR) -maxdepth 1 -type f -name "*.inv" -exec basename {} .inv \;)
 
 # clean .inv that have cooresponding .txt
 .PHONY: clean_inv
 clean_inv:				## remove .inv files that have cooresponding .txt file
 	@while read f_path; do
 	  if [[ -f "$${f_path}.txt" ]]; then
-	    [[ -f "$(SOURCEDIR)/$${f_path}.inv" ]] && /bin/rm --preserve-root=all "$(SOURCEDIR)/$${f_path}.inv" ||:
+	    [[ -f "$${f_path}.inv" ]] && /bin/rm --preserve-root=all "$${f_path}.inv" ||:
 	  fi
 	done < <(/bin/find $(SOURCEDIR) -maxdepth 1 -type f -name "*.txt" -exec basename {} .txt \;)
 
 .PHONY: html
 html:				## Sphinx build html. Only whats been changed
 ifeq ($(is_venv),1)
 	@$(SPHINXBUILDNOOPT) -b html "$(SOURCEDIR)" "$(BUILDDIR)/html"
@@ -80,15 +80,15 @@
 	@$(SPHINXBUILDNOOPT) -M latexpdf "$(SOURCEDIR)" "$(BUILDDIR)"
 
 endif
 
 ##@ Test
 
 .PHONY: linkcheck
-linkcheck:				## Sphinx check urls within docs and code base
+linkcheck: build_inv	## Sphinx check urls within docs and code base
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
-doctest:				## Confirm in-doc code does what it claims
+doctest: build_inv		## Confirm in-doc code does what it claims
 ifeq ($(is_venv),1)
 	@$(MAKE) htmlall
 	$(SPHINXBUILDNOOPT) -b doctest "$(SOURCEDIR)" "$(BUILDDIR)"
 endif
 
 ##@ Misc
```

### Comparing `sphinx_external_toc_strict-1.1.4/docs/_static/asset-gesture-like-thumbs-up.svg` & `sphinx_external_toc_strict-1.1.5/docs/_static/asset-gesture-like-thumbs-up.svg`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/_static/asset-table-of-contents.svg` & `sphinx_external_toc_strict-1.1.5/docs/_static/asset-table-of-contents.svg`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/_static/credit.txt` & `sphinx_external_toc_strict-1.1.5/docs/_static/credit.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/_static/sphinx-external-toc-strict-logo.png` & `sphinx_external_toc_strict-1.1.5/docs/_static/sphinx-external-toc-strict-logo.png`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/_static/sphinx-external-toc-strict-logo.svg` & `sphinx_external_toc_strict-1.1.5/docs/_static/sphinx-external-toc-strict-logo.svg`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/_static/toc-graphic.png` & `sphinx_external_toc_strict-1.1.5/docs/_static/toc-graphic.png`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/_static/toc_tree.pptx` & `sphinx_external_toc_strict-1.1.5/docs/_static/toc_tree.pptx`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/_toc.yml` & `sphinx_external_toc_strict-1.1.5/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/code/cli.rst` & `sphinx_external_toc_strict-1.1.5/docs/code/cli.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/conf.py` & `sphinx_external_toc_strict-1.1.5/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 
 # Original author Chris Sewell <chrisj_sewell@hotmail.com>
 # copyright = "2021, Executable Book Project"
 
 # @@@ editable
 copyright = "2023–2024, Dave Faulkmore"
 # The short X.Y.Z version.
-version = "1.1.4"
+version = "1.1.5"
 # The full version, including alpha/beta/rc tags.
-release = "1.1.4"
+release = "1.1.5"
 # The date of release, in "monthname day, year" format.
 release_date = "April 19, 2024"
 # @@@ end
 
 v = parse(release)
 version_short = f"{v.major}.{v.minor}"
 # version_xyz = f"{v.major}.{v.minor}.{v.micro}"
```

### Comparing `sphinx_external_toc_strict-1.1.4/docs/intro.rst` & `sphinx_external_toc_strict-1.1.5/docs/intro.rst`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
    :header: "Matric", "TOC", "TOC-Strict"
    :widths: auto
 
    "yaml package", `pyyaml / yaml <https://hitchdev.com/strictyaml/why-not/>`_, `strictyaml / ruemel.yaml <https://hitchdev.com/strictyaml/why/>`_
    ".hidden.files.rst", "Yes", "No"
    "docs theme", `sphinx-book-theme <https://sphinx-book-theme.readthedocs.io/en/latest>`_, `alabaster <https://alabaster.readthedocs.io/en/latest/>`_
    "markdown support", "Yes", "Yes"
-   "both", `No <https://github.com/executablebooks/sphinx-external-toc/tree/main#development-notes>`_, "Yes, root doc must be ``index.rst``"
+   "both", `No <https://github.com/executablebooks/sphinx-external-toc/#development-notes>`_, "Yes, root doc must be ``index.rst``"
    "dump yaml", "use yaml.dump", :py:func:`parsing_strictyaml.dump_yaml <sphinx_external_toc_strict.parsing_strictyaml.dump_yaml>`
    "static type checking", "patchy", "Yes (99%)"
    "coverage", "patchy", "maximium"
    "in-code manual", "No", "Yes"
 
 The core APIs should be compatible. To avoid confusion, on the command
 line, rather than ``sphinx-etoc``, use ``sphinx-etoc-strict``
```

### Comparing `sphinx_external_toc_strict-1.1.4/docs/objects-python.txt` & `sphinx_external_toc_strict-1.1.5/docs/objects-python.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/objects-sphinx-docs.txt` & `sphinx_external_toc_strict-1.1.5/docs/objects-sphinx-docs.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/objects-strictyaml-docs.txt` & `sphinx_external_toc_strict-1.1.5/docs/objects-strictyaml-docs.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/objects-strictyaml-source.txt` & `sphinx_external_toc_strict-1.1.5/docs/objects-strictyaml-source.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/requirements.pip` & `sphinx_external_toc_strict-1.1.5/docs/requirements.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/user_guide/api.rst` & `sphinx_external_toc_strict-1.1.5/docs/user_guide/api.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/user_guide/cli.rst` & `sphinx_external_toc_strict-1.1.5/docs/user_guide/cli.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/user_guide/regressions.md` & `sphinx_external_toc_strict-1.1.5/docs/user_guide/regressions.md`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/user_guide/sphinx.rst` & `sphinx_external_toc_strict-1.1.5/docs/user_guide/sphinx.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/docs/user_guide/why.rst` & `sphinx_external_toc_strict-1.1.5/docs/user_guide/why.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/howto.txt` & `sphinx_external_toc_strict-1.1.5/howto.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     - Check that the docs build correctly:
         $ tox -e docs
         or
         $ cd docs && make doctest && cd - &>/dev/null
         $ cd docs && make linkcheck && cd - &>/dev/null
         $ cd docs && make html && cd - &>/dev/null
         $ cd docs && make pdf && cd - &>/dev/null
+    - tox will affect _version.py, revert version str back to tagged version
 - commit the release-prep changes
     $ make relcommit1
     or
     $ git status
     $ git add [whatever]
     $ git commit -S -m ""
 - Done with changes to source files
```

### Comparing `sphinx_external_toc_strict-1.1.4/igor.py` & `sphinx_external_toc_strict-1.1.5/igor.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/pyproject.toml` & `sphinx_external_toc_strict-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 linkcheck_ignore = [
     "https://github.com/crdoconnor/strictyaml/blob/dfd93f9740ebd5e7150029bc3d89ea102bcddf00/strictyaml/representation.py#L48",
     "https://github.com/crdoconnor/strictyaml/blob/dfd93f9740ebd5e7150029bc3d89ea102bcddf00/strictyaml/representation.py#L114",
     "https://github.com/PyCQA/flake8/blob/fb9a02aaf77b56fcad4320971e7edca0cea93489/src/flake8/options/config.py#L56",
     "https://github.com/psf/black/blob/ea66d40dd7f1eaa20256e6fccaf6d7b853ccc541/src/black/files.py#L57",
     "https://github.com/csachs/pyproject-flake8/blob/16b9dd4d2f19dcf0bfb3a3110f98227627cd67fe/pflake8/__init__.py#L22",
     "https://github.com/csachs/pyproject-flake8/blob/16b9dd4d2f19dcf0bfb3a3110f98227627cd67fe/pflake8/__init__.py#L86",
-
+    "https://github.com/executablebooks/sphinx-external-toc/#development-notes",
 ]
 myst_enable_extensions = ["colon_fence", "html_image"]
 external_toc_exclude_missing = true
 
 exclude_patterns = [
     "_build",
     "Thumbs.db",
```

### Comparing `sphinx_external_toc_strict-1.1.4/requirements/dev.pip` & `sphinx_external_toc_strict-1.1.5/requirements/dev.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/requirements/kit.in` & `sphinx_external_toc_strict-1.1.5/requirements/kit.in`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/requirements/kit.pip` & `sphinx_external_toc_strict-1.1.5/requirements/kit.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/requirements/manage.pip` & `sphinx_external_toc_strict-1.1.5/requirements/manage.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/requirements/pip-tools.pip` & `sphinx_external_toc_strict-1.1.5/requirements/pip-tools.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/requirements/prod.pip` & `sphinx_external_toc_strict-1.1.5/requirements/prod.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/requirements/tox.in` & `sphinx_external_toc_strict-1.1.5/requirements/tox.in`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/requirements/tox.pip` & `sphinx_external_toc_strict-1.1.5/requirements/tox.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/setup.py` & `sphinx_external_toc_strict-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/__init__.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/_compat.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/_compat.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/api.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/api.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/api.pyi` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/api.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/cli.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/constants.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/constants.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/constants.pyi` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/constants.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/events.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/events.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/events.pyi` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/events.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/filename_suffix.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/filename_suffix.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/filename_suffix.pyi` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/filename_suffix.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_shared.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_shared.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_shared.pyi` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_shared.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_strictyaml.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_strictyaml.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_strictyaml.pyi` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/parsing_strictyaml.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/pep518_read.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/pep518_read.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/pep518_read.pyi` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/pep518_read.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/tools_strictyaml.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/tools_strictyaml.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/tools_strictyaml.pyi` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/tools_strictyaml.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/version_semantic.py` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict/version_semantic.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/PKG-INFO` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-external-toc-strict
-Version: 1.1.4
+Version: 1.1.5
 Summary: A sphinx extension that allows the site-map to be defined in a single YAML file.
 Author-email: Dave Faulkmore <faulkmore@protonmail.com>
 License: MIT License
         
         Copyright (c) 2021 Executable Books
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -292,15 +292,15 @@
    :header: "Matric", "TOC", "TOC-Strict"
    :widths: auto
 
    "yaml package", `pyyaml / yaml <https://hitchdev.com/strictyaml/why-not/>`_, `strictyaml / ruemel.yaml <https://hitchdev.com/strictyaml/why/>`_
    ".hidden.files.rst", "Yes", "No"
    "docs theme", `sphinx-book-theme <https://sphinx-book-theme.readthedocs.io/en/latest>`_, `alabaster <https://alabaster.readthedocs.io/en/latest/>`_
    "markdown support", "Yes", "Yes"
-   "both", `No <https://github.com/executablebooks/sphinx-external-toc/tree/main#development-notes>`_, "Yes, root doc must be ``index.rst``"
+   "both", `No <https://github.com/executablebooks/sphinx-external-toc/#development-notes>`_, "Yes, root doc must be ``index.rst``"
    "dump yaml", "use yaml.dump", "[package].parsing_strictyaml.dump_yaml"
    "static type checking", "patchy", "Yes (99%)"
    "coverage", "patchy", "maximium"
    "in-code manual", "No", "Yes"
 
 The core API should be compatible. To avoid confusion, on the command line, rather than ``sphinx-etoc``, use ``sphinx-etoc-strict``
```

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/SOURCES.txt` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/requires.txt` & `sphinx_external_toc_strict-1.1.5/src/sphinx_external_toc_strict.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/chapters.yml` & `sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/chapters.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/jb_docs_toc.yml` & `sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/jb_docs_toc.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/parts.yml` & `sphinx_external_toc_strict-1.1.5/tests/_jb_migrate_toc_files/parts.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/_toc_files/glob_md.yml` & `sphinx_external_toc_strict-1.1.5/tests/_toc_files/glob_md.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/conftest.py` & `sphinx_external_toc_strict-1.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_api.py` & `sphinx_external_toc_strict-1.1.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_cli/test_create_toc.txt` & `sphinx_external_toc_strict-1.1.5/tests/test_cli/test_create_toc.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_cli.py` & `sphinx_external_toc_strict-1.1.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_filename_suffix.py` & `sphinx_external_toc_strict-1.1.5/tests/test_filename_suffix.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_glob_md_.yml` & `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_create_toc_dict_glob_md_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_basic_.yml` & `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_basic_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml` & `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_glob_md_.yml` & `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_glob_md_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_nested_.yml` & `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_nested_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml` & `sphinx_external_toc_strict-1.1.5/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_parsing.py` & `sphinx_external_toc_strict-1.1.5/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_pep518_read.py` & `sphinx_external_toc_strict-1.1.5/tests/test_pep518_read.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_tableofcontents_.xml` & `sphinx_external_toc_strict-1.1.5/tests/test_sphinx/test_success_tableofcontents_.xml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_sphinx.py` & `sphinx_external_toc_strict-1.1.5/tests/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_tools/test_create_site_map_from_path.yml` & `sphinx_external_toc_strict-1.1.5/tests/test_tools/test_create_site_map_from_path.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_chapters_.yml` & `sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_chapters_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml` & `sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_parts_.yml` & `sphinx_external_toc_strict-1.1.5/tests/test_tools/test_migrate_jb_parts_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_tools.py` & `sphinx_external_toc_strict-1.1.5/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tests/test_version_semantic.py` & `sphinx_external_toc_strict-1.1.5/tests/test_version_semantic.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.4/tox.ini` & `sphinx_external_toc_strict-1.1.5/tox.ini`

 * *Files identical despite different names*

