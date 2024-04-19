# Comparing `tmp/sphinx_external_toc_strict-1.1.3.tar.gz` & `tmp/sphinx_external_toc_strict-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_external_toc_strict-1.1.3.tar", last modified: Thu Apr 18 12:31:38 2024, max compression
+gzip compressed data, was "sphinx_external_toc_strict-1.1.4.tar", last modified: Fri Apr 19 03:58:20 2024, max compression
```

## Comparing `sphinx_external_toc_strict-1.1.3.tar` & `sphinx_external_toc_strict-1.1.4.tar`

### file list

```diff
@@ -1,233 +1,239 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.852928 sphinx_external_toc_strict-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.804927 sphinx_external_toc_strict-1.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.804927 sphinx_external_toc_strict-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/kit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/python-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/quality.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/test-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/testsuite.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    31271 2024-04-18 12:31:38.852928 sphinx_external_toc_strict-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19092 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.808927 sphinx_external_toc_strict-1.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.808927 sphinx_external_toc_strict-1.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   147326 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/_static/toc-graphic.png
--rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/_static/toc_tree.pptx
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/docs/code/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/compat.rst
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/constrants.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/filename_suffix.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/parsing_shared.rst
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/parsing_strictyaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/pep518_read.rst
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/tools_strictyaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/version_semantic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/docs/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/docs/example/globfolder/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/example/globfolder/page1.rst
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/example/globfolder/page2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/example/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/docs/example/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/example/subfolder/page.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-black.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-docutils-source.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1111839 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-python.txt
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-sphinx-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-strictyaml-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-strictyaml-source.txt
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-toc-strict.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/requirements.pip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/user_guide/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/user_guide/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/user_guide/sphinx.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/user_guide/why.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/howto.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17383 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/igor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/dev.pip
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/kit.in
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/kit.pip
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/manage.in
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/manage.pip
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/mypy.pip
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/pins.pip
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/pip-tools.pip
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/pip.pip
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/prod.in
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/prod.pip
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/tox.pip
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:31:38.852928 sphinx_external_toc_strict-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.800927 sphinx_external_toc_strict-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.816928 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/filename_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/filename_suffix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_shared.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_strictyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/pep518_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/pep518_read.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19183 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/tools_strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/tools_strictyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/version_semantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/version_semantic.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.832928 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31271 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.820927 sphinx_external_toc_strict-1.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.824928 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/bad_option_value.yml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/bad_url.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/doc_multiple_times.yml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/doc_validation_fail.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/empty_items.yml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/empty_subtrees.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/entry_not_a_mapping.yml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/entry_unknown_link_type.yml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/file_and_glob_present.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/item_then_subtrees_key.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/items_in_glob.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/items_in_url.yml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/list.yml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/no_root.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/subtree_with_no_items.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/unknown_keys.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/unknown_keys_nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/unknown_usecase.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.824928 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/chapters.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/jb_docs_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/list_and_nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/numbered_chapters.yml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/numbered_depth.yml
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/numbered_depth_parts_subset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/numbered_parts.yml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/numbered_parts_subset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/parts.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/simple_dict.yml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/simple_list.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.824928 sphinx_external_toc_strict-1.1.3/tests/_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/basic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/basic_compressed.yml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/caption_not_entries.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/exclude_missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/glob.yml
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/glob_md.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/tableofcontents.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.824928 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/contains_toctree.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/file_not_in_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/multiple_tableofcontents.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/no_glob_match.yml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/tableofcontents_no_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.824928 sphinx_external_toc_strict-1.1.3/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_cli/test_create_toc.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_filename_suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.828928 sphinx_external_toc_strict-1.1.3/tests/test_parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_pep518_read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.828928 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_basic_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_basic_compressed_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_caption_not_entries_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_glob_md_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_tableofcontents_.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.832928 sphinx_external_toc_strict-1.1.3/tests/test_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_create_site_map_from_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_basic_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_chapters_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_list_and_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_numbered_chapters_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_numbered_depth_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_numbered_depth_parts_subset_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_numbered_parts_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_numbered_parts_subset_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_parts_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_simple_dict_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_simple_list_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_version_semantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.980598 sphinx_external_toc_strict-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.928598 sphinx_external_toc_strict-1.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.932597 sphinx_external_toc_strict-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/kit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/python-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/quality.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/test-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.github/workflows/testsuite.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31604 2024-04-19 03:58:20.980598 sphinx_external_toc_strict-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/asset-gesture-like-thumbs-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/asset-table-of-contents.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/credit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/sphinx-external-toc-strict-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/sphinx-external-toc-strict-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   147326 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/toc-graphic.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_static/toc_tree.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/compat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/constrants.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/filename_suffix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/parsing_shared.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/parsing_strictyaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/pep518_read.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/tools_strictyaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/code/version_semantic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/example/globfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/example/globfolder/page1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/example/globfolder/page2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/example/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.936597 sphinx_external_toc_strict-1.1.4/docs/example/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/example/subfolder/page.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-black.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-docutils-source.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1111839 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-sphinx-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-strictyaml-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-strictyaml-source.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/objects-toc-strict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/requirements.pip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.940598 sphinx_external_toc_strict-1.1.4/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/user_guide/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/user_guide/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/user_guide/regressions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/user_guide/sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/docs/user_guide/why.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/howto.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17383 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/igor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.940598 sphinx_external_toc_strict-1.1.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/dev.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/kit.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/kit.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/manage.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/manage.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/mypy.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/pins.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/pip-tools.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/pip.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/prod.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/prod.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/requirements/tox.pip
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:58:20.980598 sphinx_external_toc_strict-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.928598 sphinx_external_toc_strict-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.944598 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/filename_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/filename_suffix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_shared.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_strictyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/pep518_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/pep518_read.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19183 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/tools_strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/tools_strictyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/version_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/version_semantic.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.960598 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31604 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 03:58:20.000000 sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.948598 sphinx_external_toc_strict-1.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.948598 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/bad_option_value.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/bad_url.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/doc_multiple_times.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/doc_validation_fail.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/empty_items.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/empty_subtrees.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/entry_not_a_mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/entry_unknown_link_type.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/file_and_glob_present.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/item_then_subtrees_key.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/items_in_glob.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/items_in_url.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/list.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/no_root.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/subtree_with_no_items.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/unknown_keys.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/unknown_keys_nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_bad_toc_files/unknown_usecase.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.952597 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/chapters.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/jb_docs_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/list_and_nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/numbered_chapters.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/numbered_depth.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/numbered_depth_parts_subset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/numbered_parts.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/numbered_parts_subset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/parts.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/simple_dict.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/simple_list.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.952597 sphinx_external_toc_strict-1.1.4/tests/_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/basic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/basic_compressed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/caption_not_entries.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/exclude_missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/glob.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/glob_md.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_toc_files/tableofcontents.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.952597 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/contains_toctree.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/file_not_in_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/multiple_tableofcontents.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/no_glob_match.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/_warning_toc_files/tableofcontents_no_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.952597 sphinx_external_toc_strict-1.1.4/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_cli/test_create_toc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_filename_suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.956598 sphinx_external_toc_strict-1.1.4/tests/test_parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_pep518_read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.956598 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_basic_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_basic_compressed_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_caption_not_entries_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_glob_md_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_tableofcontents_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:58:20.960598 sphinx_external_toc_strict-1.1.4/tests/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_create_site_map_from_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_basic_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_file_to_sitemap_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_chapters_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_list_and_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_numbered_chapters_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_numbered_depth_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_numbered_depth_parts_subset_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_numbered_parts_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_numbered_parts_subset_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_parts_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_simple_dict_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_simple_list_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tests/test_version_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-19 03:58:09.000000 sphinx_external_toc_strict-1.1.4/tox.ini
```

### Comparing `sphinx_external_toc_strict-1.1.3/.github/workflows/codeql-analysis.yml` & `sphinx_external_toc_strict-1.1.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/.github/workflows/dependency-review.yml` & `sphinx_external_toc_strict-1.1.4/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/.github/workflows/kit.yml` & `sphinx_external_toc_strict-1.1.4/.github/workflows/kit.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/.github/workflows/python-nightly.yml` & `sphinx_external_toc_strict-1.1.4/.github/workflows/python-nightly.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/.github/workflows/quality.yml` & `sphinx_external_toc_strict-1.1.4/.github/workflows/quality.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/.github/workflows/release.yml` & `sphinx_external_toc_strict-1.1.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/.github/workflows/test-coverage.yml` & `sphinx_external_toc_strict-1.1.4/.github/workflows/test-coverage.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/.github/workflows/testsuite.yml` & `sphinx_external_toc_strict-1.1.4/.github/workflows/testsuite.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/.gitignore` & `sphinx_external_toc_strict-1.1.4/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -130,7 +130,8 @@
 
 .vscode/
 ~$*
 
 # Removed from project
 retired/
 src/sphinx_external_toc_strict/_version.py
+docs/*.inv
```

### Comparing `sphinx_external_toc_strict-1.1.3/.pre-commit-config.yaml` & `sphinx_external_toc_strict-1.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/CHANGELOG.md` & `sphinx_external_toc_strict-1.1.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/CHANGES.rst` & `sphinx_external_toc_strict-1.1.4/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,32 @@
    1. Dropped support for hidden document files
 
    Commit items for NEXT VERSION
    ..............................
 
 .. scriv-start-here
 
+.. _changes_1-1-4:
+
+Version 1.1.4 — 2024-04-19
+--------------------------
+
+- ci(.readthedocs.yml): py311 --> py39, do not build pdf, and notes
+- docs: defend assertions, links, in comparison table
+- fix: sphinx conf option master_doc index --> intro
+- docs: in comparison yaml dependency choice why and why not links
+- ci(.gitignore): eventhough pre-commit remove, ignore docs/*.inv
+- docs: advice on ramification of incorrectly set master_doc value
+- docs: add note sphinx extension sphinx-multitoc-numbering not working
+- docs: add logo files sphinx-external-toc-strict-logo.*
+- docs(credit.txt): document static asset authors and license
+- docs(_toc.yml): remove unnecessary captions. Rearrange ToC order
+- docs(user_guide/api.rst): in example fix python code
+- docs(regressions.rst): add  known regressions page, a markdown file
+
 .. _changes_1-1-3:
 
 Version 1.1.3 — 2024-04-18
 --------------------------
 
 - ci(.readthedocs.yml): python.install.requirements list rather than dict
 - style(pyproject.toml): configure project.urls
```

### Comparing `sphinx_external_toc_strict-1.1.3/CONTRIBUTING.md` & `sphinx_external_toc_strict-1.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/LICENSE` & `sphinx_external_toc_strict-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/Makefile` & `sphinx_external_toc_strict-1.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/NOTICE.txt` & `sphinx_external_toc_strict-1.1.4/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/PKG-INFO` & `sphinx_external_toc_strict-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-external-toc-strict
-Version: 1.1.3
+Version: 1.1.4
 Summary: A sphinx extension that allows the site-map to be defined in a single YAML file.
 Author-email: Dave Faulkmore <faulkmore@protonmail.com>
 License: MIT License
         
         Copyright (c) 2021 Executable Books
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Project-URL: Source code, https://github.com/msftcangoblowm/sphinx-external-toc-strict
 Project-URL: Issue tracker, https://github.com/msftcangoblowm/sphinx-external-toc-strict/issues
 Project-URL: Chat, https://mastodon.social/@msftcangoblowme
 Keywords: sphinx,extension,toc,strictyaml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -288,18 +288,19 @@
 
 sphinx-external-toc-strict is a fork of sphinx-external-toc
 
 .. csv-table:: Comparison
    :header: "Matric", "TOC", "TOC-Strict"
    :widths: auto
 
-   "yaml package", "pyyaml / yaml", "strictyaml / ruemel.yaml"
+   "yaml package", `pyyaml / yaml <https://hitchdev.com/strictyaml/why-not/>`_, `strictyaml / ruemel.yaml <https://hitchdev.com/strictyaml/why/>`_
    ".hidden.files.rst", "Yes", "No"
+   "docs theme", `sphinx-book-theme <https://sphinx-book-theme.readthedocs.io/en/latest>`_, `alabaster <https://alabaster.readthedocs.io/en/latest/>`_
    "markdown support", "Yes", "Yes"
-   "both", "No", "Yes, root doc must be ``index.rst``"
+   "both", `No <https://github.com/executablebooks/sphinx-external-toc/tree/main#development-notes>`_, "Yes, root doc must be ``index.rst``"
    "dump yaml", "use yaml.dump", "[package].parsing_strictyaml.dump_yaml"
    "static type checking", "patchy", "Yes (99%)"
    "coverage", "patchy", "maximium"
    "in-code manual", "No", "Yes"
 
 The core API should be compatible. To avoid confusion, on the command line, rather than ``sphinx-etoc``, use ``sphinx-etoc-strict``
```

### Comparing `sphinx_external_toc_strict-1.1.3/README.rst` & `sphinx_external_toc_strict-1.1.4/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -39,18 +39,19 @@
 
 sphinx-external-toc-strict is a fork of sphinx-external-toc
 
 .. csv-table:: Comparison
    :header: "Matric", "TOC", "TOC-Strict"
    :widths: auto
 
-   "yaml package", "pyyaml / yaml", "strictyaml / ruemel.yaml"
+   "yaml package", `pyyaml / yaml <https://hitchdev.com/strictyaml/why-not/>`_, `strictyaml / ruemel.yaml <https://hitchdev.com/strictyaml/why/>`_
    ".hidden.files.rst", "Yes", "No"
+   "docs theme", `sphinx-book-theme <https://sphinx-book-theme.readthedocs.io/en/latest>`_, `alabaster <https://alabaster.readthedocs.io/en/latest/>`_
    "markdown support", "Yes", "Yes"
-   "both", "No", "Yes, root doc must be ``index.rst``"
+   "both", `No <https://github.com/executablebooks/sphinx-external-toc/tree/main#development-notes>`_, "Yes, root doc must be ``index.rst``"
    "dump yaml", "use yaml.dump", "[package].parsing_strictyaml.dump_yaml"
    "static type checking", "patchy", "Yes (99%)"
    "coverage", "patchy", "maximium"
    "in-code manual", "No", "Yes"
 
 The core API should be compatible. To avoid confusion, on the command line, rather than ``sphinx-etoc``, use ``sphinx-etoc-strict``
```

### Comparing `sphinx_external_toc_strict-1.1.3/docs/Makefile` & `sphinx_external_toc_strict-1.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/docs/_static/toc-graphic.png` & `sphinx_external_toc_strict-1.1.4/docs/_static/toc-graphic.png`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/docs/_static/toc_tree.pptx` & `sphinx_external_toc_strict-1.1.4/docs/_static/toc_tree.pptx`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/docs/_toc.yml` & `sphinx_external_toc_strict-1.1.4/docs/_toc.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 root: intro
 subtrees:
 - caption: User Guide
-  numbered: true
-  entries:
-  - file: user_guide/why
-  - file: user_guide/sphinx
-  - file: user_guide/cli
-  - file: user_guide/api
-- caption: Example
-  entries:
-  - file: example/index
-    entries:
-    - file: example/subfolder/page
-    - glob: example/globfolder/*
-- caption: Code manual
   entries:
+    - file: user_guide/why
+    - file: user_guide/sphinx
+    - file: user_guide/cli
+    - file: user_guide/api
+    - file: user_guide/regressions.md
+- entries:
   - file: code/index
     entries:
     - glob: code/*
+- entries:
+  - file: example/index
+    entries:
+      - file: example/subfolder/page
+      - glob: example/globfolder/*
 - caption: Links
   entries:
   - title: GitHub Repository
     url: https://github.com/executablebooks/sphinx-external-toc
 meta:
   exclude_missing: true
   regress: intro
```

### Comparing `sphinx_external_toc_strict-1.1.3/docs/code/cli.rst` & `sphinx_external_toc_strict-1.1.4/docs/code/cli.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/docs/conf.py` & `sphinx_external_toc_strict-1.1.4/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 
 # Original author Chris Sewell <chrisj_sewell@hotmail.com>
 # copyright = "2021, Executable Book Project"
 
 # @@@ editable
 copyright = "2023–2024, Dave Faulkmore"
 # The short X.Y.Z version.
-version = "1.1.3"
+version = "1.1.4"
 # The full version, including alpha/beta/rc tags.
-release = "1.1.3"
+release = "1.1.4"
 # The date of release, in "monthname day, year" format.
-release_date = "April 18, 2024"
+release_date = "April 19, 2024"
 # @@@ end
 
 v = parse(release)
 version_short = f"{v.major}.{v.minor}"
 # version_xyz = f"{v.major}.{v.minor}.{v.micro}"
 version_xyz = version
 project = f"{proj_project} {version}"
@@ -60,25 +60,25 @@
     release=release, slug=slug
 )
 
 html_theme_options = {
     "description": proj_description,
     "show_relbars": True,
     "logo_name": False,
-    "logo": "logging-strict-logo.svg",
+    "logo": "sphinx-external-toc-strict-logo.svg",
     "show_powered_by": False,
 }
 
 latex_documents = [
     (
         proj_master_doc,
         f"{slug}.tex",
         f"{proj_project} Documentation",
         proj_authors,
-        "manual",
+        "manual",  # manual, howto, jreport (Japanese)
     )
 ]
 man_pages = [
     (
         proj_master_doc,
         slug,
         f"{proj_project} Documentation",
```

### Comparing `sphinx_external_toc_strict-1.1.3/docs/intro.rst` & `sphinx_external_toc_strict-1.1.4/docs/intro.rst`

 * *Files 8% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 
 sphinx-external-toc-strict is a fork of sphinx-external-toc
 
 .. csv-table:: Comparison
    :header: "Matric", "TOC", "TOC-Strict"
    :widths: auto
 
-   "yaml package", "pyyaml / yaml", "strictyaml / ruemel.yaml"
+   "yaml package", `pyyaml / yaml <https://hitchdev.com/strictyaml/why-not/>`_, `strictyaml / ruemel.yaml <https://hitchdev.com/strictyaml/why/>`_
    ".hidden.files.rst", "Yes", "No"
+   "docs theme", `sphinx-book-theme <https://sphinx-book-theme.readthedocs.io/en/latest>`_, `alabaster <https://alabaster.readthedocs.io/en/latest/>`_
    "markdown support", "Yes", "Yes"
-   "both", "No", "Yes, root doc must be ``index.rst``"
+   "both", `No <https://github.com/executablebooks/sphinx-external-toc/tree/main#development-notes>`_, "Yes, root doc must be ``index.rst``"
    "dump yaml", "use yaml.dump", :py:func:`parsing_strictyaml.dump_yaml <sphinx_external_toc_strict.parsing_strictyaml.dump_yaml>`
    "static type checking", "patchy", "Yes (99%)"
    "coverage", "patchy", "maximium"
    "in-code manual", "No", "Yes"
 
 The core APIs should be compatible. To avoid confusion, on the command
 line, rather than ``sphinx-etoc``, use ``sphinx-etoc-strict``
```

### Comparing `sphinx_external_toc_strict-1.1.3/docs/objects-python.txt` & `sphinx_external_toc_strict-1.1.4/docs/objects-python.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/docs/objects-sphinx-docs.txt` & `sphinx_external_toc_strict-1.1.4/docs/objects-sphinx-docs.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/docs/objects-strictyaml-docs.txt` & `sphinx_external_toc_strict-1.1.4/docs/objects-strictyaml-docs.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/docs/objects-strictyaml-source.txt` & `sphinx_external_toc_strict-1.1.4/docs/objects-strictyaml-source.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/docs/requirements.pip` & `sphinx_external_toc_strict-1.1.4/docs/requirements.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/docs/user_guide/api.rst` & `sphinx_external_toc_strict-1.1.4/docs/user_guide/api.rst`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 The ToC file is parsed to a ``SiteMap``, which is a
 :py:class:`~collections.abc.MutableMapping` subclass, with keys representing
 docnames mapping to a ``Document`` that stores information on the toctrees
 it should contain:
 
 .. code-block:: python
 
-    import yaml
-    from sphinx_external_toc.parsing import parse_toc_yaml
+    from sphinx_external_toc_strict.parsing_strictyaml import parse_toc_yaml, dump_yaml
 
     path = "path/to/_toc.yml"
     site_map = parse_toc_yaml(path)
-    yaml.dump(site_map.as_json())
+    dump_yaml(site_map)
 
 Would produce e.g.
 
 .. code-block:: yaml
 
    root: intro
    documents:
```

### Comparing `sphinx_external_toc_strict-1.1.3/docs/user_guide/cli.rst` & `sphinx_external_toc_strict-1.1.4/docs/user_guide/cli.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/docs/user_guide/sphinx.rst` & `sphinx_external_toc_strict-1.1.4/docs/user_guide/sphinx.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Configuration
 --------------
 
 Add to your ``conf.py``:
 
 .. code-block:: python
 
-    extensions = ["sphinx_external_toc"]
+    extensions = ["sphinx_external_toc_strict"]
     external_toc_path = "_toc.yml"  # optional, default: _toc.yml
     external_toc_exclude_missing = False  # optional, default: False
 
 Or to your ``pyproject.toml``
 
 .. code-block:: text
 
@@ -32,35 +32,39 @@
    ]
    myst_enable_extensions = ["colon_fence", "html_image"]
 
 Note the ``external_toc_path`` is always read as a Unix path, and can
 either be specified relative to the source directory (recommended) or
 as an absolute path.
 
-## Basic Structure
+Basic Structure
+-------------------
 
 A minimal ToC defines the top level `root` key, for a single root document file:
 
 .. code-block:: text
 
    root: intro
 
 The value of the ``root`` key will be a path to a file, in Unix format
 (folders split by ``/``), relative to the source directory, and can be
 with or without the file extension.
 
 .. note:: root file
 
-   To set the root file, other than index, the Sphinx conf key is
+   For a root file other than than index, modify the Sphinx conf key is
 
    `master_doc <https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-master_doc>`_
 
    This can be set in ``conf.py`` **or** ``pyproject.toml`` under section
    ``[tool.sphinx-pyproject]``
 
+   Incorrectly set master_doc value ramification,
+   :code:`make pdf` fails to build pdf
+
 Document files can then have a ``subtrees`` key - denoting a list of
 individual toctrees for that document - and in-turn each subtree should
 have a ``entries`` key - denoting a list of children links, that are
 one of:
 
 - ``file``: path to a single document file in Unix format,  with or
   without the file extension (as for `root`)
@@ -130,15 +134,15 @@
      - url: https://example.com
        title: Example URL Title
 
 ToC tree options
 -----------------
 
 Each subtree can be configured with a number of options (see also
-`sphinx `toctree` options <https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#directive-toctree>`_):
+`sphinx toctree options <https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#directive-toctree>`_):
 
 - ``caption`` (string): A title for the whole the subtree, e.g. shown
   above the subtree in ToCs
 
 - ``hidden`` (boolean): Whether to show the ToC within (inline of) the
   document (default ``False``).
   By default it is appended to the end of the document, but see also the
@@ -215,25 +219,27 @@
      numbered: True
      reversed: False
    entries:
    - file: doc1
      entries:
      - file: doc2
 
-.. warning:: ``numbered`` generally be used as a default
+.. note:: title numbering
 
-Since numbering cannot be changed by nested subtrees, and sphinx will
-log a warning.
+   By default, title numbering restarts for each subtree. For continuous numbering,
+   there is the unmaintained sphinx extension,
+   `sphinx-multitoc-numbering <https://github.com/executablebooks/sphinx-multitoc-numbering>`_.
 
-.. note:: title numbering
+   Tried it, didn't do the job! For now, ignore *numbered* option and
+   the non-functional sphinx extension
 
-   By default, title numbering restarts for each subtree.
-   If you want want this numbering to be continuous, check-out the
-   `sphinx-multitoc-numbering extension <https://github.com/executablebooks/sphinx-multitoc-numbering>`_.
+.. warning:: ``numbered`` not as a default
 
+   Since numbering cannot be changed by nested subtrees; sphinx will
+   log a warning
 
 Using different key-mappings
 -----------------------------
 
 For certain use-cases, it is helpful to map the ``subtrees``/``entries`` keys
 to mirror e.g. an output `LaTeX structure <https://www.overleaf.com/learn/latex/Sections_and_chapters>`_.
```

### Comparing `sphinx_external_toc_strict-1.1.3/docs/user_guide/why.rst` & `sphinx_external_toc_strict-1.1.4/docs/user_guide/why.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Why
 ====
 
-The package state is unmaintained and didn't want dependency, pyyaml.
+Primarily didn't want dependency, pyyaml. Also sphinx-external-toc package
+appears to be unmaintained.
 
 Removing pyyaml/yaml meant extensive changes. So even if the original
 author reemerges, didn't want to trouble him with a package he'll no
 longer recognize.
 
 A fork is necessary.
 
 Fixes
 
 - meta field values are scrutinized
-- fixed the issues preventing markdown support
-- unittest for mixed markdown and restructuredtext
+- rewrote file name handling issue affecting markdown support
 - static type checking
-- More extensive unittesting
+- Extensive unittest coverage
+- unittest for mixed markdown and restructuredtext
 - the dependencies
 - in-code documentation
 
 Enhancements
 
 - Hardened YAML parsing
 - Complete **code manual**
 - Makefile
 - Makefile for docs
 - semantic versioning
 - github actions
+- **mixed** markdown and ReStructuredText support
 
 Dependencies
 -------------
 
 Simplier toolchain
 ^^^^^^^^^^^^^^^^^^^
```

### Comparing `sphinx_external_toc_strict-1.1.3/howto.txt` & `sphinx_external_toc_strict-1.1.4/howto.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/igor.py` & `sphinx_external_toc_strict-1.1.4/igor.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/pyproject.toml` & `sphinx_external_toc_strict-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 keywords = ["sphinx","extension", "toc", "strictyaml"]
 readme = "README.rst"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -110,29 +110,29 @@
 [tool.sphinx-pyproject]
 language = "en"
 needs_sphinx = "1.7"
 templates_path = ["_templates",]
 html_static_path = ["_static",]
 # https://www.sphinx-doc.org/en/master/usage/markdown.html
 source_suffix = [".md", ".rst"]
-master_doc = "index"
+master_doc = "intro"
 pygments_style = "sphinx"
 html_theme = "alabaster"
 numfig = true
 autosectionlabel_prefix_document = true
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.todo",
     "sphinx.ext.doctest",
     "sphinx.ext.githubpages",
     "sphinx_paramlinks",
     "sphinx.ext.intersphinx",
     "sphinx.ext.extlinks",
-    "sphinx_external_toc_strict",  # circular?
+    "sphinx_external_toc_strict",
     "myst_parser",
 ]
 linkcheck_ignore = [
     "https://github.com/crdoconnor/strictyaml/blob/dfd93f9740ebd5e7150029bc3d89ea102bcddf00/strictyaml/representation.py#L48",
     "https://github.com/crdoconnor/strictyaml/blob/dfd93f9740ebd5e7150029bc3d89ea102bcddf00/strictyaml/representation.py#L114",
     "https://github.com/PyCQA/flake8/blob/fb9a02aaf77b56fcad4320971e7edca0cea93489/src/flake8/options/config.py#L56",
     "https://github.com/psf/black/blob/ea66d40dd7f1eaa20256e6fccaf6d7b853ccc541/src/black/files.py#L57",
```

### Comparing `sphinx_external_toc_strict-1.1.3/requirements/dev.pip` & `sphinx_external_toc_strict-1.1.4/requirements/dev.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/requirements/kit.in` & `sphinx_external_toc_strict-1.1.4/requirements/kit.in`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/requirements/kit.pip` & `sphinx_external_toc_strict-1.1.4/requirements/kit.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/requirements/manage.pip` & `sphinx_external_toc_strict-1.1.4/requirements/manage.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/requirements/pip-tools.pip` & `sphinx_external_toc_strict-1.1.4/requirements/pip-tools.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/requirements/prod.pip` & `sphinx_external_toc_strict-1.1.4/requirements/prod.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/requirements/tox.in` & `sphinx_external_toc_strict-1.1.4/requirements/tox.in`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/requirements/tox.pip` & `sphinx_external_toc_strict-1.1.4/requirements/tox.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/setup.py` & `sphinx_external_toc_strict-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/__init__.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/_compat.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/_compat.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/api.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/api.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/api.pyi` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/api.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/cli.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/constants.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/constants.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/constants.pyi` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/constants.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/events.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/events.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/events.pyi` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/events.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/filename_suffix.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/filename_suffix.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/filename_suffix.pyi` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/filename_suffix.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_shared.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_shared.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_shared.pyi` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_shared.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_strictyaml.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_strictyaml.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_strictyaml.pyi` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/parsing_strictyaml.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/pep518_read.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/pep518_read.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/pep518_read.pyi` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/pep518_read.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/tools_strictyaml.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/tools_strictyaml.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/tools_strictyaml.pyi` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/tools_strictyaml.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/version_semantic.py` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict/version_semantic.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/PKG-INFO` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-external-toc-strict
-Version: 1.1.3
+Version: 1.1.4
 Summary: A sphinx extension that allows the site-map to be defined in a single YAML file.
 Author-email: Dave Faulkmore <faulkmore@protonmail.com>
 License: MIT License
         
         Copyright (c) 2021 Executable Books
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Project-URL: Source code, https://github.com/msftcangoblowm/sphinx-external-toc-strict
 Project-URL: Issue tracker, https://github.com/msftcangoblowm/sphinx-external-toc-strict/issues
 Project-URL: Chat, https://mastodon.social/@msftcangoblowme
 Keywords: sphinx,extension,toc,strictyaml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -288,18 +288,19 @@
 
 sphinx-external-toc-strict is a fork of sphinx-external-toc
 
 .. csv-table:: Comparison
    :header: "Matric", "TOC", "TOC-Strict"
    :widths: auto
 
-   "yaml package", "pyyaml / yaml", "strictyaml / ruemel.yaml"
+   "yaml package", `pyyaml / yaml <https://hitchdev.com/strictyaml/why-not/>`_, `strictyaml / ruemel.yaml <https://hitchdev.com/strictyaml/why/>`_
    ".hidden.files.rst", "Yes", "No"
+   "docs theme", `sphinx-book-theme <https://sphinx-book-theme.readthedocs.io/en/latest>`_, `alabaster <https://alabaster.readthedocs.io/en/latest/>`_
    "markdown support", "Yes", "Yes"
-   "both", "No", "Yes, root doc must be ``index.rst``"
+   "both", `No <https://github.com/executablebooks/sphinx-external-toc/tree/main#development-notes>`_, "Yes, root doc must be ``index.rst``"
    "dump yaml", "use yaml.dump", "[package].parsing_strictyaml.dump_yaml"
    "static type checking", "patchy", "Yes (99%)"
    "coverage", "patchy", "maximium"
    "in-code manual", "No", "Yes"
 
 The core API should be compatible. To avoid confusion, on the command line, rather than ``sphinx-etoc``, use ``sphinx-etoc-strict``
```

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/SOURCES.txt` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 docs/objects-python.txt
 docs/objects-sphinx-docs.txt
 docs/objects-strictyaml-docs.txt
 docs/objects-strictyaml-source.txt
 docs/objects-toc-strict.txt
 docs/requirements.in
 docs/requirements.pip
+docs/_static/asset-gesture-like-thumbs-up.svg
+docs/_static/asset-table-of-contents.svg
+docs/_static/credit.txt
+docs/_static/sphinx-external-toc-strict-logo.png
+docs/_static/sphinx-external-toc-strict-logo.svg
 docs/_static/toc-graphic.png
 docs/_static/toc_tree.pptx
 docs/code/api.rst
 docs/code/cli.rst
 docs/code/compat.rst
 docs/code/constrants.rst
 docs/code/events.rst
@@ -53,14 +58,15 @@
 docs/code/version_semantic.rst
 docs/example/index.rst
 docs/example/globfolder/page1.rst
 docs/example/globfolder/page2.rst
 docs/example/subfolder/page.rst
 docs/user_guide/api.rst
 docs/user_guide/cli.rst
+docs/user_guide/regressions.md
 docs/user_guide/sphinx.rst
 docs/user_guide/why.rst
 requirements/dev.in
 requirements/dev.pip
 requirements/kit.in
 requirements/kit.pip
 requirements/manage.in
```

### Comparing `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/requires.txt` & `sphinx_external_toc_strict-1.1.4/src/sphinx_external_toc_strict.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/chapters.yml` & `sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/chapters.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/jb_docs_toc.yml` & `sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/jb_docs_toc.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/parts.yml` & `sphinx_external_toc_strict-1.1.4/tests/_jb_migrate_toc_files/parts.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/_toc_files/glob_md.yml` & `sphinx_external_toc_strict-1.1.4/tests/_toc_files/glob_md.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/conftest.py` & `sphinx_external_toc_strict-1.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_api.py` & `sphinx_external_toc_strict-1.1.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_cli/test_create_toc.txt` & `sphinx_external_toc_strict-1.1.4/tests/test_cli/test_create_toc.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_cli.py` & `sphinx_external_toc_strict-1.1.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_filename_suffix.py` & `sphinx_external_toc_strict-1.1.4/tests/test_filename_suffix.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_glob_md_.yml` & `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_create_toc_dict_glob_md_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_basic_.yml` & `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_basic_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml` & `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_glob_md_.yml` & `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_glob_md_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_nested_.yml` & `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_nested_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml` & `sphinx_external_toc_strict-1.1.4/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_parsing.py` & `sphinx_external_toc_strict-1.1.4/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_pep518_read.py` & `sphinx_external_toc_strict-1.1.4/tests/test_pep518_read.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_tableofcontents_.xml` & `sphinx_external_toc_strict-1.1.4/tests/test_sphinx/test_success_tableofcontents_.xml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_sphinx.py` & `sphinx_external_toc_strict-1.1.4/tests/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_tools/test_create_site_map_from_path.yml` & `sphinx_external_toc_strict-1.1.4/tests/test_tools/test_create_site_map_from_path.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_chapters_.yml` & `sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_chapters_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml` & `sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_parts_.yml` & `sphinx_external_toc_strict-1.1.4/tests/test_tools/test_migrate_jb_parts_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_tools.py` & `sphinx_external_toc_strict-1.1.4/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tests/test_version_semantic.py` & `sphinx_external_toc_strict-1.1.4/tests/test_version_semantic.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.3/tox.ini` & `sphinx_external_toc_strict-1.1.4/tox.ini`

 * *Files identical despite different names*

